# Banco Horizonte — Inventario de aplicaciones AS-IS

**Curso:** CD-03 · Arquitectura Bancaria basada en el estándar BIAN® · CPS Tech · Módulo 2
**Ámbito:** panorama aplicativo actual (línea base), su relación con procesos y actividades, y la evidencia de duplicación de datos, deuda técnica y obsolescencia.

> **[SUPUESTO — leer antes de usar]** El caso de negocio **no nombra ningún sistema**. Este inventario es una construcción didáctica, diseñada para que las patologías que el caso sí declara —H-02 datos dispersos, H-04 procesamiento nocturno, H-05 condiciones embebidas, H-07 reportes que no cuadran, H-08 integraciones frágiles, H-11 datos no explotables, H-12 cambio caro y riesgoso— **se puedan ver en el modelo** y no solo leer en una nota. No sustituye un levantamiento real.

---

## 1. Inventario de aplicaciones

| ID | Aplicación | Tipo | Tecnología | Año | Origen | Soporte | Deuda | Criticidad |
|---|---|---|---|:--:|---|---|:--:|:--:|
| **APP-01** | **SIGEB — Core Bancario** | Core | COBOL / CICS · mainframe | 1998 | A medida | ⛔ Sin soporte del fabricante | **Alta** | **Crítica** |
| **APP-02** | Módulo de Créditos | Core (submódulo) | COBOL · mainframe | 1998 | A medida | ⛔ Sin soporte | **Alta** | **Crítica** |
| **APP-03** | Motor de Scoring Crediticio | Analítica | Motor propietario · Windows Server | 2009 | Paquete | ⚠️ Soporte extendido | Media | Alta |
| **APP-04** | CRM Comercial | Front | Cliente-servidor · .NET / SQL Server | 2011 | Paquete | ⚠️ Soporte extendido | Media | Alta |
| **APP-05** | Portal de Vinculación (Onboarding) | Canal | Web Java · on-premise | 2016 | A medida | ✅ Soportado | Media | Alta |
| **APP-06** | Banca por Internet | Canal | Web Java · on-premise | 2014 | A medida | ⚠️ Soporte extendido | **Alta** | **Crítica** |
| **APP-07** | App Móvil | Canal | Híbrida (Cordova) | 2019 | A medida | ⚠️ Framework en desuso | **Alta** | **Crítica** |
| **APP-08** | Switch Transaccional | Middleware | Middleware propietario | 2007 | Paquete | ⚠️ Soporte extendido | Media | **Crítica** |
| **APP-09** | Plataforma de Agentes | Canal | Cliente-servidor + **batch nocturno** | 2012 | A medida | ⚠️ Soporte extendido | **Alta** | **Crítica** |
| **APP-10** | Pasarela de Pagos Inmediatos | Integración | Interfaz CCE / ISO 20022 | 2021 | A medida | ✅ Soportado | Baja | **Crítica** |
| **APP-11** | Contabilidad / ERP | Back office | Paquete ERP · Oracle | 2005 | Paquete | ⚠️ Versión sin soporte | **Alta** | **Crítica** |
| **APP-12** | **Reportería Regulatoria** | Back office | **MS Access + Excel + macros** | s/f | Ofimática | ⛔ No es una aplicación gobernada | **Muy alta** | **Crítica** |
| **APP-13** | Monitoreo PLAFT | Cumplimiento | Paquete · Windows Server | 2013 | Paquete | ⚠️ Soporte extendido | Media | Alta |
| **APP-14** | Datawarehouse | Analítica | ETL batch nocturno · Oracle | 2010 | A medida | ⚠️ Soporte extendido | **Alta** | Media |

**Resumen del parque:** 14 aplicaciones · antigüedad media **≈ 15 años** · **2 sin soporte** y **9 en soporte extendido** · **6 con deuda técnica alta o muy alta** · **7 críticas**.

---

## 2. Fichas de las aplicaciones que concentran el problema

