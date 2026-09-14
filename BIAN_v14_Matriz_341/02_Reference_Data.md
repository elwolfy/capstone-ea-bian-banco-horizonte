# Reference Data

**BIAN Service Landscape V14.0 · vista Matrix** — 33 Service Domains

> Curso independiente de CPS Tech · No afiliado ni acreditado por BIAN e.V. · BIAN® es marca registrada de BIAN e.V., usada con fines descriptivos.

[← Volver al índice de los 341](README.md)

---

## Contenido

**Party** · 2

[Party Routing Profile](#party-routing-profile) · [Legal Entity Directory](#legal-entity-directory)

**External Agency** · 13

[Information Provider Administration](#information-provider-administration) · [Syndicate Management](#syndicate-management) · [Interbank Relationship Management](#interbank-relationship-management) · [Correspondent Bank Relationship Management](#correspondent-bank-relationship-management) · [Correspondent Bank Directory](#correspondent-bank-directory) · [Sub Custodian Agreement](#sub-custodian-agreement) · [Product Service Agency](#product-service-agency) · [Partner Agreement](#partner-agreement) · [Contractor and Supplier Agreement](#contractor-and-supplier-agreement) · [Service Provider Operations](#service-provider-operations) · [Partner Management](#partner-management) · [Operations Log](#operations-log) · [Partner Administration](#partner-administration)

**Market Data** · 11

[Information Provider Operation](#information-provider-operation) · [Market Information Management](#market-information-management) · [Financial Market Analysis](#financial-market-analysis) · [Financial Market Research](#financial-market-research) · [Quant Model](#quant-model) · [Market Data Switch Administration](#market-data-switch-administration) · [Market Data Switch Operation](#market-data-switch-operation) · [Financial Instrument Reference Data Management](#financial-instrument-reference-data-management) · [Counterparty Administration](#counterparty-administration) · [Public Reference Data Management](#public-reference-data-management) · [Location Data Management](#location-data-management)

**Product Management** · 7

[Product Design](#product-design) · [Product Deployment](#product-deployment) · [Product Training](#product-training) · [Product Quality Assurance](#product-quality-assurance) · [Discount Pricing](#discount-pricing) · [Product Directory](#product-directory) · [Special Pricing Conditions](#special-pricing-conditions)

---

## Party Routing Profile

| | |
|---|---|
| **Patrón funcional** | `Monitor` |
| **Tipo de activo** | `Party` |
| **Artefacto genérico** | `State` |
| **Control Record** | `Party State` |
| **Ubicación Matrix** | Reference Data › Party |

**Propósito.** This service domain maintains a small profile of key indicators for a customer that is referenced during customer interactions to facilitate routing, servicing and product/service fulfillment decisions. This can include status (such as account in arrears), ratings (such as high value customer) and alerts (such possible fraud activity detected)

<details><summary><b>Atributos del Control Record</b> · 1</summary>

`Customer Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Status | 4 |
| Rating | 4 |
| Alert | 4 |

**Interfaz.** Action Terms: `Initiate` · `Request` · `Update` · `Capture` · `Retrieve` · `Control` · `Execute` · `Exchange` · `Notify` · `Evaluate`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 18 | 9 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Request` · `Update` · `Retrieve` · `Control` · `Execute` |
| BQ `Status` | `Update` · `Retrieve` · `Capture` · `Notify` · `Evaluate` |
| BQ `Rating` | `Capture` · `Retrieve` · `Update` |
| BQ `Alert` | `Update` · `Capture` · `Exchange` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Legal Entity Directory

| | |
|---|---|
| **Patrón funcional** | `Catalog` |
| **Tipo de activo** | `Legal Entity` |
| **Artefacto genérico** | `Directory Entry` |
| **Control Record** | `Legal Entity Directory Entry` |
| **Ubicación Matrix** | Reference Data › Party |

**Propósito.** This service domain maintains details of the legal entity structure of the party including dependents and associations for individuals and ownership/subsidiary structures for corporations. Some financial indicators and product coverage/activity details can be included where this defines the nature of the legal entity relationship in particular for corporate entities

<details><summary><b>Atributos del Control Record</b> · 4</summary>

`Legal Entity Reference` · `Party Reference` · `Directory Entry Date Type` · `Directory Entry Date`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Reference | 12 |
| Profile | 6 |
| Associations | 6 |

**Interfaz.** Action Terms: `Register` · `Control` · `Update` · `Exchange` · `Request` · `Retrieve` · `Execute`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 13 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Register` · `Control` · `Update` · `Exchange` · `Request` · `Execute` · `Retrieve` |
| BQ `Reference` | `Retrieve` · `Update` |
| BQ `Profile` | `Retrieve` · `Update` |
| BQ `Associations` | `Update` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Information Provider Administration

| | |
|---|---|
| **Patrón funcional** | `Agree Terms` |
| **Tipo de activo** | `Information Feed` |
| **Artefacto genérico** | `Agreement` |
| **Control Record** | `Information Feed Agreement` |
| **Ubicación Matrix** | Reference Data › External Agency |

[↑ Índice](README.md)

---

## Syndicate Management

| | |
|---|---|
| **Patrón funcional** | `Enroll` |
| **Tipo de activo** | `Syndicate` |
| **Artefacto genérico** | `Membership` |
| **Control Record** | `Syndicate Membership` |
| **Ubicación Matrix** | Reference Data › External Agency |

**Propósito.** This Service Domain manages syndicate membership and compliance

<details><summary><b>Atributos del Control Record</b> · 7</summary>

`Parameter Type` · `Selected Option` · `Request` · `Plan` · `Obligation` · `Entitlement` · `Reference`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Syndicate Compliance Clauses | 8 |
| Syndicate Eligibility Clauses | 8 |

**Interfaz.** Action Terms: `Grant` · `Notify` · `Control` · `Request` · `Register` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 13 | 11 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Grant` · `Notify` · `Control` · `Request` · `Register` · `Retrieve` · `Update` |
| BQ `Syndicate Compliance Clauses` | `Notify` · `Retrieve` · `Update` |
| BQ `Syndicate Eligibility Clauses` | `Notify` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Interbank Relationship Management

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `Bank Relationship` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `Bank Relationship Management Plan` |
| **Ubicación Matrix** | Reference Data › External Agency |

**Propósito.** Manage the bank

<details><summary><b>Atributos del Control Record</b> · 7</summary>

`Bank Reference` · `Bank Details` · `Employee or Business Unit Reference` · `Bank Relationship Type` · `Bank Relationship Description` · `Bank Relationship Budget` · `Bank Contact Details`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Contact | 8 |

**Interfaz.** Action Terms: `Create` · `Update` · `Control` · `Exchange` · `Request` · `Grant` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 11 | 4 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Create` · `Update` · `Control` · `Exchange` · `Request` · `Grant` · `Retrieve` |
| BQ `Contact` | `Create` · `Update` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Correspondent Bank Relationship Management

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `Correpondent Bank Relationship` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `Correpondent Bank Relationship Management Plan` |
| **Ubicación Matrix** | Reference Data › External Agency |

**Propósito.** This Service Domain manages correspondent bank relations, ensuring reciprocity and developing business where possible

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Type` · `Reference` · `Budget Type` · `Budget` · `Assignment` · `Duty` · `Description` · `BudgetBalance` · `Associated Party` · `Subject Matter`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Incident Troubleshooting Oversight | 8 |
| Relationship Development | 8 |
| Relationship Reciprocity Assessment | 8 |

**Interfaz.** Action Terms: `Control` · `Create` · `Exchange` · `Notify` · `Grant` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 26 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Create` · `Exchange` · `Notify` · `Grant` · `Request` · `Retrieve` · `Update` |
| BQ `Relationship Reciprocity Assessment` | `Exchange` · `Retrieve` · `Grant` · `Notify` · `Request` · `Update` |
| BQ `Incident Troubleshooting Oversight` | `Grant` · `Exchange` · `Notify` · `Retrieve` · `Request` · `Update` |
| BQ `Relationship Development` | `Exchange` · `Notify` · `Request` · `Update` · `Grant` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Correspondent Bank Directory

| | |
|---|---|
| **Patrón funcional** | `Catalog` |
| **Tipo de activo** | `Correspondent Bank` |
| **Artefacto genérico** | `Directory Entry` |
| **Control Record** | `Correspondent Bank Directory Entry` |
| **Ubicación Matrix** | Reference Data › External Agency |

**Propósito.** This service domain maintains correspondent bank reference details

<details><summary><b>Atributos del Control Record</b> · 16</summary>

`Correspondent Bank Reference` · `Contact Addresses` · `Vostro Account Reference` · `Correspondent Bank Agreement Reference` · `Correspondent Bank Name` · `BIC` · `National Clearing Code` · `Correspondent Bank Contact Address` · `Party Reference Data Directory Reference` · `Legal Entity Directory Reference` · `Payment Processing Times` · `Nostro Account Reference` · `Related Beneficiary Bank Reference` · `Related Beneficiary Bank BIC` · `Related Beneficiary Bank Name` · `Related Beneficiary Bank Currency Reference`

</details>

**Interfaz.** Action Terms: `Register` · `Update` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 4 | 2 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Register` · `Update` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Sub Custodian Agreement

| | |
|---|---|
| **Patrón funcional** | `Agree Terms` |
| **Tipo de activo** | `Sub Custodian` |
| **Artefacto genérico** | `Agreement` |
| **Control Record** | `Sub Custodian Agreement` |
| **Ubicación Matrix** | Reference Data › External Agency |

**Propósito.** This Service Domain establishes and maintains the terms governing sub custodian relationship

<details><summary><b>Atributos del Control Record</b> · 19</summary>

`Parameter Type` · `Selected Option` · `Type` · `Reference` · `Discharge Request` · `Discharge Schedule` · `Status` · `Associated Party` · `Customer Reference` · `Obligation` · `Entitlement` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Account Reference` · `Subject Matter` · `Product Reference` · `Calendar Reference` · `Associated Agreement Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Policy Term | 9 |
| Regulatory Term | 9 |
| Legal Term | 9 |

**Interfaz.** Action Terms: `Control` · `Evaluate` · `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 26 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Evaluate` · `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Legal Term` | `Evaluate` · `Exchange` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Policy Term` | `Evaluate` · `Exchange` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Regulatory Term` | `Evaluate` · `Exchange` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Product Service Agency

| | |
|---|---|
| **Patrón funcional** | `Agree Terms` |
| **Tipo de activo** | `Service Provider` |
| **Artefacto genérico** | `Agreement` |
| **Control Record** | `Service Provider Agreement` |
| **Ubicación Matrix** | Reference Data › External Agency |

**Propósito.** This Service Domain establishes and maintains contractual arrangements with product and service agencies

<details><summary><b>Atributos del Control Record</b> · 19</summary>

`Parameter Type` · `Selected Option` · `Type` · `Reference` · `Discharge Request` · `Discharge Schedule` · `Status` · `Associated Party` · `Customer Reference` · `Obligation` · `Entitlement` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Account Reference` · `Subject Matter` · `Product Reference` · `Calendar Reference` · `Associated Agreement Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Policy Term | 9 |
| Regulatory Term | 9 |
| Legal Term | 9 |

**Interfaz.** Action Terms: `Control` · `Evaluate` · `Exchange` · `Grant` · `Request` · `Notify` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 26 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Evaluate` · `Exchange` · `Grant` · `Request` · `Notify` · `Retrieve` · `Update` |
| BQ `Legal Term` | `Evaluate` · `Exchange` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Policy Term` | `Evaluate` · `Exchange` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Regulatory Term` | `Evaluate` · `Exchange` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Partner Agreement

| | |
|---|---|
| **Patrón funcional** | `Agree Terms` |
| **Tipo de activo** | `Partner` |
| **Artefacto genérico** | `Agreement` |
| **Control Record** | `Partner Agreement` |
| **Ubicación Matrix** | Reference Data › External Agency |

**Propósito.** This service domain captures and maintains comprehensive terms and conditions govering Partner relationships.

<details><summary><b>Atributos del Control Record</b> · 6</summary>

`Party Reference` · `Agreement Type` · `Agreement Jurisdiction` · `Agreement Valid From/To Date` · `Agreement Signatures/Responsible Parties` · `Document Directory Entry Instance Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Legal Term | 3 |
| Regulatory Term | 3 |
| Policy Term | 3 |

**Interfaz.** Action Terms: `Exchange` · `Update` · `Control` · `Evaluate` · `Request` · `Grant` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 16 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Exchange` · `Update` · `Control` · `Evaluate` · `Request` · `Grant` · `Retrieve` |
| BQ `Legal Term` | `Evaluate` · `Retrieve` · `Update` |
| BQ `Regulatory Term` | `Evaluate` · `Update` · `Retrieve` |
| BQ `Policy Term` | `Evaluate` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Contractor and Supplier Agreement

| | |
|---|---|
| **Patrón funcional** | `Agree Terms` |
| **Tipo de activo** | `Supplier` |
| **Artefacto genérico** | `Agreement` |
| **Control Record** | `Supplier Agreement` |
| **Ubicación Matrix** | Reference Data › External Agency |

**Propósito.** This Service Domain maintains appropriate supplier agreements/contracts

<details><summary><b>Atributos del Control Record</b> · 19</summary>

`Parameter Type` · `Selected Option` · `Type` · `Reference` · `Discharge Request` · `Discharge Schedule` · `Status` · `Associated Party` · `Customer Reference` · `Obligation` · `Entitlement` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Account Reference` · `Subject Matter` · `Product Reference` · `Calendar Reference` · `Associated Agreement Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Policy Term | 9 |
| Legal Term | 9 |
| Regulatory Term | 9 |

**Interfaz.** Action Terms: `Control` · `Evaluate` · `Exchange` · `Grant` · `Notify` · `Update` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 26 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Evaluate` · `Exchange` · `Grant` · `Notify` · `Update` · `Request` · `Retrieve` |
| BQ `Legal Term` | `Evaluate` · `Exchange` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Policy Term` | `Evaluate` · `Exchange` · `Notify` · `Request` · `Update` · `Retrieve` |
| BQ `Regulatory Term` | `Evaluate` · `Exchange` · `Notify` · `Retrieve` · `Request` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Service Provider Operations

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `Service Provider Registration` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `Service Provider Registration Operating Session` |
| **Ubicación Matrix** | Reference Data › External Agency |

**Propósito.** This Service Domain handles the range of operational actions used in production interactions with an external service provider.

<details><summary><b>Atributos del Control Record</b> · 4</summary>

`Service Provider Registration Reference` · `Reference` · `Service Provider Reference` · `TPP Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Tokens | 10 |
| Data Sharing Consents Instance Recoed | 9 |
| Customer Requests | 1 |

**Interfaz.** Action Terms: `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 1 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Partner Management

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `Partner Releationship` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `Partner Releationship Management Plan` |
| **Ubicación Matrix** | Reference Data › External Agency |

**Propósito.** This service domain handles strategic management of collaborative partners including partner development, performance and relationship tracking.

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Type` · `Reference` · `Budget Type` · `Budget` · `Assignment` · `Duty` · `Description` · `BudgetBalance` · `Associated Party` · `Subject Matter`

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Operations Log

| | |
|---|---|
| **Patrón funcional** | `Track` |
| **Tipo de activo** | `Partner Event` |
| **Artefacto genérico** | `Log` |
| **Control Record** | `Partner Event Log` |
| **Ubicación Matrix** | Reference Data › External Agency |

**Propósito.** This service domain handle the day-to-day operations of a collaborative partner related services.

<details><summary><b>Atributos del Control Record</b> · 14</summary>

`Parameter Type` · `Selected Option` · `Type` · `Schedule` · `Usage Log` · `Update Log` · `Associated Party` · `Business Unit Reference` · `Customer Reference` · `Service Configuration` · `Position` · `Position Type` · `Position Limit Time` · `Reference`

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Partner Administration

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Partner` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Partner Administrative Plan` |
| **Ubicación Matrix** | Reference Data › External Agency |

**Propósito.** This service domain handle the day-to-day operations of a collaborative partner related services.

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Budget Type` · `Budget` · `Assignment` · `Duty` · `Associated Party` · `Budget Balance` · `Subject Matter` · `Type` · `Reference` · `Description`

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Information Provider Operation

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `Information Feed` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `Information Feed Operating Session` |
| **Ubicación Matrix** | Reference Data › Market Data |

**Propósito.** Operate the interfaces to external information feed services

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Schedule` · `Status` · `Usage Log` · `Associated Party Reference` · `Service Provider Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Service Configuration` · `Reference`

</details>

**Interfaz.** Action Terms: `Initiate` · `Retrieve` · `Execute` · `Update` · `Control` · `Request` · `Exchange` · `Notify`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 8 | 5 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Retrieve` · `Execute` · `Update` · `Control` · `Request` · `Exchange` · `Notify` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Market Information Management

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Financial Market Information` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Financial Market Information Administrative Plan` |
| **Ubicación Matrix** | Reference Data › Market Data |

**Propósito.** Market information management consolidates and improves market information from multiple sources in order to build up a bank knowledge base in targeted areas

<details><summary><b>Atributos del Control Record</b> · 11</summary>

`Financial Market Information Service` · `Financial Market Information Provider` · `Financial Market information Description` · `Financial Market Information Service Type` · `Financial Market Information Service Schedule` · `Financial Market Information Service Agreement` · `Financial Market Information Database` · `Financial Market Information Subject Area` · `Financial Market Information Subject Area Description` · `Financial Market Information Subject Area Update History` · `Financial Market Information Subject Area Record`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Consolidation | 2 |
| Improvement | 4 |
| Reporting | 5 |

**Interfaz.** Action Terms: `Update` · `Exchange` · `Execute` · `Request` · `Retrieve` · `Capture` · `Create` · `Control` · `Grant`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 16 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Update` · `Exchange` · `Execute` · `Request` · `Create` · `Control` · `Grant` · `Retrieve` |
| BQ `Improvement` | `Retrieve` |
| BQ `Reporting` | `Update` · `Capture` · `Execute` · `Request` · `Create` · `Retrieve` |
| BQ `Consolidation` | `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Financial Market Analysis

| | |
|---|---|
| **Patrón funcional** | `Analyze` |
| **Tipo de activo** | `Financial Market` |
| **Artefacto genérico** | `Analysis` |
| **Control Record** | `Financial Market Analysis` |
| **Ubicación Matrix** | Reference Data › Market Data |

**Propósito.** Provide different types of financial market analysis using available financial market information and research

<details><summary><b>Atributos del Control Record</b> · 7</summary>

`Parameter Type` · `Selected Option` · `Request` · `Schedule` · `Status` · `Usage Log` · `Requester Reference`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Financial Market Insight | 4 |

**Interfaz.** Action Terms: `Execute` · `Retrieve` · `Initiate` · `Request` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 10 | 6 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Execute` · `Retrieve` · `Initiate` · `Request` · `Update` |
| BQ `Financial Market Insight` | `Execute` · `Update` · `Retrieve` · `Request` · `Initiate` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Financial Market Research

| | |
|---|---|
| **Patrón funcional** | `Catalog` |
| **Tipo de activo** | `Financial Market Research` |
| **Artefacto genérico** | `Directory Entry` |
| **Control Record** | `Financial Market Research Directory Entry` |
| **Ubicación Matrix** | Reference Data › Market Data |

**Propósito.** The service domain consolidates external financial market research

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Financial Market Research Viewpoint Type` · `Financial Market Research Viewpoint Description` · `Referenced Financial Market Research Record` · `Financial Market Research Report Type Reference` · `Financial Market Research Report Type Definition` · `Financial Market Research Report Version/Period` · `Financial Market Research Report` · `Financial Market Research Viewpoint Usage` · `Financial Market Research Report Request` · `Employee or Business Unit Reference`

</details>

**Interfaz.** Action Terms: `Register` · `Update` · `Execute` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 5 | 2 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Register` · `Update` · `Execute` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Quant Model

| | |
|---|---|
| **Patrón funcional** | `Design` |
| **Tipo de activo** | `Quant Model` |
| **Artefacto genérico** | `Specification` |
| **Control Record** | `Quant Model Specification` |
| **Ubicación Matrix** | Reference Data › Market Data |

[↑ Índice](README.md)

---

## Market Data Switch Administration

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Information Feed Switch` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Information Feed Switch Administrative Plan` |
| **Ubicación Matrix** | Reference Data › Market Data |

[↑ Índice](README.md)

---

## Market Data Switch Operation

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `Information Feed Switch` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `Information Feed Switch Operating Session` |
| **Ubicación Matrix** | Reference Data › Market Data |

**Propósito.** This service domain operates the internal information distribution facility/switch in compliance with administered external subscription information feed service access rights. Note the content is retrieved by the Market Feed Operation service domain from the various external feed services. Internal information can also be published over the switch from various bank sources (such as bank rates provided by treasury).

<details><summary><b>Atributos del Control Record</b> · 2</summary>

`Market Information Feed Service Reference` · `Market Information Feed Service Profile`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Feed Upload | 2 |
| Internal Publication | 4 |
| Distribution | 3 |

**Interfaz.** Action Terms: `Update` · `Initiate` · `Control` · `Execute` · `Retrieve` · `Request` · `Exchange`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 18 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Update` · `Initiate` · `Control` · `Execute` · `Retrieve` · `Request` |
| BQ `Feed Upload` | `Update` · `Exchange` · `Retrieve` |
| BQ `Internal Publication` | `Update` · `Initiate` · `Exchange` · `Retrieve` |
| BQ `Distribution` | `Initiate` · `Retrieve` · `Request` · `Update` · `Execute` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Financial Instrument Reference Data Management

| | |
|---|---|
| **Patrón funcional** | `Catalog` |
| **Tipo de activo** | `Financial Instrument` |
| **Artefacto genérico** | `Directory Entry` |
| **Control Record** | `Financial Instrument Directory Entry` |
| **Ubicación Matrix** | Reference Data › Market Data |

**Propósito.** This Service Domain maintains a directory of financial instrument reference data

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Description` · `Schedule` · `Version` · `Status` · `Usage Log` · `Update Log` · `Service Configuration` · `Reference` · `Financial Instrument Reference` · `Financial Market Reference`

</details>

**Behavior Qualifiers** · 6

| Behavior Qualifier | Atributos |
|---|---:|
| Warrant | 7 |
| Futures | 7 |
| Option | 7 |
| Equity | 7 |
| Debt Instrument | 7 |
| Currency | 14 |

**Interfaz.** Action Terms: `Control` · `Execute` · `Notify` · `Register` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 40 | 22 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Execute` · `Notify` · `Register` · `Request` · `Retrieve` · `Update` |
| BQ `Debt Instrument` | `Execute` · `Notify` · `Register` · `Request` · `Retrieve` · `Update` |
| BQ `Equity` | `Execute` · `Notify` · `Register` · `Request` · `Update` · `Retrieve` |
| BQ `Futures` | `Execute` · `Notify` · `Register` · `Request` · `Retrieve` · `Update` |
| BQ `Option` | `Execute` · `Notify` · `Register` · `Request` · `Retrieve` · `Update` |
| BQ `Warrant` | `Execute` · `Notify` · `Register` · `Request` · `Retrieve` · `Update` |
| BQ `Currency` | `Register` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Counterparty Administration

| | |
|---|---|
| **Patrón funcional** | `Catalog` |
| **Tipo de activo** | `Counterparty` |
| **Artefacto genérico** | `Directory Entry` |
| **Control Record** | `Counterparty Directory Entry` |
| **Ubicación Matrix** | Reference Data › Market Data |

**Propósito.** This Service Domain maintains key counterparty reference information used in the clearing and settlement of wholesale trading

<details><summary><b>Atributos del Control Record</b> · 11</summary>

`Description` · `Schedule` · `Version` · `Status` · `Usage Log` · `Update Log` · `Service Configuration` · `Reference` · `Conterparty Reference` · `Agreement Reference` · `Financial Transaction Reference`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Counterparty Permitted Transaction | 7 |
| Counterparty Entity Reference | 7 |

**Interfaz.** Action Terms: `Control` · `Execute` · `Register` · `Request` · `Notify` · `Update` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 19 | 11 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Execute` · `Register` · `Request` · `Notify` · `Update` · `Retrieve` |
| BQ `Counterparty Entity Reference` | `Notify` · `Request` · `Register` · `Execute` · `Retrieve` · `Update` |
| BQ `Counterparty Permitted Transaction` | `Execute` · `Notify` · `Register` · `Retrieve` · `Request` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Public Reference Data Management

| | |
|---|---|
| **Patrón funcional** | `Design` |
| **Tipo de activo** | `Global Standard` |
| **Artefacto genérico** | `Specification` |
| **Control Record** | `Global Standard Specification` |
| **Ubicación Matrix** | Reference Data › Market Data |

**Propósito.** Provide structured access to standard

<details><summary><b>Atributos del Control Record</b> · 8</summary>

`Parameter Type` · `Selected Option` · `Description` · `Version` · `Status` · `Usage Log` · `Feedback` · `Service Provider Reference`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Global Reference Data | 4 |

**Interfaz.** Action Terms: `Capture` · `Control` · `Initiate` · `Exchange` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 9 | 6 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Capture` · `Control` · `Initiate` · `Exchange` · `Request` · `Retrieve` · `Update` |
| BQ `Global Reference Data` | `Initiate` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Location Data Management

| | |
|---|---|
| **Patrón funcional** | `Catalog` |
| **Tipo de activo** | `Location` |
| **Artefacto genérico** | `Directory Entry` |
| **Control Record** | `Location Directory Entry` |
| **Ubicación Matrix** | Reference Data › Market Data |

**Propósito.** This service domain maintain details of the use and state of locations of interest to the bank. This can include both physical and virtual addresses. It is used to check for valid use and for sales/marketing activities

<details><summary><b>Atributos del Control Record</b> · 3</summary>

`Location Reference` · `Directory Entry Date Type` · `Directory Entry Date`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Use | 2 |
| Occupancy | 7 |
| Location | 8 |

**Interfaz.** Action Terms: `Register` · `Update` · `Control` · `Request` · `Retrieve` · `Execute` · `Exchange`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 14 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Register` · `Update` · `Control` · `Request` · `Retrieve` · `Execute` · `Exchange` |
| BQ `Location` | `Update` · `Exchange` · `Retrieve` |
| BQ `Use` | `Update` · `Retrieve` |
| BQ `Occupancy` | `Update` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Product Design

| | |
|---|---|
| **Patrón funcional** | `Design` |
| **Tipo de activo** | `Product and Service` |
| **Artefacto genérico** | `Specification` |
| **Control Record** | `Productor Service Specification` |
| **Ubicación Matrix** | Reference Data › Product Management |

**Propósito.** Develop/refine product designs and supporting specification details

<details><summary><b>Atributos del Control Record</b> · 12</summary>

`ProductandService Type` · `ProductandService Description` · `ProductandService Specification Deployment` · `Employee or Business Unit Reference` · `ProductandService Specification Deployment Configuration` · `ProductandService Specification Deployment Task Reference` · `ProductandService Specification Deployment Task Record` · `ProductandService Specification Status` · `ProductandService Specification Usage` · `ProductandService Specification Impact` · `ProductandService Specification Version` · `ProductandService Specification`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Functional Requirements | 6 |
| Testing | 10 |
| Production | 3 |

**Interfaz.** Action Terms: `Create` · `Execute` · `Request` · `Retrieve` · `Update` · `Exchange` · `Capture`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 15 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Create` · `Execute` · `Request` · `Retrieve` |
| BQ `Functional Requirements` | `Update` · `Exchange` · `Capture` · `Retrieve` · `Request` |
| BQ `Testing` | `Update` · `Retrieve` · `Exchange` |
| BQ `Production` | `Execute` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Product Deployment

| | |
|---|---|
| **Patrón funcional** | `Develop` |
| **Tipo de activo** | `Productand Service Deployment` |
| **Artefacto genérico** | `Development` |
| **Control Record** | `Productand Service Deployment Development` |
| **Ubicación Matrix** | Reference Data › Product Management |

**Propósito.** Plan and administer the production deployment new and updated products and services

<details><summary><b>Atributos del Control Record</b> · 9</summary>

`ProductandService Deployment Project Name` · `ProductandService Deployment Project Type` · `ProductandService Deployment Project Description` · `ProductandService Deployment Implementation Plan` · `ProductandService Deployment Budget` · `ProductandService Deployment Organization` · `ProductandService Deployment Schedule` · `Date Type` · `Date`

</details>

**Behavior Qualifiers** · 7

| Behavior Qualifier | Atributos |
|---|---:|
| Systems | 4 |
| IT Operations | 4 |
| HR Operations | 4 |
| Sales and Marketing | 4 |
| Servicing | 4 |
| Production | 4 |
| Production Support | 4 |

**Interfaz.** Action Terms: `Create` · `Update` · `Exchange` · `Control` · `Capture` · `Request` · `Grant` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 36 | 16 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Create` · `Update` · `Exchange` · `Control` · `Capture` · `Request` · `Grant` · `Retrieve` |
| BQ `Systems` | `Request` · `Retrieve` · `Update` · `Exchange` |
| BQ `IT Operations` | `Update` · `Exchange` · `Request` · `Retrieve` |
| BQ `HR Operations` | `Update` · `Exchange` · `Request` · `Retrieve` |
| BQ `Sales and Marketing` | `Update` · `Exchange` · `Request` · `Retrieve` |
| BQ `Servicing` | `Update` · `Exchange` · `Request` · `Retrieve` |
| BQ `Production` | `Update` · `Exchange` · `Request` · `Retrieve` |
| BQ `Production Support` | `Update` · `Request` · `Exchange` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Product Training

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Product Training` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Product Training Procedure` |
| **Ubicación Matrix** | Reference Data › Product Management |

**Propósito.** Develop and provide product specific training across the workforce. This includes all media and training mechanisms (on-line, self taught, classroom etc.)

<details><summary><b>Atributos del Control Record</b> · 20</summary>

`Parameter Type` · `Selected Option` · `Request` · `Schedule` · `Status` · `Reference` · `Business Unit Reference` · `Service Provider Reference` · `Financial Facility Reference` · `Employee Reference` · `Customer Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `ProductandService Type` · `Product and Service Instance` · `Transaction Type` · `Transaction` · `Financial Transaction Arrangement` · `Customer Agreement Reference`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Service Scheduling | 8 |
| Content Development | 8 |
| Service Delivery | 8 |
| Service Evaluation | 8 |

**Interfaz.** Action Terms: `Exchange` · `Control` · `Execute` · `Initiate` · `Retrieve` · `Request` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 28 | 12 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Exchange` · `Control` · `Execute` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Content Development` | `Exchange` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Service Delivery` | `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Service Scheduling` | `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Service Evaluation` | `Exchange` · `Retrieve` · `Request` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Product Quality Assurance

| | |
|---|---|
| **Patrón funcional** | `Assess` |
| **Tipo de activo** | `Product and Service` |
| **Artefacto genérico** | `Assessment` |
| **Control Record** | `Product and Service Assessment` |
| **Ubicación Matrix** | Reference Data › Product Management |

**Propósito.** Maintain and execute a portfolio of product quality assurance tests and certifications that can be applied to evaluate any aspect of production activity for quality assurance

<details><summary><b>Atributos del Control Record</b> · 11</summary>

`Productand Service Assessment Parameter Type` · `Productand Service Assessment Selected Option` · `Productand Service Assessment Type` · `Productand Service Assessment Reference` · `Productand Service Assessment Request` · `Productand Service Assessment Schedule` · `Productand Service Assessment Status` · `Productand Service Assessment Usage Log` · `Productand Service Assessment Requester Reference` · `Productand Service Assessment Associated Party` · `Productand Service Assessment Service Provider Reference`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Processing Error and Integrity Checks | 7 |
| Usability Checks | 7 |
| Resiliency and Performance Checks | 7 |
| Functional Consistency Checks | 7 |

**Interfaz.** Action Terms: `Exchange` · `Execute` · `Grant` · `Initiate` · `Retrieve` · `Request` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 19 | 12 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Exchange` · `Execute` · `Grant` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Functional Consistency Checks` | `Initiate` · `Retrieve` · `Update` |
| BQ `Processing Error and Integrity Checks` | `Initiate` · `Retrieve` · `Update` |
| BQ `Resiliency and Performance Checks` | `Initiate` · `Retrieve` · `Update` |
| BQ `Usability Checks` | `Initiate` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Discount Pricing

| | |
|---|---|
| **Patrón funcional** | `Assess` |
| **Tipo de activo** | `Productand Service Discount` |
| **Artefacto genérico** | `Assessment` |
| **Control Record** | `Productand Service Discount Assessment` |
| **Ubicación Matrix** | Reference Data › Product Management |

[↑ Índice](README.md)

---

## Product Directory

| | |
|---|---|
| **Patrón funcional** | `Catalog` |
| **Tipo de activo** | `Product` |
| **Artefacto genérico** | `Directory Entry` |
| **Control Record** | `Product Directory Entry` |
| **Ubicación Matrix** | Reference Data › Product Management |

**Propósito.** This service domain maintains a comprehensive directory of the bank

<details><summary><b>Atributos del Control Record</b> · 3</summary>

`Product Version` · `Configuration` · `Product Refrence`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Operations | 4 |
| Sales and Marketing | 8 |
| Servicing | 4 |
| Production | 3 |

**Interfaz.** Action Terms: `Update` · `Register` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 16 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Update` · `Register` · `Request` · `Retrieve` |
| BQ `Operations` | `Register` · `Update` · `Retrieve` |
| BQ `Sales and Marketing` | `Register` · `Update` · `Retrieve` |
| BQ `Servicing` | `Update` · `Register` · `Retrieve` |
| BQ `Production` | `Register` · `Update` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Special Pricing Conditions

| | |
|---|---|
| **Patrón funcional** | `Catalog` |
| **Tipo de activo** | `Special Pricing Conditions` |
| **Artefacto genérico** | `Directory Entry` |
| **Control Record** | `Special Pricing Conditions Directory Entry` |
| **Ubicación Matrix** | Reference Data › Product Management |

**Propósito.** Maintain a pricing list or conditions (with ranges and optional terms) categorized by various dimensions to impose exceptional product pricing conditions that override standard pricing terms (for special events/situations)

<details><summary><b>Atributos del Control Record</b> · 7</summary>

`Description` · `Schedule` · `Version` · `Status` · `Usage Log` · `Update Log` · `Service Configuration`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Pricing Terms | 6 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Request` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 10 | 6 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Pricing Terms` | `Initiate` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---
