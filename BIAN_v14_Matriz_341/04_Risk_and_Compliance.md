# Risk and Compliance

**BIAN Service Landscape V14.0 · vista Matrix** — 36 Service Domains

> Curso independiente de CPS Tech · No afiliado ni acreditado por BIAN e.V. · BIAN® es marca registrada de BIAN e.V., usada con fines descriptivos.

[← Volver al índice de los 341](README.md)

---

## Contenido

**Bank Portfolio and Treasury** · 7

[Stock Lending and Repos](#stock-lending-and-repos) · [Corporate Treasury Analysis](#corporate-treasury-analysis) · [Corporate Treasury](#corporate-treasury) · [Bank Portfolio Analysis](#bank-portfolio-analysis) · [Bank Portfolio Administration](#bank-portfolio-administration) · [Asset Securitization](#asset-securitization) · [Asset And Liability Management](#asset-and-liability-management)

**Business Analysis** · 9

[Market Analysis](#market-analysis) · [Contribution Analysis](#contribution-analysis) · [Competitor Analysis](#competitor-analysis) · [Channel Portfolio](#channel-portfolio) · [Branch Portfolio](#branch-portfolio) · [Segment Direction](#segment-direction) · [Customer Portfolio](#customer-portfolio) · [Product Portfolio](#product-portfolio) · [Market Research](#market-research)

**Regulations and Compliance** · 7

[Regulatory Reporting](#regulatory-reporting) · [Regulatory Compliance](#regulatory-compliance) · [Guideline Compliance](#guideline-compliance) · [Fraud Resolution](#fraud-resolution) · [Financial Accounting](#financial-accounting) · [Compliance Reporting](#compliance-reporting) · [Financial Statement Assessment](#financial-statement-assessment)

**Models** · 13

[Contribution Models](#contribution-models) · [Operational Risk Models](#operational-risk-models) · [Production Risk Models](#production-risk-models) · [Credit and Margin Management](#credit-and-margin-management) · [Business Risk Models](#business-risk-models) · [Customer Behavior Models](#customer-behavior-models) · [Economic Capital](#economic-capital) · [Credit Risk Models](#credit-risk-models) · [Financial Instrument Valuation Models](#financial-instrument-valuation-models) · [Market Risk Models](#market-risk-models) · [Liquidity Risk Models](#liquidity-risk-models) · [Gap Analysis](#gap-analysis) · [Fraud Model](#fraud-model)

---

## Stock Lending and Repos

| | |
|---|---|
| **Patrón funcional** | `Transact` |
| **Tipo de activo** | `Repo` |
| **Artefacto genérico** | `Transaction` |
| **Control Record** | `Repo Transaction` |
| **Ubicación Matrix** | Risk and Compliance › Bank Portfolio and Treasury |

**Propósito.** This Service Domain supports the bank offering tri-party repo transactions made between its customers to support their short term capital management requirements

<details><summary><b>Atributos del Control Record</b> · 9</summary>

`Parameter Type` · `Selected Option` · `Status` · `Type` · `Reference` · `Repurchase Agreement Reference` · `Repurchase Agreement Involved Party Reference` · `Repurchase Agreement Involvement Type` · `Repurchase Arrangement Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Repo Transaction Security Transfer | 7 |
| Repo Transaction Initiation | 7 |
| Repo Transaction Cash Transfer | 7 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 29 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Repo Transaction Cash Transfer` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Repo Transaction Initiation` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Repo Transaction Security Transfer` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Corporate Treasury Analysis

| | |
|---|---|
| **Patrón funcional** | `Analyze` |
| **Tipo de activo** | `Corporate Treasury` |
| **Artefacto genérico** | `Analysis` |
| **Control Record** | `Corporate Treasury Analysis` |
| **Ubicación Matrix** | Risk and Compliance › Bank Portfolio and Treasury |

[↑ Índice](README.md)

---

## Corporate Treasury

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `Corporate Treasury` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `Corporate Treasury Management Plan` |
| **Ubicación Matrix** | Risk and Compliance › Bank Portfolio and Treasury |

**Propósito.** This service domain orchestrates the consolidation and presentation of summary transaction details to assemble a view of the overall treasury position of the Bank

<details><summary><b>Atributos del Control Record</b> · 8</summary>

`Treasury Planning Policies And Guidelines` · `Treasury Plan Operating Parameters` · `Treasury Plan Goals` · `Enterprise Financial Statements` · `Enterprise Balance Sheet Detailed Content` · `Enterprise Bank Accounting And Cash Management Records` · `Capital/Wholesale Market Transactions` · `Currency and Rate Risk Analysis`

</details>

**Behavior Qualifiers** · 5

| Behavior Qualifier | Atributos |
|---|---:|
| Liquidity | 4 |
| Tactical Funding | 4 |
| Strategic Funding | 5 |
| Securitization | 4 |
| Bank Rates | 7 |

**Interfaz.** Action Terms: `Update` · `Capture` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 11 | 12 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Update` · `Capture` · `Retrieve` |
| BQ `Securitization` | `Update` · `Retrieve` |
| BQ `Liquidity` | `Retrieve` · `Capture` |
| BQ `Strategic Funding` | `Capture` · `Retrieve` |
| BQ `Tactical Funding` | `Retrieve` |
| BQ `Bank Rates` | `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Bank Portfolio Analysis

| | |
|---|---|
| **Patrón funcional** | `Analyze` |
| **Tipo de activo** | `Asset And Liability Portfolio` |
| **Artefacto genérico** | `Analysis` |
| **Control Record** | `Asset And Liability Portfolio Analysis` |
| **Ubicación Matrix** | Risk and Compliance › Bank Portfolio and Treasury |

[↑ Índice](README.md)

---

## Bank Portfolio Administration

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Asset And Liability Portfolio` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Asset And Liability Portfolio Administrative Plan` |
| **Ubicación Matrix** | Risk and Compliance › Bank Portfolio and Treasury |

[↑ Índice](README.md)

---

## Asset Securitization

| | |
|---|---|
| **Patrón funcional** | `Transact` |
| **Tipo de activo** | `Asset Securitization` |
| **Artefacto genérico** | `Transaction` |
| **Control Record** | `Asset Securitization Transaction` |
| **Ubicación Matrix** | Risk and Compliance › Bank Portfolio and Treasury |

**Propósito.** Determine and select assets for securitization as needed to maintain and optimize the Bank portfolio. Administer the securitization process

<details><summary><b>Atributos del Control Record</b> · 6</summary>

`Parameter Type` · `Selected Option` · `Status` · `Type` · `Transaction Type` · `Transaction`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Placement | 7 |
| Selection | 7 |
| Securitization | 7 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Execute` · `Initiate` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 22 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Request` · `Retrieve` · `Update` · `Initiate` |
| BQ `Placement` | `Exchange` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Selection` | `Exchange` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Securitization` | `Initiate` · `Exchange` · `Retrieve` · `Request` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Asset And Liability Management

| | |
|---|---|
| **Patrón funcional** | `Direct` |
| **Tipo de activo** | `Asset And Liability Portfolio` |
| **Artefacto genérico** | `Strategy` |
| **Control Record** | `Asset And Liability Portfolio Strategy` |
| **Ubicación Matrix** | Risk and Compliance › Bank Portfolio and Treasury |

**Propósito.** The unit overseeing the banks asset and liability policies and position

<details><summary><b>Atributos del Control Record</b> · 9</summary>

`Asset And Liability Balance Sheet` · `Asset And Liability Maturity Ladder` · `Asset And Liability Capital Allocation` · `Asset And Liability Policy Goal Record` · `Asset And Liability Policy Type` · `Asset And Liability Policy Type Definition` · `Asset And Liability Policy Type Goals` · `Asset And Liability Policy Type Position` · `Asset And Liability Policy Type Sensitivity Assessment`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Transaction Alignment | 11 |

**Interfaz.** Action Terms: `Create` · `Update` · `Request` · `Grant` · `Retrieve` · `Exchange`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 8 | 4 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| BQ `Transaction Alignment` | `Create` · `Exchange` · `Retrieve` · `Request` |
| **Control Record** | `Update` · `Request` · `Grant` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Market Analysis

| | |
|---|---|
| **Patrón funcional** | `Analyze` |
| **Tipo de activo** | `General Market Research` |
| **Artefacto genérico** | `Analysis` |
| **Control Record** | `General Market Research Analysis` |
| **Ubicación Matrix** | Risk and Compliance › Business Analysis |

**Propósito.** This service domain analyzes internal and external market information sources as necessary to develop specific market insights. It may maintain a collection of predefined market analyses and may also offer specific ad-hoc analysis on request

<details><summary><b>Atributos del Control Record</b> · 13</summary>

`Type` · `Specification` · `Guidance` · `Algorithm Reference` · `Request Record` · `Request` · `Employee/Business Unit Reference` · `Request Work Products` · `Request Result` · `Usage Record` · `Usage` · `Impact` · `Reference`

</details>

**Behavior Qualifiers** · 6

| Behavior Qualifier | Atributos |
|---|---:|
| Market Forecasting | 10 |
| Pricing Behavior Analsysis | 10 |
| Competitive Analysis | 10 |
| Market Segmentation Analysis | 10 |
| Channel Distribution Analysis | 10 |
| Customer Need Analysis | 10 |

**Interfaz.** Action Terms: `Evaluate` · `Execute` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 5 | 16 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Evaluate` · `Execute` · `Request` · `Retrieve` |
| BQ `Competitive Analysis` | `Evaluate` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Contribution Analysis

| | |
|---|---|
| **Patrón funcional** | `Analyze` |
| **Tipo de activo** | `Contribution` |
| **Artefacto genérico** | `Analysis` |
| **Control Record** | `Contribution Analysis` |
| **Ubicación Matrix** | Risk and Compliance › Business Analysis |

[↑ Índice](README.md)

---

## Competitor Analysis

| | |
|---|---|
| **Patrón funcional** | `Analyze` |
| **Tipo de activo** | `Competitor` |
| **Artefacto genérico** | `Analysis` |
| **Control Record** | `Competitor Analysis` |
| **Ubicación Matrix** | Risk and Compliance › Business Analysis |

**Propósito.** Solicit, consolidate and analyze competitor specific public domain data to develop competitor insights and comparisons

<details><summary><b>Atributos del Control Record</b> · 13</summary>

`Type` · `Specification` · `Guidance` · `Algorithm Reference` · `Request Record` · `Request` · `Employee/Business Unit Reference` · `Request Work Products` · `Request Result` · `Usage Record` · `Usage` · `Impact` · `Reference`

</details>

**Behavior Qualifiers** · 5

| Behavior Qualifier | Atributos |
|---|---:|
| Peer Competitor Analysis | 10 |
| Competitor SWOT Analysis | 10 |
| Competitive Benchmarking | 10 |
| Competitor Clustering or Grouping | 10 |
| Product Competitive Analysis | 10 |

**Interfaz.** Action Terms: `Evaluate` · `Retrieve` · `Execute` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 6 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| BQ `Product Competitive Analysis` | `Evaluate` · `Retrieve` |
| **Control Record** | `Evaluate` · `Execute` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Channel Portfolio

| | |
|---|---|
| **Patrón funcional** | `Analyze` |
| **Tipo de activo** | `Channel Portfolio` |
| **Artefacto genérico** | `Analysis` |
| **Control Record** | `Channel Portfolio Analysis` |
| **Ubicación Matrix** | Risk and Compliance › Business Analysis |

[↑ Índice](README.md)

---

## Branch Portfolio

| | |
|---|---|
| **Patrón funcional** | `Analyze` |
| **Tipo de activo** | `Branch Network` |
| **Artefacto genérico** | `Analysis` |
| **Control Record** | `Branch Network Analysis` |
| **Ubicación Matrix** | Risk and Compliance › Business Analysis |

[↑ Índice](README.md)

---

## Segment Direction

| | |
|---|---|
| **Patrón funcional** | `Direct` |
| **Tipo de activo** | `Segment` |
| **Artefacto genérico** | `Strategy` |
| **Control Record** | `Segment Strategy` |
| **Ubicación Matrix** | Risk and Compliance › Business Analysis |

**Propósito.** Define market segments and develop and assess performance against the segment plan's performance goals

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Period` · `Policies And Guidelines` · `Organization` · `Budget` · `Schedule` · `Segment Goal Record` · `Segment Goal Type` · `Segment Goal Definition` · `Segment Goal Organization` · `Segment Goal Result`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Initiative | 10 |

**Interfaz.** Action Terms: `Update` · `Request` · `Create` · `Exchange` · `Capture` · `Retrieve` · `Grant`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 13 | 4 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Update` · `Request` · `Create` · `Exchange` · `Capture` · `Retrieve` · `Grant` |
| BQ `Initiative` | `Create` · `Update` · `Request` · `Exchange` · `Capture` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Customer Portfolio

| | |
|---|---|
| **Patrón funcional** | `Analyze` |
| **Tipo de activo** | `Customer Portfolio` |
| **Artefacto genérico** | `Analysis` |
| **Control Record** | `Customer Portfolio Analysis` |
| **Ubicación Matrix** | Risk and Compliance › Business Analysis |

**Propósito.** Maintain a portfolio of analytical views of the customer base to support customer segment profitability and performance analysis

<details><summary><b>Atributos del Control Record</b> · 14</summary>

`Customer Portfolio Type` · `Customer Portfolio Type Definition` · `Customer Portfolio Performance Goals` · `Schedule` · `Report` · `Type` · `Result` · `Reporting Date` · `Document Directory Entry Instance Reference` · `Customer Reference` · `Reference` · `Customer Portfolio Reference` · `Customer Portfolio Criteria Reference` · `Customer Product Reference`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Profitability Analysis | 10 |
| Performance Analysis | 10 |

**Interfaz.** Action Terms: `Evaluate` · `Update` · `Request` · `Retrieve` · `Exchange` · `Execute`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 10 | 6 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Evaluate` · `Update` · `Request` · `Retrieve` |
| BQ `Performance Analysis` | `Evaluate` · `Update` · `Exchange` · `Execute` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Product Portfolio

| | |
|---|---|
| **Patrón funcional** | `Analyze` |
| **Tipo de activo** | `Product Portfolio` |
| **Artefacto genérico** | `Analysis` |
| **Control Record** | `Product Portfolio Analysis` |
| **Ubicación Matrix** | Risk and Compliance › Business Analysis |

**Propósito.** Maintain a portfolio of analytical views of the product portfolio to support product profitability and performance analysis

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Product Portfolio Make-up` · `Product Type` · `Product Type Definition` · `Product Portfolio Performance Goals` · `Schedule` · `Report` · `Product Analysis Type` · `Product Analysis Result` · `Product Analysis Reporting Date` · `Document Directory Entry Instance Reference`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Performance Analysis | 8 |

**Interfaz.** Action Terms: `Evaluate` · `Update` · `Request` · `Retrieve` · `Exchange` · `Execute`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 10 | 4 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Evaluate` · `Update` · `Request` · `Retrieve` |
| BQ `Performance Analysis` | `Evaluate` · `Update` · `Exchange` · `Execute` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Market Research

| | |
|---|---|
| **Patrón funcional** | `Catalog` |
| **Tipo de activo** | `General Market Research` |
| **Artefacto genérico** | `Directory Entry` |
| **Control Record** | `General Market Research Directory Entry` |
| **Ubicación Matrix** | Risk and Compliance › Business Analysis |

**Propósito.** This service domain handles the capture of market research from multiple external sources. This can include live feeds, analysis and reports in any form. The information is classified/catalogued and stored for retrieval.

<details><summary><b>Atributos del Control Record</b> · 9</summary>

`General Market Research Viewpoint Type` · `General Market Research Viewpoint Description` · `Referenced Market Research Record` · `Market Research Report Type` · `Market Research Report Type Definition` · `Market Research Report Version/Period` · `Market Research Report Reference` · `Market Research Report Request` · `Employee or Business Unit Reference`

</details>

**Behavior Qualifiers** · 15

| Behavior Qualifier | Atributos |
|---|---:|
| Consumer Behavior | 4 |
| Branding and Positioning | 6 |
| Customer Journey and Experience | 6 |
| Technology and Innovation | 6 |
| Regulatory and Environmental Factors | 6 |
| Target Market and Segmentation | 6 |
| Market Entry and Expansion | 6 |
| Market Size and Trends | 6 |
| Customer Demographics and Psychographics | 6 |
| Competitive Analysis | 6 |
| Distribution Channels | 6 |
| Product or Service Analysis | 4 |
| Pricing Analysis | 4 |
| Forecasting and Future Outlook | 6 |
| Marketing and Advertising | 6 |

**Interfaz.** Action Terms: `Register` · `Update` · `Execute` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 5 | 32 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Register` · `Update` · `Execute` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Regulatory Reporting

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Regulatory Compliance` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Regulatory Compliance Administrative Plan` |
| **Ubicación Matrix** | Risk and Compliance › Regulations and Compliance |

**Propósito.** This service domain administers and orchestrates the tasks required to meet the bank's regulatory reporting obligations

<details><summary><b>Atributos del Control Record</b> · 4</summary>

`Regulatory Authority Reference` · `Regulatory Reporting Schedule` · `Regulation Reference` · `Regulatory Report Type`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Consolidation | 5 |
| Authoring | 7 |
| Enquiries | 8 |

**Interfaz.** Action Terms: `Update` · `Request` · `Retrieve` · `Create` · `Capture` · `Exchange`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 13 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Update` · `Request` · `Retrieve` · `Create` |
| BQ `Consolidation` | `Retrieve` · `Update` |
| BQ `Authoring` | `Capture` · `Exchange` · `Retrieve` |
| BQ `Enquiries` | `Update` · `Exchange` · `Retrieve` · `Capture` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Regulatory Compliance

| | |
|---|---|
| **Patrón funcional** | `Assess` |
| **Tipo de activo** | `Regulatory Compliance` |
| **Artefacto genérico** | `Assessment` |
| **Control Record** | `Regulatory Compliance Assessment` |
| **Ubicación Matrix** | Risk and Compliance › Regulations and Compliance |

**Propósito.** This service domain provides a service to interpret regulatory requirements, provide guidance and define and implement a portfolio of regulatory compliance tests across all appropriate bank activities

<details><summary><b>Atributos del Control Record</b> · 22</summary>

`Regulatory Assessment Type` · `Business Unit Reference` · `Product and Service Reference` · `Customer Reference` · `Regulatory Authority Reference` · `Regulation Reference` · `Regulation Definition` · `Regulation Compliance and Reporting Requirements` · `Regulation Accountability` · `Regulation Penalties` · `Regulation Guideline` · `Document Reference` · `Regulatory Assessment Work Products` · `Regulatory Assessment Result` · `Reference` · `Assessment Requestor` · `Assessment Start Date` · `Assessment Completion Date` · `Regulation Customer Type` · `Regulation Customer Residence Status` · `Regulation Valid from Date` · `Regulation Valid to Date`

</details>

**Interfaz.** Action Terms: `Retrieve` · `Evaluate` · `Request` · `Update` · `Capture`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 5 | 2 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Retrieve` · `Evaluate` · `Request` · `Update` · `Capture` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Guideline Compliance

| | |
|---|---|
| **Patrón funcional** | `Assess` |
| **Tipo de activo** | `Guideline Compliance` |
| **Artefacto genérico** | `Assessment` |
| **Control Record** | `Guideline Compliance Assessment` |
| **Ubicación Matrix** | Risk and Compliance › Regulations and Compliance |

**Propósito.** This service domain develops and applies a portfolio of guideline compliance tests to confirm adherence to bank and regulator imposed internal procedures

<details><summary><b>Atributos del Control Record</b> · 7</summary>

`Type` · `Business Unit Reference` · `Product and Service Reference` · `Customer Reference` · `Document Reference` · `Work Products` · `Result`

</details>

**Interfaz.** Action Terms: `Evaluate` · `Retrieve` · `Update` · `Exchange` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 5 | 2 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Evaluate` · `Retrieve` · `Update` · `Exchange` · `Request` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Fraud Resolution

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Fraud Resolution` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Fraud Resolution Procedure` |
| **Ubicación Matrix** | Risk and Compliance › Regulations and Compliance |

**Propósito.** This service domain sets up and processes a fraud case resulting from fraud behavior detected during production processing

<details><summary><b>Atributos del Control Record</b> · 14</summary>

`Fraud Case Type` · `Product Instance Reference` · `Customer Reference` · `Merchant Reference` · `Intersted Party Reference` · `Contact Reference` · `Transaction Reference` · `Transaction Record` · `Case Location` · `Date` · `Employee/Business Unit Reference` · `Fraud Case Work Products` · `Fraud Case Resolution Schedule` · `Fraud Case Status`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Case Analysis | 1 |
| Case Determination | 7 |
| Case Resolution | 7 |

**Interfaz.** Action Terms: `Initiate` · `Exchange` · `Update` · `Retrieve` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 9 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Exchange` · `Update` · `Retrieve` |
| BQ `Case Analysis` | `Retrieve` |
| BQ `Case Determination` | `Exchange` · `Retrieve` |
| BQ `Case Resolution` | `Retrieve` · `Request` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Financial Accounting

| | |
|---|---|
| **Patrón funcional** | `Track` |
| **Tipo de activo** | `Financial Booking` |
| **Artefacto genérico** | `Log` |
| **Control Record** | `Financial Booking Log` |
| **Ubicación Matrix** | Risk and Compliance › Regulations and Compliance |

**Propósito.** The Financial Accounting Service Domain takes in financial facts and based on these, creates accounting instructions that will update the general ledger and sub ledger accounts

<details><summary><b>Atributos del Control Record</b> · 6</summary>

`Financial Account Type` · `Product and Service Reference` · `Business Unit Reference` · `Chart of Account/Booking Rules` · `Base Currency` · `Status`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Ledger Posting | 4 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Retrieve` · `Capture`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 7 | 4 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Retrieve` |
| BQ `Ledger Posting` | `Capture` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Compliance Reporting

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Compliance Reporting` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Compliance Reporting Administrative Plan` |
| **Ubicación Matrix** | Risk and Compliance › Regulations and Compliance |

**Propósito.** This service domain administers and orchestrates the tasks required to apply and report on internal audit control and reporting activity

<details><summary><b>Atributos del Control Record</b> · 5</summary>

`Budget Type` · `Budget` · `Assignment` · `Compliance Reporting Administrative Plan` · `Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Consolidation | 8 |
| Remediation | 8 |
| Compliance Assessment | 8 |

**Interfaz.** Action Terms: `Request` · `Initiate` · `Capture` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 18 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Request` · `Initiate` · `Retrieve` · `Update` · `Capture` |
| BQ `Consolidation` | `Capture` · `Retrieve` · `Request` · `Update` |
| BQ `Compliance Assessment` | `Capture` · `Retrieve` · `Request` · `Update` |
| BQ `Remediation` | `Capture` · `Initiate` · `Retrieve` · `Request` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Financial Statement Assessment

| | |
|---|---|
| **Patrón funcional** | `Assess` |
| **Tipo de activo** | `Financial Statement` |
| **Artefacto genérico** | `Assessment` |
| **Control Record** | `Financial Statement Assessment` |
| **Ubicación Matrix** | Risk and Compliance › Regulations and Compliance |

**Propósito.** This Service Domain supports a range of financial analyses that can be used to extract specific insights from an entity

<details><summary><b>Atributos del Control Record</b> · 11</summary>

`Parameter Type` · `Selected Option` · `Type` · `Reference` · `Request` · `Schedule` · `Status` · `Usage Log` · `Requester Reference` · `Associated Party` · `Service Provider Reference`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Risk Test | 7 |
| Sensitivity Test | 7 |
| Liquidity and Cash Flow Test | 7 |
| Asset and Liability Valuation Test | 7 |

**Interfaz.** Action Terms: `Evaluate` · `Execute` · `Grant` · `Notify` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 26 | 17 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Evaluate` · `Execute` · `Grant` · `Notify` · `Request` · `Retrieve` |
| BQ `Asset and Liability Valuation Test` | `Evaluate` · `Execute` · `Notify` · `Request` · `Retrieve` |
| BQ `Liquidity and Cash Flow Test` | `Evaluate` · `Execute` · `Notify` · `Request` · `Retrieve` |
| BQ `Risk Test` | `Evaluate` · `Execute` · `Notify` · `Request` · `Retrieve` |
| BQ `Sensitivity Test` | `Evaluate` · `Execute` · `Notify` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Contribution Models

| | |
|---|---|
| **Patrón funcional** | `Design` |
| **Tipo de activo** | `Contribution Model` |
| **Artefacto genérico** | `Specification` |
| **Control Record** | `Contribution Model Specification` |
| **Ubicación Matrix** | Risk and Compliance › Models |

[↑ Índice](README.md)

---

## Operational Risk Models

| | |
|---|---|
| **Patrón funcional** | `Design` |
| **Tipo de activo** | `Opertional Risk Model` |
| **Artefacto genérico** | `Specification` |
| **Control Record** | `Opertional Risk Model Specification` |
| **Ubicación Matrix** | Risk and Compliance › Models |

[↑ Índice](README.md)

---

## Production Risk Models

| | |
|---|---|
| **Patrón funcional** | `Design` |
| **Tipo de activo** | `Production Risk Model` |
| **Artefacto genérico** | `Specification` |
| **Control Record** | `Production Risk Model Specification` |
| **Ubicación Matrix** | Risk and Compliance › Models |

[↑ Índice](README.md)

---

## Credit and Margin Management

| | |
|---|---|
| **Patrón funcional** | `Direct` |
| **Tipo de activo** | `Credit And Margins` |
| **Artefacto genérico** | `Strategy` |
| **Control Record** | `Credit And Margins Strategy` |
| **Ubicación Matrix** | Risk and Compliance › Models |

[↑ Índice](README.md)

---

## Business Risk Models

| | |
|---|---|
| **Patrón funcional** | `Design` |
| **Tipo de activo** | `Business Operation Risk Model` |
| **Artefacto genérico** | `Specification` |
| **Control Record** | `Business Operation Risk Model Specification` |
| **Ubicación Matrix** | Risk and Compliance › Models |

[↑ Índice](README.md)

---

## Customer Behavior Models

| | |
|---|---|
| **Patrón funcional** | `Design` |
| **Tipo de activo** | `Customer Behavior Model` |
| **Artefacto genérico** | `Specification` |
| **Control Record** | `Customer Behavior Model Specification` |
| **Ubicación Matrix** | Risk and Compliance › Models |

**Propósito.** This service domain handles the design and maintenance of a portfolio of customer behavior models

<details><summary><b>Atributos del Control Record</b> · 12</summary>

`Customer Behavior Model Type` · `Customer Behavior Model Purpose` · `Customer Behavior Model Deployment` · `Employee or Business Unit Reference` · `Customer Behavior Model Deployment Configuration` · `Customer Behavior Model Deployment Task Reference` · `Customer Behavior Model Deployment Task Record` · `Customer Behavior Model Status` · `Customer Behavior Model Usage` · `Customer Behavior Model Impact` · `Customer Behavior Model Version` · `Customer Behavior Model`

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
| BQ `Functional Requirements` | `Update` · `Exchange` · `Capture` · `Request` · `Retrieve` |
| BQ `Testing` | `Update` · `Exchange` · `Retrieve` |
| BQ `Production` | `Retrieve` · `Request` · `Execute` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Economic Capital

| | |
|---|---|
| **Patrón funcional** | `Analyze` |
| **Tipo de activo** | `Economic Capital` |
| **Artefacto genérico** | `Analysis` |
| **Control Record** | `Economic Capital Analysis` |
| **Ubicación Matrix** | Risk and Compliance › Models |

[↑ Índice](README.md)

---

## Credit Risk Models

| | |
|---|---|
| **Patrón funcional** | `Design` |
| **Tipo de activo** | `Credit Risk Model` |
| **Artefacto genérico** | `Specification` |
| **Control Record** | `Credit Risk Model Specification` |
| **Ubicación Matrix** | Risk and Compliance › Models |

**Propósito.** This service domain handles the design and maintenance of a portfolio of credit models

<details><summary><b>Atributos del Control Record</b> · 8</summary>

`Parameter Type` · `Selected Option` · `Description` · `Version` · `Status` · `Usage Log` · `Feedback` · `Service Provider Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Functional Requirements | 4 |
| Production | 4 |
| Testing | 4 |

**Interfaz.** Action Terms: `Retrieve` · `Capture` · `Exchange` · `Initiate` · `Control` · `Request` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 19 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Retrieve` · `Capture` · `Exchange` · `Initiate` · `Control` · `Request` · `Update` |
| BQ `Functional Requirements` | `Capture` · `Retrieve` · `Request` · `Update` |
| BQ `Production` | `Capture` · `Retrieve` · `Request` · `Update` |
| BQ `Testing` | `Capture` · `Retrieve` · `Request` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Financial Instrument Valuation Models

| | |
|---|---|
| **Patrón funcional** | `Design` |
| **Tipo de activo** | `Market Asset Valuation Model` |
| **Artefacto genérico** | `Specification` |
| **Control Record** | `Market Asset Valuation Model Specification` |
| **Ubicación Matrix** | Risk and Compliance › Models |

[↑ Índice](README.md)

---

## Market Risk Models

| | |
|---|---|
| **Patrón funcional** | `Design` |
| **Tipo de activo** | `Market Risk Model` |
| **Artefacto genérico** | `Specification` |
| **Control Record** | `Market Risk Model Specification` |
| **Ubicación Matrix** | Risk and Compliance › Models |

[↑ Índice](README.md)

---

## Liquidity Risk Models

| | |
|---|---|
| **Patrón funcional** | `Design` |
| **Tipo de activo** | `Liquidity Risk Model` |
| **Artefacto genérico** | `Specification` |
| **Control Record** | `Liquidity Risk Model Specification` |
| **Ubicación Matrix** | Risk and Compliance › Models |

[↑ Índice](README.md)

---

## Gap Analysis

| | |
|---|---|
| **Patrón funcional** | `Analyze` |
| **Tipo de activo** | `interest Rate Gap Risk` |
| **Artefacto genérico** | `Analysis` |
| **Control Record** | `interest Rate Gap Risk Analysis` |
| **Ubicación Matrix** | Risk and Compliance › Models |

[↑ Índice](README.md)

---

## Fraud Model

| | |
|---|---|
| **Patrón funcional** | `Design` |
| **Tipo de activo** | `Fraud Model` |
| **Artefacto genérico** | `Specification` |
| **Control Record** | `Fraud Model Specification` |
| **Ubicación Matrix** | Risk and Compliance › Models |

**Propósito.** This service domain handles the design and maintenance of a portfolio of fraud models

<details><summary><b>Atributos del Control Record</b> · 12</summary>

`Fraud Model Type` · `Fraud Model Purpose` · `Fraud Model Deployment` · `Employee/Business Unit Reference` · `Fraud Model Deployment Configuration` · `Fraud Model Deployment Task Reference` · `Fraud Model Deployment Task Record` · `Fraud Model Status` · `Fraud Model Usage` · `Fraud Model Impact` · `Fraud Model Version` · `Fraud Model`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Functional Requirements | 6 |
| Testing | 10 |
| Production | 3 |

**Interfaz.** Action Terms: `Create` · `Execute` · `Retrieve` · `Request` · `Capture` · `Exchange` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 15 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Create` · `Execute` · `Retrieve` · `Request` |
| BQ `Functional Requirements` | `Capture` · `Exchange` · `Update` · `Request` · `Retrieve` |
| BQ `Testing` | `Update` · `Exchange` · `Retrieve` |
| BQ `Production` | `Execute` · `Retrieve` · `Request` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---