### APP-01 · SIGEB — Core Bancario
**Qué hace.** Es el sistema central del banco: mantiene clientes, cuentas, depósitos, créditos y la contabilidad de origen. Todo lo demás orbita a su alrededor.
**Procesos que automatiza.** PN-01 (act. 5) · PN-02 (act. 8) · PN-03 (act. 2,3,4,6) · PN-04 (act. 2,5) · PN-05 (act. 7) · PN-07 (act. 4) · PN-09 (act. 4,5) · PN-10 (act. 1).
**Objetos de datos que gobierna.** BO-CLI · BO-CTA · BO-CRE · BO-CTR · BO-TRX · BO-PRD.
**Deuda técnica (alta).** Lógica de negocio y **condiciones de producto embebidas en el código** → causa directa de H-05. Programación en COBOL con escasez de personal que lo domine. Sin capa de servicios: la integración es por archivos y accesos directos a base de datos.
**Obsolescencia.** Plataforma mainframe sin soporte del fabricante desde hace años; cada cambio exige regresión completa → H-12.
**Trazabilidad.** H-05 · H-08 · H-11 · H-12 → O-11 → CA-08 → capacidad **H2.2 Plataformas y Core Bancario**.

### APP-12 · Reportería Regulatoria (Access + Excel)
**Qué hace.** Es donde realmente se arman los reportes regulatorios y buena parte del cierre: extracciones, tablas dinámicas, macros y consolidaciones a mano.
**Procesos que automatiza.** PN-08 (act. 7) · PN-09 (act. 7) · PN-10 (act. 3,4,7,8).
**Objetos de datos.** BO-REP · copias locales de BO-TRX y BO-PRD.
**Deuda técnica (muy alta).** No es una aplicación gobernada: sin control de versiones, sin trazabilidad de cambios, sin respaldo formal, con conocimiento concentrado en pocas personas. Es el **punto único de falla** del cumplimiento.
**Trazabilidad.** H-07 → O-07 → CA-06 → capacidades **H1.1 · H1.2 · E3.1**.
**Nota para clase.** Este es el ejemplo que mejor ilustra que «automatizado» no significa «gobernado». Un Excel crítico es deuda técnica, aunque nadie lo llame sistema.

### APP-09 · Plataforma de Agentes
**Qué hace.** Opera la red de corresponsales: captura la operación en el punto de atención y la transmite al core.
**Procesos que automatiza.** PN-05 (act. 1,2,4,5) · PN-11 (act. 4,6).
**Deuda técnica (alta).** **Cierre y transmisión por lotes nocturno** — no hay procesamiento en línea contra el core. Cada nuevo comercio requiere integración específica → H-08.
**Trazabilidad.** H-04 · H-08 → O-04 → CA-03 → capacidad **M6.2 Red de Corresponsalía**.

### APP-06 / APP-07 · Banca por Internet y App Móvil
**Qué hacen.** Exponen consultas y un conjunto **limitado** de operaciones.
**Deuda técnica (alta).** Construidas contra el core por integraciones punto a punto; cada operación nueva exige desarrollo en el canal **y** en el core. La app usa un framework híbrido en desuso.
**Trazabilidad.** H-03 · H-08 · H-10 → O-03 → CA-02 → capacidad **M6.1 Canales Digitales**.

---

## 3. Matriz Aplicación × Proceso

