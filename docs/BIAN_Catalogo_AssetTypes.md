# Catálogo de Asset Types en BIAN

**Guía de referencia y variación por tipo de entidad financiera**

Curso CD-03 · Arquitectura Bancaria basada en el estándar BIAN · Material de apoyo del Módulo 3
CPS Tech · Jorge Valenzuela Posadas

> Curso independiente de CPS Tech · No afiliado ni acreditado por BIAN e.V. · BIAN® es marca registrada de BIAN e.V., usada con fines descriptivos.

---

## 0. Advertencia metodológica — léala antes de usar este catálogo

BIAN **afirma** que tiene una clasificación jerárquica de Asset Types, pero **no la publica como un árbol navegable**. La sección 2.4.3 del libro dice, literal:

> *«BIAN has defined a hierarchical Asset Type classification, up to a certain level of granularity.»*

Y no la reproduce. A diferencia de los Functional Patterns (Tabla 2-2, los 19 con descripción) y de los Generic Artifacts (Tabla 2-3 y Figura 2-8, el mapeo completo), **el Asset Type no tiene tabla propia**. En el índice del libro aparece solo en las páginas 32, 34, 40, 44, 46, 47 y 53, todas de texto y metamodelo.

Por eso este documento distingue tres niveles de evidencia, y cada entrada va marcada:

| Marca | Significado |
|---|---|
| **[LITERAL]** | Aparece textualmente en BIAN 2nd Edition o en el syllabus Foundation v3.8, con la sección citada |
| **[RECONSTRUIDO]** | Inferido a partir de los Service Domains publicados en el Service Landscape. La *existencia* del activo es segura porque hay un dominio que lo usa; su *nombre exacto* debe verificarse en el repositorio |
| **[SUPUESTO]** | Construcción didáctica propia para explicar el mecanismo o para ilustrar la variación entre entidades. No es contenido del estándar |

**Cómo usar esto sin equivocarse:** el catálogo oficial de Service Domains de BIAN **ya viene detenido en el umbral**. Si usted trabaja con ese catálogo, no necesita reconstruir la jerarquía: los activos ya están fijados. Este documento se necesita en dos situaciones, ambas frecuentes en consultoría:

1. **Tailoring** — cuando la operación real de la entidad exige mover el nivel de un activo (el caso M5 Banking Group del capítulo 4).
2. **Partir de un AS-IS propio** — cuando se identifican dominios candidatos desde un inventario de procesos, antes de contrastar contra el Service Landscape. Es exactamente el taller del Módulo 3 y el hito del Módulo 4.

---

## 1. Qué es un Asset Type

**[LITERAL] · BIAN 2nd Ed., Secc. 2.4.3**

> *«An Asset Type refers to something tangible or intangible that the bank has ownership and/or influence over and has one or more inherent uses or purposes for, that create commercial value.»*

Tres condiciones, y las tres deben cumplirse:

1. **Algo** — tangible o intangible, pero una cosa, no un atributo de otra cosa.
2. **Propiedad o influencia del banco** — el banco lo posee o lo controla.
3. **Usos inherentes que crean valor comercial** — sirve para algo que produce valor.

### 1.1 La prueba del verbo

La forma más rápida de decidir si algo es un Asset Type es **ponerle delante uno de los 19 Functional Patterns y escuchar si suena a responsabilidad**:

- «*Fulfill* la cuenta corriente» → sí. Es un activo.
- «*Catalog* los datos de referencia de la parte» → sí. Es un activo.
- «*Assess* el riesgo de crédito» → sí. Es un activo.
- «*Fulfill* la tasa por pago en ventanilla» → no. Es un dato.
- «*Manage* el canal móvil» → cuidado: el canal como *infraestructura de atención* puede ser activo; el canal como *discriminador de instancias* no lo es.

**Si ninguno de los 19 patrones encaja, no es un Asset Type: es un dato, un atributo o un Behavior Qualifier.**

