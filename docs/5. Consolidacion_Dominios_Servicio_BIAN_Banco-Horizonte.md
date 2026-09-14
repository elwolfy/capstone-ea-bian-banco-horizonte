# Consolidaciones del catálogo de Service Domains

**Capstone CD-03 · Curso de Arquitectura Bancaria basada en el Estándar BIAN**
Vista en Archi: *Horizonte · Consolidación de responsabilidades funcionales* · `Horizonte_ServiceDomains_Consolidado.ajs`

> Curso independiente de CPS Tech · No afiliado ni acreditado por BIAN e.V. · BIAN® es marca registrada de BIAN e.V., usada con fines descriptivos.

---

## Qué es este documento

La vista de derivación asignó un Service Domain a cada actividad de los procesos de Banco Horizonte. Al revisar el resultado aparecieron **seis decisiones de consolidación** que afectan a **10 de las 47 filas**.

Este documento explica **por qué** se tomó cada una. Las otras 37 filas no cambian.

**La idea central:** ninguna decisión se tomó por criterio propio. En cada caso se abrió el **Control Record** del dominio y se miró qué contiene. El registro decidió.

---

## La regla que decide todo

Cuando dos actividades caen en el mismo Service Domain, hay que preguntarse si son una o dos responsabilidades. La respuesta no es de opinión:

```
Dos actividades → el mismo Service Domain
            │
            ├─ ¿en procesos DISTINTOS?
            │        SÍ → REUTILIZACIÓN. Se dejan como están.
            │             Una responsabilidad, varios puntos de uso.
            │
            └─ ¿en el MISMO proceso?
                     │
                     └─ Abrir el Control Record.
                        ¿Tiene atributos de FASE o de ETAPA?
                              │
                              SÍ → SECUENCIA. Se dejan.
                              │    El registro mismo dice que hay etapas.
                              │
                              NO → DUPLICACIÓN. Se fusionan.
                                   Es una sola responsabilidad partida en dos.
```

**Por qué funciona.** En BIAN el Service Domain y su Control Record son **uno a uno**. El Control Record es la memoria del dominio: lo que puede recordar es exactamente lo que puede hacer. Si el registro no sabe distinguir dos momentos, no hay dos momentos.

**Contraejemplo que lo prueba.** `Party Relationship Administrative Plan` **sí** lleva `Party Life-cycle Maintenance Task`, `Lifecycle Status` y `Lifecycle Phase`. Por eso `PN-01.1` y `PN-01.3` se quedaron separadas: el registro modela fases.

---

# Las seis decisiones

| | Decisión | Filas | Tipo |
|---|---|---|---|
| **F1** | `PN-02.4` + `PN-02.5` → una actividad | 1 | Fusión |
| **F2** | `PN-10.7` + `PN-10.8` → una actividad | 1 | Fusión |
| **F3** | `PN-11.5a` absorbe la activación de `PN-11.6` | 1 | Fusión |
| **R1** | `PN-11.6` cambia de dominio | 1 | Re-derivación |
| **N1** | Se añade `PN-01.9` | 1 | Actividad nueva |
| **N2** | Se abre el proceso `PN-12` | 5 | Proceso nuevo |

---

## F1 · Evaluar y decidir un crédito son una sola cosa

**Antes**

| Actividad | Service Domain |
|---|---|
| `PN-02.4` Evaluación de capacidad de pago (scoring) | Underwriting |
| `PN-02.5` Decisión y aprobación | Underwriting |

**La pregunta.** Mismo dominio, mismo proceso. ¿Son dos responsabilidades?

**La evidencia.** Abrimos el Control Record `Underwriting Assessment`:

- **No tiene Behavior Qualifiers.** Ninguno.
- **No tiene atributos de fase.**
- Y entre sus atributos están, juntos: `Customer Income Statement`, `Customer Debt Statement`, `Customer Asset Statement`, `Customer Credit Assessment`, **`Decision`** y `Work Product`.