| Aplicación | PN-01 | PN-02 | PN-03 | PN-04 | PN-05 | PN-06 | PN-07 | PN-08 | PN-09 | PN-10 | PN-11 |
|---|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
| APP-01 Core SIGEB | ● | ● | ● | ● | ● | | ● | ● | ● | ● | |
| APP-02 Créditos | | ● | | | | | ● | | ● | | |
| APP-03 Scoring | | ● | | | | | | | | | |
| APP-04 CRM | ● | | | | | | ● | ● | | | ● |
| APP-05 Onboarding | ● | ● | ● | | | | | | | | |
| APP-06 Banca Internet | ● | ● | | ● | | | | ● | ● | | |
| APP-07 App Móvil | ● | | | ● | | | | | ● | | |
| APP-08 Switch | | | ● | | | | | | | | |
| APP-09 Agentes | | | | | ● | | | | | | ● |
| APP-10 Pagos Inmediatos | | | | ● | | | | | | | |
| APP-11 Contabilidad/ERP | | ● | ● | ● | ● | ● | ● | | | ● | |
| APP-12 Reportería | | | | | | | | ● | ● | ● | |
| APP-13 PLAFT | ● | | | ● | | | | | | ● | ● |
| APP-14 Datawarehouse | | | | | | | | | | ● | |

**Lectura.** El core interviene en **9 de 11 procesos**: es el cuello de botella estructural y explica por qué H-12 («cambiar la tecnología es caro y riesgoso») bloquea toda la estrategia. Ninguna iniciativa avanza sin tocarlo.

---

## 4. Matriz Objeto de negocio × Aplicación — la evidencia de H-02

Se marca **M** cuando la aplicación **mantiene** su propia copia del objeto (es dueña de un registro) y **L** cuando solo lo **lee**.

| Objeto | APP-01 | APP-02 | APP-03 | APP-04 | APP-05 | APP-06 | APP-07 | APP-09 | APP-11 | APP-12 | APP-13 | APP-14 | **Dueños** |
|---|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
| **BO-CLI Cliente** | **M** | | L | **M** | **M** | L | L | L | | | **M** | **M** | **5** |
| **BO-CTA Cuenta** | **M** | | | L | | L | L | **M** | L | | | **M** | **3** |
| **BO-CRE Crédito** | **M** | **M** | L | L | | L | | | L | | | **M** | **3** |
| BO-CTR Contrato | **M** | **M** | | | L | | | | | | | | 2 |
| BO-ORD Orden de pago | **M** | | | | | **M** | **M** | **M** | | | L | | **4** |
| **BO-TRX Transacción** | **M** | | | | | | | **M** | **M** | **M** | L | **M** | **5** |
| BO-ASI Asiento contable | **M** | | | | | | | | **M** | **M** | | L | **3** |
| **BO-PRD Producto** | **M** | **M** | | L | | L | L | | | **M** | | | **3** |
| BO-REP Reporte regulatorio | | | | | | | | | L | **M** | **M** | L | 2 |

### Diagnóstico de duplicación

| Objeto | Dueños | Consecuencia observada en los procesos |
|---|:--:|---|
| **Cliente** | **5** | PN-01 act. 6 (replicación manual al CRM) · PN-08 act. 3 (el asesor busca en tres sistemas). **Es H-02 en estado puro.** |
| **Transacción** | **5** | PN-10 act. 2–4: la contabilidad se reconstruye desde cinco fuentes que no cuadran. **Es H-07.** |
| **Orden de pago** | **4** | Cada canal mantiene su propio registro antes de llegar al core. |
| **Producto** | **3** | El tarifario vive en Excel (APP-12) además del core → desalineación de condiciones (H-05). |

**Ninguno de los nueve objetos tiene un único dueño.** Ese es, en una sola frase, el argumento arquitectónico de la oportunidad O-02 y de la capacidad **H2.4 Gestión de Datos e Información (BOM)** — y es exactamente el problema que BIAN resuelve asignando a cada Service Domain la propiedad única de su Control Record.

---

## 5. Integraciones — la evidencia de H-08

**Patrón dominante: punto a punto, sin bus ni capa de servicios.**