### 1.2 Los dos criterios que fijan el nivel

| Criterio | Pregunta que responde | Fuente |
|---|---|---|
| **Umbral de descomposición** (*threshold of decomposition*) | ¿Dónde dejo de bajar en la jerarquía? | [LITERAL] 2.4.3 — *«the bank either requires the functionality in its entirety or not at all»* |
| **Ciclo de vida completo** (*full lifecycle*) | ¿Hasta dónde llega la responsabilidad? | [LITERAL] 2.4.3 — *«responsible for implementing its Functional Pattern on each instance of its associated Asset Type for its full lifecycle»* |

El primero prueba la divisibilidad **funcional**; el segundo, la divisibilidad **temporal**. Un activo mal elegido suele pasar uno y fallar el otro.

---

## 2. Las tres familias de Asset Types

**[LITERAL] · BIAN 2nd Ed., Secc. 2.4.3** — el libro nombra explícitamente estas tres familias:

### 2.1 Evidentes (tangibles)

> *«Some Asset Types are obvious - for example a machine or building.»*

Cosas físicas que el banco posee. Son las más fáciles de identificar y, paradójicamente, las que menos dominios generan en un banco moderno.

### 2.2 Intangibles fácilmente identificables

> *«Some are intangible but easily identified such as knowhow, knowledge, relationships, reputation.»*

Cuatro nombrados por el libro: **know-how, conocimiento, relaciones, reputación**. Aquí vive, por ejemplo, la relación con el cliente.

### 2.3 «Capacidad de realizar» (*capacity to perform*)

> *«Some are less obvious - most common is the "capacity to perform" type which applies to many BIAN Service Domains. For example, in the case of product fulfillment and support activities like party authentication, the asset is the bank's ability to perform these activities.»*

**Es la familia más usada del estándar** y la más difícil de aceptar la primera vez. La habilidad del banco de autenticar a una parte es un activo. Esta familia es la que permite que BIAN cubra funciones que no tienen una cosa física ni un contrato detrás.

---

## 3. Catálogo de Asset Types por agrupación

**[RECONSTRUIDO]** salvo donde se indique. La existencia de cada activo se infiere de que hay Service Domains publicados que lo usan; **los nombres exactos deben verificarse en el repositorio** (`bian.org/servicelandscape-14-0-0/`), donde el Asset Type aparece por Service Domain, no como árbol independiente.

Columna «Patrón típico»: el Functional Pattern con el que más se combina. Un mismo activo puede aparecer con varios patrones y generar dominios distintos.

### 3.1 Parte y relación

| Asset Type | Familia | Patrón típico | Control Record resultante | Nota |
|---|---|---|---|---|
| **Party Reference Data** | Intangible · conocimiento | Catalog | Party Reference Data Directory Entry | **[LITERAL]** Figura 2-11. Ejemplo canónico del libro |
| **Customer Relationship** | Intangible · relaciones | Manage | Customer Relationship Management Plan | **[LITERAL]** citado en 2.4.3 como ejemplo del ciclo de vida completo |
| **Capacidad de autenticar a una parte** | Capacidad de realizar | Fulfill | Party Authentication Arrangement | **[LITERAL]** el libro nombra *party authentication* como ejemplo de *capacity to perform* |
| **Perfil de segmento de cliente** | Intangible · conocimiento | Analyze | Customer Segment Analysis | [RECONSTRUIDO] |
| **Contacto / interacción con la parte** | Capacidad de realizar | Track | Contact Log | [RECONSTRUIDO] |

### 3.2 Productos y arreglos (*arrangements*)

