# Business Support

**BIAN Service Landscape V14.0 · vista Matrix** — 68 Service Domains

> Curso independiente de CPS Tech · No afiliado ni acreditado por BIAN e.V. · BIAN® es marca registrada de BIAN e.V., usada con fines descriptivos.

[← Volver al índice de los 341](README.md)

---

## Contenido

**IT Management** · 13

[Systems Operations](#systems-operations) · [Systems Assurance](#systems-assurance) · [Systems Administration](#systems-administration) · [System Development](#system-development) · [System Deployment](#system-deployment) · [Production Release](#production-release) · [Platform Operations](#platform-operations) · [IT Systems Direction](#it-systems-direction) · [IT Standards And Guidelines](#it-standards-and-guidelines) · [Internal Network Operation](#internal-network-operation) · [Development Environment](#development-environment) · [Systems Help Desk](#systems-help-desk) · [Operational Gateway](#operational-gateway)

**Non-IT and Non-HR Enterprise Services** · 9

[Security Assurance](#security-assurance) · [Security Advisory](#security-advisory) · [Procurement](#procurement) · [Legal Compliance](#legal-compliance) · [Internal Audit](#internal-audit) · [Fixed Asset Register](#fixed-asset-register) · [Company Billing and Payments](#company-billing-and-payments) · [Approved Supplier Directory](#approved-supplier-directory) · [Legal Advisory](#legal-advisory)

**Buildings Equipment and Facilities** · 7

[Utilities Administration](#utilities-administration) · [Site Operations](#site-operations) · [Site Administration](#site-administration) · [Property Portfolio](#property-portfolio) · [Equipment Maintenance](#equipment-maintenance) · [Equipment Administration](#equipment-administration) · [Building Maintenance](#building-maintenance)

**Business Command and Control** · 6

[Business Unit Management](#business-unit-management) · [Business Unit Financial Analysis](#business-unit-financial-analysis) · [Business Unit Direction](#business-unit-direction) · [Business Unit Accounting](#business-unit-accounting) · [Business Unit Financial Operations](#business-unit-financial-operations) · [Organization Direction](#organization-direction)

**Finance** · 4

[Financial Statements](#financial-statements) · [Financial Control](#financial-control) · [Financial Compliance](#financial-compliance) · [Enterprise Tax Administration](#enterprise-tax-administration)

**Human Resource Management** · 12

[Workforce Training](#workforce-training) · [Travel and Expenses](#travel-and-expenses) · [Recruitment](#recruitment) · [Human Resources Direction](#human-resources-direction) · [Employee and Contractor Contract](#employee-and-contractor-contract) · [Employee Payroll And Incentives](#employee-payroll-and-incentives) · [Employee Evaluation](#employee-evaluation) · [Employee Data Management](#employee-data-management) · [Employee Certification](#employee-certification) · [Employee Benefits](#employee-benefits) · [Employee Assignment](#employee-assignment) · [Employee Access](#employee-access)

**Knowledge and Intellectual Property Management** · 3

[Management Manual](#management-manual) · [Knowledge Exchange](#knowledge-exchange) · [Intellectual Property Portfolio](#intellectual-property-portfolio)

**Corporate Relations** · 5

[Regulatory And Legal Authority](#regulatory-and-legal-authority) · [Investor Relations](#investor-relations) · [Corporate Relationship](#corporate-relationship) · [Corporate Communications](#corporate-communications) · [Corporate Alliance and Stake Holder](#corporate-alliance-and-stake-holder)

**Business Direction** · 5

[Corporate Strategy](#corporate-strategy) · [Corporate Policies](#corporate-policies) · [Continuity Planning](#continuity-planning) · [Enterprise Architecture](#enterprise-architecture) · [Products and Services Direction](#products-and-services-direction)

**Document Management and Archive** · 4

[Document Directory](#document-directory) · [Correspondence](#correspondence) · [Archive Services](#archive-services) · [Document Services](#document-services)

---

## Systems Operations

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `IT System` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `IT System Operating Session` |
| **Ubicación Matrix** | Business Support › IT Management |

[↑ Índice](README.md)

---

## Systems Assurance

| | |
|---|---|
| **Patrón funcional** | `Assess` |
| **Tipo de activo** | `IT System` |
| **Artefacto genérico** | `Assessment` |
| **Control Record** | `IT System Assessment` |
| **Ubicación Matrix** | Business Support › IT Management |

[↑ Índice](README.md)

---

## Systems Administration

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `IT System` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `IT System Administrative Plan` |
| **Ubicación Matrix** | Business Support › IT Management |

**Propósito.** Administer the configuration, maintenance, assignment and track usage and status of all IT assets deployed in development and production across the enterprise

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Budget Type` · `Budget` · `Assignment` · `Duty` · `Associated Party` · `Budget Balance` · `Subject Matter` · `Type` · `Reference` · `Description`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Capacity Planning and Resilience | 8 |
| Inventory | 8 |
| Configuration | 8 |
| Assurance | 8 |

**Interfaz.** Action Terms: `Capture` · `Grant` · `Exchange` · `Control` · `Initiate` · `Retrieve` · `Update` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 24 | 12 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Capture` · `Grant` · `Exchange` · `Control` · `Initiate` · `Retrieve` · `Update` · `Request` |
| BQ `Assurance` | `Capture` · `Retrieve` · `Request` · `Update` |
| BQ `Capacity Planning and Resilience` | `Capture` · `Retrieve` · `Request` · `Update` |
| BQ `Configuration` | `Capture` · `Retrieve` · `Request` · `Update` |
| BQ `Inventory` | `Capture` · `Retrieve` · `Request` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## System Development

| | |
|---|---|
| **Patrón funcional** | `Develop` |
| **Tipo de activo** | `IT System` |
| **Artefacto genérico** | `Development` |
| **Control Record** | `IT System Development` |
| **Ubicación Matrix** | Business Support › IT Management |

**Propósito.** Develop new, enhance existing applications and integrate package based systems solutions

<details><summary><b>Atributos del Control Record</b> · 9</summary>

`System Development Project Name` · `System Development Project Type` · `System Development Project Description` · `System Development Implementation Plan` · `System Development Budget` · `System Development Project Organization` · `System Development Project Schedule` · `Date Type` · `Date`

</details>

**Behavior Qualifiers** · 5

| Behavior Qualifier | Atributos |
|---|---:|
| Functional Specification | 4 |
| Technical Specification | 4 |
| Software and Data Specification | 4 |
| Testing Specification | 4 |
| Usage Specification | 4 |

**Interfaz.** Action Terms: `Update` · `Create` · `Control` · `Request` · `Exchange` · `Retrieve` · `Capture`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 31 | 12 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Update` · `Create` · `Control` · `Request` · `Exchange` · `Retrieve` |
| BQ `Functional Specification` | `Exchange` · `Update` · `Request` · `Retrieve` · `Capture` |
| BQ `Technical Specification` | `Update` · `Exchange` · `Capture` · `Retrieve` · `Request` |
| BQ `Software and Data Specification` | `Update` · `Exchange` · `Capture` · `Request` · `Retrieve` |
| BQ `Testing Specification` | `Update` · `Exchange` · `Request` · `Retrieve` · `Capture` |
| BQ `Usage Specification` | `Exchange` · `Update` · `Capture` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## System Deployment

| | |
|---|---|
| **Patrón funcional** | `Develop` |
| **Tipo de activo** | `IT System Deployment` |
| **Artefacto genérico** | `Development` |
| **Control Record** | `IT System Deployment Project` |
| **Ubicación Matrix** | Business Support › IT Management |

[↑ Índice](README.md)

---

## Production Release

| | |
|---|---|
| **Patrón funcional** | `Assess` |
| **Tipo de activo** | `Production System` |
| **Artefacto genérico** | `Assessment` |
| **Control Record** | `Production System Assessment` |
| **Ubicación Matrix** | Business Support › IT Management |

**Propósito.** Maintain and apply production release tests for new and updated systems

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Production Release Name` · `Employee or Business Unit Reference` · `Production Release Type` · `Production Release Description` · `Production Release Test Profile` · `Production Release Test Schedule` · `Production Release Consolidation Record` · `Document Directory Entry Instance Reference` · `Date Type` · `Date`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Functional Risk | 4 |
| Production Risk | 4 |
| Business Risk | 4 |
| Operational Risk | 4 |

**Interfaz.** Action Terms: `Evaluate` · `Exchange` · `Update` · `Grant` · `Retrieve` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 14 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Evaluate` · `Exchange` · `Update` · `Grant` · `Retrieve` · `Request` |
| BQ `Functional Risk` | `Exchange` · `Retrieve` |
| BQ `Production Risk` | `Retrieve` · `Exchange` |
| BQ `Business Risk` | `Exchange` · `Retrieve` |
| BQ `Operational Risk` | `Exchange` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Platform Operations

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `IT Systems Platform` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `IT Systems Platform Operating Session` |
| **Ubicación Matrix** | Business Support › IT Management |

[↑ Índice](README.md)

---

## IT Systems Direction

| | |
|---|---|
| **Patrón funcional** | `Direct` |
| **Tipo de activo** | `IT Systems` |
| **Artefacto genérico** | `Strategy` |
| **Control Record** | `IT Systems Strategy` |
| **Ubicación Matrix** | Business Support › IT Management |

[↑ Índice](README.md)

---

## IT Standards And Guidelines

| | |
|---|---|
| **Patrón funcional** | `Design` |
| **Tipo de activo** | `Technology Standards` |
| **Artefacto genérico** | `Specification` |
| **Control Record** | `Technology Standards Specification` |
| **Ubicación Matrix** | Business Support › IT Management |

**Propósito.** Define and apply comprehensive IT architectures, policies and standards as appropriate

<details><summary><b>Atributos del Control Record</b> · 8</summary>

`Parameter Type` · `Selected Option` · `Description` · `Version` · `Status` · `Usage Log` · `Feedback` · `Service Provider Reference`

</details>

**Behavior Qualifiers** · 5

| Behavior Qualifier | Atributos |
|---|---:|
| IT Policies and Guidelines | 4 |
| Product Testing and Deployment Mechanisms | 4 |
| Production Environment and Support Services | 4 |
| Production Platforms and Infrastructure | 4 |
| Development Tooling and Environment | 4 |

**Interfaz.** Action Terms: `Exchange` · `Request` · `Capture` · `Control` · `Retrieve` · `Initiate` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 37 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Exchange` · `Request` · `Capture` · `Control` · `Retrieve` · `Initiate` · `Update` |
| BQ `Development Tooling and Environment` | `Capture` · `Exchange` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `IT Policies and Guidelines` | `Capture` · `Initiate` · `Exchange` · `Retrieve` · `Update` · `Request` |
| BQ `Product Testing and Deployment Mechanisms` | `Capture` · `Initiate` · `Exchange` · `Retrieve` · `Update` · `Request` |
| BQ `Production Platforms and Infrastructure` | `Capture` · `Exchange` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Production Environment and Support Services` | `Capture` · `Exchange` · `Initiate` · `Retrieve` · `Update` · `Request` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Internal Network Operation

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `Internal Network` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `Internal Network Operating Session` |
| **Ubicación Matrix** | Business Support › IT Management |

[↑ Índice](README.md)

---

## Development Environment

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Development Environment` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Development Environment Administrative Plan` |
| **Ubicación Matrix** | Business Support › IT Management |

[↑ Índice](README.md)

---

## Systems Help Desk

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `Help Desk` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `Help Desk Operating Session` |
| **Ubicación Matrix** | Business Support › IT Management |

[↑ Índice](README.md)

---

## Operational Gateway

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `Operational Gateway` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `Operational Gateway Operating Session` |
| **Ubicación Matrix** | Business Support › IT Management |

**Propósito.** This Service Domain operates production information exchanges with external parties for non-financial messages/transactions. It may employ a broad range of channels, media and technologies as needed to support the different requirements of any particular third party interface

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Schedule` · `Status` · `Usage Log` · `Associated Party Reference` · `Service Provider Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Service Configuration` · `Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Inbound Message | 6 |
| Outbound Message | 6 |
| Outbound With Response | 6 |

**Interfaz.** Action Terms: `Execute` · `Initiate` · `Control` · `Exchange` · `Request` · `Notify` · `Update` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 29 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Execute` · `Initiate` · `Control` · `Exchange` · `Request` · `Notify` · `Update` · `Retrieve` |
| BQ `Inbound Message` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Outbound With Response` | `Exchange` · `Initiate` · `Execute` · `Request` · `Notify` · `Retrieve` · `Update` |
| BQ `Outbound Message` | `Exchange` · `Initiate` · `Execute` · `Notify` · `Request` · `Update` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Security Assurance

| | |
|---|---|
| **Patrón funcional** | `Assess` |
| **Tipo de activo** | `Security Compliance` |
| **Artefacto genérico** | `Assessment` |
| **Control Record** | `Security Compliance Assessment` |
| **Ubicación Matrix** | Business Support › Non-IT and Non-HR Enterprise Services |

[↑ Índice](README.md)

---

## Security Advisory

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Security Compliance` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Security Compliance Procedure` |
| **Ubicación Matrix** | Business Support › Non-IT and Non-HR Enterprise Services |

[↑ Índice](README.md)

---

## Procurement

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Procurement` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Procurement Administrative Plan` |
| **Ubicación Matrix** | Business Support › Non-IT and Non-HR Enterprise Services |

[↑ Índice](README.md)

---

## Legal Compliance

| | |
|---|---|
| **Patrón funcional** | `Assess` |
| **Tipo de activo** | `Legal Compliance` |
| **Artefacto genérico** | `Assessment` |
| **Control Record** | `Legal Compliance Assessment` |
| **Ubicación Matrix** | Business Support › Non-IT and Non-HR Enterprise Services |

**Propósito.** Provide specialist legal advice, assess for legal compliance and resolve legal cases as they occur

<details><summary><b>Atributos del Control Record</b> · 14</summary>

`Legal Assessment Type` · `Business Unit Reference` · `Product and Service Reference` · `Customer Reference` · `Jurisdiction Reference` · `Law Reference` · `Law Definition` · `Law Compliance and Reporting Requirements` · `Law Compliance Accountability` · `Legal Penalties` · `Legal Guideline` · `Document Reference` · `Legal Assessment Work Products` · `Legal Assessment Result`

</details>

**Interfaz.** Action Terms: `Exchange` · `Request` · `Evaluate` · `Update` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 5 | 2 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Exchange` · `Request` · `Evaluate` · `Update` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Internal Audit

| | |
|---|---|
| **Patrón funcional** | `Assess` |
| **Tipo de activo** | `Internal Audit` |
| **Artefacto genérico** | `Assessment` |
| **Control Record** | `Internal Audit Assessment` |
| **Ubicación Matrix** | Business Support › Non-IT and Non-HR Enterprise Services |

**Propósito.** Maintain and portfolio of internal audit checks. Select and execute a meaningful sample of checks and identify and resolve non-compliance

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Parameter Type` · `Selected Option` · `Type` · `Reference` · `Request` · `Schedule` · `Status` · `Usage Log` · `Service Provider Reference` · `Requester Reference`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Audit | 7 |

**Interfaz.** Action Terms: `Exchange` · `Grant` · `Execute` · `Initiate` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 14 | 6 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Exchange` · `Grant` · `Execute` · `Initiate` · `Request` · `Retrieve` · `Update` |
| BQ `Audit` | `Exchange` · `Execute` · `Grant` · `Retrieve` · `Initiate` · `Update` · `Request` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Fixed Asset Register

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Fixed Asset Register` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Fixed Asset Register Administrative Plan` |
| **Ubicación Matrix** | Business Support › Non-IT and Non-HR Enterprise Services |

[↑ Índice](README.md)

---

## Company Billing and Payments

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Enterprise Billing And Payments` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Enterprise Billing And Payments Procedure` |
| **Ubicación Matrix** | Business Support › Non-IT and Non-HR Enterprise Services |

[↑ Índice](README.md)

---

## Approved Supplier Directory

| | |
|---|---|
| **Patrón funcional** | `Enroll` |
| **Tipo de activo** | `Supplier` |
| **Artefacto genérico** | `Membership` |
| **Control Record** | `Supplier Membership` |
| **Ubicación Matrix** | Business Support › Non-IT and Non-HR Enterprise Services |

[↑ Índice](README.md)

---

## Legal Advisory

| | |
|---|---|
| **Patrón funcional** | `Advise` |
| **Tipo de activo** | `Legal Advice` |
| **Artefacto genérico** | `Advice` |
| **Control Record** | `Legal Advice` |
| **Ubicación Matrix** | Business Support › Non-IT and Non-HR Enterprise Services |

**Propósito.** The role of the Service Domain is to provide customers and bank employees with advice on legal aspects of product sales and servicing as well as on planned and executed transactions.

<details><summary><b>Atributos del Control Record</b> · 8</summary>

`Subject Area Type` · `Parameter Type` · `Selected Option` · `Request` · `Usage Log` · `Feedback` · `Type` · `Reference`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Charge | 8 |
| Legal | 8 |

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Utilities Administration

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Utilities` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Utilities Administrative Plan` |
| **Ubicación Matrix** | Business Support › Buildings Equipment and Facilities |

[↑ Índice](README.md)

---

## Site Operations

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Building Services` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Building Services Administrative Plan` |
| **Ubicación Matrix** | Business Support › Buildings Equipment and Facilities |

[↑ Índice](README.md)

---

## Site Administration

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Building` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Building Administrative Plan` |
| **Ubicación Matrix** | Business Support › Buildings Equipment and Facilities |

[↑ Índice](README.md)

---

## Property Portfolio

| | |
|---|---|
| **Patrón funcional** | `Analyze` |
| **Tipo de activo** | `Building Portfolio` |
| **Artefacto genérico** | `Analysis` |
| **Control Record** | `Building Portfolio Analysis` |
| **Ubicación Matrix** | Business Support › Buildings Equipment and Facilities |

[↑ Índice](README.md)

---

## Equipment Maintenance

| | |
|---|---|
| **Patrón funcional** | `Maintain` |
| **Tipo de activo** | `Office Equipment` |
| **Artefacto genérico** | `Maintenance Arrangement` |
| **Control Record** | `Office Equipment Maintenance Arrangement` |
| **Ubicación Matrix** | Business Support › Buildings Equipment and Facilities |

[↑ Índice](README.md)

---

## Equipment Administration

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Office Equipment` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Office Equipment Administrative Plan` |
| **Ubicación Matrix** | Business Support › Buildings Equipment and Facilities |

[↑ Índice](README.md)

---

## Building Maintenance

| | |
|---|---|
| **Patrón funcional** | `Maintain` |
| **Tipo de activo** | `Building` |
| **Artefacto genérico** | `Maintenance Arrangement` |
| **Control Record** | `Building Maintenance Arrangement` |
| **Ubicación Matrix** | Business Support › Buildings Equipment and Facilities |

[↑ Índice](README.md)

---

## Business Unit Management

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `Business Unit` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `Business Unit Management Plan` |
| **Ubicación Matrix** | Business Support › Business Command and Control |

**Propósito.** Track and report on business unit activity and financial performance

<details><summary><b>Atributos del Control Record</b> · 7</summary>

`Period` · `Business Unit Usage Policies And Guidelines` · `Business Unit Performance Goals` · `Business Unit Operating Schedule` · `Business Unit Operating Organization` · `Business Unit Resource Plan` · `Business Unit Training Plan`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Performance | 7 |
| Troubleshooting | 2 |

**Interfaz.** Action Terms: `Create` · `Exchange` · `Update` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 12 | 6 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Create` · `Exchange` · `Update` · `Request` · `Retrieve` |
| BQ `Troubleshooting` | `Create` · `Request` · `Retrieve` · `Update` |
| BQ `Performance` | `Retrieve` · `Request` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Business Unit Financial Analysis

| | |
|---|---|
| **Patrón funcional** | `Analyze` |
| **Tipo de activo** | `Business Unit Finance` |
| **Artefacto genérico** | `Analysis` |
| **Control Record** | `Business Unit Finance Analysis` |
| **Ubicación Matrix** | Business Support › Business Command and Control |

[↑ Índice](README.md)

---

## Business Unit Direction

| | |
|---|---|
| **Patrón funcional** | `Direct` |
| **Tipo de activo** | `Business Unit` |
| **Artefacto genérico** | `Strategy` |
| **Control Record** | `Business Unit Strategy` |
| **Ubicación Matrix** | Business Support › Business Command and Control |

[↑ Índice](README.md)

---

## Business Unit Accounting

| | |
|---|---|
| **Patrón funcional** | `Track` |
| **Tipo de activo** | `Business Unit Accounting` |
| **Artefacto genérico** | `Log` |
| **Control Record** | `Business Unit Accounting Log` |
| **Ubicación Matrix** | Business Support › Business Command and Control |

[↑ Índice](README.md)

---

## Business Unit Financial Operations

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Busines Unit Budegt` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Busines Unit Budegt Administrative Plan` |
| **Ubicación Matrix** | Business Support › Business Command and Control |

[↑ Índice](README.md)

---

## Organization Direction

| | |
|---|---|
| **Patrón funcional** | `Direct` |
| **Tipo de activo** | `Organization` |
| **Artefacto genérico** | `Strategy` |
| **Control Record** | `Organization Strategy` |
| **Ubicación Matrix** | Business Support › Business Command and Control |

[↑ Índice](README.md)

---

## Financial Statements

| | |
|---|---|
| **Patrón funcional** | `Analyze` |
| **Tipo de activo** | `Financial Statements` |
| **Artefacto genérico** | `Analysis` |
| **Control Record** | `Financial Statements Analysis` |
| **Ubicación Matrix** | Business Support › Finance |

[↑ Índice](README.md)

---

## Financial Control

| | |
|---|---|
| **Patrón funcional** | `Assess` |
| **Tipo de activo** | `Financial Control` |
| **Artefacto genérico** | `Assessment` |
| **Control Record** | `Financial Control Assessment` |
| **Ubicación Matrix** | Business Support › Finance |

[↑ Índice](README.md)

---

## Financial Compliance

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Financial Compliance` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Financial Compliance Procedure` |
| **Ubicación Matrix** | Business Support › Finance |

[↑ Índice](README.md)

---

## Enterprise Tax Administration

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `Tax Administration` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `Tax Administration Management Plan` |
| **Ubicación Matrix** | Business Support › Finance |

[↑ Índice](README.md)

---

## Workforce Training

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Employee Training` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Employee Training Administrative Plan` |
| **Ubicación Matrix** | Business Support › Human Resource Management |

[↑ Índice](README.md)

---

## Travel and Expenses

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Employee Travel and Expenses` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Employee Travel and Expenses Administrative Plan` |
| **Ubicación Matrix** | Business Support › Human Resource Management |

[↑ Índice](README.md)

---

## Recruitment

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Recruitment` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Recruitment Procedure` |
| **Ubicación Matrix** | Business Support › Human Resource Management |

[↑ Índice](README.md)

---

## Human Resources Direction

| | |
|---|---|
| **Patrón funcional** | `Direct` |
| **Tipo de activo** | `Human Resources` |
| **Artefacto genérico** | `Strategy` |
| **Control Record** | `Human Resources Strategy` |
| **Ubicación Matrix** | Business Support › Human Resource Management |

[↑ Índice](README.md)

---

## Employee and Contractor Contract

| | |
|---|---|
| **Patrón funcional** | `Agree Terms` |
| **Tipo de activo** | `Employee` |
| **Artefacto genérico** | `Agreement` |
| **Control Record** | `Employee Agreement` |
| **Ubicación Matrix** | Business Support › Human Resource Management |

[↑ Índice](README.md)

---

## Employee Payroll And Incentives

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Employee Payroll` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Employee Payroll Procedure` |
| **Ubicación Matrix** | Business Support › Human Resource Management |

[↑ Índice](README.md)

---

## Employee Evaluation

| | |
|---|---|
| **Patrón funcional** | `Analyze` |
| **Tipo de activo** | `Employee` |
| **Artefacto genérico** | `Analysis` |
| **Control Record** | `Employee Analysis` |
| **Ubicación Matrix** | Business Support › Human Resource Management |

[↑ Índice](README.md)

---

## Employee Data Management

| | |
|---|---|
| **Patrón funcional** | `Catalog` |
| **Tipo de activo** | `Employee` |
| **Artefacto genérico** | `Directory Entry` |
| **Control Record** | `Employee Directory Entry` |
| **Ubicación Matrix** | Business Support › Human Resource Management |

[↑ Índice](README.md)

---

## Employee Certification

| | |
|---|---|
| **Patrón funcional** | `Assess` |
| **Tipo de activo** | `Employee Certification` |
| **Artefacto genérico** | `Assessment` |
| **Control Record** | `Employee Certification Assessment` |
| **Ubicación Matrix** | Business Support › Human Resource Management |

[↑ Índice](README.md)

---

## Employee Benefits

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Employee Benefits` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Employee Benefits Administrative Plan` |
| **Ubicación Matrix** | Business Support › Human Resource Management |

[↑ Índice](README.md)

---

## Employee Assignment

| | |
|---|---|
| **Patrón funcional** | `Allocate` |
| **Tipo de activo** | `Employee` |
| **Artefacto genérico** | `Allocation` |
| **Control Record** | `Employee Allocation` |
| **Ubicación Matrix** | Business Support › Human Resource Management |

[↑ Índice](README.md)

---

## Employee Access

| | |
|---|---|
| **Patrón funcional** | `Assess` |
| **Tipo de activo** | `Employee Access` |
| **Artefacto genérico** | `Assessment` |
| **Control Record** | `Employee Access Assessment` |
| **Ubicación Matrix** | Business Support › Human Resource Management |

[↑ Índice](README.md)

---

## Management Manual

| | |
|---|---|
| **Patrón funcional** | `Design` |
| **Tipo de activo** | `Management Manual` |
| **Artefacto genérico** | `Specification` |
| **Control Record** | `Management Manual Specification` |
| **Ubicación Matrix** | Business Support › Knowledge and Intellectual Property Management |

**Propósito.** Develop, maintain and promulgate the management manual of required procedures and guidelines. Provide support in its reference and interpretation as appropriate

<details><summary><b>Atributos del Control Record</b> · 8</summary>

`Parameter Type` · `Selected Option` · `Description` · `Version` · `Status` · `Usage Log` · `Feedback` · `Service Provider Reference`

</details>

**Behavior Qualifiers** · 6

| Behavior Qualifier | Atributos |
|---|---:|
| Company Mission and Policies | 4 |
| Operational Security Procedures and Guidelines | 4 |
| Operational and Production Procedures and Guidelines | 4 |
| Employment Related Procedures and Guidelines | 4 |
| Staff Management Procedures and Guidelines | 4 |
| Legal and Regulatory Obligations and Guidelines | 4 |

**Interfaz.** Action Terms: `Capture` · `Control` · `Initiate` · `Exchange` · `Retrieve` · `Request` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 31 | 16 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Capture` · `Control` · `Initiate` · `Exchange` · `Retrieve` · `Request` · `Update` |
| BQ `Company Mission and Policies` | `Capture` · `Initiate` · `Retrieve` · `Update` |
| BQ `Employment Related Procedures and Guidelines` | `Capture` · `Initiate` · `Retrieve` · `Update` |
| BQ `Legal and Regulatory Obligations and Guidelines` | `Capture` · `Initiate` · `Retrieve` · `Update` |
| BQ `Operational Security Procedures and Guidelines` | `Capture` · `Retrieve` · `Update` · `Initiate` |
| BQ `Operational and Production Procedures and Guidelines` | `Capture` · `Retrieve` · `Initiate` · `Update` |
| BQ `Staff Management Procedures and Guidelines` | `Capture` · `Initiate` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Knowledge Exchange

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `Intellectual Property Exchange` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `Intellectual Property Exchange Operating Session` |
| **Ubicación Matrix** | Business Support › Knowledge and Intellectual Property Management |

**Propósito.** Consolidate, classify and provide structured access to consolidated market intelligence, product and procedural knowledge gained from the workforce in the execution of business to inform business activity and support continual improvement

<details><summary><b>Atributos del Control Record</b> · 9</summary>

`Schedule` · `Status` · `Usage Log` · `Reference` · `Service Provider Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Service Configuration`

</details>

**Behavior Qualifiers** · 5

| Behavior Qualifier | Atributos |
|---|---:|
| Maintenance and Access Administration | 6 |
| Indexing and Publication | 6 |
| Capture and Classification | 6 |
| Review, Refinement and Editing | 6 |
| Archiving | 6 |

**Interfaz.** Action Terms: `Execute` · `Initiate` · `Control` · `Retrieve` · `Exchange` · `Request` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 23 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Execute` · `Initiate` · `Control` · `Retrieve` · `Exchange` · `Request` · `Update` |
| BQ `Indexing and Publication` | `Exchange` · `Retrieve` · `Update` |
| BQ `Capture and Classification` | `Exchange` · `Initiate` · `Execute` · `Retrieve` · `Request` · `Update` |
| BQ `Review, Refinement and Editing` | `Exchange` · `Retrieve` · `Update` |
| BQ `Archiving` | `Retrieve` |
| BQ `Maintenance and Access Administration` | `Retrieve` · `Request` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Intellectual Property Portfolio

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Intellectual Property` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Intellectual Property Administrative Plan` |
| **Ubicación Matrix** | Business Support › Knowledge and Intellectual Property Management |

**Propósito.** Administer the bank's intellectual property assets

<details><summary><b>Atributos del Control Record</b> · 11</summary>

`Intellectual Property Asset Reference` · `Intellectual Property Asset Record` · `Intellectual Property Asset Type` · `Intellectual Property Asset Description` · `Intellectual Property Asset Title` · `Intellectual Property Asset Jurisdiction` · `Intellectual Property Asset Creator` · `Intellectual Property Asset Valuation` · `Document Directory Entry Instance Reference` · `Date Type` · `Date`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Maintenance | 9 |
| Assignment | 6 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Retrieve` · `Exchange` · `Request` · `Grant`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 14 | 6 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Retrieve` |
| BQ `Maintenance` | `Initiate` · `Exchange` · `Update` · `Retrieve` · `Request` |
| BQ `Assignment` | `Request` · `Update` · `Grant` · `Initiate` · `Exchange` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Regulatory And Legal Authority

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `Regulatory And Legal Authority Relationship` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `Regulatory And Legal Authority Relationship Management Plan` |
| **Ubicación Matrix** | Business Support › Corporate Relations |

**Propósito.** Maintain effective relations with regulators, accounting and government agencies. Oversee interactions and reporting as necessary

<details><summary><b>Atributos del Control Record</b> · 7</summary>

`Type` · `Reference` · `Budget Type` · `Budget` · `Assignment` · `Plan` · `Description`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Troubleshooting | 8 |
| Maintain Relations | 8 |
| Represent Bank Interests | 8 |
| Establish Relations | 8 |

**Interfaz.** Action Terms: `Capture` · `Retrieve` · `Exchange` · `Control` · `Grant` · `Request` · `Initiate` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 25 | 12 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Capture` · `Exchange` · `Control` · `Grant` · `Retrieve` · `Request` · `Initiate` · `Update` |
| BQ `Represent Bank Interests` | `Retrieve` · `Initiate` · `Request` · `Update` |
| BQ `Troubleshooting` | `Capture` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Maintain Relations` | `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Establish Relations` | `Initiate` · `Retrieve` · `Request` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Investor Relations

| | |
|---|---|
| **Patrón funcional** | `Enroll` |
| **Tipo de activo** | `Investor` |
| **Artefacto genérico** | `Membership` |
| **Control Record** | `Investor Membership` |
| **Ubicación Matrix** | Business Support › Corporate Relations |

[↑ Índice](README.md)

---

## Corporate Relationship

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `Corporate Partner Relationship` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `Corporate Partner Relationship Management Plan` |
| **Ubicación Matrix** | Business Support › Corporate Relations |

[↑ Índice](README.md)

---

## Corporate Communications

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `Enterprise Communication` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `Enterprise Communication Management Plan` |
| **Ubicación Matrix** | Business Support › Corporate Relations |

[↑ Índice](README.md)

---

## Corporate Alliance and Stake Holder

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `Alliance Partner Relationship` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `Alliance Partner Relationship Management Plan` |
| **Ubicación Matrix** | Business Support › Corporate Relations |

[↑ Índice](README.md)

---

## Corporate Strategy

| | |
|---|---|
| **Patrón funcional** | `Direct` |
| **Tipo de activo** | `Enterprise` |
| **Artefacto genérico** | `Strategy` |
| **Control Record** | `Enterprise Strategy` |
| **Ubicación Matrix** | Business Support › Business Direction |

[↑ Índice](README.md)

---

## Corporate Policies

| | |
|---|---|
| **Patrón funcional** | `Design` |
| **Tipo de activo** | `Corporate Policy` |
| **Artefacto genérico** | `Specification` |
| **Control Record** | `Corporate Policy Specification` |
| **Ubicación Matrix** | Business Support › Business Direction |

[↑ Índice](README.md)

---

## Continuity Planning

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `Enterprise Continuity Assurance` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `Enterprise Continuity Assurance Management Plan` |
| **Ubicación Matrix** | Business Support › Business Direction |

[↑ Índice](README.md)

---

## Enterprise Architecture

| | |
|---|---|
| **Patrón funcional** | `Design` |
| **Tipo de activo** | `Enterprise Architecture` |
| **Artefacto genérico** | `Specification` |
| **Control Record** | `Enterprise Architecture Specification` |
| **Ubicación Matrix** | Business Support › Business Direction |

**Propósito.** Define and maintain comprehensive business architectural definitions/blueprints to help organize/direct the business

<details><summary><b>Atributos del Control Record</b> · 8</summary>

`Parameter Type` · `Selected Option` · `Description` · `Version` · `Status` · `Usage Log` · `Feedback` · `ServiceProvider Reference`

</details>

**Behavior Qualifiers** · 5

| Behavior Qualifier | Atributos |
|---|---:|
| Business Architecture | 4 |
| Application Architecture | 4 |
| Technology Infrastructure | 4 |
| Organization | 4 |
| Information Architecture | 4 |

**Interfaz.** Action Terms: `Capture` · `Control` · `Exchange` · `Retrieve` · `Initiate` · `Request` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 27 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Capture` · `Control` · `Exchange` · `Retrieve` · `Initiate` · `Request` · `Update` |
| BQ `Technology Infrastructure` | `Capture` · `Retrieve` · `Request` · `Update` |
| BQ `Business Architecture` | `Capture` · `Retrieve` · `Request` · `Update` |
| BQ `Application Architecture` | `Capture` · `Retrieve` · `Request` · `Update` |
| BQ `Organization` | `Capture` · `Retrieve` · `Request` · `Update` |
| BQ `Information Architecture` | `Capture` · `Retrieve` · `Request` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Products and Services Direction

| | |
|---|---|
| **Patrón funcional** | `Direct` |
| **Tipo de activo** | `Products And Services` |
| **Artefacto genérico** | `Strategy` |
| **Control Record** | `Products And Services Strategy` |
| **Ubicación Matrix** | Business Support › Business Direction |

[↑ Índice](README.md)

---

## Document Directory

| | |
|---|---|
| **Patrón funcional** | `Catalog` |
| **Tipo de activo** | `Document` |
| **Artefacto genérico** | `Directory Entry` |
| **Control Record** | `Document Directory Entry` |
| **Ubicación Matrix** | Business Support › Document Management and Archive |

**Propósito.** This Service Domain provides a directory based categorization and storage mechanism for documents created and referenced by the bank

<details><summary><b>Atributos del Control Record</b> · 33</summary>

`Document Name` · `Location Reference` · `Business Unit or Employee Reference` · `Product and Service Reference` · `Product and Service Action Reference` · `Document Creation Date` · `Document Capture Date and Time` · `Document Type/Description` · `Document Content` · `Document Provisioning History` · `Document Provisioning Request` · `Document Provisioning Schedule` · `Document Provisioning Result` · `Document Version History` · `Document Version` · `Document Version Date` · `Document Verification History` · `Document Verification Task Description` · `Document Verification Service Provider Reference` · `Document Verification Task Result` · `Document Amendment History` · `Document Amendment Description` · `Document Amendment Result` · `Document Update History` · `Document Update Description` · `Document Update Result` · `Document Archiving History` · `Document Archiving Action` · `Document Archive Reference` · `Document Media/Format` · `Document Subject Reference` · `Document Location` · `Document Status`

</details>

**Behavior Qualifiers** · 6

| Behavior Qualifier | Atributos |
|---|---:|
| Document Update History Properties | 7 |
| Document Archiving Properties | 7 |
| Document Version Properties | 7 |
| Document Reference Properties | 7 |
| Document Amendment Properties | 7 |
| Document Verification Properties | 7 |

**Interfaz.** Action Terms: `Exchange` · `Request` · `Control` · `Execute` · `Notify` · `Register` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 44 | 23 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Exchange` · `Request` · `Control` · `Execute` · `Notify` · `Register` · `Retrieve` · `Update` |
| BQ `Document Amendment Properties` | `Execute` · `Notify` · `Register` · `Request` · `Retrieve` · `Update` |
| BQ `Document Archiving Properties` | `Execute` · `Notify` · `Register` · `Request` · `Retrieve` · `Update` |
| BQ `Document Reference Properties` | `Execute` · `Notify` · `Register` · `Request` · `Retrieve` · `Update` |
| BQ `Document Update History Properties` | `Execute` · `Notify` · `Register` · `Request` · `Retrieve` · `Update` |
| BQ `Document Verification Properties` | `Execute` · `Notify` · `Register` · `Request` · `Retrieve` · `Update` |
| BQ `Document Version Properties` | `Execute` · `Notify` · `Register` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Correspondence

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `Correspondence` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `Correspondence Operating Session` |
| **Ubicación Matrix** | Business Support › Document Management and Archive |

**Propósito.** This service domain orchestrates the production of pre-formatted correspondence and batches of correspondence

<details><summary><b>Atributos del Control Record</b> · 4</summary>

`Correspondence Service Session Statistics` · `Correspondence Service Session Report Type` · `Correspondence Service Session Report` · `Correspondence Service Session Date`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Outbound | 17 |
| Outbound With Response | 3 |
| Inbound | 9 |
| Block Mailing | 1 |

**Interfaz.** Action Terms: `Request` · `Initiate` · `Update` · `Control` · `Execute` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 18 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Request` · `Initiate` · `Update` · `Control` · `Execute` · `Retrieve` |
| BQ `Outbound` | `Retrieve` · `Initiate` · `Update` |
| BQ `Outbound With Response` | `Update` · `Retrieve` · `Initiate` |
| BQ `Inbound` | `Update` · `Initiate` · `Retrieve` |
| BQ `Block Mailing` | `Initiate` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Archive Services

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `Archive` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `Archive Operating Session` |
| **Ubicación Matrix** | Business Support › Document Management and Archive |

**Propósito.** The Archive Services Service Domain enables the bank to retain, maintain and access significant documents that are no longer actively accessed but that might be required in the future

<details><summary><b>Atributos del Control Record</b> · 11</summary>

`Schedule` · `Status` · `Usage Log` · `Associated Party Reference` · `Service Provider Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Service Configuration` · `Reference` · `Document Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Document Retrieval | 6 |
| Document Capture | 6 |
| Document Maintenance | 6 |

**Interfaz.** Action Terms: `Exchange` · `Request` · `Update` · `Execute` · `Retrieve` · `Notify` · `Control` · `Initiate`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 29 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Exchange` · `Request` · `Update` · `Execute` · `Retrieve` · `Notify` · `Control` · `Initiate` |
| BQ `Document Maintenance` | `Notify` · `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Document Capture` | `Execute` · `Notify` · `Exchange` · `Initiate` · `Request` · `Retrieve` · `Update` |
| BQ `Document Retrieval` | `Exchange` · `Initiate` · `Execute` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Document Services

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Document Service` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Document Service Procedure` |
| **Ubicación Matrix** | Business Support › Document Management and Archive |

**Propósito.** The Document Services Service Domain manages the creation and maintenance of documents throughout the bank

<details><summary><b>Atributos del Control Record</b> · 24</summary>

`Parameter Type` · `Selected Option` · `Request` · `Schedule` · `Status` · `Associated Party Reference` · `Business Unit Reference` · `Service Provider Reference` · `Financial Facility Reference` · `Employee Reference` · `Customer Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Product and Service Type` · `Product and Service Instance` · `Transaction Type` · `Transaction` · `Financial Transaction Arrangement` · `Customer Agreement Reference` · `Reference` · `Document Reference` · `Document Service Reference` · `Document Involved Party Reference`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Document Template | 0 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 6 | 5 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---
