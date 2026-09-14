# Sales and Service

**BIAN Service Landscape V14.0 · vista Matrix** — 74 Service Domains

> Curso independiente de CPS Tech · No afiliado ni acreditado por BIAN e.V. · BIAN® es marca registrada de BIAN e.V., usada con fines descriptivos.

[← Volver al índice de los 341](README.md)

---

## Contenido

**Channel Specific** · 17

[Branch Location Management](#branch-location-management) · [Contact Center Management](#contact-center-management) · [Branch Network Management](#branch-network-management) · [eBranch Management](#ebranch-management) · [Advanced Voice Services Management](#advanced-voice-services-management) · [ATM Network Management](#atm-network-management) · [Contact Center Operations](#contact-center-operations) · [Branch Location Operations](#branch-location-operations) · [eBranch Operations](#ebranch-operations) · [Advanced Voice Services Operations](#advanced-voice-services-operations) · [ATM Network Operations](#atm-network-operations) · [Branch Currency Management](#branch-currency-management) · [Branch Currency Distribution](#branch-currency-distribution) · [Product Inventory Item Management](#product-inventory-item-management) · [Product Inventory Distribution](#product-inventory-distribution) · [Card Terminal Administration](#card-terminal-administration) · [Card Terminal Operation](#card-terminal-operation)

**Cross Channel** · 11

[Party Authentication](#party-authentication) · [Transaction Authorization](#transaction-authorization) · [Point of Service](#point-of-service) · [Servicing Event History](#servicing-event-history) · [Contact Routing](#contact-routing) · [Session Dialogue](#session-dialogue) · [Interactive Help](#interactive-help) · [Contact Handler](#contact-handler) · [Customer Workbench](#customer-workbench) · [Servicing Activity Analysis](#servicing-activity-analysis) · [Service Directory](#service-directory)

**Marketing** · 9

[Business Development](#business-development) · [Brand Management](#brand-management) · [Advertising](#advertising) · [Promotional Events](#promotional-events) · [Prospect Campaign Design](#prospect-campaign-design) · [Customer Campaign Management](#customer-campaign-management) · [Customer Campaign Design](#customer-campaign-design) · [Customer Surveys](#customer-surveys) · [Prospect Campaign Management](#prospect-campaign-management)

**Sales** · 13

[Prospect Campaign Execution](#prospect-campaign-execution) · [Party Lifecycle Management](#party-lifecycle-management) · [Lead and Opportunity Management](#lead-and-opportunity-management) · [Customer Campaign Execution](#customer-campaign-execution) · [Customer Offer](#customer-offer) · [Sales Planning](#sales-planning) · [Underwriting](#underwriting) · [Commission Agreement](#commission-agreement) · [Commissions](#commissions) · [Product Matching](#product-matching) · [Product Expert Sales Support](#product-expert-sales-support) · [Product Sales Support](#product-sales-support) · [Sales Product](#sales-product)

**Customer Management** · 15

[Customer Relationship Management](#customer-relationship-management) · [Customer Product And Service Eligibility](#customer-product-and-service-eligibility) · [Customer Agreement](#customer-agreement) · [Sales Product Agreement](#sales-product-agreement) · [Customer Access Entitlement](#customer-access-entitlement) · [Customer Behavior Insights](#customer-behavior-insights) · [Customer Credit Rating](#customer-credit-rating) · [Account Recovery](#account-recovery) · [Customer Event History](#customer-event-history) · [Party Reference Data Directory](#party-reference-data-directory) · [Customer Proposition](#customer-proposition) · [Customer Product and Service Directory](#customer-product-and-service-directory) · [Customer Financial Insights](#customer-financial-insights) · [Customer Consent](#customer-consent) · [Payee Management](#payee-management)

**Servicing** · 9

[Servicing Issue](#servicing-issue) · [Customer Case Management](#customer-case-management) · [Case Root Cause Analysis](#case-root-cause-analysis) · [Customer Case](#customer-case) · [Card Case](#card-case) · [Servicing Order](#servicing-order) · [Servicing Mandate](#servicing-mandate) · [Payment Order Initiation](#payment-order-initiation) · [Loan Syndication](#loan-syndication)

---

## Branch Location Management

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `Branch Location` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `Branch Location Management Plan` |
| **Ubicación Matrix** | Sales and Service › Channel Specific |

**Propósito.** Manage and oversee branch activity, assign resources to optimize branch performance

<details><summary><b>Atributos del Control Record</b> · 7</summary>

`Type` · `Reference` · `Budget Type` · `Budget` · `Assignment` · `Branch Location Management Plan` · `Description`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Customer Liaison | 8 |
| Product and Service Planning | 8 |
| Troubleshooting | 8 |
| Staff and Location Planning | 8 |

**Interfaz.** Action Terms: `Capture` · `Control` · `Exchange` · `Grant` · `Initiate` · `Retrieve` · `Request` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 27 | 12 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Capture` · `Control` · `Exchange` · `Grant` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Product and Service Planning` | `Capture` · `Control` · `Retrieve` · `Request` · `Update` |
| BQ `Customer Liaison` | `Capture` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Staff and Location Planning` | `Capture` · `Retrieve` · `Request` · `Update` |
| BQ `Troubleshooting` | `Capture` · `Initiate` · `Retrieve` · `Request` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Contact Center Management

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `Contact Center` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `Contact Center Management Plan` |
| **Ubicación Matrix** | Sales and Service › Channel Specific |

**Propósito.** Oversee the assignment and operation of the customer contact center

<details><summary><b>Atributos del Control Record</b> · 7</summary>

`Period` · `Contact Center Usage Policies And Guidelines` · `Contact Center Service Performance Goals` · `Contact Center Service Schedule` · `Contact Center Service Operating Configuration` · `Contact Center Resource Plan` · `Contact Center Training Plan`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Performance | 7 |
| Troubleshooting | 2 |

**Interfaz.** Action Terms: `Update` · `Create` · `Exchange` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 12 | 6 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Update` · `Create` · `Exchange` · `Request` · `Retrieve` |
| BQ `Performance` | `Request` · `Retrieve` · `Update` |
| BQ `Troubleshooting` | `Create` · `Retrieve` · `Update` · `Request` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Branch Network Management

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `Branch Network` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `Branch Network Management Plan` |
| **Ubicación Matrix** | Sales and Service › Channel Specific |

[↑ Índice](README.md)

---

## eBranch Management

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `eBranch Channel` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `eBranch Channel Management Plan` |
| **Ubicación Matrix** | Sales and Service › Channel Specific |

**Propósito.** Oversee the configuration and operation of the e-branch channel facilities

<details><summary><b>Atributos del Control Record</b> · 5</summary>

`Period` · `eBranch Channel Usage Policies And Guidelines` · `eBranch Channel Service Operating Parameters` · `eBranch Channel Service Performance Goals` · `eBranch Channel Service Schedule`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Capacity Planning | 2 |
| Maintenance And Upgrades | 6 |
| Troubleshooting | 2 |

**Interfaz.** Action Terms: `Create` · `Update` · `Exchange` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 15 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Create` · `Update` · `Exchange` · `Request` · `Retrieve` |
| BQ `Maintenance And Upgrades` | `Update` · `Create` · `Request` · `Retrieve` |
| BQ `Capacity Planning` | `Update` · `Retrieve` · `Request` |
| BQ `Troubleshooting` | `Update` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Advanced Voice Services Management

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `Voice Channel` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `Voice Channel Management Plan` |
| **Ubicación Matrix** | Sales and Service › Channel Specific |

**Propósito.** Oversee the configuration and operation of the voice channel facilities

<details><summary><b>Atributos del Control Record</b> · 5</summary>

`VChannel Management Plan Period` · `VChannel Usage Policies And Guidelines` · `VChannel Service Operating Parameters` · `VChannel Service Performance Goals` · `VChannel Service Schedule`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Capacity Planning | 2 |
| Maintenance And Upgrades | 6 |
| Troubleshooting | 2 |

**Interfaz.** Action Terms: `Create` · `Exchange` · `Retrieve` · `Request` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 15 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Create` · `Exchange` · `Retrieve` · `Request` · `Update` |
| BQ `Maintenance And Upgrades` | `Update` · `Request` · `Create` · `Retrieve` |
| BQ `Capacity Planning` | `Retrieve` · `Update` · `Request` |
| BQ `Troubleshooting` | `Update` · `Retrieve` · `Request` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## ATM Network Management

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `ATM Network` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `ATM Network Management Plan` |
| **Ubicación Matrix** | Sales and Service › Channel Specific |

[↑ Índice](README.md)

---

## Contact Center Operations

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Contact Center` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Contact Center Administrative Plan` |
| **Ubicación Matrix** | Sales and Service › Channel Specific |

**Propósito.** Administer the day to day activity in the contact center

<details><summary><b>Atributos del Control Record</b> · 9</summary>

`Contact Center Service Operating Configuration` · `Customer Servicing Representative Allocation Schedule` · `Customer Servicing Representative Reference` · `Customer Servicing Representative Record` · `Customer Servicing Representative Qualification Profile` · `Customer Servicing Representative Location` · `Customer Servicing Representative Availability Schedule` · `Customer Servicing Representative Status` · `Customer Servicing Representative Assignment Record`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Assignment | 5 |
| Peak Load | 5 |
| Troubleshooting | 2 |

**Interfaz.** Action Terms: `Create` · `Update` · `Control` · `Execute` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 18 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Create` · `Update` · `Control` · `Execute` · `Request` · `Retrieve` |
| BQ `Assignment` | `Create` · `Update` · `Control` · `Request` · `Retrieve` |
| BQ `Peak Load` | `Update` · `Request` · `Retrieve` |
| BQ `Troubleshooting` | `Create` · `Update` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Branch Location Operations

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Branch Location` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Branch Location Administrative Plan` |
| **Ubicación Matrix** | Sales and Service › Channel Specific |

**Propósito.** The day to day administration of branch activity, including teller assignment and cash handling oversight

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Budget Type` · `Budget` · `Assignment` · `Duty` · `Associated Party` · `Budget Balance` · `Subject Matter` · `Type` · `Reference` · `Description`

</details>

**Behavior Qualifiers** · 6

| Behavior Qualifier | Atributos |
|---|---:|
| Cash Inventory Handling | 8 |
| Non-cash Inventory Handling | 8 |
| Staff Assignment | 8 |
| Safe Custody Operations | 8 |
| Location Security Administration | 8 |
| Workforce Administration | 8 |

**Interfaz.** Action Terms: `Control` · `Create` · `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 14 | 16 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Create` · `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Cash Inventory Handling` | `Update` · `Exchange` · `Grant` · `Notify` · `Retrieve` · `Request` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## eBranch Operations

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `eBranch Channel` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `eBranch Channel Operating Session` |
| **Ubicación Matrix** | Sales and Service › Channel Specific |

**Propósito.** This service domain operates the bank's on-line web based electronic branch capabilities - controlling access and load balancing across available communications and processing resources to optimize performance/availability

<details><summary><b>Atributos del Control Record</b> · 12</summary>

`EBranch Operations Service Menu` · `EBranch Service Session Statistics` · `EBranch Service Session Report Type` · `EBranch Service Session Report` · `EBranch Production Issue Record` · `Employee or Business Unit Reference` · `Customer Contact Record Reference` · `Production Issue Type` · `Production Issue Description` · `Production Issue Diagnosis` · `Production Issue Resolution Task` · `Production Issue Status`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Inbound | 5 |
| Outbound | 6 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Request` · `Retrieve` · `Control`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 9 | 6 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Request` · `Retrieve` · `Control` |
| BQ `Inbound` | `Retrieve` · `Initiate` |
| BQ `Outbound` | `Retrieve` · `Initiate` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Advanced Voice Services Operations

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `Voice Channel` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `Voice Channel Operating Session` |
| **Ubicación Matrix** | Sales and Service › Channel Specific |

**Propósito.** This service domain operates the telephone channel infrastructure, including the IVR and any other automated devices as appropriate

<details><summary><b>Atributos del Control Record</b> · 12</summary>

`Advanced Voice Services Operations Service Menu` · `VChannel Service Session Statistics` · `VChannel Service Session Report Type` · `VChannel Service Session Report` · `VChannel Production Issue Record` · `Employee/Business Unit Reference` · `Customer Contact Record Reference` · `Production Issue Type` · `Production Issue Description` · `Production Issue Diagnosis` · `Production Issue Resolution Task` · `Production Issue Status`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Inbound | 5 |
| Outbound | 6 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 9 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Request` · `Retrieve` |
| BQ `Inbound` | `Initiate` · `Retrieve` |
| BQ `Outbound` | `Initiate` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## ATM Network Operations

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `ATM Network` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `ATM Network Operating Session` |
| **Ubicación Matrix** | Sales and Service › Channel Specific |

**Propósito.** Handling the automated operation of the ATM network and linked devices, including tracing physical cash and document movements

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Schedule` · `Status` · `Usage Log` · `Associated Party Reference` · `Service Provider Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Service Configuration` · `Reference`

</details>

**Behavior Qualifiers** · 5

| Behavior Qualifier | Atributos |
|---|---:|
| Network Operation | 6 |
| Device Tracking | 6 |
| Cash Distribution | 6 |
| Financial Document Handling | 6 |
| Financial Transaction Capture | 6 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Execute` · `Request` · `Retrieve` · `Update` · `Initiate`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 28 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Request` · `Retrieve` · `Update` · `Initiate` |
| BQ `Cash Distribution` | `Exchange` · `Retrieve` · `Request` |
| BQ `Network Operation` | `Control` · `Initiate` · `Retrieve` · `Update` |
| BQ `Device Tracking` | `Exchange` · `Execute` · `Retrieve` · `Update` |
| BQ `Financial Document Handling` | `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Update` |
| BQ `Financial Transaction Capture` | `Exchange` · `Initiate` · `Execute` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Branch Currency Management

| | |
|---|---|
| **Patrón funcional** | `Allocate` |
| **Tipo de activo** | `Branch Cash` |
| **Artefacto genérico** | `Allocation` |
| **Control Record** | `Branch Cash Allocation` |
| **Ubicación Matrix** | Sales and Service › Channel Specific |

**Propósito.** Track cash inventory, project demand and ensure all cash is accounted for within the branch

<details><summary><b>Atributos del Control Record</b> · 17</summary>

`Parameter Type` · `Selected Option` · `<Subject Area> Type` · `Description` · `Request` · `Schedule` · `Status` · `Reference` · `Customer Reference` · `Currency` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Booking Location` · `Account Type` · `Account Reference` · `Instance`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Inventory Allocation | 3 |

**Interfaz.** Action Terms: `Capture` · `Exchange` · `Control` · `Initiate` · `Update` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 12 | 6 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Capture` · `Exchange` · `Control` · `Initiate` · `Update` · `Retrieve` |
| BQ `Inventory Allocation` | `Exchange` · `Capture` · `Control` · `Initiate` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Branch Currency Distribution

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Cash Distribution` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Cash Distribution Procedure` |
| **Ubicación Matrix** | Sales and Service › Channel Specific |

**Propósito.** Schedule and coordinate the secure distribution of cash inventory across the branch and ATM networks

<details><summary><b>Atributos del Control Record</b> · 20</summary>

`Parameter Type` · `Selected Option` · `Request` · `Schedule` · `Status` · `Reference` · `Business Unit Reference` · `Service Provider Reference` · `Financial Facility Reference` · `Employee Reference` · `Customer Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Product and Service Type` · `Product and Service Instance` · `Transaction Type` · `Transaction` · `Financial Transaction Arrangement` · `Customer Agreement Reference`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Inventory Distribution Oversight | 8 |
| Inventory Provisioning | 8 |
| Distribution Vehicle Administration | 8 |
| Distribution Planning | 8 |

**Interfaz.** Action Terms: `Exchange` · `Control` · `Execute` · `Request` · `Initiate` · `Update` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 21 | 12 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Exchange` · `Control` · `Execute` · `Request` · `Initiate` · `Update` · `Retrieve` |
| BQ `Distribution Planning` | `Exchange` · `Retrieve` · `Request` · `Update` |
| BQ `Inventory Provisioning` | `Exchange` · `Retrieve` · `Request` · `Update` |
| BQ `Inventory Distribution Oversight` | `Retrieve` · `Request` · `Update` |
| BQ `Distribution Vehicle Administration` | `Retrieve` · `Request` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Product Inventory Item Management

| | |
|---|---|
| **Patrón funcional** | `Allocate` |
| **Tipo de activo** | `Product Inventory` |
| **Artefacto genérico** | `Allocation` |
| **Control Record** | `Product Inventory Allocation` |
| **Ubicación Matrix** | Sales and Service › Channel Specific |

**Propósito.** Maintain and distribute product inventory

<details><summary><b>Atributos del Control Record</b> · 9</summary>

`Service Schedule` · `Product Inventory Holdings` · `Product and Service Type` · `Product Inventory Item Type` · `Product Inventory Item Record` · `Product Inventory Item Description` · `Product Inventory Item Supplier Details` · `Product Inventory Used Locations` · `Product Inventory Holding`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Assignment | 6 |

**Interfaz.** Action Terms: `Update` · `Request` · `Retrieve` · `Provide` · `Exchange`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 8 | 4 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Update` · `Request` · `Retrieve` |
| BQ `Assignment` | `Update` · `Provide` · `Request` · `Retrieve` · `Exchange` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Product Inventory Distribution

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Product Inventory Distribution` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Product Inventory Distribution Administrative Plan` |
| **Ubicación Matrix** | Sales and Service › Channel Specific |

**Propósito.** Administer the provisioning and distribution of product inventory across the branch network and/or distribute direct to customers (e.g. mail) where appropriate

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Budget Type` · `Budget` · `Assignment` · `Duty` · `Associated Party` · `Budget Balance` · `Subject Matter` · `Type` · `Reference` · `Description`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Provisioning | 8 |
| Oversight | 8 |
| Distribution | 8 |
| Mailing | 8 |

**Interfaz.** Action Terms: `Capture` · `Control` · `Exchange` · `Grant` · `Initiate` · `Retrieve` · `Update` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 24 | 12 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Capture` · `Control` · `Exchange` · `Grant` · `Initiate` · `Retrieve` · `Update` · `Request` |
| BQ `Oversight` | `Capture` · `Initiate` · `Retrieve` · `Update` |
| BQ `Distribution` | `Capture` · `Initiate` · `Retrieve` · `Update` |
| BQ `Mailing` | `Capture` · `Initiate` · `Retrieve` · `Update` |
| BQ `Provisioning` | `Capture` · `Initiate` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Card Terminal Administration

| | |
|---|---|
| **Patrón funcional** | `Allocate` |
| **Tipo de activo** | `Card POS Device` |
| **Artefacto genérico** | `Allocation` |
| **Control Record** | `Card POS Device Allocation` |
| **Ubicación Matrix** | Sales and Service › Channel Specific |

**Propósito.** This service domain administers the POS Network including the inventory, terminal characteristics, deployment and status of the POS devices

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Card POS Device Reference` · `Card POS Device Identifier` · `Card POS Device Type` · `Card POS Device Software Type` · `Card POS Device Software Version` · `Card POS Device Acquired Date` · `Card POS Repair Record` · `Card POS Repair Details` · `Card POS Repair Dates` · `Card POS Device Status`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Allocation | 4 |

**Interfaz.** Action Terms: `Update` · `Request` · `Provide` · `Control` · `Exchange` · `Retrieve` · `Grant` · `Capture`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 11 | 4 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Update` · `Request` · `Provide` · `Retrieve` |
| BQ `Allocation` | `Provide` · `Control` · `Exchange` · `Update` · `Retrieve` · `Grant` · `Capture` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Card Terminal Operation

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `Card POS Network` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `Card POS Network Operating Session` |
| **Ubicación Matrix** | Sales and Service › Channel Specific |

**Propósito.** This service domain handle POS operations including processing, capture and tracking of the transactions originating at the Point of Sale devices

<details><summary><b>Atributos del Control Record</b> · 1</summary>

`Card POS Terminal Operating Schedule`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Capture | 17 |
| Authorization | 1 |
| Batch | 1 |

**Interfaz.** Action Terms: `Retrieve` · `Update` · `Initiate` · `Control` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 15 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Retrieve` · `Update` · `Initiate` · `Control` |
| BQ `Capture` | `Initiate` · `Update` · `Request` · `Retrieve` |
| BQ `Authorization` | `Initiate` · `Retrieve` · `Request` |
| BQ `Batch` | `Initiate` · `Retrieve` · `Update` · `Request` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Party Authentication

| | |
|---|---|
| **Patrón funcional** | `Assess` |
| **Tipo de activo** | `Party Authentication` |
| **Artefacto genérico** | `Assessment` |
| **Control Record** | `Party Authentication Assessment` |
| **Ubicación Matrix** | Sales and Service › Cross Channel |

**Propósito.** This service domain provides a customer identify authentication service covering all channels and devices to support access to the banks products and services

<details><summary><b>Atributos del Control Record</b> · 8</summary>

`Customer Reference` · `Party Reference` · `Profile` · `Authentication Type` · `Party Authentication Consolidation Record` · `Customer Contact Authentication Level` · `Authorisation Token Reference` · `Refresh Token Reference`

</details>

**Behavior Qualifiers** · 6

| Behavior Qualifier | Atributos |
|---|---:|
| Password | 9 |
| Question | 4 |
| Document | 5 |
| Device | 5 |
| Biometric | 4 |
| Behavior | 4 |

**Interfaz.** Action Terms: `Update` · `Evaluate` · `Exchange` · `Execute` · `Request` · `Grant` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 19 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Update` · `Evaluate` · `Exchange` · `Execute` · `Request` · `Grant` · `Retrieve` |
| BQ `Password` | `Evaluate` · `Retrieve` |
| BQ `Question` | `Evaluate` · `Retrieve` |
| BQ `Document` | `Retrieve` · `Evaluate` |
| BQ `Device` | `Evaluate` · `Retrieve` |
| BQ `Biometric` | `Evaluate` · `Retrieve` |
| BQ `Behavior` | `Evaluate` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Transaction Authorization

| | |
|---|---|
| **Patrón funcional** | `Assess` |
| **Tipo de activo** | `Interactive Transaction` |
| **Artefacto genérico** | `Assessment` |
| **Control Record** | `Interactive Transaction Assessment` |
| **Ubicación Matrix** | Sales and Service › Cross Channel |

**Propósito.** This service domain handles risk based authorization for interactive customer transactions. This combines the context (channel) transaction, customer details and recent activity analysis as appropriate. The authorization may require a specific level of party/customer authentication to get approval.

<details><summary><b>Atributos del Control Record</b> · 35</summary>

`Customer Reference` · `Employee Reference` · `Product Reference` · `Product Instance Reference` · `Proposed Transaction Type` · `Proposed Transaction Value` · `Customer Contact Record Reference` · `Customer Contact Record` · `Customer Contact Record Customer Reference` · `Customer Contact Record Contact Device` · `Customer Contact Record Authentication Status` · `Customer Contact Record Routing Selection Status` · `Customer Contact Record Menu Selection` · `Customer Contact Record Servicing Request` · `Customer Contact Record Servicing Event History` · `Customer Contact Record Servicing Position Reference` · `Customer Contact Record Servicing Resource Reference` · `Customer Contact Record Activity Record` · `Customer Session Dialogue Reference` · `Customer Session Dialogue Record` · `Session Dialogue Type` · `Session Dialogue Script` · `Session Dialogue Log Reference` · `Session Dialogue Log` · `Session Dialogue Session Mechanism` · `Session Dialogue Record Session Start/End Time` · `Session Dialogue Result` · `Customer Contact Record Duration` · `Customer Contact Activity Record` · `Customer Contact Result` · `Channel Activity History Report Reference` · `Channel Activity History Report From/to` · `Channel Activity History Report` · `Transaction Authorization Guidance` · `Transaction Authorization Result`

</details>

**Interfaz.** Action Terms: `Evaluate` · `Request` · `Retrieve` · `Exchange` · `Update` · `Execute` · `Grant`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 7 | 2 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Evaluate` · `Request` · `Retrieve` · `Exchange` · `Update` · `Execute` · `Grant` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Point of Service

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `Pointof Service` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `Pointof Service Operating Session` |
| **Ubicación Matrix** | Sales and Service › Cross Channel |

**Propósito.** This service domain operates servicing positions within the bank. It administers all media connections, inventory holdings (e.g. cash), provides access to support utilities and tracks servicing activity -e.g. time spent, activity logs, capturing servicing events including commission and training related actions. In cases servicing positions can be automated

<details><summary><b>Atributos del Control Record</b> · 11</summary>

`Servicing Position Configuration/Set-up` · `Servicing Position Reference` · `Servicing Position Type` · `Servicing Position Location` · `Servicing Position Facility Type` · `Servicing Position Facility Reference` · `Servicing Position Schedule` · `Servicing Position Activity Report` · `Servicing Position Operating Session Statistics` · `Servicing Position Operating Session Report Type` · `Servicing Position Operating Session Report`

</details>

**Behavior Qualifiers** · 5

| Behavior Qualifier | Atributos |
|---|---:|
| Assisted | 2 |
| Automated | 1 |
| Interaction | 1 |
| Inventory | 3 |
| Cash Position | 5 |

**Interfaz.** Action Terms: `Update` · `Initiate` · `Control` · `Execute` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 23 | 12 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Update` · `Initiate` · `Control` · `Execute` · `Request` · `Retrieve` |
| BQ `Assisted` | `Update` · `Control` · `Retrieve` · `Initiate` |
| BQ `Automated` | `Initiate` · `Update` · `Control` · `Retrieve` |
| BQ `Interaction` | `Update` · `Control` · `Retrieve` |
| BQ `Inventory` | `Retrieve` · `Execute` · `Update` |
| BQ `Cash Position` | `Update` · `Execute` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Servicing Event History

| | |
|---|---|
| **Patrón funcional** | `Track` |
| **Tipo de activo** | `Servicing Event` |
| **Artefacto genérico** | `Log` |
| **Control Record** | `Servicing Event Log` |
| **Ubicación Matrix** | Sales and Service › Cross Channel |

**Propósito.** This service domain captures, classifies and stores servicing activity and events to support root cause analysis

<details><summary><b>Atributos del Control Record</b> · 2</summary>

`Servicing Position Reference` · `Employee or Business Unit Reference`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Assignment | 3 |
| Session | 10 |
| Servicing Facility | 2 |
| Issue | 7 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Retrieve` · `Capture`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 16 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Retrieve` |
| BQ `Assignment` | `Update` · `Capture` · `Retrieve` |
| BQ `Session` | `Capture` · `Update` · `Retrieve` |
| BQ `Issue` | `Update` · `Capture` · `Retrieve` |
| BQ `Servicing Facility` | `Update` · `Capture` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Contact Routing

| | |
|---|---|
| **Patrón funcional** | `Allocate` |
| **Tipo de activo** | `Customer Servicing Resource` |
| **Artefacto genérico** | `Allocation` |
| **Control Record** | `Customer Servicing Resource Allocation` |
| **Ubicación Matrix** | Sales and Service › Cross Channel |

**Propósito.** The Contact Routing service domain tracks servicing resource availability and makes an optimal routing decision

<details><summary><b>Atributos del Control Record</b> · 8</summary>

`Servicing Resource Allocation Service Schedule` · `Servicing Resource Reference` · `Servicing Resource Record` · `Servicing Resource Qualification Profile` · `Servicing Position Reference` · `Servicing Resource Availability Schedule` · `Servicing Resource Status` · `Servicing Session Reference`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Allocation | 4 |

**Interfaz.** Action Terms: `Provide` · `Control` · `Update` · `Exchange` · `Capture` · `Retrieve` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 12 | 4 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Provide` · `Control` · `Update` · `Exchange` · `Capture` · `Retrieve` |
| BQ `Allocation` | `Request` · `Update` · `Control` · `Exchange` · `Capture` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Session Dialogue

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Customer Contact Session` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Customer Contact Session Procedure` |
| **Ubicación Matrix** | Sales and Service › Cross Channel |

**Propósito.** This service domain handles/structures the customer narrative during an interactive session. It consolidates and presents pertinent customer information and provides servicing guidelines with standard dialogue/scripting as appropriate. It can include the capability to provoke questions to capture key relationship and sales triggers. It also ensures the correct sequencing, dialogue content and actions are performed/initiated during the customer interaction. It may further leverage the session by passing on customer notifications, status updates and triggering sales/marketing efforts.

<details><summary><b>Atributos del Control Record</b> · 11</summary>

`Customer Reference` · `Employee Reference` · `Servicing Position Reference` · `Session Mechanism` · `Session Start/End Time` · `Session Dialogue Record` · `Session Dialogue Type` · `Session Dialogue Script` · `Session Dialogue Log Reference` · `Session Dialogue Log` · `Session Dialogue Result`

</details>

**Behavior Qualifiers** · 8

| Behavior Qualifier | Atributos |
|---|---:|
| Query | 2 |
| Sales | 3 |
| Offer | 2 |
| Product or Service | 2 |
| Case | 3 |
| Order | 4 |
| Intelligence | 4 |
| History | 1 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Exchange` · `Execute` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 35 | 20 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Exchange` · `Execute` · `Request` · `Retrieve` |
| BQ `Query` | `Initiate` · `Update` · `Retrieve` |
| BQ `Authentication` | `Retrieve` · `Update` |
| BQ `Sales` | `Initiate` · `Update` · `Retrieve` |
| BQ `Offer` | `Initiate` · `Update` · `Retrieve` |
| BQ `Product or Service` | `Initiate` · `Update` · `Retrieve` · `Execute` · `Exchange` |
| BQ `Case` | `Initiate` · `Update` · `Retrieve` |
| BQ `Order` | `Initiate` · `Retrieve` · `Update` · `Exchange` |
| BQ `Intelligence` | `Initiate` · `Update` · `Retrieve` |
| BQ `History` | `Update` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Interactive Help

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `interactive Help Service` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `interactive Help Service Operating Session` |
| **Ubicación Matrix** | Sales and Service › Cross Channel |

**Propósito.** Operate the automated facility that provides interactive context sensitive servicing guidance to employees and self-serve customers

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Help Service Selection | 11 |

**Interfaz.** Action Terms: `Initiate` · `Retrieve` · `Capture` · `Execute`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 4 | 2 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| BQ `Help Service Selection` | `Initiate` · `Retrieve` · `Capture` · `Execute` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Contact Handler

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `Customer Contact` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `Customer Contact Operating Session` |
| **Ubicación Matrix** | Sales and Service › Cross Channel |

**Propósito.** This service domain handles a customer interactive contact with the bank

<details><summary><b>Atributos del Control Record</b> · 19</summary>

`Customer Contact Inbound or Outbound Indicator` · `eBranch Operating Session Reference` · `Advanced Voice Service Operating Session Reference` · `Customer Contact Record Reference` · `Customer Contact Record` · `Customer Contact Record Customer Reference` · `Customer Contact Record Contact Device` · `Customer Contact Record Authentication Status` · `Customer Contact Record Routing Selection Status` · `Customer Contact Record Menu Selection` · `Customer Contact Record Servicing Request` · `Customer Contact Record Servicing Event History` · `Customer Contact Record Servicing Position Reference` · `Customer Contact Record Servicing Resource Reference` · `Customer Contact Record Activity Record` · `Customer Session Dialogue Reference` · `Customer Session Dialogue Record` · `Customer Contact Record Duration` · `Customer Contact Record Result`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Authentication | 1 |
| Routing | 1 |
| Session | 2 |
| History | 1 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Exchange` · `Execute` · `Retrieve` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 16 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Exchange` · `Execute` · `Retrieve` · `Request` |
| BQ `Authentication` | `Retrieve` |
| BQ `Routing` | `Retrieve` |
| BQ `Session` | `Update` · `Control` · `Execute` · `Retrieve` · `Initiate` |
| BQ `History` | `Update` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Customer Workbench

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `Customer Workbench` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `Customer Workbench Operating Session` |
| **Ubicación Matrix** | Sales and Service › Cross Channel |

**Propósito.** This service domain represents customer side devices, providing a customer access portal to the banks products and services

<details><summary><b>Atributos del Control Record</b> · 9</summary>

`Customer Reference` · `Customer Workbench Device Type` · `Customer Workbench Device Registration` · `Customer Workbench Device Manufacturer` · `Customer Workbench Device Operating System/Version Number` · `Customer Workbench Device Access Permissions` · `Installed Bank Application Type` · `Installed Bank Application Version Number` · `Last Update Date and Time`

</details>

**Behavior Qualifiers** · 5

| Behavior Qualifier | Atributos |
|---|---:|
| SW Update | 4 |
| Broadcast | 2 |
| Browsing | 2 |
| Contact | 2 |
| ProductandService Access | 5 |

**Interfaz.** Action Terms: `Retrieve` · `Initiate` · `Update` · `Control` · `Execute` · `Exchange` · `Request` · `Evaluate`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 23 | 12 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Retrieve` · `Initiate` · `Update` · `Control` |
| BQ `SW Update` | `Initiate` · `Retrieve` · `Exchange` |
| BQ `Broadcast` | `Initiate` · `Request` |
| BQ `Browsing` | `Initiate` · `Execute` · `Retrieve` |
| BQ `Contact` | `Initiate` · `Retrieve` · `Update` · `Execute` · `Request` · `Evaluate` |
| BQ `ProductandService Access` | `Update` · `Initiate` · `Execute` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Servicing Activity Analysis

| | |
|---|---|
| **Patrón funcional** | `Analyze` |
| **Tipo de activo** | `Servicing Root Cause` |
| **Artefacto genérico** | `Analysis` |
| **Control Record** | `Servicing Root Cause Analysis` |
| **Ubicación Matrix** | Sales and Service › Cross Channel |

**Propósito.** This service domain analyzes servicing activity to support continual service improvement

<details><summary><b>Atributos del Control Record</b> · 7</summary>

`Servicing Activity Type` · `Servicing Activity Analysis Period` · `Servicing Activity Analysis Type` · `Servicing Activity Analysis Result` · `Servicing Activity Analysis Determination` · `Servicing Activity Analysis Recommendation` · `Servicing Activity History Report`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Root Cause Algorithm | 6 |

**Interfaz.** Action Terms: `Request` · `Execute` · `Initiate` · `Update` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 8 | 4 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Request` · `Execute` · `Initiate` · `Update` · `Retrieve` |
| BQ `Root Cause Algorithm` | `Initiate` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Service Directory

| | |
|---|---|
| **Patrón funcional** | `Catalog` |
| **Tipo de activo** | `Service` |
| **Artefacto genérico** | `Directory Entry` |
| **Control Record** | `Service Directory Entry` |
| **Ubicación Matrix** | Sales and Service › Cross Channel |

**Propósito.** This Service Domain presents a structured set of services that the customer can select from

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Description` · `Schedule` · `Version` · `Status` · `Usage Log` · `Update Log` · `Service Configuration` · `Reference` · `Customer Reference` · `Service Reference`

</details>

**Behavior Qualifiers** · 6

| Behavior Qualifier | Atributos |
|---|---:|
| Relationship Servicing | 7 |
| Product Access Servicing | 7 |
| Arrangement Servicing | 7 |
| Service Delivery Servicing | 7 |
| Access Control Servicing | 7 |
| Sales Servicing | 7 |

**Interfaz.** Action Terms: `Control` · `Execute` · `Notify` · `Register` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 43 | 23 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Execute` · `Notify` · `Register` · `Request` · `Retrieve` · `Update` |
| BQ `Access Control Servicing` | `Execute` · `Notify` · `Register` · `Request` · `Retrieve` · `Update` |
| BQ `Arrangement Servicing` | `Execute` · `Notify` · `Register` · `Request` · `Retrieve` · `Update` |
| BQ `Product Access Servicing` | `Execute` · `Notify` · `Register` · `Request` · `Retrieve` · `Update` |
| BQ `Relationship Servicing` | `Execute` · `Notify` · `Register` · `Request` · `Retrieve` · `Update` |
| BQ `Service Delivery Servicing` | `Execute` · `Notify` · `Register` · `Request` · `Retrieve` · `Update` |
| BQ `Sales Servicing` | `Execute` · `Notify` · `Register` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Business Development

| | |
|---|---|
| **Patrón funcional** | `Direct` |
| **Tipo de activo** | `Business Development` |
| **Artefacto genérico** | `Strategy` |
| **Control Record** | `Business Development Strategy` |
| **Ubicación Matrix** | Sales and Service › Marketing |

**Propósito.** Define, implement, track and assess the new business development plans

<details><summary><b>Atributos del Control Record</b> · 12</summary>

`Period` · `Policies And Guidelines` · `Organization` · `Budget` · `Schedule` · `Business Development Goal Reference` · `Business Development Goal Organization` · `Business Development Goal Result` · `Reference` · `Planned Action` · `Survey Reference` · `Market Research Reference`

</details>

**Behavior Qualifiers** · 8

| Behavior Qualifier | Atributos |
|---|---:|
| Customer Relationship | 10 |
| Product Delivery Capacity | 12 |
| Organization | 10 |
| Marketing | 10 |
| Operational Efficiency | 10 |
| Employee Development | 10 |
| Sustainability and Corporate Social Responsibility | 10 |
| Organizational Responsiveness and Flexibility | 10 |

**Interfaz.** Action Terms: `Update` · `Grant` · `Exchange` · `Create` · `Request` · `Retrieve` · `Capture`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 7 | 18 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Update` · `Grant` · `Exchange` · `Create` · `Request` · `Retrieve` · `Capture` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Brand Management

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `Brand` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `Brand Management Plan` |
| **Ubicación Matrix** | Sales and Service › Marketing |

**Propósito.** Respond to events that potentially damage the brand or provide an opportunity to strengthen/leverage brand awareness

<details><summary><b>Atributos del Control Record</b> · 4</summary>

`Brand Definition` · `Brand Value Assessment` · `Brand Usage` · `Brand Development Schedule`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Brand Advice | 5 |
| Troubleshooting | 8 |

**Interfaz.** Action Terms: `Request` · `Create` · `Update` · `Grant` · `Retrieve` · `Exchange`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 13 | 6 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Request` · `Update` · `Grant` · `Retrieve` |
| BQ `Brand Advice` | `Create` · `Update` · `Exchange` · `Request` · `Retrieve` |
| BQ `Troubleshooting` | `Create` · `Retrieve` · `Update` · `Request` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Advertising

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `Advertising Campaign` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `Advertising Campaign Management Plan` |
| **Ubicación Matrix** | Sales and Service › Marketing |

**Propósito.** Develop the plan for and oversee advertising campaign activity, including budget and resource management

<details><summary><b>Atributos del Control Record</b> · 12</summary>

`Advertising Campaign Portfolio` · `Advertising Campaign Type` · `Advertising Campaign Description` · `Advertising Campaign Metrics` · `Advertising Campaign Metric Definition` · `Advertising Campaign Metric Goal` · `Advertising Campaign Performance Record` · `Advertising Campaign Procedure Instance Reference` · `Advertising Campaign Execution Plan` · `Employee or Business Unit Reference` · `Advertising Campaign Duration` · `Advertising Campaign Procedure Result`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Market Tracking | 6 |
| Performance Assessment | 5 |
| Campaign Direction | 2 |

**Interfaz.** Action Terms: `Request` · `Create` · `Update` · `Execute` · `Retrieve` · `Grant`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 18 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| BQ `Market Tracking` | `Request` · `Execute` · `Retrieve` · `Update` |
| **Control Record** | `Create` · `Update` · `Grant` · `Request` · `Retrieve` |
| BQ `Performance Assessment` | `Create` · `Execute` · `Update` · `Request` · `Retrieve` |
| BQ `Campaign Direction` | `Update` · `Create` · `Retrieve` · `Request` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Promotional Events

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `Promotional Event` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `Promotional Event Management Plan` |
| **Ubicación Matrix** | Sales and Service › Marketing |

**Propósito.** Develop the plan for and oversee promotional event activity, including budget and resource management

<details><summary><b>Atributos del Control Record</b> · 8</summary>

`Promotional Event Portfolio` · `Promotional Event Type` · `Promotional Event Description` · `Promotional Event Metrics` · `Promotional Event Metric Definition` · `Promotional Event Metric Goal` · `Promotional Event Schedule` · `Promotional Event Performance Record`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Market Tracking | 6 |
| Impact Assessment | 5 |
| Participation | 5 |

**Interfaz.** Action Terms: `Execute` · `Update` · `Request` · `Grant` · `Retrieve` · `Create`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 18 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| BQ `Market Tracking` | `Execute` · `Update` · `Retrieve` · `Request` |
| BQ `Impact Assessment` | `Update` · `Execute` · `Request` · `Create` · `Retrieve` |
| BQ `Participation` | `Request` · `Update` · `Create` · `Retrieve` |
| **Control Record** | `Request` · `Grant` · `Retrieve` · `Update` · `Create` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Prospect Campaign Design

| | |
|---|---|
| **Patrón funcional** | `Design` |
| **Tipo de activo** | `Prospect Campaign` |
| **Artefacto genérico** | `Specification` |
| **Control Record** | `Prospect Campaign Specification` |
| **Ubicación Matrix** | Sales and Service › Marketing |

**Propósito.** Design and refine prospect campaign specifications based on their impact

<details><summary><b>Atributos del Control Record</b> · 23</summary>

`Prospect Campaign Type` · `Prospect Campaign Description` · `Prospect Campaign Metrics` · `Prospect Campaign Metric Definition` · `Prospect Campaign Metric Goal` · `Prospect Campaign Specification` · `Prospect Campaign ProductandService Usage` · `Prospect Campaign ProductandService Type` · `ProductandService Campaign Engagement Description` · `ProductandService Campaign Transfer Pricing Arrangement` · `Prospect Campaign Execution Guidelines` · `Prospect Campaign Eligibility` · `Prospect Campaign Qualifications` · `Prospect Campaign Interaction Guide` · `Prospect Campaign Consumables` · `Prospect Campaign Consumable Type` · `Prospect Campaign Consumable Description` · `Prospect Campaign Performance Record` · `Prospect Campaign Procedure Instance Reference` · `Employee or Business Unit Reference` · `Prospect Campaign Procedure Set-up` · `Prospect Campaign Procedure Version Number` · `Prospect Campaign Procedure Result`

</details>

**Interfaz.** Action Terms: `Execute` · `Update` · `Control` · `Create` · `Exchange` · `Capture` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 8 | 2 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Execute` · `Update` · `Control` · `Create` · `Exchange` · `Capture` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Customer Campaign Management

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `Customer Campaign Portfolio` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `Customer Campaign Portfolio Management Plan` |
| **Ubicación Matrix** | Sales and Service › Marketing |

**Propósito.** Assess the coverage and impact of internal/customer campaigns and redirect campaign development and execution activity accordingly

<details><summary><b>Atributos del Control Record</b> · 12</summary>

`Customer Campaign Portfolio` · `Customer Campaign Type` · `Customer Campaign Description` · `Customer Campaign Metrics` · `Customer Campaign Metric Definition` · `Customer Campaign Metric Goal` · `Customer Campaign Performance Record` · `Customer Campaign Procedure Instance Reference` · `Employee/Business Unit Reference` · `Customer Campaign Procedure Set-up` · `Customer Campaign Procedure Version Number` · `Customer Campaign Procedure Result`

</details>

**Behavior Qualifiers** · 7

| Behavior Qualifier | Atributos |
|---|---:|
| Competitive Assessment | 8 |
| Impact Assessment | 8 |
| Capability Oversight | 8 |
| Coverage Planning | 8 |
| Market Tracking | 8 |
| Performance Assessment | 5 |
| Campaign Direction | 2 |

**Interfaz.** Action Terms: `Create` · `Update` · `Request` · `Grant` · `Retrieve` · `Execute`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 18 | 16 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Create` · `Update` · `Request` · `Grant` · `Retrieve` |
| BQ `Market Tracking` | `Update` · `Execute` · `Retrieve` · `Request` |
| BQ `Performance Assessment` | `Create` · `Update` · `Retrieve` · `Execute` · `Request` |
| BQ `Campaign Direction` | `Create` · `Update` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Customer Campaign Design

| | |
|---|---|
| **Patrón funcional** | `Design` |
| **Tipo de activo** | `Customer Campaign` |
| **Artefacto genérico** | `Specification` |
| **Control Record** | `Customer Campaign Specification` |
| **Ubicación Matrix** | Sales and Service › Marketing |

**Propósito.** Design and refine customer campaign specifications based on their impact

<details><summary><b>Atributos del Control Record</b> · 23</summary>

`Customer Campaign Type` · `Customer Campaign Description` · `Customer Campaign Metrics` · `Customer Campaign Metric Definition` · `Customer Campaign Metric Goal` · `Customer Campaign Specification` · `Customer Campaign Product and Service Usage` · `Customer Campaign Product and Service Type` · `Product and Service Campaign Engagement Description` · `Product and Service Campaign Transfer Pricing Arrangement` · `Customer Campaign Execution Guidelines` · `Customer Campaign Eligibility` · `Customer Campaign Qualifications` · `Customer Campaign Interaction Guide` · `Customer Campaign Consumables` · `Customer Campaign Consumable Type` · `Customer Campaign Consumable Description` · `Customer Campaign Performance Record` · `Customer Campaign Procedure Instance Reference` · `Employee/Business Unit Reference` · `Customer Campaign Procedure Set-up` · `Customer Campaign Procedure Version Number` · `Customer Campaign Procedure Result`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Engagement Model | 5 |
| Execution Approach | 5 |
| Support Capabilities | 5 |
| Requirements Definition | 5 |

**Interfaz.** Action Terms: `Update` · `Create` · `Control` · `Exchange` · `Capture` · `Execute` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 8 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Update` · `Create` · `Control` · `Exchange` · `Capture` · `Execute` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Customer Surveys

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Customer Survey` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Customer Survey Procedure` |
| **Ubicación Matrix** | Sales and Service › Marketing |

**Propósito.** Define and execute and analyze customer surveys

<details><summary><b>Atributos del Control Record</b> · 13</summary>

`Customer Survey Type` · `Customer Survey Description` · `Employee/Business Unit Reference` · `Set-up` · `Version Number` · `Customer Survey Schedule` · `Customer Survey Consumables Inventory` · `Customer Survey Consumable Type` · `Customer Survey Consumable Holding` · `Date Type` · `Date` · `Result` · `Customer Survey Reference`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Definition | 4 |
| Survey Analysis | 1 |
| Participant Selection | 2 |
| Execution | 6 |

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Prospect Campaign Management

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `Prospect Campaign Portfolio` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `Prospect Campaign Portfolio Management Plan` |
| **Ubicación Matrix** | Sales and Service › Marketing |

**Propósito.** Assess the coverage and impact of external/prospect campaigns and redirect campaign development and execution activity accordingly

<details><summary><b>Atributos del Control Record</b> · 12</summary>

`Prospect Campaign Portfolio` · `Prospect Campaign Type` · `Prospect Campaign Description` · `Prospect Campaign Metrics` · `Prospect Campaign Metric Definition` · `Prospect Campaign Metric Goal` · `Prospect Campaign Performance Record` · `Prospect Campaign Procedure Instance Reference` · `Employee or Business Unit Reference` · `Prospect Campaign Procedure Set-up` · `Prospect Campaign Procedure Version Number` · `Prospect Campaign Procedure Result`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Market Tracking | 8 |
| Performance Assessment | 5 |
| Campaign Direction | 2 |

**Interfaz.** Action Terms: `Grant` · `Request` · `Create` · `Retrieve` · `Update` · `Execute`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 18 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Grant` · `Request` · `Retrieve` · `Create` · `Update` |
| BQ `Market Tracking` | `Request` · `Update` · `Execute` · `Retrieve` |
| BQ `Campaign Direction` | `Create` · `Request` · `Update` · `Retrieve` |
| BQ `Performance Assessment` | `Update` · `Create` · `Retrieve` · `Execute` · `Request` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Prospect Campaign Execution

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Prospect Campaign` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Prospect Campaign Procedure` |
| **Ubicación Matrix** | Sales and Service › Sales |

**Propósito.** Execute a prospect campaign (version) and track and respond to impact

<details><summary><b>Atributos del Control Record</b> · 14</summary>

`Prospect Campaign Type` · `Prospect Campaign Description` · `Employee or Business Unit Reference` · `Set-up` · `Version Number` · `Prospect Campaign Schedule` · `Prospect Campaign Consumables Inventory` · `Prospect Campaign Consumable Type` · `Prospect Campaign Consumable Holding` · `Date Type` · `Date` · `Result` · `Prospect Identification` · `Party Lifecycle Management Procedure Instance Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Candidate Selection | 3 |
| Execution | 6 |
| Analysis Feedback | 2 |

**Interfaz.** Action Terms: `Initiate` · `Control` · `Execute` · `Retrieve` · `Update` · `Exchange` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 18 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Control` · `Execute` · `Retrieve` · `Update` · `Exchange` · `Request` |
| BQ `Execution` | `Update` · `Retrieve` · `Request` · `Initiate` |
| BQ `Candidate Selection` | `Update` · `Exchange` · `Retrieve` |
| BQ `Analysis Feedback` | `Initiate` · `Update` · `Retrieve` · `Request` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Party Lifecycle Management

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Party Relationship` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Party Relationship Administrative Plan` |
| **Ubicación Matrix** | Sales and Service › Sales |

**Propósito.** This service domain tracks the state of a party relationship with the bank from the initial checks made during the establishment of a new party connection and subsequently maintained as necessary over the duration of the relationship. The checks and the maintenance requirements will vary by party type and jurisdiction. The checks cover bank specific and legal and regulatory considerations and may be updated based on a standard schedule or by request in specific circumstances.

<details><summary><b>Atributos del Control Record</b> · 11</summary>

`Customer Reference` · `Party Reference` · `Party Relationship Type` · `Party Life-cycle Maintenance Schedule` · `Party Life-cycle Maintenance Task` · `Party Life-cycle Maintenance Task Type` · `Party Life-cycle Maintenance Work Products` · `Party Life-cycle Maintenance Task Result` · `Customer Precedent Profile Update Log` · `Party Relationship Lifecycle Status` · `Party Relationship Lifecycle Phase`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Identity Proofing | 10 |
| Qualification | 9 |
| Documentation | 3 |
| Precedents | 4 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Exchange` · `Execute` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 15 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Exchange` · `Execute` · `Request` · `Retrieve` |
| BQ `Qualification` | `Retrieve` |
| BQ `Documentation` | `Update` · `Execute` · `Request` · `Retrieve` |
| BQ `Precedents` | `Update` · `Retrieve` |
| BQ `Identity Proofing` | `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Lead and Opportunity Management

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Leadand Opportunity` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Leadand Opportunity Procedure` |
| **Ubicación Matrix** | Sales and Service › Sales |

**Propósito.** This service domain captures, classifies and track sales lead/opportunities with established clients for additional products or services. It handles the processing of the opportunity through to the point of formal offer processing.

<details><summary><b>Atributos del Control Record</b> · 9</summary>

`Customer Reference` · `Customer Campaign Reference` · `Customer Campaign Type` · `Customer Campaign Version Number` · `ProductandService Type` · `Product Instance Reference` · `Employee/Business Unit Reference` · `Lead and Opportunity Description` · `Date/Time/Location`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Development | 9 |

**Interfaz.** Action Terms: `Update` · `Initiate` · `Control` · `Exchange` · `Retrieve` · `Execute` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 10 | 4 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Update` · `Initiate` · `Control` · `Exchange` · `Retrieve` |
| BQ `Development` | `Update` · `Execute` · `Request` · `Initiate` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Customer Campaign Execution

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Customer Campaign` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Customer Campaign Procedure` |
| **Ubicación Matrix** | Sales and Service › Sales |

**Propósito.** Execute a customer campaign version and track and respond to impact

<details><summary><b>Atributos del Control Record</b> · 14</summary>

`Customer Campaign Type` · `Customer Campaign Description` · `Employee or Business Unit Reference` · `Set-up` · `Version Number` · `Customer Campaign Schedule` · `Customer Campaign Consumables Inventory` · `Customer Campaign Consumable Type` · `Customer Campaign Consumable Holding` · `Customer Campaign Date` · `Result` · `Lead and Opportunity Description` · `Lead and Opportunity Reference` · `Customer Portfolio Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Candidate Selection | 6 |
| Analysis Feedback | 2 |
| Execution | 6 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Exchange` · `Execute` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 18 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Exchange` · `Execute` · `Request` · `Retrieve` |
| BQ `Candidate Selection` | `Update` · `Exchange` · `Retrieve` |
| BQ `Execution` | `Initiate` · `Update` · `Request` · `Retrieve` |
| BQ `Analysis Feedback` | `Initiate` · `Update` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Customer Offer

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Customer Offer` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Customer Offer Procedure` |
| **Ubicación Matrix** | Sales and Service › Sales |

**Propósito.** This service domain orchestrates the processing of a product offer for a new or established customer

<details><summary><b>Atributos del Control Record</b> · 13</summary>

`Customer Reference` · `Party Reference` · `Product and Service Type` · `Customer Offer Processing Schedule` · `Customer Offer Processing Task` · `Customer Offer Processing Task Type` · `Employee/Business Unit Reference` · `Customer Offer Processing Task Work Products` · `Customer Offer Processing Task Result` · `Customer Offer Involved Party` · `Customer Offer Reference` · `Product Agreement Reference` · `Product and Service Reference`

</details>

**Behavior Qualifiers** · 10

| Behavior Qualifier | Atributos |
|---|---:|
| Facility Application | 8 |
| Disclosures | 4 |
| Credit | 3 |
| Underwriting | 4 |
| Compliance | 5 |
| Audit | 5 |
| Collateral Allocation | 4 |
| Booking | 3 |
| Agreement | 2 |
| Product Initialization | 1 |

**Interfaz.** Action Terms: `Update` · `Control` · `Exchange` · `Retrieve` · `Execute` · `Request` · `Initiate`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 34 | 24 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Update` · `Control` · `Execute` · `Retrieve` · `Exchange` · `Request` · `Initiate` |
| BQ `Facility Application` | `Exchange` · `Retrieve` · `Update` |
| BQ `Disclosures` | `Update` · `Exchange` · `Retrieve` |
| BQ `Underwriting` | `Update` · `Retrieve` |
| BQ `Credit` | `Update` · `Retrieve` |
| BQ `Compliance` | `Update` · `Retrieve` |
| BQ `Audit` | `Update` · `Retrieve` |
| BQ `Collateral Allocation` | `Update` · `Exchange` · `Retrieve` |
| BQ `Booking` | `Update` · `Retrieve` |
| BQ `Correspondence and Documents` | `Update` · `Exchange` · `Retrieve` |
| BQ `Agreement` | `Update` · `Exchange` · `Retrieve` |
| BQ `Product Initialization` | `Update` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Sales Planning

| | |
|---|---|
| **Patrón funcional** | `Direct` |
| **Tipo de activo** | `Marketing And Sales` |
| **Artefacto genérico** | `Strategy` |
| **Control Record** | `Marketing And Sales Strategy` |
| **Ubicación Matrix** | Sales and Service › Sales |

[↑ Índice](README.md)

---

## Underwriting

| | |
|---|---|
| **Patrón funcional** | `Assess` |
| **Tipo de activo** | `Underwriting` |
| **Artefacto genérico** | `Assessment` |
| **Control Record** | `Underwriting Assessment` |
| **Ubicación Matrix** | Sales and Service › Sales |

**Propósito.** This service domain manages the underwriting decision process for products as appropriate (including many loan types and some insurance products)

<details><summary><b>Atributos del Control Record</b> · 27</summary>

`Underwriting Guidelines` · `Required Customer Employment History Details` · `Required Customer Debt/Asset Statement` · `Required Customer Credit Assessment` · `Required Collateral Coverage` · `Required Customer Product and Service Payment History` · `Required Customer Documents` · `Proposed Transaction Details` · `Product Instance Reference` · `Proposed Loan Terms` · `Proposed Loan Amount` · `Loan Purpose` · `Customer Reference` · `Customer Reference Details` · `Customer Product Eligibility Terms` · `Customer Employment History` · `Customer Income Statement` · `Customer Debt Statement` · `Customer Asset Statement` · `Customer Credit Assessment` · `Customer Product and Service Payment History` · `Collateral Item Reference` · `Collateral Item Type` · `Collateral Item Valuation` · `Document Reference` · `Decision` · `Work Product`

</details>

**Interfaz.** Action Terms: `Evaluate` · `Update` · `Execute` · `Request` · `Exchange` · `Grant` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 7 | 2 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Evaluate` · `Update` · `Execute` · `Request` · `Exchange` · `Grant` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Commission Agreement

| | |
|---|---|
| **Patrón funcional** | `Agree Terms` |
| **Tipo de activo** | `Employee Commission` |
| **Artefacto genérico** | `Agreement` |
| **Control Record** | `Employee Commission Agreement` |
| **Ubicación Matrix** | Sales and Service › Sales |

**Propósito.** Maintain and administer the terms and transactions for employee and broker commissions

<details><summary><b>Atributos del Control Record</b> · 15</summary>

`Parameter Type` · `Selected Option` · `Type` · `Reference` · `Request` · `Schedule` · `Status` · `Associated Party` · `Customer Reference` · `Obligation` · `Entitlement` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Account Reference`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Commission Term | 6 |

**Interfaz.** Action Terms: `Initiate` · `Request` · `Control` · `Exchange` · `Grant` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 14 | 6 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Request` · `Control` · `Exchange` · `Grant` · `Retrieve` · `Update` |
| BQ `Commission Term` | `Initiate` · `Control` · `Update` · `Grant` · `Retrieve` · `Exchange` · `Request` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Commissions

| | |
|---|---|
| **Patrón funcional** | `Transact` |
| **Tipo de activo** | `Commission` |
| **Artefacto genérico** | `Transaction` |
| **Control Record** | `Commission Transaction` |
| **Ubicación Matrix** | Sales and Service › Sales |

**Propósito.** The service domain processes commissions for transactions for eligible employees

<details><summary><b>Atributos del Control Record</b> · 6</summary>

`Parameter Type` · `Selected Option` · `Status` · `Type` · `Transaction Type` · `Transaction`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Calculation | 7 |
| Confirmation | 7 |
| Payment | 7 |

**Interfaz.** Action Terms: `Retrieve` · `Control` · `Exchange` · `Execute` · `Initiate` · `Request` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 17 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Retrieve` · `Control` · `Exchange` · `Execute` · `Initiate` · `Request` · `Update` |
| BQ `Confirmation` | `Exchange` · `Initiate` · `Retrieve` · `Update` |
| BQ `Calculation` | `Exchange` · `Retrieve` · `Update` |
| BQ `Payment` | `Exchange` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Product Matching

| | |
|---|---|
| **Patrón funcional** | `Assess` |
| **Tipo de activo** | `Product to Customer Combination` |
| **Artefacto genérico** | `Assessment` |
| **Control Record** | `Product to Customer Combination Assessment` |
| **Ubicación Matrix** | Sales and Service › Sales |

**Propósito.** Capability used to match eligible product and product combinations to a customer based on prevailing conditions such as customer type, product interest, solicitation/retention, campaign alignment

<details><summary><b>Atributos del Control Record</b> · 11</summary>

`Product/ Customer Combination Assessment Parameter Type` · `Product/ Customer Combination Assessment Selected Option` · `Product/ Customer Combination Assessment Type` · `Product/ Customer Combination Assessment Reference` · `Product/ Customer Combination Assessment Request` · `Product/ Customer Combination Assessment Schedule` · `Product/ Customer Combination Assessment Status` · `Product/ Customer Combination Assessment Usage Log` · `Product/ Customer Combination Assessment Requester Reference` · `Product/ Customer Combination Assessment Associated Party` · `Product/ Customer Combination Assessment Service Provider Reference`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Product Type Selection | 7 |
| Product Eligibility | 7 |
| Context Criteria | 7 |
| Bank and Campaign Alignment | 7 |

**Interfaz.** Action Terms: `Exchange` · `Execute` · `Grant` · `Evaluate` · `Retrieve` · `Update` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 19 | 12 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Exchange` · `Execute` · `Grant` · `Evaluate` · `Retrieve` · `Update` · `Request` |
| BQ `Bank and Campaign Alignment` | `Evaluate` · `Retrieve` · `Update` |
| BQ `Product Eligibility` | `Evaluate` · `Retrieve` · `Update` |
| BQ `Context Criteria` | `Evaluate` · `Retrieve` · `Update` |
| BQ `Product Type Selection` | `Evaluate` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Product Expert Sales Support

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Sales Specialist Support` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Sales Specialist Support Administrative Plan` |
| **Ubicación Matrix** | Sales and Service › Sales |

**Propósito.** Administer the availability and allocation of product specialists to support sales activity

<details><summary><b>Atributos del Control Record</b> · 8</summary>

`Sales Specialist Support Resource Allocation Service Schedule` · `Sales Specialist Support Resource Reference` · `Sales Specialist Support Resource Record` · `Sales Specialist Support Resource Qualification Profile` · `Sales Specialist Support Location Reference` · `Sales Specialist Support Resource Availability Schedule` · `Sales Specialist Support Resource Status` · `Sales Specialist Support Resource Assignment Record`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Assignment | 8 |

**Interfaz.** Action Terms: `Retrieve` · `Create` · `Update` · `Request` · `Exchange` · `Capture`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 10 | 4 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Retrieve` · `Create` · `Update` · `Request` |
| BQ `Assignment` | `Create` · `Request` · `Update` · `Exchange` · `Capture` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Product Sales Support

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Product Sales Support` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Product Sales Support Administrative Plan` |
| **Ubicación Matrix** | Sales and Service › Sales |

**Propósito.** This Service Domain administers customer access to product specialists

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Budget Type` · `Budget` · `Assignment` · `Duty` · `Associated Party` · `Budget Balance` · `Subject Matter` · `Type` · `Reference` · `Description`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Staff Availability Tracking | 8 |
| Staff Assignment | 8 |

**Interfaz.** Action Terms: `Control` · `Create` · `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 20 | 11 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Create` · `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Staff Assignment` | `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Staff Availability Tracking` | `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Sales Product

| | |
|---|---|
| **Patrón funcional** | `Agree Terms` |
| **Tipo de activo** | `Product and Service` |
| **Artefacto genérico** | `Agreement` |
| **Control Record** | `Product and Service Agreement` |
| **Ubicación Matrix** | Sales and Service › Sales |

**Propósito.** A representation of a product as sold to a customer, covering the operational fulfillment requirements

<details><summary><b>Atributos del Control Record</b> · 18</summary>

`Product Instance Reference` · `Underlying Product Instance Reference` · `Customer Reference` · `Bank Branch/Location Reference` · `Tax Reference` · `Entitlement Option Definition` · `Entitlement Option Setting` · `Restriction Option Definition` · `Restriction Option Setting` · `Linked Accounts` · `Link Type` · `Account Details` · `Position Limits` · `Position Limit Type` · `Position Limit Settings` · `Position Limit Value` · `Date Type` · `Date`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Operational Term | 9 |

**Interfaz.** Action Terms: `Evaluate` · `Update` · `Exchange` · `Retrieve` · `Control` · `Grant`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 9 | 4 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Evaluate` · `Update` · `Retrieve` · `Control` |
| BQ `Operational Term` | `Update` · `Exchange` · `Evaluate` · `Grant` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Customer Relationship Management

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `Customer Relationship` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `Customer Relationship Management Plan` |
| **Ubicación Matrix** | Sales and Service › Customer Management |

**Propósito.** This service domain develops and executes a customer plan to maintain and build a customer relationship

<details><summary><b>Atributos del Control Record</b> · 12</summary>

`Customer Reference` · `Employee/Business Unit Reference` · `Customer Relationship Rating Type` · `Customer Relationship Rating` · `Customer Insight Type` · `Customer Insight Description` · `Customer Budget` · `Customer Product Coverage` · `Customer Product Usage` · `Customer Product Eligibility Profile` · `Customer Sales Plan` · `Customer Profitability`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Incident | 6 |
| Development | 7 |
| Contact | 7 |

**Interfaz.** Action Terms: `Create` · `Update` · `Control` · `Request` · `Grant` · `Exchange` · `Retrieve` · `Capture`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 22 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Create` · `Update` · `Control` · `Request` · `Grant` · `Exchange` · `Retrieve` |
| BQ `Development` | `Create` · `Update` · `Exchange` · `Request` · `Retrieve` |
| BQ `Incident` | `Create` · `Update` · `Control` · `Exchange` · `Capture` · `Retrieve` |
| BQ `Contact` | `Create` · `Update` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Customer Product And Service Eligibility

| | |
|---|---|
| **Patrón funcional** | `Assess` |
| **Tipo de activo** | `Customer Eligibility` |
| **Artefacto genérico** | `Assessment` |
| **Control Record** | `Customer Eligibility Assessment` |
| **Ubicación Matrix** | Sales and Service › Customer Management |

**Propósito.** This Service Domain maintains a list of products and services for which a customer is eligible

<details><summary><b>Atributos del Control Record</b> · 6</summary>

`Customer Reference` · `Customer Product and Service Profile` · `Product and Service Type` · `Customer Product and Service Type Eligibility` · `Customer Product and Service Type Usage` · `Date`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Eligibility Check | 1 |
| Next Best | 3 |

**Interfaz.** Action Terms: `Evaluate` · `Update` · `Exchange` · `Execute` · `Request` · `Grant` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 11 | 6 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Evaluate` · `Update` · `Exchange` · `Execute` · `Request` · `Grant` · `Retrieve` |
| BQ `Eligibility Check` | `Retrieve` · `Evaluate` |
| BQ `Next Best` | `Update` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Customer Agreement

| | |
|---|---|
| **Patrón funcional** | `Agree Terms` |
| **Tipo de activo** | `Customer` |
| **Artefacto genérico** | `Agreement` |
| **Control Record** | `Customer Agreement` |
| **Ubicación Matrix** | Sales and Service › Customer Management |

**Propósito.** This service domain maintains the master customer agreement/legal contract

<details><summary><b>Atributos del Control Record</b> · 9</summary>

`Customer Reference` · `Legal Entity Reference` · `Agreement Type` · `Agreement Jurisdiction` · `Agreement Valid From/To Date` · `Agreement Signatories/Responsible Parties` · `Document Directory Entry Instance Reference` · `Sales Product Agreement Reference` · `Party Life-cycle Management Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Legal Term | 3 |
| Regulatory Term | 3 |
| Policy Term | 3 |

**Interfaz.** Action Terms: `Evaluate` · `Update` · `Exchange` · `Control` · `Request` · `Grant` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 16 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Evaluate` · `Update` · `Exchange` · `Control` · `Request` · `Grant` · `Retrieve` |
| BQ `Legal Term` | `Evaluate` · `Update` · `Retrieve` |
| BQ `Regulatory Term` | `Evaluate` · `Update` · `Retrieve` |
| BQ `Policy Term` | `Evaluate` · `Update` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Sales Product Agreement

| | |
|---|---|
| **Patrón funcional** | `Agree Terms` |
| **Tipo de activo** | `Sales Product Agreement` |
| **Artefacto genérico** | `Agreement` |
| **Control Record** | `Sales Product Agreement` |
| **Ubicación Matrix** | Sales and Service › Customer Management |

**Propósito.** This service domain maintains a structured legal agreement defining the contractual terms and conditions for an in-force product for a customer. It is subordinate to the customer's master agreement that is maintained by the Customer Agreement service domain

<details><summary><b>Atributos del Control Record</b> · 11</summary>

`Customer Reference` · `Legal Entity Reference` · `Product Instance Reference` · `Agreement Type` · `Agreement Jurisdiction` · `Agreement Valid From/To Date` · `Agreement Signatories/Responsible Parties` · `Document Directory Entry Instance Reference` · `Customer Agreement Reference` · `Party Life-cycle Management Reference` · `Banking Product Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Legal Term | 3 |
| Regulatory Term | 3 |
| Policy Term | 3 |

**Interfaz.** Action Terms: `Evaluate` · `Update` · `Control` · `Exchange` · `Request` · `Grant` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 16 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Evaluate` · `Update` · `Control` · `Exchange` · `Request` · `Grant` · `Retrieve` |
| BQ `Legal Term` | `Evaluate` · `Retrieve` · `Update` |
| BQ `Regulatory Term` | `Evaluate` · `Update` · `Retrieve` |
| BQ `Policy Term` | `Evaluate` · `Update` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Customer Access Entitlement

| | |
|---|---|
| **Patrón funcional** | `Agree Terms` |
| **Tipo de activo** | `Customer Access Profile` |
| **Artefacto genérico** | `Agreement` |
| **Control Record** | `Customer Access Profile Agreement` |
| **Ubicación Matrix** | Sales and Service › Customer Management |

**Propósito.** This service domain maintains the details of the allowed channel/device based access to products and services that the customer has in place

<details><summary><b>Atributos del Control Record</b> · 6</summary>

`Customer Reference` · `Customer Access Profile Record` · `Customer Access Agreement Valid From/To Date` · `Customer Access Agreement Signatures/Responsible Parties` · `Document Directory Entry Instance Reference` · `Customer Access Arrangement`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Restrictions | 6 |
| Preferences | 7 |

**Interfaz.** Action Terms: `Evaluate` · `Update` · `Exchange` · `Request` · `Control` · `Grant` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 13 | 6 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Evaluate` · `Update` · `Exchange` · `Request` · `Control` · `Grant` · `Retrieve` |
| BQ `Restrictions` | `Update` · `Evaluate` · `Retrieve` |
| BQ `Preferences` | `Evaluate` · `Update` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Customer Behavior Insights

| | |
|---|---|
| **Patrón funcional** | `Analyze` |
| **Tipo de activo** | `Customer Behavior` |
| **Artefacto genérico** | `Analysis` |
| **Control Record** | `Customer Behavior Analysis` |
| **Ubicación Matrix** | Sales and Service › Customer Management |

**Propósito.** This service domain applies behavioral analysis to customer event history to maintain a range of customer ratings/scores

<details><summary><b>Atributos del Control Record</b> · 11</summary>

`Customer Reference` · `Customer Behavior Insights Analysis Schedule` · `Customer Behavior Insights Analysis Record` · `Customer Insight Type` · `Customer Insight` · `Customer Insight Calculation Date` · `Customer Behavior Insights Analysis` · `Customer Behavior Insights Analysis Model Reference` · `Customer Behavior Insights Analysis Report Reference` · `Customer Behavior Insights Analysis Log Reference` · `Customer Behavior Insights Analysis Document Reference`

</details>

**Behavior Qualifiers** · 6

| Behavior Qualifier | Atributos |
|---|---:|
| Customer Engagement Insight | 8 |
| Customer Psychographic Insight | 8 |
| Customer Satisfaction and Sentiment Insight | 8 |
| Customer Journey Insight | 8 |
| Customer Retention and Churn Insight | 8 |
| Customer Demographic Insight | 8 |

**Interfaz.** Action Terms: `Evaluate` · `Exchange` · `Request` · `Execute` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 9 | 16 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Evaluate` · `Exchange` · `Request` · `Execute` · `Retrieve` |
| BQ `Insight` | `Exchange` · `Execute` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Customer Credit Rating

| | |
|---|---|
| **Patrón funcional** | `Monitor` |
| **Tipo de activo** | `Customer Credit Rating` |
| **Artefacto genérico** | `State` |
| **Control Record** | `Customer Credit Rating State` |
| **Ubicación Matrix** | Sales and Service › Customer Management |

**Propósito.** This service domain maintains and administers the bank credit assessment for customers

<details><summary><b>Atributos del Control Record</b> · 14</summary>

`Customer Reference` · `Customer Credit Rating Status Type` · `Customer Credit Rating Schedule` · `Customer Credit Rating Assessment Record` · `Assessment Customer Behavior Model Reference` · `Credit Rating Assessment Type` · `Credit Rating Assessment Date` · `Credit Rating Assessment Work Products` · `Credit Rating Assessment Result` · `Customer Credit Rating Record` · `Customer Credit Rating State` · `Customer Credit Rating Assessment` · `Customer Credit Rating Narrative` · `Customer Credit Rating Date`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Alerts | 5 |
| Internal Reporting | 3 |
| External Reporting | 5 |

**Interfaz.** Action Terms: `Initiate` · `Control` · `Exchange` · `Execute` · `Request` · `Retrieve` · `Capture`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 12 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Control` · `Exchange` · `Execute` · `Request` · `Retrieve` |
| BQ `Alerts` | `Capture` · `Retrieve` |
| BQ `Internal Reporting` | `Capture` · `Retrieve` |
| BQ `External Reporting` | `Capture` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Account Recovery

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Account Recovery` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Account Recovery Procedure` |
| **Ubicación Matrix** | Sales and Service › Customer Management |

**Propósito.** This service domain handles the restructuring of a distressed account (loan) after standard recovery procedures have been exhausted

<details><summary><b>Atributos del Control Record</b> · 27</summary>

`Account Recovery Case Type` · `Product Instance Reference` · `Linked Product Instance Reference` · `Customer Reference` · `Employee/Business Unit Reference` · `Account Number` · `Bank Branch/Location Reference` · `Date Type` · `Date` · `Involved Party Reference` · `Involved Party Obligation/Entitlement` · `Account Type` · `Account Currency` · `Account Limit Type` · `Account Limit` · `Allowed Access` · `Tax Reference` · `Account Status` · `Collateral Asset Allocation Profile` · `Collateral Type` · `Collateral Asset Description` · `Transaction Record` · `Account Recovery Case Work Products` · `Document Reference` · `Customer Commentary` · `Account Recovery Case Resolution Schedule` · `Account Recovery Case Status`

</details>

**Behavior Qualifiers** · 5

| Behavior Qualifier | Atributos |
|---|---:|
| Assessment | 1 |
| Planning | 2 |
| Writedown | 2 |
| Negotiation | 6 |
| Modification | 2 |

**Interfaz.** Action Terms: `Exchange` · `Update` · `Initiate` · `Retrieve` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 17 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| BQ `Writedown` | `Exchange` · `Update` |
| BQ `Negotiation` | `Update` · `Exchange` · `Request` · `Retrieve` |
| BQ `Modification` | `Exchange` · `Update` · `Retrieve` |
| BQ `Planning` | `Update` · `Retrieve` |
| **Control Record** | `Initiate` · `Update` · `Exchange` · `Retrieve` |
| BQ `Assessment` | `Update` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Customer Event History

| | |
|---|---|
| **Patrón funcional** | `Track` |
| **Tipo de activo** | `Customer Event` |
| **Artefacto genérico** | `Log` |
| **Control Record** | `Customer Event Log` |
| **Ubicación Matrix** | Sales and Service › Customer Management |

**Propósito.** This service domain captures, classifies and stores relationship, servicing and product fulfillment related customer events

<details><summary><b>Atributos del Control Record</b> · 4</summary>

`Customer Reference` · `Customer Event Reference` · `Reference` · `Customer Event Type`

</details>

**Behavior Qualifiers** · 6

| Behavior Qualifier | Atributos |
|---|---:|
| Sales | 8 |
| Servicing | 10 |
| Product Processing | 8 |
| Fraud | 7 |
| Life | 6 |
| Relationship | 6 |

**Interfaz.** Action Terms: `Update` · `Control` · `Retrieve` · `Initiate` · `Capture`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 22 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| BQ `Relationship` | `Update` · `Capture` · `Retrieve` |
| **Control Record** | `Control` · `Retrieve` · `Initiate` · `Update` |
| BQ `Sales` | `Update` · `Capture` · `Retrieve` |
| BQ `Servicing` | `Update` · `Capture` · `Retrieve` |
| BQ `Product Processing` | `Update` · `Capture` · `Retrieve` |
| BQ `Fraud` | `Update` · `Retrieve` · `Capture` |
| BQ `Life` | `Update` · `Retrieve` · `Capture` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Party Reference Data Directory

| | |
|---|---|
| **Patrón funcional** | `Catalog` |
| **Tipo de activo** | `Party Reference Data` |
| **Artefacto genérico** | `Directory Entry` |
| **Control Record** | `Party Reference Data Directory Entry` |
| **Ubicación Matrix** | Sales and Service › Customer Management |

**Propósito.** This service domain maintains a range of party reference information covering aspects including general reference details, contacts and associations and demographic information

<details><summary><b>Atributos del Control Record</b> · 4</summary>

`Party Reference` · `Directory Entry Date Type` · `Directory Entry Date` · `Party Type`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Reference | 24 |
| Associations | 9 |
| Demographics | 6 |
| Bank Relations | 3 |

**Interfaz.** Action Terms: `Register` · `Control` · `Update` · `Retrieve` · `Request` · `Execute` · `Exchange`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 17 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Register` · `Control` · `Update` · `Retrieve` · `Request` · `Execute` · `Exchange` |
| BQ `Demographics` | `Exchange` · `Update` · `Retrieve` |
| BQ `Reference` | `Update` · `Retrieve` |
| BQ `Associations` | `Retrieve` · `Update` · `Register` |
| BQ `Bank Relations` | `Update` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Customer Proposition

| | |
|---|---|
| **Patrón funcional** | `Agree Terms` |
| **Tipo de activo** | `Customer Proposition` |
| **Artefacto genérico** | `Agreement` |
| **Control Record** | `Customer Proposition Agreement` |
| **Ubicación Matrix** | Sales and Service › Customer Management |

**Propósito.** This Service Domain maintains bank and customer defined requirements spanning all products and services

<details><summary><b>Atributos del Control Record</b> · 19</summary>

`Parameter Type` · `Selected Option` · `Type` · `Reference` · `Discharge Request` · `Discharge Schedule` · `Status` · `Associated Party` · `Customer Reference` · `Obligation` · `Entitlement` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Account Reference` · `Subject Matter` · `Product Reference` · `Calendar Reference` · `Associated Agreement Reference`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Customer Defined Product and Service Term | 6 |
| Bank Defined Product and Service Term | 6 |

**Interfaz.** Action Terms: `Control` · `Evaluate` · `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` · `Execute`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 21 | 11 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Evaluate` · `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Bank Defined Product and Service Term` | `Evaluate` · `Exchange` · `Notify` · `Request` · `Retrieve` · `Update` · `Execute` |
| BQ `Customer Defined Product and Service Term` | `Evaluate` · `Exchange` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Customer Product and Service Directory

| | |
|---|---|
| **Patrón funcional** | `Catalog` |
| **Tipo de activo** | `Customer Product And Service` |
| **Artefacto genérico** | `Directory Entry` |
| **Control Record** | `Customer Product And Service Directory Entry` |
| **Ubicación Matrix** | Sales and Service › Customer Management |

**Propósito.** This Service Domain maintains the most important details of all the products and services that a customer has acquired from the bank

<details><summary><b>Atributos del Control Record</b> · 12</summary>

`Description` · `Schedule` · `Version` · `Status` · `Usage Log` · `Update Log` · `Service Configuration` · `Instance Reference` · `Customer Reference` · `Product Agreement Reference` · `Servicer Reference` · `Service Agreement Reference`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Service | 7 |
| Product | 9 |

**Interfaz.** Action Terms: `Control` · `Execute` · `Notify` · `Register` · `Request` · `Update` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 19 | 11 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Execute` · `Notify` · `Register` · `Request` · `Update` · `Retrieve` |
| BQ `Product` | `Execute` · `Notify` · `Register` · `Request` · `Retrieve` · `Update` |
| BQ `Service` | `Execute` · `Notify` · `Register` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Customer Financial Insights

| | |
|---|---|
| **Patrón funcional** | `Analyze` |
| **Tipo de activo** | `Customer Financial Position` |
| **Artefacto genérico** | `Analysis` |
| **Control Record** | `Customer Financial Position Analysis` |
| **Ubicación Matrix** | Sales and Service › Customer Management |

**Propósito.** This service domain applies behavioral analysis to the customer financial history to develop financial insights

<details><summary><b>Atributos del Control Record</b> · 12</summary>

`Customer Reference` · `Customer Financial Insights Analysis Record` · `Customer Financial Insight Analysis Schedule` · `Customer Insight Calculation Date` · `Customer Insight` · `Customer Insight Type` · `Customer Financial Insights Analysis` · `Customer Financial Insights Analysis Model Reference` · `Customer Financial Insights Analysis Report Reference` · `Customer Financial Insights Analysis Document Reference` · `Customer Financial Insights Analysis Log Reference` · `Customer Financial Insights Analysis Position Reference`

</details>

**Behavior Qualifiers** · 10

| Behavior Qualifier | Atributos |
|---|---:|
| Customer Acquisition Cost | 10 |
| Revenue per Customer | 10 |
| Customer Financial Insight | 10 |
| Customer Transactional Insight | 10 |
| Profitability Analysis | 10 |
| Customer Lifetime Value | 10 |
| Retention Cost | 10 |
| Churn Cost | 10 |
| Discount and Promotion Impact | 10 |
| Segmented Financial Performance | 10 |

**Interfaz.** Action Terms: `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 1 | 22 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Customer Consent

| | |
|---|---|
| **Patrón funcional** | `Agree Terms` |
| **Tipo de activo** | `Customer Mandate` |
| **Artefacto genérico** | `Agreement` |
| **Control Record** | `Customer Mandate Agreement` |
| **Ubicación Matrix** | Sales and Service › Customer Management |

[↑ Índice](README.md)

---

## Payee Management

| | |
|---|---|
| **Patrón funcional** | `Catalog` |
| **Tipo de activo** | `Payee Alias` |
| **Artefacto genérico** | `Directory Entry` |
| **Control Record** | `Payee Alias Directory Entry` |
| **Ubicación Matrix** | Sales and Service › Customer Management |

[↑ Índice](README.md)

---

## Servicing Issue

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Servicing Issue` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Servicing Issue Procedure` |
| **Ubicación Matrix** | Sales and Service › Servicing |

**Propósito.** This Service Domain handles production customer servicing issues detected in the customer servicing environment

<details><summary><b>Atributos del Control Record</b> · 21</summary>

`Parameter Type` · `Selected Option` · `Request` · `Schedule` · `Status` · `Associated Party Reference` · `Business Unit Reference` · `Service Provider Reference` · `Financial Facility Reference` · `Employee Reference` · `Customer Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Product and Service Type` · `Product and Service Instance` · `Transaction Type` · `Transaction` · `Financial Transaction Arrangement` · `Customer Agreement Reference` · `Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Production Issue Resolution | 8 |
| Production Issue Determination | 8 |
| Production Issue Analysis | 8 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 29 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Production Issue Analysis` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Production Issue Determination` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Production Issue Resolution` | `Exchange` · `Execute` · `Notify` · `Initiate` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Customer Case Management

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `Customer Case` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `Customer Case Management Plan` |
| **Ubicación Matrix** | Sales and Service › Servicing |

**Propósito.** Track and assess case load and resolution activity

<details><summary><b>Atributos del Control Record</b> · 7</summary>

`Period` · `Customer Case Policies And Guidelines` · `Customer Case Service Performance Goals` · `Customer Case Service Schedule` · `Customer Case Service Operating Configuration` · `Customer Case Resource Plan` · `Customer Case Training Plan`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Rules | 5 |
| Performance | 7 |

**Interfaz.** Action Terms: `Create` · `Update` · `Exchange` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 11 | 6 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Create` · `Update` · `Exchange` · `Request` · `Retrieve` |
| BQ `Rules` | `Update` · `Request` · `Retrieve` |
| BQ `Performance` | `Update` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Case Root Cause Analysis

| | |
|---|---|
| **Patrón funcional** | `Analyze` |
| **Tipo de activo** | `Customer Case Root Cause` |
| **Artefacto genérico** | `Analysis` |
| **Control Record** | `Customer Case Root Cause Analysis` |
| **Ubicación Matrix** | Sales and Service › Servicing |

**Propósito.** Root cause analysis business function reviews case reports to identify possible improvements to eliminate/mitigate servicing issues

<details><summary><b>Atributos del Control Record</b> · 7</summary>

`Parameter Type` · `Selected Option` · `Request` · `Schedule` · `Status` · `Usage Log` · `Requester Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Credit and Fraud Related Issue Analysis | 4 |
| Product and Service Issue Analysis | 4 |
| Operations and Servicing Issue Analysis | 4 |

**Interfaz.** Action Terms: `Request` · `Execute` · `Retrieve` · `Initiate` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 20 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Request` · `Execute` · `Retrieve` · `Initiate` · `Update` |
| BQ `Credit and Fraud Related Issue Analysis` | `Execute` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Operations and Servicing Issue Analysis` | `Execute` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Product and Service Issue Analysis` | `Execute` · `Initiate` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Customer Case

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Customer Case` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Customer Case Procedure` |
| **Ubicación Matrix** | Sales and Service › Servicing |

**Propósito.** This service domain handles the initiation, tracking, resolution and reporting on customer cases

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Customer Case Type` · `Product Instance Reference` · `Customer Reference` · `Customer Contact Record Reference` · `Product Transaction Reference` · `Product Transaction Record` · `Case Location` · `Date` · `Employee/Business Unit Reference` · `Customer Case Resolution Schedule`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Analysis | 3 |
| Determination | 4 |
| Resolution | 6 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Exchange` · `Execute` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 14 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Exchange` · `Execute` · `Request` · `Retrieve` |
| BQ `Analysis` | `Update` · `Retrieve` |
| BQ `Determination` | `Update` · `Retrieve` |
| BQ `Resolution` | `Update` · `Exchange` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Card Case

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Card Case` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Card Case Procedure` |
| **Ubicación Matrix** | Sales and Service › Servicing |

**Propósito.** This service domain handles the processing of a customer card case, typically a disputed charge

<details><summary><b>Atributos del Control Record</b> · 27</summary>

`Card Case Type` · `Product Instance Reference` · `Customer Reference` · `Customer Contact Record Reference` · `Case Location` · `Date` · `Employee/Business Unit Reference` · `Card Transaction Reference` · `Card Transaction Record` · `Card Transaction Product Instance Reference` · `Card Holder Reference` · `Card Transaction Issued Device Reference` · `Card Transaction Network Reference` · `Card Transaction Issuing Bank Reference` · `Card Transaction Merchant Acquiring Bank Reference` · `Card Transaction Type` · `Card Transaction Currency` · `Card Transaction Amount Type` · `Card Transaction Amount` · `Card Transaction Merchant Reference` · `Card Transaction Location Reference` · `Card Transaction ProductandService Reference` · `Card Transaction Date and Time` · `Card Transaction FX Conversion Charge` · `Card Transaction Intercharge Fee` · `Card Transaction Authorization Record` · `Card Case Resolution Schedule`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Consolidation | 7 |
| Chargeback | 2 |
| Arbitration | 6 |
| Resolution | 10 |

**Interfaz.** Action Terms: `Update` · `Initiate` · `Control` · `Exchange` · `Execute` · `Retrieve` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 17 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Update` · `Initiate` · `Control` · `Exchange` · `Execute` · `Retrieve` · `Request` |
| BQ `Consolidation` | `Update` · `Retrieve` |
| BQ `Chargeback` | `Update` · `Retrieve` |
| BQ `Arbitration` | `Update` · `Exchange` · `Retrieve` |
| BQ `Resolution` | `Update` · `Exchange` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Servicing Order

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Servicing Order` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Servicing Order Procedure` |
| **Ubicación Matrix** | Sales and Service › Servicing |

**Propósito.** This service domain handles the processing of a customer servicing request as a predefined procedure. A range of standard servicing requests can be supported. The process can include a check of permissions when the request is made by a third party/service provider

<details><summary><b>Atributos del Control Record</b> · 12</summary>

`Third Party Reference` · `Third Party Servicing Mandate Reference` · `Third Party Servicing Mandate` · `Customer Reference` · `Customer Eligibility Assessment Instance Reference` · `Servicing Order Type` · `Servicing Order Task Record` · `Servicing Order Description` · `Date` · `Employee/Business Unit Reference` · `Servicing Order Work Product` · `Servicing Order Work Task Result`

</details>

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Exchange` · `Execute` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 7 | 2 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Exchange` · `Execute` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Servicing Mandate

| | |
|---|---|
| **Patrón funcional** | `Agree Terms` |
| **Tipo de activo** | `Servicing Mandate` |
| **Artefacto genérico** | `Agreement` |
| **Control Record** | `Servicing Mandate Agreement` |
| **Ubicación Matrix** | Sales and Service › Servicing |

**Propósito.** This service domain maintains the allowed customer servicing arrangements for a service provider covering general access to the bank's products and services and optionally customer specific arrangements

<details><summary><b>Atributos del Control Record</b> · 11</summary>

`Customer Reference` · `Type` · `Jurisdiction` · `Valid From/To Date` · `Responsible Parties` · `Document Directory Entry Instance Reference` · `Product and Service Profile Reference` · `Product and Service Profile` · `Product and Service Type` · `Product and Service Type Eligibility` · `Reference`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Customer Mandate | 5 |

**Interfaz.** Action Terms: `Evaluate` · `Update` · `Control` · `Exchange` · `Request` · `Grant` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 13 | 4 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Evaluate` · `Update` · `Control` · `Exchange` · `Request` · `Grant` · `Retrieve` |
| BQ `Customer Mandate` | `Evaluate` · `Update` · `Control` · `Exchange` · `Grant` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Payment Order Initiation

| | |
|---|---|
| **Patrón funcional** | `Transact` |
| **Tipo de activo** | `Payment Order Initiation` |
| **Artefacto genérico** | `Transaction` |
| **Control Record** | `Payment Order Initiation Transaction` |
| **Ubicación Matrix** | Sales and Service › Servicing |

**Propósito.** This service domain provides a customer payment service. It captures the payer and payee details and other key properties of the payment and initiates the orchestration of the transaction. It provides support for repeating/scheduled payments.

<details><summary><b>Atributos del Control Record</b> · 21</summary>

`Payment Transaction Type` · `Recurring Payment Record` · `Recurring Payment Customer Reference` · `Recurring Payment Reference` · `Customer Reference` · `Payment Transaction` · `Payer Reference` · `Payer Bank Reference` · `Payer Product Instance Reference` · `Payee Reference` · `Payee Bank Reference` · `Payee Product Instance Reference` · `Amount` · `Currency` · `Date Type` · `Date` · `Payment Fees/Charges` · `Payment Mechanism` · `Payment Purpose` · `Document Directory Entry Instance Reference` · `Document Content`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Compliance | 3 |
| Confirmation | 1 |
| Order Initiation | 3 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Retrieve` · `Exchange`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 7 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Retrieve` |
| BQ `Compliance` | `Retrieve` |
| BQ `Confirmation` | `Retrieve` |
| BQ `Order Initiation` | `Exchange` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Loan Syndication

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Syndicated Loan Application` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Syndicated Loan Application Procedure` |
| **Ubicación Matrix** | Sales and Service › Servicing |

**Propósito.** Loan Syndication is a Service Domain that supports orgination, set-up and servicing of syndicated loans. It provides services that are used in lead banks, agents and banks providing administrative support. It handles the orchestration of origination and servicing processes for syndicated loans.

<details><summary><b>Atributos del Control Record</b> · 21</summary>

`Parameter Type` · `Selected Option` · `Request` · `Schedule` · `Status` · `Associated Party Reference` · `Business Unit Reference` · `Service Provider Reference` · `Financial Facility Reference` · `Employee Reference` · `Customer Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Product and Service Type` · `Product and Service Instance` · `Transaction Type` · `Transaction` · `Financial Transaction Arrangement` · `Customer Agreement Reference` · `Reference`

</details>

**Interfaz.** Action Terms: `Retrieve` · `Initiate` · `Update` · `Control`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 4 | 2 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Retrieve` · `Initiate` · `Update` · `Control` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---