| Asset Type | Familia | Patrón típico | Control Record resultante | Nota |
|---|---|---|---|---|
| **Current Account** | Intangible · relación contractual | Fulfill | Current Account Arrangement | **[LITERAL]** Figuras 2-9, 2-25 y 2-28. El ejemplo más desarrollado del libro |
| **Savings Account** | Intangible · relación contractual | Fulfill | Savings Account Arrangement | [RECONSTRUIDO] |
| **Term Deposit** | Intangible · relación contractual | Fulfill | Term Deposit Arrangement | [RECONSTRUIDO] |
| **Loan / préstamo** | Intangible · relación contractual | Fulfill | Loan Arrangement | **[LITERAL]** en el caso M5 el libro habla de los SD que cumplen *loan agreements* |
| **Credit Facility / línea de crédito** | Intangible · relación contractual | Fulfill | Credit Facility Arrangement | [RECONSTRUIDO] |
| **Standing Order** | Intangible · instrucción permanente | Fulfill | Standing Order Arrangement | **[LITERAL]** Figura 4-4. Caso de promoción de Behavior Qualifier a Asset Type |
| **Especificación de producto** | Intangible · know-how | Design | Product Specification | [RECONSTRUIDO] — aquí vive el tarifario, no en un activo «tasa» |

### 3.3 Pagos y transacciones

| Asset Type | Familia | Patrón típico | Control Record resultante | Nota |
|---|---|---|---|---|
| **Pago** | Capacidad de realizar | Transact | Payment Transaction | [RECONSTRUIDO] |
| **Orden de pago** | Intangible · instrucción | Process | Payment Order Procedure | [RECONSTRUIDO] |
| **Relación de corresponsalía** | Intangible · relaciones | Manage | Correspondent Management Plan | [RECONSTRUIDO] |
| **Capacidad de compensar y liquidar** | Capacidad de realizar | Operate | Clearing Operating Session | [RECONSTRUIDO] |

### 3.4 Riesgo, cumplimiento y control

| Asset Type | Familia | Patrón típico | Control Record resultante | Nota |
|---|---|---|---|---|
| **Riesgo de crédito de una parte** | Intangible · conocimiento | Assess | Credit Risk Assessment | [RECONSTRUIDO] |
| **Modelo de riesgo** | Intangible · know-how | Design | Risk Model Specification | [RECONSTRUIDO] |
| **Obligación regulatoria** | Intangible · obligación | Fulfill | Regulatory Compliance Arrangement | [RECONSTRUIDO] |
| **Caso de investigación PLAFT** | Capacidad de realizar | Process | Investigation Procedure | [RECONSTRUIDO] |
| **Exposición de riesgo de mercado** | Intangible · posición | Monitor | Market Risk State | [RECONSTRUIDO] |
| **Evento de fraude** | Capacidad de realizar | Assess | Fraud Assessment | [RECONSTRUIDO] |

### 3.5 Finanzas y contabilidad

| Asset Type | Familia | Patrón típico | Control Record resultante | Nota |
|---|---|---|---|---|
| **Journal financiero** | Intangible · registro | Track | Financial Journal Log | [RECONSTRUIDO] |
| **Posición financiera** | Intangible · posición | Monitor | Financial Position State | [RECONSTRUIDO] |
| **Obligación tributaria** | Intangible · obligación | Fulfill | Tax Arrangement | [RECONSTRUIDO] |
| **Presupuesto de la unidad** | Intangible · plan | Manage | Budget Management Plan | [RECONSTRUIDO] |

### 3.6 Canales y puntos de servicio

| Asset Type | Familia | Patrón típico | Control Record resultante | Nota |
|---|---|---|---|---|
| **Sucursal / local de atención** | Evidente · edificio | Manage | Branch Management Plan | [RECONSTRUIDO] — el libro nombra «building» como activo evidente |
| **Cajero automático** | Evidente · máquina | Operate | ATM Operating Session | [RECONSTRUIDO] — el libro nombra «machine» como activo evidente |
| **Punto de atención de terceros (agente / corresponsal)** | Intangible · relaciones | Administer | Agent Administrative Plan | [RECONSTRUIDO] |
| **Canal digital** | Capacidad de realizar | Operate | Channel Operating Session | [RECONSTRUIDO] — atención: el canal como infraestructura, no como discriminador de instancias |

