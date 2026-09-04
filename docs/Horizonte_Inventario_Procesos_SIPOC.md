# Banco Horizonte — Inventario de procesos y SIPOC extendido (AS-IS)

**Curso:** CD-03 · Arquitectura Bancaria basada en el estándar BIAN® · CPS Tech · Módulo 2
**Ámbito:** línea base (AS-IS) de procesos, actividades y su automatización.

> **Origen de la información.** Los procesos **PN-01 a PN-08** provienen del caso (secciones 6 y 7); **PN-09, PN-10 y PN-11** se derivan de hallazgos y oportunidades declarados (H-05/O-05, H-07/O-07, H-08/O-08). **Las actividades, roles, entradas y salidas NO están en el caso**: son supuestos didácticos consistentes con los hallazgos H-01…H-12, marcados **[SUPUESTO]**. Deben validarse con el negocio antes de tomarse como levantamiento real.

---

## 1. Metamodelo de trazabilidad

La cadena que sostiene todo el ejercicio, alineada al metamodelo BIAN (capas de estrategia / arquitectura de negocio):

```
Service Domain  --sirve-->  Capacidad L2  --sirve-->  Actividad
                                                          |
                                                    (composición)
                                                          v
                                                       Proceso  --realiza-->  Capacidad L1
```

- El **proceso realiza** la capacidad de negocio (L1).
- La **actividad es servida** por la capacidad granular (L2).
- La **capacidad L2 es servida** por los **Service Domains** de BIAN — la capa de arquitectura de negocio sirve a la capa de estrategia, conforme al metamodelo BIAN v14.
- **En el Módulo 2** se modela hasta la capacidad L2. **En los Módulos 3–4** se conectan los Service Domains a esas capacidades L2 y el proceso se re-expresa como orquestación (Business Scenario BIAN).

**Aplicaciones:** el servicio de aplicación **sirve** a la actividad. Una actividad **sin** servicio de aplicación es, por definición en este modelo, **trabajo manual**.

---

## 2. Inventario de procesos

| ID | Proceso | Tipo | Origen | Capacidad L1 | Estado | Act. | Manuales |
|---|---|---|---|---|---|:--:|:--:|
| **PN-01** | Vinculación de clientes (onboarding) | Misional | [CASO §7] | M1 · M6 | AS-IS | 8 | 2 |
| **PN-02** | Originación y otorgamiento de crédito | Misional | [CASO §7] | M3 · M2 · M5 | AS-IS | 9 | 2 |
| **PN-03** | Apertura y operación de cuentas de ahorro | Misional | [CASO §7] | M4 · M2 · M5 | AS-IS | 7 | 0 |
| **PN-04** | Ejecución de pagos y transferencias | Misional | [CASO §7] | M5 · H1 | AS-IS | 7 | 0 |
| **PN-05** | Operación en agente / corresponsal | Misional | [CASO §7] | M6 · M5 · H1 | AS-IS | 8 | 2 |
| **PN-06** | Pago y cobro en efectivo por referencia | Misional | [CASO §7] | M5 · M6 · E1 | **TO-BE** | 7 | 2 |
| **PN-07** | Administración y cobranza del crédito | Misional | [CASO §6] | M3 · E2 | AS-IS | 6 | 1 |
| **PN-08** | Atención de consultas y reclamos | Misional | [CASO §4,§6] | M1 · M6 | AS-IS | 7 | 2 |
| **PN-09** | Lanzamiento y modificación de productos | Gestión | [DERIVADO H-05] | M2 · E4 | AS-IS | 7 | 3 |
| **PN-10** | Cierre contable y reportería regulatoria | Soporte | [DERIVADO H-07] | H1 · E3 | AS-IS | 9 | 6 |
| **PN-11** | Incorporación de comercios y agentes | Soporte | [DERIVADO H-08] | E1 · M6 | AS-IS | 6 | 3 |

**Totales:** 11 procesos · 81 actividades · **23 manuales (28 %)**.