**La lógica.** Los insumos de la evaluación y la decisión viven en el **mismo registro, en la misma instancia**. `Decision` no es un registro nuevo: es un atributo más del mismo expediente de suscripción. El registro no distingue dos momentos, luego no hay dos responsabilidades.

**Después**

| Actividad | Service Domain |
|---|---|
| `PN-02.4` **Suscripción y decisión de crédito** | Underwriting |

**Y la objeción razonable:** *«pero en el banco evalúa un analista y decide un comité».* Cierto, y no cambia nada. Eso es **organización**, no arquitectura. BIAN modela **responsabilidad, no ejecutor**. Los dos pasos se documentan dentro de la actividad; el dominio sigue siendo uno.

> **Qué enseña.** Que el organigrama no dicta el catálogo. Si cada traspaso entre personas creara un Service Domain, tendríamos tantos dominios como puestos de trabajo.

---

## F2 · Dos reportes al regulador son una sola responsabilidad

**Antes**

| Actividad | Service Domain |
|---|---|
| `PN-10.7` Elaboración de reportes regulatorios (SBS) | Regulatory Reporting · faceta `Authoring` |
| `PN-10.8` Elaboración de reportes PLAFT (UIF) | Regulatory Reporting · faceta `Authoring` |

**La pregunta.** Mismo dominio, misma faceta, mismo proceso. Lo único distinto es **a quién se le reporta**. ¿Eso hace dos responsabilidades?

**La evidencia.** El Control Record `Regulatory Compliance Administrative Plan` tiene **exactamente cuatro atributos**:

| Atributo |
|---|
| **`Regulatory Authority Reference`** |
| `Regulatory Reporting Schedule` |
| `Regulation Reference` |
| **`Regulatory Report Type`** |

**La lógica.** La autoridad destinataria y el tipo de reporte **ya son datos del registro**. Cuando la única diferencia entre dos actividades es un valor que el propio Control Record guarda como atributo, esas actividades son **una sola, parametrizada**.

**Después**

| Actividad | Service Domain |
|---|---|
| `PN-10.7` **Elaboración de reportes regulatorios (SBS y UIF)** | Regulatory Reporting · faceta `Authoring` |

**¿Y por qué no Compliance Reporting para el PLAFT?** Porque ese dominio es otra cosa. Su definición publicada dice que *administra y orquesta las tareas para aplicar y reportar sobre la actividad de control y reporte de **auditoría interna***. Es auditoría interna, no reporte a un regulador externo. La frontera queda documentada.

> **Qué enseña.** A leer el Control Record como criterio de diseño de procesos. Si la variación entre dos actividades ya es un atributo del registro, sobra una actividad.

---

## F3 · Habilitar y activar un agente es un solo ejercicio del plan

**Antes**

| Actividad | Service Domain |
|---|---|
| `PN-11.5a` Habilitación del agente | Partner Administration |
| `PN-11.6` Activación y monitoreo | Partner Administration |

**La pregunta.** La misma de F1: ¿el registro distingue etapas?

**La evidencia.** El Control Record `Partner Administrative Plan` tiene estos atributos, y ninguno más:

`Budget Type` · `Budget` · `Assignment` · `Duty` · `Associated Party` · `Budget Balance` · `Subject Matter` · `Type` · `Reference` · `Description`

**Sin Behavior Qualifiers. Sin atributos de fase.**

**La lógica.** Habilitar y activar son el mismo acto administrativo sobre el mismo plan. El registro no puede distinguirlos, luego no son dos responsabilidades.

**Después**

| Actividad | Service Domain |
|---|---|
| `PN-11.5a` **Habilitación y activación del agente** | Partner Administration |

> **Qué enseña.** Que la misma regla da resultados opuestos según el registro. `Party Lifecycle Management` **sí** modela fases y por eso conserva dos actividades; `Partner Administration` no las modela y por eso fusiona. El criterio es único, la respuesta depende del dato.

---

## R1 · Monitorear no es administrar

**Antes**

| Actividad | Service Domain |
|---|---|
| `PN-11.6` Activación y **monitoreo** | Partner Administration |

Al fusionar la activación en F3 quedó suelto el monitoreo. Y ahí apareció algo mejor.

