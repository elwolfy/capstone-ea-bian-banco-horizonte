# Caso de Negocio — Banco Horizonte

**Curso:** CD-03 · Arquitectura Bancaria basada en el Estándar BIAN® · CPS Tech
**Uso:** caso transversal del Proyecto Capstone. Este documento describe el banco **en lenguaje de negocio**; es el **insumo** a partir del cual, a lo largo de las sesiones, se construirán las vistas de arquitectura.

> **Aviso:** «Banco Horizonte» es una entidad **ficticia** creada con fines didácticos. Las referencias a ComproPago y SPIN se usan solo como ejemplos de mercado, públicamente conocidos, del tipo de producto que el caso menciona; no implican afiliación ni las representan.

---

## 1. El banco (reseña y misión)

Banco Horizonte es un **banco grande y tradicional del Perú, con 40 años de historia**. Nació como banca de personas y, con los años, amplió su alcance a empresas y a la pequeña y mediana empresa (pyme). Es una marca reconocida, con una amplia red de agencias a nivel nacional y una base de clientes construida a lo largo de cuatro décadas.

**Misión:** impulsar la inclusión y el progreso financiero de las personas, las empresas y las pymes del Perú, ofreciendo productos de crédito y ahorro confiables y una banca cada vez más simple, cercana y digital, que llegue tanto a quienes aún operan con efectivo como a quienes viven en el mundo 100 % digital.

Su tamaño y trayectoria son su fortaleza, pero también su reto: sus sistemas y su forma de operar fueron diseñados en otra época, cuando la agencia era el centro de todo, y hoy le cuesta moverse a la velocidad que el cliente digital exige.

---

## 2. Productos y segmentos de cliente

Los productos principales del banco son el **crédito** y el **ahorro**, dirigidos a tres grandes segmentos:

- **Personas:** cuentas de ahorro, créditos de consumo y tarjetas.
- **Empresas:** cuentas, financiamiento y servicios de pago.
- **Pymes:** ahorro y crédito para la pequeña y mediana empresa, un segmento clave para el crecimiento del país.

A estos se suma, de forma creciente, el cliente que opera por canales digitales.

---

## 3. Línea de innovación y la oportunidad

El banco ha creado una **línea de innovación** con dos focos claros, definidos por el comportamiento del cliente:

1. **Clientes no bancarizados que pagan en efectivo.** Personas que hoy no tienen (o no usan) una cuenta y realizan sus pagos de forma física. El banco busca acercarlos con soluciones simples de **pago y cobro en efectivo** a través de comercios y agentes, como puerta de entrada al sistema financiero (referencia de mercado: modelos tipo *ComproPago*).

2. **Clientes nativos digitales.** Personas que realizan **todas** sus transacciones desde el celular y esperan resolver todo sin pisar una agencia. Para ellos, el banco impulsa una **billetera digital** y una experiencia móvil completa (referencia de mercado: modelos tipo *SPIN*).

**La oportunidad.** Al trabajar el segmento nativo digital, el banco identifica una oportunidad mayor: si logra **consolidar su banca digital** (app móvil y banca web) hasta ofrecer una experiencia 100 % digital sólida, podría **capturar al cliente nativo digital de México y Brasil**, mercados grandes y con alta adopción digital, sin necesidad de abrir agencias. Esa es la ambición de crecimiento de largo plazo; su condición previa es tener, primero, una banca digital consolidada en Perú.

---

## 4. Modelo de Negocio (Business Model Canvas)

| Bloque | Contenido |
|---|---|
| **1. Segmentos de Cliente** | Personas; empresas; pymes; clientes no bancarizados que pagan en efectivo; clientes nativos digitales. *(Oportunidad: nativos digitales de México y Brasil.)* |
| **2. Propuesta de Valor** | Crédito y ahorro confiables; banca simple y cercana; pagos y transferencias inmediatos (Yape/Plin); pago y cobro en efectivo para no bancarizados; billetera y experiencia 100 % digital para nativos digitales. |
| **3. Canales** | Red de agencias; agentes / corresponsales en comercios; app móvil y banca web; contact center. |
| **4. Relación con el Cliente** | Atención en agencia; autoservicio digital; soporte omnicanal; acompañamiento a empresas y pymes. |
| **5. Fuentes de Ingreso** | Intereses de créditos; comisiones de pagos, transferencias y servicios; mantenimiento de cuentas; comisiones de red de agentes. |
| **6. Recursos Clave** | Licencia bancaria (SBS); red de agencias y de agentes; plataforma tecnológica y app; base de clientes e información; equipo humano y línea de innovación. |
| **7. Actividades Clave** | Otorgar y administrar créditos; captar ahorro; procesar pagos; atender y vincular clientes; gestionar riesgo y cumplimiento; operar los canales. |
| **8. Socios Clave** | Comercios y agentes corresponsales; cámara de compensación e interoperabilidad de pagos (BCRP); proveedores tecnológicos; centrales de riesgo; reguladores. |
| **9. Estructura de Costos** | Red de agencias y agentes; tecnología e infraestructura; personal; cumplimiento, riesgo y seguridad; captación de clientes. |