**Lectura:** la carga manual se concentra en **PN-10 (6 de 9 actividades manuales)** — el cierre contable y la reportería regulatoria —, seguido de **PN-09** y **PN-11**. Los procesos transaccionales de cara al cliente (PN-03, PN-04) están automatizados; el problema no es la transacción, es **todo lo que hay alrededor**.

### Roles y actores

| Código | Rol / Actor | Tipo |
|---|---|---|
| RL-CLI | Cliente | Business Actor (externo) |
| RL-COM | Comercio aliado / Agente corresponsal | Business Actor (externo) |
| RL-REG | Regulador (SBS · UIF · BCRP) | Business Actor (externo) |
| RL-ASE | Asesor de agencia | Business Role |
| RL-ANC | Analista de crédito | Business Role |
| RL-OFC | Oficial de cumplimiento | Business Role |
| RL-CON | Analista contable | Business Role |
| RL-OPE | Analista de operaciones (back office) | Business Role |
| RL-PRO | Gestor de producto | Business Role |
| RL-SOP | Asesor de contact center | Business Role |
| RL-TI | Analista de TI | Business Role |

### Objetos de negocio

BO-CLI Cliente · BO-CTA Cuenta · BO-CRE Crédito (arreglo) · BO-CTR Contrato · BO-ORD Orden de pago · BO-TRX Transacción · BO-ASI Asiento contable · BO-PRD Producto · BO-REP Reporte regulatorio

---

## 3. SIPOC extendido por proceso

**Leyenda de tipo de actividad:** ⚙️ automatizada · 🖐️ **manual** · ◐ híbrida

---

### PN-01 · Vinculación de clientes (onboarding)

| SIPOC | Contenido |
|---|---|
| **S — Proveedor** | Cliente; entidad de identidad (validación documental); UIF (listas restrictivas) |
| **I — Entrada** | Solicitud de vinculación; documento de identidad; datos de contacto y perfil |
| **O — Salida** | Cliente registrado y habilitado para operar; expediente de vinculación |
| **C — Cliente** | Cliente final; áreas comerciales; cumplimiento |
| **Disparador** | Evento: «Solicitud de vinculación recibida» |

| # | Actividad | Tipo | Rol | Sistema | Capacidad L2 | Dolor |
|---|---|:--:|---|---|---|---|
| 1 | Recepción de la solicitud | ◐ | RL-ASE | APP-05 / agencia | M1.1 Registro y Onboarding | H-01 |
| 2 | Captura de datos y documentos | ◐ | RL-ASE | APP-05 | M1.1 Registro y Onboarding | H-01 · H-02 |
| 3 | Validación de identidad | ◐ | RL-ASE | APP-05 | M1.2 Identidad y Autenticación | H-01 |
| 4 | Verificación en listas y perfil PLAFT | ⚙️ | RL-OFC | APP-13 | E3.2 PLAFT | — |
| 5 | Registro del cliente en el core | ⚙️ | RL-ASE | APP-01 | M1.1 Registro y Onboarding | H-02 |
| 6 | **Replicación del cliente al CRM** | 🖐️ | RL-OPE | APP-04 | M1.3 CRM | **H-02** |
| 7 | Habilitación de credenciales y canales | ◐ | RL-ASE | APP-06 · APP-07 | M1.2 Identidad y Autenticación | H-03 |
| 8 | **Entrega de bienvenida y activación** | 🖐️ | RL-ASE | — | M1.4 Experiencia y Servicio | H-01 |

**Controles:** KYC (SBS) · PLAFT (UIF, Ley 27693) · Protección de datos (Ley 29733).
**Observación:** la actividad 6 es la evidencia operativa de H-02 — el cliente se crea dos veces, en el core y en el CRM, con un paso manual entre ambos.

---

### PN-02 · Originación y otorgamiento de crédito

| SIPOC | Contenido |
|---|---|
| **S — Proveedor** | Cliente; central de riesgos; áreas de riesgo y producto |
| **I — Entrada** | Solicitud de crédito; documentación de ingresos; historial crediticio |
| **O — Salida** | Crédito aprobado y desembolsado; contrato formalizado; asiento contable |
| **C — Cliente** | Cliente final; riesgos; contabilidad |
| **Disparador** | Evento: «Solicitud de crédito recibida» |