**La pregunta.** ¿Sobre qué activo actúa realmente el monitoreo de un agente?

**La evidencia.** Tres dominios distintos tocan al mismo socio, cada uno con su propio verbo y su propio activo:

| Service Domain | Patrón funcional | Tipo de activo | Control Record |
|---|---|---|---|
| **Partner Agreement** | `Agree Terms` | `Partner` | `Partner Agreement` |
| **Partner Administration** | `Administer` | `Partner` | `Partner Administrative Plan` |
| **Operations Log** | `Track` | **`Partner Event`** | **`Partner Event Log`** |

**La lógica.** Monitorear no es administrar un plan: es **registrar lo que va pasando**. El patrón es `Track`, y el activo no es el socio sino el **evento** de su operación. Ese activo tiene dominio propio y registro propio.

**Después**

| Actividad | Service Domain |
|---|---|
| `PN-11.6` **Monitoreo de la operación del agente** | Operations Log |

> **Qué enseña.** Es la mejor lección de granularidad del caso: **tres dominios sobre el mismo socio**. Lo que se pacta con él, el plan con que se le administra, y el registro de lo que hace. Tres verbos, tres activos, tres registros. Confundirlos es lo que produce los sistemas monolíticos de gestión de terceros.

---

## N1 · Faltaba el contrato marco

**Antes.** El proceso `PN-01` crea la relación con el cliente, captura sus datos y documentos, valida su identidad, verifica listas, habilita credenciales y canales, y activa productos.

**Nunca firma el acuerdo marco.**

**La pregunta.** ¿Es un olvido del levantamiento o realmente no existe la actividad?

**La evidencia.** Está en la estructura. El Control Record `Customer Agreement` contiene entre sus atributos:

| Atributo | Apunta a |
|---|---|
| **`Sales Product Agreement Reference`** | El contrato de producto de `PN-02.7` |
| **`Party Life-cycle Management Reference`** | El plan de relación de `PN-01.1` |

Y la definición publicada de **Sales Product Agreement** lo dice sin rodeos: *es subordinado al acuerdo maestro del cliente, que mantiene el dominio Customer Agreement*.

**La lógica.** Sin `Customer Agreement`, el contrato de crédito de `PN-02.7` **no tiene padre**, y esos dos atributos quedan apuntando al vacío. El metamodelo exige la actividad aunque el levantamiento no la haya visto.

**Después**

| Actividad | Patrón | Activo | Service Domain |
|---|---|---|---|
| `PN-01.9` **Suscripción del contrato marco** | `Agree Terms` | `Customer` | **Customer Agreement** |

> **Qué enseña.** Es el argumento más fuerte del método completo: **la derivación no solo valida lo que hay, descubre lo que falta**. Y no es un formalismo: el contrato marco de servicios financieros es una obligación real de transparencia.

---

## N2 · Dentro de un proceso había dos

**Antes.** Un solo proceso, `PN-11 Incorporación de comercios y agentes`, mezclaba dos figuras.

**La pregunta.** ¿Un comercio y un agente corresponsal son lo mismo para BIAN?

**La evidencia.** No. Son **dos tipos de activo distintos**, y por eso dos dominios distintos, aunque el verbo sea el mismo:

| | Agente corresponsal | Comercio adquirente |
|---|---|---|
| Patrón funcional | `Agree Terms` | `Agree Terms` — **el mismo** |
| Tipo de activo | `Partner` | `Merchant Relationship` — **distinto** |
| Service Domain | **Partner Agreement** | **Merchant Relations** |
| Control Record | `Partner Agreement` | `Merchant Relationship Agreement` |

**La lógica.** Los 341 Service Domains son MECE **por tipo de activo**. Mantener las dos figuras en un solo proceso obliga a elegir entre dos dominios que el estándar separa a propósito. El solapamiento no estaba en BIAN: estaba en el proceso.

**Después.** `PN-11` se queda con los agentes corresponsales, y se abre un proceso nuevo:

