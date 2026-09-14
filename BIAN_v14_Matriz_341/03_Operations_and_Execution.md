# Operations and Execution

**BIAN Service Landscape V14.0 · vista Matrix** — 130 Service Domains

> Curso independiente de CPS Tech · No afiliado ni acreditado por BIAN e.V. · BIAN® es marca registrada de BIAN e.V., usada con fines descriptivos.

[← Volver al índice de los 341](README.md)

---

## Contenido

**Product Specific Fulfillment › Loans and Deposits** · 15

[Loan](#loan) · [Leasing](#leasing) · [Current Account](#current-account) · [Corporate Current Account](#corporate-current-account) · [Consumer Loan](#consumer-loan) · [Corporate Loan](#corporate-loan) · [Term Deposit](#term-deposit) · [Corporate Lease](#corporate-lease) · [Merchandising Loan](#merchandising-loan) · [Mortgage Loan](#mortgage-loan) · [Fiduciary Agreement](#fiduciary-agreement) · [Savings Account](#savings-account) · [Virtual Account](#virtual-account) · [Standing Order](#standing-order) · [Term Deposit Framework Agreement](#term-deposit-framework-agreement)

**Product Specific Fulfillment › Investment Management** · 5

[Investment Portfolio Planning](#investment-portfolio-planning) · [Investment Portfolio Analysis](#investment-portfolio-analysis) · [Investment Portfolio Management](#investment-portfolio-management) · [eTrading Workbench](#etrading-workbench) · [Investment Account](#investment-account)

**Product Specific Fulfillment › Trade Banking** · 15

[Letter of Credit](#letter-of-credit) · [Bank Guarantee](#bank-guarantee) · [Credit Management](#credit-management) · [Credit Facility](#credit-facility) · [Project Finance](#project-finance) · [Limit and Exposure Management](#limit-and-exposure-management) · [Syndicated Loan](#syndicated-loan) · [Cash Management And Account Services](#cash-management-and-account-services) · [Direct Debit Mandate](#direct-debit-mandate) · [Cheque Lock Box](#cheque-lock-box) · [Factoring](#factoring) · [Cash Concentration](#cash-concentration) · [Notional Pooling](#notional-pooling) · [Corporate Payroll Services](#corporate-payroll-services) · [Direct Debit](#direct-debit)

**Product Specific Fulfillment › Wholesale Trading** · 12

[Trading Book Oversight](#trading-book-oversight) · [Trading Models](#trading-models) · [Dealer Desk](#dealer-desk) · [Quote Management](#quote-management) · [Suitability Checking](#suitability-checking) · [Credit Risk Operations](#credit-risk-operations) · [Market Making](#market-making) · [ECM And DCM](#ecm-and-dcm) · [Program Trading](#program-trading) · [Trader Position Operations](#trader-position-operations) · [Market Order](#market-order) · [Market Order Execution](#market-order-execution)

**Product Specific Fulfillment › Cards** · 8

[Credit Card](#credit-card) · [Card Authorization](#card-authorization) · [Card Transaction Capture](#card-transaction-capture) · [Merchant Relations](#merchant-relations) · [Merchant Acquiring Facility](#merchant-acquiring-facility) · [Card Network Participant Facility](#card-network-participant-facility) · [Card Transaction Tracking](#card-transaction-tracking) · [Corporate Card Service](#corporate-card-service)

**Product Specific Fulfillment › Market Operations** · 12

[Mutual Fund Administration](#mutual-fund-administration) · [Hedge Fund Administration](#hedge-fund-administration) · [Unit Trust Administration](#unit-trust-administration) · [Trade Confirmation Matching](#trade-confirmation-matching) · [Order Allocation](#order-allocation) · [Securities Fails Processing](#securities-fails-processing) · [Trade and Price Reporting](#trade-and-price-reporting) · [Custody Administration](#custody-administration) · [Corporate Action](#corporate-action) · [Financial Instrument Valuation](#financial-instrument-valuation) · [Trade Clearing](#trade-clearing) · [Trade Settlement](#trade-settlement)

**Product Specific Fulfillment › Corporate Financing and Advisory Services** · 5

[Public Offering](#public-offering) · [Private Placement](#private-placement) · [Mergers and Acquisitions Advisory](#mergers-and-acquisitions-advisory) · [Corporate Tax Advisory](#corporate-tax-advisory) · [Corporate Finance](#corporate-finance)

**Product Specific Fulfillment › Consumer Services** · 11

[Corporate Trust Services](#corporate-trust-services) · [Currency Exchange](#currency-exchange) · [Bank Drafts](#bank-drafts) · [Brokered Product Proxy](#brokered-product-proxy) · [Consumer Investments](#consumer-investments) · [Customer Tax Handling](#customer-tax-handling) · [Consumer Advisory Services](#consumer-advisory-services) · [Trust Services](#trust-services) · [Funeral Policy](#funeral-policy) · [Claim Assessment](#claim-assessment) · [Claim Administration](#claim-administration)

**Cross Product Operations › Payments** · 11

[Financial Message Analysis](#financial-message-analysis) · [Financial Gateway](#financial-gateway) · [Central Cash Handling](#central-cash-handling) · [Card Financial Settlement](#card-financial-settlement) · [Card eCommerce Gateway](#card-ecommerce-gateway) · [Card Clearing](#card-clearing) · [Cheque Processing](#cheque-processing) · [Payment Rail](#payment-rail) · [Payment Settlement](#payment-settlement) · [Payment Confirmation](#payment-confirmation) · [Payment Orchestration](#payment-orchestration)

**Cross Product Operations › Account Management** · 12

[Reward Points Account](#reward-points-account) · [Product Combination](#product-combination) · [Position Management](#position-management) · [Position Keeping](#position-keeping) · [Fraud Evaluation](#fraud-evaluation) · [Fraud Diagnosis](#fraud-diagnosis) · [Customer Position](#customer-position) · [Counterparty Risk](#counterparty-risk) · [Accounts Receivable](#accounts-receivable) · [Account Reconciliation](#account-reconciliation) · [Securities Position Keeping](#securities-position-keeping) · [Transaction Engine](#transaction-engine)

**Cross Product Operations › Operational Services** · 20

[Reward Points Awards And Redemption](#reward-points-awards-and-redemption) · [Open Item Management](#open-item-management) · [Leasing Item Administration](#leasing-item-administration) · [Issued Device Tracking](#issued-device-tracking) · [Issued Device Administration](#issued-device-administration) · [Disbursement](#disbursement) · [Delinquent Account Handling](#delinquent-account-handling) · [Channel Activity History](#channel-activity-history) · [Channel Activity Analysis](#channel-activity-analysis) · [Card Transaction Switch](#card-transaction-switch) · [Card Collections](#card-collections) · [Customer Billing](#customer-billing) · [Internal Bank Account](#internal-bank-account) · [Processing Order](#processing-order) · [Incentive Program Directory](#incentive-program-directory) · [Incentive Account](#incentive-account) · [Rewards Menu](#rewards-menu) · [Rewards Inventory](#rewards-inventory) · [Rewards Delivery](#rewards-delivery) · [Issued Certificate Directory](#issued-certificate-directory)

**Cross Product Operations › Collateral Administration** · 4

[Collections](#collections) · [Collateral Allocation Management](#collateral-allocation-management) · [Party Asset Directory](#party-asset-directory) · [Collateral Asset Administration](#collateral-asset-administration)

---

## Loan

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Loan` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Loan Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |

**Propósito.** This service domain handles the fulfillment of a general loan product. This includes the initial set-up of the loan facility and the completion of scheduled and ad-hoc product processing tasks

<details><summary><b>Atributos del Control Record</b> · 38</summary>

`Product Instance Reference` · `Loan Number` · `Customer Reference` · `Party Reference` · `Customer Agreement Reference` · `Customer Credit Assessment Reference` · `Insurance Reference` · `Delinquency/Collection Reference` · `Bank Branch/Location Reference` · `Bank Accounting Unit Reference` · `Loan Type` · `Loan Amount` · `Loan Currency` · `Loan Rate Type` · `Loan Applicable Rate` · `Repayment Type` · `Interest Type` · `Interest Accrual Method` · `Loan Origination Date` · `Loan Maturity Date` · `Collateral Reference` · `Collateral Allocation` · `Tax Reference` · `Loan Access Terms` · `Entitlement Option Definition` · `Entitlement Option Setting` · `Restriction Option Definition` · `Restriction Option Setting` · `Associations` · `Association Type` · `Association Obligation/Entitlement` · `Association Reference` · `Loan Repayment Schedule` · `Staged Repayment Statement` · `Customer Commentary` · `Loan Outstanding Balance` · `Date Type` · `Date`

</details>

**Behavior Qualifiers** · 9

| Behavior Qualifier | Atributos |
|---|---:|
| Disbursement | 6 |
| Maintenance | 6 |
| Repayment | 7 |
| Modification | 3 |
| Financial Status Tracking | 0 |
| Interest | 18 |
| Charge | 18 |
| Debit and Credit | 7 |
| Collateral Allocation | 9 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Retrieve` · `Execute` · `Request` · `Exchange`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 24 | 18 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Retrieve` |
| BQ `Charge` | `Execute` · `Retrieve` |
| BQ `Interest` | `Retrieve` · `Execute` |
| BQ `Disbursement` | `Retrieve` |
| BQ `Debit and Credit` | `Update` · `Execute` · `Request` · `Retrieve` |
| BQ `Maintenance` | `Request` · `Retrieve` |
| BQ `Repayment` | `Update` · `Execute` · `Request` · `Retrieve` |
| BQ `Modification` | `Initiate` · `Exchange` · `Update` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Leasing

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Leasing` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Leasing Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |

**Propósito.** The leasing products enables customers to finance equipment purchases using the leased item as collateral when necessary

<details><summary><b>Atributos del Control Record</b> · 13</summary>

`Parameter Type` · `Selected Option` · `Type` · `Reference` · `Schedule` · `Status` · `Currency` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Booking Location` · `Account Type` · `Account Reference`

</details>

**Behavior Qualifiers** · 12

| Behavior Qualifier | Atributos |
|---|---:|
| Issued Device | 19 |
| Sweep | 17 |
| Charge | 18 |
| Debit and Credit | 14 |
| Deposit | 14 |
| Collateral Allocation | 9 |
| Financial Status Tracking | 7 |
| Booking | 7 |
| Payment | 33 |
| Interest | 25 |
| Amount Block | 10 |
| Corporate Action | 10 |

**Interfaz.** Action Terms: `Control` · `Execute` · `Exchange` · `Request` · `Initiate` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 44 | 26 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Execute` · `Exchange` · `Request` · `Initiate` · `Retrieve` · `Update` |
| BQ `Charge` | `Exchange` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Payment` | `Exchange` · `Initiate` · `Retrieve` · `Update` |
| BQ `Sweep` | `Exchange` · `Initiate` · `Retrieve` · `Update` |
| BQ `Deposit` | `Initiate` · `Retrieve` · `Update` |
| BQ `Collateral Allocation` | `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Corporate Action` | `Initiate` · `Retrieve` · `Update` |
| BQ `Issued Device` | `Initiate` · `Retrieve` · `Update` |
| BQ `Financial Status Tracking` | `Initiate` · `Retrieve` · `Update` |
| BQ `Debit and Credit` | `Initiate` · `Retrieve` · `Update` |
| BQ `Interest` | `Retrieve` · `Update` |
| BQ `Amount Block` | `Initiate` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Current Account

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Current Account` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Current Account Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |

**Propósito.** This service domain orchestrates a consumer checking/demand deposit account

<details><summary><b>Atributos del Control Record</b> · 25</summary>

`Product Instance Reference` · `Current Account Number` · `Customer Reference` · `Bank Branch/Location Reference` · `Account Type` · `Account Currency` · `Tax Reference` · `Entitlement Option Definition` · `Entitlement Option Setting` · `Restriction Option Definition` · `Restriction Option Setting` · `Associations` · `Association Type` · `Association Obligation or Entitlement` · `Association Reference` · `Linked Accounts` · `Link Type` · `Account Details` · `Limit Type` · `Limit Settings` · `Limit Value` · `Account Date Type` · `Account Date` · `Account Balance` · `Account Status`

</details>

**Behavior Qualifiers** · 10

| Behavior Qualifier | Atributos |
|---|---:|
| Sweep | 11 |
| Debit and Credit | 7 |
| Payment | 26 |
| Financial Status Tracking | 0 |
| Interest | 18 |
| Issued Device | 19 |
| Booking | 8 |
| Charge | 18 |
| Amount Block | 10 |
| Deposit | 7 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Retrieve` · `Execute` · `Exchange`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 34 | 20 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Retrieve` |
| BQ `Interest` | `Retrieve` · `Execute` |
| BQ `Charge` | `Initiate` · `Retrieve` · `Execute` · `Update` |
| BQ `Sweep` | `Execute` · `Initiate` · `Update` · `Retrieve` |
| BQ `Debit and Credit` | `Update` · `Initiate` · `Retrieve` · `Execute` |
| BQ `Payment` | `Initiate` · `Exchange` · `Execute` · `Update` · `Retrieve` |
| BQ `Issued Device` | `Update` · `Retrieve` · `Initiate` |
| BQ `Booking` | `Execute` |
| BQ `Deposit` | `Execute` · `Initiate` · `Update` · `Retrieve` |
| BQ `Amount Block` | `Retrieve` · `Update` · `Initiate` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Corporate Current Account

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Corporate Current Account` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Corporate Current Account Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |

**Propósito.** This service domain orchestrates a corporate checking/demand deposit account

<details><summary><b>Atributos del Control Record</b> · 23</summary>

`Product Instance Reference` · `Corporate Current Account Number` · `Customer Reference` · `Bank Branch/Location Reference` · `Account Type` · `Account Currency` · `Tax Reference` · `Entitlement Option Definition` · `Entitlement Option Setting` · `Restriction Option Definition` · `Restriction Option Setting` · `Associations` · `Association Type` · `Association Obligation/Entitlement` · `Association Reference` · `Linked Accounts` · `Link Type` · `Account Details` · `Account Date Type` · `Account Date` · `Limit Settings` · `Limit Value` · `Limit Type`

</details>

**Behavior Qualifiers** · 10

| Behavior Qualifier | Atributos |
|---|---:|
| Financial Status Tracking | 0 |
| Booking | 8 |
| Interest | 18 |
| Charge | 18 |
| Sweep | 10 |
| Issued Device | 19 |
| Payment | 26 |
| Debit and Credit | 8 |
| Amount Block | 10 |
| Deposit | 7 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Retrieve` · `Execute` · `Exchange`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 34 | 20 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Retrieve` |
| BQ `Interest` | `Retrieve` · `Execute` |
| BQ `Charge` | `Initiate` · `Execute` · `Retrieve` · `Update` |
| BQ `Sweep` | `Initiate` · `Update` · `Execute` · `Retrieve` |
| BQ `Debit and Credit` | `Initiate` · `Update` · `Execute` · `Retrieve` |
| BQ `Payment` | `Initiate` · `Update` · `Exchange` · `Execute` · `Retrieve` |
| BQ `Issued Device` | `Initiate` · `Update` · `Retrieve` |
| BQ `Amount Block` | `Initiate` · `Retrieve` · `Update` |
| BQ `Deposit` | `Execute` · `Retrieve` · `Initiate` · `Update` |
| BQ `Booking` | `Execute` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Consumer Loan

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Consumer Loan` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Consumer Loan Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |

**Propósito.** This service domain handles the fulfillment of a consumer loan product

<details><summary><b>Atributos del Control Record</b> · 38</summary>

`Product Instance Reference` · `Consumer Loan Number` · `Customer Reference` · `Party Reference` · `Customer Agreement Reference` · `Customer Credit Assessment Reference` · `Insurance Reference` · `Delinquency/Collection Reference` · `Bank Branch/Location Reference` · `Bank Accounting Unit Reference` · `Loan Type` · `Loan Amount` · `Loan Currency` · `Loan Rate Type` · `Loan Applicable Rate` · `Repayment Type` · `Interest Type` · `Interest Accrual Method` · `Loan Origination Date` · `Loan Maturity Date` · `Collateral Reference` · `Collateral Allocation` · `Tax Reference` · `Loan Access Terms` · `Entitlement Option Definition` · `Entitlement Option Setting` · `Restriction Option Definition` · `Restriction Option Setting` · `Associations` · `Association Type` · `Association Obligation/Entitlement` · `Association Reference` · `Loan Repayment Schedule` · `Staged Repayment Statement` · `Customer Commentary` · `Loan Outstanding Balance` · `Account Date Type` · `Account Date`

</details>

**Behavior Qualifiers** · 12

| Behavior Qualifier | Atributos |
|---|---:|
| Disbursement | 6 |
| Maintenance | 6 |
| Repayment | 7 |
| Financial Status Tracking | 0 |
| Amount Block | 10 |
| Booking | 8 |
| Interest | 18 |
| Debit and Credit | 7 |
| Issued Device | 19 |
| Charge | 18 |
| Modification | 5 |
| Collateral Allocation | 9 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Retrieve` · `Execute` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 29 | 24 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Retrieve` |
| BQ `Interest` | `Retrieve` · `Execute` |
| BQ `Charge` | `Execute` · `Retrieve` · `Update` |
| BQ `Disbursement` | `Retrieve` |
| BQ `Maintenance` | `Request` · `Retrieve` |
| BQ `Debit and Credit` | `Update` · `Execute` · `Request` · `Retrieve` |
| BQ `Repayment` | `Update` · `Execute` · `Request` · `Retrieve` |
| BQ `Amount Block` | `Initiate` · `Retrieve` · `Update` |
| BQ `Issued Device` | `Initiate` · `Retrieve` · `Update` |
| BQ `Booking` | `Execute` |
| BQ `Modification` | `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Corporate Loan

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Corporate Loan` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Corporate Loan Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |

**Propósito.** This service domain handles the fulfillment of a corporate loan product

<details><summary><b>Atributos del Control Record</b> · 38</summary>

`Product Instance Reference` · `Corporate Loan Number` · `Customer Reference` · `Party Reference` · `Customer Agreement Reference` · `Customer Credit Assessment Reference` · `Insurance Reference` · `Delinquency/Collection Reference` · `Bank Branch/Location Reference` · `Bank Accounting Unit Reference` · `Loan Type` · `Loan Amount` · `Loan Currency` · `Loan Rate Type` · `Loan Applicable Rate` · `Repayment Type` · `Interest Type` · `Interest Accrual Method` · `Loan Origination Date` · `Loan Maturity Date` · `Collateral Reference` · `Collateral Allocation` · `Tax Reference` · `Loan Access Terms` · `Entitlement Option Definition` · `Entitlement Option Setting` · `Restriction Option Definition` · `Restriction Option Setting` · `Associations` · `Association Type` · `Association Obligation/Entitlement` · `Association Reference` · `Loan Repayment Schedule` · `Staged Repayment Statement` · `Customer Commentary` · `Loan Outstanding Balance` · `Date Type` · `Date`

</details>

**Behavior Qualifiers** · 12

| Behavior Qualifier | Atributos |
|---|---:|
| Disbursement | 6 |
| Maintenance | 6 |
| Repayment | 7 |
| Financial Status Tracking | 0 |
| Amount Block | 10 |
| Booking | 8 |
| Interest | 18 |
| Charge | 18 |
| Issued Device | 19 |
| Debit and Credit | 7 |
| Modification | 4 |
| Collateral Allocation | 9 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Retrieve` · `Execute` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 29 | 24 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Retrieve` |
| BQ `Interest` | `Retrieve` · `Execute` |
| BQ `Charge` | `Execute` · `Retrieve` · `Update` |
| BQ `Disbursement` | `Retrieve` |
| BQ `Maintenance` | `Request` · `Retrieve` |
| BQ `Debit and Credit` | `Update` · `Request` · `Execute` · `Retrieve` |
| BQ `Repayment` | `Update` · `Execute` · `Request` · `Retrieve` |
| BQ `Amount Block` | `Initiate` · `Retrieve` · `Update` |
| BQ `Booking` | `Execute` |
| BQ `Issued Device` | `Initiate` · `Retrieve` · `Update` |
| BQ `Modification` | `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Term Deposit

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Term Deposit` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Term Deposit Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |

**Propósito.** A Term Deposit is an interest bearing account into which a customer can place a fixed amount of funds for a fixed amount of time. The Service Domain handles the opening, servicing and maturity processing of a Term Deposit.

<details><summary><b>Atributos del Control Record</b> · 50</summary>

`Product Instance Reference` · `Account Number` · `Customer Reference` · `Bank Branch/Location Reference` · `Account Type` · `Account Currency` · `Tax Reference` · `Entitlement Option Definition` · `Entitlement Option Setting` · `Restriction Option Definition` · `Restriction Option Setting` · `Associations` · `Association Type` · `Association Obligation/Entitlement` · `Association Reference` · `Linked Accounts` · `Link Type` · `Account Details` · `Account Date Type` · `Account Date` · `Statements Schedule` · `Statement Type` · `Statement Transaction Type` · `Statement Period` · `Statement Report` · `Term Deposit Amount` · `Term Deposit Duration` · `Term Deposit Maturity Date` · `Term Deposit Open Date` · `Initial Deposit Payer Reference` · `Initial Deposit Payer Name` · `Initial Deposit Payer Account Reference` · `Initial Deposit Payer Bank Reference` · `Initial Deposit Amount` · `Initial Deposit Value Date` · `Early Termination Fee Amount` · `Early Termination Document Reference` · `Early Termination Document Summary` · `Closing Settlement Payee Reference` · `Closing Settlement Payee Name` · `Closing Settlement Payee Account Reference` · `Closing Settlement Payee External Account Number` · `Closing Settlement Payee Bank Reference` · `Closing Settlement Amount` · `Closing Settlement Payment Mechanism Type` · `Sales Product Agreement Reference` · `Contract Number of Payer` · `Limit Type` · `Limit Value` · `Limit Settings`

</details>

**Behavior Qualifiers** · 11

| Behavior Qualifier | Atributos |
|---|---:|
| Financial Status Tracking | 0 |
| Interest | 20 |
| Charge | 19 |
| Sweep | 10 |
| Issued Device | 19 |
| Payments | 26 |
| Debit and Credit | 7 |
| Booking | 8 |
| Rollover | 3 |
| Amount Block | 10 |
| Deposit | 7 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Retrieve` · `Execute` · `Exchange`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 35 | 22 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Retrieve` |
| BQ `Interest` | `Retrieve` · `Execute` |
| BQ `Charge` | `Initiate` · `Execute` · `Retrieve` · `Update` |
| BQ `Sweep` | `Initiate` · `Update` · `Execute` · `Retrieve` |
| BQ `Debit and Credit` | `Initiate` · `Update` · `Execute` · `Retrieve` |
| BQ `Payments` | `Initiate` · `Update` · `Exchange` · `Execute` · `Retrieve` |
| BQ `Issued Device` | `Initiate` · `Update` · `Retrieve` |
| BQ `Booking` | `Execute` |
| BQ `Rollover` | `Update` |
| BQ `Amount Block` | `Initiate` · `Update` · `Retrieve` |
| BQ `Deposit` | `Initiate` · `Update` · `Execute` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Corporate Lease

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Corporate Lease` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Corporate Lease Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |

**Propósito.** The Corporate Lease product provides corporate customers with loans to support leasing activity for property and equipment

<details><summary><b>Atributos del Control Record</b> · 13</summary>

`Parameter Type` · `Selected Option` · `Type` · `Schedule` · `Status` · `Reference` · `Currency` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Booking Location` · `Account Type` · `Account Reference`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Administration | 7 |
| Fulfill | 7 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Request` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 18 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Administration` | `Exchange` · `Control` · `Retrieve` · `Request` · `Update` |
| BQ `Fulfill` | `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Update` · `Request` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Merchandising Loan

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Merchandising Loan` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Merchandising Loan Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |

**Propósito.** Fulfillment of loan product used in the purchase of a larger merchandise item such as a car or boat. The purchased item is typically treated as collateral for the loan

<details><summary><b>Atributos del Control Record</b> · 14</summary>

`Parameter Type` · `Selected Option` · `Type` · `Reference` · `Schedule` · `Status` · `Associated Party` · `Currency` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Booking Location` · `Account Type` · `Account Reference`

</details>

**Behavior Qualifiers** · 12

| Behavior Qualifier | Atributos |
|---|---:|
| Issued Device | 19 |
| Deposit | 14 |
| Interest | 25 |
| Payment | 33 |
| Billing | 7 |
| Charge | 25 |
| Sweep | 17 |
| Financial Status Tracking | 7 |
| Booking | 7 |
| Debit and Credit | 14 |
| Amount Block | 10 |
| Collateral Allocation | 9 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Request` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 47 | 28 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Billing` | `Exchange` · `Initiate` · `Retrieve` · `Update` |
| BQ `Charge` | `Exchange` · `Initiate` · `Retrieve` · `Request` · `Update` · `Execute` |
| BQ `Payment` | `Exchange` · `Initiate` · `Retrieve` · `Update` |
| BQ `Sweep` | `Exchange` · `Initiate` · `Retrieve` · `Update` |
| BQ `Collateral Allocation` | `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Deposit` | `Initiate` · `Retrieve` · `Update` |
| BQ `Issued Device` | `Initiate` · `Retrieve` · `Update` |
| BQ `Debit and Credit` | `Initiate` · `Retrieve` · `Update` |
| BQ `Booking` | `Retrieve` · `Update` |
| BQ `Interest` | `Retrieve` · `Update` · `Execute` |
| BQ `Financial Status Tracking` | `Execute` |
| BQ `Amount Block` | `Initiate` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Mortgage Loan

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Mortgage Loan` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Mortgage Loan Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |

**Propósito.** Fulfillment of a loan product for the purpose of property purchase. Note different servicing patterns can be applied to interest calculations and principle and interest repayments

<details><summary><b>Atributos del Control Record</b> · 13</summary>

`Parameter Type` · `Selected Option` · `Type` · `Reference` · `Schedule` · `Status` · `Currency` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Booking Location` · `Account Type` · `Account Reference`

</details>

**Behavior Qualifiers** · 12

| Behavior Qualifier | Atributos |
|---|---:|
| Payment | 33 |
| Deposit | 14 |
| Interest | 25 |
| Debit and Credit | 14 |
| Amount Block | 10 |
| Issued Device | 19 |
| Collateral Allocation | 9 |
| Charge | 25 |
| Billing | 7 |
| Booking | 7 |
| Financial Status Tracking | 7 |
| Sweep | 17 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Update` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 47 | 28 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Update` · `Request` |
| BQ `Billing` | `Exchange` · `Initiate` · `Retrieve` · `Update` |
| BQ `Charge` | `Exchange` · `Initiate` · `Retrieve` · `Request` · `Update` · `Execute` |
| BQ `Payment` | `Exchange` · `Initiate` · `Retrieve` · `Update` |
| BQ `Sweep` | `Exchange` · `Initiate` · `Retrieve` · `Update` |
| BQ `Deposit` | `Initiate` · `Retrieve` · `Update` |
| BQ `Collateral Allocation` | `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Issued Device` | `Initiate` · `Retrieve` · `Update` |
| BQ `Debit and Credit` | `Initiate` · `Retrieve` · `Update` |
| BQ `Booking` | `Retrieve` · `Update` |
| BQ `Interest` | `Retrieve` · `Update` · `Execute` |
| BQ `Financial Status Tracking` | `Execute` |
| BQ `Amount Block` | `Initiate` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Fiduciary Agreement

| | |
|---|---|
| **Patrón funcional** | `Agree Terms` |
| **Tipo de activo** | `Fiduciary Relationship` |
| **Artefacto genérico** | `Agreement` |
| **Control Record** | `Fiduciary Relationship Agreement` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |

**Propósito.** An agreement where the bank agrees to act on behalf of the customer in a financial matter and in accordance with the agreement terms

<details><summary><b>Atributos del Control Record</b> · 19</summary>

`Parameter Type` · `Selected Option` · `Type` · `Reference` · `Discharge Request` · `Discharge Schedule` · `Status` · `Associated Party` · `Customer Reference` · `Obligation` · `Entitlement` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Account Reference` · `Subject Matter` · `Product Reference` · `Calendar Reference` · `Associated Agreement Reference`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Fiduciary | 7 |
| Charge | 7 |

**Interfaz.** Action Terms: `Exchange` · `Initiate` · `Retrieve` · `Request` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 8 | 6 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| BQ `Fiduciary` | `Exchange` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Charge` | `Exchange` · `Retrieve` · `Request` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Savings Account

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Savings Account` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Savings Account Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |

**Propósito.** This service domain orchestrates a consumer savings account. The typical range of services and fees covers payments from and scheduled and ad-hoc deposits to the account, standing orders, sweeps, and liens.

<details><summary><b>Atributos del Control Record</b> · 23</summary>

`Product Instance Reference` · `Savings Account Number` · `Customer Reference` · `Bank Branch/Location Reference` · `Account Type` · `Account Currency` · `Tax Reference` · `Entitlement Option Definition` · `Entitlement Option Setting` · `Restriction Option Definition` · `Restriction Option Setting` · `Associations` · `Association Type` · `Association Obligation/Entitlement` · `Association Reference` · `Linked Accounts` · `Link Type` · `Account Details` · `Account Date Type` · `Account Date` · `Limit Settings` · `Limit Type` · `Limit Value`

</details>

**Behavior Qualifiers** · 10

| Behavior Qualifier | Atributos |
|---|---:|
| Financial Status Tracking | 0 |
| Interest | 18 |
| Charge | 18 |
| Debit and Credit | 8 |
| Payment | 26 |
| Issued Device | 19 |
| Sweep | 10 |
| Booking | 8 |
| Amount Block | 10 |
| Deposit | 7 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Retrieve` · `Execute` · `Exchange`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 34 | 20 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Retrieve` |
| BQ `Charge` | `Execute` · `Retrieve` · `Initiate` · `Update` |
| BQ `Interest` | `Retrieve` · `Execute` |
| BQ `Sweep` | `Initiate` · `Update` · `Execute` · `Retrieve` |
| BQ `Debit and Credit` | `Retrieve` · `Update` · `Initiate` · `Execute` |
| BQ `Payment` | `Initiate` · `Update` · `Execute` · `Exchange` · `Retrieve` |
| BQ `Issued Device` | `Initiate` · `Update` · `Retrieve` |
| BQ `Booking` | `Execute` |
| BQ `Amount Block` | `Initiate` · `Retrieve` · `Update` |
| BQ `Deposit` | `Update` · `Execute` · `Retrieve` · `Initiate` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Virtual Account

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Virtual Account` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Virtual Account Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |

**Propósito.** A Virtual Account is a bank account that is defined on an underlying real account. It can receive and send payments for the underlying account while behaving towards the outside as a separate account.

<details><summary><b>Atributos del Control Record</b> · 13</summary>

`Parameter Type` · `Selected Option` · `Type` · `Reference` · `Schedule` · `Status` · `Currency` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Booking Location` · `Account Type` · `Account Reference`

</details>

**Behavior Qualifiers** · 10

| Behavior Qualifier | Atributos |
|---|---:|
| Financial Status Tracking | 7 |
| Direct Debit | 7 |
| Booking | 8 |
| Amount Block | 10 |
| Maintenance | 7 |
| Issued Device | 19 |
| Interest | 25 |
| Payment | 15 |
| Charge | 25 |
| Withdrawal | 7 |

**Interfaz.** Action Terms: `Capture` · `Control` · `Exchange` · `Execute` · `Retrieve` · `Grant` · `Request` · `Initiate` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 42 | 24 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Capture` · `Control` · `Exchange` · `Execute` · `Retrieve` · `Grant` · `Request` · `Initiate` · `Update` |
| BQ `Direct Debit` | `Capture` · `Control` · `Grant` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Payment` | `Capture` · `Grant` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Charge` | `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Interest` | `Execute` · `Exchange` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Financial Status Tracking` | `Execute` |
| BQ `Amount Block` | `Initiate` · `Retrieve` · `Update` |
| BQ `Issued Device` | `Initiate` · `Retrieve` · `Update` |
| BQ `Booking` | `Execute` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Standing Order

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Standing Order` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Standing Order Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |

**Propósito.** Customers can issue standing orders to the bank. In most cases this is for the execution of a periodical payment, but there are other standing instructions like, sweeping balances at end of month, topping off excess funds for a current account, etc.

<details><summary><b>Atributos del Control Record</b> · 20</summary>

`Standing Order Regulation Reference` · `Standing Order Regulation Type` · `Standing Order Jurisdiction` · `Standing Order Product Reference` · `Standing Order Amount` · `Standing Order Frequency` · `Standing Order Identification` · `Standing Order Status` · `Standing Order Schedule` · `Standing Order Creditor Agent` · `Standing Order Creditor Account` · `Standing Order Debtor Account` · `Standing Order Creditor` · `Standing Order Debtor` · `Standing Order Amount Currency` · `Standing Order Validity Period` · `Standing Order Type` · `Number of Payments` · `Standing Order Account Reference` · `Standing Order Payment Transaction Reference`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Standing Order Payment | 14 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Request` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 11 | 6 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Standing Order Payment` | `Exchange` · `Initiate` · `Update` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Term Deposit Framework Agreement

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Term Deposit Framework Agreement` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Term Deposit Framework Agreement Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |

**Propósito.** A Term Deposit Framework Agreement is an agreement between a customer and the bank under which individual term deposits can be opened. It specifies standard conditions that will apply to each underlying term deposit.

<details><summary><b>Atributos del Control Record</b> · 18</summary>

`Parameter Type` · `Selected Option` · `Type` · `Calendar Reference` · `Status` · `Associated Party` · `Currency` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Booking Location` · `Account Type` · `Account Reference` · `Customer Reference` · `Position` · `Product Reference` · `Position Limit` · `Reference`

</details>

**Interfaz.** Action Terms: `Initiate` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 3 | 2 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Investment Portfolio Planning

| | |
|---|---|
| **Patrón funcional** | `Agree Terms` |
| **Tipo de activo** | `Managed Investment Portfolio` |
| **Artefacto genérico** | `Agreement` |
| **Control Record** | `Managed Investment Portfolio Agreement` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Investment Management |

**Propósito.** Agree the policies and required make-up of an investment portfolio and ensure all required bank and regulatory terms and conditions are addressed

<details><summary><b>Atributos del Control Record</b> · 11</summary>

`Customer Reference` · `Legal Entity Reference` · `Investment Portfolio Instance Reference` · `Investment Portfolio Agreement Type` · `Investment Portfolio Agreement Jurisdiction` · `Investment Portfolio Agreement Valid From/To Date` · `Investment Portfolio Agreement Signatories/Responsible Parties` · `Document Directory Entry Instance Reference` · `Customer Agreement Instance Reference` · `Party Relationship Procedure Instance Reference` · `Managed Investment Portfolio Agreement`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Investment Terms | 3 |

**Interfaz.** Action Terms: `Evaluate` · `Update` · `Control` · `Exchange` · `Retrieve` · `Request` · `Grant`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 11 | 4 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Evaluate` · `Update` · `Control` · `Exchange` · `Retrieve` · `Request` · `Grant` |
| BQ `Investment Terms` | `Request` · `Evaluate` · `Update` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Investment Portfolio Analysis

| | |
|---|---|
| **Patrón funcional** | `Analyze` |
| **Tipo de activo** | `Managed Investment Portfolio` |
| **Artefacto genérico** | `Analysis` |
| **Control Record** | `Managed Investment Portfolio Analysis` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Investment Management |

**Propósito.** Assess and report on investment portfolio make-up, valuation and performance

<details><summary><b>Atributos del Control Record</b> · 11</summary>

`Product Instance Reference` · `Customer Reference` · `Employee or Business Unit Reference` · `Investment Portfolio Instance Reference` · `Investment Portfolio Analysis Schedule` · `Investment Account Arrangement Instance Reference` · `Investment Portfolio Analysis Report` · `Investment Portfolio Analysis Type` · `Investment Portfolio Analysis Result` · `Investment Portfolio Analysis Reporting Date` · `Document Directory Entry Instance Reference`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Performance Analysis | 8 |

**Interfaz.** Action Terms: `Evaluate` · `Exchange` · `Request` · `Execute` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 9 | 4 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Evaluate` · `Exchange` · `Request` · `Execute` · `Retrieve` |
| BQ `Performance Analysis` | `Retrieve` · `Exchange` · `Request` · `Execute` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Investment Portfolio Management

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Managed Investment Portfolio` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Managed Investment Portfolio Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Investment Management |

**Propósito.** Manage an investment portfolio, initiating trading to leverage market opportunities, remaining within portfolio trading policies

<details><summary><b>Atributos del Control Record</b> · 8</summary>

`Investment Portfolio Trading Policies` · `Investment Portfolio Policy Type` · `Investment Portfolio Policy Description` · `Investment Portfolio Policy Limits and Constraints` · `Investment Portfolio Instance Reference` · `Investment Portfolio Holdings` · `Investment Portfolio Security Type` · `Investment Portfolio Security Holding`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Opportunity | 2 |
| Trade | 3 |
| Financial Status Tracking | 3 |

**Interfaz.** Action Terms: `Control` · `Initiate` · `Update` · `Exchange` · `Execute` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 14 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Initiate` · `Update` · `Exchange` · `Execute` · `Request` · `Retrieve` |
| BQ `Opportunity` | `Retrieve` |
| BQ `Financial Status Tracking` | `Retrieve` |
| BQ `Trade` | `Update` · `Request` · `Retrieve` · `Exchange` · `Initiate` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## eTrading Workbench

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `eTrading Workbench` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `eTrading Workbench Operating Session` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Investment Management |

**Propósito.** This Service Domain supports consumer securities trading of their investment portfolio through the bank

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Schedule` · `Status` · `Usage Log` · `Associated Party Reference` · `Service Provider Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Service Configuration` · `Reference`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Market Order Quotation | 6 |
| Market Order Initiation | 6 |
| Market Price Analysis | 6 |
| Investment Portfolio Valuation | 6 |

**Interfaz.** Action Terms: `Execute` · `Exchange` · `Control` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 36 | 17 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Execute` · `Exchange` · `Control` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Market Order Initiation` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Market Order Quotation` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Market Price Analysis` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Investment Portfolio Valuation` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Investment Account

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Investment Account` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Investment Account Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Investment Management |

**Propósito.** This service domain handles the non-cash holdings positions for a customer, covering multiple instruments as necessary

<details><summary><b>Atributos del Control Record</b> · 28</summary>

`Product Instance Reference` · `Investment Account Number` · `Customer Reference` · `Bank Branch/Location Reference` · `Linked Cash Account` · `Link Type` · `Account Details` · `Investment Account Type` · `Investment Account Instrument Profile` · `Investment Account Instrument Record` · `Instrument Type` · `Instrument Reference` · `Trading Marketplace Reference` · `Instrument Processing Schedule` · `Instrument Event Type` · `Instrument Event Description` · `Instrument Event Date` · `Tax Reference` · `Entitlement Option Definition` · `Entitlement Option Setting` · `Restriction Option Definition` · `Restriction Option Setting` · `Linked Accounts` · `Date Type` · `Date` · `Limit Type` · `Limit Value` · `Limit Settings`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Corporate Action | 10 |
| Debit and Credit | 8 |
| Charge | 18 |
| Deposit | 7 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Retrieve` · `Execute` · `Exchange` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 25 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Retrieve` |
| BQ `Debit and Credit` | `Retrieve` · `Execute` · `Update` · `Initiate` · `Exchange` |
| BQ `Corporate Action` | `Initiate` · `Exchange` · `Retrieve` · `Execute` · `Update` |
| BQ `Charge` | `Initiate` · `Update` · `Exchange` · `Execute` · `Retrieve` · `Request` |
| BQ `Deposit` | `Retrieve` · `Exchange` · `Initiate` · `Update` · `Execute` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Letter of Credit

| | |
|---|---|
| **Patrón funcional** | `Transact` |
| **Tipo de activo** | `Letter Of Credit` |
| **Artefacto genérico** | `Transaction` |
| **Control Record** | `Letter Of Credit Transaction` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Trade Banking |

**Propósito.** This Service Domain handles the pricing and issuance of letters of credit to its corporate customers in support of their international trading requirements

<details><summary><b>Atributos del Control Record</b> · 29</summary>

`Parameter Type` · `Selected Option` · `Status` · `Type` · `Reference` · `Letter Of Credit Agreement Reference` · `Letter Of Credit Additional Involved Party Reference` · `Letter Of Credit Involvement Type` · `Letter Of Credit Arrangement Reference` · `Letter of Credit Financial Instrument Reference` · `Letter of Credit Identification` · `Letter of Credit Name` · `Letter of Credit Purpose` · `Letter of Credit Type` · `Letter of Credit Amount` · `Letter of Credit Expiry Terms and Conditions` · `Letter of Credit Governance Rules and Law` · `Letter of Credit Underlying Transaction` · `Letter of Credit Presentation Details` · `Letter of Credit Enclosed File` · `Letter of Credit Involved Account Reference` · `Letter of Credit Obligor` · `Letter of Credit Applicant` · `Letter of Credit Issuer` · `Letter of Credit Beneficiary` · `Letter of Credit Advising Party` · `Letter of Credit Termination Terms and Conditions` · `Letter of Credit Issuance Terms and Conditions` · `Letter of Credit Delivery Channel`

</details>

**Behavior Qualifiers** · 8

| Behavior Qualifier | Atributos |
|---|---:|
| Seller Obligation Confirmation | 7 |
| Customer Collateral Allocation | 7 |
| Letter of Credit Definition and Pricing | 7 |
| Customer Payment | 7 |
| Letter of Credit Amendment | 19 |
| Letter of Credit Termination | 7 |
| Letter of Credit Demand Payment | 23 |
| Letter of Credit Issuance | 15 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 50 | 27 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Customer Collateral Allocation` | `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Notify` · `Request` · `Update` |
| BQ `Letter of Credit Issuance` | `Exchange` · `Execute` · `Retrieve` · `Initiate` · `Notify` · `Request` · `Update` |
| BQ `Customer Payment` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Retrieve` · `Request` · `Update` |
| BQ `Letter of Credit Definition and Pricing` | `Exchange` · `Execute` · `Notify` · `Request` · `Initiate` · `Retrieve` · `Update` |
| BQ `Seller Obligation Confirmation` | `Exchange` · `Execute` · `Initiate` · `Request` · `Notify` · `Retrieve` · `Update` |
| BQ `Letter of Credit Demand Payment` | `Exchange` · `Execute` · `Notify` · `Initiate` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Bank Guarantee

| | |
|---|---|
| **Patrón funcional** | `Transact` |
| **Tipo de activo** | `Bank Guarantee` |
| **Artefacto genérico** | `Transaction` |
| **Control Record** | `Bank Guarantee Transaction` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Trade Banking |

**Propósito.** This Service Domain handles the pricing and issuance of a broad range of bank guarantee instruments

<details><summary><b>Atributos del Control Record</b> · 26</summary>

`Bank Guarantee Customer Reference` · `Bank Guarantee Customer Name` · `Bank Guarantee Customer Branch Reference` · `Bank Guarantee Beneficiary Reference` · `Bank Guarantee Beneficiary Name` · `Bank Guarantee Beneficiary Bank Reference` · `Bank Guarantee Start Date` · `Bank Guarantee Expiry Date` · `Customer Tax Identifier` · `Bank Guarantee Amount` · `Bank Guarantee Currency Reference` · `Bank Guarantee Purpose` · `Credit Facility Reference` · `Collateral Allocation Management Reference` · `SWIFT Message ID` · `Document Directory Reference` · `Sales Product Agreement Reference` · `Entitlement Option Definition` · `Entitlement Option Setting` · `Restriction Option Definition` · `Restriction Option Setting` · `Customer Commentary` · `Association Type` · `Association Obligation` · `Association Reference` · `Bank Guarantee Status`

</details>

**Behavior Qualifiers** · 6

| Behavior Qualifier | Atributos |
|---|---:|
| Collection | 7 |
| Bank Guarantee Issuance and Booking | 7 |
| Bank Guarantee Payout | 7 |
| Customer Payment | 7 |
| Customer Collateral Allocation | 7 |
| Bank Guarantee Definition and Pricing | 7 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` · `Execute`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 50 | 23 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` · `Execute` |
| BQ `Collection` | `Exchange` · `Execute` · `Initiate` · `Request` · `Notify` · `Retrieve` · `Update` |
| BQ `Bank Guarantee Definition and Pricing` | `Exchange` · `Execute` · `Initiate` · `Request` · `Retrieve` · `Notify` · `Update` |
| BQ `Customer Payment` | `Execute` · `Exchange` · `Notify` · `Initiate` · `Request` · `Retrieve` · `Update` |
| BQ `Bank Guarantee Payout` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Customer Collateral Allocation` | `Exchange` · `Execute` · `Initiate` · `Request` · `Notify` · `Retrieve` · `Update` |
| BQ `Bank Guarantee Issuance and Booking` | `Execute` · `Exchange` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Credit Management

| | |
|---|---|
| **Patrón funcional** | `Assess` |
| **Tipo de activo** | `Credit Pricing` |
| **Artefacto genérico** | `Assessment` |
| **Control Record** | `Credit Pricing Assessment` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Trade Banking |

**Propósito.** This service domain provides a bank-wide function to qualify credit pricing for offered products and services

<details><summary><b>Atributos del Control Record</b> · 11</summary>

`Business Unit Reference` · `Customer Reference` · `Sector Reference` · `Product Type` · `Proposed Transaction Reference` · `Proposed Transaction Record` · `Proposed Transaction Type` · `Proposed Transaction Amount` · `Proposed Transaction Record Date` · `Proposed Transaction Booking Entity` · `Proposed Transaction Credit Pricing Assessment`

</details>

**Interfaz.** Action Terms: `Evaluate` · `Grant` · `Update` · `Exchange` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 5 | 2 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Evaluate` · `Grant` · `Update` · `Exchange` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Credit Facility

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Credit Line` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Credit Line Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Trade Banking |

**Propósito.** The Credit Facility Service Domain manages the Credit Facilities that a Corporate Customer has with the bank

<details><summary><b>Atributos del Control Record</b> · 34</summary>

`Product Instance Reference` · `Credit Facility Number` · `Customer Reference` · `Associated Party Reference` · `Customer Agreement Reference` · `Customer Credit Rating Reference` · `Insurance Reference` · `Bank Branch/Location Reference` · `Bank Accounting Unit Reference` · `Credit Facility Type` · `Credit Facility Amount` · `Credit Facility Currency` · `Credit Facility Rate Type` · `Credit Facility Maturity Date` · `Tax Reference` · `Entitlement Option Definition` · `Entitlement Option Setting` · `Restriction Option Definition` · `Restriction Option Setting` · `Associated Party Association Type` · `Associated Party Association Obligation` · `Customer Commentary` · `Credit Facility Association Type` · `Credit Facility Decreasing Schedule` · `Available Amount` · `Amount Block Amount` · `Amount Block Start Date` · `Amount Block Expiry Date` · `Amount Block Status` · `Credit Facility Opening Date` · `Credit Facility Closed Date` · `Sales Product Agreement Reference` · `Associated Product Conditions` · `Credit Facility Status`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Charge | 18 |
| Credit Allocation | 10 |

**Interfaz.** Action Terms: `Retrieve` · `Initiate` · `Execute` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 10 | 6 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Retrieve` · `Initiate` · `Update` |
| BQ `Credit Allocation` | `Initiate` · `Retrieve` · `Update` |
| BQ `Charge` | `Execute` · `Retrieve` · `Update` · `Initiate` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Project Finance

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Project Finance` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Project Finance Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Trade Banking |

**Propósito.** This Service Domain fulfills project financing by which major (government) projects can attract privet sector financing

<details><summary><b>Atributos del Control Record</b> · 18</summary>

`Parameter Type` · `Selected Option` · `Type` · `Calendar Reference` · `Status` · `Associated Party` · `Currency` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Booking Location` · `Account Type` · `Account Reference` · `Customer Reference` · `Position` · `Product Reference` · `Position Limit` · `Reference`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Maintenance | 7 |
| Instrument Design | 7 |
| Repayment | 15 |
| Placement | 7 |

**Interfaz.** Action Terms: `Control` · `Execute` · `Exchange` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 36 | 17 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Execute` · `Exchange` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Placement` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Maintenance` | `Exchange` · `Initiate` · `Notify` · `Retrieve` · `Execute` · `Request` · `Update` |
| BQ `Repayment` | `Exchange` · `Initiate` · `Request` · `Retrieve` · `Notify` · `Execute` · `Update` |
| BQ `Instrument Design` | `Execute` · `Notify` · `Initiate` · `Request` · `Exchange` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Limit and Exposure Management

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `Limit And Exposure` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `Limit And Exposure Management Plan` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Trade Banking |

[↑ Índice](README.md)

---

## Syndicated Loan

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Syndicated Loan` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Syndicated Loan Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Trade Banking |

**Propósito.** Handle the processing of syndicated loans with the bank playing the lead coordination role with other syndicate bank members. Note some initial preparation may have been made through prior customer offer processing.

<details><summary><b>Atributos del Control Record</b> · 13</summary>

`Parameter Type` · `Selected Option` · `Type` · `Reference` · `Schedule` · `Status` · `Currency` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Booking Location` · `Account Type` · `Account Reference`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Origination | 7 |
| Syndicate | 7 |
| Instrument Design | 7 |
| Fulfillment | 7 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Update` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 24 | 12 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Update` · `Request` |
| BQ `Fulfillment` | `Exchange` · `Retrieve` · `Request` · `Update` |
| BQ `Origination` | `Exchange` · `Retrieve` · `Request` · `Update` |
| BQ `Syndicate` | `Exchange` · `Retrieve` · `Request` · `Update` |
| BQ `Instrument Design` | `Initiate` · `Exchange` · `Retrieve` · `Request` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Cash Management And Account Services

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Cash Management And Account Services` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Cash Management And Account Services Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Trade Banking |

**Propósito.** This service domain orchestrates a cash management and accounting services facility typically used by corporations

<details><summary><b>Atributos del Control Record</b> · 23</summary>

`Product Instance Reference` · `Cash Management And Account Services Account Number` · `Customer Reference` · `Bank Branch/Location Reference` · `Account Type` · `Account Currency` · `Tax Reference` · `Entitlement Option Definition` · `Entitlement Option Setting` · `Restriction Option Definition` · `Restriction Option Setting` · `Associations` · `Association Type` · `Association Obligation/Entitlement` · `Association Reference` · `Linked Accounts` · `Link Type` · `Account Details` · `Limit Type` · `Limit Settings` · `Limit Value` · `Account Date Type` · `Account Date`

</details>

**Behavior Qualifiers** · 9

| Behavior Qualifier | Atributos |
|---|---:|
| Positive Pay | 4 |
| Sweep | 10 |
| Amount Block | 10 |
| Issued Device | 19 |
| Interest | 18 |
| Charge | 18 |
| Debit and Credit | 7 |
| Deposit | 7 |
| Payment | 26 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Retrieve` · `Execute` · `Exchange` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 34 | 20 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Retrieve` |
| BQ `Interest` | `Retrieve` |
| BQ `Charge` | `Initiate` · `Retrieve` · `Execute` |
| BQ `Sweep` | `Initiate` · `Retrieve` · `Execute` · `Update` |
| BQ `Debit and Credit` | `Execute` · `Initiate` · `Update` · `Retrieve` |
| BQ `Payment` | `Initiate` · `Execute` · `Update` · `Exchange` · `Retrieve` |
| BQ `Issued Device` | `Initiate` · `Update` · `Request` · `Retrieve` |
| BQ `Positive Pay` | `Retrieve` · `Exchange` |
| BQ `Deposit` | `Initiate` · `Update` · `Execute` · `Retrieve` |
| BQ `Amount Block` | `Initiate` · `Update` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Direct Debit Mandate

| | |
|---|---|
| **Patrón funcional** | `Catalog` |
| **Tipo de activo** | `Direct Debit Mandate` |
| **Artefacto genérico** | `Directory Entry` |
| **Control Record** | `Direct Debit Mandate Directory Entry` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Trade Banking |

**Propósito.** This service domains manages the customer mandates associated with direct debit processing for a corporate client

<details><summary><b>Atributos del Control Record</b> · 7</summary>

`Mandated Customer Reference` · `Mandate Description` · `Mandate Collection Valid Period` · `Direct Debit Mandate Reference` · `Reference` · `Customer Product Instance Reference` · `Direct Debit Mandate Payee Reference`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Mandate Registration | 18 |

**Interfaz.** Action Terms: `Register` · `Retrieve` · `Update` · `Control` · `Execute` · `Exchange` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 10 | 4 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Register` · `Retrieve` · `Update` · `Control` |
| BQ `Mandate Registration` | `Register` · `Update` · `Execute` · `Exchange` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Cheque Lock Box

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Lock Box` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Lock Box Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Trade Banking |

**Propósito.** This Service Domain support paper cheque processing services offered to corporate customers

<details><summary><b>Atributos del Control Record</b> · 18</summary>

`Parameter Type` · `Selected Option` · `Type` · `Calendar Reference` · `Status` · `Associated Party` · `Currency` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Booking Location` · `Account Type` · `Account Reference` · `Customer Reference` · `Position` · `Product Reference` · `Position Limit` · `Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Issue Resolution | 7 |
| Transaction Batch | 11 |
| Payment | 7 |

**Interfaz.** Action Terms: `Notify` · `Control` · `Exchange` · `Execute` · `Initiate` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 25 | 13 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Notify` · `Control` · `Exchange` · `Execute` · `Initiate` · `Request` · `Retrieve` · `Update` |
| BQ `Issue Resolution` | `Execute` · `Exchange` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Payment` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Transaction Batch` | `Initiate` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Factoring

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Factoring` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Factoring Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Trade Banking |

**Propósito.** This Service Domain supports a factoring service for corporate customers enabling them to convert accounts receivable into immediate funds at a discount

<details><summary><b>Atributos del Control Record</b> · 18</summary>

`Parameter Type` · `Selected Option` · `Type` · `Calendar Reference` · `Status` · `Associated Party` · `Currency` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Booking Location` · `Account Type` · `Account Reference` · `Customer Reference` · `Position` · `Product Reference` · `Position Limit` · `Reference`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Factoring Processing | 7 |
| Account Receivable Factoring | 7 |
| Factoring Purchase | 7 |
| Factoring Evaluation | 7 |

**Interfaz.** Action Terms: `Exchange` · `Control` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 36 | 17 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Exchange` · `Control` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Account Receivable Factoring` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Factoring Processing` | `Exchange` · `Execute` · `Notify` · `Initiate` · `Request` · `Retrieve` · `Update` |
| BQ `Factoring Evaluation` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Factoring Purchase` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Cash Concentration

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Account Balance Sweeping` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Account Balance Sweeping Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Trade Banking |

**Propósito.** Cash Concentration is a cash management service aimed at moving a balance, or part of a balance of an account to a different account to meet various requirements

<details><summary><b>Atributos del Control Record</b> · 18</summary>

`Parameter Type` · `Selected Option` · `Type` · `Calendar Reference` · `Status` · `Associated Party` · `Currency` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Booking Location` · `Account Type` · `Account Reference` · `Customer Reference` · `Position` · `Product Reference` · `Position Limit` · `Reference`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Cash Transfer | 7 |

**Interfaz.** Action Terms: `Control` · `Request` · `Exchange` · `Notify` · `Execute` · `Update` · `Initiate` · `Retrieve` · `Activate`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 16 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Request` · `Exchange` · `Notify` · `Execute` · `Update` · `Initiate` · `Retrieve` · `Activate` |
| BQ `Cash Transfer` | `Exchange` · `Execute` · `Initiate` · `Request` · `Notify` · `Update` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Notional Pooling

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Notional Pooling` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Notional Pooling Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Trade Banking |

**Propósito.** Notional pooling allows corporate customer with multiple active accounts to pool credit and debit balances to provide a single centralized liquidity position and to minimize interest expense, simplify cash management and retain a degree of local autonomy to the accounts

<details><summary><b>Atributos del Control Record</b> · 19</summary>

`Parameter Type` · `Selected Option` · `Type` · `Calendar Reference` · `Status` · `Associated Party` · `Currency` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Booking Location` · `Account Type` · `Account Reference` · `Customer Reference` · `Position` · `Product Reference` · `Position Limit` · `Reference` · `Arrangement Reference`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Cash Transfer | 7 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Notify` · `Request` · `Initiate` · `Retrieve` · `Execute` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 15 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Notify` · `Request` · `Initiate` · `Retrieve` · `Update` · `Execute` |
| BQ `Cash Transfer` | `Execute` · `Exchange` · `Request` · `Update` · `Notify` · `Initiate` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Corporate Payroll Services

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Employee Payment Services` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Employee Payment Services Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Trade Banking |

**Propósito.** The Corporate Payroll Services Service Domain handles payroll payment processing for the employees of a corporate customer

<details><summary><b>Atributos del Control Record</b> · 18</summary>

`Parameter Type` · `Selected Option` · `Type` · `Calendar Reference` · `Status` · `Associated Party` · `Currency` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Booking Location` · `Account Type` · `Account Reference` · `Customer Reference` · `Position` · `Product Reference` · `Position Limit` · `Reference`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Transaction Batch | 0 |
| Issue Resolution | 7 |

**Interfaz.** Action Terms: `Control` · `Initiate` · `Execute` · `Notify` · `Request` · `Retrieve` · `Exchange` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 14 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Initiate` · `Execute` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Issue Resolution` | `Exchange` · `Initiate` · `Execute` · `Update` · `Request` · `Retrieve` · `Notify` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Direct Debit

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Direct Debit` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Direct Debit Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Trade Banking |

**Propósito.** Fulfils a direct debit agreement. Handles the creditor side of direct debits

<details><summary><b>Atributos del Control Record</b> · 13</summary>

`Parameter Type` · `Selected Option` · `Type` · `Reference` · `Schedule` · `Status` · `Currency` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Booking Location` · `Account Type` · `Account Reference`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Reporting | 7 |
| Payment Batch | 7 |

**Interfaz.** Action Terms: `Control` · `Retrieve` · `Exchange` · `Execute` · `Update` · `Initiate` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 11 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Retrieve` · `Update` · `Initiate` · `Request` |
| BQ `Payment Batch` | `Retrieve` · `Execute` |
| BQ `Reporting` | `Retrieve` · `Initiate` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Trading Book Oversight

| | |
|---|---|
| **Patrón funcional** | `Manage` |
| **Tipo de activo** | `Trading Position` |
| **Artefacto genérico** | `Management Plan` |
| **Control Record** | `Trading Position Management Plan` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Wholesale Trading |

**Propósito.** This Service Domain oversees the bank's trading book (a type of account ledger that records details of frequently traded securities held by the bank) to manage the banks market risk

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Type` · `Reference` · `Budget Type` · `Budget` · `Assignment` · `Duty` · `Description` · `BudgetBalance` · `Associated Party` · `Subject Matter`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Trading Book Risk Mitigation | 8 |
| Trading Book Analysis and Reporting | 8 |

**Interfaz.** Action Terms: `Control` · `Notify` · `Update` · `Exchange` · `Request` · `Grant` · `Retrieve` · `Create`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 20 | 11 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Notify` · `Update` · `Exchange` · `Grant` · `Request` · `Retrieve` · `Create` |
| BQ `Trading Book Analysis and Reporting` | `Exchange` · `Update` · `Grant` · `Notify` · `Request` · `Retrieve` |
| BQ `Trading Book Risk Mitigation` | `Request` · `Update` · `Exchange` · `Grant` · `Notify` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Trading Models

| | |
|---|---|
| **Patrón funcional** | `Design` |
| **Tipo de activo** | `Trading Model` |
| **Artefacto genérico** | `Specification` |
| **Control Record** | `Trading Model Specification` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Wholesale Trading |

[↑ Índice](README.md)

---

## Dealer Desk

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `Dealer Desk` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `Dealer Desk Operating Session` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Wholesale Trading |

**Propósito.** The Dealer Workbench represents the bank dealing desk facility supporting one or more trading lines of activity

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Schedule` · `Status` · `Usage Log` · `Associated Party Reference` · `Service Provider Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Service Configuration` · `Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Dealer Desk Consolidated Position Tracking | 6 |
| Dealer Desk Trading Assignment and Limits | 6 |
| Information Feed Administration | 6 |

**Interfaz.** Action Terms: `Exchange` · `Execute` · `Control` · `Initiate` · `Request` · `Notify` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 29 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Exchange` · `Execute` · `Control` · `Initiate` · `Request` · `Notify` · `Retrieve` · `Update` |
| BQ `Dealer Desk Consolidated Position Tracking` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Update` · `Retrieve` |
| BQ `Dealer Desk Trading Assignment and Limits` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Information Feed Administration` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Update` · `Retrieve` · `Request` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Quote Management

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Quotation` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Quotation Procedure` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Wholesale Trading |

**Propósito.** This service domain handles the procedure used by traders to obtain and selecting quotes from market makers

<details><summary><b>Atributos del Control Record</b> · 21</summary>

`Parameter Type` · `Selected Option` · `Request` · `Schedule` · `Status` · `Associated Party Reference` · `Business Unit Reference` · `Service Provider Reference` · `Financial Facility Reference` · `Employee Reference` · `Customer Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Product and Service Type` · `Product and Service Instance` · `Transaction Type` · `Transaction` · `Financial Transaction Arrangement` · `Customer Agreement Reference` · `Reference`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Market Quote Selection | 8 |
| Market Quote Request | 8 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 22 | 11 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Market Quote Selection` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Market Quote Request` | `Exchange` · `Execute` · `Initiate` · `Request` · `Notify` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Suitability Checking

| | |
|---|---|
| **Patrón funcional** | `Assess` |
| **Tipo de activo** | `Suitability` |
| **Artefacto genérico** | `Assessment` |
| **Control Record** | `Suitability Assessment` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Wholesale Trading |

**Propósito.** Confirm that all involved counterparties are suitable for a proposed market trade.

<details><summary><b>Atributos del Control Record</b> · 16</summary>

`Employee or Business Unit Reference` · `Customer Reference` · `Market Order Type` · `Investment Portfolio Instance Reference` · `Customer Market Order Processing Instruction` · `Proposed Market Order Transaction` · `Investment Account Arrangement Instance Reference` · `Security Type` · `Amount` · `Date Type` · `Date` · `Type` · `Document Directory Entry Instance Reference` · `Correspondence Instance Reference` · `Suitability Compliance Assessment Work Products` · `Suitability Compliance Assessment Result`

</details>

**Interfaz.** Action Terms: `Evaluate` · `Update` · `Exchange` · `Request` · `Grant` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 6 | 2 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Evaluate` · `Update` · `Exchange` · `Request` · `Grant` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Credit Risk Operations

| | |
|---|---|
| **Patrón funcional** | `Monitor` |
| **Tipo de activo** | `Trading Credit Position` |
| **Artefacto genérico** | `State` |
| **Control Record** | `Trading Credit Position Measurement` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Wholesale Trading |

**Propósito.** This Service Domain monitors counterparty credit limits in the trading unit

<details><summary><b>Atributos del Control Record</b> · 14</summary>

`Parameter Type` · `Selected Option` · `Type` · `Reference` · `Description` · `Schedule` · `Status` · `Usage Log` · `Update Log` · `Customer Reference` · `Product Reference` · `Service Configuration` · `Service Configuration Tresholds and Limits` · `Service Configuration Notification Arrangements`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Trading Counterparty Credit Limit Indicator | 8 |

**Interfaz.** Action Terms: `Control` · `Evaluate` · `Execute` · `Notify` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 10 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Evaluate` · `Execute` · `Notify` · `Request` |
| BQ `Trading Counterparty Credit Limit Indicator` | `Evaluate` · `Execute` · `Notify` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Market Making

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Market Making` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Market Making Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Wholesale Trading |

**Propósito.** This Service Domain enables the bank to fulfill its market making function typically in collaboration with a trading exchange. The bank maintains a buy/sell quote for the securities it supports as a market maker and accepts buy/sell orders on request

<details><summary><b>Atributos del Control Record</b> · 18</summary>

`Parameter Type` · `Selected Option` · `Type` · `Calendar Reference` · `Status` · `Associated Party` · `Currency` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Booking Location` · `Account Type` · `Account Reference` · `Customer Reference` · `Position` · `Product Reference` · `Position Limit` · `Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Order | 7 |
| Position Tracking | 7 |
| Quote | 7 |

**Interfaz.** Action Terms: `Control` · `Initiate` · `Exchange` · `Execute` · `Notify` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 29 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Initiate` · `Exchange` · `Execute` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Quote` | `Exchange` · `Execute` · `Request` · `Notify` · `Initiate` · `Retrieve` · `Update` |
| BQ `Order` | `Execute` · `Exchange` · `Initiate` · `Retrieve` · `Notify` · `Request` · `Update` |
| BQ `Position Tracking` | `Exchange` · `Execute` · `Request` · `Initiate` · `Notify` · `Update` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## ECM And DCM

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `ECM And DCM` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `ECM And DCM Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Wholesale Trading |

**Propósito.** Supports the specification, pricing and issuance of equity and debt primary capital market products for corporate financing services

<details><summary><b>Atributos del Control Record</b> · 13</summary>

`Product Instance Reference` · `Customer Reference` · `Bank Branch/Location Reference` · `Business Unit Reference` · `Document Directory Entry Instance Reference` · `Associations` · `Association Type` · `Association Obligation/Entitlement` · `Association Reference` · `ECM And DCM Fulfillment Schedule` · `Date Type` · `Date` · `ECM And DCM Instrument Record`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Instrument Design | 7 |
| Prospectus | 7 |
| Placement | 9 |

**Interfaz.** Action Terms: `Initiate` · `Request` · `Retrieve` · `Update` · `Exchange`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 14 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Exchange` · `Request` · `Retrieve` |
| BQ `Instrument Design` | `Request` · `Retrieve` · `Update` |
| BQ `Prospectus` | `Update` · `Request` · `Retrieve` |
| BQ `Placement` | `Update` · `Retrieve` · `Request` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Program Trading

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `Program Trading` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `Program Trading Operating Session` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Wholesale Trading |

**Propósito.** This Service Domain supports a program trading capability where the trading decisions are made based on predefined/programmed rules and policies. Manual oversight and monitoring capabilities are supported as appropriate

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Schedule` · `Status` · `Usage Log` · `Associated Party Reference` · `Service Provider Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Service Configuration` · `Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Program Trade Execution | 6 |
| Program Traded Portfolio Algorithm | 6 |
| Program Traded Portfolio Maintenance | 6 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 29 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Program Trade Execution` | `Exchange` · `Execute` · `Initiate` · `Request` · `Retrieve` · `Notify` · `Update` |
| BQ `Program Traded Portfolio Algorithm` | `Exchange` · `Execute` · `Initiate` · `Request` · `Notify` · `Retrieve` · `Update` |
| BQ `Program Traded Portfolio Maintenance` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Trader Position Operations

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `Traded Position` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `Traded Position Operating Session` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Wholesale Trading |

**Propósito.** This Service Domain supports the activities of individual traders working within a trading book group

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Schedule` · `Status` · `Usage Log` · `Associated Party Reference` · `Service Provider Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Service Configuration` · `Reference`

</details>

**Behavior Qualifiers** · 5

| Behavior Qualifier | Atributos |
|---|---:|
| Trade Deal Blotter | 6 |
| Trade Quote and Pricing | 6 |
| Trade Capture and Reporting | 6 |
| Trader Security Position Management and Analysis | 6 |
| Trader Trading Permissions and Limits | 6 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Update` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 43 | 20 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Update` · `Retrieve` |
| BQ `Trade Capture and Reporting` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Trade Deal Blotter` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Trade Quote and Pricing` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Trader Security Position Management and Analysis` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Trader Trading Permissions and Limits` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Market Order

| | |
|---|---|
| **Patrón funcional** | `Transact` |
| **Tipo de activo** | `Market Order` |
| **Artefacto genérico** | `Transaction` |
| **Control Record** | `Market Order Transaction` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Wholesale Trading |

**Propósito.** Market Order records an instruction from a customer or his or her representative to buy or sell securities. It follows the order during its lifetime and reports back to the requestor on the execution.

<details><summary><b>Atributos del Control Record</b> · 15</summary>

`Market Order Instruction Type` · `Customer Reference` · `Employee or Business Unit Reference` · `Investment Portfolio Instance Reference` · `Customer Market Order Processing Instruction` · `Document Directory Entry Instance Reference` · `Correspondence Instance Reference` · `Market Order Transaction` · `Investment Account Arrangement Instance Reference` · `Current Account Arrangement Instance Reference` · `Market Order Type` · `Security Type` · `Amount` · `Date Type` · `Date`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Compliance | 3 |
| Confirmation | 1 |
| Quote | 1 |
| Trade Initiation | 3 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Retrieve` · `Exchange`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 8 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Retrieve` |
| BQ `Confirmation` | `Retrieve` |
| BQ `Quote` | `Retrieve` |
| BQ `Compliance` | `Retrieve` |
| BQ `Trade Initiation` | `Exchange` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Market Order Execution

| | |
|---|---|
| **Patrón funcional** | `Transact` |
| **Tipo de activo** | `Market Trade` |
| **Artefacto genérico** | `Transaction` |
| **Control Record** | `Market Trade Transaction` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Wholesale Trading |

**Propósito.** The Market Order Execution Service Domain is responsible for the booking of securities transactions (e.g. resulting from market orders or some types of corporate actions) on investment accounts, so in terms of security name plus quantity.

<details><summary><b>Atributos del Control Record</b> · 13</summary>

`Market Order Transaction Instance Reference` · `Customer Reference` · `Employee or Business Unit Reference` · `Customer Market Order Processing Instruction` · `Market Order Transaction` · `Investment Account Arrangement Instance Reference` · `Current Account Arrangement Instance Reference` · `Market Order Type` · `Security Type` · `Amount` · `Date Type` · `Date` · `Market Order Trade Initiation Instance Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Quote | 3 |
| Trade Initiation | 3 |
| Position | 11 |

**Interfaz.** Action Terms: `Request` · `Initiate` · `Update` · `Control` · `Exchange` · `Retrieve` · `Execute`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 16 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Request` · `Initiate` · `Update` · `Retrieve` |
| BQ `Position` | `Control` · `Retrieve` · `Request` · `Exchange` |
| BQ `Trade Initiation` | `Exchange` · `Retrieve` · `Initiate` · `Update` · `Execute` · `Request` |
| BQ `Quote` | `Initiate` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Credit Card

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Credit Card` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Credit Card Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Cards |

**Propósito.** This service domain orchestrates the scheduled maintenance and transactional activities associated with credit card product fulfillment

<details><summary><b>Atributos del Control Record</b> · 32</summary>

`Product Instance Reference` · `Customer Reference` · `Party Reference` · `Bank Branch/Location Reference` · `Account Currency` · `Secondary Billing Currency` · `Tax Reference` · `Entitlement Option Definition` · `Entitlement Option Setting` · `Restriction Option Definition` · `Restriction Option Setting` · `Allowed Access` · `Configuration/Options` · `Option Definition` · `Option Setting` · `Associations` · `Association Type` · `Association Obligation/Entitlement` · `Association Reference` · `Linked Accounts` · `Link Type` · `Account Details` · `Date Type` · `Date` · `Statements Schedule` · `Statement Type` · `Statement Transaction Type` · `Statement Period` · `Statement Report` · `Limit Type` · `Limit Value` · `Limit Settings`

</details>

**Behavior Qualifiers** · 8

| Behavior Qualifier | Atributos |
|---|---:|
| Billing | 9 |
| Repayment | 9 |
| Card Payment | 16 |
| Credit Plan | 3 |
| Financial Status Tracking | 0 |
| Interest | 18 |
| Charge | 18 |
| Issued Device | 19 |

**Interfaz.** Action Terms: `Initiate` · `Retrieve` · `Update` · `Control` · `Execute` · `Exchange` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 28 | 16 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Retrieve` · `Update` · `Control` |
| BQ `Interest` | `Retrieve` · `Execute` |
| BQ `Charge` | `Retrieve` · `Update` · `Execute` |
| BQ `Billing` | `Execute` · `Update` · `Retrieve` |
| BQ `Repayment` | `Update` · `Execute` · `Retrieve` |
| BQ `Card Payment` | `Update` · `Exchange` · `Retrieve` · `Execute` |
| BQ `Issued Device` | `Initiate` · `Update` · `Exchange` · `Request` · `Retrieve` |
| BQ `Credit Plan` | `Initiate` · `Update` · `Retrieve` · `Request` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Card Authorization

| | |
|---|---|
| **Patrón funcional** | `Assess` |
| **Tipo de activo** | `Credit Card Authorization` |
| **Artefacto genérico** | `Assessment` |
| **Control Record** | `Credit Card Authorization Assessment` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Cards |

**Propósito.** This service domain is responsible for the real time card authorization decisions for credit/charge cards

<details><summary><b>Atributos del Control Record</b> · 21</summary>

`Network Reference` · `Participant Acquirer Bank Reference` · `Participant Issuer Bank Reference` · `Card Transaction Record` · `Card Transaction Product Instance Reference` · `Card Holder Reference` · `Card Transaction Issued Device Reference` · `Card Transaction Network Reference` · `Card Transaction Issuing Bank Reference` · `Card Transaction Merchant Acquiring Bank Reference` · `Card Transaction Type` · `Card Transaction Currency` · `Card Transaction Amount Type` · `Card Transaction Amount` · `Card Transaction Merchant Reference` · `Card Transaction Location Reference` · `Card Transaction Product and Service Reference` · `Card Transaction Date and Time` · `Card Transaction FX Conversion Charge` · `Card Transaction Intercharge Fee` · `Card Transaction Authorization Record`

</details>

**Behavior Qualifiers** · 6

| Behavior Qualifier | Atributos |
|---|---:|
| Device Check | 7 |
| Authentication | 7 |
| Credit Check | 1 |
| Fraud Check | 1 |
| Stand In | 2 |
| Authorization | 7 |

**Interfaz.** Action Terms: `Update` · `Evaluate` · `Exchange` · `Execute` · `Request` · `Grant` · `Retrieve` · `Control`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 16 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Update` · `Evaluate` · `Exchange` · `Execute` · `Request` · `Grant` · `Retrieve` · `Control` |
| BQ `Device Check` | `Update` · `Retrieve` |
| BQ `Authentication` | `Retrieve` · `Update` |
| BQ `Fraud Check` | `Retrieve` |
| BQ `Credit Check` | `Retrieve` |
| BQ `Stand In` | `Retrieve` |
| BQ `Authorization` | `Evaluate` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Card Transaction Capture

| | |
|---|---|
| **Patrón funcional** | `Transact` |
| **Tipo de activo** | `Card Financial Capture` |
| **Artefacto genérico** | `Transaction` |
| **Control Record** | `Card Financial Capture Transaction` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Cards |

**Propósito.** A distributed facility to capture card transactions at the point of sale

<details><summary><b>Atributos del Control Record</b> · 6</summary>

`Parameter Type` · `Selected Option` · `Status` · `Type` · `Transaction Type` · `Card Financial Capture Transaction`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Transaction Reversal | 7 |
| Transaction Authorization | 7 |
| Transaction Consolidation | 7 |
| Transaction Capture | 7 |

**Interfaz.** Action Terms: `Exchange` · `Execute` · `Control` · `Initiate` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 22 | 12 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Exchange` · `Execute` · `Control` · `Initiate` · `Request` · `Retrieve` · `Update` |
| BQ `Transaction Consolidation` | `Exchange` · `Control` · `Execute` · `Initiate` · `Retrieve` · `Update` |
| BQ `Transaction Authorization` | `Initiate` · `Retrieve` · `Update` |
| BQ `Transaction Capture` | `Initiate` · `Retrieve` · `Update` |
| BQ `Transaction Reversal` | `Initiate` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Merchant Relations

| | |
|---|---|
| **Patrón funcional** | `Agree Terms` |
| **Tipo de activo** | `Merchant Relationship` |
| **Artefacto genérico** | `Agreement` |
| **Control Record** | `Merchant Relationship Agreement` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Cards |

**Propósito.** This service domain maintains the terms and conditions agreed with merchants for cards related activity

<details><summary><b>Atributos del Control Record</b> · 19</summary>

`Parameter Type` · `Selected Option` · `Type` · `Reference` · `Discharge Request` · `Discharge Schedule` · `Status` · `Associated Party` · `Customer Reference` · `Obligation` · `Entitlement` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Account Reference` · `Subject Matter` · `Product Reference` · `Calendar Reference` · `Associated Agreement Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Regulatory Term | 9 |
| Legal Term | 9 |
| Operational Term | 14 |

**Interfaz.** Action Terms: `Request` · `Notify` · `Retrieve` · `Update` · `Exchange` · `Evaluate` · `Control` · `Grant`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 26 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Request` · `Exchange` · `Control` · `Notify` · `Retrieve` · `Update` · `Evaluate` · `Grant` |
| BQ `Operational Term` | `Notify` · `Retrieve` · `Evaluate` · `Exchange` · `Request` · `Update` |
| BQ `Regulatory Term` | `Update` · `Evaluate` · `Retrieve` · `Exchange` · `Notify` · `Request` |
| BQ `Legal Term` | `Evaluate` · `Request` · `Retrieve` · `Exchange` · `Notify` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Merchant Acquiring Facility

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Merchant Acquiring` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Merchant Acquiring Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Cards |

**Propósito.** This service domain orchestrates the activities related to Merchant fulfillment, Merchant Account maintenance, Merchant transactional activities and settlement, including the billing of merchant fees and charges.

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Product Instance Reference` · `Customer Reference` · `Party Reference` · `Bank Branch/Location Reference` · `Account Currency` · `Tax Reference` · `Operational Terms` · `Limit Type` · `Limit Value` · `Limit Settings`

</details>

**Behavior Qualifiers** · 5

| Behavior Qualifier | Atributos |
|---|---:|
| Support Facility | 5 |
| Clearing | 18 |
| Chargeback | 19 |
| Settlement | 5 |
| Charge | 18 |

**Interfaz.** Action Terms: `Update` · `Initiate` · `Control` · `Request` · `Retrieve` · `Execute` · `Exchange`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 19 | 12 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Update` · `Initiate` · `Control` · `Request` · `Retrieve` |
| BQ `Support Facility` | `Retrieve` |
| BQ `Clearing` | `Execute` · `Update` · `Retrieve` |
| BQ `Charge` | `Update` · `Exchange` · `Retrieve` · `Execute` |
| BQ `Chargeback` | `Execute` · `Update` · `Retrieve` |
| BQ `Settlement` | `Update` · `Retrieve` · `Execute` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Card Network Participant Facility

| | |
|---|---|
| **Patrón funcional** | `Agree Terms` |
| **Tipo de activo** | `Card Network Participant` |
| **Artefacto genérico** | `Agreement` |
| **Control Record** | `Card Network Participant Agreement` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Cards |

**Propósito.** This service domain orchestrates the activities related to the inclusion of new Acquirers and Issuers in the Card Network, their terms and conditions and their status

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Product and Service Reference` · `Customer Reference` · `Party Reference` · `Facility Terms` · `Participant Acquirer Bank Reference` · `Participant Acquirer Bank Clearing and Settlement Terms` · `Participant Acquirer Bank Service Schedule` · `Participant Issuer Bank Reference` · `Participant Issuer Bank Clearing and Settlement Terms` · `Participant Issuer Bank Service Schedule`

</details>

**Interfaz.** Action Terms: `Initiate` · `Update` · `Retrieve` · `Control`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 4 | 2 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Retrieve` · `Control` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Card Transaction Tracking

| | |
|---|---|
| **Patrón funcional** | `Track` |
| **Tipo de activo** | `Credit Card Position` |
| **Artefacto genérico** | `Log` |
| **Control Record** | `Credit Card Position Log` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Cards |

**Propósito.** Maintain a log of credit card bookings and authorizations for operational and management information, tracking and reconciliation purposes

<details><summary><b>Atributos del Control Record</b> · 14</summary>

`Parameter Type` · `Selected Option` · `Type` · `Schedule` · `Usage Log` · `Update Log` · `Associated Party` · `Business Unit Reference` · `Customer Reference` · `Service Configuration` · `Position` · `Position Type` · `Position Limit Time` · `Reference`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Card Transaction Event | 7 |

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Corporate Card Service

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Corporate Card` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Corporate Card Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Cards |

[↑ Índice](README.md)

---

## Mutual Fund Administration

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Mutual Fund` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Mutual Fund Administrative Plan` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Market Operations |

**Propósito.** The Mutual Fund Administration Service Domain handles all aspects of the set-up and operation of mutual funds that can be offered to the bank's general (non-accredited) customers

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Budget Type` · `Budget` · `Assignment` · `Duty` · `Associated Party` · `Budget Balance` · `Subject Matter` · `Type` · `Reference` · `Description`

</details>

**Behavior Qualifiers** · 8

| Behavior Qualifier | Atributos |
|---|---:|
| Fund Management Fee | 8 |
| Fund Investor, Middle and Back Office Service | 8 |
| Fund Development | 8 |
| Fund Inflows and Outflow | 8 |
| Fund Financial Reporting | 8 |
| Fund Enrolment | 8 |
| Fund Accounting | 8 |
| Fund Tax Administration | 8 |

**Interfaz.** Action Terms: `Control` · `Create` · `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 56 | 29 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Create` · `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Fund Accounting` | `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Fund Development` | `Exchange` · `Grant` · `Notify` · `Request` · `Update` · `Retrieve` |
| BQ `Fund Enrolment` | `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Fund Financial Reporting` | `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Fund Inflows and Outflow` | `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Fund Investor, Middle and Back Office Service` | `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Fund Management Fee` | `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Fund Tax Administration` | `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Hedge Fund Administration

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Hedge Fund` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Hedge Fund Administrative Plan` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Market Operations |

**Propósito.** The Hedge Fund Administration Service Domain handles all aspects of the set-up and operation of a hedge fund

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Budget Type` · `Budget` · `Assignment` · `Duty` · `Associated Party` · `Budget Balance` · `Subject Matter` · `Type` · `Reference` · `Description`

</details>

**Behavior Qualifiers** · 9

| Behavior Qualifier | Atributos |
|---|---:|
| Fund Investor, Middle and Back Office Service | 8 |
| Fund Inflows and Outflow | 8 |
| Fund Financial Reporting | 8 |
| Fund Development | 8 |
| Fund Tax Administration | 8 |
| Fund Enrolment Certification | 8 |
| Fund Accounting | 8 |
| Fund Performance Fee | 8 |
| Fund Management | 8 |

**Interfaz.** Action Terms: `Create` · `Exchange` · `Notify` · `Control` · `Grant` · `Request` · `Update` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 62 | 32 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Create` · `Exchange` · `Notify` · `Control` · `Grant` · `Request` · `Update` · `Retrieve` |
| BQ `Fund Accounting` | `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Fund Enrolment Certification` | `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Fund Development` | `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Fund Investor, Middle and Back Office Service` | `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Fund Inflows and Outflow` | `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Fund Financial Reporting` | `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Fund Management` | `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Fund Performance Fee` | `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Fund Tax Administration` | `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Unit Trust Administration

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Unit Trust` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Unit Trust Administrative Plan` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Market Operations |

**Propósito.** This Service Domain handles the implementation and fulfillment of unit investment trusts

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Budget Type` · `Budget` · `Assignment` · `Duty` · `Associated Party` · `Budget Balance` · `Subject Matter` · `Type` · `Reference` · `Description`

</details>

**Behavior Qualifiers** · 6

| Behavior Qualifier | Atributos |
|---|---:|
| Fund Financial Reporting | 8 |
| Fund Investor, Middle and Back Office Service | 8 |
| Fund Enrolment | 8 |
| Fund Tax Administration | 8 |
| Fund Accounting | 8 |
| Fund Management Fee | 8 |

**Interfaz.** Action Terms: `Control` · `Create` · `Notify` · `Request` · `Exchange` · `Grant` · `Update` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 44 | 23 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Create` · `Notify` · `Request` · `Exchange` · `Grant` · `Update` · `Retrieve` |
| BQ `Fund Accounting` | `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Fund Investor, Middle and Back Office Service` | `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Fund Enrolment` | `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Fund Financial Reporting` | `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Fund Management Fee` | `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Fund Tax Administration` | `Exchange` · `Grant` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Trade Confirmation Matching

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `Trade Matching` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `Trade Matching Operating Session` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Market Operations |

**Propósito.** This Service Domain supports the bank's interface to a central market matching and confirmation service whether the bank acts as broker dealer or institutional investor

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Schedule` · `Status` · `Usage Log` · `Associated Party Reference` · `Service Provider Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Service Configuration` · `Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Unmatched Market Trade Escalation | 6 |
| Transaction Confirmation/Affirmation | 6 |
| Transaction Reporting | 6 |

**Interfaz.** Action Terms: `Exchange` · `Control` · `Execute` · `Initiate` · `Notify` · `Request` · `Update` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 29 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Exchange` · `Control` · `Execute` · `Initiate` · `Notify` · `Request` · `Update` · `Retrieve` |
| BQ `Transaction Confirmation/Affirmation` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Unmatched Market Trade Escalation` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Transaction Reporting` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Order Allocation

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Securities Allocation` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Securities Allocation Procedure` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Market Operations |

**Propósito.** This Service Domain allocates partially fulfilled market trades

<details><summary><b>Atributos del Control Record</b> · 21</summary>

`Parameter Type` · `Selected Option` · `Request` · `Schedule` · `Status` · `Associated Party Reference` · `Business Unit Reference` · `Service Provider Reference` · `Financial Facility Reference` · `Employee Reference` · `Customer Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Product and Service Type` · `Product and Service Instance` · `Transaction Type` · `Transaction` · `Financial Transaction Arrangement` · `Customer Agreement Reference` · `Reference`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Update (Partially Completed) Market Order | 8 |
| Apply Order Allocation Rules | 8 |

**Interfaz.** Action Terms: `Exchange` · `Control` · `Initiate` · `Execute` · `Request` · `Notify` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 22 | 11 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Exchange` · `Control` · `Initiate` · `Execute` · `Request` · `Notify` · `Retrieve` · `Update` |
| BQ `Apply Order Allocation Rules` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Update (Partially Completed) Market Order` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Securities Fails Processing

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Security Trading Fails` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Security Trading Fails Procedure` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Market Operations |

**Propósito.** This Service Domain handles the resolution of clerical and processing errors that lead to failures in the securities trade clearing and settlement processes

<details><summary><b>Atributos del Control Record</b> · 21</summary>

`Parameter Type` · `Selected Option` · `Request` · `Schedule` · `Status` · `Associated Party Reference` · `Business Unit Reference` · `Service Provider Reference` · `Financial Facility Reference` · `Employee Reference` · `Customer Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Product and Service Type` · `Product and Service Instance` · `Transaction Type` · `Transaction` · `Financial Transaction Arrangement` · `Customer Agreement Reference` · `Reference`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Securities Fail Determination | 8 |
| Securities Fail Analysis | 8 |

**Interfaz.** Action Terms: `Control` · `Execute` · `Exchange` · `Initiate` · `Request` · `Notify` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 22 | 11 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Execute` · `Exchange` · `Initiate` · `Request` · `Notify` · `Retrieve` · `Update` |
| BQ `Securities Fail Analysis` | `Exchange` · `Execute` · `Request` · `Initiate` · `Notify` · `Retrieve` · `Update` |
| BQ `Securities Fail Determination` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Retrieve` · `Request` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Trade and Price Reporting

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `Market Trade Reporting` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `Market Trade Reporting Operating Session` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Market Operations |

**Propósito.** This Service Domain operates an automated facility that reports executed market trades to the market place as required by the rules of market participation

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Schedule` · `Status` · `Usage Log` · `Associated Party Reference` · `Service Provider Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Service Configuration` · `Reference`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Transaction Reporting | 6 |

**Interfaz.** Action Terms: `Exchange` · `Control` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 15 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Exchange` · `Control` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Transaction Reporting` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Custody Administration

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Custody` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Custody Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Market Operations |

**Propósito.** A service to provide safe custody services for marketable securities for bank customers

<details><summary><b>Atributos del Control Record</b> · 13</summary>

`Parameter Type` · `Selected Option` · `Type` · `Reference` · `Schedule` · `Status` · `Currency` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Booking Location` · `Account Type` · `Account Reference`

</details>

**Behavior Qualifiers** · 5

| Behavior Qualifier | Atributos |
|---|---:|
| Dividend | 7 |
| Regulatory Submission | 7 |
| Charge | 7 |
| Safe Keeping | 7 |
| Settlement | 7 |

**Interfaz.** Action Terms: `Retrieve` · `Request` · `Initiate` · `Execute` · `Control` · `Exchange` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 26 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Retrieve` · `Request` · `Initiate` · `Control` · `Exchange` · `Execute` · `Update` |
| BQ `Settlement` | `Execute` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Dividend` | `Initiate` · `Retrieve` |
| BQ `Safe Keeping` | `Control` · `Retrieve` · `Request` · `Update` |
| BQ `Charge` | `Initiate` · `Exchange` · `Retrieve` · `Update` |
| BQ `Regulatory Submission` | `Execute` · `Initiate` · `Retrieve` · `Request` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Corporate Action

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Corporate Action` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Corporate Action Procedure` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Market Operations |

**Propósito.** This Service Domain supports the various custodial tasks associated with processing associated corporate actions

<details><summary><b>Atributos del Control Record</b> · 25</summary>

`Parameter Type` · `Selected Option` · `Request` · `Schedule` · `Status` · `Associated Party Reference` · `Business Unit Reference` · `Service Provider Reference` · `Financial Facility Reference` · `Employee Reference` · `Customer Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Product and Service Type` · `Product and Service Instance` · `Transaction Type` · `Transaction` · `Financial Transaction Arrangement` · `Customer Agreement Reference` · `Reference` · `Corporate Action Reference` · `Corporate Action Arrangement Reference` · `Corporate Action Involved Party Reference` · `Corporate Action Involvement Type`

</details>

**Behavior Qualifiers** · 5

| Behavior Qualifier | Atributos |
|---|---:|
| Security Spin-Off Action | 8 |
| Security Rights Issue Action | 8 |
| Security Mergers and Acquisition Action | 8 |
| Security Dividend Payment | 8 |
| Stock Split or Reversal Action | 8 |

**Interfaz.** Action Terms: `Control` · `Initiate` · `Execute` · `Exchange` · `Notify` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 43 | 17 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Initiate` · `Execute` · `Exchange` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Security Mergers and Acquisition Action` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Security Dividend Payment` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Security Rights Issue Action` | `Execute` · `Exchange` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Security Spin-Off Action` | `Execute` · `Exchange` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Stock Split or Reversal Action` | `Execute` · `Exchange` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Financial Instrument Valuation

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Market Asset Valuation` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Market Asset Valuation Procedure` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Market Operations |

**Propósito.** This Service Domain provides a range of financial asset valuation services

<details><summary><b>Atributos del Control Record</b> · 21</summary>

`Parameter Type` · `Selected Option` · `Request` · `Schedule` · `Status` · `Associated Party Reference` · `Business Unit Reference` · `Service Provider Reference` · `Financial Facility Reference` · `Employee Reference` · `Customer Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Product and Service Type` · `Product and Service Instance` · `Transaction Type` · `Transaction` · `Financial Transaction Arrangement` · `Customer Agreement Reference` · `Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Asset Valuation | 8 |
| Asset Valuation Approach Selection | 8 |
| Asset Valuation Information Consolidation | 8 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 29 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Asset Valuation Approach Selection` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Asset Valuation Information Consolidation` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Asset Valuation` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Trade Clearing

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Trade Clearing` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Trade Clearing Procedure` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Market Operations |

**Propósito.** This Service Domain handles the back office processes that confirm and notify interested parties that securities and funds are available as traded in anticipation of settlement processing

<details><summary><b>Atributos del Control Record</b> · 21</summary>

`Parameter Type` · `Selected Option` · `Request` · `Schedule` · `Status` · `Associated Party Reference` · `Business Unit Reference` · `Service Provider Reference` · `Financial Facility Reference` · `Employee Reference` · `Customer Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Product and Service Type` · `Product and Service Instance` · `Transaction Type` · `Transaction` · `Financial Transaction Arrangement` · `Customer Agreement Reference` · `Reference`

</details>

**Behavior Qualifiers** · 5

| Behavior Qualifier | Atributos |
|---|---:|
| Market Trade Settlement Initiation | 8 |
| Market Trade Funds and Security Availability Assurance | 8 |
| Market Trade Out Trade Resolution | 8 |
| Market Trade Confirmation | 8 |
| Market Trade Matching | 8 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Update` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 43 | 20 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Update` · `Retrieve` |
| BQ `Market Trade Confirmation` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Market Trade Funds and Security Availability Assurance` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Market Trade Matching` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Market Trade Out Trade Resolution` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Market Trade Settlement Initiation` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Trade Settlement

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Trade Settlement` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Trade Settlement Procedure` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Market Operations |

**Propósito.** This Service Domain handles the final movement of cash and securities between depositories as previously confirmed in the clearing process, in order to settle a market trade

<details><summary><b>Atributos del Control Record</b> · 21</summary>

`Parameter Type` · `Selected Option` · `Request` · `Schedule` · `Status` · `Associated Party Reference` · `Business Unit Reference` · `Service Provider Reference` · `Financial Facility Reference` · `Employee Reference` · `Customer Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Product and Service Type` · `Product and Service Instance` · `Transaction Type` · `Transaction` · `Financial Transaction Arrangement` · `Customer Agreement Reference` · `Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Market Trade Securities Settlement | 8 |
| Market Trade Settlement Confirmation | 8 |
| Market Trade Cash Settlement | 8 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 29 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Market Trade Cash Settlement` | `Exchange` · `Notify` · `Initiate` · `Execute` · `Request` · `Retrieve` · `Update` |
| BQ `Market Trade Settlement Confirmation` | `Initiate` · `Execute` · `Exchange` · `Notify` · `Request` · `Update` · `Retrieve` |
| BQ `Market Trade Securities Settlement` | `Execute` · `Initiate` · `Notify` · `Exchange` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Public Offering

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Public Offering` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Public Offering Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Corporate Financing and Advisory Services |

**Propósito.** This Service Domain supports a broad range of complex financial, accounting and regulatory actions involved in providing advice and practical support to companies going public and/or raising additional capital through the issuance of publicly traded securities

<details><summary><b>Atributos del Control Record</b> · 18</summary>

`Parameter Type` · `Selected Option` · `Type` · `Calendar Reference` · `Status` · `Associated Party` · `Currency` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Booking Location` · `Account Type` · `Account Reference` · `Customer Reference` · `Position` · `Product Reference` · `Position Limit` · `Reference`

</details>

**Behavior Qualifiers** · 6

| Behavior Qualifier | Atributos |
|---|---:|
| Underwriting | 7 |
| Prospectus | 7 |
| Placement | 7 |
| Compliance | 7 |
| Instrument Design | 7 |
| Item Registration | 7 |

**Interfaz.** Action Terms: `Control` · `Initiate` · `Execute` · `Notify` · `Exchange` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 50 | 23 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Initiate` · `Execute` · `Notify` · `Exchange` · `Request` · `Retrieve` · `Update` |
| BQ `Compliance` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Item Registration` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Underwriting` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Instrument Design` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Prospectus` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Placement` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Private Placement

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Private Placement` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Private Placement Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Corporate Financing and Advisory Services |

**Propósito.** This Service Domain provides the complete range of functions involved in providing private placement services to corporate customers.

<details><summary><b>Atributos del Control Record</b> · 18</summary>

`Parameter Type` · `Selected Option` · `Type` · `Calendar Reference` · `Status` · `Associated Party` · `Currency` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Booking Location` · `Account Type` · `Account Reference` · `Customer Reference` · `Position` · `Product Reference` · `Position Limit` · `Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Maintenance | 7 |
| Placement | 7 |
| Instrument Design | 7 |

**Interfaz.** Action Terms: `Exchange` · `Execute` · `Control` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 29 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Exchange` · `Execute` · `Control` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Placement` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Maintenance` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Instrument Design` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Mergers and Acquisitions Advisory

| | |
|---|---|
| **Patrón funcional** | `Advise` |
| **Tipo de activo** | `Mergers And Acquisition` |
| **Artefacto genérico** | `Advice` |
| **Control Record** | `Mergers And Acquisition Advice` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Corporate Financing and Advisory Services |

**Propósito.** This Service Domain handles mergers and acquisition, IPO, MBO and LBO projects with the bank acting in the lead and/or subordinate role

<details><summary><b>Atributos del Control Record</b> · 8</summary>

`Subject Area Type` · `Parameter Type` · `Selected Option` · `Request` · `Usage Log` · `Feedback` · `Type` · `Reference`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Merger and Acquisition | 8 |

**Interfaz.** Action Terms: `Exchange` · `Initiate` · `Notify` · `Request` · `Update` · `Control` · `Execute` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 15 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| BQ `Merger and Acquisition` | `Exchange` · `Execute` · `Initiate` · `Request` · `Notify` · `Retrieve` · `Update` |
| **Control Record** | `Exchange` · `Initiate` · `Notify` · `Request` · `Update` · `Control` · `Execute` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Corporate Tax Advisory

| | |
|---|---|
| **Patrón funcional** | `Advise` |
| **Tipo de activo** | `Corporate Tax Advice` |
| **Artefacto genérico** | `Advice` |
| **Control Record** | `Corporate Tax Advice` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Corporate Financing and Advisory Services |

**Propósito.** A fee or commission based product providing tax specific assessments, advice and guidance for corporate customers

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Product Instance Reference` · `Customer Reference` · `Bank Branch/Location Reference` · `Employee/Business Unit Reference` · `Corporate Tax Advisory Work Products` · `Document Directory Entry Instance Reference` · `Session Schedule` · `Consolidation Record` · `Date Type` · `Date`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Taxation | 6 |
| Charge | 5 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Request` · `Retrieve` · `Control` · `Exchange` · `Execute`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 14 | 6 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Request` · `Retrieve` · `Control` |
| BQ `Taxation` | `Initiate` · `Retrieve` · `Update` · `Request` |
| BQ `Charge` | `Initiate` · `Update` · `Exchange` · `Execute` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Corporate Finance

| | |
|---|---|
| **Patrón funcional** | `Advise` |
| **Tipo de activo** | `Corporate Finance Services` |
| **Artefacto genérico** | `Advice` |
| **Control Record** | `Corporate Finance Services Advice` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Corporate Financing and Advisory Services |

**Propósito.** This Service Domain handles the provision of a broad range of financial advisory services to corporate clients

<details><summary><b>Atributos del Control Record</b> · 9</summary>

`Subject Area Type` · `Parameter Type` · `Selected Option` · `Request` · `Usage Log` · `Feedback` · `Type` · `Reference` · `Arrangement Reference`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Strategic Funding | 8 |
| Tactical Funding | 8 |
| Taxation | 8 |
| Capital Structuring | 8 |

**Interfaz.** Action Terms: `Exchange` · `Execute` · `Initiate` · `Update` · `Control` · `Request` · `Notify` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 36 | 17 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Exchange` · `Initiate` · `Update` · `Control` · `Request` · `Execute` · `Notify` · `Retrieve` |
| BQ `Strategic Funding` | `Exchange` · `Initiate` · `Execute` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Taxation` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Capital Structuring` | `Execute` · `Exchange` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Tactical Funding` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Corporate Trust Services

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Corporate Trust Services` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Corporate Trust Services Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Consumer Services |

**Propósito.** This Service Domain provides corporate trust services centered on the handling of debt instruments and escrow account support

<details><summary><b>Atributos del Control Record</b> · 18</summary>

`Parameter Type` · `Selected Option` · `Type` · `Calendar Reference` · `Status` · `Associated Party` · `Currency` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Booking Location` · `Account Type` · `Account Reference` · `Customer Reference` · `Position` · `Product Reference` · `Position Limit` · `Reference`

</details>

**Behavior Qualifiers** · 5

| Behavior Qualifier | Atributos |
|---|---:|
| Escrow | 7 |
| Financing | 7 |
| Project Finance | 7 |
| Court Liaison | 7 |
| Loan Agency and Administration | 7 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 43 | 20 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Project Finance` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Escrow` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Court Liaison` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Retrieve` · `Request` · `Update` |
| BQ `Financing` | `Execute` · `Exchange` · `Initiate` · `Notify` · `Retrieve` · `Request` · `Update` |
| BQ `Loan Agency and Administration` | `Exchange` · `Execute` · `Notify` · `Initiate` · `Retrieve` · `Update` · `Request` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Currency Exchange

| | |
|---|---|
| **Patrón funcional** | `Transact` |
| **Tipo de activo** | `Currency Exchange` |
| **Artefacto genérico** | `Transaction` |
| **Control Record** | `Currency Exchange Transaction` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Consumer Services |

**Propósito.** Service Domain supports over the counter currency exchange

<details><summary><b>Atributos del Control Record</b> · 6</summary>

`Parameter Type` · `Selected Option` · `Status` · `Type` · `Transaction Type` · `Transaction`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Quote | 7 |
| Document Handling | 7 |
| FX Transaction Capture | 7 |

**Interfaz.** Action Terms: `Execute` · `Initiate` · `Control` · `Exchange` · `Retrieve` · `Request` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 18 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Execute` · `Initiate` · `Control` · `Exchange` · `Retrieve` · `Request` · `Update` |
| BQ `FX Transaction Capture` | `Exchange` · `Retrieve` · `Initiate` · `Update` |
| BQ `Document Handling` | `Execute` · `Initiate` · `Retrieve` · `Update` |
| BQ `Quote` | `Initiate` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Bank Drafts

| | |
|---|---|
| **Patrón funcional** | `Transact` |
| **Tipo de activo** | `Bearer Document` |
| **Artefacto genérico** | `Transaction` |
| **Control Record** | `Bearer Document Transaction` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Consumer Services |

**Propósito.** This Service Domain support bank guaranteed payment transactions such as bank drafts

<details><summary><b>Atributos del Control Record</b> · 8</summary>

`Parameter Type` · `Selected Option` · `Status` · `Type` · `Reference` · `Bearer Document Reference` · `Bearer Document Instruction Reference` · `Bearer Document Involved Party Reference`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Bank Guaranteed Payment Remittance | 7 |
| Bearer Document Creation and Registration | 7 |
| Customer Payment | 7 |
| Bank Guaranteed Payment Specification | 7 |

**Interfaz.** Action Terms: `Exchange` · `Control` · `Execute` · `Retrieve` · `Initiate` · `Notify` · `Update` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 36 | 17 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Exchange` · `Control` · `Execute` · `Retrieve` · `Initiate` · `Notify` · `Update` · `Request` |
| BQ `Bank Guaranteed Payment Remittance` | `Exchange` · `Execute` · `Initiate` · `Request` · `Notify` · `Update` · `Retrieve` |
| BQ `Customer Payment` | `Exchange` · `Execute` · `Notify` · `Initiate` · `Request` · `Retrieve` · `Update` |
| BQ `Bearer Document Creation and Registration` | `Execute` · `Exchange` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Bank Guaranteed Payment Specification` | `Initiate` · `Exchange` · `Execute` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Brokered Product Proxy

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Brokered Product` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Brokered Product Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Consumer Services |

**Propósito.** This Service Domain oversees all activities associated with the coordinated delivery of 3rd party products and services

<details><summary><b>Atributos del Control Record</b> · 6</summary>

`Consent Reference` · `Active Access Token Reference` · `Reference` · `Service Provider Reference` · `Service User Reference` · `Third Party Provider Reference`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Service Access | 2 |

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Consumer Investments

| | |
|---|---|
| **Patrón funcional** | `Transact` |
| **Tipo de activo** | `Consumer Securities Order` |
| **Artefacto genérico** | `Transaction` |
| **Control Record** | `Consumer Securities Order Transaction` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Consumer Services |

**Propósito.** Handle the consumer front-end trading requests. These will typically be blocked/netted for market execution

<details><summary><b>Atributos del Control Record</b> · 15</summary>

`Consumer Securities Order Instruction Type` · `Customer Reference` · `Employee or Business Unit Reference` · `Investment Portfolio Instance Reference` · `Consumer Securities Order Processing Instruction` · `Document Directory Entry Instance Reference` · `Correspondence Instance Reference` · `Consumer Securities Order Transaction` · `Investment Account Arrangement Instance Reference` · `Current Account Arrangement Instance Reference` · `Market Order Type` · `Security Type` · `Amount` · `Date Type` · `Date`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Quote | 1 |
| Compliance | 3 |
| Confirmation | 1 |
| Order Initiation | 3 |

**Interfaz.** Action Terms: `Retrieve` · `Initiate` · `Update` · `Exchange`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 8 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| BQ `Quote` | `Retrieve` |
| **Control Record** | `Initiate` · `Update` · `Retrieve` |
| BQ `Confirmation` | `Retrieve` |
| BQ `Compliance` | `Retrieve` |
| BQ `Order Initiation` | `Exchange` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Customer Tax Handling

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Customer Tax Obligation` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Customer Tax Obligation Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Consumer Services |

**Propósito.** This service domain handles consumer tax reporting obligations

<details><summary><b>Atributos del Control Record</b> · 6</summary>

`Customer Reference` · `Customer Tax Handling Arrangement Record` · `Taxation Jurisdiction Reference` · `Applicable Taxation Rule Reference` · `Applicable Taxation Rule Definition` · `Customer Tax Reporting Schedule`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Consolidation | 8 |
| Analysis | 1 |
| Reporting | 5 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Execute` · `Request` · `Retrieve` · `Exchange`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 14 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Execute` · `Request` · `Retrieve` |
| BQ `Consolidation` | `Update` · `Retrieve` |
| BQ `Analysis` | `Exchange` · `Update` · `Retrieve` |
| BQ `Reporting` | `Update` · `Exchange` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Consumer Advisory Services

| | |
|---|---|
| **Patrón funcional** | `Advise` |
| **Tipo de activo** | `Consumer Advice` |
| **Artefacto genérico** | `Advice` |
| **Control Record** | `Consumer Advice` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Consumer Services |

**Propósito.** Offer financial advisory services to consumer customers, possibly for a fee

<details><summary><b>Atributos del Control Record</b> · 12</summary>

`Product Instance Reference` · `Customer Reference` · `Bank Branch/Location Reference` · `Employee or Business Unit Reference` · `Work Products` · `Document Directory Entry Instance Reference` · `Session Schedule` · `Profile` · `Advice Type` · `Consolidation Record` · `Date Type` · `Date`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Financial Planning | 2 |
| Taxation | 2 |
| Product Guidance | 6 |
| Charge | 5 |

**Interfaz.** Action Terms: `Update` · `Initiate` · `Control` · `Request` · `Retrieve` · `Exchange` · `Execute`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 19 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Update` · `Initiate` · `Control` · `Request` · `Retrieve` |
| BQ `Financial Planning` | `Initiate` · `Update` · `Retrieve` |
| BQ `Taxation` | `Initiate` · `Update` · `Retrieve` |
| BQ `Product Guidance` | `Initiate` · `Retrieve` · `Update` |
| BQ `Charge` | `Retrieve` · `Initiate` · `Update` · `Exchange` · `Execute` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Trust Services

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Trust Services` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Corporate Trust Services Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Consumer Services |

**Propósito.** This Service Domain support a range of trust management services offered to high value customers

<details><summary><b>Atributos del Control Record</b> · 18</summary>

`Parameter Type` · `Selected Option` · `Type` · `Calendar Reference` · `Status` · `Associated Party` · `Currency` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Booking Location` · `Account Type` · `Account Reference` · `Customer Reference` · `Position` · `Product Reference` · `Position Limit` · `Reference`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Court Liaison | 7 |
| Loan Agency and Administration | 7 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Update` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 22 | 11 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Update` · `Request` · `Retrieve` |
| BQ `Court Liaison` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Loan Agency and Administration` | `Exchange` · `Execute` · `Notify` · `Initiate` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Funeral Policy

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Funeral Policy` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Funeral Policy Facility` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Consumer Services |

**Propósito.** The Funeral Policy Service Domain handles the general product maintenance, premium payments and initiates claims processing

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Instance Record Identification` · `Funeral Policy Number` · `Policy Holder Reference` · `Insured Persons Reference` · `Beneficiary or Nominee Reference` · `Policy Coverage Type` · `Policy Term` · `Policy Effective Date` · `Policy Status` · `Governing Law or Jurisdiction`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Administration | 8 |
| Billing | 12 |
| Claim Initiation | 8 |

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Claim Assessment

| | |
|---|---|
| **Patrón funcional** | `Assess` |
| **Tipo de activo** | `Claim Validation` |
| **Artefacto genérico** | `Assessment` |
| **Control Record** | `Claim Validation Assessment` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Consumer Services |

**Propósito.** The Claim Assessment Service Domain runs through the required tests to confirm the veracity of a claim made under an insurance policy

<details><summary><b>Atributos del Control Record</b> · 19</summary>

`Claim Assessment Type` · `Instance Record Identification` · `Claim Assessment Request` · `Claim Assessment Schedule` · `Claim Assessment Status` · `Claim Assessment Usage Log Reference` · `Claim Assessment Requester Reference` · `Claim Assessment Associated Party Reference` · `Claim Assessment Service Provider Reference` · `Claim Identification` · `Claim Type` · `Claim Date` · `Policy Reference` · `Policyholder Reference` · `Claim Assessment Assessor Reference` · `Insured Event Reference` · `Claim Assessment Complemented Date` · `Claim Assessment Supporting Document Reference` · `Claim Assessment Result`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Eligibility Check | 9 |
| Entitlement Check | 9 |
| External Agency Evaluation | 9 |
| Authentication | 9 |

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Claim Administration

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Claim Processing` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Claim Processing Administrative Plan` |
| **Ubicación Matrix** | Operations and Execution › Product Specific Fulfillment › Consumer Services |

**Propósito.** The claim administration Service Domain implements the payment and support obligations of the policy in respect to a verified claim

<details><summary><b>Atributos del Control Record</b> · 14</summary>

`Claim Administration Identification` · `Claim Reference` · `Policy Reference` · `Product Type` · `Claimant Reference` · `Beneficiary or Payee Reference` · `Service Provider Reference` · `Internal Actor Reference` · `Claim Administration Status` · `Claim Stage` · `Start Date` · `Last Updated Date` · `SLA or Processing Timeline` · `Instance Record Identification`

</details>

**Behavior Qualifiers** · 5

| Behavior Qualifier | Atributos |
|---|---:|
| Administration | 12 |
| Documentation | 11 |
| Negotiation | 13 |
| Communication | 12 |
| Disbursement | 13 |

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Financial Message Analysis

| | |
|---|---|
| **Patrón funcional** | `Analyze` |
| **Tipo de activo** | `Financial Network Gateway` |
| **Artefacto genérico** | `Analysis` |
| **Control Record** | `Financial Network Gateway Analysis` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Payments |

[↑ Índice](README.md)

---

## Financial Gateway

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `Financial Gateway` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `Financial Gateway Operating Session` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Payments |

**Propósito.** This service domain operates automated message interfaces to secure networks such as SWIFT, TELEX, ACH and Financial Market reporting services

<details><summary><b>Atributos del Control Record</b> · 14</summary>

`Financial Gateway Service Type` · `Financial Gateway Service Session Statistics` · `Financial Gateway Service Session Report Type` · `Financial Gateway Service Session Report` · `Financial Gateway Service Session Date` · `Financial Gateway Service Session Issue Record` · `Employee or Business Unit Reference` · `Message Reference` · `Production Issue Type` · `Production Issue Description` · `Production Issue Diagnosis` · `Production Issue Resolution Task` · `Production Issue Record` · `Production Issue Status`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Inbound | 4 |
| Outbound | 5 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 9 | 6 |

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

## Central Cash Handling

| | |
|---|---|
| **Patrón funcional** | `Allocate` |
| **Tipo de activo** | `Central Cash` |
| **Artefacto genérico** | `Allocation` |
| **Control Record** | `Central Cash Allocation` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Payments |

**Propósito.** Track cash inventory, project demand and allocate inventory across the branch/ATM network

<details><summary><b>Atributos del Control Record</b> · 17</summary>

`Parameter Type` · `Selected Option` · `<Subject Area> Type` · `Description` · `Request` · `Schedule` · `Status` · `Reference` · `Customer Reference` · `Currency` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Booking Location` · `Account Type` · `Account Reference` · `Instance`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Projection and Allocation | 3 |
| Tracking and Allocation | 3 |

**Interfaz.** Action Terms: `Capture` · `Control` · `Exchange` · `Initiate` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 18 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Capture` · `Control` · `Exchange` · `Initiate` · `Retrieve` · `Update` |
| BQ `Projection and Allocation` | `Capture` · `Initiate` · `Control` · `Exchange` · `Update` · `Retrieve` |
| BQ `Tracking and Allocation` | `Exchange` · `Capture` · `Control` · `Initiate` · `Update` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Card Financial Settlement

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Card Financial Settlement` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Card Financial Settlement Procedure` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Payments |

**Propósito.** This service domain orchestrates the settlement of the transactions between the Issuers and the Acquirers through the Card Networks

<details><summary><b>Atributos del Control Record</b> · 6</summary>

`Network Reference` · `Card Financial Settlement Process Type` · `Card Financial Settlement Process Date and Time` · `Card Financial Settlement Service Schedule` · `Participant Acquirer Bank Reference` · `Participant Issuer Bank Reference`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Consolidation | 13 |
| Processing | 2 |
| Instruction | 2 |
| Payment | 0 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Retrieve` · `Control`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 12 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Retrieve` · `Control` |
| BQ `Consolidation` | `Retrieve` · `Update` |
| BQ `Processing` | `Retrieve` · `Update` |
| BQ `Payment` | `Update` · `Retrieve` |
| BQ `Instruction` | `Update` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Card eCommerce Gateway

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `eCommerce Gateway` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `eCommerce Gateway Operating Session` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Payments |

**Propósito.** This service domain orchestrates the processing of e-commerce transactions for authentication, authorization and capture of the financial transactions

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Reference` · `Schedule` · `Status` · `Usage Log` · `Associated Party Reference` · `Service Provider Reference` · `Service Configuration` · `Service Provider Schedule` · `Service Type` · `Type`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Card Payment | 14 |
| Transaction Batch | 3 |
| Card Authentication | 2 |
| Transaction Authorization | 2 |

**Interfaz.** Action Terms: `Control` · `Initiate` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 14 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Retrieve` |
| BQ `Card Payment` | `Initiate` · `Update` · `Retrieve` |
| BQ `Transaction Batch` | `Update` · `Initiate` · `Retrieve` |
| BQ `Card Authentication` | `Retrieve` · `Initiate` · `Update` |
| BQ `Transaction Authorization` | `Update` · `Initiate` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Card Clearing

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Card Clearing` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Card Clearing Procedure` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Payments |

**Propósito.** This service domain orchestrates the capture and consolidation of card financial transactions originating from various sources. It also handles the clearing of the transactions from the Acquirers to the Issuers through the Card Networks

<details><summary><b>Atributos del Control Record</b> · 8</summary>

`Network Reference` · `Participant Acquirer Bank Reference` · `Participant Acquirer Bank Clearing and Settlement Terms` · `Participant Issuer Bank Reference` · `Participant Issuer Bank Clearing and Settlement Terms` · `Card Clearing Process Type` · `Card Clearing Process Date and Time` · `Card Clearing Service Schedule`

</details>

**Behavior Qualifiers** · 7

| Behavior Qualifier | Atributos |
|---|---:|
| Capture | 16 |
| Addressing | 1 |
| FX Conversion | 2 |
| Charge | 2 |
| Matching | 1 |
| Reconciliation | 1 |
| Routing | 1 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Retrieve` · `Execute`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 13 | 16 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Retrieve` |
| BQ `Capture` | `Update` · `Retrieve` |
| BQ `Addressing` | `Retrieve` |
| BQ `FX Conversion` | `Retrieve` |
| BQ `Charge` | `Update` · `Retrieve` · `Execute` |
| BQ `Matching` | `Retrieve` |
| BQ `Reconciliation` | `Retrieve` |
| BQ `Routing` | `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Cheque Processing

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `Cheque Processing` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `Cheque Processing Operating Session` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Payments |

**Propósito.** Handle the processing of paper cheques, generating financial transactions for processing

<details><summary><b>Atributos del Control Record</b> · 9</summary>

`Schedule` · `Status` · `Usage Log` · `Reference` · `Service Provider Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Service Configuration`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Cheque Extraction | 6 |
| Cheque Exception Handling | 6 |
| Financial Transaction Initiation | 6 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Request` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 13 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Financial Transaction Initiation` | `Exchange` · `Retrieve` |
| BQ `Cheque Exception Handling` | `Retrieve` · `Update` · `Initiate` |
| BQ `Cheque Extraction` | `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Payment Rail

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `Payment Rail` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `Payment Rail Operating Session` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Payments |

**Propósito.** This Service Domain handles the operational interface with payment service providers, formatting outbound transactions and onward routing inbound transactions during scheduled operating sessions. It also links to holding account facilities for net payment handling

<details><summary><b>Atributos del Control Record</b> · 10</summary>

`Schedule` · `Status` · `Usage Log` · `Associated Party Reference` · `Service Provider Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Service Configuration` · `Reference`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Payment Clearing and Settlement | 6 |
| Payment Account Reconciliation | 6 |
| Inbound Transaction | 6 |
| Outbound Transaction | 6 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 36 | 17 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Inbound Transaction` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Outbound Transaction` | `Exchange` · `Initiate` · `Execute` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Payment Account Reconciliation` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |
| BQ `Payment Clearing and Settlement` | `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Payment Settlement

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Payment Settlement` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Payment Settlement Procedure` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Payments |

[↑ Índice](README.md)

---

## Payment Confirmation

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Payment Confirmation` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Payment Confirmation Procedure` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Payments |

[↑ Índice](README.md)

---

## Payment Orchestration

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Payment Orchestration` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Payment Orchestration Procedure` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Payments |

[↑ Índice](README.md)

---

## Reward Points Account

| | |
|---|---|
| **Patrón funcional** | `Track` |
| **Tipo de activo** | `Reward Points` |
| **Artefacto genérico** | `Log` |
| **Control Record** | `Reward Points Log` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Account Management |

**Propósito.** Administer the booking and remittance of rewards points

<details><summary><b>Atributos del Control Record</b> · 13</summary>

`Parameter Type` · `Selected Option` · `Type` · `Schedule` · `Usage Log` · `Update Log` · `Reference` · `Business Unit Reference` · `Customer Reference` · `Service Configuration` · `Position` · `Position Type` · `Position Limit Time`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Capture | 7 |
| Expiration | 7 |

**Interfaz.** Action Terms: `Capture` · `Control` · `Exchange` · `Grant` · `Initiate` · `Retrieve` · `Request` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 16 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Capture` · `Control` · `Exchange` · `Grant` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Capture` | `Capture` · `Initiate` · `Retrieve` · `Update` |
| BQ `Expiration` | `Capture` · `Initiate` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Product Combination

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Product Combination` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Product Combination Facility` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Account Management |

**Propósito.** Product Combination supports bundled products applying necessary constraints on embedded product fulfillment and ensuring product performance analysis takes correct account of embedded products' contribution

<details><summary><b>Atributos del Control Record</b> · 13</summary>

`Parameter Type` · `Selected Option` · `Type` · `Reference` · `Schedule` · `Status` · `Currency` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Booking Location` · `Account Type` · `Account Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Support Facility | 7 |
| Transfer Pricing | 7 |
| Fulfillment | 7 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Request` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 21 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Fulfillment` | `Control` · `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Transfer Pricing` | `Exchange` · `Retrieve` · `Request` · `Update` |
| BQ `Support Facility` | `Initiate` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Position Management

| | |
|---|---|
| **Patrón funcional** | `Monitor` |
| **Tipo de activo** | `Financial Position` |
| **Artefacto genérico** | `State` |
| **Control Record** | `Financial Position State` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Account Management |

**Propósito.** The Service Domain tracks the bank's consolidated financial positions for major customers and complex market conditions

<details><summary><b>Atributos del Control Record</b> · 12</summary>

`Position Type` · `Position Customer Reference` · `Position Sector` · `Position Product Type` · `Position Definition` · `Position Thresholds/Limits` · `Position Value` · `Position Notification Arrangement Reference` · `Position Notification Arrangement Record` · `Position Notification Business Unit Reference` · `Position Notification Details` · `Position Notification Record`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Trial Transaction | 7 |
| Transaction Application | 7 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 10 | 6 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Request` |
| BQ `Trial Transaction` | `Initiate` · `Update` · `Retrieve` |
| BQ `Transaction Application` | `Initiate` · `Update` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Position Keeping

| | |
|---|---|
| **Patrón funcional** | `Track` |
| **Tipo de activo** | `Financial Position` |
| **Artefacto genérico** | `Log` |
| **Control Record** | `Financial Position Log` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Account Management |

**Propósito.** This service domain maintains a log of monetary or value transactions and entitlements log posted to product facilities. Reconciled financial transactions are subsequently used for posting to the accounting systems.

<details><summary><b>Atributos del Control Record</b> · 22</summary>

`Transaction Log Type` · `Product Instance Reference` · `Customer Reference` · `Counterparty Reference` · `Base Currency` · `Interest Application Record` · `Interest Transaction` · `Transaction Description` · `Transaction Rate Type` · `Transaction Interest Charge` · `Managed Position Limits` · `Position Limit Type` · `Position Limit Settings` · `Position Limit Value` · `Amount Block` · `Amount Block Type` · `Priority` · `Amount` · `Date Type` · `Date` · `Initiation Date` · `Status`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Financial Transaction Capture | 3 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Retrieve` · `Capture`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 7 | 4 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Retrieve` |
| BQ `Financial Transaction Capture` | `Update` · `Capture` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Fraud Evaluation

| | |
|---|---|
| **Patrón funcional** | `Assess` |
| **Tipo de activo** | `Fraud Evaluation` |
| **Artefacto genérico** | `Assessment` |
| **Control Record** | `Fraud Evaluation Assessment` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Account Management |

**Propósito.** The service domain executes fraud behavioral pattern tests to detect possible fraudulent transactions/activity

<details><summary><b>Atributos del Control Record</b> · 7</summary>

`Product Production Session Reference` · `Fraud Evaluation Test Profile` · `Fraud Evaluation Ensemble Technique Type` · `Fraud Evaluation Ensemble Technique Definition` · `Fraud Evaluation Transaction Consolidation Record` · `Fraud Evaluation Production Anomaly Record` · `Fraud Evaluation Production Anomaly Production Transaction Reference`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Rule Sets and Decision Trees | 2 |
| Models | 2 |

**Interfaz.** Action Terms: `Evaluate` · `Exchange` · `Execute` · `Retrieve` · `Grant` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 8 | 6 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Evaluate` · `Exchange` · `Execute` · `Grant` · `Request` · `Retrieve` |
| BQ `Rule Sets and Decision Trees` | `Retrieve` |
| BQ `Models` | `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Fraud Diagnosis

| | |
|---|---|
| **Patrón funcional** | `Analyze` |
| **Tipo de activo** | `Fraud Diagnosis` |
| **Artefacto genérico** | `Analysis` |
| **Control Record** | `Fraud Diagnosis Analysis` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Account Management |

**Propósito.** This service domain handles the evaluation of detected possible fraud to support an appropriate response to contain the exposure

<details><summary><b>Atributos del Control Record</b> · 7</summary>

`Product Production Session Reference` · `Fraud Diagnosis Evaluation Profile` · `Fraud Diagnosis Transaction Consolidation Record` · `Fraud Evaluation Production Anomaly Record` · `Fraud Evaluation Production Anomaly Production Transaction Reference` · `Fraud Diagnosis Determination` · `Fraud Diagnosis Recommendation`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Customer Behavior | 2 |
| Economic Model | 2 |
| Analyst Review | 5 |

**Interfaz.** Action Terms: `Update` · `Evaluate` · `Exchange` · `Request` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 9 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Update` · `Evaluate` · `Exchange` · `Request` · `Retrieve` |
| BQ `Economic Model` | `Retrieve` |
| BQ `Customer Behavior` | `Retrieve` |
| BQ `Analyst Review` | `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Customer Position

| | |
|---|---|
| **Patrón funcional** | `Monitor` |
| **Tipo de activo** | `Customer Position` |
| **Artefacto genérico** | `State` |
| **Control Record** | `Customer Position State` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Account Management |

**Propósito.** This service domain maintains a consolidated financial position for a customer, combining details from all products and services in use

<details><summary><b>Atributos del Control Record</b> · 4</summary>

`Customer Reference` · `Customer Positio Reference` · `Account Reference` · `Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Cashflow | 10 |
| Credit | 4 |
| Collateral Allocation | 11 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Execute` · `Request` · `Retrieve` · `Exchange` · `Capture` · `Evaluate` · `Notify`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 19 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Execute` · `Request` · `Retrieve` |
| BQ `Cashflow` | `Exchange` · `Capture` · `Retrieve` · `Evaluate` · `Notify` |
| BQ `Credit` | `Exchange` · `Capture` · `Retrieve` · `Notify` · `Evaluate` |
| BQ `Collateral Allocation` | `Exchange` · `Capture` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Counterparty Risk

| | |
|---|---|
| **Patrón funcional** | `Monitor` |
| **Tipo de activo** | `Counterparty Credit Risk` |
| **Artefacto genérico** | `State` |
| **Control Record** | `Counterparty Credit Risk Measurement` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Account Management |

[↑ Índice](README.md)

---

## Accounts Receivable

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Accounts Receivable` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Accounts Receivable Procedure` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Account Management |

**Propósito.** This service domain handles accounts receivable for invoices issue by the bank to customers and partners. It includes follow-up and resolution activity for delayed/missed payments

<details><summary><b>Atributos del Control Record</b> · 20</summary>

`Parameter Type` · `Selected Option` · `Request` · `Schedule` · `Status` · `Reference` · `Business Unit Reference` · `Service Provider Reference` · `Financial Facility Reference` · `Employee Reference` · `Customer Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Product and Service Type` · `Product and Service Instance` · `Transaction Type` · `Transaction` · `Financial Transaction Arrangement` · `Customer Agreement Reference`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Resolution | 8 |
| Customer Negotiation | 8 |
| Payment | 8 |
| Receivables Evaluation | 8 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Retrieve` · `Execute` · `Initiate` · `Update` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 22 | 12 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Retrieve` · `Execute` · `Initiate` · `Update` · `Request` |
| BQ `Payment` | `Initiate` · `Retrieve` · `Update` |
| BQ `Receivables Evaluation` | `Exchange` · `Initiate` · `Retrieve` · `Update` |
| BQ `Resolution` | `Initiate` · `Retrieve` · `Update` |
| BQ `Customer Negotiation` | `Initiate` · `Retrieve` · `Exchange` · `Update` · `Request` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Account Reconciliation

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Account Reconciliation` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Account Reconciliation Procedure` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Account Management |

**Propósito.** This Service Domain handles account reconciliation tasks

<details><summary><b>Atributos del Control Record</b> · 27</summary>

`Parameter Type` · `Selected Option` · `Request` · `Schedule` · `Status` · `Associated Party Reference` · `Business Unit Reference` · `Service Provider Reference` · `Financial Facility Reference` · `Employee Reference` · `Customer Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Product and Service Type` · `Product and Service Instance` · `Transaction Type` · `Transaction` · `Financial Transaction Arrangement` · `Customer Agreement Reference` · `Reference` · `Account Reference` · `Document Reference` · `Reconciliation Transaction Reference` · `Reconciliation Arrangement Reference` · `Reconciliation Request Reference` · `System Reference`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Account Assessment | 8 |
| Account Resolution | 8 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Initiate` · `Retrieve` · `Notify` · `Request` · `Update` · `Execute`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 22 | 15 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Initiate` · `Retrieve` · `Notify` · `Request` · `Execute` · `Update` |
| BQ `Account Assessment` | `Exchange` · `Initiate` · `Request` · `Update` · `Notify` · `Execute` · `Retrieve` |
| BQ `Account Resolution` | `Request` · `Update` · `Execute` · `Notify` · `Retrieve` · `Exchange` · `Initiate` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Securities Position Keeping

| | |
|---|---|
| **Patrón funcional** | `Track` |
| **Tipo de activo** | `Securities Position` |
| **Artefacto genérico** | `Log` |
| **Control Record** | `Securities Position Log` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Account Management |

**Propósito.** This service domain maintains a securities transaction log to support securities investment activity

<details><summary><b>Atributos del Control Record</b> · 20</summary>

`Securities Transaction Log Type` · `Product Instance Reference` · `Customer Reference` · `Counterparty Reference` · `Instrument Profile` · `Instrument Record` · `Securities Instrument Type` · `Securities Instrument Reference` · `Securities Position Limits` · `Securities Position Limit Type` · `Securities Position Limit Settings` · `Securities Position Limit Value` · `Securities Amount Block` · `Securities Amount Block Type` · `Priority` · `Amount` · `Date Type` · `Date` · `Initiation Date` · `Status`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Securities Transaction Capture | 3 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Retrieve` · `Capture`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 7 | 4 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Retrieve` |
| BQ `Securities Transaction Capture` | `Update` · `Retrieve` · `Capture` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Transaction Engine

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Transaction Schedule` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Transaction Schedule Facility` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Account Management |

**Propósito.** Orchestrate a schedule of payment transaction and reporting activities for the fulfillment of certain long term instruments or structured facilities

<details><summary><b>Atributos del Control Record</b> · 21</summary>

`Product Instance Reference` · `ProductandService Type` · `Transaction Schedule Fulfillment Schedule` · `Transaction Schedule Work Task Record` · `Transaction Schedule Work Task Type` · `Transaction Schedule Work Task Description` · `Transaction Schedule Work Task Work Products` · `Document Directory Entry Instance Reference` · `Transaction Schedule Work Task Result` · `Transaction Schedule Task Fee Transaction` · `Transaction Schedule Work Task Fee Transaction Description` · `Transaction Schedule Work Task Fee Transaction Type` · `Transaction Schedule Work Task Fee Transaction Charge` · `Transaction Schedule Financial Transaction` · `Transaction Schedule Financial Transaction Product Instance Reference` · `Transaction Schedule Financial Transaction Type` · `Transaction Schedule Financial Transaction Description` · `Transaction Schedule Financial Transaction Amount` · `Correspondence Instance Reference` · `Date Type` · `Date`

</details>

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Exchange` · `Execute` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 6 | 2 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Exchange` · `Execute` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Reward Points Awards And Redemption

| | |
|---|---|
| **Patrón funcional** | `Transact` |
| **Tipo de activo** | `Reward Points` |
| **Artefacto genérico** | `Transaction` |
| **Control Record** | `Reward Points Transaction` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Operational Services |

**Propósito.** Handle the allocation and redemption of rewards points for customer transaction activity

<details><summary><b>Atributos del Control Record</b> · 6</summary>

`Parameter Type` · `Selected Option` · `Status` · `Type` · `Transaction Type` · `Transaction`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Redemption | 7 |
| Award | 7 |

**Interfaz.** Action Terms: `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Request` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 14 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Award` | `Exchange` · `Initiate` · `Retrieve` · `Update` |
| BQ `Redemption` | `Exchange` · `Initiate` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Open Item Management

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Open Item` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Open Item Procedure` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Operational Services |

**Propósito.** This service domain provides a service for handling the resolution of open items against accounts (such as overdue loan payments)

<details><summary><b>Atributos del Control Record</b> · 8</summary>

`Open Item Type` · `Open Item Description` · `Product Instance Reference` · `Party Reference` · `Loan Repayment Schedule` · `Loan Outstanding Balance` · `Loan Termination Date` · `Repayment Statement`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Tracking | 6 |
| Repayment | 7 |

**Interfaz.** Action Terms: `Control` · `Request` · `Retrieve` · `Update` · `Initiate` · `Exchange` · `Execute`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 11 | 6 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Request` · `Retrieve` · `Update` · `Initiate` |
| BQ `Tracking` | `Retrieve` |
| BQ `Repayment` | `Update` · `Exchange` · `Execute` · `Retrieve` · `Initiate` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Leasing Item Administration

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Leasing Item` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Leasing Item Administrative Plan` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Operational Services |

**Propósito.** Track the status of the assets underlying leasing agreements as they represent collateral items that could be accessed in the event of account recovery

<details><summary><b>Atributos del Control Record</b> · 5</summary>

`Budget Type` · `Budget` · `Assignment` · `Leasing Item Administrative Plan` · `Reference`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Valuation | 8 |
| Assurance | 8 |
| Item Registration | 8 |

**Interfaz.** Action Terms: `Capture` · `Control` · `Exchange` · `Grant` · `Initiate` · `Retrieve` · `Request` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 20 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Capture` · `Control` · `Exchange` · `Grant` · `Initiate` · `Retrieve` · `Request` · `Update` |
| BQ `Assurance` | `Capture` · `Initiate` · `Retrieve` · `Update` |
| BQ `Item Registration` | `Capture` · `Retrieve` · `Initiate` · `Update` |
| BQ `Valuation` | `Capture` · `Initiate` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Issued Device Tracking

| | |
|---|---|
| **Patrón funcional** | `Monitor` |
| **Tipo de activo** | `Issued Device` |
| **Artefacto genérico** | `State` |
| **Control Record** | `Issued Device State` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Operational Services |

**Propósito.** This service domain handles operational access to issued device tracking services. Services report on the status of devices such as cards, fobs, etc. that have been issued to customers. Service notifications include fraud warnings/alerts and device cancellation.

<details><summary><b>Atributos del Control Record</b> · 3</summary>

`Information Feed Provider Reference` · `Issued Device Allocation Instance Reference` · `Issued Device Allocation Status`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Internal Notification | 7 |
| External Report | 8 |

**Interfaz.** Action Terms: `Control` · `Retrieve` · `Update` · `Initiate` · `Capture`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 10 | 6 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Initiate` · `Update` · `Retrieve` |
| BQ `Internal Notification` | `Retrieve` · `Update` · `Capture` |
| BQ `External Report` | `Update` · `Capture` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Issued Device Administration

| | |
|---|---|
| **Patrón funcional** | `Allocate` |
| **Tipo de activo** | `Issued Device` |
| **Artefacto genérico** | `Allocation` |
| **Control Record** | `Issued Device Allocation` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Operational Services |

**Propósito.** This service domain administers the issuance of authentication tokens to customers and third party service providers. Tokens here include physical devices such as cards, fobs, readers and intangible

<details><summary><b>Atributos del Control Record</b> · 6</summary>

`Customer Reference` · `Product Instance Reference` · `Issued Device Type` · `Associated Permissions` · `Issue Date` · `Valid From-To Date`

</details>

**Behavior Qualifiers** · 7

| Behavior Qualifier | Atributos |
|---|---:|
| Password Assignment | 4 |
| Question Assignment | 5 |
| Device Assignment | 7 |
| Biometric Assignment | 2 |
| Reader Assignment | 5 |
| Cheques Assignment | 3 |
| Token Assignment | 11 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Exchange` · `Retrieve` · `Capture` · `Execute` · `Provide`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 39 | 16 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Exchange` · `Retrieve` |
| BQ `Password Assignment` | `Update` · `Control` · `Retrieve` · `Capture` · `Initiate` · `Exchange` |
| BQ `Question Assignment` | `Control` · `Initiate` · `Update` · `Exchange` · `Capture` · `Retrieve` |
| BQ `Biometric Assignment` | `Initiate` · `Exchange` · `Update` · `Control` · `Retrieve` |
| BQ `Device Assignment` | `Retrieve` · `Update` · `Control` · `Capture` |
| BQ `Reader Assignment` | `Update` · `Retrieve` · `Control` · `Capture` |
| BQ `Cheques Assignment` | `Initiate` · `Exchange` · `Retrieve` · `Control` |
| BQ `Token Assignment` | `Retrieve` · `Capture` · `Update` · `Execute` · `Provide` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Disbursement

| | |
|---|---|
| **Patrón funcional** | `Transact` |
| **Tipo de activo** | `Disbursement` |
| **Artefacto genérico** | `Transaction` |
| **Control Record** | `Disbursement Transaction` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Operational Services |

**Propósito.** This service domain handles the disbursement of funds to newly established loans/facilities as necessary

<details><summary><b>Atributos del Control Record</b> · 27</summary>

`Product Instance Reference` · `Initiating Customer Reference` · `Beneficiary Reference` · `Payment Amount` · `Payment Currency` · `Disbursement Execution Date` · `Authorising Employee Reference` · `Initiating Account Reference` · `Beneficiary Account Reference` · `Beneficiary External Account Number` · `Beneficiary Name` · `Beneficiary Address` · `Beneficiary Bank Reference` · `Payment Value Date` · `Payment Execution Date` · `Payment Details` · `Disbursement Type` · `Disbursement Tax Account Reference` · `Disbursement Tax Amount` · `Disbursement Tax Currency` · `Disbursement Tax Type` · `Disbursement Fee Account Reference` · `Disbursement Fee Amount` · `Disbursement Fee Currency` · `Disbursement Fee Type` · `Disbursement Status` · `Disbursement Process Reference`

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

## Delinquent Account Handling

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Delinquent Account` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Delinquent Account Procedure` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Operational Services |

**Propósito.** This service domain handles delinquent accounts for follow-up of payments due through periodic review and contacts

<details><summary><b>Atributos del Control Record</b> · 36</summary>

`Product Instance Reference` · `Product Account Number` · `ProductandService Type` · `Customer Reference` · `Bank Branch/Location Reference` · `Issued Device` · `Account Currency` · `Tax Reference` · `Associations` · `Association Type` · `Association Obligation and Entitlement` · `Association Reference` · `Linked Accounts` · `Link Type` · `Account Details` · `Position Limits` · `Position Limit Type` · `Position Limit Settings` · `Position Limit Value` · `Collateral Asset Allocation Instance Reference` · `Collateral Asset Allocation Profile` · `Date Type` · `Date` · `Billing Transactions` · `Billing Transaction Reference` · `Payment Transactions` · `Payment Transaction Reference` · `Product Transactions` · `Product Transaction Reference` · `Interest Transactions` · `Interest Transaction Reference` · `Fee Transactions` · `Fee Transaction Reference` · `Credit Plan Reference` · `Credit Plan Type` · `Delinquent Account Processing Schedule`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Assessment | 2 |
| Contact | 10 |
| Payment | 2 |
| Resolution | 3 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Retrieve` · `Control` · `Execute` · `Exchange` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 16 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Execute` · `Retrieve` |
| BQ `Assessment` | `Retrieve` |
| BQ `Contact` | `Initiate` · `Request` · `Retrieve` |
| BQ `Payment` | `Update` · `Exchange` · `Initiate` · `Retrieve` |
| BQ `Resolution` | `Update` · `Exchange` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Channel Activity History

| | |
|---|---|
| **Patrón funcional** | `Track` |
| **Tipo de activo** | `Channel Activity` |
| **Artefacto genérico** | `Log` |
| **Control Record** | `Channel Activity Log` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Operational Services |

**Propósito.** This service domains consolidates and captures customer channel usage activity to support channel activity analysis

<details><summary><b>Atributos del Control Record</b> · 2</summary>

`Customer Reference` · `Date`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Event | 24 |

**Interfaz.** Action Terms: `Initiate` · `Retrieve` · `Control` · `Update` · `Capture`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 7 | 4 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Retrieve` · `Control` · `Update` |
| BQ `Event` | `Update` · `Capture` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Channel Activity Analysis

| | |
|---|---|
| **Patrón funcional** | `Analyze` |
| **Tipo de activo** | `Channel Activity` |
| **Artefacto genérico** | `Analysis` |
| **Control Record** | `Channel Activity Analysis` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Operational Services |

**Propósito.** This service domain tracks and analyzes channel activity to support relationship development, to detect unwanted behavior, possible fraud, and to constrain channel use as necessary

<details><summary><b>Atributos del Control Record</b> · 6</summary>

`Channel Type` · `Period` · `Type` · `Result` · `Record` · `Channel Activity History Report`

</details>

**Behavior Qualifiers** · 6

| Behavior Qualifier | Atributos |
|---|---:|
| Customer Fraud | 3 |
| Merchant Fraud | 3 |
| Customer Behavior | 3 |
| Merchant Behavior | 3 |
| Bot | 3 |
| Device Error | 3 |

**Interfaz.** Action Terms: `Exchange` · `Evaluate` · `Request` · `Retrieve` · `Execute`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 16 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Exchange` · `Evaluate` · `Request` · `Retrieve` |
| BQ `Customer Fraud` | `Execute` · `Retrieve` |
| BQ `Merchant Fraud` | `Execute` · `Retrieve` |
| BQ `Merchant Behavior` | `Retrieve` · `Execute` |
| BQ `Customer Behavior` | `Execute` · `Retrieve` |
| BQ `Bot` | `Execute` · `Retrieve` |
| BQ `Device Error` | `Execute` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Card Transaction Switch

| | |
|---|---|
| **Patrón funcional** | `Operate` |
| **Tipo de activo** | `Card Transaction Switch` |
| **Artefacto genérico** | `Operating Session` |
| **Control Record** | `Card Transaction Switch Operating Session` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Operational Services |

**Propósito.** This service domain orchestrates the switching and routing of Card Authorization and Financial transactions

<details><summary><b>Atributos del Control Record</b> · 5</summary>

`Network Reference` · `Participant Acquirer Bank Reference` · `Participant Acquirer Bank transaction Routing Details` · `Participant Issuer Bank Reference` · `Participant Issuer Bank Transaction Routing Details`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Transaction Capture | 16 |
| Transaction Routing | 0 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Exchange` · `Retrieve` · `Control`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 7 | 4 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Exchange` · `Retrieve` · `Control` |
| BQ `Transaction Capture` | `Initiate` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Card Collections

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Card Collections` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Card Collections Procedure` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Operational Services |

**Propósito.** This service domain administers the recovery of outstanding amounts from cancelled card accounts through internal or external collection agencies

<details><summary><b>Atributos del Control Record</b> · 17</summary>

`Product Instance Reference` · `Product and Service Type` · `Customer Reference` · `Card Type` · `Card Account Status` · `Card Account Limits` · `Configuration/Options` · `Tax Reference` · `Billing Transactions` · `Billing Transaction Reference` · `Payment Transactions` · `Payment Transaction Reference` · `Product Transactions` · `Product Transaction Reference` · `Statements` · `Statements Reference` · `Card Collections Processing Schedule`

</details>

**Behavior Qualifiers** · 4

| Behavior Qualifier | Atributos |
|---|---:|
| Assignment | 6 |
| Payment Terms | 10 |
| Payment | 3 |
| Resolution | 2 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Execute` · `Request` · `Retrieve` · `Exchange`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 16 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Execute` · `Request` · `Retrieve` |
| BQ `Assignment` | `Retrieve` |
| BQ `Payment Terms` | `Exchange` · `Retrieve` · `Update` |
| BQ `Payment` | `Initiate` · `Update` · `Exchange` · `Retrieve` |
| BQ `Resolution` | `Update` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Customer Billing

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Customer Billing` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Customer Billing Procedure` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Operational Services |

**Propósito.** This service domains provides a central service to compose, issue and track customer billing and invoices

<details><summary><b>Atributos del Control Record</b> · 14</summary>

`Customer Billing Transaction Type` · `Customer Billing Transaction Description` · `Customer Reference` · `Product Instance Reference` · `Customer Agreement Reference` · `Customer Billing ProductandService/Action Description` · `Customer Billing Party` · `Customer Billing Address` · `Customer Billing Period` · `Customer Billing Statement` · `Customer Billing Amount` · `Customer Billing Payment Due Date` · `Customer Billing Payment Details` · `Customer Billing Payment Schedule`

</details>

**Behavior Qualifiers** · 3

| Behavior Qualifier | Atributos |
|---|---:|
| Invoicing | 6 |
| Tracking and Reminders | 6 |
| Payment | 2 |

**Interfaz.** Action Terms: `Initiate` · `Update` · `Control` · `Execute` · `Request` · `Retrieve` · `Exchange`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 15 | 8 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Initiate` · `Update` · `Control` · `Execute` · `Request` · `Retrieve` |
| BQ `Invoicing` | `Update` · `Retrieve` |
| BQ `Tracking and Reminders` | `Initiate` · `Exchange` · `Retrieve` |
| BQ `Payment` | `Initiate` · `Exchange` · `Update` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Internal Bank Account

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Internal Bank Account` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Internal Bank Account Facility` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Operational Services |

**Propósito.** This Service Domain manages the banking-related accounts that are not owned by customers. These are not general ledger accounts. Typical examples are holding accounts and mirror accounts.

<details><summary><b>Atributos del Control Record</b> · 17</summary>

`Internal Bank Account Status` · `Internal Bank Account Calendar Reference` · `Internal Bank Account Reference` · `Internal Bank Account Currency` · `Internal Bank Account Associated Party` · `Internal Bank Account Selected Option` · `Internal Bank Account Position` · `Internal Bank Account Parameter Type` · `Internal Bank Account Type` · `Internal Bank Account Regulation Type` · `Internal Bank Account Customer Reference` · `Internal Bank Account Booking Location` · `Internal Bank Account Regulation Reference` · `Internal Bank Account Jurisdiction` · `Internal Bank Account Position Limit` · `Internal Bank Account Product Reference` · `Reference`

</details>

**Behavior Qualifiers** · 1

| Behavior Qualifier | Atributos |
|---|---:|
| Booking | 8 |

**Interfaz.** Action Terms: `Control` · `Capture` · `Notify` · `Execute` · `Initiate` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 7 | 5 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Capture` · `Notify` · `Initiate` · `Retrieve` · `Update` |
| BQ `Booking` | `Execute` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Processing Order

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Processing Order` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Processing Order Procedure` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Operational Services |

**Propósito.** The Processing Order Service Domain handles the processing of a service request that comes in via a secure channel from a known requestor, which is typically an automated process itself and not a customer.

<details><summary><b>Atributos del Control Record</b> · 21</summary>

`Parameter Type` · `Selected Option` · `Request` · `Schedule` · `Status` · `Associated Party Reference` · `Business Unit Reference` · `Service Provider Reference` · `Financial Facility Reference` · `Employee Reference` · `Customer Reference` · `Processing Order ProcedureType` · `Service Provider Schedule` · `Service Type` · `Product and Service Type` · `Product and Service Instance` · `Processing Order ProcedureTransaction Type` · `Processing Order ProcedureTransaction` · `Financial Transaction Arrangement` · `Customer Agreement Reference` · `Reference`

</details>

**Interfaz.** Action Terms: `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 8 | 5 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Initiate` · `Notify` · `Request` · `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Incentive Program Directory

| | |
|---|---|
| **Patrón funcional** | `Catalog` |
| **Tipo de activo** | `Incentive Program` |
| **Artefacto genérico** | `Directory Entry` |
| **Control Record** | `Incentive Program Directory Entry` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Operational Services |

**Propósito.** This service domain maintains specifications of the various Incentive Programs that are on offer to customers

<details><summary><b>Atributos del Control Record</b> · 8</summary>

`Description` · `Schedule` · `Version` · `Status` · `Usage Log` · `Update Log` · `Service Configuration` · `Reference`

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Incentive Account

| | |
|---|---|
| **Patrón funcional** | `Fulfill` |
| **Tipo de activo** | `Incentive Account` |
| **Artefacto genérico** | `Facility` |
| **Control Record** | `Incentive Account Facility` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Operational Services |

**Propósito.** This service domain orchestrates the scheduled maintenance and transactional activities associated with Incentive Program fulfillment

<details><summary><b>Atributos del Control Record</b> · 6</summary>

`Account Reference` · `Incentive Account Product Reference` · `Reference` · `Incentive Account Agreement Reference` · `Incentive Account Arrangement Reference` · `Incentive Account Involvement`

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Rewards Menu

| | |
|---|---|
| **Patrón funcional** | `Catalog` |
| **Tipo de activo** | `Rewards Option` |
| **Artefacto genérico** | `Directory Entry` |
| **Control Record** | `Rewards Option Directory Entry` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Operational Services |

**Propósito.** The service domain presents a set of eligible rewards a customer can select from.

<details><summary><b>Atributos del Control Record</b> · 8</summary>

`Description` · `Schedule` · `Version` · `Status` · `Usage Log` · `Update Log` · `Service Configuration` · `Reference`

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Rewards Inventory

| | |
|---|---|
| **Patrón funcional** | `Allocate` |
| **Tipo de activo** | `Rewards Inventory` |
| **Artefacto genérico** | `Allocation` |
| **Control Record** | `Rewards Inventory Allocation` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Operational Services |

**Propósito.** The service domain handles the allocation of rewards from available inventory.

<details><summary><b>Atributos del Control Record</b> · 17</summary>

`Parameter Type` · `Selected Option` · `Type` · `Description` · `Request` · `Schedule` · `Status` · `Reference` · `Customer Reference` · `Currency` · `Regulation Reference` · `Regulation Type` · `Jurisdiction` · `Booking Location` · `Account Type` · `Account Reference` · `Instance`

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Rewards Delivery

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Rewards Delivery` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Rewards Delivery Procedure` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Operational Services |

**Propósito.** The service domain orchestrates the entire end-to-end process for delivering a redeemed reward.

<details><summary><b>Atributos del Control Record</b> · 21</summary>

`Parameter Type` · `Selected Option` · `Request` · `Schedule` · `Status` · `Associated Party Reference` · `Business Unit Reference` · `Service Provider Reference` · `Financial Facility Reference` · `Employee Reference` · `Customer Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Product and Service Type` · `Product and Service Instance` · `Transaction Type` · `Transaction` · `Financial Transaction Arrangement` · `Customer Agreement Reference` · `Reference`

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Issued Certificate Directory

| | |
|---|---|
| **Patrón funcional** | `Catalog` |
| **Tipo de activo** | `Issued Certificate` |
| **Artefacto genérico** | `Directory Entry` |
| **Control Record** | `Issued Certificate Directory Entry` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Operational Services |

**Propósito.** This service domain faciliatates the issuance of Rewards Certificates and their redemption.

<details><summary><b>Atributos del Control Record</b> · 8</summary>

`Description` · `Schedule` · `Version` · `Status` · `Usage Log` · `Update Log` · `Service Configuration` · `Reference`

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Collections

| | |
|---|---|
| **Patrón funcional** | `Process` |
| **Tipo de activo** | `Collateral Asset Liquidation` |
| **Artefacto genérico** | `Procedure` |
| **Control Record** | `Collateral Asset Liquidation Procedure` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Collateral Administration |

**Propósito.** Handles the liquidation of assets to offset the losses for problem accounts

<details><summary><b>Atributos del Control Record</b> · 20</summary>

`Parameter Type` · `Selected Option` · `Request` · `Schedule` · `Status` · `Reference` · `Business Unit Reference` · `ServiceProvider Reference` · `Financial Facility Reference` · `Employee Reference` · `Customer Reference` · `Type` · `Service Provider Schedule` · `Service Type` · `Product and Service Type` · `Product and Service Instance` · `Transaction Type` · `Transaction` · `Financial Transaction Arrangement` · `Customer Agreement Reference`

</details>

**Behavior Qualifiers** · 5

| Behavior Qualifier | Atributos |
|---|---:|
| Debt Factoring | 8 |
| Collateral Valuation | 8 |
| Collateral Liquidation | 8 |
| Collections Assessment | 8 |
| Collections Account Update | 8 |

**Interfaz.** Action Terms: `Control` · `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Update` · `Request`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 24 | 14 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Control` · `Exchange` · `Execute` · `Initiate` · `Retrieve` · `Update` · `Request` |
| BQ `Collateral Valuation` | `Exchange` · `Initiate` · `Retrieve` · `Update` |
| BQ `Collateral Liquidation` | `Initiate` · `Exchange` · `Retrieve` · `Update` |
| BQ `Debt Factoring` | `Initiate` · `Exchange` · `Retrieve` · `Update` |
| BQ `Collections Assessment` | `Initiate` · `Retrieve` · `Update` |
| BQ `Collections Account Update` | `Retrieve` · `Update` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Collateral Allocation Management

| | |
|---|---|
| **Patrón funcional** | `Allocate` |
| **Tipo de activo** | `Collateral Asset` |
| **Artefacto genérico** | `Allocation` |
| **Control Record** | `Collateral Asset Allocation` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Collateral Administration |

**Propósito.** The Service Domain manages the allocation of party owned assets to bank issued lending and other asset products

<details><summary><b>Atributos del Control Record</b> · 17</summary>

`Collateral Allocation Amount` · `Collateral Allocation Description` · `Collateral Allocation End Date` · `Collateral Allocation Start Date` · `Collateral Allocation Recall Amount` · `Collateral Allocation Recall Schedule` · `Collateral Allocation Recall Result` · `Collateral Current Value Amount` · `Collateral Earmarked Amount` · `Collateral Earmarked End Date` · `Collateral Earmarked Start Date` · `Collateral Status` · `Party Asset Description` · `Party Asset Directory Reference` · `Product Instance Name` · `Product Instance Reference` · `Evaluate Acceptability Result Description`

</details>

**Interfaz.** Action Terms: `Update` · `Retrieve` · `Exchange` · `Capture`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 4 | 2 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Update` · `Retrieve` · `Exchange` · `Capture` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Party Asset Directory

| | |
|---|---|
| **Patrón funcional** | `Catalog` |
| **Tipo de activo** | `Party Asset` |
| **Artefacto genérico** | `Directory Entry` |
| **Control Record** | `Party Asset Directory Entry` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Collateral Administration |

**Propósito.** This directory maintains reference details of assets held by a party, usually a customer of the bank. In most case, the bank

<details><summary><b>Atributos del Control Record</b> · 9</summary>

`Description` · `Schedule` · `Version` · `Status` · `Usage Log` · `Update Log` · `Service Configuration` · `Reference` · `Party Asset Reference`

</details>

**Behavior Qualifiers** · 7

| Behavior Qualifier | Atributos |
|---|---:|
| Asset Type Classification | 0 |
| Asset Title Ownership | 0 |
| Asset Location or Jurisdiction | 0 |
| Asset Properties | 15 |
| Asset Insurance | 11 |
| Asset Estimated Value | 10 |
| Asset Maintenance | 9 |

**Interfaz.** Action Terms: `Register` · `Update` · `Retrieve`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 12 | 10 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| BQ `Asset Properties` | `Register` · `Update` · `Retrieve` |
| BQ `Asset Estimated Value` | `Update` · `Register` · `Retrieve` |
| BQ `Asset Insurance` | `Register` · `Update` · `Retrieve` |
| BQ `Asset Maintenance` | `Update` · `Register` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---

## Collateral Asset Administration

| | |
|---|---|
| **Patrón funcional** | `Administer` |
| **Tipo de activo** | `Collateral Asset` |
| **Artefacto genérico** | `Administrative Plan` |
| **Control Record** | `Collateral Asset Administrative Plan` |
| **Ubicación Matrix** | Operations and Execution › Cross Product Operations › Collateral Administration |

**Propósito.** This service domain maintains the status of a customers collateral assets, including scheduled and ad-hoc valuations

<details><summary><b>Atributos del Control Record</b> · 18</summary>

`Collateral Asset Reference` · `Collateral Asset Record` · `Collateral Asset Type` · `Collateral Asset Properties` · `Collateral Asset Description` · `Collateral Asset Title` · `Collateral Asset Ownership` · `Collateral Asset Interested Parties` · `Collateral Asset Location` · `Collateral Asset Jurisdiction` · `Collateral Asset Document Reference` · `Collateral Asset Document Type` · `Collateral Asset Insurance Reference` · `Collateral Asset Pledged Date` · `Collateral Asset Valuation History` · `Collateral Asset Valuation Schedule` · `Collateral Asset Maintenance Schedule` · `Collateral Asset Status`

</details>

**Behavior Qualifiers** · 2

| Behavior Qualifier | Atributos |
|---|---:|
| Valuation | 5 |
| Maintenance | 4 |

**Interfaz.** Action Terms: `Create` · `Update` · `Retrieve` · `Request` · `Exchange`

| Operaciones inbound | Eventos outbound |
|---:|---:|
| 12 | 6 |

<details><summary><b>Qué Action Term activa qué Behavior Qualifier</b></summary>

| Nivel | Action Terms que lo activan |
|---|---|
| **Control Record** | `Create` · `Update` · `Retrieve` |
| BQ `Valuation` | `Create` · `Update` · `Request` · `Retrieve` |
| BQ `Maintenance` | `Update` · `Create` · `Exchange` · `Request` · `Retrieve` |

</details>

**Semántica.** BOM mapping: Sí · ISO 20022: Sí

[↑ Índice](README.md)

---