| # | Actividad | Tipo | Rol | Sistema | Capacidad L2 | Dolor |
|---|---|:--:|---|---|---|---|
| 1 | Recepción de la solicitud de crédito | ◐ | RL-ASE | APP-05 · APP-06 | M3.1 Originación | H-01 · H-03 |
| 2 | **Conformación del expediente** | 🖐️ | RL-ASE | — | M3.1 Originación | **H-01 · H-02** |
| 3 | Consulta a central de riesgos | ⚙️ | RL-ANC | APP-03 | E2.1 Riesgo de Crédito | — |
| 4 | Evaluación de capacidad de pago (scoring) | ◐ | RL-ANC | APP-03 | M3.2 Evaluación y Decisión | **H-06** |
| 5 | **Decisión y aprobación (comité si excede autonomía)** | 🖐️ | RL-ANC | — | M3.2 Evaluación y Decisión | **H-06** |
| 6 | Definición de condiciones (monto, plazo, tasa) | ◐ | RL-PRO | APP-02 | M2.1 Diseño y Configuración | H-05 |
| 7 | Formalización del contrato | ◐ | RL-ASE | APP-02 | M2.2 Acuerdos y Contratos | — |
| 8 | Desembolso | ⚙️ | RL-OPE | APP-01 | M5.1 Ejecución de Pagos | — |
| 9 | Registro contable del desembolso | ⚙️ | — | APP-11 | H1.1 Contabilidad (Ledger) | — |

**Controles:** evaluación crediticia (SBS) · Basilea III · transparencia de tasas (SBS/Indecopi).
**Observación:** las actividades 2, 4 y 5 concentran el dolor H-06; el tiempo no se pierde en el sistema sino en el expediente y en la decisión.

---

### PN-03 · Apertura y operación de cuentas de ahorro

| SIPOC | Contenido |
|---|---|
| **S — Proveedor** | Cliente; gestión de producto |
| **I — Entrada** | Solicitud de apertura; cliente vinculado; producto y condiciones |
| **O — Salida** | Cuenta abierta y operativa; contrato; movimientos registrados |
| **C — Cliente** | Cliente final; contabilidad |
| **Disparador** | Evento: «Solicitud de apertura de cuenta» |

| # | Actividad | Tipo | Rol | Sistema | Capacidad L2 | Dolor |
|---|---|:--:|---|---|---|---|
| 1 | Solicitud de apertura | ◐ | RL-ASE | APP-05 | M4.1 Cuentas de Ahorro | H-03 |
| 2 | Selección de producto y condiciones | ◐ | RL-ASE | APP-01 | M2.1 Diseño y Configuración | H-05 |
| 3 | Apertura de la cuenta en el core | ⚙️ | RL-ASE | APP-01 | M4.1 Cuentas de Ahorro | — |
| 4 | Formalización del contrato | ◐ | RL-ASE | APP-01 | M2.2 Acuerdos y Contratos | — |
| 5 | Entrega de medios de acceso | ◐ | RL-ASE | APP-08 | M5.4 Gestión de Tarjetas | — |
| 6 | Registro de depósitos y retiros | ⚙️ | — | APP-01 | M5.1 Ejecución de Pagos | — |
| 7 | Registro contable | ⚙️ | — | APP-11 | H1.1 Contabilidad (Ledger) | — |

**Controles:** Fondo de Seguro de Depósitos · transparencia (SBS).

---

### PN-04 · Ejecución de pagos y transferencias

| SIPOC | Contenido |
|---|---|
| **S — Proveedor** | Cliente; cámara de compensación (BCRP) |
| **I — Entrada** | Orden de pago o transferencia; datos del beneficiario |
| **O — Salida** | Pago ejecutado; confirmación al cliente; asiento contable |
| **C — Cliente** | Cliente final; beneficiario; contabilidad |
| **Disparador** | Evento: «Orden de pago recibida» |