---

## 5. Marco legal y regulatorio (Perú)

El banco opera bajo la supervisión y las normas del sistema financiero peruano. Este marco es un **insumo** del caso, porque condiciona lo que el banco puede y debe hacer:

- **SBS** (Superintendencia de Banca, Seguros y AFP) — Ley N° 26702: autorización, solvencia y supervisión.
- **BCRP** — política de encaje e **interoperabilidad de pagos inmediatos** (Yape/Plin).
- **Basilea III** y **provisiones dinámicas** — requerimientos de capital y provisiones por riesgo de crédito.
- **Ley N° 29985 (Dinero Electrónico)** — base para billeteras y valor almacenado.
- **UIF** — prevención del lavado de activos (PLAFT).
- **Ley N° 29733** — protección de datos personales.
- **DL 1531 y normas de seguridad de la información (SBS)** — ciberseguridad.
- **Reglamento de cajeros corresponsales (SBS)** — operación a través de agentes.

*(La expansión a México y Brasil implicará, en su momento, cumplir los marcos de esos países; se considera solo como horizonte de largo plazo.)*

---

## 6. Lo que hace el banco (funciones de negocio)

En lenguaje de negocio, el banco realiza hoy, de forma cotidiana, estas grandes funciones:

- **Atender y vincular clientes:** dar de alta a un cliente, conocerlo (identidad y documentos) y mantener su información y su relación con el banco.
- **Otorgar y administrar créditos:** recibir solicitudes, evaluar la capacidad de pago, aprobar, definir condiciones, desembolsar y luego administrar y cobrar el crédito.
- **Captar ahorro:** abrir y operar cuentas de ahorro y depósitos para personas, empresas y pymes.
- **Procesar pagos y transferencias:** ejecutar pagos, transferencias y desembolsos, incluidos los pagos inmediatos.
- **Operar los canales:** agencias, agentes/corresponsales, app móvil, banca web y contact center.
- **Gestionar riesgo y cobranzas:** controlar el riesgo de crédito y recuperar la cartera.
- **Cumplir la regulación:** prevención de lavado, protección de datos, seguridad y reportes al regulador.
- **Administrar las finanzas:** contabilidad, tesorería y reportes financieros.
- **Sostener la tecnología:** los sistemas y la plataforma que soportan todo lo anterior.
- **Innovar:** crear nuevas soluciones para no bancarizados y para nativos digitales.

Estas funciones describen **qué** hace el banco; no son todavía un artefacto de arquitectura. Ordenarlas y estructurarlas formalmente será parte del trabajo de las sesiones.

---

## 7. Procesos principales (en lenguaje de negocio)

Así vive el cliente los procesos más importantes del banco hoy:

- **Hacerse cliente (vinculación).** La persona se acerca a una agencia o entra a la app, entrega sus datos y documentos; el banco valida su identidad y la habilita para operar. Hoy es un trámite con varios pasos y, a veces, presencial.

- **Pedir y recibir un crédito.** El cliente solicita un crédito; el banco evalúa su capacidad de pago, decide, define las condiciones (monto, plazo, tasa), formaliza el contrato y realiza el desembolso. Hoy la evaluación es lenta y poco predecible.

- **Ahorrar.** El cliente abre una cuenta de ahorro con ciertas condiciones y luego realiza depósitos y retiros por los distintos canales.

- **Pagar y transferir.** El cliente da la orden de un pago o transferencia; el banco la valida y la ejecuta según lo pactado, y la registra. Se espera que sea inmediato.

- **Operar a través de un agente / corresponsal.** En una bodega o comercio afiliado, el cliente deposita, retira o paga. Hoy estas operaciones se terminan de reflejar en el banco recién al día siguiente.

- **Pagar en efectivo sin ser cliente (no bancarizados).** Una persona sin cuenta paga o cobra en efectivo en un punto físico usando una referencia; es la puerta de entrada que la línea de innovación quiere abrir.

