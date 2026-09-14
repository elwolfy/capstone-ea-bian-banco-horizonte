# BIAN v14 · Service Landscape · vista Matrix

**341 Service Domains** · 5 Business Areas · 26 Business Domains de primer nivel · 10 anidados

> Curso independiente de CPS Tech · No afiliado ni acreditado por BIAN e.V. · BIAN® es marca registrada de BIAN e.V., usada con fines descriptivos.

---

## Cómo se lee

Cada Service Domain es la síntesis de un **patrón funcional** aplicado a un **tipo de activo**. La ejecución de ese patrón produce un **artefacto genérico**, y el registro que lo gobierna es la suma de ambos:

```
Control Record = Asset Type + Generic Artifact
```

El Service Domain y su Control Record son **uno a uno**: ése es el nivel donde el catálogo cumple MECE. Los Business Domains anidados se tratan como capacidades de negocio agrupadoras, no como un nivel del metamodelo.

---

## Business Areas

| Business Area | Service Domains | Detalle |
|---|---:|---|
| **Sales and Service** | 74 | [ver fichas](01_Sales_and_Service.md) |
| **Reference Data** | 33 | [ver fichas](02_Reference_Data.md) |
| **Operations and Execution** | 130 | [ver fichas](03_Operations_and_Execution.md) |
| **Risk and Compliance** | 36 | [ver fichas](04_Risk_and_Compliance.md) |
| **Business Support** | 68 | [ver fichas](05_Business_Support.md) |
| | **341** | |

---

## Cobertura del catálogo

| Dato | Cobertura |
|---|---|
| Patrón funcional | 341 / 341 · 100 % |
| Tipo de activo | 341 / 341 · 100 % |
| Control Record | 341 / 341 · 100 % |
| Propósito publicado | 258 / 341 · 76 % |
| Atributos del Control Record | 257 / 341 · 75 % |
| Behavior Qualifiers | 230 / 341 · 67 % |
| Action Terms | 242 / 341 · 71 % |
| API semántica publicada | 258 / 341 · 76 % |

En total: **3 392 atributos** de Control Record, **865 Behavior Qualifiers**, **4 580 operaciones inbound** y **2 684 eventos outbound**.

---

## Patrones funcionales en uso

| Patrón funcional | Artefacto genérico | Service Domains |
|---|---|---:|
| `Fulfill` | `Facility` | 43 |
| `Process` | `Procedure` | 42 |
| `Administer` | `Administrative Plan` | 31 |
| `Operate` | `Operating Session` | 30 |
| `Manage` | `Management Plan` | 26 |
| `Analyze` | `Analysis` | 24 |
| `Assess` | `Assessment` | 23 |
| `Catalog` | `Directory Entry` | 20 |
| `Design` | `Specification` | 20 |
| `Agree Terms` | `Agreement` | 18 |
| `Transact` | `Transaction` | 14 |
| `Direct` | `Strategy` | 11 |
| `Track` | `Log` | 10 |
| `Allocate` | `Allocation` | 9 |
| `Monitor` | `State` | 7 |
| `Advise` | `Advice` | 5 |
| `Enroll` | `Membership` | 3 |
| `Develop` | `Development` | 3 |
| `Maintain` | `Maintenance Arrangement` | 2 |

---

## Índice completo · los 341 Service Domains