| # | Actividad | Tipo | Rol | Sistema | Capacidad L2 | Dolor |
|---|---|:--:|---|---|---|---|
| 1 | Recepción de la orden | ⚙️ | RL-CLI | APP-06 · APP-07 | M6.1 Canales Digitales | **H-03** |
| 2 | Validación (saldo, límites, beneficiario) | ⚙️ | — | APP-01 | M5.1 Ejecución de Pagos | — |
| 3 | Verificación PLAFT de la operación | ⚙️ | RL-OFC | APP-13 | E3.2 PLAFT | — |
| 4 | Enrutamiento (interno / interbancario inmediato) | ⚙️ | — | APP-10 | M5.2 Pagos Inmediatos | — |
| 5 | Ejecución del cargo y abono | ⚙️ | — | APP-01 | M5.1 Ejecución de Pagos | — |
| 6 | Confirmación al cliente | ⚙️ | — | APP-07 | M6.1 Canales Digitales | — |
| 7 | Registro contable | ⚙️ | — | APP-11 | H1.1 Contabilidad (Ledger) | — |

**Controles:** sistemas de pago (BCRP) · interoperabilidad · PLAFT (UIF).
**Observación:** proceso plenamente automatizado. El dolor H-03 no está en la ejecución sino en el **alcance limitado del canal**: muchas operaciones simplemente no se ofrecen en la app.

---

### PN-05 · Operación en agente / corresponsal

| SIPOC | Contenido |
|---|---|
| **S — Proveedor** | Cliente; comercio aliado / agente corresponsal |
| **I — Entrada** | Operación en efectivo (depósito, retiro, pago); identificación del cliente |
| **O — Salida** | Operación aplicada en la cuenta; saldo actualizado; asiento contable |
| **C — Cliente** | Cliente final; contabilidad; operaciones |
| **Disparador** | Evento: «Operación registrada en agente» |

| # | Actividad | Tipo | Rol | Sistema | Capacidad L2 | Dolor |
|---|---|:--:|---|---|---|---|
| 1 | Identificación del cliente en el agente | ◐ | RL-COM | APP-09 | M6.2 Red de Corresponsalía | — |
| 2 | Captura de la operación | ⚙️ | RL-COM | APP-09 | M6.2 Red de Corresponsalía | — |
| 3 | **Entrega o recepción de efectivo** | 🖐️ | RL-COM | — | M6.2 Red de Corresponsalía | — |
| 4 | Registro provisional en la plataforma de agentes | ⚙️ | — | APP-09 | M6.2 Red de Corresponsalía | **H-04** |
| 5 | **Cierre y transmisión por lotes (nocturno)** | ⚙️ | — | APP-09 | M6.2 Red de Corresponsalía | **H-04** |
| 6 | **Conciliación de operaciones de agentes** | 🖐️ | RL-OPE | — | H4.1 Back Office | **H-04** |
| 7 | Aplicación en el core y ajuste de saldos | ⚙️ | — | APP-01 | M4.1 Cuentas de Ahorro | **H-04** |
| 8 | Registro contable | ⚙️ | — | APP-11 | H1.1 Contabilidad (Ledger) | — |

**Controles:** reglamento de cajeros corresponsales (SBS).
**Observación:** las actividades 4 a 7 son **la explicación mecánica de H-04**. La operación se captura en línea pero se aplica al día siguiente porque hay un cierre por lotes y una conciliación manual en el medio.

---

### PN-06 · Pago y cobro en efectivo por referencia — **TO-BE**

> Proceso **propuesto**, no existe hoy. El caso lo declara como la puerta de entrada que la línea de innovación quiere abrir (H-09 · O-08).

| SIPOC | Contenido |
|---|---|
| **S — Proveedor** | Persona sin cuenta; empresa emisora del cobro; comercio aliado |
| **I — Entrada** | Referencia de pago; efectivo |
| **O — Salida** | Pago confirmado en línea; notificación al beneficiario; liquidación al comercio |
| **C — Cliente** | Persona no bancarizada; empresa beneficiaria; comercio aliado |
| **Disparador** | Evento: «Referencia de pago generada» |