| Actividad de `PN-12` | Patrón | Activo | Service Domain |
|---|---|---|---|
| `PN-12.1` Prospección y evaluación del comercio | `Process` | `Leadand Opportunity` | Lead and Opportunity Management |
| `PN-12.2` Evaluación de riesgo y cumplimiento | `Assess` | `Regulatory Compliance` | Regulatory Compliance |
| `PN-12.3` Firma del contrato de afiliación | `Agree Terms` | `Merchant Relationship` | **Merchant Relations** |
| `PN-12.4` Instalación y administración de terminales POS | `Allocate` | `Card POS Device` | **Card Terminal Administration** |
| `PN-12.5` Activación del comercio y operación de la cuenta | `Fulfill` | `Merchant Acquiring` | **Merchant Acquiring Facility** |

**Un efecto colateral valioso.** Al abrir `PN-12`, dos dominios pasan a invocarse desde más procesos:

- `Lead and Opportunity Management` → ahora en `PN-11` y `PN-12`
- `Regulatory Compliance` → ahora en `PN-01`, `PN-11` y `PN-12`

Eso **no es duplicación**: es reutilización. Una responsabilidad única con varios puntos de invocación, que es precisamente el argumento del desacoplamiento.

> **Qué enseña.** Que el mismo patrón funcional sobre activos distintos produce dominios distintos. Y que cuando parece haber un solapamiento en BIAN, casi siempre el solapamiento está en cómo declaramos el proceso.
>
> **Nota de tailoring.** Si Banco Horizonte no afilia comercios, `PN-12` se retira completo. Eso es *tailoring por ausencia*, y se justifica por escrito.

---

# Efecto de las seis decisiones

| | Antes | Después |
|---|---|---|
| Procesos | 5 | **6** |
| Filas de derivación | 43 | **47** |
| Service Domains | 26 | **31** |
| **Duplicaciones** | **5** | **1** |
| Reutilización entre procesos | 8 filas | **11 filas** |
| Filas sin duplicación ni acoplamiento indebido | 25 de 43 · 58 % | **34 de 47 · 72 %** |

**La duplicación que queda** es `PN-01.5 Registro del cliente en el core`, y no se resuelve consolidando actividades: repite el mismo `Catalog` sobre `Party Reference Data` que `PN-01.2a` porque el banco tiene **dos sistemas de registro de la parte**. Es una brecha de arquitectura, y va al roadmap.

## Los cinco Service Domains que se incorporan

| Service Domain | Patrón | Activo | Control Record | Origen |
|---|---|---|---|---|
| **Customer Agreement** | `Agree Terms` | `Customer` | `Customer Agreement` | N1 |
| **Operations Log** | `Track` | `Partner Event` | `Partner Event Log` | R1 |
| **Merchant Relations** | `Agree Terms` | `Merchant Relationship` | `Merchant Relationship Agreement` | N2 |
| **Card Terminal Administration** | `Allocate` | `Card POS Device` | `Card POS Device Allocation` | N2 |
| **Merchant Acquiring Facility** | `Fulfill` | `Merchant Acquiring` | `Merchant Acquiring Facility` | N2 |

Los 31 son del catálogo estándar de 341. **Cero dominios a medida.**

---

# Lo que hay que retener

**1. El Control Record es el árbitro.** Ante la duda de si dos actividades son una o dos, se abre el registro y se miran sus atributos. No se discute.

**2. La misma regla da respuestas opuestas.** `Party Lifecycle Management` conserva dos actividades y `Partner Administration` fusiona, con el mismo criterio aplicado. La regla es única; el dato decide.

**3. El método encuentra lo que falta.** `PN-01.9` no salió del levantamiento: salió de dos atributos que apuntaban al vacío.

**4. El mismo verbo sobre activos distintos son dominios distintos.** `Agree Terms` sobre `Partner` y sobre `Merchant Relationship` no son intercambiables, y por eso `PN-11` tenía que partirse.

**5. Fusionar no es perder detalle.** Las 37 filas que no cambian —el 79 %— confirman que la derivación de línea base era correcta. Las consolidaciones quitaron redundancia y completaron vacíos; no corrigieron errores de asignación.