### 3.7 Recursos internos de la empresa

| Asset Type | Familia | Patrón típico | Control Record resultante | Nota |
|---|---|---|---|---|
| **Personal / recurso humano** | Evidente · persona | Allocate | Resource Allocation | [RECONSTRUIDO] — el patrón *Allocate* está definido para «staff and/or facilities» **[LITERAL]** Tabla 2-3 |
| **Instalación / facility** | Evidente · edificio | Allocate | Facility Allocation | [RECONSTRUIDO] |
| **Equipo / máquina** | Evidente · máquina | Maintain | Equipment Maintenance Arrangement | [RECONSTRUIDO] |
| **Activo de TI** | Evidente · máquina | Administer | IT Asset Administrative Plan | [RECONSTRUIDO] |
| **Estrategia de la unidad** | Intangible · know-how | Direct | Strategy | [RECONSTRUIDO] — *Direct* produce *Strategy* **[LITERAL]** Tabla 2-3 |

### 3.8 Conocimiento y mercado

| Asset Type | Familia | Patrón típico | Control Record resultante | Nota |
|---|---|---|---|---|
| **Datos de mercado** | Intangible · conocimiento | Catalog | Market Data Directory Entry | [RECONSTRUIDO] |
| **Reputación / marca** | Intangible · reputación | Manage | Brand Management Plan | [RECONSTRUIDO] — el libro nombra «reputation» como activo intangible **[LITERAL]** |
| **Know-how especializado** | Intangible · know-how | Advise | Advice | [RECONSTRUIDO] |
| **Campaña comercial** | Intangible · plan | Manage | Campaign Management Plan | [RECONSTRUIDO] |

---

## 4. Cómo varía el catálogo entre entidades financieras

### 4.1 El principio

**[LITERAL]** El libro dice que BIAN definió los Asset Types **«likely»** —probables— que se encuentran en cualquier banco, y que el Service Landscape *«is not intended to represent a design blueprint for any bank»*.

De ahí la asimetría que sostiene todo el estándar:

> **Los 19 Functional Patterns y sus 19 Generic Artifacts son un catálogo CERRADO. La jerarquía de Asset Types es la parte AJUSTABLE.**

Eso es lo que permite que dos entidades con activos muy distintos sigan hablando el mismo idioma arquitectónico.

### 4.2 Las cuatro formas de variación

| Forma | Qué ocurre | Ejemplo |
|---|---|---|
| **Ausencia** | El activo no existe en esa entidad | Una caja municipal no tiene *custodia de valores* ni *cartera de trading* |
| **Generalización** (subir) | Varios activos se funden en uno más general | **[LITERAL]** Caso M5: los SD que cumplen agreements de préstamo se fusionan; el patrón sigue siendo *Fulfil*, el Asset Type se generaliza |
| **Especialización** (bajar) | Un Behavior Qualifier se promueve a Asset Type | **[LITERAL]** Caso M5: *Standing Order* deja de ser qualifier del Current Account y pasa a ser activo con dominio propio |
| **Extensión** | Aparece un activo que el catálogo no cubre | Figuras locales o regulatorias: crédito grupal solidario, aporte social de un socio |

### 4.3 Matriz comparativa por tipo de entidad

Leyenda: **✔** existe y es central · **○** existe pero marginal o tercerizado · **✘** no aplica · **▲** aparece especializado o con nombre propio