| # | Actividad | Tipo | Rol | Sistema | Capacidad L2 | Dolor |
|---|---|:--:|---|---|---|---|
| 1 | Generación de la referencia de pago | ⚙️ | — | *(sin sistema hoy)* | M5.3 Pagos con Referencia | **H-09** |
| 2 | **Presentación de la referencia en el punto físico** | 🖐️ | RL-CLI | — | M5.3 Pagos con Referencia | H-09 |
| 3 | **Recepción del efectivo** | 🖐️ | RL-COM | — | M5.3 Pagos con Referencia | H-09 |
| 4 | Confirmación en línea del pago | ⚙️ | — | *(sin sistema hoy)* | M5.3 Pagos con Referencia | **H-09** |
| 5 | Notificación al beneficiario | ⚙️ | — | *(sin sistema hoy)* | M5.3 Pagos con Referencia | — |
| 6 | Liquidación con el comercio aliado | ⚙️ | — | *(sin sistema hoy)* | E1.4 Alianzas y Ecosistema | — |
| 7 | Registro contable | ⚙️ | — | APP-11 | H1.1 Contabilidad (Ledger) | — |

**Controles:** cajeros corresponsales (SBS) · PLAFT para operaciones sin cuenta (UIF).
**Observación:** cuatro de las siete actividades **no tienen sistema que las soporte**. Ese vacío es exactamente la capacidad nueva M5.3.

---

### PN-07 · Administración y cobranza del crédito

| SIPOC | Contenido |
|---|---|
| **S — Proveedor** | Crédito desembolsado; cliente; áreas de riesgo |
| **I — Entrada** | Cronograma de cuotas; pagos recibidos; situación de mora |
| **O — Salida** | Cuotas cobradas; cartera clasificada; provisiones constituidas |
| **C — Cliente** | Cliente final; riesgos; contabilidad; SBS |
| **Disparador** | Evento: «Vencimiento de cuota» |

| # | Actividad | Tipo | Rol | Sistema | Capacidad L2 | Dolor |
|---|---|:--:|---|---|---|---|
| 1 | Generación y cobro de cuotas | ⚙️ | — | APP-02 | M3.3 Administración y Cobranza | — |
| 2 | Identificación de mora | ⚙️ | — | APP-02 | M3.3 Administración y Cobranza | — |
| 3 | Gestión de cobranza temprana | ◐ | RL-OPE | APP-04 | M3.3 Administración y Cobranza | H-02 |
| 4 | Clasificación del deudor y cálculo de provisión | ◐ | RL-ANC | APP-01 · APP-11 | E3.3 Gestión de Provisiones | — |
| 5 | **Cobranza judicial y castigo de cartera** | 🖐️ | RL-OPE | — | M3.3 Administración y Cobranza | — |
| 6 | Registro contable de provisiones | ⚙️ | — | APP-11 | H1.1 Contabilidad (Ledger) | — |

**Controles:** provisiones dinámicas (SBS) · Basilea III.

---

### PN-08 · Atención de consultas y reclamos

| SIPOC | Contenido |
|---|---|
| **S — Proveedor** | Cliente; áreas operativas |
| **I — Entrada** | Consulta o reclamo por cualquier canal |
| **O — Salida** | Caso resuelto y comunicado; reporte de reclamos al regulador |
| **C — Cliente** | Cliente final; SBS |
| **Disparador** | Evento: «Contacto de cliente recibido» |

| # | Actividad | Tipo | Rol | Sistema | Capacidad L2 | Dolor |
|---|---|:--:|---|---|---|---|
| 1 | Recepción del contacto | ◐ | RL-SOP | APP-04 | M6.4 Contact Center | — |
| 2 | Identificación y autenticación del cliente | ◐ | RL-SOP | APP-04 | M1.2 Identidad y Autenticación | H-02 |
| 3 | **Búsqueda de información en varios sistemas** | 🖐️ | RL-SOP | APP-01 · APP-04 · APP-06 | M1.3 CRM | **H-02** |
| 4 | Registro del caso | ⚙️ | RL-SOP | APP-04 | M1.4 Experiencia y Servicio | — |
| 5 | Resolución o derivación | ◐ | RL-SOP | APP-04 | M1.4 Experiencia y Servicio | — |
| 6 | Cierre y comunicación al cliente | ◐ | RL-SOP | APP-04 | M1.4 Experiencia y Servicio | — |
| 7 | **Reporte de reclamos al regulador** | 🖐️ | RL-OFC | APP-12 | E3.1 Cumplimiento y Reporte | **H-07** |