| Origen → Destino | Mecanismo | Frecuencia | Observación |
|---|---|---|---|
| APP-05 → APP-01 | Servicio propietario | En línea | — |
| APP-01 → APP-04 | **Archivo plano** | Diario | Origen de la replicación manual (PN-01 act. 6) |
| APP-06 / APP-07 → APP-01 | Servicio propietario | En línea | Un desarrollo por operación expuesta |
| APP-09 → APP-01 | **Archivo por lotes** | **Nocturna** | Causa de H-04 |
| APP-08 → APP-01 | Middleware propietario | En línea | — |
| APP-10 → APP-01 | ISO 20022 | En línea | Única integración con estándar de industria |
| APP-01 / APP-09 / APP-08 → APP-11 | **Archivo plano** | Diario | Contabilidad alimentada por archivos |
| APP-01 / APP-11 / APP-09 → APP-14 | **ETL batch** | Nocturna | — |
| APP-14 / APP-11 → APP-12 | **Extracción manual** | Por período | **Sin integración: lo hace una persona** |
| APP-01 → APP-13 | Archivo plano | Diario | — |

**Conteo:** 13 interfaces, de las cuales **6 son por archivo o lote** y **1 es manual**. Solo **una** (APP-10) usa un estándar de industria. Ese perfil es el que hace que «cada nuevo canal o alianza exija integraciones costosas y frágiles».

---

## 6. Clasificación de deuda técnica y obsolescencia

### Escala de obsolescencia (ciclo de vida)

| Estado | Aplicaciones |
|---|---|
| ✅ **Soportado** | APP-05 · APP-10 |
| ⚠️ **Soporte extendido / tecnología en desuso** | APP-03 · APP-04 · APP-06 · APP-07 · APP-08 · APP-09 · APP-11 · APP-13 · APP-14 |
| ⛔ **Sin soporte / no gobernado** | APP-01 · APP-02 · APP-12 |

### Escala de deuda técnica

| Nivel | Aplicaciones | Razón declarada |
|---|---|---|
| **Muy alta** | APP-12 | Ofimática crítica sin gobierno ni trazabilidad |
| **Alta** | APP-01 · APP-02 · APP-06 · APP-07 · APP-09 · APP-11 · APP-14 | Lógica embebida, integración punto a punto, procesamiento por lotes, frameworks en desuso |
| **Media** | APP-03 · APP-04 · APP-08 · APP-13 | Versiones atrasadas, acoplamiento moderado |
| **Baja** | APP-05 · APP-10 | Construidas con criterios actuales |

### Prioridad de intervención (deuda × criticidad)

1. **APP-01 / APP-02 — Core.** Deuda alta + criticidad crítica + interviene en 9 procesos. Es CA-08.
2. **APP-12 — Reportería.** Deuda muy alta + riesgo regulatorio directo. Es CA-06 / O-07.
3. **APP-09 — Agentes.** Deuda alta + causa única de H-04. Es CA-03.
4. **APP-06 / APP-07 — Canales.** Deuda alta + es la brecha central del caso. Es CA-02.

---

## 7. Cierre de la cadena de trazabilidad

Con este inventario queda completa la cadena que veníamos construyendo:

```
Meta  ->  Resultado esperado  ->  Capacidad L1  ->  Curso de acción  ->  Recurso
                                       ▲
                                       │ composición (la L2 compone a la L1)
                                  Capacidad L2  ◄── sirve ──  Service Domain (M3-M4)
                                       ▲                            ▲
                                       │ realiza                    │ usa
                                    Proceso ── composición ──►  Actividad
                                                                    ▲
                                                                    │ sirve
                                                          Servicio de aplicación
                                                                    │
                                                             Aplicación AS-IS
```

**Las cinco reglas del metamodelo:** el Service Domain **sirve** a la capacidad L2 · la capacidad L2 **compone** a la L1 · el proceso **realiza** una capacidad (L1 o L2) · el proceso **se compone** de actividades · la actividad **usa** un Service Domain.

Cualquier elemento del modelo puede auditarse ahora en ambos sentidos: desde una meta hasta el sistema que hoy la sostiene, y desde un sistema obsoleto hasta la meta de negocio que está poniendo en riesgo.

---

*Caso ficticio con fines didácticos. Repositorio: github.com/elwolfy/capstone-ea-bian-banco-horizonte*