| Asset Type | Banco universal | Caja municipal / microfinanciera | Banco digital / neobanco | Cooperativa de ahorro y crédito | Banca de inversión y custodia |
|---|---|---|---|---|---|
| Party Reference Data | ✔ | ✔ | ✔ | ▲ *socio*, no *cliente* | ✔ |
| Customer Relationship | ✔ | ✔ | ✔ | ▲ *relación asociativa* | ✔ |
| Capacidad de autenticar | ✔ | ✔ | ✔ crítica | ✔ | ✔ |
| Current Account | ✔ | ○ | ✔ | ✔ | ○ |
| Savings Account | ✔ | ✔ | ✔ | ✔ | ✘ |
| Term Deposit | ✔ | ✔ | ○ | ✔ | ○ |
| Loan | ✔ | ✔ ▲ *crédito individual* | ○ | ✔ | ✘ |
| **Crédito grupal solidario** | ✘ | ▲ **activo propio** | ✘ | ○ | ✘ |
| **Aporte social / capital del socio** | ✘ | ○ | ✘ | ▲ **activo propio** | ✘ |
| Credit Facility | ✔ | ○ | ○ | ○ | ✔ |
| Standing Order | ✔ | ○ | ✔ | ○ | ✘ |
| Pago | ✔ | ✔ | ✔ | ✔ | ○ |
| Relación de corresponsalía | ✔ | ▲ **red de agentes**, central | ○ | ○ | ✔ |
| Riesgo de crédito | ✔ | ✔ ▲ evaluación de campo | ✔ ▲ scoring alternativo | ✔ | ○ |
| Riesgo de mercado | ✔ | ✘ | ✘ | ✘ | ✔ central |
| **Instrumento en custodia** | ○ | ✘ | ✘ | ✘ | ▲ **activo central** |
| **Mandato de inversión** | ○ | ✘ | ✘ | ✘ | ▲ **activo central** |
| Journal financiero | ✔ | ✔ | ✔ | ✔ | ✔ |
| Obligación regulatoria | ✔ | ✔ ▲ régimen específico | ✔ | ✔ ▲ régimen cooperativo | ✔ |
| Sucursal | ✔ | ✔ central | ✘ | ✔ | ○ |
| Cajero automático | ✔ | ○ | ✘ tercerizado | ○ | ✘ |
| Punto de atención de terceros | ○ | ✔ **central** | ○ | ○ | ✘ |
| Canal digital | ✔ | ○ | ✔ **es el banco** | ○ | ✔ |
| Efectivo en bóveda | ✔ | ✔ central | ✘ | ✔ | ✘ |

**[SUPUESTO]** La matriz es una construcción didáctica. Su valor no está en los símbolos sino en la conversación que provoca: en un taller real, cada celda debe justificarse.

---

## 5. Cinco casos de variación, desarrollados

### Caso 1 — Generalizar: el grupo M5 sube un escalón · [LITERAL]

**Situación.** El grupo M5 tenía varios Service Domains cumpliendo *agreements* de préstamo, uno por tipo de producto comercial de cada banco miembro.

**Movimiento.** Los fusiona en un dominio de préstamo más general. El Functional Pattern sigue siendo *Fulfil*; **el Asset Type se generaliza**.

**Razón, en palabras del libro.** La «fábrica de productos» del grupo —las áreas que aseguran el cumplimiento de los acuerdos— soporta productos **según el tipo de características, no según su presentación comercial**. Cada banco miembro tiene su propio catálogo comercial, pero la fábrica es la misma.

**Lección.** La razón para mover el nivel es **operativa**, no estética. Se sube cuando la operación real no distingue lo que el catálogo comercial distingue.

---

### Caso 2 — Especializar: el Standing Order se independiza · [LITERAL]

**Situación.** *Standing Order* —la orden de pago recurrente— era un **Behavior Qualifier** dentro del Control Record del dominio *Current Account*.

**Movimiento.** El grupo decide que ese activo es independiente de la cuenta. El Behavior Qualifier **se promueve a Asset Type** y nace un Service Domain propio que cumple su *arrangement*.

**Efecto en el dato, literal del libro.** El qualifier *desaparece* del Control Record del Current Account, y lo que era *«Payment Service Arrangement»* pasa a llamarse *«Standing Order Agreement»* en el BOM del nuevo dominio. El objeto sigue relacionado con el *Current Account Agreement* a través de *«Payment Instruction Involved Account»*.