**Controles:** reglamento de atención al usuario (SBS).
**Observación:** la actividad 3 es la manifestación más visible de H-02 para el cliente: el asesor tiene que abrir tres sistemas para responder una pregunta.

---

### PN-09 · Lanzamiento y modificación de productos

| SIPOC | Contenido |
|---|---|
| **S — Proveedor** | Gestión de producto; riesgos; cumplimiento; TI |
| **I — Entrada** | Propuesta comercial; condiciones (tasas, comisiones, plazos) |
| **O — Salida** | Producto disponible en los canales; tarifario actualizado |
| **C — Cliente** | Áreas comerciales; cliente final; SBS |
| **Disparador** | Evento: «Propuesta de producto aprobada» |

| # | Actividad | Tipo | Rol | Sistema | Capacidad L2 | Dolor |
|---|---|:--:|---|---|---|---|
| 1 | **Definición comercial del producto** | 🖐️ | RL-PRO | — | M2.1 Diseño y Configuración | H-05 |
| 2 | **Evaluación de riesgo y cumplimiento** | 🖐️ | RL-ANC · RL-OFC | — | E2.1 Riesgo de Crédito | — |
| 3 | **Especificación funcional de condiciones** | 🖐️ | RL-PRO · RL-TI | — | M2.1 Diseño y Configuración | **H-05** |
| 4 | Desarrollo y parametrización en el core | ◐ | RL-TI | APP-01 · APP-02 | M2.1 Diseño y Configuración | **H-05 · H-12** |
| 5 | Pruebas y certificación | ◐ | RL-TI | APP-01 | — | H-05 · H-12 |
| 6 | Publicación en canales | ◐ | RL-TI | APP-06 · APP-07 | M6.1 Canales Digitales | **H-08** |
| 7 | Actualización del tarifario | ◐ | RL-PRO | APP-12 | M2.3 Tarifas y Precios | H-07 |

**Controles:** transparencia de información (SBS/Indecopi) · reglamento de productos.
**Observación:** la actividad 4 es la causa raíz de H-05 — **las condiciones del producto están embebidas en el código del core**, así que cambiar una tasa es un ciclo de desarrollo, no una parametrización.

---

### PN-10 · Cierre contable y reportería regulatoria y de cumplimiento

> El proceso con mayor carga manual del banco: **6 de 9 actividades**.

| SIPOC | Contenido |
|---|---|
| **S — Proveedor** | Core bancario; plataforma de agentes; switch; PLAFT; datawarehouse |
| **I — Entrada** | Movimientos del día; saldos; alertas; parámetros contables |
| **O — Salida** | Estados financieros; reportes regulatorios (SBS); reportes PLAFT (UIF) |
| **C — Cliente** | Alta dirección; SBS; UIF; auditoría |
| **Disparador** | Evento: «Cierre del día / cierre del período» |

| # | Actividad | Tipo | Rol | Sistema | Capacidad L2 | Dolor |
|---|---|:--:|---|---|---|---|
| 1 | Cierre de operaciones del día | ⚙️ | — | APP-01 | H1.1 Contabilidad (Ledger) | — |
| 2 | **Extracción de datos del core y satélites** | 🖐️ | RL-CON | APP-14 | H1.1 Contabilidad (Ledger) | **H-07 · H-11** |
| 3 | **Consolidación manual en hojas de cálculo** | 🖐️ | RL-CON | APP-12 | H1.1 Contabilidad (Ledger) | **H-07** |
| 4 | **Conciliación entre contabilidad y operaciones** | 🖐️ | RL-CON · RL-OPE | APP-12 | H1.1 Contabilidad (Ledger) | **H-07 · H-04** |
| 5 | **Ajustes manuales y reclasificaciones** | 🖐️ | RL-CON | APP-11 | H1.1 Contabilidad (Ledger) | **H-07** |
| 6 | Generación de estados financieros | ◐ | RL-CON | APP-11 | H1.2 Reportería Regulatoria | — |
| 7 | **Elaboración de reportes regulatorios (SBS)** | 🖐️ | RL-CON · RL-OFC | APP-12 | H1.2 Reportería Regulatoria | **H-07** |
| 8 | Elaboración de reportes PLAFT (UIF) | ◐ | RL-OFC | APP-13 · APP-12 | E3.2 PLAFT | H-07 |
| 9 | **Envío al regulador** | 🖐️ | RL-OFC | — | E3.1 Cumplimiento y Reporte | — |