| # | Service Domain | Patrón | Tipo de activo | Control Record | Ubicación Matrix |
|---:|---|---|---|---|---|
| 1 | [ATM Network Management](01_Sales_and_Service.md#atm-network-management) | `Manage` | `ATM Network` | `ATM Network Management Plan` | Sales and Service › Channel Specific |
| 2 | [ATM Network Operations](01_Sales_and_Service.md#atm-network-operations) | `Operate` | `ATM Network` | `ATM Network Operating Session` | Sales and Service › Channel Specific |
| 3 | [Account Reconciliation](03_Operations_and_Execution.md#account-reconciliation) | `Process` | `Account Reconciliation` | `Account Reconciliation Procedure` | Operations and Execution › Cross Product Operations › Account Management |
| 4 | [Account Recovery](01_Sales_and_Service.md#account-recovery) | `Process` | `Account Recovery` | `Account Recovery Procedure` | Sales and Service › Customer Management |
| 5 | [Accounts Receivable](03_Operations_and_Execution.md#accounts-receivable) | `Process` | `Accounts Receivable` | `Accounts Receivable Procedure` | Operations and Execution › Cross Product Operations › Account Management |
| 6 | [Advanced Voice Services Management](01_Sales_and_Service.md#advanced-voice-services-management) | `Manage` | `Voice Channel` | `Voice Channel Management Plan` | Sales and Service › Channel Specific |
| 7 | [Advanced Voice Services Operations](01_Sales_and_Service.md#advanced-voice-services-operations) | `Operate` | `Voice Channel` | `Voice Channel Operating Session` | Sales and Service › Channel Specific |
| 8 | [Advertising](01_Sales_and_Service.md#advertising) | `Manage` | `Advertising Campaign` | `Advertising Campaign Management Plan` | Sales and Service › Marketing |
| 9 | [Approved Supplier Directory](05_Business_Support.md#approved-supplier-directory) | `Enroll` | `Supplier` | `Supplier Membership` | Business Support › Non-IT and Non-HR Enterprise Services |
| 10 | [Archive Services](05_Business_Support.md#archive-services) | `Operate` | `Archive` | `Archive Operating Session` | Business Support › Document Management and Archive |
| 11 | [Asset And Liability Management](04_Risk_and_Compliance.md#asset-and-liability-management) | `Direct` | `Asset And Liability Portfolio` | `Asset And Liability Portfolio Strategy` | Risk and Compliance › Bank Portfolio and Treasury |
| 12 | [Asset Securitization](04_Risk_and_Compliance.md#asset-securitization) | `Transact` | `Asset Securitization` | `Asset Securitization Transaction` | Risk and Compliance › Bank Portfolio and Treasury |
| 13 | [Bank Drafts](03_Operations_and_Execution.md#bank-drafts) | `Transact` | `Bearer Document` | `Bearer Document Transaction` | Operations and Execution › Product Specific Fulfillment › Consumer Services |
| 14 | [Bank Guarantee](03_Operations_and_Execution.md#bank-guarantee) | `Transact` | `Bank Guarantee` | `Bank Guarantee Transaction` | Operations and Execution › Product Specific Fulfillment › Trade Banking |
| 15 | [Bank Portfolio Administration](04_Risk_and_Compliance.md#bank-portfolio-administration) | `Administer` | `Asset And Liability Portfolio` | `Asset And Liability Portfolio Administrative Plan` | Risk and Compliance › Bank Portfolio and Treasury |
| 16 | [Bank Portfolio Analysis](04_Risk_and_Compliance.md#bank-portfolio-analysis) | `Analyze` | `Asset And Liability Portfolio` | `Asset And Liability Portfolio Analysis` | Risk and Compliance › Bank Portfolio and Treasury |
| 17 | [Branch Currency Distribution](01_Sales_and_Service.md#branch-currency-distribution) | `Process` | `Cash Distribution` | `Cash Distribution Procedure` | Sales and Service › Channel Specific |
| 18 | [Branch Currency Management](01_Sales_and_Service.md#branch-currency-management) | `Allocate` | `Branch Cash` | `Branch Cash Allocation` | Sales and Service › Channel Specific |
| 19 | [Branch Location Management](01_Sales_and_Service.md#branch-location-management) | `Manage` | `Branch Location` | `Branch Location Management Plan` | Sales and Service › Channel Specific |
| 20 | [Branch Location Operations](01_Sales_and_Service.md#branch-location-operations) | `Administer` | `Branch Location` | `Branch Location Administrative Plan` | Sales and Service › Channel Specific |
| 21 | [Branch Network Management](01_Sales_and_Service.md#branch-network-management) | `Manage` | `Branch Network` | `Branch Network Management Plan` | Sales and Service › Channel Specific |
| 22 | [Branch Portfolio](04_Risk_and_Compliance.md#branch-portfolio) | `Analyze` | `Branch Network` | `Branch Network Analysis` | Risk and Compliance › Business Analysis |
| 23 | [Brand Management](01_Sales_and_Service.md#brand-management) | `Manage` | `Brand` | `Brand Management Plan` | Sales and Service › Marketing |
| 24 | [Brokered Product Proxy](03_Operations_and_Execution.md#brokered-product-proxy) | `Fulfill` | `Brokered Product` | `Brokered Product Facility` | Operations and Execution › Product Specific Fulfillment › Consumer Services |
| 25 | [Building Maintenance](05_Business_Support.md#building-maintenance) | `Maintain` | `Building` | `Building Maintenance Arrangement` | Business Support › Buildings Equipment and Facilities |
| 26 | [Business Development](01_Sales_and_Service.md#business-development) | `Direct` | `Business Development` | `Business Development Strategy` | Sales and Service › Marketing |
| 27 | [Business Risk Models](04_Risk_and_Compliance.md#business-risk-models) | `Design` | `Business Operation Risk Model` | `Business Operation Risk Model Specification` | Risk and Compliance › Models |
| 28 | [Business Unit Accounting](05_Business_Support.md#business-unit-accounting) | `Track` | `Business Unit Accounting` | `Business Unit Accounting Log` | Business Support › Business Command and Control |
| 29 | [Business Unit Direction](05_Business_Support.md#business-unit-direction) | `Direct` | `Business Unit` | `Business Unit Strategy` | Business Support › Business Command and Control |
| 30 | [Business Unit Financial Analysis](05_Business_Support.md#business-unit-financial-analysis) | `Analyze` | `Business Unit Finance` | `Business Unit Finance Analysis` | Business Support › Business Command and Control |
| 31 | [Business Unit Financial Operations](05_Business_Support.md#business-unit-financial-operations) | `Administer` | `Busines Unit Budegt` | `Busines Unit Budegt Administrative Plan` | Business Support › Business Command and Control |
| 32 | [Business Unit Management](05_Business_Support.md#business-unit-management) | `Manage` | `Business Unit` | `Business Unit Management Plan` | Business Support › Business Command and Control |
| 33 | [Card Authorization](03_Operations_and_Execution.md#card-authorization) | `Assess` | `Credit Card Authorization` | `Credit Card Authorization Assessment` | Operations and Execution › Product Specific Fulfillment › Cards |
| 34 | [Card Case](01_Sales_and_Service.md#card-case) | `Process` | `Card Case` | `Card Case Procedure` | Sales and Service › Servicing |
| 35 | [Card Clearing](03_Operations_and_Execution.md#card-clearing) | `Process` | `Card Clearing` | `Card Clearing Procedure` | Operations and Execution › Cross Product Operations › Payments |
| 36 | [Card Collections](03_Operations_and_Execution.md#card-collections) | `Process` | `Card Collections` | `Card Collections Procedure` | Operations and Execution › Cross Product Operations › Operational Services |
| 37 | [Card Financial Settlement](03_Operations_and_Execution.md#card-financial-settlement) | `Process` | `Card Financial Settlement` | `Card Financial Settlement Procedure` | Operations and Execution › Cross Product Operations › Payments |
| 38 | [Card Network Participant Facility](03_Operations_and_Execution.md#card-network-participant-facility) | `Agree Terms` | `Card Network Participant` | `Card Network Participant Agreement` | Operations and Execution › Product Specific Fulfillment › Cards |
| 39 | [Card Terminal Administration](01_Sales_and_Service.md#card-terminal-administration) | `Allocate` | `Card POS Device` | `Card POS Device Allocation` | Sales and Service › Channel Specific |
| 40 | [Card Terminal Operation](01_Sales_and_Service.md#card-terminal-operation) | `Operate` | `Card POS Network` | `Card POS Network Operating Session` | Sales and Service › Channel Specific |
| 41 | [Card Transaction Capture](03_Operations_and_Execution.md#card-transaction-capture) | `Transact` | `Card Financial Capture` | `Card Financial Capture Transaction` | Operations and Execution › Product Specific Fulfillment › Cards |
| 42 | [Card Transaction Switch](03_Operations_and_Execution.md#card-transaction-switch) | `Operate` | `Card Transaction Switch` | `Card Transaction Switch Operating Session` | Operations and Execution › Cross Product Operations › Operational Services |
| 43 | [Card Transaction Tracking](03_Operations_and_Execution.md#card-transaction-tracking) | `Track` | `Credit Card Position` | `Credit Card Position Log` | Operations and Execution › Product Specific Fulfillment › Cards |
| 44 | [Card eCommerce Gateway](03_Operations_and_Execution.md#card-ecommerce-gateway) | `Operate` | `eCommerce Gateway` | `eCommerce Gateway Operating Session` | Operations and Execution › Cross Product Operations › Payments |
| 45 | [Case Root Cause Analysis](01_Sales_and_Service.md#case-root-cause-analysis) | `Analyze` | `Customer Case Root Cause` | `Customer Case Root Cause Analysis` | Sales and Service › Servicing |
| 46 | [Cash Concentration](03_Operations_and_Execution.md#cash-concentration) | `Fulfill` | `Account Balance Sweeping` | `Account Balance Sweeping Facility` | Operations and Execution › Product Specific Fulfillment › Trade Banking |
| 47 | [Cash Management And Account Services](03_Operations_and_Execution.md#cash-management-and-account-services) | `Fulfill` | `Cash Management And Account Services` | `Cash Management And Account Services Facility` | Operations and Execution › Product Specific Fulfillment › Trade Banking |
| 48 | [Central Cash Handling](03_Operations_and_Execution.md#central-cash-handling) | `Allocate` | `Central Cash` | `Central Cash Allocation` | Operations and Execution › Cross Product Operations › Payments |
| 49 | [Channel Activity Analysis](03_Operations_and_Execution.md#channel-activity-analysis) | `Analyze` | `Channel Activity` | `Channel Activity Analysis` | Operations and Execution › Cross Product Operations › Operational Services |
| 50 | [Channel Activity History](03_Operations_and_Execution.md#channel-activity-history) | `Track` | `Channel Activity` | `Channel Activity Log` | Operations and Execution › Cross Product Operations › Operational Services |
| 51 | [Channel Portfolio](04_Risk_and_Compliance.md#channel-portfolio) | `Analyze` | `Channel Portfolio` | `Channel Portfolio Analysis` | Risk and Compliance › Business Analysis |
| 52 | [Cheque Lock Box](03_Operations_and_Execution.md#cheque-lock-box) | `Fulfill` | `Lock Box` | `Lock Box Facility` | Operations and Execution › Product Specific Fulfillment › Trade Banking |
| 53 | [Cheque Processing](03_Operations_and_Execution.md#cheque-processing) | `Operate` | `Cheque Processing` | `Cheque Processing Operating Session` | Operations and Execution › Cross Product Operations › Payments |
| 54 | [Claim Administration](03_Operations_and_Execution.md#claim-administration) | `Administer` | `Claim Processing` | `Claim Processing Administrative Plan` | Operations and Execution › Product Specific Fulfillment › Consumer Services |
| 55 | [Claim Assessment](03_Operations_and_Execution.md#claim-assessment) | `Assess` | `Claim Validation` | `Claim Validation Assessment` | Operations and Execution › Product Specific Fulfillment › Consumer Services |
| 56 | [Collateral Allocation Management](03_Operations_and_Execution.md#collateral-allocation-management) | `Allocate` | `Collateral Asset` | `Collateral Asset Allocation` | Operations and Execution › Cross Product Operations › Collateral Administration |
| 57 | [Collateral Asset Administration](03_Operations_and_Execution.md#collateral-asset-administration) | `Administer` | `Collateral Asset` | `Collateral Asset Administrative Plan` | Operations and Execution › Cross Product Operations › Collateral Administration |
| 58 | [Collections](03_Operations_and_Execution.md#collections) | `Process` | `Collateral Asset Liquidation` | `Collateral Asset Liquidation Procedure` | Operations and Execution › Cross Product Operations › Collateral Administration |
| 59 | [Commission Agreement](01_Sales_and_Service.md#commission-agreement) | `Agree Terms` | `Employee Commission` | `Employee Commission Agreement` | Sales and Service › Sales |
| 60 | [Commissions](01_Sales_and_Service.md#commissions) | `Transact` | `Commission` | `Commission Transaction` | Sales and Service › Sales |
| 61 | [Company Billing and Payments](05_Business_Support.md#company-billing-and-payments) | `Process` | `Enterprise Billing And Payments` | `Enterprise Billing And Payments Procedure` | Business Support › Non-IT and Non-HR Enterprise Services |
| 62 | [Competitor Analysis](04_Risk_and_Compliance.md#competitor-analysis) | `Analyze` | `Competitor` | `Competitor Analysis` | Risk and Compliance › Business Analysis |
| 63 | [Compliance Reporting](04_Risk_and_Compliance.md#compliance-reporting) | `Administer` | `Compliance Reporting` | `Compliance Reporting Administrative Plan` | Risk and Compliance › Regulations and Compliance |
| 64 | [Consumer Advisory Services](03_Operations_and_Execution.md#consumer-advisory-services) | `Advise` | `Consumer Advice` | `Consumer Advice` | Operations and Execution › Product Specific Fulfillment › Consumer Services |
| 65 | [Consumer Investments](03_Operations_and_Execution.md#consumer-investments) | `Transact` | `Consumer Securities Order` | `Consumer Securities Order Transaction` | Operations and Execution › Product Specific Fulfillment › Consumer Services |
| 66 | [Consumer Loan](03_Operations_and_Execution.md#consumer-loan) | `Fulfill` | `Consumer Loan` | `Consumer Loan Facility` | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |
| 67 | [Contact Center Management](01_Sales_and_Service.md#contact-center-management) | `Manage` | `Contact Center` | `Contact Center Management Plan` | Sales and Service › Channel Specific |
| 68 | [Contact Center Operations](01_Sales_and_Service.md#contact-center-operations) | `Administer` | `Contact Center` | `Contact Center Administrative Plan` | Sales and Service › Channel Specific |
| 69 | [Contact Handler](01_Sales_and_Service.md#contact-handler) | `Operate` | `Customer Contact` | `Customer Contact Operating Session` | Sales and Service › Cross Channel |
| 70 | [Contact Routing](01_Sales_and_Service.md#contact-routing) | `Allocate` | `Customer Servicing Resource` | `Customer Servicing Resource Allocation` | Sales and Service › Cross Channel |
| 71 | [Continuity Planning](05_Business_Support.md#continuity-planning) | `Manage` | `Enterprise Continuity Assurance` | `Enterprise Continuity Assurance Management Plan` | Business Support › Business Direction |
| 72 | [Contractor and Supplier Agreement](02_Reference_Data.md#contractor-and-supplier-agreement) | `Agree Terms` | `Supplier` | `Supplier Agreement` | Reference Data › External Agency |
| 73 | [Contribution Analysis](04_Risk_and_Compliance.md#contribution-analysis) | `Analyze` | `Contribution` | `Contribution Analysis` | Risk and Compliance › Business Analysis |
| 74 | [Contribution Models](04_Risk_and_Compliance.md#contribution-models) | `Design` | `Contribution Model` | `Contribution Model Specification` | Risk and Compliance › Models |
| 75 | [Corporate Action](03_Operations_and_Execution.md#corporate-action) | `Process` | `Corporate Action` | `Corporate Action Procedure` | Operations and Execution › Product Specific Fulfillment › Market Operations |
| 76 | [Corporate Alliance and Stake Holder](05_Business_Support.md#corporate-alliance-and-stake-holder) | `Manage` | `Alliance Partner Relationship` | `Alliance Partner Relationship Management Plan` | Business Support › Corporate Relations |
| 77 | [Corporate Card Service](03_Operations_and_Execution.md#corporate-card-service) | `Fulfill` | `Corporate Card` | `Corporate Card Facility` | Operations and Execution › Product Specific Fulfillment › Cards |
| 78 | [Corporate Communications](05_Business_Support.md#corporate-communications) | `Manage` | `Enterprise Communication` | `Enterprise Communication Management Plan` | Business Support › Corporate Relations |
| 79 | [Corporate Current Account](03_Operations_and_Execution.md#corporate-current-account) | `Fulfill` | `Corporate Current Account` | `Corporate Current Account Facility` | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |
| 80 | [Corporate Finance](03_Operations_and_Execution.md#corporate-finance) | `Advise` | `Corporate Finance Services` | `Corporate Finance Services Advice` | Operations and Execution › Product Specific Fulfillment › Corporate Financing and Advisory Services |
| 81 | [Corporate Lease](03_Operations_and_Execution.md#corporate-lease) | `Fulfill` | `Corporate Lease` | `Corporate Lease Facility` | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |
| 82 | [Corporate Loan](03_Operations_and_Execution.md#corporate-loan) | `Fulfill` | `Corporate Loan` | `Corporate Loan Facility` | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |
| 83 | [Corporate Payroll Services](03_Operations_and_Execution.md#corporate-payroll-services) | `Fulfill` | `Employee Payment Services` | `Employee Payment Services Facility` | Operations and Execution › Product Specific Fulfillment › Trade Banking |
| 84 | [Corporate Policies](05_Business_Support.md#corporate-policies) | `Design` | `Corporate Policy` | `Corporate Policy Specification` | Business Support › Business Direction |
| 85 | [Corporate Relationship](05_Business_Support.md#corporate-relationship) | `Manage` | `Corporate Partner Relationship` | `Corporate Partner Relationship Management Plan` | Business Support › Corporate Relations |
| 86 | [Corporate Strategy](05_Business_Support.md#corporate-strategy) | `Direct` | `Enterprise` | `Enterprise Strategy` | Business Support › Business Direction |
| 87 | [Corporate Tax Advisory](03_Operations_and_Execution.md#corporate-tax-advisory) | `Advise` | `Corporate Tax Advice` | `Corporate Tax Advice` | Operations and Execution › Product Specific Fulfillment › Corporate Financing and Advisory Services |
| 88 | [Corporate Treasury](04_Risk_and_Compliance.md#corporate-treasury) | `Manage` | `Corporate Treasury` | `Corporate Treasury Management Plan` | Risk and Compliance › Bank Portfolio and Treasury |
| 89 | [Corporate Treasury Analysis](04_Risk_and_Compliance.md#corporate-treasury-analysis) | `Analyze` | `Corporate Treasury` | `Corporate Treasury Analysis` | Risk and Compliance › Bank Portfolio and Treasury |
| 90 | [Corporate Trust Services](03_Operations_and_Execution.md#corporate-trust-services) | `Fulfill` | `Corporate Trust Services` | `Corporate Trust Services Facility` | Operations and Execution › Product Specific Fulfillment › Consumer Services |
| 91 | [Correspondence](05_Business_Support.md#correspondence) | `Operate` | `Correspondence` | `Correspondence Operating Session` | Business Support › Document Management and Archive |
| 92 | [Correspondent Bank Directory](02_Reference_Data.md#correspondent-bank-directory) | `Catalog` | `Correspondent Bank` | `Correspondent Bank Directory Entry` | Reference Data › External Agency |
| 93 | [Correspondent Bank Relationship Management](02_Reference_Data.md#correspondent-bank-relationship-management) | `Manage` | `Correpondent Bank Relationship` | `Correpondent Bank Relationship Management Plan` | Reference Data › External Agency |
| 94 | [Counterparty Administration](02_Reference_Data.md#counterparty-administration) | `Catalog` | `Counterparty` | `Counterparty Directory Entry` | Reference Data › Market Data |
| 95 | [Counterparty Risk](03_Operations_and_Execution.md#counterparty-risk) | `Monitor` | `Counterparty Credit Risk` | `Counterparty Credit Risk Measurement` | Operations and Execution › Cross Product Operations › Account Management |
| 96 | [Credit Card](03_Operations_and_Execution.md#credit-card) | `Fulfill` | `Credit Card` | `Credit Card Facility` | Operations and Execution › Product Specific Fulfillment › Cards |
| 97 | [Credit Facility](03_Operations_and_Execution.md#credit-facility) | `Fulfill` | `Credit Line` | `Credit Line Facility` | Operations and Execution › Product Specific Fulfillment › Trade Banking |
| 98 | [Credit Management](03_Operations_and_Execution.md#credit-management) | `Assess` | `Credit Pricing` | `Credit Pricing Assessment` | Operations and Execution › Product Specific Fulfillment › Trade Banking |
| 99 | [Credit Risk Models](04_Risk_and_Compliance.md#credit-risk-models) | `Design` | `Credit Risk Model` | `Credit Risk Model Specification` | Risk and Compliance › Models |
| 100 | [Credit Risk Operations](03_Operations_and_Execution.md#credit-risk-operations) | `Monitor` | `Trading Credit Position` | `Trading Credit Position Measurement` | Operations and Execution › Product Specific Fulfillment › Wholesale Trading |
| 101 | [Credit and Margin Management](04_Risk_and_Compliance.md#credit-and-margin-management) | `Direct` | `Credit And Margins` | `Credit And Margins Strategy` | Risk and Compliance › Models |
| 102 | [Currency Exchange](03_Operations_and_Execution.md#currency-exchange) | `Transact` | `Currency Exchange` | `Currency Exchange Transaction` | Operations and Execution › Product Specific Fulfillment › Consumer Services |
| 103 | [Current Account](03_Operations_and_Execution.md#current-account) | `Fulfill` | `Current Account` | `Current Account Facility` | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |
| 104 | [Custody Administration](03_Operations_and_Execution.md#custody-administration) | `Fulfill` | `Custody` | `Custody Facility` | Operations and Execution › Product Specific Fulfillment › Market Operations |
| 105 | [Customer Access Entitlement](01_Sales_and_Service.md#customer-access-entitlement) | `Agree Terms` | `Customer Access Profile` | `Customer Access Profile Agreement` | Sales and Service › Customer Management |
| 106 | [Customer Agreement](01_Sales_and_Service.md#customer-agreement) | `Agree Terms` | `Customer` | `Customer Agreement` | Sales and Service › Customer Management |
| 107 | [Customer Behavior Insights](01_Sales_and_Service.md#customer-behavior-insights) | `Analyze` | `Customer Behavior` | `Customer Behavior Analysis` | Sales and Service › Customer Management |
| 108 | [Customer Behavior Models](04_Risk_and_Compliance.md#customer-behavior-models) | `Design` | `Customer Behavior Model` | `Customer Behavior Model Specification` | Risk and Compliance › Models |
| 109 | [Customer Billing](03_Operations_and_Execution.md#customer-billing) | `Process` | `Customer Billing` | `Customer Billing Procedure` | Operations and Execution › Cross Product Operations › Operational Services |
| 110 | [Customer Campaign Design](01_Sales_and_Service.md#customer-campaign-design) | `Design` | `Customer Campaign` | `Customer Campaign Specification` | Sales and Service › Marketing |
| 111 | [Customer Campaign Execution](01_Sales_and_Service.md#customer-campaign-execution) | `Process` | `Customer Campaign` | `Customer Campaign Procedure` | Sales and Service › Sales |
| 112 | [Customer Campaign Management](01_Sales_and_Service.md#customer-campaign-management) | `Manage` | `Customer Campaign Portfolio` | `Customer Campaign Portfolio Management Plan` | Sales and Service › Marketing |
| 113 | [Customer Case](01_Sales_and_Service.md#customer-case) | `Process` | `Customer Case` | `Customer Case Procedure` | Sales and Service › Servicing |
| 114 | [Customer Case Management](01_Sales_and_Service.md#customer-case-management) | `Manage` | `Customer Case` | `Customer Case Management Plan` | Sales and Service › Servicing |
| 115 | [Customer Consent](01_Sales_and_Service.md#customer-consent) | `Agree Terms` | `Customer Mandate` | `Customer Mandate Agreement` | Sales and Service › Customer Management |
| 116 | [Customer Credit Rating](01_Sales_and_Service.md#customer-credit-rating) | `Monitor` | `Customer Credit Rating` | `Customer Credit Rating State` | Sales and Service › Customer Management |
| 117 | [Customer Event History](01_Sales_and_Service.md#customer-event-history) | `Track` | `Customer Event` | `Customer Event Log` | Sales and Service › Customer Management |
| 118 | [Customer Financial Insights](01_Sales_and_Service.md#customer-financial-insights) | `Analyze` | `Customer Financial Position` | `Customer Financial Position Analysis` | Sales and Service › Customer Management |
| 119 | [Customer Offer](01_Sales_and_Service.md#customer-offer) | `Process` | `Customer Offer` | `Customer Offer Procedure` | Sales and Service › Sales |
| 120 | [Customer Portfolio](04_Risk_and_Compliance.md#customer-portfolio) | `Analyze` | `Customer Portfolio` | `Customer Portfolio Analysis` | Risk and Compliance › Business Analysis |
| 121 | [Customer Position](03_Operations_and_Execution.md#customer-position) | `Monitor` | `Customer Position` | `Customer Position State` | Operations and Execution › Cross Product Operations › Account Management |
| 122 | [Customer Product And Service Eligibility](01_Sales_and_Service.md#customer-product-and-service-eligibility) | `Assess` | `Customer Eligibility` | `Customer Eligibility Assessment` | Sales and Service › Customer Management |
| 123 | [Customer Product and Service Directory](01_Sales_and_Service.md#customer-product-and-service-directory) | `Catalog` | `Customer Product And Service` | `Customer Product And Service Directory Entry` | Sales and Service › Customer Management |
| 124 | [Customer Proposition](01_Sales_and_Service.md#customer-proposition) | `Agree Terms` | `Customer Proposition` | `Customer Proposition Agreement` | Sales and Service › Customer Management |
| 125 | [Customer Relationship Management](01_Sales_and_Service.md#customer-relationship-management) | `Manage` | `Customer Relationship` | `Customer Relationship Management Plan` | Sales and Service › Customer Management |
| 126 | [Customer Surveys](01_Sales_and_Service.md#customer-surveys) | `Process` | `Customer Survey` | `Customer Survey Procedure` | Sales and Service › Marketing |
| 127 | [Customer Tax Handling](03_Operations_and_Execution.md#customer-tax-handling) | `Fulfill` | `Customer Tax Obligation` | `Customer Tax Obligation Facility` | Operations and Execution › Product Specific Fulfillment › Consumer Services |
| 128 | [Customer Workbench](01_Sales_and_Service.md#customer-workbench) | `Operate` | `Customer Workbench` | `Customer Workbench Operating Session` | Sales and Service › Cross Channel |
| 129 | [Dealer Desk](03_Operations_and_Execution.md#dealer-desk) | `Operate` | `Dealer Desk` | `Dealer Desk Operating Session` | Operations and Execution › Product Specific Fulfillment › Wholesale Trading |
| 130 | [Delinquent Account Handling](03_Operations_and_Execution.md#delinquent-account-handling) | `Process` | `Delinquent Account` | `Delinquent Account Procedure` | Operations and Execution › Cross Product Operations › Operational Services |
| 131 | [Development Environment](05_Business_Support.md#development-environment) | `Administer` | `Development Environment` | `Development Environment Administrative Plan` | Business Support › IT Management |
| 132 | [Direct Debit](03_Operations_and_Execution.md#direct-debit) | `Fulfill` | `Direct Debit` | `Direct Debit Facility` | Operations and Execution › Product Specific Fulfillment › Trade Banking |
| 133 | [Direct Debit Mandate](03_Operations_and_Execution.md#direct-debit-mandate) | `Catalog` | `Direct Debit Mandate` | `Direct Debit Mandate Directory Entry` | Operations and Execution › Product Specific Fulfillment › Trade Banking |
| 134 | [Disbursement](03_Operations_and_Execution.md#disbursement) | `Transact` | `Disbursement` | `Disbursement Transaction` | Operations and Execution › Cross Product Operations › Operational Services |
| 135 | [Discount Pricing](02_Reference_Data.md#discount-pricing) | `Assess` | `Productand Service Discount` | `Productand Service Discount Assessment` | Reference Data › Product Management |
| 136 | [Document Directory](05_Business_Support.md#document-directory) | `Catalog` | `Document` | `Document Directory Entry` | Business Support › Document Management and Archive |
| 137 | [Document Services](05_Business_Support.md#document-services) | `Process` | `Document Service` | `Document Service Procedure` | Business Support › Document Management and Archive |
| 138 | [ECM And DCM](03_Operations_and_Execution.md#ecm-and-dcm) | `Fulfill` | `ECM And DCM` | `ECM And DCM Facility` | Operations and Execution › Product Specific Fulfillment › Wholesale Trading |
| 139 | [Economic Capital](04_Risk_and_Compliance.md#economic-capital) | `Analyze` | `Economic Capital` | `Economic Capital Analysis` | Risk and Compliance › Models |
| 140 | [Employee Access](05_Business_Support.md#employee-access) | `Assess` | `Employee Access` | `Employee Access Assessment` | Business Support › Human Resource Management |
| 141 | [Employee Assignment](05_Business_Support.md#employee-assignment) | `Allocate` | `Employee` | `Employee Allocation` | Business Support › Human Resource Management |
| 142 | [Employee Benefits](05_Business_Support.md#employee-benefits) | `Administer` | `Employee Benefits` | `Employee Benefits Administrative Plan` | Business Support › Human Resource Management |
| 143 | [Employee Certification](05_Business_Support.md#employee-certification) | `Assess` | `Employee Certification` | `Employee Certification Assessment` | Business Support › Human Resource Management |
| 144 | [Employee Data Management](05_Business_Support.md#employee-data-management) | `Catalog` | `Employee` | `Employee Directory Entry` | Business Support › Human Resource Management |
| 145 | [Employee Evaluation](05_Business_Support.md#employee-evaluation) | `Analyze` | `Employee` | `Employee Analysis` | Business Support › Human Resource Management |
| 146 | [Employee Payroll And Incentives](05_Business_Support.md#employee-payroll-and-incentives) | `Process` | `Employee Payroll` | `Employee Payroll Procedure` | Business Support › Human Resource Management |
| 147 | [Employee and Contractor Contract](05_Business_Support.md#employee-and-contractor-contract) | `Agree Terms` | `Employee` | `Employee Agreement` | Business Support › Human Resource Management |
| 148 | [Enterprise Architecture](05_Business_Support.md#enterprise-architecture) | `Design` | `Enterprise Architecture` | `Enterprise Architecture Specification` | Business Support › Business Direction |
| 149 | [Enterprise Tax Administration](05_Business_Support.md#enterprise-tax-administration) | `Manage` | `Tax Administration` | `Tax Administration Management Plan` | Business Support › Finance |
| 150 | [Equipment Administration](05_Business_Support.md#equipment-administration) | `Administer` | `Office Equipment` | `Office Equipment Administrative Plan` | Business Support › Buildings Equipment and Facilities |
| 151 | [Equipment Maintenance](05_Business_Support.md#equipment-maintenance) | `Maintain` | `Office Equipment` | `Office Equipment Maintenance Arrangement` | Business Support › Buildings Equipment and Facilities |
| 152 | [Factoring](03_Operations_and_Execution.md#factoring) | `Fulfill` | `Factoring` | `Factoring Facility` | Operations and Execution › Product Specific Fulfillment › Trade Banking |
| 153 | [Fiduciary Agreement](03_Operations_and_Execution.md#fiduciary-agreement) | `Agree Terms` | `Fiduciary Relationship` | `Fiduciary Relationship Agreement` | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |
| 154 | [Financial Accounting](04_Risk_and_Compliance.md#financial-accounting) | `Track` | `Financial Booking` | `Financial Booking Log` | Risk and Compliance › Regulations and Compliance |
| 155 | [Financial Compliance](05_Business_Support.md#financial-compliance) | `Process` | `Financial Compliance` | `Financial Compliance Procedure` | Business Support › Finance |
| 156 | [Financial Control](05_Business_Support.md#financial-control) | `Assess` | `Financial Control` | `Financial Control Assessment` | Business Support › Finance |
| 157 | [Financial Gateway](03_Operations_and_Execution.md#financial-gateway) | `Operate` | `Financial Gateway` | `Financial Gateway Operating Session` | Operations and Execution › Cross Product Operations › Payments |
| 158 | [Financial Instrument Reference Data Management](02_Reference_Data.md#financial-instrument-reference-data-management) | `Catalog` | `Financial Instrument` | `Financial Instrument Directory Entry` | Reference Data › Market Data |
| 159 | [Financial Instrument Valuation](03_Operations_and_Execution.md#financial-instrument-valuation) | `Process` | `Market Asset Valuation` | `Market Asset Valuation Procedure` | Operations and Execution › Product Specific Fulfillment › Market Operations |
| 160 | [Financial Instrument Valuation Models](04_Risk_and_Compliance.md#financial-instrument-valuation-models) | `Design` | `Market Asset Valuation Model` | `Market Asset Valuation Model Specification` | Risk and Compliance › Models |
| 161 | [Financial Market Analysis](02_Reference_Data.md#financial-market-analysis) | `Analyze` | `Financial Market` | `Financial Market Analysis` | Reference Data › Market Data |
| 162 | [Financial Market Research](02_Reference_Data.md#financial-market-research) | `Catalog` | `Financial Market Research` | `Financial Market Research Directory Entry` | Reference Data › Market Data |
| 163 | [Financial Message Analysis](03_Operations_and_Execution.md#financial-message-analysis) | `Analyze` | `Financial Network Gateway` | `Financial Network Gateway Analysis` | Operations and Execution › Cross Product Operations › Payments |
| 164 | [Financial Statement Assessment](04_Risk_and_Compliance.md#financial-statement-assessment) | `Assess` | `Financial Statement` | `Financial Statement Assessment` | Risk and Compliance › Regulations and Compliance |
| 165 | [Financial Statements](05_Business_Support.md#financial-statements) | `Analyze` | `Financial Statements` | `Financial Statements Analysis` | Business Support › Finance |
| 166 | [Fixed Asset Register](05_Business_Support.md#fixed-asset-register) | `Administer` | `Fixed Asset Register` | `Fixed Asset Register Administrative Plan` | Business Support › Non-IT and Non-HR Enterprise Services |
| 167 | [Fraud Diagnosis](03_Operations_and_Execution.md#fraud-diagnosis) | `Analyze` | `Fraud Diagnosis` | `Fraud Diagnosis Analysis` | Operations and Execution › Cross Product Operations › Account Management |
| 168 | [Fraud Evaluation](03_Operations_and_Execution.md#fraud-evaluation) | `Assess` | `Fraud Evaluation` | `Fraud Evaluation Assessment` | Operations and Execution › Cross Product Operations › Account Management |
| 169 | [Fraud Model](04_Risk_and_Compliance.md#fraud-model) | `Design` | `Fraud Model` | `Fraud Model Specification` | Risk and Compliance › Models |
| 170 | [Fraud Resolution](04_Risk_and_Compliance.md#fraud-resolution) | `Process` | `Fraud Resolution` | `Fraud Resolution Procedure` | Risk and Compliance › Regulations and Compliance |
| 171 | [Funeral Policy](03_Operations_and_Execution.md#funeral-policy) | `Fulfill` | `Funeral Policy` | `Funeral Policy Facility` | Operations and Execution › Product Specific Fulfillment › Consumer Services |
| 172 | [Gap Analysis](04_Risk_and_Compliance.md#gap-analysis) | `Analyze` | `interest Rate Gap Risk` | `interest Rate Gap Risk Analysis` | Risk and Compliance › Models |
| 173 | [Guideline Compliance](04_Risk_and_Compliance.md#guideline-compliance) | `Assess` | `Guideline Compliance` | `Guideline Compliance Assessment` | Risk and Compliance › Regulations and Compliance |
| 174 | [Hedge Fund Administration](03_Operations_and_Execution.md#hedge-fund-administration) | `Administer` | `Hedge Fund` | `Hedge Fund Administrative Plan` | Operations and Execution › Product Specific Fulfillment › Market Operations |
| 175 | [Human Resources Direction](05_Business_Support.md#human-resources-direction) | `Direct` | `Human Resources` | `Human Resources Strategy` | Business Support › Human Resource Management |
| 176 | [IT Standards And Guidelines](05_Business_Support.md#it-standards-and-guidelines) | `Design` | `Technology Standards` | `Technology Standards Specification` | Business Support › IT Management |
| 177 | [IT Systems Direction](05_Business_Support.md#it-systems-direction) | `Direct` | `IT Systems` | `IT Systems Strategy` | Business Support › IT Management |
| 178 | [Incentive Account](03_Operations_and_Execution.md#incentive-account) | `Fulfill` | `Incentive Account` | `Incentive Account Facility` | Operations and Execution › Cross Product Operations › Operational Services |
| 179 | [Incentive Program Directory](03_Operations_and_Execution.md#incentive-program-directory) | `Catalog` | `Incentive Program` | `Incentive Program Directory Entry` | Operations and Execution › Cross Product Operations › Operational Services |
| 180 | [Information Provider Administration](02_Reference_Data.md#information-provider-administration) | `Agree Terms` | `Information Feed` | `Information Feed Agreement` | Reference Data › External Agency |
| 181 | [Information Provider Operation](02_Reference_Data.md#information-provider-operation) | `Operate` | `Information Feed` | `Information Feed Operating Session` | Reference Data › Market Data |
| 182 | [Intellectual Property Portfolio](05_Business_Support.md#intellectual-property-portfolio) | `Administer` | `Intellectual Property` | `Intellectual Property Administrative Plan` | Business Support › Knowledge and Intellectual Property Management |
| 183 | [Interactive Help](01_Sales_and_Service.md#interactive-help) | `Operate` | `interactive Help Service` | `interactive Help Service Operating Session` | Sales and Service › Cross Channel |
| 184 | [Interbank Relationship Management](02_Reference_Data.md#interbank-relationship-management) | `Manage` | `Bank Relationship` | `Bank Relationship Management Plan` | Reference Data › External Agency |
| 185 | [Internal Audit](05_Business_Support.md#internal-audit) | `Assess` | `Internal Audit` | `Internal Audit Assessment` | Business Support › Non-IT and Non-HR Enterprise Services |
| 186 | [Internal Bank Account](03_Operations_and_Execution.md#internal-bank-account) | `Fulfill` | `Internal Bank Account` | `Internal Bank Account Facility` | Operations and Execution › Cross Product Operations › Operational Services |
| 187 | [Internal Network Operation](05_Business_Support.md#internal-network-operation) | `Operate` | `Internal Network` | `Internal Network Operating Session` | Business Support › IT Management |
| 188 | [Investment Account](03_Operations_and_Execution.md#investment-account) | `Fulfill` | `Investment Account` | `Investment Account Facility` | Operations and Execution › Product Specific Fulfillment › Investment Management |
| 189 | [Investment Portfolio Analysis](03_Operations_and_Execution.md#investment-portfolio-analysis) | `Analyze` | `Managed Investment Portfolio` | `Managed Investment Portfolio Analysis` | Operations and Execution › Product Specific Fulfillment › Investment Management |
| 190 | [Investment Portfolio Management](03_Operations_and_Execution.md#investment-portfolio-management) | `Fulfill` | `Managed Investment Portfolio` | `Managed Investment Portfolio Facility` | Operations and Execution › Product Specific Fulfillment › Investment Management |
| 191 | [Investment Portfolio Planning](03_Operations_and_Execution.md#investment-portfolio-planning) | `Agree Terms` | `Managed Investment Portfolio` | `Managed Investment Portfolio Agreement` | Operations and Execution › Product Specific Fulfillment › Investment Management |
| 192 | [Investor Relations](05_Business_Support.md#investor-relations) | `Enroll` | `Investor` | `Investor Membership` | Business Support › Corporate Relations |
| 193 | [Issued Certificate Directory](03_Operations_and_Execution.md#issued-certificate-directory) | `Catalog` | `Issued Certificate` | `Issued Certificate Directory Entry` | Operations and Execution › Cross Product Operations › Operational Services |
| 194 | [Issued Device Administration](03_Operations_and_Execution.md#issued-device-administration) | `Allocate` | `Issued Device` | `Issued Device Allocation` | Operations and Execution › Cross Product Operations › Operational Services |
| 195 | [Issued Device Tracking](03_Operations_and_Execution.md#issued-device-tracking) | `Monitor` | `Issued Device` | `Issued Device State` | Operations and Execution › Cross Product Operations › Operational Services |
| 196 | [Knowledge Exchange](05_Business_Support.md#knowledge-exchange) | `Operate` | `Intellectual Property Exchange` | `Intellectual Property Exchange Operating Session` | Business Support › Knowledge and Intellectual Property Management |
| 197 | [Lead and Opportunity Management](01_Sales_and_Service.md#lead-and-opportunity-management) | `Process` | `Leadand Opportunity` | `Leadand Opportunity Procedure` | Sales and Service › Sales |
| 198 | [Leasing](03_Operations_and_Execution.md#leasing) | `Fulfill` | `Leasing` | `Leasing Facility` | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |
| 199 | [Leasing Item Administration](03_Operations_and_Execution.md#leasing-item-administration) | `Administer` | `Leasing Item` | `Leasing Item Administrative Plan` | Operations and Execution › Cross Product Operations › Operational Services |
| 200 | [Legal Advisory](05_Business_Support.md#legal-advisory) | `Advise` | `Legal Advice` | `Legal Advice` | Business Support › Non-IT and Non-HR Enterprise Services |
| 201 | [Legal Compliance](05_Business_Support.md#legal-compliance) | `Assess` | `Legal Compliance` | `Legal Compliance Assessment` | Business Support › Non-IT and Non-HR Enterprise Services |
| 202 | [Legal Entity Directory](02_Reference_Data.md#legal-entity-directory) | `Catalog` | `Legal Entity` | `Legal Entity Directory Entry` | Reference Data › Party |
| 203 | [Letter of Credit](03_Operations_and_Execution.md#letter-of-credit) | `Transact` | `Letter Of Credit` | `Letter Of Credit Transaction` | Operations and Execution › Product Specific Fulfillment › Trade Banking |
| 204 | [Limit and Exposure Management](03_Operations_and_Execution.md#limit-and-exposure-management) | `Manage` | `Limit And Exposure` | `Limit And Exposure Management Plan` | Operations and Execution › Product Specific Fulfillment › Trade Banking |
| 205 | [Liquidity Risk Models](04_Risk_and_Compliance.md#liquidity-risk-models) | `Design` | `Liquidity Risk Model` | `Liquidity Risk Model Specification` | Risk and Compliance › Models |
| 206 | [Loan](03_Operations_and_Execution.md#loan) | `Fulfill` | `Loan` | `Loan Facility` | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |
| 207 | [Loan Syndication](01_Sales_and_Service.md#loan-syndication) | `Process` | `Syndicated Loan Application` | `Syndicated Loan Application Procedure` | Sales and Service › Servicing |
| 208 | [Location Data Management](02_Reference_Data.md#location-data-management) | `Catalog` | `Location` | `Location Directory Entry` | Reference Data › Market Data |
| 209 | [Management Manual](05_Business_Support.md#management-manual) | `Design` | `Management Manual` | `Management Manual Specification` | Business Support › Knowledge and Intellectual Property Management |
| 210 | [Market Analysis](04_Risk_and_Compliance.md#market-analysis) | `Analyze` | `General Market Research` | `General Market Research Analysis` | Risk and Compliance › Business Analysis |
| 211 | [Market Data Switch Administration](02_Reference_Data.md#market-data-switch-administration) | `Administer` | `Information Feed Switch` | `Information Feed Switch Administrative Plan` | Reference Data › Market Data |
| 212 | [Market Data Switch Operation](02_Reference_Data.md#market-data-switch-operation) | `Operate` | `Information Feed Switch` | `Information Feed Switch Operating Session` | Reference Data › Market Data |
| 213 | [Market Information Management](02_Reference_Data.md#market-information-management) | `Administer` | `Financial Market Information` | `Financial Market Information Administrative Plan` | Reference Data › Market Data |
| 214 | [Market Making](03_Operations_and_Execution.md#market-making) | `Fulfill` | `Market Making` | `Market Making Facility` | Operations and Execution › Product Specific Fulfillment › Wholesale Trading |
| 215 | [Market Order](03_Operations_and_Execution.md#market-order) | `Transact` | `Market Order` | `Market Order Transaction` | Operations and Execution › Product Specific Fulfillment › Wholesale Trading |
| 216 | [Market Order Execution](03_Operations_and_Execution.md#market-order-execution) | `Transact` | `Market Trade` | `Market Trade Transaction` | Operations and Execution › Product Specific Fulfillment › Wholesale Trading |
| 217 | [Market Research](04_Risk_and_Compliance.md#market-research) | `Catalog` | `General Market Research` | `General Market Research Directory Entry` | Risk and Compliance › Business Analysis |
| 218 | [Market Risk Models](04_Risk_and_Compliance.md#market-risk-models) | `Design` | `Market Risk Model` | `Market Risk Model Specification` | Risk and Compliance › Models |
| 219 | [Merchandising Loan](03_Operations_and_Execution.md#merchandising-loan) | `Fulfill` | `Merchandising Loan` | `Merchandising Loan Facility` | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |
| 220 | [Merchant Acquiring Facility](03_Operations_and_Execution.md#merchant-acquiring-facility) | `Fulfill` | `Merchant Acquiring` | `Merchant Acquiring Facility` | Operations and Execution › Product Specific Fulfillment › Cards |
| 221 | [Merchant Relations](03_Operations_and_Execution.md#merchant-relations) | `Agree Terms` | `Merchant Relationship` | `Merchant Relationship Agreement` | Operations and Execution › Product Specific Fulfillment › Cards |
| 222 | [Mergers and Acquisitions Advisory](03_Operations_and_Execution.md#mergers-and-acquisitions-advisory) | `Advise` | `Mergers And Acquisition` | `Mergers And Acquisition Advice` | Operations and Execution › Product Specific Fulfillment › Corporate Financing and Advisory Services |
| 223 | [Mortgage Loan](03_Operations_and_Execution.md#mortgage-loan) | `Fulfill` | `Mortgage Loan` | `Mortgage Loan Facility` | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |
| 224 | [Mutual Fund Administration](03_Operations_and_Execution.md#mutual-fund-administration) | `Administer` | `Mutual Fund` | `Mutual Fund Administrative Plan` | Operations and Execution › Product Specific Fulfillment › Market Operations |
| 225 | [Notional Pooling](03_Operations_and_Execution.md#notional-pooling) | `Fulfill` | `Notional Pooling` | `Notional Pooling Facility` | Operations and Execution › Product Specific Fulfillment › Trade Banking |
| 226 | [Open Item Management](03_Operations_and_Execution.md#open-item-management) | `Process` | `Open Item` | `Open Item Procedure` | Operations and Execution › Cross Product Operations › Operational Services |
| 227 | [Operational Gateway](05_Business_Support.md#operational-gateway) | `Operate` | `Operational Gateway` | `Operational Gateway Operating Session` | Business Support › IT Management |
| 228 | [Operational Risk Models](04_Risk_and_Compliance.md#operational-risk-models) | `Design` | `Opertional Risk Model` | `Opertional Risk Model Specification` | Risk and Compliance › Models |
| 229 | [Operations Log](02_Reference_Data.md#operations-log) | `Track` | `Partner Event` | `Partner Event Log` | Reference Data › External Agency |
| 230 | [Order Allocation](03_Operations_and_Execution.md#order-allocation) | `Process` | `Securities Allocation` | `Securities Allocation Procedure` | Operations and Execution › Product Specific Fulfillment › Market Operations |
| 231 | [Organization Direction](05_Business_Support.md#organization-direction) | `Direct` | `Organization` | `Organization Strategy` | Business Support › Business Command and Control |
| 232 | [Partner Administration](02_Reference_Data.md#partner-administration) | `Administer` | `Partner` | `Partner Administrative Plan` | Reference Data › External Agency |
| 233 | [Partner Agreement](02_Reference_Data.md#partner-agreement) | `Agree Terms` | `Partner` | `Partner Agreement` | Reference Data › External Agency |
| 234 | [Partner Management](02_Reference_Data.md#partner-management) | `Manage` | `Partner Releationship` | `Partner Releationship Management Plan` | Reference Data › External Agency |
| 235 | [Party Asset Directory](03_Operations_and_Execution.md#party-asset-directory) | `Catalog` | `Party Asset` | `Party Asset Directory Entry` | Operations and Execution › Cross Product Operations › Collateral Administration |
| 236 | [Party Authentication](01_Sales_and_Service.md#party-authentication) | `Assess` | `Party Authentication` | `Party Authentication Assessment` | Sales and Service › Cross Channel |
| 237 | [Party Lifecycle Management](01_Sales_and_Service.md#party-lifecycle-management) | `Administer` | `Party Relationship` | `Party Relationship Administrative Plan` | Sales and Service › Sales |
| 238 | [Party Reference Data Directory](01_Sales_and_Service.md#party-reference-data-directory) | `Catalog` | `Party Reference Data` | `Party Reference Data Directory Entry` | Sales and Service › Customer Management |
| 239 | [Party Routing Profile](02_Reference_Data.md#party-routing-profile) | `Monitor` | `Party` | `Party State` | Reference Data › Party |
| 240 | [Payee Management](01_Sales_and_Service.md#payee-management) | `Catalog` | `Payee Alias` | `Payee Alias Directory Entry` | Sales and Service › Customer Management |
| 241 | [Payment Confirmation](03_Operations_and_Execution.md#payment-confirmation) | `Process` | `Payment Confirmation` | `Payment Confirmation Procedure` | Operations and Execution › Cross Product Operations › Payments |
| 242 | [Payment Orchestration](03_Operations_and_Execution.md#payment-orchestration) | `Process` | `Payment Orchestration` | `Payment Orchestration Procedure` | Operations and Execution › Cross Product Operations › Payments |
| 243 | [Payment Order Initiation](01_Sales_and_Service.md#payment-order-initiation) | `Transact` | `Payment Order Initiation` | `Payment Order Initiation Transaction` | Sales and Service › Servicing |
| 244 | [Payment Rail](03_Operations_and_Execution.md#payment-rail) | `Operate` | `Payment Rail` | `Payment Rail Operating Session` | Operations and Execution › Cross Product Operations › Payments |
| 245 | [Payment Settlement](03_Operations_and_Execution.md#payment-settlement) | `Process` | `Payment Settlement` | `Payment Settlement Procedure` | Operations and Execution › Cross Product Operations › Payments |
| 246 | [Platform Operations](05_Business_Support.md#platform-operations) | `Operate` | `IT Systems Platform` | `IT Systems Platform Operating Session` | Business Support › IT Management |
| 247 | [Point of Service](01_Sales_and_Service.md#point-of-service) | `Operate` | `Pointof Service` | `Pointof Service Operating Session` | Sales and Service › Cross Channel |
| 248 | [Position Keeping](03_Operations_and_Execution.md#position-keeping) | `Track` | `Financial Position` | `Financial Position Log` | Operations and Execution › Cross Product Operations › Account Management |
| 249 | [Position Management](03_Operations_and_Execution.md#position-management) | `Monitor` | `Financial Position` | `Financial Position State` | Operations and Execution › Cross Product Operations › Account Management |
| 250 | [Private Placement](03_Operations_and_Execution.md#private-placement) | `Fulfill` | `Private Placement` | `Private Placement Facility` | Operations and Execution › Product Specific Fulfillment › Corporate Financing and Advisory Services |
| 251 | [Processing Order](03_Operations_and_Execution.md#processing-order) | `Process` | `Processing Order` | `Processing Order Procedure` | Operations and Execution › Cross Product Operations › Operational Services |
| 252 | [Procurement](05_Business_Support.md#procurement) | `Administer` | `Procurement` | `Procurement Administrative Plan` | Business Support › Non-IT and Non-HR Enterprise Services |
| 253 | [Product Combination](03_Operations_and_Execution.md#product-combination) | `Fulfill` | `Product Combination` | `Product Combination Facility` | Operations and Execution › Cross Product Operations › Account Management |
| 254 | [Product Deployment](02_Reference_Data.md#product-deployment) | `Develop` | `Productand Service Deployment` | `Productand Service Deployment Development` | Reference Data › Product Management |
| 255 | [Product Design](02_Reference_Data.md#product-design) | `Design` | `Product and Service` | `Productor Service Specification` | Reference Data › Product Management |
| 256 | [Product Directory](02_Reference_Data.md#product-directory) | `Catalog` | `Product` | `Product Directory Entry` | Reference Data › Product Management |
| 257 | [Product Expert Sales Support](01_Sales_and_Service.md#product-expert-sales-support) | `Administer` | `Sales Specialist Support` | `Sales Specialist Support Administrative Plan` | Sales and Service › Sales |
| 258 | [Product Inventory Distribution](01_Sales_and_Service.md#product-inventory-distribution) | `Administer` | `Product Inventory Distribution` | `Product Inventory Distribution Administrative Plan` | Sales and Service › Channel Specific |
| 259 | [Product Inventory Item Management](01_Sales_and_Service.md#product-inventory-item-management) | `Allocate` | `Product Inventory` | `Product Inventory Allocation` | Sales and Service › Channel Specific |
| 260 | [Product Matching](01_Sales_and_Service.md#product-matching) | `Assess` | `Product to Customer Combination` | `Product to Customer Combination Assessment` | Sales and Service › Sales |
| 261 | [Product Portfolio](04_Risk_and_Compliance.md#product-portfolio) | `Analyze` | `Product Portfolio` | `Product Portfolio Analysis` | Risk and Compliance › Business Analysis |
| 262 | [Product Quality Assurance](02_Reference_Data.md#product-quality-assurance) | `Assess` | `Product and Service` | `Product and Service Assessment` | Reference Data › Product Management |
| 263 | [Product Sales Support](01_Sales_and_Service.md#product-sales-support) | `Administer` | `Product Sales Support` | `Product Sales Support Administrative Plan` | Sales and Service › Sales |
| 264 | [Product Service Agency](02_Reference_Data.md#product-service-agency) | `Agree Terms` | `Service Provider` | `Service Provider Agreement` | Reference Data › External Agency |
| 265 | [Product Training](02_Reference_Data.md#product-training) | `Process` | `Product Training` | `Product Training Procedure` | Reference Data › Product Management |
| 266 | [Production Release](05_Business_Support.md#production-release) | `Assess` | `Production System` | `Production System Assessment` | Business Support › IT Management |
| 267 | [Production Risk Models](04_Risk_and_Compliance.md#production-risk-models) | `Design` | `Production Risk Model` | `Production Risk Model Specification` | Risk and Compliance › Models |
| 268 | [Products and Services Direction](05_Business_Support.md#products-and-services-direction) | `Direct` | `Products And Services` | `Products And Services Strategy` | Business Support › Business Direction |
| 269 | [Program Trading](03_Operations_and_Execution.md#program-trading) | `Operate` | `Program Trading` | `Program Trading Operating Session` | Operations and Execution › Product Specific Fulfillment › Wholesale Trading |
| 270 | [Project Finance](03_Operations_and_Execution.md#project-finance) | `Fulfill` | `Project Finance` | `Project Finance Facility` | Operations and Execution › Product Specific Fulfillment › Trade Banking |
| 271 | [Promotional Events](01_Sales_and_Service.md#promotional-events) | `Manage` | `Promotional Event` | `Promotional Event Management Plan` | Sales and Service › Marketing |
| 272 | [Property Portfolio](05_Business_Support.md#property-portfolio) | `Analyze` | `Building Portfolio` | `Building Portfolio Analysis` | Business Support › Buildings Equipment and Facilities |
| 273 | [Prospect Campaign Design](01_Sales_and_Service.md#prospect-campaign-design) | `Design` | `Prospect Campaign` | `Prospect Campaign Specification` | Sales and Service › Marketing |
| 274 | [Prospect Campaign Execution](01_Sales_and_Service.md#prospect-campaign-execution) | `Process` | `Prospect Campaign` | `Prospect Campaign Procedure` | Sales and Service › Sales |
| 275 | [Prospect Campaign Management](01_Sales_and_Service.md#prospect-campaign-management) | `Manage` | `Prospect Campaign Portfolio` | `Prospect Campaign Portfolio Management Plan` | Sales and Service › Marketing |
| 276 | [Public Offering](03_Operations_and_Execution.md#public-offering) | `Fulfill` | `Public Offering` | `Public Offering Facility` | Operations and Execution › Product Specific Fulfillment › Corporate Financing and Advisory Services |
| 277 | [Public Reference Data Management](02_Reference_Data.md#public-reference-data-management) | `Design` | `Global Standard` | `Global Standard Specification` | Reference Data › Market Data |
| 278 | [Quant Model](02_Reference_Data.md#quant-model) | `Design` | `Quant Model` | `Quant Model Specification` | Reference Data › Market Data |
| 279 | [Quote Management](03_Operations_and_Execution.md#quote-management) | `Process` | `Quotation` | `Quotation Procedure` | Operations and Execution › Product Specific Fulfillment › Wholesale Trading |
| 280 | [Recruitment](05_Business_Support.md#recruitment) | `Process` | `Recruitment` | `Recruitment Procedure` | Business Support › Human Resource Management |
| 281 | [Regulatory And Legal Authority](05_Business_Support.md#regulatory-and-legal-authority) | `Manage` | `Regulatory And Legal Authority Relationship` | `Regulatory And Legal Authority Relationship Management Plan` | Business Support › Corporate Relations |
| 282 | [Regulatory Compliance](04_Risk_and_Compliance.md#regulatory-compliance) | `Assess` | `Regulatory Compliance` | `Regulatory Compliance Assessment` | Risk and Compliance › Regulations and Compliance |
| 283 | [Regulatory Reporting](04_Risk_and_Compliance.md#regulatory-reporting) | `Administer` | `Regulatory Compliance` | `Regulatory Compliance Administrative Plan` | Risk and Compliance › Regulations and Compliance |
| 284 | [Reward Points Account](03_Operations_and_Execution.md#reward-points-account) | `Track` | `Reward Points` | `Reward Points Log` | Operations and Execution › Cross Product Operations › Account Management |
| 285 | [Reward Points Awards And Redemption](03_Operations_and_Execution.md#reward-points-awards-and-redemption) | `Transact` | `Reward Points` | `Reward Points Transaction` | Operations and Execution › Cross Product Operations › Operational Services |
| 286 | [Rewards Delivery](03_Operations_and_Execution.md#rewards-delivery) | `Process` | `Rewards Delivery` | `Rewards Delivery Procedure` | Operations and Execution › Cross Product Operations › Operational Services |
| 287 | [Rewards Inventory](03_Operations_and_Execution.md#rewards-inventory) | `Allocate` | `Rewards Inventory` | `Rewards Inventory Allocation` | Operations and Execution › Cross Product Operations › Operational Services |
| 288 | [Rewards Menu](03_Operations_and_Execution.md#rewards-menu) | `Catalog` | `Rewards Option` | `Rewards Option Directory Entry` | Operations and Execution › Cross Product Operations › Operational Services |
| 289 | [Sales Planning](01_Sales_and_Service.md#sales-planning) | `Direct` | `Marketing And Sales` | `Marketing And Sales Strategy` | Sales and Service › Sales |
| 290 | [Sales Product](01_Sales_and_Service.md#sales-product) | `Agree Terms` | `Product and Service` | `Product and Service Agreement` | Sales and Service › Sales |
| 291 | [Sales Product Agreement](01_Sales_and_Service.md#sales-product-agreement) | `Agree Terms` | `Sales Product Agreement` | `Sales Product Agreement` | Sales and Service › Customer Management |
| 292 | [Savings Account](03_Operations_and_Execution.md#savings-account) | `Fulfill` | `Savings Account` | `Savings Account Facility` | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |
| 293 | [Securities Fails Processing](03_Operations_and_Execution.md#securities-fails-processing) | `Process` | `Security Trading Fails` | `Security Trading Fails Procedure` | Operations and Execution › Product Specific Fulfillment › Market Operations |
| 294 | [Securities Position Keeping](03_Operations_and_Execution.md#securities-position-keeping) | `Track` | `Securities Position` | `Securities Position Log` | Operations and Execution › Cross Product Operations › Account Management |
| 295 | [Security Advisory](05_Business_Support.md#security-advisory) | `Process` | `Security Compliance` | `Security Compliance Procedure` | Business Support › Non-IT and Non-HR Enterprise Services |
| 296 | [Security Assurance](05_Business_Support.md#security-assurance) | `Assess` | `Security Compliance` | `Security Compliance Assessment` | Business Support › Non-IT and Non-HR Enterprise Services |
| 297 | [Segment Direction](04_Risk_and_Compliance.md#segment-direction) | `Direct` | `Segment` | `Segment Strategy` | Risk and Compliance › Business Analysis |
| 298 | [Service Directory](01_Sales_and_Service.md#service-directory) | `Catalog` | `Service` | `Service Directory Entry` | Sales and Service › Cross Channel |
| 299 | [Service Provider Operations](02_Reference_Data.md#service-provider-operations) | `Operate` | `Service Provider Registration` | `Service Provider Registration Operating Session` | Reference Data › External Agency |
| 300 | [Servicing Activity Analysis](01_Sales_and_Service.md#servicing-activity-analysis) | `Analyze` | `Servicing Root Cause` | `Servicing Root Cause Analysis` | Sales and Service › Cross Channel |
| 301 | [Servicing Event History](01_Sales_and_Service.md#servicing-event-history) | `Track` | `Servicing Event` | `Servicing Event Log` | Sales and Service › Cross Channel |
| 302 | [Servicing Issue](01_Sales_and_Service.md#servicing-issue) | `Process` | `Servicing Issue` | `Servicing Issue Procedure` | Sales and Service › Servicing |
| 303 | [Servicing Mandate](01_Sales_and_Service.md#servicing-mandate) | `Agree Terms` | `Servicing Mandate` | `Servicing Mandate Agreement` | Sales and Service › Servicing |
| 304 | [Servicing Order](01_Sales_and_Service.md#servicing-order) | `Process` | `Servicing Order` | `Servicing Order Procedure` | Sales and Service › Servicing |
| 305 | [Session Dialogue](01_Sales_and_Service.md#session-dialogue) | `Process` | `Customer Contact Session` | `Customer Contact Session Procedure` | Sales and Service › Cross Channel |
| 306 | [Site Administration](05_Business_Support.md#site-administration) | `Administer` | `Building` | `Building Administrative Plan` | Business Support › Buildings Equipment and Facilities |
| 307 | [Site Operations](05_Business_Support.md#site-operations) | `Administer` | `Building Services` | `Building Services Administrative Plan` | Business Support › Buildings Equipment and Facilities |
| 308 | [Special Pricing Conditions](02_Reference_Data.md#special-pricing-conditions) | `Catalog` | `Special Pricing Conditions` | `Special Pricing Conditions Directory Entry` | Reference Data › Product Management |
| 309 | [Standing Order](03_Operations_and_Execution.md#standing-order) | `Fulfill` | `Standing Order` | `Standing Order Facility` | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |
| 310 | [Stock Lending and Repos](04_Risk_and_Compliance.md#stock-lending-and-repos) | `Transact` | `Repo` | `Repo Transaction` | Risk and Compliance › Bank Portfolio and Treasury |
| 311 | [Sub Custodian Agreement](02_Reference_Data.md#sub-custodian-agreement) | `Agree Terms` | `Sub Custodian` | `Sub Custodian Agreement` | Reference Data › External Agency |
| 312 | [Suitability Checking](03_Operations_and_Execution.md#suitability-checking) | `Assess` | `Suitability` | `Suitability Assessment` | Operations and Execution › Product Specific Fulfillment › Wholesale Trading |
| 313 | [Syndicate Management](02_Reference_Data.md#syndicate-management) | `Enroll` | `Syndicate` | `Syndicate Membership` | Reference Data › External Agency |
| 314 | [Syndicated Loan](03_Operations_and_Execution.md#syndicated-loan) | `Fulfill` | `Syndicated Loan` | `Syndicated Loan Facility` | Operations and Execution › Product Specific Fulfillment › Trade Banking |
| 315 | [System Deployment](05_Business_Support.md#system-deployment) | `Develop` | `IT System Deployment` | `IT System Deployment Project` | Business Support › IT Management |
| 316 | [System Development](05_Business_Support.md#system-development) | `Develop` | `IT System` | `IT System Development` | Business Support › IT Management |
| 317 | [Systems Administration](05_Business_Support.md#systems-administration) | `Administer` | `IT System` | `IT System Administrative Plan` | Business Support › IT Management |
| 318 | [Systems Assurance](05_Business_Support.md#systems-assurance) | `Assess` | `IT System` | `IT System Assessment` | Business Support › IT Management |
| 319 | [Systems Help Desk](05_Business_Support.md#systems-help-desk) | `Operate` | `Help Desk` | `Help Desk Operating Session` | Business Support › IT Management |
| 320 | [Systems Operations](05_Business_Support.md#systems-operations) | `Operate` | `IT System` | `IT System Operating Session` | Business Support › IT Management |
| 321 | [Term Deposit](03_Operations_and_Execution.md#term-deposit) | `Fulfill` | `Term Deposit` | `Term Deposit Facility` | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |
| 322 | [Term Deposit Framework Agreement](03_Operations_and_Execution.md#term-deposit-framework-agreement) | `Fulfill` | `Term Deposit Framework Agreement` | `Term Deposit Framework Agreement Facility` | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |
| 323 | [Trade Clearing](03_Operations_and_Execution.md#trade-clearing) | `Process` | `Trade Clearing` | `Trade Clearing Procedure` | Operations and Execution › Product Specific Fulfillment › Market Operations |
| 324 | [Trade Confirmation Matching](03_Operations_and_Execution.md#trade-confirmation-matching) | `Operate` | `Trade Matching` | `Trade Matching Operating Session` | Operations and Execution › Product Specific Fulfillment › Market Operations |
| 325 | [Trade Settlement](03_Operations_and_Execution.md#trade-settlement) | `Process` | `Trade Settlement` | `Trade Settlement Procedure` | Operations and Execution › Product Specific Fulfillment › Market Operations |
| 326 | [Trade and Price Reporting](03_Operations_and_Execution.md#trade-and-price-reporting) | `Operate` | `Market Trade Reporting` | `Market Trade Reporting Operating Session` | Operations and Execution › Product Specific Fulfillment › Market Operations |
| 327 | [Trader Position Operations](03_Operations_and_Execution.md#trader-position-operations) | `Operate` | `Traded Position` | `Traded Position Operating Session` | Operations and Execution › Product Specific Fulfillment › Wholesale Trading |
| 328 | [Trading Book Oversight](03_Operations_and_Execution.md#trading-book-oversight) | `Manage` | `Trading Position` | `Trading Position Management Plan` | Operations and Execution › Product Specific Fulfillment › Wholesale Trading |
| 329 | [Trading Models](03_Operations_and_Execution.md#trading-models) | `Design` | `Trading Model` | `Trading Model Specification` | Operations and Execution › Product Specific Fulfillment › Wholesale Trading |
| 330 | [Transaction Authorization](01_Sales_and_Service.md#transaction-authorization) | `Assess` | `Interactive Transaction` | `Interactive Transaction Assessment` | Sales and Service › Cross Channel |
| 331 | [Transaction Engine](03_Operations_and_Execution.md#transaction-engine) | `Fulfill` | `Transaction Schedule` | `Transaction Schedule Facility` | Operations and Execution › Cross Product Operations › Account Management |
| 332 | [Travel and Expenses](05_Business_Support.md#travel-and-expenses) | `Administer` | `Employee Travel and Expenses` | `Employee Travel and Expenses Administrative Plan` | Business Support › Human Resource Management |
| 333 | [Trust Services](03_Operations_and_Execution.md#trust-services) | `Fulfill` | `Trust Services` | `Corporate Trust Services Facility` | Operations and Execution › Product Specific Fulfillment › Consumer Services |
| 334 | [Underwriting](01_Sales_and_Service.md#underwriting) | `Assess` | `Underwriting` | `Underwriting Assessment` | Sales and Service › Sales |
| 335 | [Unit Trust Administration](03_Operations_and_Execution.md#unit-trust-administration) | `Administer` | `Unit Trust` | `Unit Trust Administrative Plan` | Operations and Execution › Product Specific Fulfillment › Market Operations |
| 336 | [Utilities Administration](05_Business_Support.md#utilities-administration) | `Administer` | `Utilities` | `Utilities Administrative Plan` | Business Support › Buildings Equipment and Facilities |
| 337 | [Virtual Account](03_Operations_and_Execution.md#virtual-account) | `Fulfill` | `Virtual Account` | `Virtual Account Facility` | Operations and Execution › Product Specific Fulfillment › Loans and Deposits |
| 338 | [Workforce Training](05_Business_Support.md#workforce-training) | `Administer` | `Employee Training` | `Employee Training Administrative Plan` | Business Support › Human Resource Management |
| 339 | [eBranch Management](01_Sales_and_Service.md#ebranch-management) | `Manage` | `eBranch Channel` | `eBranch Channel Management Plan` | Sales and Service › Channel Specific |
| 340 | [eBranch Operations](01_Sales_and_Service.md#ebranch-operations) | `Operate` | `eBranch Channel` | `eBranch Channel Operating Session` | Sales and Service › Channel Specific |
| 341 | [eTrading Workbench](03_Operations_and_Execution.md#etrading-workbench) | `Operate` | `eTrading Workbench` | `eTrading Workbench Operating Session` | Operations and Execution › Product Specific Fulfillment › Investment Management |

---

## Fuente

Vista **Matrix** del BIAN Service Landscape **V14.0** (`bian.org/servicelandscape-14-0-0`), las vistas `<SD> SD Overview` y `<SD> Control Record Diagram`, y el repositorio `github.com/bian-official/public`, release 14.0.0.

Los ejemplos de los libros de BIAN no son fuente de nomenclatura y no entran en este catálogo.