**Lección — la más importante del documento.** Al mover la frontera del Asset Type **no se mueve solo la función: se mueve el dueño del dato**. Este es el mecanismo con el que se corrige un problema de propiedad de datos, no un ejercicio de nomenclatura.

---

### Caso 3 — Extender: el crédito grupal solidario en microfinanzas · [SUPUESTO]

**Situación.** Una caja municipal o entidad de microfinanzas coloca crédito grupal solidario: un grupo de personas se garantiza mutuamente, la evaluación es del grupo y del individuo a la vez, y la mora de uno afecta a todos.

**¿Es un activo nuevo o es un préstamo con otras condiciones?** Aplique los dos criterios:

- *Umbral*: ¿puede el banco quedarse con la mitad de «cumplir el acuerdo de crédito grupal»? No: la garantía solidaria es indivisible del acuerdo.
- *Ciclo de vida*: ¿responde alguien por el grupo de principio a fin, con vida propia distinta de la de cada crédito individual? Sí — el grupo se forma, se evalúa, se renueva y se disuelve.

**Conclusión.** El grupo solidario **tiene ciclo de vida propio**, luego es un Asset Type nuevo, no una variante del préstamo. La garantía solidaria no es un atributo del contrato individual: es la sustancia del acuerdo grupal.

**Contraste.** «Crédito de consumo» y «crédito vehicular» **no** son activos nuevos: mismo patrón, mismo activo, distintas condiciones del *arrangement*.

---

### Caso 4 — Ausencia y desplazamiento: el banco digital · [SUPUESTO]

**Desaparecen.** *Sucursal*, *efectivo en bóveda*, *cajero automático propio*. No es que estén tercerizados: no existen en el modelo de negocio.

**Se vuelven críticos.** *Capacidad de autenticar a una parte* pasa de ser un dominio de soporte a ser el corazón del riesgo operativo. *Canal digital* deja de ser un punto de contacto entre varios: **es el banco**.

**Aparece la tentación del error.** Con un solo canal, es fácil que alguien proponga «Service Domain de la App Móvil». Eso es cortar por canal, es decir, por instancias. La app no es un activo: es el medio por el que se accede a muchos dominios.

**Y aparece un activo genuinamente nuevo.** La *identidad digital verificada* —con su ciclo de vida propio: se crea, se eleva de nivel, se revoca— es candidata a Asset Type propio, distinta de *Party Reference Data*.

---

### Caso 5 — El mismo nombre, otro significado: la cooperativa · [SUPUESTO]

**Situación.** En una cooperativa de ahorro y crédito, el cliente **es socio**: aporta capital, tiene derechos políticos, elige y puede ser elegido.

**El error fácil.** Traducir *socio* como *Party Reference Data* y seguir adelante. Se pierde la mitad del modelo.

**El análisis correcto.** Hay dos activos, no uno:

1. **Party Reference Data** — los datos de referencia de la persona. Idéntico a cualquier banco.
2. **Aporte social / capital del socio** — con su ciclo de vida propio: se suscribe, se paga, genera derechos, se rescata al retirarse. Nadie más responde por él.

**Y un tercer candidato.** El *derecho político del socio* —voto, elegibilidad— es una responsabilidad con ciclo de vida propio que ningún banco comercial tiene.

**Lección.** Cuando una entidad usa una palabra distinta para lo que parece el mismo concepto, casi siempre hay un activo adicional escondido detrás de esa palabra.

---

## 6. Qué NO es un Asset Type — las siete confusiones frecuentes