**Controles:** Manual de Contabilidad (SBS) · reportes SBS · UIF · ISO 20022.
**Observación:** este proceso es **la prueba viva de H-07**. No hay una base transaccional única: la contabilidad se reconstruye cada período desde varias fuentes, con Excel de por medio, y por eso «no siempre cuadra» con cumplimiento. Es también el proceso que la oportunidad O-07 ataca de frente.

---

### PN-11 · Incorporación y habilitación de comercios y agentes

| SIPOC | Contenido |
|---|---|
| **S — Proveedor** | Comercio candidato; áreas de riesgo, cumplimiento y TI |
| **I — Entrada** | Solicitud de afiliación; documentación del comercio |
| **O — Salida** | Comercio afiliado, integrado y operativo como punto de atención |
| **C — Cliente** | Comercio aliado; red de canales; clientes de la zona |
| **Disparador** | Evento: «Solicitud de afiliación de comercio» |

| # | Actividad | Tipo | Rol | Sistema | Capacidad L2 | Dolor |
|---|---|:--:|---|---|---|---|
| 1 | **Prospección y evaluación del comercio** | 🖐️ | RL-OPE | APP-04 | E1.4 Alianzas y Ecosistema | — |
| 2 | Evaluación de riesgo y cumplimiento del aliado | ◐ | RL-OFC | APP-13 | E3.2 PLAFT | — |
| 3 | **Firma del contrato de corresponsalía** | 🖐️ | RL-OPE | — | E1.4 Alianzas y Ecosistema | — |
| 4 | Integración técnica del punto de atención | ◐ | RL-TI | APP-09 | H2.3 Integración y APIs | **H-08** |
| 5 | **Habilitación y capacitación** | 🖐️ | RL-OPE | — | E1.4 Alianzas y Ecosistema | — |
| 6 | Activación y monitoreo | ⚙️ | — | APP-09 | M6.2 Red de Corresponsalía | — |

**Controles:** reglamento de cajeros corresponsales (SBS) · PLAFT.
**Observación:** la actividad 4 materializa H-08 — cada nuevo punto exige una integración específica contra la plataforma de agentes, sin contrato de servicio estandarizado.

---

## 4. Matriz de trazabilidad Proceso → Hallazgo

| Hallazgo | Procesos donde se manifiesta |
|---|---|
| H-01 Demasiado tiempo y pasos | PN-01 · PN-02 |
| H-02 Información dispersa, datos repetidos | PN-01 · PN-02 · PN-07 · PN-08 |
| H-03 App y web solo consulta | PN-01 · PN-02 · PN-03 · PN-04 |
| H-04 Agentes se reflejan al día siguiente | PN-05 · PN-10 |
| H-05 Lanzar producto toma meses | PN-02 · PN-03 · PN-09 |
| H-06 Evaluación de crédito lenta | PN-02 |
| H-07 Reportes no cuadran | PN-08 · PN-09 · PN-10 |
| H-08 Integraciones costosas y frágiles | PN-09 · PN-11 |
| H-09 No bancarizados sin mecanismo | PN-06 |
| H-11 Datos no explotables | PN-10 |
| H-12 Cambio tecnológico caro y riesgoso | PN-09 |

**H-10** (nativos digitales) no se manifiesta en un proceso concreto sino en la **ausencia** de procesos digitales de extremo a extremo — se evidencia por omisión.

---

*Caso ficticio con fines didácticos. Repositorio: github.com/elwolfy/capstone-ea-bian-banco-horizonte*