Estos relatos de proceso son el **insumo** sobre el que, en las sesiones, se detallarán las actividades y se diseñarán las mejoras.

---

## 8. Assessment de co-creación (fase Discovery)

En la fase **Discovery** se realizaron talleres de **co-creación** con las áreas de negocio, operaciones, tecnología, riesgos, cumplimiento y la línea de innovación: se exploró el problema y se identificaron oportunidades. El resultado se resume en dos listas, cada elemento con un **identificador único**. Estas listas son el sustento de negocio para las decisiones de las siguientes sesiones.

### 8.1 Hallazgos y problemas (`H-##`)

| ID | Hallazgo (en palabras del negocio) |
|---|---|
| **H-01** | Abrir una cuenta o pedir un crédito toma demasiado tiempo y pasos. |
| **H-02** | La información del cliente está dispersa; se le piden los mismos datos una y otra vez. |
| **H-03** | La app y la banca web dejan consultar, pero no realizar la mayoría de operaciones. |
| **H-04** | Los pagos y depósitos hechos en agentes se reflejan recién al día siguiente. |
| **H-05** | Lanzar o modificar un producto (tasas, condiciones) toma meses. |
| **H-06** | La evaluación de un crédito es lenta y poco predecible. |
| **H-07** | Los reportes de contabilidad y de cumplimiento no siempre cuadran entre sí. |
| **H-08** | Cada nuevo canal o alianza exige integraciones costosas y frágiles. |
| **H-09** | Los no bancarizados no tienen una forma simple de pagar y cobrar en efectivo con el banco. |
| **H-10** | Los clientes nativos digitales esperan una experiencia 100 % digital que hoy no está completa. |
| **H-11** | Los datos no están ordenados para explotarlos con analítica o inteligencia artificial. |
| **H-12** | Cambiar la tecnología es caro y riesgoso, lo que frena la estrategia. |

### 8.2 Oportunidades de solución (`O-##`)

| ID | Oportunidad | Responde a |
|---|---|---|
| **O-01** | Vinculación (onboarding) 100 % digital, rápida y sin repetir datos. | H-01, H-02 |
| **O-02** | Una sola vista confiable de la información del cliente. | H-02 |
| **O-03** | App y banca web que permitan operar de extremo a extremo. | H-03, H-10 |
| **O-04** | Pagos y depósitos en tiempo real, incluidos los de agentes. | H-04 |
| **O-05** | Catálogo de productos configurable para lanzar/ajustar en días. | H-05 |
| **O-06** | Evaluación de crédito más rápida y consistente. | H-06 |
| **O-07** | Una base única y confiable de operaciones para contabilidad y cumplimiento. | H-07 |
| **O-08** | Solución de pago y cobro en efectivo para no bancarizados. | H-09 |
| **O-09** | Billetera digital para nativos digitales, base para crecer a México y Brasil. | H-10 |
| **O-10** | Ordenar los datos para habilitar analítica e inteligencia artificial. | H-11 |
| **O-11** | Modernizar la tecnología para poder cambiar rápido y con menor riesgo. | H-08, H-12 |

---

## 9. Del caso a la arquitectura (nota pedagógica)

Todo lo anterior —la misión, el modelo de negocio, el marco regulatorio, las funciones, los procesos y el assessment de co-creación— es el **insumo de negocio** del proyecto. A lo largo de las sesiones se irá transformando, de manera pedagógica, en **vistas de arquitectura empresarial**, para mostrar cómo se usan la arquitectura empresarial y el estándar BIAN.

En el **Módulo 1** se elaboran, a partir de este caso, la **vista motivacional**, la **vista de capacidades** y la **vista estratégica**. El proyecto se construye en un **repositorio ArchiMate en GitHub que se actualiza en cada sesión**.

---

### Estado del caso (para tu aprobación)
- **Banco:** ✅ grande y tradicional, Perú, 40 años; productos crédito y ahorro para personas, empresas y pymes.
- **Innovación:** ✅ no bancarizados (pago en efectivo) + nativos digitales (billetera/100 % digital).
- **Oportunidad:** ✅ consolidar la banca digital y capturar nativos digitales de México y Brasil.
- **Lenguaje:** ✅ de negocio; sin desarrollar capacidades ni dominios de servicio (se construyen en las sesiones).
- **Insumos:** ✅ misión, modelo de negocio (Canvas), marco regulatorio, funciones, procesos y assessment (H/O con IDs).
- **Siguiente paso (con tu aprobación):** construir el script del mapa de capacidades del caso.