| Se propone como activo | Qué es en realidad | Cómo detectarlo |
|---|---|---|
| **Una tasa o comisión** | Behavior Qualifier del *arrangement*. **[LITERAL]** el libro lista *«Service Fees (handles the array of fees and penalties applicable to the current account facility)»* como Behavior Qualifier del Current Account Arrangement | Ningún verbo de los 19 le calza: «*fulfill* la tasa» no significa nada |
| **Un canal** (ventanilla, app, agencia) | Discriminador de **instancias**, no de funcionalidad | «Solo en ventanilla» = misma responsabilidad, menos casos |
| **Un segmento** (banca personas, pyme, corporativa) | Discriminador de instancias | Mismo patrón sobre el mismo activo, distinta población |
| **Un producto comercial** (crédito vehicular) | Condiciones del *arrangement* | Si dos productos comparten patrón y activo, no son dos activos |
| **Una etapa del ciclo de vida** (originación, cobranza) | Momento de la vida del mismo activo | Pasa la prueba del umbral y **falla** la del ciclo de vida |
| **Un área organizacional** (Gerencia de Operaciones) | Estructura, no función | El corte de BIAN es funcional, no organizacional |
| **Un sistema** (el core, el CRM) | Realización tecnológica | BIAN es agnóstico: el sistema realiza dominios, no los define |

---

## 7. Plantilla de trabajo para el taller

Para cada actividad del inventario AS-IS:

| # | Actividad AS-IS | ¿Qué comportamiento se ejecuta? (uno de los 19) | ¿Sobre qué activo actúa? | ¿Pasa el umbral? | ¿Cubre el ciclo de vida completo? | Control Record (AT + GA) | Service Domain candidato |
|---|---|---|---|---|---|---|---|
| 1 | | | | Sí / No — por qué | Sí / No — por qué | | |

**Reglas de llenado que conviene exigir:**

1. El patrón se elige **antes** que el activo. El umbral depende del par, no del activo aislado.
2. Si la respuesta a «¿pasa el umbral?» es *no*, se baja un escalón y se vuelve a empezar. No se anota el dominio.
3. Si la respuesta a «¿ciclo de vida completo?» es *no*, el candidato es una **etapa**, no un dominio. Se sube al activo que sí tiene vida propia.
4. El Control Record se escribe por **concatenación literal** de Asset Type + Generic Artifact, aunque suene raro. Si suena imposible de nombrar, casi siempre el activo está mal elegido.
5. Todo activo declarado **propio de la entidad** (extensión) se justifica por escrito con los dos criterios, como en los casos 3 y 5 de este documento.

---

## 8. Fuentes

**Literales**

- BIAN 2nd Edition — *A framework for the financial services industry*. Cap. 2, Secc. 2.4.1 (Functional Pattern), 2.4.2 (Generic Artifact), **2.4.3 (Asset Type y threshold of decomposition)**, 2.5 (Control Record e Information Profile), 2.5.2 (Behavior Qualifier Type).
- BIAN 2nd Edition. Figuras 2-8 (mapeo FP → GA), **2-9 (Current Account: FP, AT, GA)**, 2-11 (Control Record Party Reference Data Directory Entry), 2-25 (Service Operations sobre los niveles del Information Profile), 2-28 (Service Domain Overview Diagram de Current Account).
- BIAN 2nd Edition. Cap. 4, **Figuras 4-3 y 4-4** (tailoring del M5 Banking Group: generalización de préstamos y separación del Standing Order).
- Syllabus BIAN Foundation v3.8 — Tema 5, *Service Domains and their patterns*; *Control Record and Information Profile and their patterns*.

**Para verificar nomenclatura**

- Repositorio digital de BIAN: `bian.org/servicelandscape-14-0-0/` — el Asset Type aparece por Service Domain, no como árbol independiente.
- Portal de APIs semánticas: `portal.bian.org`

---

*Documento de apoyo del curso CD-03. Las marcas [LITERAL], [RECONSTRUIDO] y [SUPUESTO] son parte del material: se mantienen al citarlo o proyectarlo, para que el alumno distinga siempre qué es el estándar y qué es interpretación docente.*
