
# Temenos Transact — Islamic_Banking Module Documentation


> **Comprehensive User Guide**
> Generated: 13 April 2026
> Content: Configuration | Reference | Field Descriptions | Glossary


## Table of Contents

  - [Islamic_Banking Module Overview](#islamic_banking-module-overview)
    - [Sub-Module Summary](#sub-module-summary)
    - [How to Use This Guide](#how-to-use-this-guide)
  - [Chapter 1: Islamic_Banking - ID](#chapter-1-islamic_banking---id)
    - [Features in Islamic_Banking - ID](#features-in-islamic_banking---id)
    - [1.1  Account Statements](#11-account-statements)
    - [1.2  COB Processing](#12-cob-processing)
    - [1.3  Charges and Commissions](#13-charges-and-commissions)
    - [1.4  Hybrid Pooling](#14-hybrid-pooling)
    - [1.5  Arrangement Pool Linking](#15-arrangement-pool-linking)
    - [1.6  Islamic Accounts](#16-islamic-accounts)
    - [1.7  Islamic Deposit Products](#17-islamic-deposit-products)
    - [1.8  Misc](#18-misc)
    - [1.9  Payment of Profit Amount using Charges](#19-payment-of-profit-amount-using-charges)
    - [1.10  PDS Distribution](#110-pds-distribution)
    - [1.11  PDS Simulation](#111-pds-simulation)
    - [1.12  Charges](#112-charges)
    - [1.13  SubAccounts](#113-subaccounts)
    - [1.14  Limit Balance](#114-limit-balance)
    - [1.15  Misc](#115-misc)
    - [1.16  Misc](#116-misc)
    - [1.17  Chargeoff](#117-chargeoff)
    - [1.18  Charges](#118-charges)
    - [1.19  LendingRule78](#119-lendingrule78)
    - [1.20  Loan Commitment](#120-loan-commitment)
    - [1.21  Migration of LendingArrangements](#121-migration-of-lendingarrangements)
    - [1.22  Payment Holiday](#122-payment-holiday)
    - [1.23  Scheduling Payments](#123-scheduling-payments)
    - [1.24  Weighted Average Rate](#124-weighted-average-rate)
    - [1.25  Misc](#125-misc)
  - [Chapter 2: Islamic_Banking - IS](#chapter-2-islamic_banking---is)
    - [Features in Islamic_Banking - IS](#features-in-islamic_banking---is)
    - [2.1  Account Statements](#21-account-statements)
    - [2.2  ProductBuilder](#22-productbuilder)
    - [2.3  Charges and Commissions](#23-charges-and-commissions)
    - [2.4  Hybrid Pooling](#24-hybrid-pooling)
    - [2.5  Upfront Profit in Club Finance](#25-upfront-profit-in-club-finance)
    - [2.6  Asset Capture](#26-asset-capture)
    - [2.7  Asset Review](#27-asset-review)
    - [2.8  Commodity Delivery and Sale](#28-commodity-delivery-and-sale)
    - [2.9  CreatingFacility for IslamicFinanceProducts](#29-creatingfacility-for-islamicfinanceproducts)
    - [2.10  Finance Profit Accrual Product](#210-finance-profit-accrual-product)
    - [2.11  Finance Profit Upfront Sale Product Group](#211-finance-profit-upfront-sale-product-group)
    - [2.12  Islamic Contract](#212-islamic-contract)
    - [2.13  IslamicSyndicateFinance](#213-islamicsyndicatefinance)
    - [2.14  Misc](#214-misc)
    - [2.15  Payment Management](#215-payment-management)
    - [2.16  PaymentManagementUsingPO](#216-paymentmanagementusingpo)
    - [2.17  ProfitDeclaration](#217-profitdeclaration)
    - [2.18  Charges](#218-charges)
    - [2.19  SubAccounts](#219-subaccounts)
    - [2.20  Limit Balance](#220-limit-balance)
    - [2.21  Misc](#221-misc)
    - [2.22  Chargeoff](#222-chargeoff)
    - [2.23  Charges](#223-charges)
    - [2.24  LendingRule78](#224-lendingrule78)
    - [2.25  Loan Commitment](#225-loan-commitment)
    - [2.26  Migration of LendingArrangements](#226-migration-of-lendingarrangements)
    - [2.27  Misc](#227-misc)
    - [2.28  Payment Holiday](#228-payment-holiday)
    - [2.29  Scheduling Payments](#229-scheduling-payments)
    - [2.30  Weighted Average Rate](#230-weighted-average-rate)
    - [2.31  Misc](#231-misc)
  - [Appendix A: Glossary of T24 Applications & Fields](#appendix-a-glossary-of-t24-applications-fields)
    - [Applications](#applications)
    - [Fields Referenced](#fields-referenced)
  - [Appendix B: Consolidated Field Reference](#appendix-b-consolidated-field-reference)
    - [Islamic_Banking - ID (ID)](#islamic_banking---id-id)
    - [Islamic_Banking - IS (IS)](#islamic_banking---is-is)

---


## Islamic_Banking Module Overview


This document provides comprehensive documentation for the **Islamic_Banking** module of Temenos Transact. It covers **2 sub-modules** with a total of **56 feature areas**.


### Sub-Module Summary


| # | Sub-Module | Code | Features | Description |
|---|-----------|------|----------|-------------|
| 1 | **Islamic_Banking - ID** | `ID` | 25 | Islamic_Banking - ID module of Temenos Transact |
| 2 | **Islamic_Banking - IS** | `IS` | 31 | Islamic_Banking - IS module of Temenos Transact |


### How to Use This Guide


Each feature in this document is organized into the following sections:

- 📖 **Introduction** — Overview and purpose of the feature
- ⚙️ **Configuration** — How to set up and configure the feature
- 🔧 **Working With** — Operational usage and field descriptions
- 📋 **Tasks** — Step-by-step procedures
- 📊 **Outputs** — Reports, enquiries, and generated outputs

Each feature includes a **Quick Reference Card** at the top with application names, key fields, prerequisites, and a summary. Appendices provide a full glossary, consolidated field tables, and end-to-end use-case scenarios.

---


## Chapter 1: Islamic_Banking - ID


Islamic_Banking - ID module of Temenos Transact


### Features in Islamic_Banking - ID


| # | Feature | Sections |
|---|---------|----------|
| 1.1 | Account Statements | Intro |
| 1.2 | COB Processing | Worki |
| 1.3 | Charges and Commissions | Worki |
| 1.4 | Hybrid Pooling | Worki |
| 1.5 | Arrangement Pool Linking | Intro, Confi, Tasks, Outpu |
| 1.6 | Islamic Accounts | Intro, Confi, Tasks, Outpu |
| 1.7 | Islamic Deposit Products | Intro, Confi, Tasks, Outpu |
| 1.8 | Misc | Intro |
| 1.9 | Payment of Profit Amount using Charges | Intro, Confi, Worki, Tasks, Outpu |
| 1.10 | PDS Distribution | Intro, Confi, Tasks, Outpu |
| 1.11 | PDS Simulation | Intro, Confi, Tasks, Outpu |
| 1.12 | Charges | Worki |
| 1.13 | SubAccounts | Confi |
| 1.14 | Limit Balance | Intro |
| 1.15 | Misc | Intro |
| 1.16 | Misc | Intro |
| 1.17 | Chargeoff | Worki |
| 1.18 | Charges | Worki |
| 1.19 | LendingRule78 | Intro |
| 1.20 | Loan Commitment | Confi |
| 1.21 | Migration of LendingArrangements | Worki |
| 1.22 | Payment Holiday | Intro, Confi, Worki |
| 1.23 | Scheduling Payments | Confi, Worki |
| 1.24 | Weighted Average Rate | Intro |
| 1.25 | Misc | Intro |


### 1.1  Account Statements


> **📇 Quick Reference Card**
> 
> **Purpose:** *Statement Property Class is used to specify the account level statement settings such as Stmt Frequency , Start Date , No Activity Indicator etc. For arrangements without Statement Property Class, the Account Statement functionality continues.*
> 
> **Key Fields:** *Frequency*, *No Activity Indicator*, *Start Date*, *Stmt*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Statement Property Class is used to specify the account level statement settings such as Stmt Frequency , Start Date , No Activity Indicator etc. For arrangements without Statement Property Class, the Account Statement functionality continues.

---


### 1.2  COB Processing


> **📇 Quick Reference Card**
> 
> **Applications:** `AA.ACCRUAL.FREQUENCY`, `AA.ACTIVITY.CLASS`, `AA.ARRANGEMENT.ACTIVITY`, `AA.DECISION.PARAMETER`, `AA.INTEREST.ACCRUALS`, `AA.NEXT.ACTIVITY`, `AA.SCHEDULED.ACTIVITY`, `ACCR.REV.PARAM` ... +4 more
> 
> **Key Fields:** *Activity Type*, *Default Ol Accrual*, *Pre Cob Check*, *Prod Prop Ol Accrual*, *Prop Ol Accrual*, *Property Ol Accrual*
> 
> **Sections:** 🔧 Working With


#### 🔧 Working With

The following section describes the unauthorised activities, scheduled activities and their sequence during COB processing along with other technical information.


##### Unauthorised Activities in COB processing

The AA framework unlike other applications performs all the activities considering and including unauthorised activities. For example, a secondary activity like a scheduled disbursement is triggered in Unauthorised status even when the new arrangement is pending authorisation. It does not allow the user to create yet an activity when another activity is Unauthorised status because of this reason.

Any transaction activity in the Retail Accounts module is a financial transaction initiated from other applications and is usually in Unauthorised status (considering the maker-checker concept). It is possible to trigger another regular activity or transaction activity in unauthorised status when a debit arrangement or a credit arrangement activity is unauthorised. The system differentiates the debit arrangement and credit arrangement activity using the Direct Accounting Activity Type in AA.ACTIVITY.CLASS .

During COB, no unauthorised activity across the AA framework should be considered for batch processing. The system deletes all the unauthorised AA activities when COB is initiated and re-creates these activities when COB process is completed.

This ensures that the unauthorised activities do not affect the system processing like day-end accruals on the authorised balance and scheduled payments.

For certain HVT account products, as part of business there can be a huge number of unauthorised transaction activities in the system when COB is initiated. Deleting these activities and re-creating them might result in huge performance issues.

AA.DECISION.PARAMETER is used to configure these Account products from which the unauthorised debit and credit arrangements can be retained during the COB processing.


##### Batches and Jobs

The following section describes the handling of Scheduled Activities in AA.


###### Scheduled Activities

Arrangement activities are processed using the AA.ARRANGEMENT.ACTIVITY application and these can be initiated in a number of ways:

- User initiated request
- Non AA-transaction initiated – For example when crediting or debiting an arrangement account from an existing application.
- As a scheduled process – The activity should be processes automatically according to a some schedule defined for the product or arrangement

Some activities may be initiated in more than one way. The valid initiation types are defined in the AA.ACTIVITY.CLASS definition which is released by Temenos. The definition is contained in the Activity Type field. The initiation method of activities is pre-defined and cannot be amended.

Scheduled activities are processed as part of the Close of Business (COB) and specific BATCH records are released with the relevant jobs required to perform the contract processing.


###### Sequence of Activities in Batch Processes

Several activities may be scheduled to be processed for an arrangement on the same date, the sequence the activities are performed in is important and this is defined as part of the AA.ACTIVITY.CLASS definition.

Each batch process that should perform the scheduled activity is specified in the AA.ACTIVITY.CLASS record together with a numeric sequence which is used to determine the order that the activities are executed for an arrangement.

The definition of the batch and sequence are pre-defined and cannot be amended.


###### Arrangement Contract Scheduled Activities

Arrangement contracts for products that have scheduled activities maintains a list of scheduled activities to be performed for that arrangement together with the next scheduled event date and the last time it was performed.

These details are maintained in AA.SCHEDULED.ACTIVITY . The details are updated as part of the activity processing for arrangement property maintenance and the scheduled activity itself. For example, the creation of a new loan contract updates the next scheduled MAKEDUE activity when the PAYMENT.SCHEDULE is initially defined or subsequently modified. The MAKEDUE activity itself cycles forward to the next due date and ensure that AA.SCHEDULED.ACTIVITY reflects this.


###### Accrual Frequency

Activities such as Accrual and Amortisation perform internal accounting processing (that is, the booking of P&L) rather than actions that relate to the customer of the contract. The frequency for performing these activities does not form part of the product definition and is instead controlled by a central accrual frequency definition in AA.ACCRUAL.FREQUENCY .

A single definition exists for each financial company that allows the frequency to be defined at the following levels for properties that can be accrued:

1. For a specific property of a specific product.
2. For a specific property in any product.
3. For any property.

For each of theses combinations different frequencies can be defined for local and foreign currency contracts.The following frequency options are allowed for accrual:

- DAILY – The accrual processing takes place for each Calendar day, that is, on a Friday COB for a normal weekend, there are three accrual activities processed for a contract.
- BSNSS – The accrual processing takes place for each business day, that is, on a Friday COB for a normal weekend, there is one accrual activity for a contract that covers the period Friday – Sunday inclusive.
- Mnndd – The accrual is performed every nn months on the dd day of the month. If 31 is defined as the day, this indicates that processing must take place on the last day of the month.
- Null – No accrual is to be processed on scheduled basis at all.

Only properties that belong the Interest or Charge Property Classes can be defined in AA.ACCRUAL.FREQUENCY . It is also possible to reverse the earlier accruals/amortisation and rebook them daily by setting up ACCR.REV.PARAM . For more details, refer to the Reporting user guide.

In the above example, the following frequencies are applied:

- Product HIGHVALUELOAN. Interest property CURRINT for local currency contracts is accrued monthly on the 15 th of the month. Interest property CURRINT for foreign currency contracts is accrued on a daily basis. Interest property PENALTYINT for local currency contracts is accrued monthly on the 15 th of the month. Interest property PENALTYINT for foreign currency contracts is accrued daily.
- Any product other than HIGHVALUELOAN using PENALTYINT interest property. Local currency contracts are accrued monthly on the last day of the month. Foreign currency contracts are accrued daily.
- Any other interest property or product. Local currency contracts perform no scheduled accrual. Foreign contracts are accrued quarterly on the last day of the month.

Activities that determine their processing frequency as scheduled tasks are defined in the AA.ACTIVITY.CLASS record. The Activity Type field contains ACCRUAL to indicate this. This is pre-determined and cannot be modified.

The accrual of interest and charges is processed as part of the AA.SERVICE.PROCESS during COB. However, the system can process the interest and charge accruals online, by setting the Default Ol Accrual , Property Ol Accrual , and Prod Prop Ol Accrual fields in the record in AA.ACCRUAL.FREQUENCY . In this case, the online accrual of interest and charges is processed by running the AA.ONLINE.ACCRUAL.SERVICE service. Read here to know more about the online processing of accruals.


##### Processing the Activity

When a scheduled activity is processed, an AA.ARRANGEMENT.ACTIVITY transaction gets performed the transaction request contains the arrangement number, required activity and effective date for the request. The effective is the actual date that the activity should be processed on.

The activity request is performed by the TSA service running the process through OFS. Scheduled activities are processed without the need to separate authorisation, in the case of processing error or exception the activity request leaves in HLD status and can be completed manually. The detail of error and exception (for example, override) processing depends on the operation of the specific activity.

For frequently repeated activities such as accrual, the same AA.ARRANGEMENT.ACTIVITY transaction is used for each scheduled event. For all other scheduled activities, separate AA.ARRANGEMENT.ACTIVITY transactions gets generated.

It is possible to reverse scheduled activity requests after the scheduled activity has taken place (subject to any restrictions that a specific activity may have).


###### Transaction Management

For each arrangement and processing date, the system processes all scheduled activities together. Activities are performed in the correct sequence and forms a single database transaction, Any error or failure of an activity means that all activities for that arrangement and processing date are not going to be processed.


###### AA.EOD.PROCESS

This batch performs arrangement processing in the End of Day section of the close of business. The Batch is defined for each Financial company in a multi-company implementation and runs in the system wide section of the close of business.

The following processes are run as part of this batch:

- Processing of Payments in and out of arrangement accounts generated as part of the close of business.
- Processing of scheduled activities for the products.


###### AA.SOD.PROCESS

This batch performs arrangement processing in the Start of Day section of the close of business. The Batch is defined for each Financial company in a multi-company implementation and runs in the start of day section of the close of business.

The following processes are run as part of this batch:

- Processing of Payments in and out of arrangement accounts generated as part of the close of business.
- Processing of scheduled activities for the products.


###### AA.SERVICE.PROCESS

This job performs the processing of all scheduled activities. The process checks for all current arrangement contracts to see if there a scheduled activity due to be processed as part of the Close of Business.

Activities are processed by generating AA.ARRANGEMENT.ACTIVITY records as described above.

When run in the End of Day close of business, this process is repeated for each calendar date between and including the current system date and the period end date. For each processing date, all contracts are processed.

When run in the Start of Day close of business the process can only be performed in the case of a month end that is, the last working day was in the previous month). The processing gets repeated for each calendar date between and including the 1 st day of the month up to the calendar date before the current system date.


###### Online Processing of Accruals and Rate Changes

The following activities which are triggered as part of the AA Service Process during COB, can be triggered online by running the AA.ONLINE.ACCRUAL.SERVICE service thereby reducing the execution time of COB.

- Applying Basic and Periodic Interest rate changes on the arrangements.
- Accrual of interest and charges.

When the ONLINE.ACCRUAL.SERVICE is run, the system triggers the Rate Change processing first, followed by the Online accrual processing.

When there is a change to the records in BASIC.INTEREST and/or PERIODIC.INTEREST , associated arrangements are updated with the changes. The system performs this as part of AA Service Process during COB where it triggers the corresponding activities in those associated arrangements. The process of applying the rate changes to the associated arrangements can be performed online by running the AA.ONLINE.ACCRUAL.SERVICE online service. When this service is run, the system tracks any changes to the BI/PI keys. For all the associated arrangements using these keys, the system updates the rate changes by triggering the corresponding activity, similar to how the rate changes are processed during COB.

When the activity to update the arrangement is triggered, the system validates if the accrual for the day is already processed. If the accrual for the day is already processed in the arrangement, then the system performs a reverse-replay to recalculate the accrual amount and posts the adjustments for the arrangement. These recalculations and adjustments are processed as follows:

- As part of the update activity itself for loans and deposits (or)
- By updating the AA.RR.SERVICE.LIST for accounts. This list is cleared when the reverse-replay service namely AA.RR.SERVICE is run. The accruals on the current date are processed using the latest prevailing effective rate.

The user can perform the online accrual of interest and charges by setting the Default Ol Accrual , Property Ol Accrual , or Prod Prop Ol Accrual fields to Yes in the record in AA.ACCRUAL.FREQUENCY .

- Prod Prop Ol Accrual - For a specific property of a specific product.
- Property Ol Accrual - For a specific property in any product.
- Default Ol Accrual - For all interest and charge properties belonging to any product.

In this case, the user must run the AA.ONLINE.ACCRUAL.SERVICE service during which the system processes the accruals:

- Accrues the interest and charges.
- Updates the records in AA.INTEREST.ACCRUALS and/or EB.ACCRUAL for the properties.
- Raises the accounting entries for the accruals in the arrangement.

The user can enable online accrual processing for all interest and charge properties by defining the Default Ol Accrual field as Yes in the record in AA.ACCRUAL.FREQUENCY . If the user does not choose to enable online accrual processing for a specific property or a specific property from a specific product, then the user can set the Property Ol Accrual and Prod Prop Ol Accrual fields to Null. In this case, only for those specific properties that belong to the specific products, the system skips online processing of accruals. For these properties, the accruals are processed as part of the AA Service Process during COB. The vice versa is also possible, where the user can set Default Ol Accrual as Null and enable online accrual processing for a specific property or a specific property from a specific product by setting the Property Ol Accrual and Prod Prop Ol Accrual fields to Yes respectively. In this case, only for those specific properties the accruals are processed online, and for all other properties the accruals are processed during COB.

As an example, in the below screenshot, since the Default Ol Accrual is set as Yes, online accrual processing is enabled for all interest and charge properties belonging to all products. Further, since Prop Ol Accrual is set as Null for CRPROFIT property and Prod Prop Ol Accrual is set as Yes for CRPROFIT property that belongs to the MUDARABA.MONTHLY.MIN.ACCOUNT product.

Hence, the online accrual processing is skipped for all arrangements using the CRPROFIT property except for the arrangements under the MUDARABA.MONTHLY.MIN.ACCOUNT product. For the arrangements belonging to the MUDARABA.MONTHLY.MIN.ACCOUNT product, the system performs online accruals for the CRPROFIT property. For all other arrangements, the accrual for the CRPPROFIT property is processed during COB.

> **⚠️ Note:** It is recommended to use regular COB accrual for properties using Linked Rates and not configure online accruals for the same. If an activity is scheduled for the day which affects the balance or the rate, then the online accruals are skipped for that day. In such cases, the system performs the accrual for the day during COB after the scheduled activity is processed. This is because the change in balance or rate necessitates an adjustment and recalculation to the accrued interest or charge amount. When processed during COB, the system performs the accrual after the scheduled activity is processed and therefore, the accrual amount is calculated using the correct balance or rate.

- When online accrual processing is enabled using the AA.ACCRUAL.FREQUENCY setup, it is mandatory to run the AA.ONLINE.ACCRUAL.SERVICE service.
- The user should configure the system to mandate that the AA.ONLINE.ACCRUAL.SERVICE service is run at least once for the day for the user to be able to run the Close of Business (COB). The Pre Cob Check field of the record in TSA.SERVICE for the AA.ONLINE.ACCRUAL.SERVICE service, must be set to Yes when the online accrual functionality is used. This ensures the rate fixing and the online accruals are processed before COB is initiated. Otherwise, the accruals for the day are skipped all together.
- When both online accrual and early schedule processing (set at the account arrangement level) are enabled, then the processing of accruals and rate change are handled by the Intraday service (AA.INTRADAY.PROCESS) for those accounts. In this case, the user must run the Intraday Process service everyday. The Pre Cob Check field of the record in TSA.SERVICE for the service AA.INTRADAY.PROCESS, must be set to Yes when the early schedule processing is enabled.


###### Technical Details

The selection of contracts is driven from the AA.NEXT.ACTIVITY internal table . This contains one record for each arrangement contract with the contract number and next scheduled activity date of any type, it is maintained with the AA.SCHEDULED.ACTIVITY table. A filter routine is used to ensure that only arrangements with an activity due for that process date, or with a possible accrual frequency are added to the JOB.LIST for processing.


###### AA.COB.PAY.IN.OUT

This job submits and completes processing of AA.ARRANGEMENT.ACTIVITY requests generated by non-AA transactions during close of business. During close of business processing, the payment transactions generates AA.ARRANGEMENT.ACTIVITY requests in HLD status.

The processing checks all AA.ARRANGEMENT.ACTIVITY records in HLD status that are for activities relating to payment types. Payment Type activities are identified by the definition of ACCOUNTING in the Activity Type of the underlying ACTIVITY.CLASS.

The requests are submitted to OFS in zero authoriser mode. In the case of error or override, the transaction remains in HLD status and must be processed manually.

The AA.ARRANGEMENT.ACTIVITY $NAU table is selected. The record processing determines that:

- The record status is HLD
- The activity is a payment type

If both cases are true, then the activity starts processing.


> **Related Applications:** `AA.ACCRUAL.FREQUENCY`, `AA.ACTIVITY.CLASS`, `AA.ARRANGEMENT.ACTIVITY`, `AA.DECISION.PARAMETER`, `AA.INTEREST.ACCRUALS`, `AA.NEXT.ACTIVITY`, `AA.SCHEDULED.ACTIVITY`, `ACCR.REV.PARAM`, `BASIC.INTEREST`, `EB.ACCRUAL`, `PERIODIC.INTEREST`, `TSA.SERVICE`

---


### 1.3  Charges and Commissions


> **📇 Quick Reference Card**
> 
> **Sections:** 🔧 Working With


#### 🔧 Working With

The users can configure the charges to be due on the first, next, or last payment. The charges are triggered on occurrence of a specific activity and it is due to the customer as per the configuration.

If a user has set the charge collection on the next payment, but the system levies the charge on creation of the contract, it is still due only on the next payment date, that is, it is not due immediately. It is scheduled to be collected on the first payment date as per the schedule configuration.

Alternatively, if a user configures the collection of charge on the first payment, but the first payment date lapses when the customer triggers an activity, the system raises an override and schedules the charge along with the next upcoming payment.


##### Collecting Fee for External Event

The Record Event activity class registers an external event manually in the system. In asset financing, the financial institution can collect a delivery fee when the asset is delivered to the lessee or customer. This is an external event and not connected to the system. The user can manually register the event in the system using ASSET.FINANCE-RECORD.EVENT-ARRANGEMENT. Similarly, below activities are used for collecting charges for external events:

- Failed collection of the asset: At the end of the term, if the lessor is unable to collect the asset, the financial institution levies a charge for the failure of collection of assets. The activity can be registered in the system using ASSET.FINANCE-RECORD.FAILED.COLLECTION-ARRANGEMENT activity. A failed collection fee is levied on the arrangement when the user triggers this activity manually.
- Payment return fee: Lease payments scheduled for collection from an external system might fail due to various reasons like account unavailability or insufficient funds. System triggers ASSET.FINANCE-RECORD.DD.RETURN-ARRANGEMENT activity to register the payment failure. The user can configure a payment return fee on occurrence of this activity.

User creates an arrangement with the condition that the system collects the delivery fee when the ASSET.FINANCE-RECORD.EVENT-ARRANGEMENT activity is triggered.

Delivering the asset to the lessee is an external event. The user triggers ASSET.FINANCE-RECORD.EVENT-ARRANGEMENT in the system to register this external event. System prompts an alert message that a fee is levied for the activity.

System schedules the delivery fee to be collected along with the first payment.

---


### 1.4  Hybrid Pooling


> **📇 Quick Reference Card**
> 
> **Key Fields:** *AA Bundle ID*, *Align Dates*, *Alt Acct Id*, *Alt Acct Type*, *Alt Id Type*, *Alternate Id*, *Alternate Id Type*, *Back-to-Back FX* ... +27 more
> 
> **Sections:** 🔧 Working With


#### 🔧 Working With

The below are the different process to create a hybrid cash pool:

| Process | Activity | System/User |
|---|---|---|
| Create pool in pending live | BUNDLE-NEW.OFFER-ARRANGEMENT | Orchestration service |
| Create accounts in pending live | ACCOUNTS-NEW.OFFER-ARRANGEMENT | Orchestration service |
| Set go live date for pool | BUNDLE-UPDATE.LIVE.DATE-PRODUCT.BUNDLE | User |
| Set go live date for accounts in pool (be spoke) | BUNDLE-RESTRUCTURE-BUNDLE.HIERARCHY | User |
| Bring accounts to Live | ACCOUNTS-NEW-ARRANGEMENT | Scheduled by orchestration service and processed by COB orchestration process |
| Bring pool to live | BUNDLE-NEW-ARRANGEMENT | User/CB Orchestration process |
| Add standalone account | ACCOUNTS-TRANSFORM-ARRANGEMENT | Scheduled by orchestration service and processed by COB orchestration process |
| Remove pool account | ACCOUNTS-TRANSFORM-ARRANGEMENT | Scheduled by orchestration service and processed by COB orchestration process |
| Close pool account | ACCOUNTS-SETTLE-PAYOFF | Scheduled by orchestration service and processed by COB orchestration process |

This section describes the steps and sequences to be followed, to manually create the various account part of a BN pool structure.

The navigation is as follows,

- Product Catalog.
- Select Product Catalog from the User Menu

> **⚠️ Note:** These accounts (including the master account bundle arrangement) can be created forward dated. They are activated by the system at SOD on that date.

Create CT accounts in the desired currencies.

- Switch off settlement instructions on pay-in and pay-out sides.

Create a new bundle arrangement under the master account product.

- Attach the CTs to the product bundle.
- Identify the currency of the master account and choose the corresponding CT account to be the recipient of the bundle.

Create summary or transaction account in the order of the hierarchy.

- The parent must be created first before creating the child.
- If TR1 has its parent as CS1, which has its parent as SA1, then SA1 is created, followed by CS1 and then TR1.
- Once an account is created, its parent can only be set or changed through the purpose built internal restructuring activity.
- Normal Update-Account activity cannot be used.
- Similarly, once an account is created, the bundle arrangement (master account) and link account number (CT account) can be updated through the purpose built External Restructuring Activity.
- Switch off settlement instructions on pay-in and pay-out sides.
- Once the accounts are created, the normal workflow on updating their conditions are to be followed through the arrangement overview. The new activity drilldown links to setup, Bank interest or fees or schedule and settlement Internal interest or fees or schedule and settlement conditions.


###### Generating IBAN

When the Bundle for the master account product is created in Draft status and when it is subsequently moved to the New Offer status, the IBAN is generated based on the values defined for Generate Iban and Alt Id Type . The IBAN can be seen in the AA.ARRANGEMENT record of the underlying contract.

As displaying the entire IBAN Value on the card is not feasible, it displays few characters of IBAN and appends it with three dots , for example, GB12DEMO60161300087537 is displayed as GB12DEMO6061…; on hovering over the text it displays the full string value.

The Alternate Id Type and Alternate Id of the Alt Id Types can be viewed in the expand header of each card. For the accounts other than master, T24.IBAN value gets displayed on the card instead of Account ID. If T24.IBAN value is available, the Alt Acct Type and Alt Acct Id get displayed on the expand card header.

When creating the CT accounts except for Limit (in case of MCCFor SCCF or MCF or SCF) is updated, no other special attribute needs to be specified to attach it to a master account, since it is done through the UPDATE-PRODUCT.BUNDLE activity. The user does this activity directly on the bundle arrangement (master account).

Once the CTs and MAs are created, when creating SA or CS or TR or MTR, it is important to capture the pool and hierarchy details via the purpose built attributes in Account property.

The following is a screenshot of a TR being created new, attached to an existing Pool under SA1 as its parent. The navigation for this could either be from the Product Catalog or the Master Account Overview.

The Master account is the bundle arrangement.

- If the account added or created is in a different Temenos Transact company than the master account, then the master account reference must be captured suffixed with its company mnemonic. In the example above, since the master account is in Temenos Transact Company BNK, it must be captured as AA1710732QS1/BNK for the system to recognise it.
- Linked Account number is the CT Account. If left blank and if a valid CT in this currency exists, then the system would default it. If a value is entered, the system validates that it is a valid participant in this Bundle Arrangement and that its currency matches this account’s currency.

- Parent account is used to capture the parent in the hierarchy. It is an optional field and when left blank, it mean the account being created would be added to the pool directly under the master account level.
- If a value is entered, the system would validate that it is, A valid member of the Bundle Hierarchy An allowed parent of this account Enabled for multi-currency if its currency is different from that of this account’s currency

In case of opening CS or SA, the above rules hold true except for the Linked Account Number (for which input is allowed).

The accounts in the BN pool can be internally moved (at any point). To facilitate this, the ACCOUNTS-CHANGE.PARENT-ARRANGEMENT activity is initiated from the New Activity menu.

During this process happens, the balances from the previously linked parent account is also transferred.

The above screenshot shows a TR account linked to SA account 2000003347. The SA and linked TR account’s balances are the same.

From the New Activity menu in the TR account, the User activity ACCOUNTS-CHANGE.PARENT-ARRANGEMENT is initiated.

For a restructuring, this activity runs at COB, hence, the Effective Date needs to be day + 1. The new parent account is changed to 2000003355, which is the new SA account. After authorisation and a COB is run, the restructure process is initiated.

The above screenshot shows that the balance (USD 88,592.08) is moved from (2000003347) to (2000003355) account.

This section enables the user to understand creation of BN pool.

BN structure creation process starts from creating a master arrangement in a draft status. The user can provide the necessary details to create the master arrangement by selecting the NEW STRUCTURE tab in Graphical User Interface (GUI). Mandatory information is Product Name, Country (on which the Master arrangement is created), Currency (master account) and Structure Name (optional).

To create a new BN structure, from the GENERAL TRADING screen,

1. Click NEW STRUCTURE .
2. Enter the mandatory information and then click CREATE . The master arrangement is created in view mode.
3. Click to add new accounts to BN structure. The symbol is enabled.
4. Click to add new accounts to the BN structure. The Add Account to Structure pop-up window opens.
5. Select the respective account type to add a new accounts to the pool. Standalone accounts can be selected and added to the BN structure by filtering the accounts by Currency.
6. Click to add multiple accounts to the pool. Example: To add two SA accounts, select the currency and company from the drop-down list. Once the account placed holder is created, click OK to create the placeholder card in GUI.
7. Click Save to save the BN pool structure in GUI. GUI passes the information to Temenos Transact to store the placeholder details. The user can save the changes in GUI after the BN pool structure is approved by corporate. When the user saves the Master arrangement in GUI, Temenos Transact does not any validation.

The BN structure can be edited and updated with new accounts and removal account by selecting the edit options. The Draft BN structure can be edited with the following details.

- Adding new placeholders
- Removing placeholder accounts
- Changing Parent details
- Adding Standalone accounts
- Adding a new parent placeholder for child accounts

Click Validate and Commit . The CT placeholders are created automatically. CT account is opened in Master account company for each currency of TR accounts.

To disconnect account placeholder, Click on each cards. The account card is removed immediately from the BN pool structure. When the Summary Account (SA) or Currency Summary (CS) placeholders are removed from BN pool, the child accounts are linked to the immediate parent. The parent accounts can be removed along with the child accounts from BN pool.

> **⚠️ Note:** Account number is not generated in Temenos Transact, hence the conversion of TR account to standalone is not possible.

To add standalone accounts to BN pool, click on the respective cards.

> **⚠️ Note:** This icon is enabled only for Master or SA or CS accounts.

Standalone accounts can be added under SA and CS account or directly under the master arrangement without any parent. Until the BN pool becomes live, the standalone account terms and conditions remains the same. Once the live date reaches, the account is converted to TR and the new product conditions applies. The account number remains the same as standalone account and only the change product activity is triggered.

Export. The BN structure can be exported as PDF, HTML, Excel, Power Point and Word. The exported BN structure is produced with the corporate customer for any modifications or changes in the structure. BN structure can be exported during Draft, Preliminary and Live status.

Go Preliminary to move the pool to preliminary. To move the pool to Preliminary status, the Pool Orchestration Service is run after committing the Activity. Once the Go Preliminary is triggered on a particular BN pool, the user can click on top-left and GUI displays the GUI landing page.

Once the preliminary process completed, the status of BN pool structure is moved and updated as Preliminary. Account number is generated on each placeholder and appears on each cards. Temenos Transact generates CT account automatically for each currency of TR accounts.

Click Edit to update the Terms and Conditions.

This section enables maintenance of cover control

This option is available in Tools menu. Click Edit to update the cover control setup. Accounts part of BN pool are listed as tree view and the changes can be updated in each account. Cover control on CT accounts are not applicable and hence the options are not enabled. Enable Apply settings to sub-structure to copy the cover control setup to child accounts.

Credit check is set for internal or external transactions or both. When the options is Null, the credit is applied during the transaction processing. Click Save to update the changes in Temenos Transact.

Click Edit to add new SA,CS,TR or MTR accounts in preliminary BN structure. The similar process is followed in Draft to add new accounts in preliminary. The user can commit the changes once the placeholders are created. Once the BN pool is committed in GUI, account number is generated immediately in Temenos Transact and appears on each card. The user can update the terms and conditions for the new account created in BN Pool.

To sets the Global Go Live Date from CARD VIEW Click Go Live on top-right of the BN Pool structure in GUI.

In the below screen, the Global Go Live is set for Bundle arrangements and the custom Go Live date option is for individual accounts part of BN Pool structure. Set the Global Go Live Date first and then the customer go live date, else an error message is displayed. Custom Go Live date is an optional input, participant accounts in BN pool goes live with the same date as Master or Bundle go live. When the go live date is set for individual accounts, then the accounts are live only on that particular date. Transactions are not allowed until the accounts are moved to LIVE.

The Custom go live date can be the same as Master live date as or later than Master live date. Temenos Transact displays an error message when the customer go live date is before Master live date.

This section enables maintenance of CT Accounts

CT Account

CT accounts provides static information of accounts such as CUSTOMER NAME, CUSTOMER ID, ACCOUNT NUMBER, STATUS and SCHEDULED CHANGES. CT expand card also has an option to setup or amend the interest conditions. When the limit is available for the CT account, GUI allows editing of limit on CT accounts.

CT Account Transactions

CT Account balances

Limit Conditions

To update or amend the limit records, click Edit. Once the changes and amendments are done, click Commit to submit the changes in Temenos transact.

Interest Conditions

Click Interest conditions on CT account in expand view, the version of Interest calculations are launched. The interest activity can be set with immediate effort or for a future effective date. On committing the changes, GUI passes the information to Temeons Transact to update interest details.

Summary Account/Currency Summary

SA account provides the static information of accounts such as CUSTOMER NAME , CUSTOMER ID , ACCOUNT NUMBER , STATUS and SCHEDULE CHANGES . It provides the combined balances of all the child accounts linked under the SA accounts. It is multi-currency accounts; hence, any allowed currencies can be linked to SA. When the SA account is having a multi-currency child accounts, then the balance is combined to SA account currency. SA expand card can setup or amend interest conditions and internal cover control.

When the user clicks on Interest condition, the respective version is launched to update the internal interest conditions. Manage Limit option allows the user to setup the internal and external cover control. Manage limit version is launched and the GUI allows to update and commit the changes.

TR Account

Expanded view of TR account provides the static information of accounts such as CUSTOMER NAME , CUSTOMER ID , ACCOUNT NUMBER , STATUS and Schedule Changes. TR account provides the balances and transactions of the respective TR accounts. The user can view the transactions by providing the start and end date. TR expand card can setup or amend interest conditions and internal cover control.

When the user clicks on Interest condition, the respective version is launched to update the internal interest conditions. Manage Limit option allows the user to setup the internal and external cover control. Manage limit version is launched and the GUI allows to update and commit the changes.

TR Account Transfer Services

Setting Future Internal STO/Sweeps

On selecting the Transfer services, the process remains the same. Refer Transact process flow.

When the CT Accounts are created (except for Limit in case of MCCF or SCCF or MCF or SCF) are updated, no other special attribute is specified to attach it to a master account using the UPDATE-PRODUCT.BUNDLE activity. The user does it directly on the bundle arrangement (master account).

When the CTs and MAs are created and when creating (SA or CS or TR or MTR), the pool and hierarchy details should be captured using the purpose built attributes in Account property.

The below screenshot shows a new TR attached to an existing pool under SA1 as its parent. The navigation for this is from the Product Catalog or the Master Account Overview.

The master account is the bundle arrangement.

When the account added or created is in a Temenos Transact company different from the master account, the master account reference should be captured and suffixed with its company mnemonic. In the above screenshot, since the master account is in Temenos Transact company BNK, it must be captured as AA1710732QS1/BNK for the system to identify.

Linked Account Number is the CT account. If this field is left blank and when a valid CT in this currency exists, then the system defaults it.

- When a value is entered in this field, the system checks if it is a valid participant in the bundle arrangement and currency matches the account’s currency.

Parent Account is used to capture the parent in the hierarchy. It is an optional field and when left blank, the account created is added to the pool directly under the master account level. When a value is entered in this field, the system validates if it is,

- A valid member of the bundle hierarchy
- An allowed parent of this account
- Enabled for multi-currency (if the currency is different from that of the account’s currency)

> **⚠️ Note:** The above rules hold true when opening CS or SA, (except for the Linked Account Number for which input is not allowed).

The AA.BUNDLE.HIERARCHY.DETAILS (system maintained table) is used for any investigation or analysis purposes or to know the pool structure on a given date.

85308 is the top most summary account and the grand parent of 85332, 85348, 85359 and 85367 (all from the same company) and also a parent of 2000003266 (from a different company). This illustrates that the pool hierarchy can contain accounts across borders ( Temenos Transact companies or books).

Posting transactions on a BN pool is possible through the transaction account (that has External Posting set as Yes).

> **⚠️ Note:** The system blocks any direct posting on CS or SA or CT.

Whenever a transaction is posted in a TR account, the core accounting engine does the following:

- Makes a posting on the TR as a memo posting and diverts it as a real entry in the corresponding CT account (specified in Link AC Number field in Account Property)
- Replicates the same memo entry in the parent of the TR (specified in the Parent Account field in Account Property) and its parent and so on up to the top level parent.

Internal or external transactions are controlled by the Transaction Type attribute in TRANSACTION table. This and the internal cover control attributes in Limit property class drives the validations on these transactions for TR or CS and SA accounts.

| Account Type | Company Name | System Date |
|---|---|---|
| CT account (100001) | Temenos core banking Norway company | 25/10/2017 |
| TR account (100002) | Temenos core banking Norway Sweden | 23/10/2017 |
| TR account (100003) | Temenos Core Banking Norway Finland | 24/10/2017 |

To make a bundle go live, enter the current or future date in the Master Live Date field.

- If the current date is given, run the AA.POOL.ORCHESTRATION.SERVICE service to make the pool go live online.
- If the current date is given but service is not run, the bundle does not go live during the End of Day processes. In this case, to make the bundle go live, enter the current date, the following day (and run the service), or a future date in the Master Live Date field .
- If a future date is given, the bundle goes live during the SOD process of the given date.

When a pool structure (bundle arrangement) is created, subsequent maintenance activities either at Pool or individual account level can be carried out from the bundle arrangement overview.

Find Bundle Arrangement

The spectacles icon takes the user to the arrangement overview

Bundle Arrangement Overview

The New Activity lists the user activities that are performed at the bundle level. This is used to launch the Update Product Bundle activity to add more CTs to the master account.

The Bundle Participants section lists the CT accounts that are part of the master account. The spectacles icon drills down to the respective CT account arrangement overview

The Hierarchy section of the bundle arrangement overview lists the various accounts that are part of the hierarchy. The spectacles icon drills down to the respective account arrangement overview.

The Add A/C to Pool tab allows user to add different types of accounts to the pool. This is to provide easy access from the bundle overview and requires customisation of the enquiry based on the products displayed.

The settlement property specifies the default settlement (in the case of CS/SA/CT) and counter booking account (in the case of TR/CS/SA). Navigate from the bundle overview into the respective account overview, the user can launch Update-Settlement activity from the New Activity List.

For example, counter booking for a TR account.

New Activity List

The below screenshot shows a default settlement account for a CS

When the settlement account is specified, the relevant pay in or pay out settlement instructions need to be switched on by setting the value to Yes.

The user navigates to the respective account arrangement overview and New Activity List to launch the Update Limit activity to set internal limit for a TR/CS/SA.

The below screenshot shows an internal limit on a TR

Setting the Internal Limit to 1,000.00 results in the maximum debit balance on this account to be 5,000.00.

Even though the Group Balance is close to 1 Million USD + 10 Million in Credit Facility, debiting USD 6,000.00 from this Account would result in the following override message.

To set a restriction of limit utilisation by a CT on shared limit, the user can navigate to the respective Account Arrangement Overview and select the New Activity List to launch the Update Limit activity.

The below screenshot shows Bundle Participants in bundle overview:

The below screenshot shows a New Activity on CT Account Overview

Update limit to restrict maximum utilisation of the available balance by the EUR CT to EUR 15,000.00.

The financial summary of the EUR CT is shown below:

The account balance of the EUR TR is shown below:

Debiting EUR 20,000.00 from TR results in this limit excess message on the EUR CT account 85294.

| Column 1 | Column 2 |
|---|---|
| Interest all types (credit or debit or special) | The system calculates an up-to-date accrual of each individual interest property. Makes required adjustments to any of these interest properties. Honours adjusted periods, that is, a forward dated effective date. |
| Tax on interest | When defined, the system calculates all tax up to this point on each individual property. |
| Charges all types (periodic or scheduled or activity) | The system calculates all types of charges up to the effective date. Makes up-to-date accrual of the individual charge properties. Evaluates all activity charges. |
| Tax on charges | The system calculates all tax up to this point on all charge properties. |
| Evaluate all activity restrictions | Per product definition, any defined rules need to be honoured. |
| Evaluate and generate any associated messaging | Per product definition activity messaging generates the appropriate advice. |
| Evaluate all current core services attached | A validation report is generated. |
| When the calculated balance is negative, validation shows an error. | Manual steps are needed to bring the balance into credit. The process can then be run again. |

The accounts in the BN pool can be internally moved at any point. To facilitate this, the activity ACCOUNTS-CHANGE.PARENT-ARRANGEMENT is initiated from the New Activity menu.

When this process happens, the balances from the previously linked parent account is also be transferred.

The above screenshot sows a TR is linked to SA account (2000003347) and this SA account has the same balance as the linked TR account.

New Activity menu from the TR account, the User activity ACCOUNTS-CHANGE.PARENT-ARRANGEMENT can be initiated.

For restructuring, this activity happen during COB, hence, the Effective Date should be day +1.

The new parent account is changed to 2000003355, which is a new SA account.

After authorisation and a COB is run, the restructure process is initiated.

A balance of USD 88,592.08 is moved from (2000003347) to (2000003355) account.

BN Pool accounts can be moved from one parent account to another parent accounts. To move an account, select the respective account, click and click Move account . Once the account is selected to move, select the target account and click Paste . When the account is already in Draft or Preliminary, the account is moved to the target parent immediately.

Select the target parent account and click Paste . When the account is in preliminary, the account is moved to the target parent account immediately.

Account 2000003328 is moved to the new parent, that is, bundle arrangement.

If the account is in Live, then the account is moved on the next working day or with a future business date. The account remains with the existing parent, terms and conditions remains the same. Once the system reaches the schedule date, the account is moved to the new parent.

Intra-cash pool movement of the Sub-structure (GUI)

To move the sub-structure from one parent to another parent account, right-click the account that needs to be moved the new parent. New dialog box appears with confirmation, whether the account wants to be moved with sub-structure or only with the selected account. By clicking on Also move sub-structure , the entire sub-structure is moved to the new parent.

Temenos Transact scheduled a new activity and the account is moved on the scheduled date. Hover on the card to view the change parent details.

Financial institutions collect charges on master cash pool account, which is the master arrangement for the pool hierarchy, even when master cash pool account is a non-financial product.

Temenos core banking suite levies charges on master cash pool account (non-financial product) by extending the functionality of some of the property class to the bundle product line.

The charges levied on master cash pool account is posted to the nominated financial settlement account.

- Bundle account /master account detail = Arrangement No AA17132HJ8T0
- Settlement account detail = Arrangement No AA171323JK92, account no 85073
- CT account detail = Arrangement NO AA17131SVQ33, account no 85057
- For the above master account following charges are configured
- Subscription and setup fees are fixed as USD 1000 and EUR 500 respectively.

The below screenshot shows the Master Account overview:

The setup fee is configured as fixed amount of EUR 500 for this bundle accouent.

Subscription fee is configured as fixed amount of USD 10000 for this bundle account.

Schedule for collection of subscription fees is 3 days.

Defined default settlement account is 85073.

Defined settlement account 85073

Charges are levied on master account, debited to default settlement account as shown below:

> **⚠️ Note:** Difference in the charge amount for setup fee is due to the currency difference.

| Column 1 | Column 2 | Column 3 |
|---|---|---|
| Account Number | DR/CR | Amount |
| 12345 | DR | EUR 1,000 |
| 67899 | CR | USD 1,0811.77 |
| 22333 | CR | EUR 1,000 |
| 44555 | DR | USD 1,0811.77 |

When the user updates rate through Preferential Pricing FX condition, (with a date effective in the future), the new rates are available to all TRs from that date.

When the user updates rate in Preferential Pricing FX condition, with a date effective in the past (T-3),

- Existing transfers are not recalculated.
- New internal FX transactions takes rates effective as of the booking date.

The system automatically closes the pricing arrangement on static review, if the customer is no longer eligible for this pricing arrangement

- This would happen as the Eligibility rules for the Internal FX Pricing arrangement are the same as that of the Master Account.
- When a customer is not eligible to open a master account, the customer is not eligible to have an internal FX pricing arrangement either.

| DR | CR |
|---|---|
| EUR TR 1,000.00 | Contra EUR TR 1,000.00 |
| Contra USD TR 1,250.00 | USD TR 1,250.00 |

In the CUSTOMER.MASS.BLOCK application, the user can provide the AA Bundle Arrangement ID in the AA Bundle ID field to block all the accounts, which are part of that bundle for transaction processing.

In case of BN, by entering the AA Bundle Arrangement ID and committing the record, all currency top accounts, which are part of that bundle is blocked for transaction processing (posted against transaction accounts, which are part of the same BN structure).

Example: A BN structure is created in the system with master account arrangement bundle ID as AA171075RFH6.

This bundle arrangement has two currency top accounts: AA17107RHMWK (EUR) and AA17107BB6H6 (USD).


###### Block Entire Cashpool structure (GUI)

To block the entire BN structure, select Emergency Block from Tools menu. Select SUSPEND CASHPOOL to block all accounts, which are part of the respective bundle for transaction processing.

> **⚠️ Note:** To block the BN pool, Start date is a mandatory field. Expiry date is an optional field.

Suspend can be done with future start date and expiry date. Once the Temenos Transact reaches the particular Start of Day (SOD), all the accounts which are part of that Bundle are blocked for Transactions. Fund transfer, standing order and sweeping scheduled (between the accounts in the bundle structure) are also suspended.

Once the BN pool structure is blocked, further maintenance on accounts is also suspended and the structure blocked message is displayed.

To unblock the BN structure, select Unblock Structure from the Tools menu. Enter the date in the Expiry date field and provide the reason and click UNBLOCK STRUCTURE button.

> **⚠️ Note:** The date in Expiry date can be current or future date and when,

- Current date is provided, the structure is unblocked immediately and the user can perform transactions on BN accounts.
- Future date is provide, Temenos Transact removes the blocked status during the start of day of the particular end date.

To block the sub-structure, Select Emergency Block from Tools menu and click BLOCK ACCOUNT OR SUB- STRUCTURE . By selecting the parent accounts GUI blocks the child accounts linked under the parent account. In Temenos Transact child accounts are not blocked and only parent account is blocked. When the user initiates the transaction on TR accounts, Temenos Transact displays an error message and further transactions are not allowed. Enter date in Start date and Expiry date fields to block the sub-structure and a particular account. Temenos Transact allows to block the sub-structure or an account with future start date and end date.

When the user selects the parent account, the child accounts linked under the parent are selected automatically and in GUI, the status is shown as blocked.

Once the sub-structure and accounts are blocked, the status is updated on each account and the tool tip is shown on each card with the date on which the account is blocked. When the parent is blocked, the child account details are also updated as blocked in GUI.

Block details are updated in card and tree view.

To unblock sub-structure or an account, select Unblock Account or Sub Structure . The blocked accounts are selected by default. The user can deselect an account when there is no need to unblock. Enter the Expiry date and click UNBLOCK ACCOUNTS to commit the changes in Temenos Transact. Expiry date can be current or future dated. When current date is used to unblock the account, it is unblocked immediately and Temenos Transact allows to initiate transactions.

BN pool GUI structure is refreshed with the changes in Temenos Transact and the blocked status is updated in GUI. Once the account is unblocked, the strike line on an account is removed immediately.

A CUSTOMER.MASS.BLOCK record is created to block the two CT accounts starting 18 April 2017, until 19 April 2017.

By giving the bundle arrangement ID and committing this record, the CT accounts are blocked and no transactions are posted against any transaction accounts linked to these currency top accounts.

The accounts are unblocked by giving the expiry date and an unblocking code.

A BN structure is created in the system, having a master account arrangement bundle ID as AA171075RFH6.

This bundle arrangement has two currency top accounts: AA17107RHMWK (EUR) and AA17107BB6H6 (USD).

A TR account can be disconnected from a BN pool and then it can be ultimately closed. In such cases, the balances, capitalised interest and charges are transferred to another account.

The general process to disconnect and close an account from the BN structure is as follows:

- The user switches the TR account from off balance sheet to on balance sheet. This is done when user executes an activity to remove the TR account from the pool, a change product is also executed.

> **⚠️ Note:** When closure is attempted, validation is done to confirm that link to the BN pool is removed. If not, a related error is displayed.

Click here to refer Arrangement Closure.

These reports are accessible through the Corporate Single Customer View (SCV) of corporate user menu under balance netting or in the role based home page for balance netting administrator.

The key reports are explained below.

This report provides an overview on the latest terms and conditions registered in the account. The details include cover control, internal or external credit limits, payment restrictions and blocked amounts.

The details provided in this report are:

- Account type
- Account number
- Currency
- Date for latest modifications
- Cover control (on/off)
- Capitalisation account
- Frequency of capitalisation
- Settlement account
- Deposit interest (margin and base rate used)
- Deposit fee (negative interest as a fee)
- Lending interest
- Lending fee
- Unauthorised overdraft interest
- Unauthorised overdraft fee
- Penalty fee (in regards unauthorised overdraft)
- Day method
- Inheritance
- Thresholds
- Blocked amounts
- Unable to check if conditions and terms seen are internal or external

When the user selects several accounts, the search can be limited to comprise only accounts in a certain currency.

The below screenshot shows the terms and condition of master account - Interest:

The below screenshot shows the terms and condition of master account – Charge:

The below screenshot shows the terms and condition of master account – Schedule:

The basic account information per current day for a BN cash pool account are shown below:

- Account type
- Activation date
- Disconnected date
- Date for latest modifications
- Scheduled event(s) and the date for it
- Account number both BBAN and IBAN format
- Account country (that is, the country in which the account is located)
- Currency
- Balance reporting (which type, for example, account statements such as MT940, MT941)
- Frequency of the statement (for transaction accounts only)
- Parent account
- Settlement account
- Capitalisation account
- Customer name
- Customer ID

> **⚠️ Note:** The closure date is also displayed for closed accounts.

The below screenshot shows that a search on master account displays the summary and currency summary account and transaction account in the hierarchy.

The user Credit report for BN accounts is available with the below details:

- Account number and account type
- Limit attached to accounts within the structure
- Type of limit
- The size of the limit
- Currency of the limit
- Interest and fees linked to the limit
- Automatic renewal
- Placed securities (type of collateral)
- Registration date
- End date
- Renewal date

The below screenshot shows that a search on master account displays the summary and currency summary account and transaction account in the hierarchy.

This report displays all the internal cash pool services that are linked to the accounts in the hierarchy.

- Automated balance transfer
- Internal automated balance zeroing
- Internal FX balance transfer
- Internal standing order

The below screenshot shows that a search on master account displays the summary and currency summary account and transaction account in the hierarchy.

The following details are found for a selected balance netting account:

- Account number and account type
- Interest type
- Accrued interest
- Capitalised interest current year
- Capitalised interest previous year
- Capitalised interest latest period
- Date for latest capitalisation
- Specification of accrued interest
- Internal interest calculated but requested not to be capitalised for the current year
- Internal interest calculated but requested not to be capitalised for the previous year
- Internal interest calculated but requested not to be capitalised for the latest period

The below screenshot shows that a search on master account displays, the summary and currency summary account and transaction account in the hierarchy. The results can be exported to an excel.

The user can extract information on structural changes in a hierarchy at account closed and accounts moved level. The latter is within a structure or to another BN structure in a bank. Only live structures apply for structural changes (not draft or preliminary).

A below report on structural changes of all MA bundles in Temenos Transact are:

- The list is sorted by MA bundle owner and not by the change.
- Specify the account type taking part in the structural change
- Specify the type of structural change (add, delete and move)
- Specify if the structural change is conducted by a bank user or the customer
- Specify the ID of the user who registered or entered the change
- Account number and customer ID of account involved in the structural change
- If account is moved, then the user should specify the parent account number to which the account is moved ( MA /SA/ CS)
- The go live date of the structural change
- The date the structural change was registered
- Total number of structural changes (aggregate of added, closed and moved respectively) in each MA bundle. This can be used to simplify charging the customer of the structural changes.

A report on structural changes in a specific MA bundle:

- State the MA bundle the structural changes are extracted from
- Specify the account type taking part in the structural change
- Account number and customer ID of account involved in the structural change
- Specify the type of structural change (add, delete and move)
- Specify if the structural change is conducted by a bank user or the customer
- Specify the ID of the user who registered/entered the change
- If account is moved, specify to which parent account number the account is moved ( MA /SA/ CS)
- The go live date of the structural change
- The date the structural change was registered
- Total number of structural changes (aggregate of added, closed and moved respectively) in the specific MA bundle. This is done to simplify charging the customer of the structural changes.

This report displays all transactions (booked during the given period of dates) and transfer details (such as, reference number) if attached to the payment.

If a TR is moved from one structure to another and the search date is before start date in new structure, the system displays the historical transactions only for searches on TR account.

Transactions can be filtered by:

- Transactions within a certain currency
- Customer internal transactions
- Intra-cash pool transactions
- Transactions between certain amounts
- All debit and credit transactions

A search on master account displays the summary and currency summary account and transaction account in the hierarchy

The Integrity Check Days attribute in Bundle Hierarchy Property Class is used to schedule an evaluation on ‘n’ number of days before an event is triggered in the bundle.

The first integrity check is run ‘n’ number of days before go live date for a pool in preliminary status.

This validation runs on continuous basis ‘n’ number of days before every event in the Bundle.

> **⚠️ Note:** Integrity check days are calculated as ‘n’ working days.

- Integrity check orchestrates the validations from MA level to the underlying accounts in the hierarchy.
- The system triggers the Activity Class BUNDLE-INTEGRITY.CHECK-ARRANGEMENT to run the integrity check.
- The user can trigger ad-hoc integrity checks by manually running the activity class for integrity check. The system automatically runs the pool orchestration service and generates integrity report.

- Validations are run on the bundle and results are recorded in AA.POOL.EXCEPTION.LOG. The record ID is Arrangement Number-INTEGRITY.REPORT.

- It is possible to query on this table using the bundle (arrangement) number. This displays a single screen that contains all the validations related to all the accounts in the bundle, especially the failures

- Drilldown to the individual accounts are available to take correction actions.

The below are the validations based on pool events.

A complete scan is carried out when go live date is set.

When the live date is given (not null), the scan is carried out at the pool level.

- Pool cannot go live without even a single CT.
- CT cannot exist without MA and TR.

The system validates,

- If the bank is working on the dates in which pool has tasks scheduled at SOD
- If previous calendar date is a working day

- A warning message giving the childless CS or SA or CT is closed automatically
- Currency availability in weighted rate calculation (CT and SA) CT: When 4 CTs are in bundle but only three currencies are specified in custom type in Recipient CT Interest property, then exception message is raised for the missing custom type in that currency SA: Validates if all the currencies for which balance is maintained in ECB, are specified in the custom type

- Currency market rate for currencies in secondary currency market Takes recipient’s secondary currency market, and scan through CURRENCY table in recipient CT company for each allowed currency of the bundle and see if there is a rate definition for this secondary currency market. An exception is recorded for the missing rate definition

- Settlement account validation All properties, payment types have settlement accounts (payment schedule, activity charges and rule break charges) Settlement and counter booking belong to the same pool and currency, the status of those accounts for the date (this account’s go live date atleast) required Settlement account specified in bundle settlement Settlement instruction switched on (if not, warning message) Settlement and counter booking account should be available for the go live date of the CS or SA or TR During new offer of SA or CS, a new offer TR can be attached as a settlement account but it must be set to go live for the SA or CS Go live date

When an account is linked to the pool, the below validations are performed:

- External sweeps are set for the account
- External STOs are set for the account
- Account with negative balance (error is raised when TR account is linked)
- AC pre closure validations are performed
- Account is scheduled for closure TR has external sweep or STO

When an account is delinked from the pool, the below validations are performed:

- Internal sweeps are set for the account
- Internal STOs are set for the account
- AC Pre closure validations
- Account scheduled for closure TR has internal sweep or STO

During the closure of an account, the below validations are performed:

- Negative balance in account
- Sweeps setup in account
- Accounts has a record already in AC block closure


###### Closure of entire pool structure (GUI)

BN pool can be closed during Draft, Preliminary and Live status. To close the BN pool structure, right-click the 3 dots on Master card and select Close Entire Pool . Closure of live BN pool online is not possible. It is possible on the next business day or on a future date.

Closing the preliminary BN pool is done online and future scheduling is not possible. Master arrangement and SA, CS, TR or MTR accounts linked to the pool is closed online and Tree or Card view is updated accordingly. GUI displays a warning message to the user before closing the entire BN pool. When the user clicks on YES, GUI passes the information to Temenos Transact and the accounts are closed.

Cross pool event go live date against destination pool go live date and parent go live date is validated and exceptions are logged in case of breach.

> **⚠️ Note:** When these validations are not met, exception log is updated with a warning message.

Cross-pool movements of the Sub-structure

When arrangement is part of a hierarchy of accounts such as, a cash pool hierarchy, the arrangement interest, charge and capitalisation frequencies need to be set (not at product level but at another arrangement higher up in the hierarchy). In a cash pool structure, this means setting conditions for inheritance at the (parent or grandparent) or (pool or currency specific concentration level).This helps in easy maintenance of these conditions in a single place instead of having to deal with the individual arrangements at the lowest level, which also happen to be the normal transaction accounts.

---


### 1.5  Arrangement Pool Linking


> **📇 Quick Reference Card**
> 
> **Purpose:** *Pools are used to group the deposits or finance contract together, for distributing the profit earned from finance to the deposits. Linking deposit or finance contracts to pools allows the flexibility to define risk and rewards of the assets are clearly linked to specific pool.*
> 
> **Applications:** `ID.POOL.CONDITION`, `ID.POOL.PARAMETER`
> 
> **Key Fields:** *Appl Field Name*, *Default Pool*, *Define Pool ID*, *Description*, *Field Operation*, *Field Operator*, *Pool*, *Value From* ... +1 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Pools are used to group the deposits or finance contract together, for distributing the profit earned from finance to the deposits. Linking deposit or finance contracts to pools allows the flexibility to define risk and rewards of the assets are clearly linked to specific pool.

Islamic banks allows to create multiple pools based on risk and reward expectations of depositors. Islamic banks use each deposit pool for different maturity and duration and invests accordingly. Deposits and finance contracts are linked to particular pools for profit calculation and distribution according to banks liquidity management strategy.

Banks pool money from shareholders, depositors and savings account holders and invests in Shariah compliant projects or business. Here, the bank acts as a Mudarib (fund manager). Out of the profit made from the investments, the bank charges Mudarib fee for managing the funds. They deduct the reserves like Investment Risk Reserve (IRR) and Profit Equalization Reserve (PER) from the profit for future contingency purposes. The remaining distributable profits are paid to the depositors based on the weighted balance of the investments made.

The depositors can deposit in

- Restricted pools – The customer is informed about the investments made and it is called restricted Mudaraba.
- Unrestricted pool – The projects for investment cannot be disclosed and the bank can invest in any projects, which are Shariah compliant.


#### ⚙️ Configuration

When an asset or liability transaction is created, the pool ID should be captured. The user enters the pool ID manually or automatically by setting up the conditions in ID.POOL.CONDITION table.


##### UnderstandingID.POOL.CONDITION

This table is used to setup the conditions for defaulting pool ID in relevant applications. This table setup identifies the relevant pool based on file field names, field operation, and their values. When condition is not satisfied, the system allows the user to define the default pool and this pool can be linked to particular contract.

| Field Name | Description/Usage |
|---|---|
| Default Pool | Captures the default pool ID. If the conditions mentioned in the below fields do not satisfy, then the pool ID mentioned is defaulted. Allows a valid record from ID.POOL.PARAMETER . |
| Pool | Captures the pool ID to be defaulted, if the conditions mentioned in Appl Field Name , Field Operator , Value From , and Value To fields are satisfied. Allows a valid record from ID.POOL.PARAMETER . |
| Appl Field Name | symbol. |
| Field Operator | Captures the operator used during evaluation. Allows valid operators such as, Eq, Ge, Gt, Le, Lt, Lk, Ne, Nr, Rg, and UI. |
| Value From | Captures the starting value used for evaluation in Appl Field Name along with condition mentioned in Field Operator . |
| Value To | Captures the ending value used for evaluation in Appl Field Name along with condition mentioned in Field Operator . |
| Field Operation | Joins multiple condition for evaluation using and/or operators. |

| Column 1 | Column 2 |
|---|---|
| Description | Arrangement Condition |
| Default Pool | 2 |
| Pool | 1 |
| Appl Field Name | CATEGORY |
| Field Operator | Rg |
| Value From | 3010 |
| Value To | 3014 |


#### 📋 Tasks

Pools are used to group the deposits or finance contracts together for distributing the profit earned from finance contracts to the deposits. Linking deposit or finance contracts to particular pools allows the flexibility to define risk and rewards of the assets linked to specific pool and also for profit calculation and distribution according to banks liquidity management strategy.


##### Workflow

The user can perform the following activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Manual Linking of Pool ID . |
| Contract Screen | Enter a valid pool define ID in the Define Pool ID field. Format of the ID should be in the form of . For example, . Click the Edit icon. |
| Define Pool ID | Enter values in the following fields: Effective date Current Pool Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Authorise/ Delete/ View Pool ID Link . |
| Unauthorised Pool Define | Click the View icon corresponding to a record. |
| Define Pool ID | The system displays the details of Pool Define ID. |


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to Pool Movement.


##### Enquiries and Reports

The user can view the below enquiry

Pool Movement Tracker

This enquiry displays the pool movement history for a Finance or Deposit or an Account arrangement.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA


> **Related Applications:** `ID.POOL.CONDITION`, `ID.POOL.PARAMETER`

---


### 1.6  Islamic Accounts


> **📇 Quick Reference Card**
> 
> **Purpose:** *This topic enables the user to understand the Islamic account functionality.*
> 
> **Key Fields:** *Currency*, *Customer*, *Effective Date*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

This topic enables the user to understand the Islamic account functionality.


##### Mudaraba Savings Accounts

The saving account is defined from a Sharia perspective as a Mudaraba contract between

- Bank (Mudarib) who invests the client funds
- Client (Rab-ul-mal) who funds the account.

The two parties to this type of contract are capital provider or depositor and entrepreneur or bank. Bank intermediates the funds on a profit sharing basis into financing and investment activities. The profit from such a venture is shared between the two parties according to the agreed profit sharing ratio.


##### Mudaraba Daily Product Savings Accounts

It is a variation in savings account based upon the Mudaraba contract. Profit amount is calculated based upon the daily balance and tier or slab it falls in on each day. Daily accruals are posted by using the configured tier rate (Band or Level) and recalculate, pay the profit amount using the profit rate declared through Profit Distribution System (PDS).

| Month | Minimum Balance | Actual Balance | PDS Balance | Days | PDS Balance (Quarterly) | Average Balance | Rate | Profit |
|---|---|---|---|---|---|---|---|---|
| Jan | 5000 | 4500 | 0 | 31 | 0 | 0 | 6% | 0 |
| 01-Feb to 07-Feb | 5000 | 6500 | 6500 | 7 | 45500 | 505.5555556 | 6% | 7.479452055 |
| 08-Feb to 28-Feb | 5000 | 7300 | 6500 | 21 | 136500 | 1516.666667 | 6% | 22.43835616 |
| Mar | 5000 | 8000 | 8000 | 31 | 248000 | 2755.555556 | 6% | 40.76712329 |
|  |  |  | Total | 90 | 430000 | 4777.777778 |  |  |

| Calculation Criteria | Value | Calculation Criteria | Value |
|---|---|---|---|
| PDS Start date | 1-Jan-22 | PDS Start date | 1-Jan-22 |
| PDS End date | 31-Jan-22 | PDS End date | 31-Jan-22 |
| Number of days | 31 | Number of days | 31 |
| Minimum daily balance | 5000 | Minimum daily balance | 5000 |
| Daily balance from 01 Jan to 29 Jan | 8500 | Daily balance from 01 Jan to 29 Jan | 8500 |
| Daily balance from 30 Jan to 31 Jan | 6300 | Daily balance from 30 Jan to 31 Jan (ineligible days) | 4500 |
| Profit eligibility | Yes | Profit eligibility | Yes |
| Profit rate | 5% | Profit rate | 5% |
| Profit Amount 1 (8500 * 29 days * 5%/365) | 33.7671233 | Profit amount 1 (8500 * 29 days * 5%/365) | 33.7671233 |
| Profit amount 2 (6300 * 2 days * 5%/365) | 1.7260274 | Profit amount 2 (0 * 2 days * 5%/365) | 0 |
| Total profit | 35.4931507 | Total profit | 33.7671233 |


#### ⚙️ Configuration

The topic enables the user to understand the configuration for Islamic Accounts


##### Pool ID Default setup

The below mentioned product condition should be attached to AA.PRD.DES.ACTIVITY.API Property Class related property.

Refer to Retail Accounts user guide for detailed AA accounts configuration setup.


##### Payment of Profit Amount as Charges

This feature is for banks who do not prefer to capture the profit rate at the account level for notional profit accruals. Also, there is no need to report the daily notional profit accruals for the accounts. As and when the PDS distribution is performed the profit rate or profit amount calculated during the PDS simulation is paid to the account as charges. The impact on the expenses profit and loss category is adjusted only on the PDS distribution date.

Read Payment of Profit Amount as Charges topic to understand the functionality in detail.


#### 📋 Tasks

Related topics:

- Open Mudaraba Account
- Amend Mudaraba Account
- Set or Reset Dormancy (AA)
- Islamic Financing processes

The Islamic savings account is defined from a Sharia perspective as a Mudaraba contract between the two parties such as a capital provider or depositor and an entrepreneur or bank. It is created by using the Retail Accounts module.


##### Workflow

The user can perform the following activities:

| SCREENS | WORKFLOW |
|---|---|
|  | AA – Product Catalog . |
| Product Group | In the Islamic Accounts section, click the Products icon, corresponding to the Islamic Savings Account product group. |
| Products | In the Islamic Savings Account section, click the New Arrangement icon, corresponding to the Mudaraba Accounts product. |
| New Arrangement | Enter values in the following fields: Customer Currency Effective Date Click the Validate icon to check for errors and overrides. Click the Commit icon. Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
|  | AA – Product Catalog . |
| Product Group | In the Islamic Accounts section, click the Products icon, corresponding to the Islamic Savings Account product group. |
| Products | In the Islamic Savings Account section, click the New Arrangement icon, corresponding to the Mudaraba Daily Product Savings Accounts product. |
| New Arrangement | Enter values in the following fields: Customer Currency Effective Date Click the Validate icon to check for errors and overrides. Click the Commit icon. Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
|  | AA – Product Catalog . |
| Product Group | In the Islamic Accounts section, click the Products icon, corresponding to the Islamic Savings Account product group. |
| Products | In the Islamic Savings Account section, click the New Arrangement icon, corresponding to the Mudaraba Account – Monthly minimum product. |
| New Arrangement | Enter values in the following fields: Customer Currency Effective Date Click the Validate icon to check for errors and overrides. Click the Commit icon. Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
|  | AA – Product Catalog . |
| Product Group | In the Islamic Accounts section, click the Products icon, corresponding to the Islamic Savings Account product group. |
| Products | In the Islamic Savings Account section, click the New Arrangement icon, corresponding to the Mudaraba Account – Daily minimum product. |
| New Arrangement | Enter values in the following fields: Customer Currency Effective Date Click the Validate icon to check for errors and overrides. Click the Commit icon. Accept the overrides, if any. |


#### 📊 Outputs

There are no Outputs available for Islamic Accounts feature.

---


### 1.7  Islamic Deposit Products


> **📇 Quick Reference Card**
> 
> **Purpose:** *Islamic bank uses Islamic deposits to lend finance contracts and increase profit for the shareholders. The shareholders receives the profit amount when deposit or investment makes profit. Similarly, they may also lose a proportion of their capital in case deposit posts a loss. Islamic deposits are b...*
> 
> **Key Fields:** *Actual Amt*, *Amount*, *Apply PDS Profit Rate*, *Currency*, *Customer*, *Effective Date*, *Fixed Rate*, *Profit Capitalisation* ... +4 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Islamic bank uses Islamic deposits to lend finance contracts and increase profit for the shareholders. The shareholders receives the profit amount when deposit or investment makes profit. Similarly, they may also lose a proportion of their capital in case deposit posts a loss. Islamic deposits are based on Mudaraba and Wakala structures. The agreement between the depositor and the Islamic banks does not indicate a specific rate of return. It merely sets the ratio in which profits and losses may be distributed between the parties of the contract.

Different tenures may be chosen, as mutually agreed by both parties. Islamic deposits enable depositors to earn profits that are compliant with Shariah laws. The bank invests the client deposit in Shariah-compliant business and investment funds.

Refer to Fixed Deposit (AD) user guide for deposit arrangements functionality.


#### ⚙️ Configuration

This topic enables the user to understand the configuration for Islamic Deposit Products.


##### Setting up Default Pool ID

The below mentioned product condition should be attached to AA.PRD.DES.ACTIVITY.API Property Class related property.

Refer to, Fixed Deposits (AD) user guide for AA deposits configuration setup.


#### 📋 Tasks

Related topics:

- Open Mudaraba Deposit
- Open Wakala Deposit
- Perform Early Withdrawal of Mudaraba Deposit
- Perform Early Withdrawal of Wakala Deposit
- Islamic Financing processes

Islamic banks use Islamic deposits, which are based on Mudaraba and Wakala structures, to lend finance contracts which increases the profit for shareholders. The shareholders receive the profit amount when the deposit or investment makes profit. The agreement between the depositors and the Islamic banks does not indicate a specific rate of return. It only sets the ratio in which the profits and losses may be distributed between the parties of the contract. An additional gift, Special HIBA, in the form of currency may also be provided to the customers.


##### Workflow

The user can create a new arrangement for any of the deposit products listed under the Islamic Deposits product group.

The following products are grouped under the Islamic Deposit product group.

- 1 Month Mudaraba Deposit
- 3 Months Mudaraba Deposit
- 6 Months Mudaraba Deposit
- 12 Months Mudaraba Deposit
- 2 Years Mudaraba Deposit
- Long Term Mudaraba Deposit
- Mudaraba Savings Plan
- Advance Profit Fixed Mudaraba Deposit
- Wakala Deposits

| SCREENS | WORKFLOW |
|---|---|
|  | AA – Product Catalog . |
| Product Group | Click the Islamic Deposits section. Click the Products icon corresponding to the Islamic Deposits product group. |
| Products | In the Islamic Deposits section, click the New Arrangement icon corresponding to any one of the following deposit products: 1 Month Mudaraba Deposit 3 Months Mudaraba Deposit 6 Months Mudaraba Deposit 12 Months Mudaraba Deposit 2 years Mudaraba Deposit |
| New Arrangement | Enter values in the following fields : Customer Currency Effective Date Click the Validate icon to check for errors and overrides. In the Commitment section, enter a value in the Amount field. In the Special HIBA Profit section, enter a profit rate in the Fixed Rate field. Click the Settlement Instructions section. In the Basic tab, under Initial Funding, Charges Settlement, enter a value in the Settlement A/c field. In the Basic tab, under Interest & Redemption Settlement, enter a value in the Settlement A/c field. In the Deposit Condition section, select a value from the Profit Pay Method field drop-down. For Fixed Profit Mudaraba Deposit, set the Apply PDS Profit Rate field to 'Not Required'. Click the Validate icon to check for errors and overrides. Click the Commit icon. Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
|  | AA – Product Catalog . |
| Product Group | Click the Islamic Deposits section. Click the Products icon corresponding to the Islamic Deposits product group. |
| Products | In the Islamic Deposits section, click the New Arrangement icon corresponding to the Long Term Mudaraba Deposit product. |
| New Arrangement | Enter values in the following fields: Customer Currency Effective Date Click the Validate icon to check for errors and overrides. In the Commitment section, enter values in the following fields: Amount Term In the Special HIBA Profit section, enter a profit rate in the Fixed Rate field. Click the Settlement Instructions section. In the Basic tab, under Initial Funding, Charges Settlement, enter a value in the Settlement A/c field. In the Basic tab, under Interest & Redemption Settlement, enter a value in the Settlement A/c field. In the Deposit Condition section, select a value from the Profit Pay Method field drop-down. For Fixed Profit Mudaraba Deposit, set the Apply PDS Profit Rate field to 'Not Required'. Click the Validate icon to check for errors and overrides. Click the Commit icon. Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
|  | AA – Product Catalog . |
| Product Group | Click the Islamic Deposits section. Click the Products icon corresponding to the Islamic Deposits product group. |
| Products | In the Islamic Deposits section, click the New Arrangement icon corresponding to the Mudaraba Savings Plan product. |
| New Arrangement | Enter values in the following fields: Customer Currency Effective Date Click the Validate icon to check for errors and overrides. In the Commitment section, enter values in the following fields: Amount Term In the Schedule section, enter a value in the Actual Amt field corresponding to DEPOSIT.SAVINGS Payment Type. Click the Settlement Instructions section. In the Basic tab, under Initial Funding, Charges Settlement, enter a value in the Settlement A/c field. In the Basic tab, under Interest & Redemption Settlement, enter a value in the Settlement A/c field. In the Deposit Condition section, check the Profit Capitalisation field set to Yes. Click the Validate icon to check for errors and overrides. Click the Commit icon Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
|  | AA – Product Catalog . |
| Product Group | Click the Islamic Deposits section. Click the Products icon corresponding to the Islamic Deposits product group. |
| Products | In the Islamic Deposits section, click the New Arrangement icon corresponding to the Advance Profit Fixed Mudaraba Deposit product. |
| New Arrangement | Enter values in the following fields: Customer Currency Effective Date Click the Validate icon to check for errors and overrides. In the Commitment section, enter values in the following fields: Amount Term Click the Settlement Instructions section. In the Basic tab, under Initial Funding, Charges Settlement, enter a value in the Settlement A/c field. In the Basic tab, under Interest & Redemption Settlement, enter a value in the Settlement A/c field. In the Deposit Condition section, select Yes in the Recalc Profit field for profit recalculation at pre-closure. Click the Validate icon to check for errors and overrides. Click the Commit icon Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
|  | AA – Product Catalog . |
| Product Group | Click the Islamic Deposits section. Click the Products icon corresponding to the Islamic Deposits product group. |
| Products | In the Islamic Deposits section, click the New Arrangement icon corresponding to the Wakala Deposits product. |
| New Arrangement | Enter values in the following fields: Customer Currency Effective Date Click the Validate icon to check for errors and overrides. In the Commitment section, enter values in the following fields: Amount Term In the Special HIBA Profit section, enter a profit rate in the Fixed Rate field. Click the Settlement Instructions section. In the Basic tab, under Initial Funding, Charges Settlement, enter a value in the Settlement A/c field. In the Basic tab, under Interest & Redemption Settlement, enter a value in the Settlement A/c field. In the Deposit Condition section, select a value in the Profit Pay Method field drop-down. Click the Validate icon to check for errors and overrides. Click the Commit icon Accept the overrides, if any. |


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to Islamic Deposit Products.


##### Enquiries and Reports

This section allows the user to view the enquiry related to Mudaraba Deposit.

Mudaraba Deposits Booked Today

This enquiry displays the list of Mudaraba Deposits booked on any given system day.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


### 1.8  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *Profit Distribution System (PDS) provides the mechanism for Islamic banks to calculate and distribute profits for,*
> 
> **Applications:** `AA.ACCRUAL.FREQUENCY`, `AA.ARRANGEMENT`, `ACCOUNT`, `CATEGORY`, `CURRENCY`, `CURRENCY.MARKET`, `CUSTOMER`, `EB.API` ... +16 more
> 
> **Key Fields:** *Account Cat*, *Account Seq*, *Accrual Rate*, *Acct weightage*, *Activity*, *Addl Reserve Rtn*, *Addl reserve Rtn*, *Amount From* ... +92 more
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- Temenos Transact Services
- System Maintained Files

Profit Distribution System (PDS) provides the mechanism for Islamic banks to calculate and distribute profits for,

- Mudaraba deposits
- Wakala deposits
- Mudaraba savings accounts

The module manages various pools with finance or deposit products linked to those pools. Banks pool funds from customers and these funds are used to perform business activities such as investment, financing, purchase and lease using Islamic principles. Profit earned from business activities is distributed for deposit and account holders.


##### Defining Product Features

The following are the product features:

- Automatic allocation of pool ID based on the conditions parameterised. Islamic finance, deposit and account products assigned to a particular pool ID during booking.
- Multiple pools can be created with, Profit and expense categories setup for each pool Manual addition of additional income or expense Routine based modification of the calculated net profit amount Ability to setup profit calculation order (IRR, PER, Mudarib share and routine based calculation) for each pool. This can be set in any order at the pool level. Profit distribution frequency for each account or deposit type linked to the pool
- Setting up of tier balance-based profit calculation for accounts by using Band or Level profit rates.
- Setting up of special weightages for priority customer at customer or account level
- Amendment of pool ID assigned to the deposit or account from the last PDS end date +1
- Profit Equalization Reserve (PER) can be defined for each pool ID and can be utilised in the subsequent months, when needed
- Defines Investment Risk Reserve (IRR) for each pool ID and can be utilised in subsequent months, when needed
- Pay Hiba using special spread as additional profit
- Ability to accrue profit for Mudaraba deposits or Mudaraba accounts by using the provisional rate. Posting of accrual adjustment accounting entries on the date of PDS distribution based on the actual profit rate. The banks can set an option to use the last distributed profit rate as provisional accrual rate for the next period.
- Ability to capitalise the profit amount for Mudaraba deposits based upon the profit payment method.
- Ability to add shareholder contribution to the pool calculation by using manual or automatic method
- Ability to reverse the Last PDS distribution run.
- Provisions to run simulation before profit distribution
- Ability to pay the profit amount calculated during PDS simulation for Mudaraba savings accounts without posting profit accruals (using the charges feature).
- Customised enquiries to see the results

The following are the list of major functionalities supported:

- Linking pool ID with deposits or accounts
- Islamic deposit arrangements – Creation and maintenance
- Islamic accounts – Creation and maintenance
- Profit distribution system management Simulation Target rate update Input spread and special spread Input target rate Simulation – Projection

- Distribution
- Reverse – Distribution


##### Configuration

This section explains the various parameters and system core table setup that need to be set for operation of the profit distribution.


###### ID.SYSTEM.PARAMETER

This table specifies the system level attributes for setting up profit distribution process. The key parameters are listed below:

- Allowed ID is SYSTEM
- Defines profit distribution frequency for paying profit amount to Mudaraba deposits or accounts. It can be setup at pool or system level. During profit distribution, calculated profit amount is paid to the customer based on Distrib Freq field from ID.POOL.PARAMETER table. In case, Distrib Freq field is not set in ID.POOL.PARAMETER table, then the system uses the distribution frequency set in Distrib Freq field from ID.SYSTEM.PARAMETER table.
- Defines transaction types to raise accounting entries
- Defines the number of days after which the pool tracker file records are moved to history files
- Defines the user activities that can be run during distribution process for arrangements
- Defines the posting restriction code used for Islamic accounts marked to close on PDS run
- Setup the Migration Mode field to update the history of PDS calculations from the legacy system during data migration. Once the data migration is completed it needs to be switched off as it enables the bank to update the PDS profit rate for the past period, which is used during profit amount recalculation for Mudaraba deposits.
- Setup the Direct Pay Profit field as Yes to pay the profit amount as charges without posting any profit accruals. If this field is set as yes, then: It is not possible modify the field value. It is not possible to reverse the last PDS distribution. Special HIBA profit rate is not considered during the profit payment.

After the system level configuration, the banks set-ups the model parameters as explained below:


##### Model Parameters

The parameter files and system tables are setup to support the Islamic profit distribution operations. This section provides a brief overview of the system and parameter setup for holding the static data.

This table is used to configure the conditions for setting default values for the pool ID in the relevant applications. When an asset or liability transaction is created, the pool ID should be captured. The user can enter the pool ID manually or enable the system to populate automatically by setting up the conditions in this table. The key parameters details are listed below:

- Allowed IDs are valid application names, for example, AA.ARRANGEMENT , ACCOUNT , SEC.TRADE , LD.LOANS.AND.DEPOSITS , MM.MONEY.MARKET and LETTER.OF.CREDIT .
- Defines the conditions to identify the pool ID based on the Appl Field Name , Field Operator , Value From and Value To fields.
- Defaults the pool, when the other defined conditions fails to identify the pool.

| Field | Description |
|---|---|
| Income Cat | This field is used to define the income accrual PL category. It is a multi-value field used along with Income Product Cat for mapping the product income. PL categories set in the Accounting product condition of the respective product, needs to be mapped in this field. Allowed values are from the CATEGORY table . |
| Income Product Cat | This field is used to set the income product category. The finance product categories required for the pool calculation are set in this field . Allowed values are from the CATEGORY table. |
| Income Product | This field is reserved for future use. |
| Oth Income Cat | This field is used to set the income PL category for capturing the non–product related income. It is a multi-value field used along with Oth Income Pct for calculating the pool income. Allowed values are from the CATEGORY table. |
| Oth Acct Pct | This field is used to capture the percentage of other income to be consider in the pool calculation. Allowed values are from 0 -100. |
| Oth Income Acct | This field is used to set the income from the internal accounts. It is a multi-value field used along with Oth Inc Acct Pct for calculating the pool income. Allowed values are from the ACCOUNT table. |
| Oth Inc Acct Pct | This field is used to capture the percentage of other income from accounts to be used during the pool calculation. Allowed values are from 0 – 100. |

PDS calculation uses weighted (average or minimum or daily) balance of Mudaraba deposits or Mudaraba accounts or Wakala deposits. The pool condition for setting up the weightage can be set by using the combination of Pool ID, Category (differentiates the tenor), Currency, Profit distribution frequency and Broken Deposits condition (BRK). The weightage for each pool condition along with the IRR percentage, PER percentage, Mudarib share, accrual profit rate are set in this table for each balance amount bracket.

- Id - The ID comprises of . . . . . The ID accepts a value of ‘ALL’ for Pool ID and Category. 1.3251.USD – Implies, ‘Category 3251’, linked to ‘Pool 1’, and ‘Currency is USD’. ALL.ALL.GBP – Implies, ‘Category ALL’, linked to ‘Pool ALL’, and ‘Currency is GBP’. 1.3051.AED.M01 – Implies, ‘Category 3051’, linked to ‘Pool 1’, ‘Currency is AED’, and ‘Profit distribution frequency is M01’. 1. ALL.SAR – Implies, ‘Category ALL’, linked to ‘Pool 1’ and ‘Currency is SAR’. 1.3001.USD.ALL.BRK – Implies, ‘Category 3001’, linked to ‘Pool 1’, ‘Currency is USD’, Broken deposit condition.
- Description - This field is used to provide a description. It is a multi-lingual field that allows to set description in multiple languages.
- Amount From - This field is used to capture the starting range for the balance bracket amount. Numeric values allowed are up to 19 digits.
- Amount To - This field is used to capture the ending range for the balance bracket amount. Both values in the Amount from and Amount to fields are inclusive in the range. Numeric values allowed are up to 19 digits.
- Weightage - This field is used to capture the weightage in terms of percentage to apply on the amount. Allowed values are from 0 - 999999% up to six decimals. The weightage set in this field is used to calculate weighted balance for deposit balance ranges in the balance bracket.
- Mud Share - This field is used to capture the Mudarib share percentage. Allowed values are from 0% - 100% up to six decimals. The weightage set in this field is used to calculate the Mudarib fee.
- Irr Percent - This field is used to capture the Investment Risk Reserve percentage. Allowed values are from 0% - 100% up to six decimals. The weightage set in this field is used to calculate the IRR amount.
- Per Percent - This field is used to capture the Profit Equalization Reserve Percentage. Allowed values are from 0% - 100% up to six decimals. Weightage setup in this field used to calculate the PER amount.
- Accrual Rate - This field is used to default the profit rate used for daily accruals to Mudaraba deposits. During Mudaraba deposit booking, the profit rate set for the pool condition is evaluated and set as default in the deposit arrangement by considering the values input in the arrangement input page. If the set pool condition ends with ‘BRK’ keyword, then the profit rate is used during profit amount recalculation for pre-closed deposits.
- Update Rate - This field is used to indicate whether the profit rate calculated during PDS run needs to update automatically to the pool condition. Allowed values are : Yes - Then update takes place automatically to the Accrual Rate field with the profit rate calculated in PDS run. No - Then a manual update is required for the Accrual Rate field as and when required.
- Apply as Tier Rate - While creating the Mudaraba savings account, it is possible to define the profit rate as a tier rate with band or level conditions. This field can be set as Yes to default the accrual rate configured for different balance brackets. It cannot be set as Yes for ALL.ALL condition. It is not allowed to modify this field definition after authorisation.
- Band or Level – This field is used to indicate whether the tier definition of profit rates is applied by using band or level calculation method. It is not allowed to modify this field definition after authorisation.

PDS calculation uses different calculation methods like daily, average and minimum. It is possible to define this, by using a combination of Pool ID, Category and ALL. Currency wise minimum balance for excluding accounts or minimum deposit period for excluding the Mudaraba deposits from participating in pool calculation is set in this table.

- Id - ID comprises of or . It is possible to provide ‘ALL’ for Pool ID and Category (ALL.ALL). The configuration is used to set and refer the exclusion conditions in ID.ACCOUNT.CONDITION during PDS simulation.

- 1.3601 – Denotes the conditions set for ‘Pool 1’ and ‘Category 3601’
- 3605 – Denotes the conditions set for ‘Category 3605’. Conditions are applicable for all pools.
- ALL.ALL – Denotes the conditions set for ‘Pool ALL’ and ‘Category ALL’. Conditions are applicable for ALL pools and ALL categories.
- U-3601 – Denotes the conditions set for ‘Category 3601’. The minimum balance exclusion criteria can be defined in ID.ACCOUNT.CONDITION . While running PDS simulation the exclusion conditions configured in ID.ACCOUNT.CONDITION should be evaluated for the accounts opened with the category 3601. The minimum balance amount set in ID.PDS.CATEGORY becomes void for this setup.

- Description - This field is used to provide a description. It is a multi-lingual field that allows to set description in multiple languages.
- Calc Balance Type – This field is used to set the different balances that the PDS calculation or distribution for deposits or accounts use. Allowed values are ‘Daily’, ‘Average’, and ‘Minimum’. Based upon the balance type set in this field the participation balance for deposits or accounts is calculated.
- Dist Balance Type - This field is for future use.
- Currency & Min Balance - ‘Currency’ and ‘Min Balance’ are multi-value fields used to set the currency wise minimum balance required for Mudaraba savings accounts participating in the pool calculation. If the condition is not satisfied, then the balance of the respective Mudaraba account is excluded in pool calculation and the profit amount is not paid. Allowed values for Currency field is a valid record from CURRENCY table. Allowed values for Min Balance field is numeric.
- Min Dep Period – This field is used to set the minimum deposit period for Mudaraba deposits participating in Pool calculation. If the condition is not satisfied, then the balance of the respective Mudaraba deposit is excluded in pool calculation and the profit amount is not paid. Allowed values are from 0D – 999D.

It is necessary to provide special weightages for the specific customers that provide more business value to the bank. This table used to set the weightage at the customer or account level.

During simulation calculation, the weightage for each pool condition is fetched from the weightage set in ID.PDS.WEIGHT . The special weightage set at the customer or account level is used if available for PDS calculation.

- Id - Allowed values are from the CUSTOMER application.
- Weightage - This field is used to capture the weightage in terms of percentage to apply on the amount. Allowed values are from 0% - 999999%. Weightage set in this field is used to calculate the weighted balance for deposit balance ranges in the balance bracket.
- Customer Acct - This field is used to capture the account number of the customer. Allowed values are from the ACCOUNT application. It is a multi-value field used to setup different weightages for each account.
- Acct weightage - This field is used to capture the weightage in terms of percentage to apply on the amount. Allowed values are from 0 - 999999%. The weightage set in this field is used to calculate the weighted balance for deposit balance ranges in the balance bracket.

This parameter table is used to configure the accrual frequency. It is required to configure accrual frequency as Monthly for the product configured with transaction exclusion and balance exclusion criteria.

This table is used to configure the evaluation criteria required to calculate the transaction count and balance exclusions. It can be configured for each product along with the profit property name used for evaluation (Product Name – Property Name). The following are the related fields.

- Exclusion Evaluation Cycle – This field indicates the evaluation period of the configured conditions. The default value is Monthly, which implies that the exclusion criteria must be evaluated on a monthly basis.
- Conditions Evaluation Period – This field indicates the evaluation period of minimum balance criteria. The supported values are Monthly and Daily.
- PDS Category I D – This field indicates the unique identification of the record in the ID.PDS.CATEGORY table. The user can configure the balance amount used for PDS calculation in the existing parameter in the ID.PDS.CATEGORY table. This field is used to provide a link to the ID.PDS.CATEGORY table and validate that the calculation balance type is Minimum. It is required to create a separate record in the ID.PDS.CATEGORY table for the configured account product category by using the ID as U- .
- Min Balance Amount – This field indicates the currency-wise minimum balance amount used for evaluating the minimum balance amount exclusion.
- Min Balance Evaluation Start Date – This field indicates whether the system should begin the minimum balance evaluation from the account opened date or the account funded value date.
- Initiation Type – This field indicates the transaction initiation type for transaction exclusion evaluation. To configure the transaction exclusion criteria, set the transaction initiation type as Customer for the account debit activities.
- Exclude/Include Activity - This field indicates including or excluding the required activities for the transaction exclusion evaluation.
- Exclude/Include Indicator – This field indicates including or excluding the required activities from the transaction exclusion evaluation. It is defaulted from the Exclude/Include Activity field and does not allow the user to enter any value.
- Tran Threshold Count – This field indicates the allowed transaction count eligible for-profit payment. The user needs to create separate transaction codes for the transactions posted through various channels (branch, internet banking, mobile banking, and other channels).
- Activity mapping.

This parameter table is used to set the tenor-wise recalculation categories used for automatic profit amount recalculation during the pre-closure of the Mudaraba deposit.

- ID – This field allows a valid deposit product created using arrangement architecture.
- Rest period – This field is used to capture the tenor of the deposit in months or days. R can be used to capture the remaining term.
- Recalc category - This field is used to capture the category code used during profit recalculation.
- Recalc profit adjustment percentage – This field is used to capture the recalculated profit adjustment amount percentage. The profit amount is recalculated by using the completed tenor multiplied by the ‘recalculate profit adjustment percentage’ to arrive at the profit amount paid to the customer account.


##### Model Products

| Product Group | Product Name | Features |
|---|---|---|
|  | Pool Linking | Linking finance or deposit or account to pool with manual or automatic process |
| Islamic Deposits | 1 Month Mudaraba Deposit 12 Month Mudaraba Deposit 2 Year Mudaraba Deposit 3 Month Mudaraba Deposit 6 Month Mudaraba Deposit Long Term Mudaraba Deposit | Creates Mudaraba deposit for different currency or tenor using AA - Deposits product line. Books deposits for different tenor with or without rollover. The user defined property class and product condition features are used to capture the pool ID, deposit conditions, and early maturity recalculation options. Mudaraba deposit can be booked with the notional profit rate setup in ID.PDS.WEIGHT . |
| Advanced profit fixed Mudaraba Deposit | Mudaraba deposit can be booked with the notional profit rate setup in ID.PDS.WEIGHT . Profit amount is paid to the deposit customer on the deposit booking date. |  |
| Mudaraba Savings Plan | This is a recurring deposit product based upon Mudaraba. It can be opened for various tenor, currency and funding can be made based upon different frequency. It is possible to capitalise the profit amount calculated during PDS calculation. |  |
| Wakala Deposit | Wakala deposit for different currency or tenor is created by using AA – Deposits product line. Books deposits for different tenor with or without rollover. The user defined property class and product condition features are used to capture the pool ID. Wakala deposit can be booked with the notional profit rate setup in ID.PDS.WEIGHT . |  |
| Islamic Savings Accounts | Mudaraba Accounts Mudaraba Daily Product Savings Accounts | Mudaraba accounts for different currency can be opened by using AA – Accounts product line. Profit rate used for daily accruals defaulted from the notional profit rate setup in ID.PDS.WEIGHT . It is possible to setup the Tier balance-based calculation with Band or Level profit rate setup. The user defined property class and product condition features are used to capture the pool ID. |
|  | PDS Process – Simulation | The net profit amount is calculated from the income or expenses of the pool during the specified period. When net profit amount is derived, it is split based on the weighted average balance, (which takes into account the contributions to the pool, from each Mudaraba Deposit, Mudaraba Account, Wakala Deposit and share holder contribution). The weighted average calculation is based on the weightage setup during the parameter configuration. Applies IRR%, PER%, Mudarib share% calculation to reduce the net profit for each deposit before arriving at the distributable profit amount. Distributable profit rate is calculated from the profit amount. |
|  | PDS Process – Distribution | Applies identified profit rate to the underlying Mudaraba deposits or Mudaraba accounts. Based on the profit pay method available in Mudaraba deposits, profit amount is paid to the customer account on distribution date or at later date. For Mudaraba accounts profit amount is paid by using profit distribution frequency. For Wakala deposits profit adjustment accounting entries are generated. |
|  | Reverse – PDS Process – Distribution | After distributing the profit amount to the Mudaraba deposits or Mudaraba account or Wakala deposits, it is possible to reverse the PDS distribution. During the reversal, the accounting entries raised during old PDS distribution are reversed. New PDS distribution accounting entries are generated based upon the calculated adjustment amount. New PDS profit rate is distributed to the Deposits or Accounts, which posts the adjustment accounting entries for the profit amount calculated during old PDS distribution. |


> **Related Applications:** `AA.ACCRUAL.FREQUENCY`, `AA.ARRANGEMENT`, `ACCOUNT`, `CATEGORY`, `CURRENCY`, `CURRENCY.MARKET`, `CUSTOMER`, `EB.API`, `ID.ACCOUNT.CONDITION`, `ID.CUSTOMER.PREFERENCES`, `ID.DEPOSIT.BALANCES`, `ID.PDS.ACTION`, `ID.PDS.CATEGORY`, `ID.PDS.WEIGHT`, `ID.POOL.CONDITION`, `ID.POOL.PARAMETER`, `ID.PRECLOSE.CUSTOMISE`, `ID.SYSTEM.PARAMETER`, `INTEREST.BASIS`, `IS.PDS.WEIGHT`, `LD.LOANS.AND.DEPOSITS`, `LETTER.OF.CREDIT`, `MM.MONEY.MARKET`, `SEC.TRADE`

---


### 1.9  Payment of Profit Amount using Charges


> **📇 Quick Reference Card**
> 
> **Purpose:** *While creating a Mudaraba savings account, the notional profit rate is captured or populated from the parameter tables. The profit accruals are posted using the notional profit rate during the month and it is used for end of the day reporting as well. Subsequently, after running the PDS calculation ...*
> 
> **Applications:** `ID.PDS.WEIGHT`, `ID.POOL.PARAMETER`, `ID.SYSTEM.PARAMETER`
> 
> **Key Fields:** *Direct Pay Profit*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

While creating a Mudaraba savings account, the notional profit rate is captured or populated from the parameter tables. The profit accruals are posted using the notional profit rate during the month and it is used for end of the day reporting as well. Subsequently, after running the PDS calculation for the current period, the PDS profit rate is calculated and applied to the underlying Mudaraba savings accounts linked to the pool during PDS distribution.

If the bank does not prefer to capture or perform daily profit accruals using the notional profit rate. As and when PDS simulation is performed the profit amount or profit rate is calculated for the period. During PDS distribution it is required to pay the profit amount calculated during PDS simulation to each Mudaraba savings account. Special HIBA profit is not handled as part of this solution.

During account closure, it is not required to pay the accrued profit amount to the customer account. It is required to consider these accounts during current PDS calculation to calculate and credit the eligible profit amount into the suspense account. Subsequently, the user takes further action on the credited profit amount.


#### ⚙️ Configuration

To implement the profit payment for accounts through charges, configure the following as mentioned:

The Direct Pay Profit field value must be set as Yes. Once this field is set as ‘Yes’, it is not allowed to modify the field value again and to reverse the Last PDS distribution.

The Direct Pay Profit field value must be set as Yes. Once this field is set as ‘Yes’, it is not allowed to modify the field value again.

> **⚠️ Note:** This field is available only for Internal purpose and it is not possible set this field value in the implementing client sites.

The accrual profit rate configured in ID.PDS.WEIGHT needs to be updated as ZERO and update rate as ‘No’ for all the configured pool conditions.

New charge property PDSPROFIT must be configured in the Mudaraba savings account product as a credit charge. This charge property is used to pay the profit amount during PDS distribution.

Relevant charge product condition must be configured as below:

> **⚠️ Note:** The charges must be capitalised to the customer accounts.

The charge property must be added to the Activity charges and the method must be set as Capitalize.

The closure period configured in the Closure product condition needs to be greater than 30D. This is to ensure that the Account record is in LIVE and not archived even after the account closure date.

The property and product condition must be added to the product designer of the Account product before proofing and publishing the product.


#### 🔧 Working With

This section describes how the payment of profit amount to accounts using charges, works in the following scenarios.


##### Creating an Account

A Mudaraba savings account can be created from the products available in the product catalogue. While creating the account, it is required to capture the customer id, currency, and effective date. During validation the details of the customer is defaulted into the relevant arrangement conditions. The profit rate for the account arrangement is defaulted as 0% and the profit accruals are not posted to the account. After authorisation, the account arrangement is created successfully.


##### Closing an Account

It is expected to capture the profit rate at the account level as 0% as no profit accruals are posted to the account arrangement. During the account closure, the system pays only the principal amount to the customer account and the account is marked as closed.

U-IDSUSPENSE) with the account number and customer name as additional narration. The user needs to take further action on the credited balances into the account.


##### Triggering PDS distribution

While triggering the PDS distribution, the configuration in the system or pool parameter is validated for the option set in ‘Direct payment of profit’.

- If it is set as NULL in both the configuration tables, then the profit amount is paid using the existing profit payment logic by triggering both Rate change and Schedule change activities.
- If it set as Yes in either the system parameter or the pool parameter, then the profit amount is paid directly to the customer account through charges posting.


##### Accounting

| Daily Accrual – Principal Profit |
|---|
| NA |

| PDS Distribution |  |  |  |  |  |
|---|---|---|---|---|---|
| Reverse/ Replay in AA | DR/CR | Accounting Head/ Asset Type | Amount | Entry Type STMT/CATEG/SPEC | Transaction Type |
| NA | DR | PL Account (Profit Expenses) | Profit amount calculated based upon the PDS Rate | CATEG |  |
| NA | CR | Customer Account | Profit amount calculated based upon the PDS Rate | STMT |  |

| Profit Payment on the Frequency date |
|---|
| NA |

| Reverse - Profit distribution |
|---|
| Not allowed |


#### 📋 Tasks

There are no Tasks available for Payment of Profit Amount to Accounts using Charges feature.


#### 📊 Outputs

There are no Outputs available for Payment of Profit Amount to Accounts using Charges feature.


> **Related Applications:** `ID.PDS.WEIGHT`, `ID.POOL.PARAMETER`, `ID.SYSTEM.PARAMETER`

---


### 1.10  PDS Distribution


> **📇 Quick Reference Card**
> 
> **Purpose:** *When the profit rate is finalised with simulation or target rate process, the identified profit rate is applied to the underlying Mudaraba deposits or Mudaraba accounts. The relevant accounting entries are raised and this activity is run only once for a selected simulation period for a particular po...*
> 
> **Applications:** `AA.ACTIVITY`, `EB.LOOKUP`, `ID.PDS.ACTION`, `ID.POOL.PARAMETER`, `ID.SYSTEM.PARAMETER`
> 
> **Key Fields:** *Action*, *Type*, *User Activity*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

When the profit rate is finalised with simulation or target rate process, the identified profit rate is applied to the underlying Mudaraba deposits or Mudaraba accounts. The relevant accounting entries are raised and this activity is run only once for a selected simulation period for a particular pool (during distribution process).


##### Profit Payment during Distribution

The following are the different types of accounts and deposits:

| Accounts/ Deposits | Profit Payment |
|---|---|
| Mudaraba deposits | Based on profit pay method, profit amount is paid to customer on distribution run date or rollover date or maturity date or distribution frequency. |
| Wakala deposits | Adjustment accounting entries are raised (if chosen). Otherwise, Daily or Minimum or Average balance of Wakala deposit is added to shareholder equity amount. |
| Mudaraba accounts | Profit amount is paid based on the profit distribution frequency setup in ID.POOL.PARAMETER table. |

> **⚠️ Note:** The Action field is set to Distribution in ID.PDS.ACTION table to execute PDS distribution.

This option is used to reverse the last PDS distribution executed for a pool. To perform reversal of PDS distribution,

1. Reversal request for PDS distribution – While initiating the request for reversal of PDS distribution, the old PDS distribution reference number is captured.
2. Creation of simulation for the reversed PDS distribution period – New PDS simulation can be initiated for the reversal request initiated PDS period. It is possible to trigger PDS simulation for subsequent period only after completing the PDS distribution for the reversal requested period.
3. PDS Target rate update – This option is used to modify the profit rate calculated during PDS simulation
4. PDS distribution: Reverse old PDS distribution – While processing the PDS distribution, if old PDS distribution reference number is captured in ID.PDS.ACTION , then old PDS distribution accounting entries are reversed. Process PDS distribution


#### ⚙️ Configuration

The below topic allows the user to understand the configuration for PDS distribution


##### Configuration for ID.SYSTEM.PARAMETER

During PDS distribution, the profit amount accrued by using notional and PDS rate need to reversed and posted respectively.

The setting up of activities for reverse and replay is handled in ID.SYSTEM.PARAMETER table. The below field are setup:

| Field Name | Description |
|---|---|
| Action | This field is used to setup the list of actions and activities linked to the action. It is a mandatory field. Valid values are: Accounts Change Schedule Accounts rate Change Deposits Change Schedule Deposits rate Change Accounts Apply Changes To Close at PDS The above listed valid values are setup in EB.LOOKUP table with record ID as ID.DIST ACTION |
| User Activity | This field is used to setup the AA.ACTIVITY ID linked to Action field. |

> **⚠️ Note:** The Type field is set as Restore in AA.ACTIVITY for the above defined user activities as shown below:


#### 📋 Tasks

Related topics:

- Perform Profit Distribution
- View Profit Distribution Projection - Simulation
- Islamic Financing processes

When the profit rate is finalised with simulation or target rate process, the identified profit rate is applied to the underlying Mudaraba deposits or Mudaraba accounts.


##### Workflow

The user can perform the following activities:

This enquiry displays the list of PDS action IDs to perform distribution. The user can view or authorise the records.

To view the PDS action ID, follow the below steps:

1. Input Distribution .
2. In the Distribution screen, click the View icon corresponding to a record to view the details of PDS action ID.

To authorise the PDS action ID, follow the below steps:

1. Input Distribution .
2. In the Distribution screen, click the Authorise icon corresponding to a record.
3. In the PDS-Distribution screen, verify the details and then click the Authorise icon.

This enquiry displays the list of PDS action IDs pending for authorisation. The user can authorise or delete or view the unauthorised records.

To view the PDS action ID, follow the below steps:

1. Authorise/ Delete/ View Distribution .
2. In the Unauthorised Distribution screen, click the View icon corresponding to a record.

To authorise the PDS action ID, follow the below steps:

1. Authorise/ Delete/ View Distribution .
2. In the Unauthorised Distribution screen, click the Authorise icon corresponding to a record.
3. In the PDS Distribution Action view screen, verify the details and then click the Authorise icon.

To delete the PDS action ID, follow the below steps:

1. Authorise/ Delete/ View Distribution .
2. In the Unauthorised Distribution screen, click the Delete icon corresponding to a record.
3. In the PDS Distribution Action View screen, click the Delete icon.

This enquiry displays the list of PDS action IDs to perform reversal of distribution. The user can view or authorise the record.

To view the PDS action ID, follow the below steps:

1. Input – Reverse Distribution .
2. In the Reverse Distribution screen, click the View icon corresponding to a record to view the details of PDS action ID.

To authorise the PDS action ID, follow the below steps:

1. Input – Reverse Distribution .
2. In the Reverse Distribution screen, click the Authorise icon corresponding to a record.
3. In the PDS-Reverse Distribution screen, verify the details and then click the Authorise icon.

This enquiry displays the list of PDS action IDs pending for authorisation. The user can authorise, delete or view the unauthorised records.

To view the PDS action ID, follow the below steps:

1. Authorise /Delete /View Reverse Distribution .
2. In the Unauthorised Reverse Distribution screen, click the View icon corresponding to a record.

To authorise the PDS action ID, follow the below steps:

1. Authorise /Delete /View Reverse Distribution .
2. In the Unauthorised Reverse Distribution screen, click the Authorise icon corresponding to a record.
3. In the Reverse PDS Distribution screen, verify the details and then click the Authorise icon.

To delete the PDS action ID, follow the below steps:

1. Authorise /Delete /View Reverse Distribution .
2. In the Unauthorised Reverse Distribution screen, click the Delete icon corresponding to a record.
3. In the Reverse PDS Distribution screen, click the Delete icon.


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to PDS - Distribution.


##### Enquiries and Reports

The section allows the user to view the simulation calculation details.

Early Matured Deposits added to SH Funds

This enquiry displays the list of Mudaraba Deposits that are pre-closed during the simulation period and the balances added to the shareholder funds.

Adjustment Entries raised for LIVE Deposits

This enquiry displays the accounting entries raised for LIVE Mudaraba Deposits.

Adj entries raised for Normal Matured Deposit

This enquiry displays the accounting entries raised for normal matured Mudaraba Deposits during the simulation period.

PDS Distribution - AA Activity OFS status

This enquiry displays the list of arrangement activities executed for Deposit or Account arrangement during PDS distribution along with the OFS status and OFS failure messages. Also, it displays OFS status for the accounts that are Closed on PDS run.

PDS Enquiries-Combined

This enquiry displays the combined view of PDS Simulation Summary, Pool Income Expenses Details and Band-wise Balance Summary.

Special HIBA Payment Summary

This enquiry displays the Special HIBA Amount for all arrangements that are part of the PDS. It also displays the other details such as, Average Balance, HIBA Effective Date From and Date To.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA


> **Related Applications:** `AA.ACTIVITY`, `EB.LOOKUP`, `ID.PDS.ACTION`, `ID.POOL.PARAMETER`, `ID.SYSTEM.PARAMETER`

---


### 1.11  PDS Simulation


> **📇 Quick Reference Card**
> 
> **Purpose:** *PDS has set of steps to calculate the profit rate used for distributing profit amount to Mudaraba deposits, Mudaraba savings accounts or Wakala deposits. Simulation process allows calculation of profit amount based on income and expenses from the finance contracts or arrangements participating in th...*
> 
> **Applications:** `CATEG.ENTRY`, `ID.CATEG.ENT.DETAILS`, `ID.CATEG.ENT.UPDATE`, `ID.PDS.WEIGHT`, `ID.POOL.PARAMETER`
> 
> **Key Fields:** *Action*, *Action Reference*, *End Date*, *Last Update Date*, *Pds Action Id*, *Pool Ref*, *Spcl Spread Rate*, *Spread Rate* ... +2 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

PDS has set of steps to calculate the profit rate used for distributing profit amount to Mudaraba deposits, Mudaraba savings accounts or Wakala deposits. Simulation process allows calculation of profit amount based on income and expenses from the finance contracts or arrangements participating in the pool and distributes profit amount to deposits and account holders.

It has the ability to simulate the PDS calculation by setting up a different parameter. Once satisfied, the simulated record are used to distribute profit amount to the deposit or account holders.

The following Action can be performed in simulation module:

| Process | Description |
|---|---|
| Simulation | The net profit amount is calculated from the income or expenses of the pool during the specified period. When the net profit amount is derived, it is split based on the weighted average method, which takes into account the contributions to the pool from each (Mudaraba deposit, Mudaraba account, Wakala deposit and shareholder equity). The weighted average balance calculation is based on the percentages and weights setup during the parameter configuration. The IRR%, PER%, Mudarib share% setup in ID.PDS.WEIGHT is used to reduce the split net profit for each deposit before arriving at the distributable profit amount. The profit amount is converted into profit rate. |
| Targetupdate | The user can amend the profit rate calculated to match the market expectations. Such amendment results in recalculation of the distributable profit amount. |
| Distribution | When the profit rate is finalised, it is applied to the underlying Mudaraba deposits or Mudaraba accounts. Based on the profit pay method available in Mudaraba deposits, profit is paid to the customer account on (distribution or at later date). For Mudaraba accounts, profit is paid by using profit distribution frequency setup in the ID.POOL.PARAMETER . For Wakala deposits, based on the parameter setup, profit adjustment accounting entries are generated. Otherwise, it is added to the shareholder equity. |
| Projection | This option is used to run the simulation from the simulation start date till the simulation end date. Simulation end date can be a future date. The net profit amount is calculated from the income or expenses of the pool during the specified period from simulation start date till the last working day. Net profit amount is projected from Last working day + 1 till the simulation end date by using the pro-rata calculation. When the projected net profit amount is derived, it is split based on the weighted average method, which considers the contributions to the pool from each (Mudaraba deposit, Mudaraba account, Wakala deposit and shareholder equity). The weighted average balance calculation is based on the percentages and weights setup during the parameter configuration. The IRR%, PER%, Mudarib share% setup in ID.PDS.WEIGHT is used to reduce the split net profit for each deposit before arriving at the distributable profit amount. The profit amount is converted into profit rate. It is not possible to distribute the projected simulation calculation. |
| Reverse Distribution | This option is used to reverse the last PDS distribution performed by user for a Pool on any day before running the subsequent PDS distribution. The PDS distribution accounting entries raised during old PDS distribution is reversed. But, the arrangement activities triggered as part of old PDS distribution to Mudaraba deposits or Mudaraba savings accounts is not reversed. Since, AA – Deposits module has the capability to reverse and replay the activities happened in the past, it uses the functionalities: Reversal request for old PDS distribution [Last] can be initiated. New simulation request for the old PDS distribution period is triggered. Target rate update is used to modify the profit rate calculated during simulation. During PDS distribution, the accounting entries generated for the old PDS distribution is reversed. New PDS distribution accounting entries are generated. |


#### ⚙️ Configuration

The profit accrued from finance contracts or arrangements are stored in CATEG.ENTRY , on a daily basis,

XXX/ID.CATEG.ENTRY.EXTRACT service processes accrual records from CATEG.ENTRY table and updates the ID.CATEG.ENT.DETAILS table in a format, which accelerates the ID.PROFIT.CALCULATION service.

- The XXX/ ID.CATEG.ENTRY.EXTRACT service should be available in the PDS area. This service is run online or attached to Close of Business (COB) process
- The Simulation start date and end date should be within the range as mentioned in the Start Date and Last Update Date fields in ID.CATEG.ENT.UPDATE .


#### 📋 Tasks

Related topics:

- Perform Profit Distribution
- View Profit Distribution Projection - Simulation
- Islamic Financing processes

Profit Distribution System (PDS) has set of steps to calculate the profit rate used for distribution to Mudaraba deposits or Mudaraba` savings accounts and Wakala deposits. Simulation process allows calculation of profit amount based on income and expenses from the finance contracts or arrangements participating in the pool and distributes the profit amount to deposits and account holders. It has the ability to simulate the PDS calculation by setting up a different parameter. Once satisfied, the simulated records distribute the profit amount to the deposit or account holders.


##### Workflow

The user can perform the following activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Input Simulation . |
| Contract Screen | Click the New icon. |
| PDS Simulation | Enter values in the following mandatory fields: Pool Ref Start Date End Date Click the Validate icon to check for errors and overrides. Click the Commit icon. |

This enquiry displays the list of PDS action IDs that are pending for authorisation. The user can authorise or delete or view the unauthorised records.

To view the PDS action ID, follow the below steps:

1. Authorise/ Delete/ View Simulation .
2. In the Unauthorised Simulation screen, click the View icon of a corresponding record to view the details of PDS action ID.

To authorise the PDS action ID, follow the below steps:

1. Authorise/ Delete/ View Simulation .
2. In the Unauthorised Simulation screen, click the Authorise icon corresponding to a record.
3. In the PDS Action view screen, verify the details and then click the Authorise icon.
4. Run the following simulation services: BNK/ID.PROFIT.CALCULATION BNK/ID.POOL.BALANCES BNK/ID.SIMULATION.CALC

To delete the PDS action ID, follow the below steps:

1. Authorise/ Delete/ View Simulation .
2. In the Unauthorised Simulation screen, click the Delete icon corresponding to a record.
3. In the PDS Action View screen, click the Delete icon.

This enquiry displays the list of PDS action IDs to perform target updation. The user can view or authorise the records.

To view the PDS action ID, follow the below steps:

1. Input – Target Update .
2. In the Target Update screen, click the View icon of corresponding record to view the details of PDS action ID.

To authorise the PDS action ID, follow the below steps:

1. Input – Target Update.
2. In the Target Update screen, click the Authorise icon corresponding to a record.
3. In the PDS-Target Update screen, verify the details and then click the Authorise icon.

| SCREENS | WORKFLOW |
|---|---|
|  | Input Spread and Special Spread . |
| Input Spread and Special Spread | Enter a value in the Pds Action Id field. Click the FIND button. |
| Input Spread and Special Spread | Select a corresponding record and enter values in the following fields: Spread Rate Spcl Spread Rate The user can select the required number of records and update the fields. Click the Apply the chosen operation to the selected row(s) icon. Click the OK button in the dialog box. Spread Rate and Spcl Spread Rate is applied to the selected records successfully. |

| SCREENS | WORKFLOW |
|---|---|
|  | Input – Target Rate . |
| Input Target Rate | Enter a value in the Pds Action Id field. Click the FIND button. |
| Input Target Rate | Select a corresponding record and enter a value in the Target Rate field. The user can select the required number of records and update the fields. Click the Apply the chosen operation to the selected row(s) icon. Click the OK button in the dialog box. The Target Rate is applied to the selected records successfully. |

| SCREENS | WORKFLOW |
|---|---|
|  | Target Update Status Monitor . |
| Targetupdate Service Status | Enter values in the required fields. Click the FIND button. |
| Targetupdate Service Status | This screen displays the Target update Status of the PDS. Run the Target Update Service BNK/ID.TARGET.UPDATE |

|  | WORKFLOW |
|---|---|
|  | Input Simulation – Projection . |
| Contract Screen | Click the New icon. |
| PDS - Projection | Enter values in the following mandatory fields: Pool Ref Start Date End Date Click the Validate icon to check for errors and overrides. Click the Commit icon. |

This enquiry displays the list of PDS action IDs for reverse distribution. The user can create a new PDS simulation record.

To create new PDS simulation record, follow the below steps:

1. Input Simulation – Reverse Distribution .
2. In the Simulation – Reverse Distribution screen, click the New icon corresponding to a record.
3. In the PDS Simulation – Reverse Distribution screen, the following field values are automatically populated. Pool Ref Start Date End Date Action Reference
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon.


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to PDS - Simulation.


##### Enquiries and Reports

The section allows the user to view the Simulation calculation details.

View - Consolidated Simulation Results

This enquiry displays the Simulation calculation details.

Pool Income and Expenses details

The enquiry displays the income and expenses calculated for the Simulation period.

PDS Simulation Summary

This enquiry displays the simulation calculation results based on the deposit or account.

PDS Band wise Balances Summary

This enquiry displays the balances for each pool condition based on the band.

PDS-COPR Marked Accounts List

This enquiry displays the list of accounts that are marked as close on PDS run.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA


> **Related Applications:** `CATEG.ENTRY`, `ID.CATEG.ENT.DETAILS`, `ID.CATEG.ENT.UPDATE`, `ID.PDS.WEIGHT`, `ID.POOL.PARAMETER`

---


### 1.12  Charges


> **📇 Quick Reference Card**
> 
> **Key Fields:** *Def Account*, *Method*
> 
> **Sections:** 🔧 Working With


#### 🔧 Working With

Financial institutions can impose charges at the multi-currency arrangement on occurrence of a specific activity (activity charge) or on a specific frequency (scheduled charge).

These charges can be debit charges collected from customer or credit charges that can be paid to the customer. Only a flat amount can be collected or paid as a charge. The Issue Bill activity is triggered on the settlement arrangement for the activity or scheduled charge to get processed. The defined charge will only be capitalised against the defined settlement account. The Generate Charges Activity is used by the system to capitalise these charges to the liquidation account mentioned in the Settlement condition.

The system updates the base currency sub-account as the default settlement account of the MCY arrangement. During MCY account creation, the base currency sub-account may be created automatically by the system or manually by the user subject to product configuration .

When the base currency sub-account is created:

- Automatically ( by the system) – The system defaults the base currency sub-account as the Def Account . This Def Account cannot be changed during MCY arrangement opening. The charges like new arrangement fees can be collected from the base currency sub account. Post creation of the MCY Account, the user can amend the default settlement account which could be any sub-account within the MCY structure or an AR (Retail Account) account outside MCY structure.
- Manually (by the user) – The system defaults the base currency as the default settlement account Def Account during base currency sub-account opening if the field is blank.

It is possible to specify a Payment Type specific settlement account for different type of charges. When an account is updated in Def Account or other settlement accounts, the system ensures that the accounting condition is available for the Charge Property Class in that account.

> **⚠️ Note:** When a charge is defined at time of arrangement opening, if automatic creation of sub-account is not defined, the settlement account should be updated by the user. Else, charges cannot be collected.


##### Illustrations

The following section illustrates how a scheduled or an activity charge can be set up during MCY creation, raised and settled from liquidation account.


###### Activity Charges

It is possible to collect an account opening fee as an activity charge at the time of MCY arrangement opening. As the base currency account has to be opened automatically, the charge is collected from the base currency sub-account. In the below example a MCY arrangement is created with a debit and credit charge defined during MCY account creation. The following are defined:

- A new arrangement activity charge of USD10 (debit charge)
- A bonus charge of USD 20 (credit charge) is defined during MCY account creation.
- Method is set as Capitalise.

These charges are capitalised to the base currency sub-account.

In the MCY arrangement, the charge and bill info details are shown below.

The debit and credit Bill Details Overview display the charge amount, corresponding settlement account ID and charge property name.

The charges are created at the MCY arrangement level and collected from the liquidation account level using the Generate Charges Activity as seen below:


###### Scheduled Charge

Consider a USD10 annual administrative fee scheduled in the MCY arrangement.

The settlement account gets automatically updated with base currency sub-account.

The Payment Schedule condition gets updated.

---


### 1.13  SubAccounts


> **📇 Quick Reference Card**
> 
> **Applications:** `AA.PRODUCT.DESIGNER`
> 
> **Key Fields:** *Activity Link*, *Allowed Product*, *Base Ccy Product*, *Master Arrangement*, *Product Only*
> 
> **Sections:** ⚙️ Configuration


#### ⚙️ Configuration

The sub-accounts are account arrangements created in the product defined in the Allowed Product field of Sub-Arrangement Rules of the MCY product. The linkage between sub-arrangements and a parent arrangement within a multi-currency (MCY) account is supported using the Master Arrangement field of AAA. In addition, information related to the connection between the two arrangements is updated in the Activity Link type field .

Refer to Configuration of AR Accounts for more details on the configuration of Sub-Accounts.

Refer to Configuration of AR Accounts for more details on the configuration of Sub-Accounts.

Further, the arrangement account product for the sub-account should have the Product Only field set as ‘Mcy’ in the AA.PRODUCT.DESIGNER . This setup specifies that this product is for MCY sub-accounts only and it allows the bank to differentiate between the features of regular current, savings and MCY sub-accounts.


##### Automatic Creation of Base Currency Sub-Account

When the MCY arrangement is created, the system can be configured to create the base currency sub-account automatically. The automatic account creation can be configured by setting up the Base Ccy Product field in Sub-arrangement Rules condition of the MCY arrangement. The product should be a MCY only Product in AR product line. When the user gives this (Base Ccy Product) product in the Sub-arrangement of the MCY product configuration (or at MCY arrangement level), the base currency sub-account creates automatically in this product as part of MCY account creation.


> **Related Applications:** `AA.PRODUCT.DESIGNER`

---


### 1.14  Limit Balance


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Limit Property Class can maintain the balance information of total sanctioned, utilised, unutilised and excess.*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

The Limit Property Class can maintain the balance information of total sanctioned, utilised, unutilised and excess.

- In case of a single limit, the information is maintained on the same account that is linked with the limit.
- In case of a shared limit, the user can maintain this information in one of the accounts that is linked with the limit (or) can make use of a dedicated account.

The Limit Property Class holds the account information that maintains the limit balance information.

When a limit is defined based on a time code, it is possible to maintain balance information based on time code definition. The user can choose to maintain time code balances in addition to the summary balances.

Since limit balance information is maintained as balance types, the user can calculate fees or charges corresponding to each balance. For instance, the user can calculate

- A charge on the total limit amount
- An interest on the utilised and unutilised amount
- A penalty interest on the overdrawn limit amount.

---


### 1.15  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *&#9432; Content migrated from existing User Guide. Was earlier available as lore ipsum.*
> 
> **Applications:** `AA.PAYMENT.TYPE`, `AA.PRODUCT.DESIGNER`, `AA.PRODUCT.GROUP`, `AA.PRODUCT.LINE`, `AA.PROPERTY`, `AA.PROPERTY.CLASS`, `EB.EVENTS`, `LIMIT` ... +1 more
> 
> **Key Fields:** *Mandatory*, *Optional*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- APIs
- Temenos Transact Services

&#9432; Content migrated from existing User Guide. Was earlier available as lore ipsum.

Retail Accounts (AR) is one of the modules under Arrangement Architecture (AA) umbrella of products and is part of the Temenos Retail Banking suite of products.

The AR module provides financial account functionality and its maintenance for a financial institution. The module allows the user to create current or checking and savings accounts using the AA framework, under the Accounts product line, and perform a series of related activities on it.

A few of the key functionality included are:

- Create a new account arrangement
- Perform credit or debit activity or transactions for the account
- Accrue credit or debit interest accruals
- Capitalise interest to account balances
- Monitor charges and commissions
- Monitor inactivity or dormancy
- Issue cheque book or passbook
- Issue mandates


##### Configuring Retail Accounts

The AA.PRODUCT.LINE application provides a high-level definition of the business components (property classes), required to construct a product belonging to that line.

A product line is described by the property classes which constitute it. A financial institution can use these building blocks (property classes) to construct individual products, which can then be made available for sale to its customers.

AR has the following property classes.

| Column 1 | Column 2 | Column 3 |
|---|---|---|
| ACCOUNT ACCOUNTING ACTIVITY.API ACTIVITY.CHARGES ACTIVITY.MAPPING ACTIVITY.MESSAGING ACTIVITY.PRESENTATION ACTIVITY.RESTRICTION ALERTS AGENT COMMISSION BALANCE.AVAILABILITY | BALANCE.MAINTENANCE CHANGE.PRODUCT CHARGE CHARGE.OVERRIDE CLOSURE CONSTRAINT CUSTOMER DORMANCY ELIGIBILITY FACILITY INTEREST INHERITANCE | LIMIT OFFICERS PAYMENT.RULES PAYMENT.SCHEDULE PAYOFF PAYOUT.RULES PERIODIC.CHARGES PRICING.RULES REPORTING SETTLEMENT STATEMENT TAX |

The AA.PROPERTY is an instance of AA.PROPERTY.CLASS and these components constitute an account product. The property classes and properties are made Mandatory or Optional based on the AA.PRODUCT.GROUP level but subject to the Product Line definition. The AA.PRODUCT.DESIGNER is used to create the Account Products required.


##### Illustrating Model Parameters

The product conditions of a property class are evaluated to bring out the features of the property class. The system defaults the values in the product condition in an arrangement during its creation. The negotiability or default values and other restrictions are also defined in the product condition. These product conditions along with the properties derived from the property classes are grouped together to build products.

The product conditions are dated and some of the product conditions have currency as part of their ID. When the currency forms a part of the product condition ID, the user needs to create different conditions for each currency in which the product is available. When a new condition is created or an existing one is amended, the product to which the condition is linked has to be proofed and published.

| S.NO | Parameters | Description |
|---|---|---|
| 1 | Account | The Account property class is used by all the products which are account based. This property class primarily controls the description of the account. The ACCOUNT property allows the user to define and control balance treatment, posting restriction, linked account number (for memo accounts), currency market, date convention related setup for the account. Although the account names are account specific, generic titles can be defaulted from the product and can be replaced or given additional detail at the arrangement level. Each product defined and processed in AA can have a single ACCOUNT Property defined. |
| 2 | Activity Charges | The Activity Charges property class defines the charges that have to be applied when a particular activity is triggered on the arrangement. The charges so applied can be made due, capitalised or deferred. The user can enable auto settle the charges made due from unallocated credit balance by setting this to Yes. In accounts, charges are enabled for dormancy, settle payoff and ageing. This property class is also extensively used for all AA related modules, charges are set for various other activities. |
| 3 | Activity Restriction | The Activity Restriction property class is used to specify a restriction on a particular transaction. The restriction rules including the relevant periodic attributes and activities are defined in the product condition. These rules are then used to define activity based or property based restrictions. A rule if broken can be set to result in an override or error. A charge can be attached for this and can be set to be made due, capitalised or deferred. For the AR module, activity restriction is extensively used for restricting transactions by number, type, and so on. This is also extensively used in other modules to restrict the user from doing various user activity based on the life cycle status of contracts. |
| 4 | Balance Availability | The Balance Availability property class allows the user to control the following features pertaining to AR module: Notice amount and period, which needs to be given by a customer for withdrawing money from his account. Default Credit Check and Available Balance update related set up. Activity class or Activity specific credit check, and NSF related fees pertaining to it Tolerance Amount or Tolerance Currency - To indicate the grace amount, which is the allowed overdraft before the bank imposes NSF or OD fees. Overdraft Grace Period - To waive the NSF fee levied on the account, if the customer clears the debit balance within the stipulated grace period. |
| 5 | Dormancy | The Dormancy property class allows the user to control the parameterisation of inactive or dormant accounts and movement of the same into various buckets at the arrangement or product level. The same can be controlled based on period, and some exceptions or rules also can be added for evaluation and movement. The user can include or exclude certain activity or activity class for the evaluation. It is possible to, Configure different Dormancy status based on the period of inactivity Specify different charges and charging frequency for each Dormancy status Apply some exception rule filtering at an individual arrangement level (for example, account is in debit balance) and such rules can either be an API or a rule created using the Rules Engine Specify notices and notice frequency for each Dormancy status Specify Activities or Activity Classes or Activity Initiation Types which are qualified to keep an account active. Auto Reset can be enabled based on status or on Activity Type. |
| 6 | Facility | The Facility is a service component for financial products designed using arrangement architecture. The Facility property class controls the list of available services for an arrangement account. When an external activity (financial or non-financial) is triggered and the corresponding service group is mapped to an activity through Activity Mapping and EB.EVENTS . And the same came allowed or restricted or charged corresponding error message is raised to stop the activity. |
| 7 | Inheritance | The Inheritance property class is used for BN pool structure for inheriting the product conditions set at Parent level arrangement to the Child level arrangement accounts. The product conditions that are set for inheritance are attached to Property records with type as Inheritance Only. The properties to be inherited can be controlled both at source and target level. |
| 8 | Interest | The Interest property class is used for all interest definition and processing in AA. A product defined and processed in AA can have multiple interest properties defined (for example, principal interest, penalty interest, commission, etc. Interest rates can be defined as fixed , floating , periodic or linked rate (referring an INTEREST property from other arrangement), routine based calculation. Tiered interest can also be defined. Further it is possible to define a negative rate, minimum interest amount and waive the interest. Interest adjustment can be done in run time, and adjustment related detail or values can be captured in adjustment related fields. |
| 9 | Limit | The Limit property class primarily controls the use of LIMIT module by the product. We can set up single or shared limit. We can define the LIMIT.REFERENCE applicable for a specific product such that the system defaults the same in an arrangement. For a new limit, at the arrangement level, the LIMIT.SERIAL has to be given as NEW. The AR module can have self-contained secondary limit without having actual limit attached to it. Overdraft status or notice for AR module is handled inside the Limit Property class. Further Limits can be set to use the LIMIT module (AL and AD) or it can be managed only within the arrangement architecture framework. |
| 10 | Payment Schedule | The Payment Schedule property class is used by all products which have amounts billed (that is,made due) or capitalised or Pay. A Payment Schedule can be comprised of one or more payment definitions with conditions such as payment Type and Method, arrangement properties, dates and amounts. The AA.PAYMENT.TYPE application is used to define the standard payment types such as constant, linear, actual and fixed equal and so on, that can be used by a product. This payment type is then attached to each payment schedule definition. The start and end date can be specified, the user can specify the repayment of arrangement to commence after ‘n’ months from the arrangement date or ‘n’ months before the maturity or ‘n’ months after the change product or reset and rollover has happened. |
| 11 | Periodic Charges | The Periodic Charges property class acts as a container to group different charge properties and calculate a periodic charge amount. The Payment Schedule property class drives this property class. A periodic charge property can be attached in payment schedule and on schedule date periodic charge amount is calculated. At the arrangement level adjustment can be done by the user on whole periodic charge. |
| 12 | Statement | The Statement property class is used to define the legacy ACCT.STATEMENT feature at the AA level. Statements may be produced daily (every working day), every 1-9 weeks, twice a month (on the 15th and the last day of the month) or every 1-12 months on any day of the month. Up to nine statement cycles may be specified for each account, and each statement cycle is independent. In addition to this, special interim statements can be enabled. This property class also controls whether or not advices are to be produced when interest and charges are applied, and whether detailed interest statements (interest scale) should be produced. Within a statement cycle, it is possible to define multiple frequencies with a combination of weekly and monthly, such that statements are produced on the dates specified by both frequencies, but only contain details of entries since the last statement in that cycle. |


##### Illustrating Model Products

The AR product line provides current and savings account functionalities. The module allows the user to create savings or current accounts using the AA framework under the Accounts product line.

| S.No | Product Name | Product Attributes |
|---|---|---|
| 1 | Current Accounts | Corporate account with fixed debit interest Regular current account with floating Interest for both debit and credit interest, amount based capping of NSF Charges and waivers during account closure Current account with periodic charge Current account limit secured by deposit Current account for staff with additional interest Account with predefined overdraft limit of USD 250 Premium current account with some restriction on balance, and activities Current with some SME related features enabled Current account for SME - self service account Current account for students Current account for bundling, and gaining additional benefit through bundle Fully negotiable account Master account collects the interest from the Sub account and pays the interest accordingly Sub account pays the interest to the master account according to the maintained balance Payroll Account with cashback and count based capping of NSF Charges. Current Account for elite customers where the cheque issue fee is waived based on the relationship of the customer with the bank. The pricing evaluation runs on multiple arrangements of the customer which are fetched from Holdings MS and only those arrangements which are not in Non-accrual basis status is selected for pricing. Transact must be integrated with Holdings MS and the extension data mapping for this criteria set is to be configured locally to use this feature in the model product. |
| 2 | Savings Accounts | Regular saving account with basic features Regular saving account with restriction in Interest capitalisation Savings account for child Savings account for non resident Regular salary savings account Traditional notice savings account Savings account for staff |
| 3 | Summary Accounts | Summary account Currency summary account |


> **Related Applications:** `AA.PAYMENT.TYPE`, `AA.PRODUCT.DESIGNER`, `AA.PRODUCT.GROUP`, `AA.PRODUCT.LINE`, `AA.PROPERTY`, `AA.PROPERTY.CLASS`, `EB.EVENTS`, `LIMIT`, `LIMIT.REFERENCE`

---


### 1.16  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *Fixed Deposits is a part of the Retail Banking suite of products.*
> 
> **Applications:** `AA.PAYMENT.TYPE`, `AA.PRODUCT.LINE`
> 
> **Key Fields:** *Amount*, *Auto Settle*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- APIs
- Temenos Transact Services

Fixed Deposits is a part of the Retail Banking suite of products.

A deposit is an investment instrument in which the customer can invest a fixed amount for a defined period and interest rate of return on the investment.

Generally, the interest rate on deposit investments remains the same for the entire tenure. These investments secure the customer to avail benefits of fixed return without getting affected by the market fluctuations. Deposits are considered as liquid assets for the customers as they can be redeemed and converted to cash.

The customer can opt for the deposits to be either,

- Rolled over—allows the customer for better rate of return when interest rates are increased on deposit products, or
- Renewed automatically—provides special interest rates until the customer opts to close the deposit product.

A customer can use deposits as collaterals and pledge to raise loan. The bank can levy an additional interest for these loans, over and above the deposit interest rates. This additional interest is much lesser than the interest rates offered on regular loan products.

The banks offer savings schemes like Recurring Deposit, which encourage customers to deposit a fixed amount every month and earn interest.

The Retail Deposits (AD) module is a part of the Retail banking suite of products. It provides various deposit features that a financial institution can offer to its customer.

The AD module supports,

- An entire range of deposit features with configurable conditions. The system allows flexibility within which the bank can add new deposit products, to meet its ongoing requirements.
- The complete lifecycle of a deposit account that includes creation, funding, and maintenance of deposit. Maintenance activities include, Amendment of interest rate. Scheduling of periodic interest payment to customer accounts. Capitalisation of interest to deposit principal amount. Renewal and rollover of deposits. Change product. Redemption of deposits. Closure of deposits at maturity.
- The regulatory requirements, such as, Eligibility for opening and operating deposit accounts, Tax on interest. Restriction of operations such as cash deposits, multiple withdrawals etc. Risk Free Rates(RFR) processing using the Lookback market convention based on lookback days.

A financial institution can design a variety of deposit products to cater to the requirement of various customer segments. The user can design and configure a Product using the Temenos three-layer product configuration mechanism (that is, Product Line, Product Group, and Product) in the Product Builder application. This application helps the financial institution to deliver the product on time. Temenos’ robust Arrangement Architecture helps to minimise the time consumed to go to market with the product and modify the characteristics of the product as and when required with a flexible configuration and minimal customisation approach.

The system supports the banks to,

- Define various product conditions for term deposits and create different type of deposits based on the target customer requirements.
- Provide a powerful and user-friendly framework that supports diverse interest, fee, and transaction charges setup.
- Integrate with Temenos Pricing to offer an efficient preferential pricing tool, which is configurable based on the customer segmentation.
- Amend, reverse, or update arrangements with effective date as back date with recalculation and adjustment features, if required.
- Provide an option to settle funding and payout of deposit proceeds to multiple accounts and in multi-currency as well.
- Provide the user, role-based home pages with custom set of screens, enquiries, or menus as per the requirement of the user to perform daily tasks.


##### Configuring Retail Deposits

This topic enables the user to familiarise with the process of configuring the Retail Deposit (AD) module.


##### Property Classes

The Deposits under AA.PRODUCT.LINE provide high-level definition of the business components (property classes) required for the Deposit product line.

The Product Lines are defined by Temenos and cannot be created by the user.

The financial institution can use the business components to build individual deposit products based on the customer target-segment requirements.

The mandatory and optional property classes of Deposit Product line is available in the Deposits product line record. Read the Property Classes user guide for more information.


##### Product Builder

The application has the ability to enable the user to construct banking products by combining different business components. The PRODUCT.LINES feature provides the functionality for different banking areas, which are licensed by Temenos and each product line utilises a number of property classes (business components) that are fully configurable.

The Product Builder has the ability to,

- Build product families.
- Inherit properties from the product family structure.
- Determine the properties that a product is comprised of.
- Control the default values that can be applied to product arrangements.
- Apply dated conditions for products.
- Apply full control of scope of negotiation between product and arrangement conditions.
- Control negotiation of attributes over time.
- Design, proof, or publish lifecycle for product management.

Read the Arrangements COB processing user guide and Retail Deposits Services for more information.


##### Illustrating Model Parameters

The Product Conditions of a Property Class are evaluated to bring out the features of the Property Class. The system defaults the values in the Product Condition, in an arrangement during its creation. The negotiability, default values and other restrictions are also defined in the Product Condition. These conditions along with the Properties derived from the Property Classes are grouped together to build the Products.

The Product Conditions are dated and some of them have currency as part of their ID. When the currency forms a part of the Product Condition ID, then the user has to create different conditions for each currency in which the product is available. When a new condition is created or an existing condition is amended, the product to which the condition is linked, has to be proofed and published.

The model parameters consists of the following:

The Account Property Class is used by all products, which are account based. This Property Class primarily controls the description of the account. The Account Property allows the user to define and control balance treatment, posting restriction, linked account number (for memo accounts), currency market, date convention related setup for the account.

The Activity Charges Property Class defines the charges that have to be applied when a particular activity is triggered on the arrangement. These charges can be made due, capitalised or deferred. The user can enable auto settle the charges made due from unallocated credit balance by setting the Auto Settle field to Yes.

In accounts, charges are enabled for dormancy, settle payoff and ageing. This Property Class is also used for all AA related modules and charges are set for various other activities.

The Activity Restriction Property Class is used to specify the restriction on a particular transaction. The user can define the restriction rules including the relevant periodic attributes and activities in the Product Condition. These rules are then used to define activity-based or property-based restrictions. A rule, if broken, can be set to result in an override or error.

A charge can be attached to this Product Condition and set to be made due, capitalised or deferred.

The Term Amount Property Class is used by financial products, which involve an amount that is lent or deposited for a specified period. This Property Class controls the commitment made by the bank and the customer. The user must enter the total amount, which has to be lent or deposited for the term (that is, the committed amount) in the Amount field. During the product definition, it is common to restrict the initial amount through negotiation rules (for example, 5000

The user can also define one or more commitment tranches using the Term Amount Property Class.

The Interest Property Class is used for all interest definition and processing in AA. A product defined and processed in AA can have multiple Interest Properties defined (for example, principal interest, penalty interest, commission, etc.). The interest rates can be defined as fixed , floating, periodic, linked (referring an Interest Property from other arrangement), routine based calculation and tiered interest. Further, it is possible to define a negative rate, minimum interest amount and waive the interest.

Interest adjustment can be done in runtime, and adjustment related details or values can be captured in the adjustment related fields.

The Payment Schedule Property Class is used by all the products, which have amounts billed (that is, made due) or capitalised or pay. A Payment Schedule can be comprised of one or more payment definitions with conditions, such as payment type and method, arrangement Properties, dates and amounts. The AA.PAYMENT.TYPE application is used to define the standard payment types such as Constant, Linear, Actual and Fixed Equal etc., that can be used by a product. This payment type is then attached to each payment schedule definition. The user can specify the start and end dates, and the repayment of arrangement to commence after n months from the arrangement date or n months before the maturity or n months after the change product or reset and rollover has happened.

The Periodic Charges Property Class acts as a container to group different Charge Properties and calculate a periodic charge amount. The Payment Schedule Property Class drives this Property Class. A periodic charge property can be attached in payment schedule. On schedule date, periodic charge amount is calculated.

At the arrangement level, the user can adjust entire periodic charge.

The Payment Rules Property Class controls the sequence and order in which bills or outstanding balances need to be settled. An arrangement may have several bills outstanding and each bill may be comprised of multiple amounts (for example, principal, principal interest, penalty, tax, charges, etc.). When a customer makes a payment, the entire due amount may not be satisfied. The Payment Rules Property Class is used to define the method by which a single payment can be applied to multiple bills and amount types.

The Payout Rules Property Class is used by various Product Lines, which have amounts billed and made due for payment to the customer. It is used to define the method by which a single payment can be applied to multiple bills and amount types.

The Tax Property Class primarily controls the taxes applicable for the arrangement. Taxes can be calculated for Interest, Charges, Periodic charges, Account property, and activities. Tax can be calculated using either Net or Gross method for specific activities. The pre-defined tax rate or tax amount (for activities) can be overwritten at the arrangement activity level using context types.


##### Illustrating Model Products

The Retail Deposits (AD) Product Line provides Term Deposits, Bonds and Savings Plan functionalities. The module allows the user to create Term Deposits, Bonds and Savings Plan using the AA framework under the Deposits Product Line.

| S.No | Product Name | Product Attributes |
|---|---|---|
| 1 | Bonds | Bonds with Fixed term as 1 year Bonds with Fixed term as 3 year Bonds with Fixed term as 6 Months |
| 2 | Term Deposits | Term deposits for 3 months Term deposits for 6 months Term deposits for 9 months Term deposits for 12 months Term deposits for 18 months 2 year Term deposits 3 year Term deposits Long Term deposits Short Term deposits Call Deposits Fully Negotiable deposits |
| 3 | Savings Plan | Commitment Savings Plan |
| 4 | Retirement Plan Deposits | Term Deposits with tax condition defined to calculate withholding tax on the following activities: Deposit Withdraw Deposit Redemption Issue Bill for Deposit Interest The withholding taxes can be overwritten at the arrangement activity level by passing values using the context set of fields. |


> **Related Applications:** `AA.PAYMENT.TYPE`, `AA.PRODUCT.LINE`

---


### 1.17  Chargeoff


> **📇 Quick Reference Card**
> 
> **Applications:** `AA.ACCOUNT.DETAILS`, `AA.ACTIVITY.HISTORY`, `AA.BILL.DETAILS`, `AA.INTEREST.ACCRUALS`, `CATEG.ENTRY`, `RE.CONSOL.SPEC.ENTRY`
> 
> **Key Fields:** *Bill Type*, *Charge Off Amount*, *Charge Off Percentage*, *Charge off Amount*, *Charge off Percentage*, *Full Chargeoff*, *New Property Amount*, *Or Prop Amt* ... +8 more
> 
> **Sections:** 🔧 Working With


#### 🔧 Working With

Working with Loan Charge-off Key Features Charge-off is different from writing off the arrangement. The key features of charge-off are: A full or multiple partial charge-off transaction is possible. The interest on the charge-off balance should accrue, but is not passed to income. Reversal of charge-off transactions is possible Removal from charge-off or partial removal from charge-off (that is, a lessening of the charge-off amount) is possible as well. Dual accounting –that is, having two sets of books, the customer record vs. the bank record and applying payments independently to the two records. The charge-off feature is available for the Lending Product Line. The Charge-off Property has to be included in the product for charging off an account. Activity Class - Charge-off Full/Complete Charge-off The LENDING-CHARGEOFF-ARRANGEMENT Activity Class is used for charge-off of an arrangement. The complete outstanding in the loan is charged off. Partial Charge-off or Charge-off in Parts It is possible to charge off a loan, in parts. The LENDING-CHARGE-OFF-ACCOUNT Activity Class is used to charge-off the Account Property balance, based on the charge-off order. This is used to both charge-off an amount of principal (that is, increase charge-off amount) and to reduce the charge-off (that is, decrease the charge-off amount) if required. If a loan is being charged-off for the first time, this Activity is responsible for creating the charge-off balances as well as the customer’s shadow balances. Handling Charge-off under FASB Regulations For handling charge-off under certain specific regulations (FASB), the bank user uses the CHARGEOFF-REPORTING activity. Dual Accounting For loan contracts, apart from the customer balances, it is possible to store two separate balances, the bank balances along with the charge-off balances. When a Lending Product with Charge-off Property is proofed and published, the system automatically creates the balance type records to maintain charge-off balances along with the customer and bank balances. For a loan that is charged off, for CUR , the balances prior to the Charge-off Activity is stored as a shadow CUR CUST. The charge-off amount is stored in CUR CO and the amount under banks book is stored as CUR . The CUR CO charge-off balance, is the contingent balance and CUR CUST is a balance used for internal purpose and CUR is only non-contingent in nature. When the LENDING-CREDIT-ARRANGEMENT activity is processed, the amount credited to UNC is also credited to UNC CUST. When the LENDING-DEBIT-ARRANGEMENT activity is processed, the amount debited from UNC is also be debited from UNC CUST. Shadow Balances When a loan is charged-off, the borrower is unaware of this action, and continues to receive regular billing notices. As a result, when a loan is fully or partially charged off there is a situation to maintain two sets of books: A customer record (that is, the customer’s view of the balances and bills) A bank record (that is, the bank’s view of the balances). Prior to the charge-off, the customer and the bank records are the same (and therefore there is only one set of books). However once a loan is partially or fully charged off, the views are different. Customer Record Banks generally don’t communicate charge-off decision to the customers. So, a customer is unaware of a charge-off. Copying the balances prior to the Charge-off Activity creates a shadow record. This now becomes the customer record and does not include any of the effects of the charge-off. The bills and payments continue to be processed normally against this customer record. The payments received have to be apportioned as per the Payment Rules according to the customer. The customer balances are apportioned in this repayment order. Bank Record Full/Complete Charge-off For a full or complete charge-off using the LENDING-CHARGEOFF-ARRANGEMENT activity, there are no bank balances. The BNK balances are zero in this case. Charge-off in Parts/Partial Charge-off A charge-off creates the shadow balances for the customer record that do not include the effects of the charge-off (that is, the customer is completely unaware). As a result, the existing balances (customer balance less charge-off amount) continue to be referred to as the bank record and includes the effects of the charge-off (for example, the charged-off balance). As the arrangement advances, it also contains the interest accrual on the bank balance and charged-off balance separately. Additionally payments to the loan are allocated in a different manner on the bank record than on the customer record. This is based upon the value of the book balances and the status of the loan (for example, partially charged-off, fully charged-off or non-accrual). Internal inquiry screens display both the customer and the bank record, once a loan is partially or fully charged off. Reports breakdown the information this way as well – including both the bank balances and the customer balances. Charge-Off Balances The CUR CO and each ACC CO balance corresponds to the charge-off balance for the principal and the interest respectively. The system creates these balances by appending a CO at the end of each balance type. Multiple Interest Accruals For a full charge-off, the system accrues interest for charge-off and the customer balances namely CO and CUST balances. There is no bank balance to accrue interest for the BNK balances. For a partial charge-off (charge-off in parts), the system accrues interest for bank balance (for example, CUR ), charge-off and the customer balances. The system also accrues interest for the chargeoff and customer balances namely CO and CUST balances. It is necessary to accrue both charge-off and customer interest on the corresponding balances separately. Full/Complete Charge-off During a full charge-off, the arrangement balances are moved to the Chargeoff PL. As part of shadow accounting, CUR CUST and CUR CO balances are maintained during a full Chargeoff. This results in the accrual of balances per Interest Property for each of this principal balance. Each of them accrues interest at the same rate but based upon their balance. ACC CUST is accrued on CUR CUST and ACC CO is accrued on CUR CO. Though multiple interest accruals are done based on different balances, definition of source balance for each type of accrual is not required. Product configuration contains: Property Source INTEREST CURACCOUNT Corresponding Accruals in a full charge-off loan are: Balance Source ACCINTERESTCO CURACCOUNTCO ACCINTERESTCUST CURACCOUNTCUST Partial Charge-off or Charge-off in Parts In a partial charge-off, there are three balances: CUR , CUR CUST, CUR CO. Hence, there are three accrual balances per Interest Property and each accrues interest at the same rate but based upon their balance. ACC is accrued on CUR then ACC CUST is accrued on CUR CUST. Though multiple interest accruals are done based on different balances, definition of source balance for each type of accrual is not required. The interest is calculated on: Property Source INTEREST CURACCOUNT Corresponding accruals in a partial charge-off loan are: Balance Source ACCINTEREST CURACCOUNT ACCINTERESTCO CURACCOUNTCO ACCINTERESTCUST CURACCOUNTCUST Product Setup and Charge-off Balances When a Lending Product with Charge-off Property is proofed and published, the system automatically creates the below balance type records to maintain customer, bank and charge-off balances. Except bank balances, other balance type records which are created by system are contingent in nature. Bank Balances Charge-off Balances Customer Balances CUR CUR CO CUR CUST DUE DUE CUST CUST UNC UNC CUST ACC ACC CO ACC CUST DUE DUE CUST CUST CUR CO balance type holds the cumulative amount that’s been charged-off against an account. ACC CO balance type is used for posting the accrued interest on charged-off balances namely CUR CO. Dual Billing In the case where a loan is in Charge-Off status, AA.BILL.DETAILS is updated with both the customer and the bank due amounts. For a complete charge-off, the reflection of the charge-off billing is found in the billed balances. The bank amount is zero For a partial charge-off, two sets of figures (the customer and bank amounts) are calculated and stored on the bill. The customer and the bank amounts differ due to the effect of the charged-off principal as well as the alternate way of applying credits to the arrangement. Illustration of Partial Charge-off The changes that happen in an arrangement when a charge-off is performed is illustrated with the help of the below example. The arrangement is in delinquent status and is being charged off using the LENDING-CHARGEOFF-ACCOUNT Activity giving the transaction amount as 80,000 USD. This means 80,000 USD of principal is charged off. The Loan Arrangement Overview is displayed below. The Charge-off Activity is shown below. The Loan Arrangement Overview After Charge-off is shown below. Comparison of Arrangement Balances Before And After Charge-off The ECB balances before charge-off of 80,000 is shown below. The ECB balances after charge-off of 80,000 is shown below. Note that the arrangement balances have changed as a result of the charge-off. Bill Generated Before/After Charge-off On bill generation, AA.BILL.DETAILS is updated with both the customer and the bank due amounts for each of these accruals. AA.BILL.DETAILS stores the bank related fields that get updated on and after the charge-off of an arrangement. Once the charge-off is done, then the customer balances are stored in existing amount related fields and bank balances are stored in the BNK (bank) fields. Overdue processing is triggered based on the bills getting aged. The Os Prop Amt and Or Prop Amt fields of the bill are based on the customer balances(original amount) and regular overdue processing is triggered for the same. Balance type AA.BILL.DETAILS CUR Os Prop Amt Bnk Or Prop Amt Bnk CUR CUST Os Prop Amt Or Prop Amt Key Features of Full/Complete Charge-off A complete charge-off is done using the LENDING-CHARGEOFF-ARRANGEMENT activity. After a complete charge-off is made in the arrangement, the Full Chargeoff field in the AA.ACCOUNT.DETAILS application displays Yes. During charge-off, the loan principal is charged off to the PL Category assigned to the Account property class. The interest is charged off to the PL Category assigned to the Interest property class. Any tax is charged-off to the PL Category assigned to the Tax property class. Validations During a Complete Charge-off When this activity is executed, the system performs the below validations and results in error in below scenarios: The bank performs the charge off after clearing any outstanding credit balances of the loan (like UNC/INV/AVL). Hence if there are any credit balances available during a charge-off, the system raises the following error. When there is a charge with outstanding pay balance, the arrangement cannot be charged off. The pay balance must be cleared and then charge-off should be triggered in the system. Post charge-off, the banks do not prefer to disburse any further loans or increase the loan commitment further. Hence, the disbursement activity is not allowed after the charge off. During the cooling and cancel period, the loan charge-off is not allowed. Any income to the arrangement is booked to the Chargeoff PL of that Property An arrangement that has undergone partial charge-off can undergo full charge-off, but an arrangement that is completely charged off cannot be charged off further. Loans cannot go to negative rate when loan is in charge-off. Dormant loans cannot be charged off. When an arrangement has a charge set to amortise, the charge cannot be charged off. The system raises an error when the user tries to do a full charge-off when there is a charge amortisation in progress. During charge-off, the system calculates the penalty interest if this has been configured and this helps the bank to access the real charge-off amount for all the property. Illustration of Charge-off Consider a loan that has few bills outstanding and is delinquent. Perform a charge-off. The charged-off arrangement is shown below. The charge-off information in AA.ACCOUNT.DETAILS is as shown below. Arrangement Balances Movement The loan principal balances and billed interest balances are moved to Chargeoff PL and are stored in CO and CUST balances as off-balance sheet items. Here, the sum is: ACCPRINCIPALINTCO=ACCPRINCIPALINTCUST+DELPRINCIPALINTCUST CURACCOUNTCO=DELACCOUNTCUST+CURACCOUNTCUST Bills A bill that was already generated is also updated with the charge-off information. In a full charge-off, the BNK balances for the Property after charge-off is zero. The billed amount and outstanding balance here represents the CUST balance, as shown below Interest Accruals After a charge-off, the interest accruals are under CUST and CO balances. Charge Bills Charge-Off An arrangement with interest and charge bills is being fully charged off, including all interest and charges in the bills along with outstanding principal. Any Activity Charge, Periodic Charge and Rule break charge are also charged off. This is subject to certain evaluation: The system evaluates if there are any pay charges outstanding and raises an error to indicate that the same must be settled. The system evaluates if there is charge collected that is undergoing amortisation, then the system doesn’t allow to charge off that arrangement. Consider an arrangement that has been charged off. During a charge-off, charge bills are also charged off. A rule break that is being charged off is shown below. The balances after the charge-off, also reflects the charges being charged off. Accounting for Charges in Charge-off RE.CONSOL.SPEC.ENTRY is generated during the charge-off of the principal decrease fee, a rule break fee. For charge-off books it is as shown below. For customer books it is as shown below. Activity Charge for charge-off books is shown below. Activity Charge for customer books is shown below The charge-off entries for the charge debited in the banks PL are as follows: For the Rule break fee: For the Activity Charge: Charge-off of Upfront Profit Contracts It is possible to setup upfront profit in loan arrangements. For such a loan, the interest is collected upfront and is booked to the PL over a period as accruals. Read Islamic Finance-Upfront Sale for more information. The below arrangement has upfront bills with outstanding bills. This arrangement has a profit amount of 10,000 USD that is collected for a year’s tenure. The upfront profit is booked between RECDEFERREDPFT and ACCDEFERREDPFT at the time of booking the arrangement. DR RECDEFERREDPFT -10,000 CR ACCDEFERREDPFT 10,000 During accruals, the profit is booked between ACCDEFERREDPFT and PL DR ACCDEFERREDPFT -48.84 CR PL 48.84 The accruals for the month are -1513.79 and the balance in ACCDEFERREDPFT is 8486.21 at the end of month. On the due date of the profit, the accruals of the month are posted to the RECDEFERREDPFT from DUEDEFERREDPFT DR DUEDEFERREDPFT -1513.79 CR RECDEFERREDPFT 1513.79 As a result of this, RECDEFERREDPFT has a balance of -8486.21 Time Head Movement Balances Creation RECDEFERREDPFT -10,000 -10,000 Creation ACCDEFERREDPFT 10,000 10,000 Monthly Accrual ACCDEFERREDPFT -1513.79 8486.21 Due date RECDEFERREDPFT 1513.79 8486.21 Illustration of Charge-off Upfront Profit The arrangement is now charged off. The balances from CURACCOUNT have moved to CURACCOUNTCO. A part of the principal amount is billed already. So CURACCOUNTCUST+DELACCOUNTCUST amounts to the total principal. The bill is in delinquent status from the customer perspective and the balance is stored in DELDEFERREDPFTCUST as -1513.79. The RECDEFFEREDPFTCUST gives the outstanding amount as per customer, -8,486.21 that is pending receivable. There are four days accrual after the last bill date for 180.38 that has resulted in the ACCDEFERREDPFTCUST is 8305.83 (8,486.21-180.38). Time Head Movement Balances Creation RECDEFERREDPFT -10,000 -10,000 Creation ACCDEFERREDPFT 10,000 10,000 Monthly Accrual ACCDEFERREDPFT -1513.79 8486.21 Due date RECDEFERREDPFT 1513.79 8486.21 4 days accruals after due date ACCDEFERREDPFT -180.37 8305.83 Repayment in the Charge-Off Loan A repayment received in the upfront profit loan arrangement is allocated as per the payment rule given below. The balances of the same loan arrangement after a couple of days are; Time Head Movement Balances Creation RECDEFERREDPFT -10,000 -10,000 Creation ACCDEFERREDPFT 10,000 10,000 Monthly Accrual ACCDEFERREDPFT -1513.79 8486.21 Due date RECDEFERREDPFT 1513.79 8486.21 6 days accruals after due date ACCDEFERREDPFT -270.56 8215.64 The same update is in the AA.INTEREST.ACCRUALS as shown below. A payment of 5000 on the arrangement and this is apportioned against the CUST and CO balances as per the Payment Rules and Chargeoff Rules respectively. In customer perspective, the Payment Rules apportions the payment towards to DEFFEREDPFT first and then the ACCOUNT Property as seen below. The same is reflected in arrangement balances as shown below. In charge-off perspective, the repayment works as explained below. The Charge-off condition governs the repayment rule for charge off balances. The Charge-off condition for the upfront profit loan is given below. In this arrangement, the loan is fully charged off. So the Billed and Current Balance Type options do not have any impact and the system apportions the payment for the CHARGEOFF balance type. Thus, the full payment of 5000 is apportioned to the ACCOUNT balance. This can be seen in the screenshot below. In banks’ books repayment is as explained below. The repayment is received in the banks’ book against the CHARGEOFF PL as indicated in Accounting Condition. The repayment of 5000 is credited to the PL indicated in this accounting condition as seen below. Charge-off in Charge Component - Upfront Profit Contract In the contract below, a charge booked at the time of arrangement creation is shown. The impact on the charge bill during a charge-off is shown in the subsequent screenshots The arrangement balances before a charge-off are shown below. The arrangement balances after charge-off as shown below. A comparison of the bill details before and after the charge-off is shown below: The accounting entries in charge-off are as follows: The charge-off entry in the PL, is a debit to the banks PL as seen in CATEG.ENTRY . The charge-off entries to bank and customer books are as RE.CONSOL.SPEC.ENTRY . In the charge-off books, the CO entry is as shown below. In the customer books, the CUST entry is as shown below.

In a business situation where the bank user must capture a bill in a loan that has undergone charge-off, the user can do so with the capture bill (LENDING-CAPTURE.BILL-BALANCE.MAINTENANCE) activity on such a loan. This activity can be used only for the arrangement that has undergone a full charge-off (LENDING-CHARGEOFF-ARRANGEMENT). As a result of this bill capture activity, the system releases the bill and balances in the customer books and the charge-off books.

Consider a scenario of dispute with the customer and the contract is charged off. The bank prefers to collect some charges or re-raise a bill that was previously paid, due to a customer dispute. In this case, the bank user can capture the bill and record it as an outstanding amount with the customer.

Consider a loan that is fully charged off using the LENDING-CHARGEOFF-ARRANGEMENT activity. The balances charged-off include the principal and interest as highlighted below.

- Charge-off principal - 46,369.61 (Outstanding principal).
- Charge- off interest - 31.62 (Accrued interest amount after the first installment).

This loan has only one installment bill which is already settled.

In this example, the client has raised a dispute with the bank on the 3871.49 bill dated Apr 12, 2023. So, the bank decides to refund the bill. At a later date, the claim is proved false and the bank wanted to raise the bill with the same amount for the customer.

The user captures the bill in this charged-off loan using the LENDING-CAPTURE.BILL-BALANCE.MAINTENANCE activity. The details of Bill Type , Payment Type , Payment Method , Payment amount , Property , Original Property Amount , and New Property Amount are entered based on the first installment bill details.

Though the bill is to claim the dues that were refunded earlier, the capture bill can be raised only for the current value date (not forward or back-valued) for the required payment type, bill type, and the bill amount for the components required. The bill date must also be the current date (not forward or back-valued).

Post capture bill activity, a due bill is created, and the system automatically updates the respective charge-off balances and customer balances in ECB.

Post capture bill activity:

- The charge-off principal is updated as 50000 (46169.61 + 3830.39)
- The charge-off interest is updated as 72.72 (31.62 + 41.10).

When an activity is triggered back-valued after this capture bill activity, the capture bill activity is also effectively reversed and replayed. As the bill is a manually created bill, the components of the bill do not undergo a change but the bill is reversed and replayed staying unaffected.


##### Handling Charge-off under FASB Regulations

In order to provision loan under FASB, the user can trigger the LENDING-CHARGEOFF-REPORTING activity and specify the required charge-off amount or percentage.

Consider a delinquent loan with the balances stated below.

The user triggers the Charge Off Reporting activity from the New Activities menu on the loan overview screen.

The user inputs the required Charge off Amount for partial charge-off of the loan.

> **⚠️ Note:** To achieve partial charge-off, either the Charge Off Amount or Charge Off Percentage attribute can be used. In case a percentage is specified, the percentage is converted into amount and stored.

Charge off details updated in AA.ACTIVITY.HISTORY are shown below:

Charge off details updated in AA.ACCOUNT.DETAILS are shown below:

Consider a delinquent loan with the balances stated below.

The user prefers to fully charge-off the loan and provides the Charge off Percentage as 100.

The charge off details updated in AA.ACTIVITY.HISTORY are shown below.

The percentage is converted to amount by an API and stored.

Charge off details updated in AA.ACCOUNT.DETAILS are shown below:

> **⚠️ Note:** Only during a full charge-off the Full Chargeoff attribute is updated as Yes.

| AA Activity | IFRS Operation | Description |
|---|---|---|
| LENDING-IFRS.CHARGEOFF-REPORTING | CHARGE OFF | Indicates the loan is charged-off for the first instance. |
|  | CHARGE OFF INCREASE | Indicates loan is charged- off for an additional amount from earlier levels. |
|  | CHARGE OFF DECREASE | Indicates loan charge-off amount is decreased by specifying a negative amount. |
| LENDING-APPLYPAYMENT-PAYMENT.RULES ENDING- | RECOVERY | Indicates a repayment made on the loan. |
| LENDING-WRITE.OFF-BALANCE.MAINTENANCE | WRITE OFF | Indicates loan has been completely written off |
|  | WRITE OFF PARTIAL | Indicates a partial write off scenario which instead of entire loan only certain bills and/or balances are written off on contract. |
|  | ADJUSTMENT | Indicates any bill and/or balance adjustments made on the contract. |
| LENDING-MATURE-ARRANGEMENT | MATURE | Indicates loan has matured |
| LENDING-RESUME-ARRANGEMENT | RESUME | Indicates loan is resumed |

The following section provides examples of using SUSPEND.STATUS and CHARGEOFF.STATUS periodic attributes

The SUSPEND.STATUS periodic attribute allows the user to evaluate if loan is suspended or not and suitably configures any activity restrictions based on the suspense status of the loan. The evaluation is done based the suspend information stored in AA.ACCOUNT.DETAILS and allows the bank user to configure an error/override in the Activity Restriction condition.

Consider an example in which user needs to restrict a charge-off operation on a performing loan which is not suspended. If this periodic attribute is configured at product or arrangement level, then a user cannot trigger the charge off activity on a loan which is not suspended.

A rule is configured to check if the loan is in suspended status or not.

The rule is evaluated when an activity (charge off activity is considered in the case below) is triggered and based on the evaluation result an override (or error) is raised. Additionally, a rule break charge is applied if necessary.

This periodic attribute allows the user to evaluate and place activity restrictions based on the charge off status of the loan. This evaluates the charge off information in AA.ACCOUNT.DETAILS and allows the bank user to configure an error/override in Activity Restriction condition, based on the charge off status of the loan.

Consider an example in which user needs to restrict a resume operation on a charged-off loan. If this periodic is configured at product or arrangement level, then the user cannot trigger resume on a loan which is fully and/or partially charged-off.

A rule is configured to check if the contract is in suspended status or not. The rule can be configured to evaluate if loan is fully or partially charged-off.

The rule is evaluated when an activity (resume activity is considered in the case below) is triggered and based on the evaluation result an override (or error) is raised. Additionally, a rule break charge is applied if necessary.


> **Related Applications:** `AA.ACCOUNT.DETAILS`, `AA.ACTIVITY.HISTORY`, `AA.BILL.DETAILS`, `AA.INTEREST.ACCRUALS`, `CATEG.ENTRY`, `RE.CONSOL.SPEC.ENTRY`

---


### 1.18  Charges


> **📇 Quick Reference Card**
> 
> **Applications:** `EB.ACCRUAL`
> 
> **Key Fields:** *Start Date*
> 
> **Sections:** 🔧 Working With


#### 🔧 Working With

The following are different scenarios encountered while processing loan charges.


##### Charge Currency Different from Arrangement Currency

When the charge currency is different from arrangement currency , an override message is displayed as below.


##### Rule Break Charges

The below screenshot displays the Arrangement Overview.

The Term Amount increases AA activity and the associated override message is seen when the activity is committed.

Changes can be seen in the Total Commitment and the charges that were associated with the increase in Term Amount can be seen.


##### Amortisation of Charges

Once an arrangement has been created, an EB.ACCRUAL record is created per configuration for the amortisation process. Each record shows certain information, such as the daily accrual to date and the start and the end date of accrual.

The below screenshot displays EB.ACCRUAL record.


##### Stop Suspend / Resume Amortisation of Charges

Consider a loan product with Processing Fee (Debit charge) of $100 fee collected from customer upfront and amortised from the loan creation date until maturity. Loan Term is 100 days. The daily amortised fee amount is $1.

The fee amortisation is set to Stop Suspend from the day the loan is moved to non-performing stage. The amortisation of the said Processing Fee when the charge is Stop Suspend is tabulated below. The amortisation of the fee for Suspend charge type is also illustrated to draw comparison between the accounting entries booked against both charge types.

| TERM DAYS | SUSPEND | STOP.SUSPEND |
|---|---|---|
| Day 1 | Dr ACC 100 Cr P/L 0 | Dr ACC 100 Cr P/L 0 |
| Day 5 (COB) | Dr ACC 95 Cr P/L 5 | Dr ACC 95 Cr P/L 5 |
| Day 60 (COB) | Dr ACC 40 Cr P/L 60 | Dr ACC 40 Cr P/L 60 |
| Day 61 | Loan moved to ‘Non-Performing’ status |  |
| Day 61 (COB) | Dr ACC 39 Cr P/L 60 Cr ACC SP 1 | Amortization is stopped until Resume is triggered. |
| Day 80 (COB) | Dr ACC 20 Cr P/L 60 Cr ACC SP 20 | Amortization is stopped until Resume is triggered. |
| Day 81 | Loan Resumes to 'Performing' status |  |
| Day 81 (COB) | Dr ACC 19 Cr P/L 81 Cr ACC SP 0 | Dr ACC 38 Cr P/L 62 |
| Day 91 (COB) | Dr ACC 9 Cr P/L 91 | Dr ACC 18 Cr P/L 82 |
| Day 100 (COB) | Dr ACC 0 Cr P/L 100 | Dr ACC 0 Cr P/L 100 |


##### Suspend or Resume Accrual or Amortisation of Credit Charge

Consider an example where a loan product is set with a Charge property that is payable (Credit type) and set to Suspend. The charge is set to be amortized until maturity.

For illustration, the arrangement created for this loan product with Agent Expense (Credit charge) with a Pay bill for $100. The amortisation is configured for $1 daily and set to happen from the loan creation date until maturity. Loan Term is 100 days. Assume the charges are booked upfront and amortized over the term.

Further, the amortisation of the charge is set to Suspend from the day the loan becomes non-performing.

The below illustration tabulates the amortisation of the said ‘Agent Expense’ when the charge is Suspend. The amortisation of a debit charge with property type Suspend is also illustrated to draw comparison between the accounting entries booked against both credit and debit charge.

- ACC represents unamortized fee balance.
- ACC SP represents suspended fee balance.
- Income P/L represents the income account/head into which fee income is amortized.
- ACC represents unamortized agent expense balance.
- ACC SP represents suspended expense balance.
- Expense P/L represents the expense account/head into which expense is amortized.

All amounts in the table below indicate closing balances under the respective heads. Assume income and expense heads are zero to begin with.

| TERM DAYS | AMORTISATION OF CREDIT CHARGE[BG1] [SN2] | AMORTISATION OF DEBIT CHARGE |
|---|---|---|
| Day 1 | Expense P/L 0 ACC -100 | ACC 100 Income P/L 0 |
| Day 5 (COB) | Expense P/L -5 ACC -95 | ACC 95 Income P/L 5 |
| Day 60 (COB) | Expense P/L -60 ACC -40 | ACC 40 Income P/L 60 |
| Day 61 | Loan Suspended due to ‘Non-Performing’ status |  |
| Day 61 (COB) | Expense P/L -60 ACC -39 ACC SP -1 | ACC 39 Income P/L 60 ACC SP 1 |
| Day 95 (COB) | Expense P/L -60 ACC -5 ACC SP -35 | ACC 5 Income P/L 60 ACC SP 35 |
| Day 96 | Loan Resumes to 'Performing' status |  |
| Day 96 (At Resume) | Expense P/L -95 ACC -5 ACC SP 0 | ACC 5 Income P/L 95 ACC SP 0 |
| Day 96 (COB) | Expense P/L -96 ACC -4 ACC SP 0 | ACC 4 Income P/L 96 ACC SP 0 |
| Day 100 (COB) | Expense P/L -100 ACC 0 ACC SP 0 | ACC 0 Income P/L 100 ACC SP 0 |


##### Income Recognition Using Cost-Recovery Method

Read Income Recognition Under Cost Recovery Method section in Interest property class for more information on the underlying configuration.

Consider the following example where a contract is booked with the following details.

- Tenure -150 Days.
- Per-day daily accrual in the account - 1.
- Interest property type for PRINCIPALINT - SUSPEND,SUSPENDOVERDUE,AMORT RECOVERY SUSPEND.
- Interest property type for PENALINT - SUSPEND, AMORT RECOVERY SUSPEND.

The following table shows how the income recognition works under Cost-Recovery method:

| Activity | Principal Interest (Set to Suspend Overdues) | Remarks for Principal Interest balance movement | Penal Interest (Set to Suspend) | Remarks for Penal Interest balance movement |
|---|---|---|---|---|
| Day 1 | Accrued Principal Interest [ACC PRINCIPAL INT] – 0 P/L - 0 | Daily Accruals happen from Day 1 to day 90 | Accrued Penalty Interest [ACC PENALINT] – 0 P/L - 0 |  |
| Day 10 | ACC PRINCIPALINT – 10 Dr P/L – 10 Cr |  | ACC PENALINT – 0 P/L - 0 |  |
| Day 90 | ACC PRINCIPALINT – 90 Dr P/L – 90 Cr |  | ACC PENALINT – 0 P/L - 0 |  |
| Day 91 – Loan suspend due to prolonged delinquency | ACC PRINCIPALINT – 90 Dr Suspended Principal Interest ACC PRINCIPALINT SP – 90 Cr P/L - 0 | On Day 91, the loan is suspended. The balance from P/L is moved to ACCPRINCIPALINTSP | ACC PENALINT – 0 Suspended Penalty Interest ACC PENALINT SP – 0 P/L - 0 |  |
| Day 100 | ACC PRINCIPALINT – 100 Dr ACC PRINCIPALINT SP – 100 Cr |  | ACC PENALINT – 10 Dr ACC PENALINT SP – 10 Cr | Daily Accruals for PENALINT happen from Day 100 |
| Day 101 – Repayment 35 | ACC PRINCIPALINT – 70 Dr Repayment applied as per payment rule to due interest ACC PRINCIPALINT SP – 70 Cr Based on repayment amount 30 debited from SP and credited to IAP Interest applied to principal [RSP PRINCIPALINT] – 30 Cr P/L - 0 | Repayment of principal interest is done on Day 101. The balance from ACCPRINCIPALINTSP is moved to RSP PRINCIPALINT | ACC PENALINT – 5 Dr Repayment applied as per payment rule to due interest ACC PENALINT SP – 5 Cr Repayment amount of 5 debited from SP and credited to IAP Interest applied to principal [RSP PENALINT] – 5 Cr P/L - 0 | Repayment of penal interest is done on Day 101. The balance from ACC PENALINTSP is moved to RSP PENALINT |
| Day 110 EOD | ACC PRINCIPALINT – 80 Dr ACC PRINCIPALINT SP – 80 Cr RSP PRINCIPALINT – 30 Cr P/L - 0 |  | ACC PENALINT – 15 Dr ACC PENALINT SP – 15 Cr RSP PENALINT – 5 Cr P/L - 0 |  |
| Day 111 – Repayment 95 (principal interest – 80 and penal interest - 15) | ACC PRINCIPALINT – 0 ACC PRINCIPALINT SP – 0 RSP PRINCIPALINT – 110 Cr P/L – 0 |  | ACC PENALINT – 0 ACC PENALINT SP – 0 RSP PENALINT – 20 Cr P/L - 0 |  |
| Day 111 – RESUME | ACC PRINCIPALINT – 0 ACC PRINCIPALINT SP – 0 RSP PRINCIPALINT – 0 Amortization record (ACR) generated for RSP balance. ACR PRINCIPALINT – 110 Cr Straight line amount calculated at 110/40 = 2.75 per day P/L – 0 | On day 111 the loan is resumed. Amortization record is generated for RSP. The balance is moved from RSP PRINCIPALINT to ACR PRINCIPALINT | ACC PENALINT – 0 ACC PENALINT SP – 0 RSP PENALINT – 0 Amortization record (ACR) generated for RSP balance ACR PENALINT – 20 Cr Straight line amount calculated at 20/40 = 0.50 per day P/L - 0 | On day 111 the loan is resumed. Amortization record is generated for RSP. The balance is moved from RSP PENALINT to ACR PENALINT |
| Day 111 EOD | ACC PRINCIPALINT – 1 Dr ACC PRINCIPALINT SP – 0 RSP PRINCIPALINT – 0 ACR PRINCIPALINT – 107.25 Cr P/L – 3.75 Cr [1 from daily accrual and 2.75 from recovery interest] | Straight line amount calculated at 110/40 = 2.75 per day ACR PRINCIPALINT is debited by 2.75 and Income a/c is credited. | ACC PENALINT – 0 ACC PENALINT SP – 0 RSP PENALINT – 0 ACR PENALINT – 19.50 Cr P/L – 0.50 Cr [from recovery interest] | Straight line amount calculated at 20/40 = 0.50 per day ACR PENALINT is debited by 0.50 and Income a/c is credited |
| Day 120 EOD | ACC PRINCIPALINT – 10 Dr ACC PRINCIPALINT SP – 0 RSP PRINCIPALINT – 0 ACR PRINCIPALINT – 82.5 P/L – 37.5 [10+27.50] |  | ACC PENALINT – 0 ACC PENALINT SP – 0 RSP PENALINT – 0 ACR PENALINT – 15 P/L – 5 |  |
| Day 130 EOD | ACC PRINCIPALINT – 20 Dr ACC PRINCIPALINT SP – 0 RSP PRINCIPALINT – 0 ACR PRINCIPALINT – 55 P/L – 75 [37.50+10+27.50] |  | ACC PENALINT – 0 ACC PENALINT SP – 0 RSP PENALINT – 0 ACR PENALINT – 10 P/L – 10 |  |
| Day 131 – Loan Suspend due to market conditions – EOD | ACC PRINCIPALINT – 21 Dr ACC PRINCIPALINT SP – 21 Cr [20+1] RSP PRINCIPALINT – 0 ACR PRINCIPALINT – 52.25 ACR PRINCIPALINT SP – 2.75 P/L – 55 (20 reversed to ACC SP) | Loan is suspended from day 131. The property PRINCIPALINT is configured as “SUSPEND OVERDUES”. The income which is booked so for is reversed to ACCSP. P/L is debited and ACC PRINCIPALINT SP IS credited. | ACC PENALINT – 1 Dr ACC PENALINT SP – 1 Cr RSP PENALINT – 0 ACR PENALINT – 9.50 ACR PENALINT SP – 0.50 P/L – 10 | Here the PENALINT property is configured as ‘SUSPEND’. Here no income is booked so far and hence reversal is not required. |
| Day 140 EOD | ACC PRINCIPALINT – 30 Dr ACC PRINCIPALINT SP – 30 Cr RSP PRINCIPALINT – 0 ACR PRINCIPALINT – 27.5 ACR PRINCIPALINT SP – 27.5 P/L – 55 |  | ACC PENALINT – 10 Dr ACC PENALINT SP – 10 Cr RSP PENALINT – 0 ACR PENALINT – 5 ACR PENALINT SP – 5 P/L – 10 |  |
| Day 141 – Repayment – 40 (30 repaid towards Principal Interest+10 repaid towards Penal Interest) | ACC PRINCIPALINT – 0 ACC PRINCIPALINT SP – 0 RSP PRINCIPALINT – 30 Cr ACR PRINCIPALINT – 27.5 Cr ACR PRINCIPALINT SP – 27.5 Cr P/L – 55 |  | ACC PENALINT – 0 ACC PENALINT SP – 0 RSP PENALINT – 10 Cr ACR PENALINT – 5 Cr ACR PENALINT SP – 5 Cr P/L – 10 |  |
| Day 141 – Resume 2nd time | ACC PRINCIPALINT – 0 Dr ACC PRINCIPALINT SP – 0 Cr RSP PRINCIPALINT – 0 ACR PRINCIPALINT – 85 Cr (27.5+27.5+30) ACR PRINCIPALINT SP – 0 P/L – 55 | Each time resume is triggered, based on RSP and ACRSP balance a new amortization record is generated in EB Accrual application. | ACC PENALINT – 0 Dr ACC PENALINT SP – 0 Cr RSP PENALINT – 0 ACR PENALINT – 20 (5+5+10) ACR PENALINT SP – 0 P/L – 10 |  |
| Day 141 EOD | ACC PRINCIPALINT – 1 Dr ACC PRINCIPALINT SP – 0 Cr RSP PRINCIPALINT – 0 ACR PRINCIPALINT – 76.5 Cr Amortization resumed at 85/10 =8.50 per day ACR PRINCIPALINT SP – 0 P/L – 64.50 [55+8.50+1] |  | ACC PENALINT – 0 Dr ACC PENALINT SP – 0 Cr RSP PENALINT – 0 ACR PENALINT – 18 Amortization resumed at 20/10 = 2 per day ACR PENALINT SP – 0 P/L – 12[10+2] |  |
| Day 145 EOD | ACC PRINCIPALINT – 5 Dr ACC PRINCIPALINT SP – 0 RSP PRINCIPALINT – 0 ACR PRINCIPALINT – 32.5 Cr ACR PRINCIPALINT SP – 0 P/L – 102.5 [64.50+(8.50*4)+(1*4)] |  | ACC PENALINT – 0 Dr ACC PENALINT SP – 0 RSP PENALINT – 0 ACR PENALINT – 10 Cr ACR PENALINT SP – 0 P/L – 20 [12+(2*4)] |  |
| Day 150 EOD – Loan Maturity | ACC PRINCIPALINT – 10 Dr ACC PRINCIPALINT SP – 0 RSP PRINCIPALINT – 0 ACR PRINCIPALINT – 0 A CR PRINCIPALINT SP – 0 P/L – 150 [102.50+(8.50*5)+(1*5)] |  | ACC PENALINT – 0 Dr ACC PENALINT SP – 0 RSP PENALINT – 0 ACR PENALINT – 0 ACR PENALINT SP – 0 P/L – 30 [20+(2*5)] |  |
| Day 150 – Payoff |  | After loan is payoff |  |  |
| After payoff |  | ACC PRINCIPALINT – 0 ACC PRINCIPALINT SP – 0 RSP PRINCIPALINT – 0 ACR PRINCIPALINT – 0 ACR PRINCIPALINT SP – 0 P/L – 150 | ACC PENALINT – 0 ACC PENALINT SP – 0 RSP PENALINT – 0 ACR PENALINT – 0 ACR PENALINT SP – 0 P/L – 30 |  |

> **⚠️ Note:** Each time a resume is triggered, based on RSP and ACRSP balance a new amortization record is generated in the EB.ACCRUAL application.


##### Preferential Pricing

The below screenshot displays the New Arrangement Fee waived off because the arrangement has been created as a Valued Customer.


##### Rebate Processing

The below screenshot displays the rebate processing.

For some loan products, the customers protect their loan commitment with the help of insurance covers against risks such as death and disability. The insurance policy can be for the entire loan term or particular period such as yearly and then it is renewed at the end of every period. Rebate processing provides a facility to rebate the outstanding amount of premium for loan insurance on pre-closure or on cancellation at a later stage or cancellation within a certain grace period.

The aim of the rebate processing feature is, to render the ability to use a local routine for certain types of amortisation calculation. However, in AA, the generic accrual processing mechanism allows the user to amortise or accrue fixed amounts supplied by applications through a direct API or accounting entries. The standard method of processing is to straight line the amount on a daily basis.

It is possible to post to an internal account category (instead of PL) in the Accounting version.

The user can define the start date of accrual calculation. From that day, the accrual and account postings begin. On the first day, the calculation is based on the beginning of the accrual period – Start Date in the EB.ACCRUAL record. The changes to the grace period is considered only if the record is reversed, and if the record is reversed, no accounting activity takes place.

This feature provides an option to rebate the outstanding amount of premium for loan insurance on pre-closure or on cancellation at a later stage or cancellation within a certain grace period.

Home loan insurance, or any mortgage redemption insurance plan, is part of a banker's sales pitch when extending sizable long-term credit, such as a home loan. These plans hedge the risk of loss in case the borrower dies or becomes disabled during the loan term, especially an unsecured loan. The banks fund the insurance portion as part of the loan amount, which is repaid by the customers as part of the loan. The insurance policy can be done for the entire loan term or particular period.

The solution deals with the option to define the grace period, rebate on cancellation of an insurance contract and insurance rebate on pre-closure of a loan.


##### Pre-Closure and Dues Settlement

The below arrangement has a start date of 18 Apr with cooling date set as 23 Apr. As the customer opted not to proceed with the loan, the user closes the arrangement before the cooling date and the system displays the error message that the dues are not settled. Unless the dues are either settled or waived, the system does not allow the user to close the arrangement.


##### Tax on Charges

It is possible to levy a tax on charge if necessary. The below screenshot displays the Tax on Charges.


##### Pre-Closure of a Loan and Rebate Processing

An arrangement is created with Insurance Property as shown in the below screenshot.

The charge percentage is negotiable at arrangement level to add or less value based on the customer’s credibility.


> **Related Applications:** `EB.ACCRUAL`

---


### 1.19  LendingRule78


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Rule of 78 is a method used by lenders to calculate interest on a loan. It gives greater weight to months in the earlier part of a borrower’s loan cycle when calculating interest, which increases the profit for the lender.*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

The Rule of 78 is a method used by lenders to calculate interest on a loan. It gives greater weight to months in the earlier part of a borrower’s loan cycle when calculating interest, which increases the profit for the lender.

The Rule of 78 (R78) is a sum-of-the-digits method, summing up of the digits one through 12 - the number of months in a year =78 as a basis for profit accrual distribution . R78 is a method regardless of the finance tenor if it is exactly one year loan with 12 instalments. For applying Rule 78, the total interest collected from the customer is pre-calculated using the Fixed profit rate or fixed interest rate and distributes the interest over the loan life according to the R78 calculation. The interest portion charged for the prior month is much higher than the later one. By using R78, if customer does not terminate the finance before maturity, the interest amount calculated by using flat rate and Rule of 78 finance is equivalent.

Customers can pay the same amount in total. However, if customers pay off the finance early, they end up paying more than the flat rate method.

It is possible to configure and use Rule78 arrangements for both Profit bearing and upfront profit arrangements (Murabaha).

---


### 1.20  Loan Commitment


> **📇 Quick Reference Card**
> 
> **Applications:** `AA.ACCOUNT.DETAILS`, `AA.PERIODIC.ATTRIBUTE`, `AC.ALLOCATION.RULE`, `AC.ALLOCATION.RULES`, `AC.EVENT`
> 
> **Key Fields:** *Amount*, *Change Amount*, *Commitment Drawdown*, *Commitment Reversal*, *Cooling Date Adj*, *Cooling Period*, *Full Commitment Activity*, *Pre Notice Activity* ... +10 more
> 
> **Sections:** ⚙️ Configuration


#### ⚙️ Configuration

The Term Amount Property Class is used to define the commitment given to a contract.

- The Amount attribute in the Term Amount Property Class is used to define the commitment (maximum) amount of the Arrangement.
- The Term attribute in the Term Amount Property Class is used to define the commitment term of the Arrangement. The Amount attribute is currency specific, that is, the user must have one instance of each Product Condition for each currency of the product (or products) that use the Product Condition.
- The Commitment Drawdown attribute in the Term Amount Property class is used to define the disbursement method for the arrangement with options as Manual, Auto or Schedule. While the Schedule option disburses funds based on the schedule definitions in Payment Schedule property conditions, the Auto option disburses the funds through Term Amount property conditions with no dependency on Payment Schedule.

- The Change Amount attribute in the Term Amount Property Class is used to increase or decrease the commitment amount of the arrangement during the life cycle using the INCREASE or DECREASE action.
- The Change Amount attribute represents the amount to be increased or decreased on the original amount.
- To increase, the input in this attribute has to be greater than zero.
- To decrease, the input in this attribute has to be lesser than zero.

- The Change Term Activity allows the user to modify (that is, increase or decrease) the term of an arrangement, subject to the negotiation rules.

The Commitment Reversal attribute in the Term Amount condition enables the user to configure the reversal of the total commitment balance either at maturity or during the pending closure process. This attribute has the following options :

- None or On Maturity - The system reverses the total commitment balance at term maturity.
- On Closure - It reverses the total commitment balance only during pending closure process.

> **⚠️ Note:** Both the commitment amount and the term can be modified during the life cycle of the arrangement, subject to negotiation rules, periodic rules and the current outstanding amount.

When a loan is pre closed (early matured) within the Cooling Period defined for the product, its interest and charges can be waived. This cooling period can be defined as the number of calendar days in the Closure and Term Amount Property Classes. These features are mutually exclusive.

The Cooling Period attribute in the Term Amount Property Class determines the time period during which the amount can be redeemed without making due any accrued interest in the case of pre-closure of an arrangement. In the case of interest already made due, redeem Arrangement Activity during the cooling period only stops paying the accrued interest and due interest paid is not reversed back.

With respect to the pre-closure charges, the charges have to be configured as Rule Break Charges with Rule Start attribute set to Cooling-off.

In AA.PERIODIC.ATTRIBUTE , the value for the Rule Start attribute set as Cooling-off calculates the start date from which restriction has to be applied. If Cooling-off is opted, then the periodic restriction starts from the cooling date as specified in the AA.ACCOUNT.DETAILS .

The below screen shot displays the Periodic Attribute setup for charge trigger after the cooling period.

The following AC.EVENT records are used in AC.ALLOCATION.RULES .

The below screen shot displays INTEREST-ADJUST.REDEEM-PAY.

The below screen shot displays the INTEREST-ADJUST.REDEEM-PAY-CM record.

The below screen shot displays the INTEREST-ADJUST.REDEEM-PAY-PM record.

The below screen shot displays INTEREST-ADJUST.REDEEM-PAY-PY event type in the AC.ALLOCATION.RULE .

The AC.ALLOCATION.RULE set up should be as done as indicated in the above screenshots for the AC.EVENT records.

The Closure Property Class is used to define the cooling period for loan pre-closure without interest and charges. The Cooling Period field of a loan is defined as number of days (calendar) and in case it is a holiday, the Cooling Date Adj field can be used to adjust the cooling period to the next working day.

Property Class wise or Property wise choice is available for waiving or retaining the charge or interest applied during the cooling period using the Waive Class, Waive Prop and Waive Bill Type attributes. The Waive Bill Type attribute can be set to waive accrued amount, billed amount or both.

> **⚠️ Note:** For interest, only the current interest (accrued) can be waived. For charges, the waiver has to be applied on both billed and current (accrued) charges. The Cooling Period attribute in the Term Amount Property Class is mutually exclusive of the Cooling Period attribute in the Closure Property Class. If found in both the places, the system raises an error at the proofing stage.

The Loan Cancellation functionality allows a loan to be automatically cancelled if the commitment amount is not fully availed by the customer in the stipulated time period. The stipulated time is defined as the number of days under Term Amount Property Class.

The system schedules the LENDING-CANCEL-ARRANGEMENT Activity, which triggers the cancellation if the loan is not fully disbursed by that cancel period.

The banks can configure a pre-advice to be sent to the customer to indicate the cancellation that would come up due to the pending disbursement. The pre-advice configuration is achieved through the Activity Messaging Property which has associated multi-value attributes, such as Pre Notice Activity and Pre Notice Days . The Pre Notice Activity attribute has to be LENDING-CANCEL-ARRANGEMENT and Pre Notice Days attribute controls the time in advance when the notification has to be sent.

Certain type of loan products require the loan to be made available in tranches over multiple time frames, this enables the borrowers to withdraw the loan amount in a phased manner to meet the periodic requirement of cash flows.

The Full Commitment Activity attribute in the Term Amount Property Class when set to Yes triggers the LENDING-FULL.DISBURSE-ARRANGEMENT Activity when the loan is fully disbursed.


##### Overdrawn Commitment

The update to commitment balances is controlled by two attributes in the Term Amount Property Class.

- Update Utilised Commitment - indicates whether to raise utilized commitment balance or not.
- Update Commit on Capitalisation - indicates how capitalisation impacts various the commitment balances.

For Retail Loans, the setup of the two attributes below can be configured in two ways

| Scenario | Update Utilised Commitment | Update Commit On Capitalisation | System Behavior |
|---|---|---|---|
| A | No | Current | Follows existing behavior and capitalised charges are maintained in CUR balance of TERM.AMOUNT. |
| B | Yes | Overdraw | Utilisation and Capitalised amounts are maintained in new balances, UTL and OVD respectively.OVD represents the capitalised amounts while UTL represents the utilised commitment amount, excluding the capitalised amount. |


##### Scenario A

Impact of Loan Commitment Balances during Multiple Disbursements and Fee Capitalization

A loan is disbursed in multiple tranches with a linked disbursement fee that is capitalised. The impact on commitment balance is described below.

The configuration in Term Amount product condition for Scenario A is presented below.

- Update Utilised Commitment - No
- Update Commit on Capitalisation - Current

| Step | Nature of Activity (or) Transaction | Transaction Amount (USD) | TOT (Total Commitment) (USD) | CUR (Unutilised Commitment) (USD) | CUR Account (Current Account Principal) (USD) | Due Outstanding (Due Account) (USD) |
|---|---|---|---|---|---|---|
| 1 | New Loan | 1,000,000 | 1,000,000 | 1,000,000 | - | - |
| 2 | Disbursement | 1,000,000 | 1,000,000 | - | 1,000,000 | - |
| 3 | Due | 200,000 | 1,000,000 | - | 800,000 | 200,000 |
| 4 | Repayment | 200,000 | 1,000,000 | 200,000 | 800,000 | - |
| 5 | Disbursement | 100,000 | 1,000,000 | 100,000 | 900,000 | - |
| 6 | Capitalisation | 500,000 | 1,000,000 | - | 1,400,000 | - |
| 7 | Repayment | 300,000 | 1,000,000 | 300,000 | 1,100,000 | - |
| 8 | Repayment | 300,000 | 1,000,000 | 600,000 | 800,000 | - |

| Step | Nature of Activity (or) Transaction | Transaction Amount (USD) | TOT (Total Commitment) (USD) | CUR (Unutilised Commitment) (USD) | CUR Account (Current Account Principal) (USD) |
|---|---|---|---|---|---|
| 1 | New Loan | 100,000 | 100,000 | 100,000 | - |
| 2 | Disbursement | 60,000 | 100,000 | 40,000 | 60,000 |
| 3 | Capitalisation | 2,000 | 100,000 | 38,000 | 62,000 |
| 4 | Disbursement | 38,000 | 100,000 | - | 100,000 |
| 5 | Capitalisation | 2,000 | 100,000 | - | 102,000 |
| 6 | Repayment | 10,000 | 100,000 | - | 92,000 |


##### Scenario B

In certain Lending businesses, especially in Consumer Lending scenarios, when the loan disbursement happens in multiple stages, requirement is that commitment is not to be affected when the fees are capitalised during disbursement and is handled separately without affecting the available commitment for future disbursement . This allows the bank to fully disburse the sanctioned loan amount to the customer.

A loan of USD 100 is sanctioned with two disbursements (USD 70 and USD 30). A disbursement fee of USD 5 is capitalised each time a disbursement happens. Assume there are no other interest, fees or charges.

When 70 USD is disbursed, a fee of USD 5 is capitalised on the loan and the commitment reduces from 100 USD to USD 25 . This means, only 25 USD is available for subsequent disbursement against a required amount of 30 USD.

Similar to the above scenario, when a loan is Revolving, say a loan of 100 USD is fully disbursed and subsequently an activity charge is capitalised for 5 USD. At this point the principal outstanding is 105 USD and when a repayment is triggered for say 5 USD towards the fee portion, the available commitment gets reinstated by 5 USD. This means that against a 100 USD loan, 105 could be drawn since commitment was reinstated for the repaid amount towards the capitalised fees.

For loans in which the bank wants to overcome the above behaviour, the Term Amount product condition is configured with Update Utilised Commitment field set as Yes and Update Commit on Capitalisation set as Overdraw.

> **⚠️ Note:** When the Update Utilised Commitment field is set as Yes, the Update Commit on Capitalisation field must be set to either Overdraw or Current And Overdraw. These are the only combinations allowed at this point of time for the Lending product line when the Update Utilised Commitment field is set as Yes. For other combinations the system raises a validation or proofing error.

The UTL and OVD commitment balance types are used for the above configuration.

Impact of Loan Commitment Balances during Multiple Disbursements and Fee Capitalization

A loan is disbursed in multiple tranches with a linked disbursement fee that is capitalised. Impact on commitment balance is described below.

The configuration in Term Amount product condition for Scenario B is presented below.

- Update Utilised Commitment - Yes
- Update Commit on Capitalisation - Overdraw

|  |  |  | Total Commitment | Unutilised Commitment | Utilised Commitment | Overdraw Commitment | Current Outstanding | Due Outstanding |
|---|---|---|---|---|---|---|---|---|
|  | Activity | Txn Amount (USD) | TOT (USD) | CUR (USD) | UTL (USD) | OVD (USD) | CUR (USD) | DUE (USD) |
| 1 | New Loan | 1,000,000 | 1,000,000 | 1,000,000 | - | - | - | - |
| 2 | Disbursement | 1,000,000 | 1,000,000 | - | 1,000,000 | - | 1,000,000 | - |
| 3 | Due | 200,000 | 1,000,000 | - | 1,000,000 | - | 800,000 | 200,000 |
| 4 | Repayment | 200,000 | 1,000,000 | 200,000 | 800,000 | - | 800,000 | - |
| 5 | Disbursement | 100,000 | 1,000,000 | 100,000 | 900,000 | - | 900,000 | - |
| 6 | Capitalisation | 500,000 | 1,000,000 | 100,000 | 900,000 | 500,000 | 1,400,000 | - |
| 7 | Repayment | 300,000 | 1,000,000 | 100,000 | 900,000 | 200,000 | 1,100,000 | - |
| 8 | Repayment | 300,000 | 1,000,000 | 100,000 | 800,000 | - | 800,000 | - |

|  |  |  | Total Commitment | Unutilised Commitment | Utilised Commitment | Overdraw Commitment | Current Outstanding | Due Outstanding |
|---|---|---|---|---|---|---|---|---|
|  | Activity | Txn Amount (USD) | TOT (USD) | CUR (USD) | UTL (USD) | OVD (USD) | CUR (USD) | DUE |
| 1 | New Loan | 100,000 | 100,000 | 100,000 | - | - | - | - |
| 2 | Disbursement | 60,000 | 100,000 | 40,000 | 60,000 | - | 60,000 | - |
| 3 | Capitalisation | 2,000 | 100,000 | 40,000 | 60,000 | 2,000 | 62,000 | - |
| 4 | Disbursement | 40,000 | 100,000 | - | 100,000 | 2,000 | 102,000 | - |
| 5 | Capitalisation | 2,000 | 100,000 | - | 100,000 | 4,000 | 104,000 | - |
| 6 | Repayment | 10,000 | 100,000 | - | 94,000 | - | 94,000 | - |

> **⚠️ Note:** For Scenario B, the Overdrawn Commitment functionality for a loan which has Revolving field set to 'Prepayment' is currently not available.

A validation is introduced to restrict the below configuration.

- Update Utilised Commitment - Yes
- Update Commit on Capitalisation - Overdraw
- Revolving - Prepayment


> **Related Applications:** `AA.ACCOUNT.DETAILS`, `AA.PERIODIC.ATTRIBUTE`, `AC.ALLOCATION.RULE`, `AC.ALLOCATION.RULES`, `AC.EVENT`

---


### 1.21  Migration of LendingArrangements


> **📇 Quick Reference Card**
> 
> **Applications:** `AA.ACTIVITY.CLASS`, `AA.ARRANGEMENT.ACTIVITY`, `AA.CONTEXT TYPE`, `ACCOUNT`, `CUSTOMER`, `EB.CASHFLOW`, `LIMIT`, `PERIODIC.RATE`
> 
> **Key Fields:** *AMC*, *Activity*, *Arrangement*, *Context Name*, *Context Value*, *Context name*, *Currency*, *Customer* ... +25 more
> 
> **Sections:** 🔧 Working With


#### 🔧 Working With

This section deals with the migration of lending arrangements.


##### General Approach

The following general approach is recommended:

- Analyse existing products and create equivalent products using the AL module.
- Determine requirements for historic data in Temenos' system.
- Prepare extract of legacy loan contract data and balances.
- Create new arrangements from the legacy loan contract data.
- Create the outstanding legacy bills.
- Update the penalty balances.

To takeover legacy loans to AL, the following activities must already have taken place before creating the arrangements:

Each loan arrangement has to be linked to a customer in the CUSTOMER application. Every loan has to be captured in the Temenos' Lending module to ensure that the associated client data is made available in our system and the legacy loan data can be associated with the customer number in the Temenos' system.

For each customer in a loan arrangement, a corresponding LIMIT record is created in our system before creating the arrangement.

A loan can be a long-term contract in the legacy system, which can be ongoing for several years. The usual practice for the takeover of financial contracts is for the contract to be takeover to take place with an effective date that is equal to a scheduled date (for example, interest or principal due date).

The contract is created with principal balance and interest rates at the selected event date as a new contract. Interest rate and principal changes after the event date are loaded into our system as future-dated activities. Details of previous history and balances are not used in the contract processing in our system.

The date chosen can be the last payment date, which can be a past date.

> **⚠️ Note:** It is possible to takeover a contract in the middle of an interest period, but this adds additional complexity to the process. Interest calculations are split in the two systems with associated profit and loss being accrued partly in the legacy system and Temenos' system.

Existing contracts are analysed to identify the earliest date that can be used to create an arrangement.

The existing products in the legacy system has to be analysed and products have to be created for the Lending Product Line that provides the same functionality.

The legacy system is unlikely to provide functionality in exactly the same way as Temenos' system and data may not map directly from the legacy system to our system.

Properties, Product Property Conditions and Products have to be created with an effective date that is on or earlier than the earliest contract date for takeover identified in the legacy data.

Products have to be published, including any known future conditions and made available for sale before arrangements can be created.

It is unlikely that the legacy system has the concepts of product inheritance and negotiable attributes as our system so the legacy products are likely to be supported best by:

- Not using any inheritance in the product structure.
- Making the majority of attributes negotiable for arrangements.

The AA module supports the ability to record arrangement level conditions for information purposes only. Once the arrangement is created, it is possible to load historic conditions if required. Any data loaded prior to the creation date in our system are not used for processing and is not a mandatory requirement.

Temenos' system cannot process the adjustment to loan contracts with an effective date prior to the takeover date. The usual approach is to make the amendment in the legacy system if still available, or manually calculate the adjustment. The adjustment can then be applied to the arrangement in our system effective the takeover date.

The value of outstanding bills have to be taken over into Temenos' system with an effective date equal to the start date of the arrangement in our system or the takeover date. Data has to be made available for overdue bills.

The value of penalty interest and charges calculated (accrued) by the legacy system has to be made available at the takeover date (that is, effective date of arrangement creation in our system). It provides the ability to take these balances over.

The following data should be made available (or be able to be derived) in Temenos' system:

- Customer number.
- Product name.
- Effective Date for the takeover of the contract.
- Currency of Arrangement.
- Outstanding principal balance as at the Effective Date.

> **⚠️ Note:** A possible scenario is that a contract that has passed its maturity date in the legacy system but has outstanding bills and has a current principal of zero at the effective date of takeover.

A separate extract of overdue bills for existing arrangements has to be prepared. It includes,

- The bill due date.
- The breakdown of properties and outstanding amount for the bill.
- A legacy contract identifier that should be possible to link to the created arrangement number after takeover.

Any outstanding penalty interest or charge accrual balances for loans should be prepared and should identify

- The Property name (for example, PENALTYINT)
- The balance amount for the Property.

| Field | Content | Description |
|---|---|---|
| Arrangement | NEW | Requests New ID for the arrangement |
| Activity | LENDING-TAKEOVER-ARRANGEMENT | Create a new arrangement for takeover |
| Effective Date | Period Start Date | The date on which the legacy contract starts in our system, usually the start of an interest period. |
| Customer | Customer | The customer number allocated to the customer of the legacy loan contract. |
| Product | Product | The name of the product created as an equivalent to the legacy product. |
| Currency | Currency | Currency of the legacy loan. |
| Orig Contract Date | Legacy Start Date | The original start date of the legacy contract for information purposes |
| Legacy War Rate | Legacy War Rate | To retrieve the data provided in Context Name and Context Value fields and update the PERIODIC.RATE . |

| Field | Content | Description |
|---|---|---|
| Arrangement | Arrangement No | Indicates the arrangement number allocated by the takeover activity. |
| Activity | LENDING-CAPTURE.BILL-BALANCE.MAINTENANCE | Indicates the activity name which creates the new bill for an existing arrangement. |
| Effective Date | Period Start Date | Indicates the date when the legacy contract starts in our system. This is usually the start of an interest period. |
| Property.1 | Balance Maintenance Property Name | Indicates the name of the Balance Maintenance Property. |
| Field Name.1.1 | Bill Date | Indicates the name of the field to be updated in the balance maintenance property. |
| Field Value.1.1 | Bill Date | Indicates the original date the bill was created in the legacy system |
| Field Name.1.2 | PAYMENT.DATE | Indicates the name of the field to update in the Balance Maintenance Property. |
| Field Value.1.2 | Due Date | Indicates the original due date of the bill in the legacy system. |
| Field Name.1.3 | OR.BILL.AMOUNT | Indicates the name of the field to update in the Balance Maintenance Property. |
| Field Value.1.3 | Original amount | Indicates the original total amount of the bill issued in the legacy system. |
| Field Name.1.4 | PROPERTY-N | Indicates the name of the field to update in the Balance Maintenance Property. |
| Field Value.1.4 | Name of property | Indicates the name of the billed Property. |
| Field Name.1.5 | OR.PROP.AMT-N | Indicates the name of the field to update in the Balance Maintenance Property. |
| Field Value.1.5 | Original property amount | Indicates the original billed amount of the Property billed. |
| Field Name.1.6 | NEW.PROP.AMT-N | Indicates the name of the field to update in the Balance Maintenance Property. |
| Field Value.1.6 | Current outstanding property amount | Indicates the current outstanding billed amount for the associated Property to be taken over. |

| Field | Content | Description |
|---|---|---|
| Arrangement | Arrangement No | Indicates the arrangement number allocated by the takeover activity |
| Activity | LENDING-CAPTURE.BALANCE-BALANCE.MAINTENANCE | Indicates the activity that creates new balance for an existing arrangement |
| Effective Date | Period Start Date | Indicates the date at which the legacy contract starts in Temenos' system, usually the start of an interest period |
| Property 1 | Balance Maintenance Property Name | Indicates the name of the Balance Maintenance Property. |
| Field Name.1.1 | ADJUST.PROP-N | Indicates the name of the field used to update in the Balance Maintenance Property. |
| Field Value.1.1 | Penalty property | Indicates the name of the Penalty Interest or Charge Property to adjust. |
| Field Name.1.2 | ADJ.BAL.TYPE-N.N | Indicates the name of the field to update in the Balance Maintenance Property. |
| Field Value.1.2 | Balance name | Indicates the name of the penalty balance for the Associated Property, for example, CURPENINT. |
| Field Name.1.3 | NEW.BAL.AMT-N.N | Indicates the name of the field used to update in the Balance Maintenance Property. |
| Field Value.1.3 | Original amount | Indicates the balance amount for the associated property to takeover. |

During migration or takeover activity the TAKEOVER.CASHFLOW-REPORTING Cashflow type activity class allows the user to specify the EIR or carry cost which is handed off to the Cashflow engine.

Read Capturing EIR/AMC during Migration in Reporting Property Class for further information.

The following section describes the methods used in triggering TAKEOVER CASH FLOW REPORTING Activity


###### Using AMC Method

1. The following screenshot is Lending Arrangement overview after Takeover is completed
2. The TAKEOVER CASHFLOW REPORTING activity is triggered .The Takeover method is “AMC” and EIR is input as 5.
3. EB.CASHFLOW is updated with the following details Event Type updated as TAKEOVER-PERFORMING for the performing loan


###### Using EIR Method

1. The following screenshot is Lending Arrangement overview after the takeover activity. This loan is in Suspend Status.
2. The TAKEOVER CASHFLOW REPORTING activity is triggered .The Takeover method is “EIR” and AMC is input as 70.
3. EB.CASHFLOW is updated with the following details AMC value is updated in the Takeover Npv field. Event Type is updated as “TAKEOVER-SUSPEND” for the suspended loan


###### Takeover Sequence

The following section describes the takeover sequence in detail.


###### Takeover process – AA Contract with Reporting PC (in IFRS standard)

This process is for existing bank with AA loans & IFRS reporting in their system but switching to FASB standards (from IFRS).

1. Update Reporting condition for the loan product.
2. Proof and Publish the product.
3. Trigger IFRS activity.
4. Update EIR or AMC as required and commit.
5. EB Cashflow gets updated.


###### Takeover process – AA Contract without Reporting PC (without IFRS standard)

This process is for existing bank with AA loans without IFRS module initially but later comply.

1. Add Reporting condition for the loan product.
2. Proof and Publish the product.
3. Trigger IFRS activity.
4. Update EIR or AMC as required and commit.
5. EB Cashflow gets updated.


###### Full Takeover from legacy (Non AA, Non IFRS case)

This process involves migration of loans from legacy system into Temenos' solution with AA & IFRS functionality.

1. Create Loan product with Reporting condition
2. Complete loan Takeover sequence to migrate the outstanding loan bills and balances.
3. Trigger IFRS activity.
4. Update EIR or AMC as required and commit.
5. EB Cashflow gets updated.


> **Related Applications:** `AA.ACTIVITY.CLASS`, `AA.ARRANGEMENT.ACTIVITY`, `AA.CONTEXT TYPE`, `ACCOUNT`, `CUSTOMER`, `EB.CASHFLOW`, `LIMIT`, `PERIODIC.RATE`

---


### 1.22  Payment Holiday


> **📇 Quick Reference Card**
> 
> **Purpose:** *Banks offer convenient repayment options for lending products in order to please the customers. To facilitate such flexibility, the system should allow banks to skip or modify (increase or decrease) some of their scheduled repayments based on certain rules defined at multiple levels (such as Product...*
> 
> **Applications:** `AA.ACCOUNT.DETAILS`, `AA.PERIODIC.ATTRIBUTE`
> 
> **Key Fields:** *Bill Type*, *Calc Type*, *Combine Bill At Parent*, *Comparison Type*, *Hol Restrict Item*, *Hol Restrict Type*, *Modify/Cancel Payment Holidays*, *New Payment Amount* ... +20 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With


#### 📖 Introduction

Banks offer convenient repayment options for lending products in order to please the customers. To facilitate such flexibility, the system should allow banks to skip or modify (increase or decrease) some of their scheduled repayments based on certain rules defined at multiple levels (such as Product or Arrangement). Payment Holiday is one of the features offered by banks that allow customers to skip payments based on some rules of the bank and within a prescribed limit, which is also controlled.


#### ⚙️ Configuration

The system can be configured to allow modifications to the scheduled payments by either skipping or modifying the payment amount. This type of flexible repayment is achieved by using the Payment Holiday Transaction Class. There are no product conditions required and each time the conditions have to be captured afresh by the user.

Flexible repayment instructions are captured using the LENDING-UPDATE-PAYMENT.HOLIDAY activity and any subsequent changes to the flexible repayment are made through the LENDING-CHANGE-PAYMENT.HOLIDAY activity.


##### Defining Payment Holiday

Using the LENDING-UPDATE-PAYMENT.HOLIDAY activity, the user can define a payment holiday based on the Payment Type or Bill Type . The user, further has to define the Number of Instalments and the New Payment Amount (if the New Payment Amount is a Reduced Payment Amount than the Original Payment Amount).

- New Payment Amount - Determines the reduced repayment amount (the field is optional, if left blank the entire payment is considered)
- Number of Instalments - Determines the installments that need to be skipped or should have a reduced repayment amount.
- Recalculation – Allows the user to define the type of recalculations on the schedule, due to the payment holiday definition. The Recalculation options are Payment, Residual, Term, Progressive Payment and Maturity Then Payment (Read Recalculation Based on Activities in Payment Schedule)

In the screenshot below, the options to recalculate during the payment holiday and defer holiday interest period are illustrated.


##### Defining Multiple Payment Holiday

When the user defines multiple holiday payments with multiple start dates, then the payment schedule projection honours all the payment holidays.

> **⚠️ Note:** There may be few payments between holiday start dates.


##### Amending Payment Holiday

Amendments to the existing holiday payments definition can be made using the LENDING-CHANGE-PAYMENT.HOLIDAY Activity.


##### Restricting Items from Payment Holiday

If some payment type or bills types have to be restricted, it can be defined in the Payment Schedule conditions using the Hol Restrict Type and Hol Restrict Item set of fields. The user has to choose the restriction on holiday processing based on either the property class, property, bill type or payment type.

Consider a scenario, if the Charge property class is selected for restriction, then flexible repayment is not allowed for any of the scheduled charges. This can be achieved by setting Hol Restrict Type as Property Class and Hol Restrict Item as CHARGE.

Read Restriction in Flexible Repayment in Payment Holiday for more information.


##### Repayment of Holiday Interest

During a payment holiday, the system continues to accrue interest as per the original configuration. The holiday interest accrued during the payment holiday period is collected in the first upcoming schedule post holiday. When the accrued interest breaches the permissible amount of the first upcoming schedule post holiday, the accrued interest is moved to the subsequent bills.

When the payment holiday is declared, the system can be configured to collect the accrued interest during the holiday period as a separate schedule by setting Repay Type as Deferred.

- When Repay Type is left blank, the accrued interest is collected in upcoming schedules as a priority but when it is set as Deferred, the holiday period’s accrued interest is billed as a separate item in the payment schedule. The system automatically moves the holiday interest accrued to a separate balance type and starts billing it in a separate payment type after the payment holiday.
- Repay Period - Specifies the number of billing cycles required to collect the accrued holiday interest. When left blank, the holiday interest is collected as schedules till maturity.
- Refer Settlement Type - Reuses the settlement instructions of another existing payment type.

Read Repayment of the Accrued Holiday Interest for more information.


###### Balance Type for Holiday Interest

It is possible to collect the interest accrued during the payment holiday as a separate schedule. Read Flexible Repayment Definition in Payment Holiday Property Class for more information.

When the system is configured to collect the payment holiday interest in a specific schedule, the system should bill the holiday interest separately. It automatically moves the interest accrued during the payment holiday to a separate balance type to achieve this separate billing. The unbilled accrual during the payment holiday is moved from ACC to HOL (that is, from Accrued Interest Balance Type to Holiday Interest Balance Type).

The holiday interest accrued during the holiday is moved to the HOL balance type using the LENDING-DEFER-PAYMENT.HOLIDAY activity.


###### Payment Type for Holiday Interest

The HOL holiday interest is billed as a separate component in the payment schedule automatically under the Payment Type that has the Calc Type as Holiday.

> **⚠️ Note:** Ensure that the Combine Bill At Parent field is set to Yes for HOLIDAY.INTEREST Payment type for combining the holiday interest and other payment types.

When a holiday is declared for more than one interest property, separate payment types are scheduled for each of the interest property. The holiday interest is scheduled in the same frequency in which the original interest is collected and the number of schedules are based on the Repay Period specified. When left blank the schedules continue till maturity. This interest can be collected from the same settlement instruction as that of Payment Type given in Refer Settlement Type .

The system schedules the Forward Recalculate Activity at the end of the holiday period to update the Payment Schedule for the holiday interest component.

The repayment of the interest accrued during the payment holiday starts immediately after payment holiday or grace period ends. The system schedules an activity for changing the payment schedule to accommodate the HOLIDAY.INTEREST payment type on the last day of the defined payment holiday. The HOLIDAY.INTEREST Payment Type is set up in such a way that the Start Date of the HOLIDAY.INTEREST Payment Type is the immediate next due date (as that of the Payment Type or Bill Type defined in the Payment Holiday) after the payment holiday.

The user can amend the details of the holiday interest payment that is automatically scheduled after the holiday interest schedule is updated in the arrangement (after the holiday period).


##### Defining Payment Holiday Limit

When the customer opts for a flexible payment, the bank may choose to place a control on the amount of flexibility used by the customer. The bank can control the repayment amount that is being skipped or reduced during a payment holiday. This control can be configured in the Payment Schedule condition at the product or arrangement levels.


###### Periodic Attribute Class

The HOLIDAY.LIMIT and the HOLIDAY.LIMIT.REVOLVING periodic attribute classes are used to define the flexible payment limit.

- HOLIDAY LIMIT - Calculates the maximum amount or maximum percentage of amount taken as payment holiday when utilising a flexible payment.
- HOLIDAY LIMIT REVOLVING - Calculates the maximum amount or percentage that can be taken as a payment holiday where the holiday limit available is reinstated during further ad hoc payments.


###### Periodic Attribute

The banks or FIIs can define periodic attributes from the Periodic Attribute Classes. The periodic attribute controls the rule and its impact on the product through fields like:

- Periodic Type - Determines the period for which the Rule should be active on the Product. The options are Life, Initial, Repeating, Rolling, Current and Assessment Period.
- Comparison Type – Evaluates rules by comparing the values captured by the user against the arrangement values with the comparison type defined here. This should be a valid record in EB.COMPARISON.TYPE .
- Rule Start Date - Determines the date from which the Rule should be made effective. The options are Arrangement, Agreement, Start, Anniversary and Cooling Off.

Other attributes are not mandatory. Read Periodic Rules for more information.

The PAYMENT.LIMIT.REVOLVING periodic attribute is configured in the Payment Schedule condition to restrict the Payment Holiday Limit to a maximum amount or maximum percentage defined by the banks or FIIs. This rule is configured to be effective on an arrangement from the Arrangement Effective date throughout the life of the arrangement.

This rule allows to reinstate the Payment Holiday Limit during any adhoc or excess payment over and above the due amount.

The FLEXIBLE.PAYMENT.LIMIT periodic attribute is configured in the Payment Schedule condition to restrict the Payment Holiday Limit to a maximum amount or maximum percentage defined by the banks or FIIs. This rule is configured to be effective on an arrangement from the Arrangement Effective date throughout the life of the arrangement.

The periodic attribute defined in the Payment Schedule condition is evaluated every time a new payment holiday is declared. These periodic attributes can also allow banks to create period-based rules (for example USD 1000 Flexible Payment Amount Limit per year) by configuring the Periodic Type (in the Periodic Attribute) and the available flexible payment limit gets checked every time a payment holiday or flexible payment is requested for the given period (the Period can be Life, Initial, Repeating, Rolling, Current and Assessment Period). For a revolving Holiday Limit, any excess repayment over and above the due amount replenishes the flexible payment limit (to the extent of the initial limit value defined).

The utilisation of the Payment Holiday Limit, is based on scheduled bill and how much the customer has paid for the Scheduled Bill. Read Payment Holiday Limit for more information. The Payment Holiday limit is evaluated whenever there is a change in Payment Schedule like a change in the repayment amount due to the change in the interest rate.

> **⚠️ Note:** As it is possible to break the limit during standard system processing and not only during a user activity (like change in payment amount due to change in interest change in term or cancelling the declared holiday and so on), it is recommended to configure the Periodic Rule to generate an override rather an error so that during system processing any changes are automatically approved. However, during a user-initiated activity an approval is required to exceed the limit.


##### Configuring Payment Holiday Limit

The Payment Holiday Limit can be any of the following:

- Fixed amount - When the Payment Holiday limit is configured as a fixed amount, the system allows the banks or FIIs to provide payment holiday to the customer upto the defined Fixed Payment Holiday Limit.
- Percentage based on a balance type

For configuring a Fixed Payment Holiday Limit, the FLEXIBLE.PAYMENT.LIMIT/PAYMENT.LIMIT.REVOLVING periodic attribute is set up as follows, in the Periodic Rule Tab of Payment Schedule Product Condition of the product.

As per the above setup, the system is configured to raise an override for Payment Holiday Limit above USD 50,000.

For configuring a Payment Holiday Limit based of a Balance Type (that is, a percentage of the Balance Type), the FLEXIBLE.PAYMENT.LIMIT/PAYMENT.LIMIT.REVOLVING periodic attribute is set up as follows in the Periodic Rule tab of Payment Schedule Product Condition of the product.

Then in the Negotiation Rule tab, the following configuration is followed to set up a Payment Holiday Limit, which is 10% of the Total Commitment (TOTCOMMITMENT) Limit.

Any Payment Holiday limit above the defined value raises an override.

It has to be noted that, the Payment Limit Revolving periodic attribute is used to reinstate the payment holiday limit balance, during the adhoc or excess payment over and above the due amount. The banks or the FIIs can configure:

- Different percentage in the Nr Value
- Different evaluation source balance in the Nr Value Source (for example, CURACCOUNT)

That is, in the Negotiable Rules tab the Value Source , Options , Type , Value , and Message controls the Payment Holiday Limit and the related message to be displayed if the limit is breached.

> **⚠️ Note:** ’Balance Name’.


##### Controlling Payment Holidays Count

Banks/FIIs can implement a control on the number of payment holidays, for a given Bill type or Payment type defined in an arrangement for a period by configuring the periodic attribute of the HOLIDAY.COUNT periodic attribute class in the Payment Schedule condition at the product or arrangement levels.


###### Defining Periodic Attribute Class

The HOLIDAY.COUNT periodic attribute class is used to define the number of payment holidays within a period.

It evaluates the number of holidays defined in an arrangement from AA.ACCOUNT.DETAILS and there by implements the restriction on the definition of payment holidays. During a rule evaluation, the system excludes any cancelled payment holiday, while ascertaining the overall payment holiday count for the period.


###### Defining Periodic Attribute

Banks/FIIs can define periodic attribute from the periodic attribute classes and these periodic attributes control the rule and its impact on the products. Read Periodic Rules for more information.

The user configures the HOLIDAY.COUNT.YEARLY periodic attribute in the Payment Schedule condition to restrict the number of payment holidays defined in a year, as required by the banks or FIIs. This rule is configured to be effective on an arrangement from the Arrangement Effective date and the rule repeats every year.


###### Configuring Holiday Count

For restricting the number of payment holidays for a particular year, HOLIDAY.COUNT.YEARLY is set up as follows in the Periodic Rule tab of Payment Schedule product condition.


##### Defining Restriction on Consecutive Payment Holidays

Parallel payment holiday (that is, if an arrangement is within a payment holiday period and the user tries to further define a payment holiday, before the current payment holiday period is completed) is restricted when the Repay Type field is set as Deferred in the Payment Holiday Transaction Class. When Repay Type is set blank, the user can define a parallel payment holiday.

However, the banks/FIIs can implement restrictions on the definition of parallel payment holiday when Repay Type is blank, through the periodic attribute of the HOLIDAY.RESTRICT periodic attribute class.


###### Defining Periodic Attribute Class

The HOLIDAY.RESTRICT periodic attribute class is used to restrict payment holidays defined in parallel to an existing payment holiday.

The HOLIDAY.RESTRICT periodic attribute class evaluates the existing defined payment holiday dates from AA.ACCOUNT.DETAILS with that of the current activity date of payment holiday definition and there by implements the restriction, if required.


###### Defining Periodic Attribute

The user configures the HOLIDAY.RESTRICT.LIFE periodic attribute in the Payment Schedule condition to restrict any parallel payment holiday, that is, if an arrangement is within a payment holiday period the system restricts defining further payment holiday, unless the existing payment holiday period is completed. This rule is configured to be effective on an arrangement from the arrangement effective date, throughout the life of the arrangement.

The periodic attribute defined in the Payment Schedule condition evaluates the current system date and existing holiday dates in AA.ACCOUNT.DETAILS when a new payment holiday is declared. These restrictions on applying the payment holiday can be configured for different periods (for example, the life of arrangement, a period from renewal of the arrangement, repeating for period and so on) by configuring the Periodic Type and Rule Start Date in the AA.PERIODIC.ATTRIBUTE .

However, configuring the Periodic Type as Initial, doesn’t impose any restriction of definition of consecutive payment holiday as defined above.


###### Configuring Holiday Restriction

For restricting the parallel payment holidays throughout the life of the arrangement, HOLIDAY.RESTRICT.LIFE is set up as follows in the Periodic Rule tab of Payment Schedule product condition.

> **⚠️ Note:** The Pr Value for the Periodic Attribute should be Null. The system restricts definition of parallel payment for payment holidays having Repay Type as Deferred, without the configuration of the Periodic Attribute in the Payment Schedule product condition.


##### Cancelling Skipped Schedules

It allows the user to cancel the skipped schedules, through the LENDING-CHANGE-PAYMENT.HOLIDAY activity. However, cancellation is only allowed, when the upcoming holidays post cancellation is consecutive and it cannot be on an ad-hoc basis.

Read Cancellation of Holidays Declared for more information.


##### Paying-off during Payment Holiday

It is possible to payoff a loan in a holiday or grace period and/or a loan carrying the unbilled holiday interest. The payoff statement is generated for the entire loan outstanding including the accrued holiday interest and due holiday amount.

The Payment Rules used for payoff should include the holiday interest component. This enables the system to include the pending HOL . Read Payment Rules for more information.


#### 🔧 Working With

This section explains about the payment holiday definitions and processing of the same under various circumstances.

Payment Holiday for scheduled payments can be declared by triggering the UPDATE-PAYMENT.HOLIDAY activity (the same can be achieved from the Arrangement Overview page through Request Payment Holidays) and by setting the relevant holiday related attributes as explained in Configuring Payment Holiday . The above said UPDATE-PAYMENT- HOLIDAY activity can be simulated and also be converted to live.

The flexible repayment achieved using a payment holiday is explained in the below workflow:

A loan is created on 1st Jan, 2020 for one year having payments due every month. Assume the customer decides to skip the schedules for the month of April, May and June. The system achieves this flexible repayment through the below flow of activities.


##### Defining Holiday

Banks or FIIs can define the payment holiday on an arrangement for Instalment Deferral or Decrease, by using the LENDING-UPDATE-PAYMENT.HOLIDAY activity or accessing the Request Payment Holiday field in the Arrangement Overview page and there by providing the Payment Type or Bill Type , Number of Installments and the New Payment Amount fields as required.

The payment holiday is defined based on the Payment Type or Bill Type , so that, all the components of the specified Bill Type or Payment Type are subjected to the Payment Holiday, unless a restriction is defined though the Payment Schedule product condition. Read Restriction in Flexible Repayment in Payment Holiday for more information.

Banks or FIIS can reduce the repayment amount for a particular period by capturing the New Payment Amount and Number of Installments .

The below screenshot displays the payment holiday that can be declared by enabling the Request Payment Holidays field in the Arrangement Overview page. Here, the user has selected to apply Payment Holiday for three installments from the schedule due on Jul 15, 2021.

The payment holiday details are captured in AA.ACCOUNT.DETAILS , whenever a payment holiday is defined as shown below for the specified example.

The details of the holiday is evident in the Payment Holiday drill down in the Arrangement Overview page.


##### Simulating Payment Holiday

The system allows simulation of a payment holiday, to understand the impact of the payment holiday on the arrangement and then execute the same (instead of directly executing the same). In the below screenshot the user selects the Request Payment Holiday option in the Arrangement Overview page, from where Apply Payment Holiday simulation for the installment of the month Aug 2021 was selected.

The payment holiday simulation results are available under the Simulation tab in the Arrangement Overview page. The details of the simulation are stored in the $SIM files that can be used for further actions. The simulation results are printable and helps the banks to take the holiday execution forward.


##### Repayment of Holiday Interest

The system continues to accrue interest even during a payment holiday. This accrued interest is automatically collected in the upcoming installment/s immediately after the regular payment resumes.

The user has an option to repay the holiday interest as an additional schedule over a specific period or until maturity. This is achieved by using the Payment Holiday attributes, Repay Type , Repay Period and Refer Settlement (Read Payment Holiday Attributes for more information)

This section describes the Payment Holiday to reduce the repayment amount and defer the interest over a period.

- Consider a payment in which the monthly instalment is 120 (70 principal and 50 interest) and the payment rule is set to service the interest first. If the payment is decreased from 120 to 70, the interest is billed fully and remaining towards the principal or any other component as defined. Thus, there is no accrued holiday interest for processing and trying to defer the holiday interest raises an error. If the instalment is decreased from 120 to 40, the interest is partially billed for 40 against accrual of 50. The system tracks the unbilled interest portion for the entire holiday period and considers the same for processing holiday interest after the payment holiday period, based on the Repay Type , Repay Period and Refer Settlement fields in Payment Holiday Transaction Class.

- Consider a payment in which the monthly instalment is 120 (70 principal and 50 interest) and the payment rule is set to service the principal first. If the instalment is decreased from 120 to 60, the interest is billed fully and remaining towards the principal or any other component as defined. Thus, there is no accrued holiday interest for processing and trying to defer the holiday interest raises an error.

> **⚠️ Note:** Whenever, a new payment amount is defined while declaring a Payment Holiday, the new amount adjusts the repayment (during the Payment Holiday) in the order of charge, interest and principal components, irrespective of the Payment Rule condition. The remaining amount of the repayment amount, that gets postponed due to the Payment Holiday, is adjusted after the payment holiday period, as per the configuration in Payment Holiday Transaction Class condition.

When a payment holiday is declared for May, June and July installment with Repay Type left blank (that is, the system first adjusts the accrued holiday interest, before the adjusting the normal interest due and principal) the system adjusts the interest accrued during the holiday period, immediately after the defined Payment Holiday.

In the above example, it can be observed that the instalments due for the months May, Jun and Jul are skipped and as per the schedule it is observed that the interest component is adjusted first, from the month of Aug 2022 (instalment date immediately after the Payment Holiday) to Feb 2023.

> **⚠️ Note:** In Constant or Fixed Equal repayment Payment type, the monthly instalment is recalculated to be a fixed amount till the maturity of the loan. In such scenarios, the instalment, immediately after the Payment Holiday, may not clear the entire accrued holiday interest. In such cases, the system apportions the entire repayment to the accrued interest, till the holiday interest is completely paid off and thus the initial few instalments might only adjust the interest component.

Consider a payment holiday for the months of Mar, Apr and May installments with Repay type set as Deferred and Repay Period left blank. The system collects the interest accrued during the payment holiday namely the Holiday Interest, scheduled equally throughout the life of the loan.

Here, it can be observed that the instalments due for the months Mar, Apr and May 2022 are skipped and as per the schedule it is observed that the holiday interest is equally collected throughout the life of the arrangement.

The interest accrued during the holiday period is USD 6095.89 (as seen in AA.ACCOUNT.DETAILS ) and the remaining number of instalment is 297 (that is, (25*12) months – 3 Months= 297 Months). Thus, the Holiday Interest is 6095.89/297 = USD 20.52 per month, till maturity.

| Schedule Months | TOTAL Repayment | Instalment | Principal | Interest | Payment Holiday Interest | Payment Holiday Accrued Interest | Payment Holiday Accrued Interest Cumulative | Outstanding |
|---|---|---|---|---|---|---|---|---|
| 12/2020 | 428.07 | 428.07 | 407.24 | 20.83 |  |  |  | 4592.76 |
| 01/2021 | 0 | 0 | 0 | 0 |  | 19.14 | 19.14 | 4592.76 |
| 02/2021 | 0 | 0 | 0 | 0 |  | 19.14 | 38.28 | 4592.76 |
| 03/2021 | 0 | 0 | 0 | 0 |  | 19.14 | 57.42 | 4592.76 |
| 04/2021 | 592.18 | 585 | 565.86 | 19.14 | 7.18 |  | 50.24 | 4026.9 |
| 05/2021 | 592.18 | 585 | 568.22 | 16.78 | 7.18 |  | 43.06 | 3458.68 |
| 06/2021 | 0 | 0 | 0 | 0 | 0 | 14.41 | 57.48 | 3458.68 |
| 07/2021 | 0 | 0 | 0 | 0 | 0 | 14.41 | 71.89 | 3458.68 |
| 08/2021 | 0 | 0 | 0 | 0 | 0 | 14.41 | 86.3 | 3458.68 |
| 09/2021 | 1191.37 | 1162.6 | 1148.19 | 14.41 | 28.77 |  | 57.53 | 2310.49 |
| 10/2021 | 1191.37 | 1162.6 | 1152.97 | 9.63 | 28.77 |  | 28.76 | 1157.52 |
| 11/2021 | 1191.10 | 1162.34 | 1157.52 | 4.82 | 28.76 |  | 0 | 0 |


##### IFRS Contract with EB Cashflow having Payment Holiday

Consider a scenario where the loan has a monthly interest accrual of 30 and bank has defined a holiday for three instalments. The holiday interest is set to be collected over the four subsequent cycles.

| Scenario | ACC | HOL | DUE Regular | DUE Holiday | Total DUE Interest |
|---|---|---|---|---|---|
| Holiday granted for 3 months at the beginning of the month |  |  |  |  |  |
| Day 1 | 1 Dr | 0 | 0 | 0 | 0 |
| Day 30 | 30 Dr | 0 | 0 | 0 | 0 |
| End of 1st month/Day 30 | 30 Dr | 0 | 0 | 0 | 0 |
| End of 2nd Month | 60 Dr | 0 | 0 | 0 | 0 |
| End of 3rd Month | 90 Dr | 0 | 0 | 0 | 0 |
| SOD of 3rd Month End | 0 | 90 Dr | 0 | 0 | 0 |
| End of Holiday |  |  |  |  |  |
| End of 4th Month | 30 Dr | 90 Dr | 0 | 0 | 0 |
| Bill raised at the SOD of 4th month | 0 | 67.5 Dr | 30 Dr | 22.5 (holiday interest is calculated based as Tot Residual Balance/ 4) | 52.5 Dr |
| Bill raised at the SOD of 5th month | 0 | 45 Dr | 30 Dr | 22.5 Dr | 52.5 Dr |
| Bill raised at the SOD of 6th month | 0 | 22.5 Dr | 30 Dr | 22.5 Dr | 52.5 Dr |
| Bill raised at the SOD of 7th month | 0 | 0 | 30 Dr | 22.5 Dr | 52.5 Dr |

The LENDING-UPDATE-PAYMENT.HOLIDAY is a cashflow type activity. Thus, when Update Holiday is triggered, in the above scenario the cashflow handoff happens as projected below.

| Timeline | Cashflow handoff (Overall Interest) |
|---|---|
| In the above illustration consider that the PH was sanctioned on Apr 1 for three instalments |  |
| 30th Mar | 0 |
| 30th Apr | 0 |
| 30th May | 0 |
| 30th June | 52.5 |
| 30th July | 52.5 |
| 30th Aug | 52.5 |
| 30th Sept | 52.5 |


##### Impact of Change Schedule in Payment Holiday

When the bank/FIIs defines the Repay Period as Deferred, the holiday interest linked to Payment Type or Bill Type gets deferred for the specified period as mentioned in the Repay Period . At the end of holiday period, the system generates a holiday interest payment type automatically for the holiday interest balances associated with the loan and schedule the holiday interest Payment Type by mirroring the schedule associated with the Interest Property in the Payment Type or Bill Type (as defined during UPDATE-PAYMENT.HOLIDAY Activity). Read Payment Type for Holiday Interest for more information.

Once the Payment Holiday is defined, any change in the schedule (frequency change, bill type change, payment type change, start/end dates), cancels or voids all the future Payment Holiday defined (cancels the existing payment holiday). That is, if an arrangement is in a Payment Holiday Period or has defined a Payment Holiday Period for a future date, the change in schedule cancels all the payment holidays from the date of change of schedule.

An override is raised by the system for modification in the schedule of loan carrying Payment Holiday or having a future date Payment Holiday. Fresh holiday instructions need to be declared, if necessary for additional bills.

> **⚠️ Note:** The change in schedule affects the Payment Holiday, irrespective of the usage of the Repay Type field, while defining the Payment Holiday.

For example, during a payment holiday, if the user tries to change the future schedule dates of the loan, then the existing payment holiday from the current date is cancelled by the system and user should request a fresh payment holiday for the recent holiday.

The same holds good when there is payment holiday scheduled in future and the payment schedule is changed prior to that scheduled payment holiday.

A mortgage arrangement of USD 300,000 for 25 years, is opened and disbursed as on Apr 15, 2021. Repayment is set as monthly, and Payment Type set as Constant.

As per the customer request, the bank/FIIs applied for a Payment Holiday, from May to Sep. Now the customer requests a change in the repayment schedule of the arrangement from monthly to bi-weekly, before the payment holiday gets exhausted. This results in raising an override stating 'Change in payment schedule will ignore payment holiday requests if available' and there by makes all the existing Payment Holiday defined as void.


##### Payment Holiday Dates

The following section describes backdated and future dated payment holidays with illustrations.


###### Back Dated Payment Holidays

When a customer is unable to repay his loan and has missed few installments, it is possible that the bank declares those missed installments as payment holidays and restructures the loan. In this scenario, the holiday start date cannot be less than the Activity effective date. For the holiday start to be backdated, the Activity has to be run backdated. This means that, the bank or FIIs can provide a Back Dated Payment Holiday, if the LENDING-UPDATE-PAYMENT.HOLIDAY activity is also back dated.

Consider a mortgage that is in NAB status due to outstanding bills.

Now the customer approaches the bank/FII requesting for a back dated payment holiday, from Feb 1, 2022 to May 1, 2022 and the same gets approved. Accordingly, bank/FIIs agrees for the same.

After the payment holiday is declared, the customer does not miss any payment and his overdue status is reassessed based on the new schedule. The loan is not in NAB status after this restructure of declaring a back value dated payment holiday.


###### Future Dated Payment Holiday

If the start date is in the future, then the base date for holiday payment calculation, is the previous payment date of the holiday start date.


##### Amending Payment Holiday

Payment holiday definition can be reversed, by reversing the actual activity. Any amendments to the existing holiday payments definition can be made by using the CHANGE-PAYMENT.HOLIDAY activity. This functionality helps the bank/FIIs to modify or cancel an already defined Payment Holiday.


##### Payment Holiday Limit

Payment Holiday Limits allow the bank/FIIs to provide flexible payment or payment holiday options to the customer, by either reducing the repayment amount or by skipping the same, upto a defined limit agreed by the bank/FIIs and the customer. The Payment Holiday limit can be defined by configuring the Payment Schedule Condition as explained in Payment Holiday Limit.

When the repayment obligation is reduced or skipped for a customer, the system compares the amount reduced from the original repayment and with that of the available payment limit defined. An error or an override can be defined, if the limit is breached as per the banks/FIIs convenience.

There can be situations, when the schedule payment amount may change due to changes in rate of interest, term or cancelling the declared holiday in the loan. In such circumstances, the system automatically updates the Payment Holiday limit based on the new payment amount and triggers an alert to the customer when the limit is breached.

Consider the following conditions:

- The maximum limit for flexible repayment is USD 30000
- Every month instalment is due for USD 10000.

Consider a contract, having a term of one year for USD 120000 as on Jan 1,2020. The customer now requests for a payment holiday of the entire installment, for the months of Apr, May and Jun. Accordingly bank sanctions the payment holiday. Thus the Payment Holiday Limit now is USD 30000 and the Utilised Payment Holiday Limit is USD 30000.

Later the customer approaches the bank requesting for cancelation of the Payment Holiday, for Jun. This is approved by the bank and thereby the Available Payment Holiday limit becomes USD 10000 and Utilised Payment Holiday Limit now is USD 20000.

Now, the bank decides to increase the interest for the said contract, after Apr. This results in increasing the payment amount from USD 10000 to USD 11000 for the month of May. Since the month of May is within the defined Payment Holiday, the Utilised Payment Holiday Limit increases to USD 21000 and the Available Payment Holiday limit becomes USD 9000.

A mortgage arrangement of USD 500,000 for 25 years, is opened and disbursed as on Jan 1, 2022. The Payment Holiday Limit for the arrangement is set at USD 50,000.

A Payment Holiday is applied on the arrangement, for the months of Feb to Jun 2022, for the Payment Type Constant, Repay type Deferred and Repay Period left blank (that is, the system collects the interest accrued during the Payment Holiday or Holiday Interest, equally throughout the life of the loan).

The bank as on Apr 19, 2022 decides to increase the margin of the interest from 0.50 to 25.00.

This in turn affects the scheduled payments from Apr 19,2022 and the same can be seen in the schedule of the arrangement. However as the arrangement is in the Payment Holiday Period (that is, from Feb to Jun 2022), the said increase in the interest, is adjusted with Payment Holiday limit. The same can be observed, by the reduction of Available Payment Holiday limit from USD 35.381.95 to USD 34.113.45 as shown below.

Consider a loan having a Payment Holiday Limit of USD 3000 and monthly installment of USD 4500. In this scenario, while placing a Payment Holiday request, the system displays an error message, as the available Payment Holiday Limit is less than the monthly instalment and thus the New Payment Amount field should be entered maximum to the extent of 3000 USD.


##### Revolving Payment Holiday Limit

A Payment Holiday Limit can be configured to reinstate to its initial defined Payment Holiday limit, due to adhoc or excess repayments, over and above the due amount. This can be configured as defined in the Payment Holiday Limit in Payment Holiday configuration. Upon creation of an arrangement, the customer can request for a repayment holiday. The system evaluates the Repayment Holiday Limit for the product and accordingly reduces or skips the repayment obligation, as per the Flexible Payment Limit available. For revolving Payment Holiday Limit, any excess payment towards the principal, results in the evaluation of the Available Payment Holiday Limit with that of the Payment Holiday Limit defined and there by restoring the Payment Holiday limit to the extend of the defined Payment Holiday Limit (This is termed as Limit Restoration). The Available Holiday Limit is updated online and the same is evident in the Arrangement Overview page. This process can be understood from the scenarios below.

Consider a one year loan, starting from Jan 1, 2021, for an amount of USD 120000. The monthly repayment is say USD 10000 and Payment Holiday Limit USD 30000.

After settling the bills of Jan, Feb and March, the customer requests for a payment holiday on Mar 20 for next two bills. As the payment holiday is given for USD 20000, the holiday limit is reduced to USD 10000. When the customer makes a repayment of USD 50000 towards the principal of the loan on Mar 25, it reinstates the Payment Holiday Limit to its initial defined Payment Holiday Limit of USD 30000.

Consider a loan account in overdue status for USD 4500. The Payment Holiday Limit for the said loan is defined as USD 5000 and the Available Payment Holiday Limit for the loan as of now, is USD 2000.

The customer now approaches the bank for an excess payment of USD 6000.

The system adjusts excess payment, against the overdue amount of USD 4500 and the remaining amount of USD 1500 is used to replenish the Available Payment Holiday Limit (maximum to the extend of the initial defined Payment Holiday Limit of USD 5000). The New Available Payment Holiday Limit is USD 3500.

Consider a loan having Payment Holiday Limit of USD 5000 and monthly installment amount of USD 4500. The customer holds an excess amount of USD 6000 in his loan account.

Now the customer requests a Payment Holiday for the coming two months, summing to an amount of USD 9000 (that is, 2*USD 4500=USD 9000). The customer expects the same to be approved (as he holds an excess amount of USD 6000 in his loan account and has a Payment Holiday limit of USD 5000), however the system raises an error, as the system while defining the Payment Holiday checks the Payment Holiday limit and the customer only has a Payment Holiday Limit of USD 5000.

> **⚠️ Note:** The system does not consider the excess amount during repayment holiday request evaluation.


##### Controlling Payment Holidays Count

Banks/FIIs can control the number payment holidays allowed in an arrangement by configuring the HOLIDAY.COUNT periodic attribute in the Payment Schedule product condition. (Read Controlling Payment Holidays Count Configuration for more information)

Consider a mortgage arrangement in Lending product line, where the number of payment holidays that can be defined in a year is restricted to five (using the HOLIDAY.COUNT.YEARLY periodic attribute). If the user defines more than the stipulated payment holidays, the system raises an override.

When the customer tries to define a payment holiday for six instalments, the system displays the following override message: Maximum negotiable value of 5 has been exceeded by 1 in field SCHEDULE.


##### Defining Restriction on Consecutive Payment Holidays

The system supports restriction of payment holiday in parallel (that is, if an arrangement is within a payment holiday, further definition of a payment holiday is restricted, unless and until the current payment holiday period has expired), through the HOLIDAY.RESTRICT.LIFE periodic attribute, configured in the Payment Schedule product condition (Read Payment Holiday Configuration for more information).

> **⚠️ Note:** The system restricts definition of parallel payment for payment holidays having Repay Type as Deferred, without the configuration of the Periodic Attribute in the Payment Schedule product condition.

Consider a mortgage arrangement in Lending product line with HOLIDAY.RESTRICT.LIFE periodic attribute configured to raise an error, while defining a parallel payment holiday. Payment Holiday is already defined for the months of February, March, April, May, June and July.

The system’s current date is April 19, 2022 and the user tries to define a payment holiday for the month of August. The system displays the following error: Multiple Holiday requests are restricted in same holiday period.


##### Paying-off during Payment Holiday

Payoff Simulation and Direct Payoff of the loan arrangement, in a holiday or grace period, as well as, the loan arrangement carrying the unbilled holiday interest, is possible. The payoff statement is generated for the entire loan outstanding including the accrued holiday interest and due holiday amount.

Consider that a user triggers a payoff on a loan which is within the payment holiday period. The principal is 1000, due interest amount is 200, accrued interest is 50 and holiday interest balance is 20 (holiday balance represents accrued holiday interest which is yet to be billed).

The loan payoff simulation generates a payoff statement reflecting the holiday interest property along with the property like principal, interest and any fees or charges.

For the above example a payoff statement is generated with the components below.

- Payoff amount = 1270
- Account = 1000
- Interest = 270 (that is, Due Interest Amount=200, Accrual Interest=50 and Holiday Interest= 20)

Payoff bill includes the holiday interest accrual as part of the overall payoff bill.

Consider a user triggers payoff on a loan after payment holiday period ends. The principal is 1000, due interest is 205 (that is, Due interest for the current bill is 200 and the due Holiday Interest is 5), accrued interest is 50 and holiday interest balance is 15 (holiday balance represents accrued holiday interest which is yet to be billed).

The loan payoff simulation generates a payoff statement reflecting the holiday interest property along with the property like principal, interest and any fees or charges.

For the above example a payoff statement will be generated with the components below.

- Payoff amount = 1270
- Account = 1000
- Interest = 270 (that is, Due Interest Amount=205, Accrued Interest=50 and Holiday Interest=15)

Payoff bill includes the due holiday interest amounts and holiday interest accrual as part of the overall payoff bill.


##### Cancelling Holidays Declared

The user has an option to cancel or shorten the holidays declared, through Modify/Cancel Payment Holidays field in the Arrangement Overview page. The system triggers LENDING-CHANGE-PAYMENT.HOLIDAY when a payment holiday is modified or cancelled.

The payment holiday can be fully cancelled or modified to cancel specific number of holidays. But this cancellation should be consecutive. Out of four schedules marked as holiday, it is possible to:

- Cancel first
- Cancel last
- Cancel first few
- Cancel last few

But it is not possible to cancel the holidays in between or in a random order.

Change in schedule after cancel of payment holiday for Jul is:

Cancellation or shortening of holidays can be done only for consecutive schedules and error is raised when the user attempts to cancel the non – consecutive holidays.


##### Payment Holiday During Migration

The system allows migrations of loans under active Payment Holiday definitions. There are possibly two scenarios to be considered during migration or upgrade of loans.

- Loan under payment holiday period at the time of migration
- Loan completed grace or holiday period repaying holiday interest at the time of migration


###### Legacy Migration

The migration sequence in case of legacy loans with payment holiday is as follows:

1. Takeover arrangement
2. Capture outstanding loan bills and balances
3. If the loan is migrated during the holiday period, capture accrued interest (Holiday Interest).
4. Capture any future holidays using ‘Update Holiday’ and recalculate options can be configured suitably.


###### Upgrading Clients

For a customer upgrade to a loan product having payment holiday functionality,

1. Cancel existing holiday instructions
2. Re-configure fresh holiday instruction with defer option.


###### Legacy Migration

The migration sequence in case of legacy loans with payment holiday are as follows.

1. Takeover Arrangement
2. Capture outstanding loan bills and balances including the Holiday Interest due and accrued
3. Update ‘Schedule’ for ‘Holiday Interest’ and specify start and end dates based on the period over which the holiday interest is billed


###### Upgrading Clients

For a customer upgrade to a loan product having Payment Holiday,

1. The accrue interest is billed fully at the end of the Holiday Period
2. The holiday Instructions are performed if needed with Holiday functionality in the New Loan Product.
3. If bank perform upgrade after the end of holiday period and before billing of accrued holiday interest and wishes to use deferred functionality, then they can reverse the earlier holiday requests and reconfigure fresh holiday instructions with defer option.

The Update Holiday activity allows Payment Holiday to be defined for a repayment scheduled on loan takeover or migration date.

Consider a scenario where the loan takeover or migration date - May 1, 2021, as per the original schedule, and last repayment date is Nov 1, 2021

The user triggers Payment Holiday on May 1, 2021 for the repayment scheduled on the same day (May 1, 2021) with recalculation option as Term. The repayment due for May 1 is considered as a holiday by the system and extends the schedule to Dec 1, 2021 (as term is recalculated).

| Timeline | Accrual | Handoff |
|---|---|---|
| Month 1 | 30 | NA |
| Migration triggered with holiday accrual booked under MIGRPHINT property. This property is set to exclude from EIR calculation. Post migration interest is booked under PHINT property. Holiday declared for month 2 & 3 and repay period set as ‘4’ cycles. |  |  |
| Month 2 (Holiday) | PHINT – 30 MIGRPHINT -30 | NA |
| Month 3 (Holiday) | PHINT – 60 MIGRPHINT -30 | NA |
| End of Holiday period. Here both pre and post migration interest portion are assumed to set as deferred and repaid over 4 billing cycles. The overall pre migrated holiday interest (MIGRPHINT) is split across 4 cycles at 30/4=7.50 The overall post migrated holiday interest (PHINT) is split across 4 cycles at 60/4 = 15 |  |  |
| Month 4 |  | PHINT – 15; MIGRPHINT – 7.50 (Exclude from EIR) |
| Month 5 |  | PHINT – 15; MIGRPHINT – 7.50 (Exclude from EIR) |
| Month 6 |  | PHINT – 15; MIGRPHINT – 7.50 (Exclude from EIR) |
| Month 7 |  | PHINT – 15; MIGRPHINT – 7.50 (Exclude from EIR) |


> **Related Applications:** `AA.ACCOUNT.DETAILS`, `AA.PERIODIC.ATTRIBUTE`

---


### 1.23  Scheduling Payments


> **📇 Quick Reference Card**
> 
> **Applications:** `AA.ARR.PAYMENT.SCHEDULE`, `AA.ARRANGEMENT.ACTIVITY`, `AA.BILL.DETAILS`, `AA.INTEREST.ACCRUALS`, `AA.PAYMENT.TYPE`, `AA.PRD.DES.PAYMENT.SCHEDULE`, `AA.PROPERTY.CLASS`, `AA.SIMULATION.CAPTURE` ... +1 more
> 
> **Key Fields:** *Actual Amount*, *Actual Amt*, *Actual Pay Date*, *Advance Payment Restriction*, *Aging Status*, *Alt Payment Method*, *Alt Payment Routine*, *Amortisation Term* ... +49 more
> 
> **Sections:** ⚙️ Configuration | 🔧 Working With


#### ⚙️ Configuration

The following section describes the configuration required for scheduling payments.


##### Scheduling Payments

The Payment Schedule Property Class is used to schedule the payments for a loan arrangement. The user can input Payment Schedule values. Payment Type is a mandatory information and can be created by users. The available Payment Types are stored in AA.PAYMENT.TYPE table, which can be accessed through the AA Product Builder. Some of the payment types supported by AA are listed below:

- Constant: This results in constant repayments, that is, the principal and interest repayment are constant. It is used for Annuity arrangements. It requires both account and interest properties to be specified in the Payment Schedule Property Class. The Charge Property can be optionally added.
- Linear: Here, the principal repayment remains fixed over the lifetime of the arrangement. Optional properties such as Interest, Charge and Tax may be included. The actual amounts calculated by these properties are added to the fixed principal amount repayment. For a bill to be generated for Linear Payment Type on the arrangement creation date, Schedule Type must be set as Online and during the arrangement creation in Payment Schedule, set the Start Date field as the arrangement start date.
- Actual: When the Type is Manual, then the allowed Calculation Type is Actual, in which case, the user has to specify an amount in the arrangement for the Payment Type. When the Type is Calculated, Actual is normally used for repayment of the calculated property classes (for example, Interest, Charge and Tax) and the amount is determined on each payment schedule date. It can also be used in conjunction with the Account Property Class, such as, Principal, when a percentage need to be specified in the Payment Schedule Property Class.
- Transaction: This makes use of the disbursement transaction amount and capped charges linked with the activity as the source to calculate the payment amount.
- Percentage: In this calculation type, the repayment is linearly distributed for the percentage defined over the period. This is allowed for both Principal and Interest properties together for blended payments and just the Account property for Principal only payments.
- Fixed Equal Repayment: Payment Type Fixed Equal defines a manual repayment amount for the loan. As the name indicates, it is a fixed repayment amount given by the user. In addition it is also possible to specify the component that has to be fully invoiced which could supersede the fixed equal repayment amount defined by the user. Please refer to scheduling payment types
- Progressive: On choosing this type, a progressive percentage should be defined in the Prog Pay Perc field . The system calculates an amount which is progressing by the rate specified in Prog Pay Perc . Exactly same as CONSTANT type when Prog Pay Perc is defined as 0. Optionally user routine could be attached for this type.
- Other: It is a user routine attached to the Calculation Routine field.
- Rule 78 Routine based calculation: The lending arrangement can have payment schedules built on Rule 78 calculation. A Routine based Payment Type can be used to achieve this. The Cal Routine in those payment types should use the AA.CALCULATE.RULE78.PRIN.AMOUNT and AA.CALCULATE.RULE78.INTEREST.AMOUNT routines to build the principal and interest schedules respectively. Read Rule78 payment setup for more information.

- Payment Method : Once the Payment Type has been specified, the user can specify whether the amount is Due (to or from the customer), Pay (for rebates and automatic scheduled disbursement) or Capitalised.Interest only bills of loans can be capitalised to the principal for Islamic finance contracts and conventional loans.
- Max Percentage: Restricts the percentage definition in Percentage attribute in Payment Schedule product conditions. The repayment percentage of original loan principal definition is restricted to maximum of percentage defined in this attribute. Amortisation Schedule always covers 100% of total granted loan amount but the calculation percentage is based on the maximum percentage defined.

Payment Schedule conditions can be pre-constructed through AA.PAYMENT.TYPE and default values can be assigned to Payment Schedule conditions during the arrangement creation using an API validation.

Read AA.PAYMENT.TYPE in Payment Schedule property class for further details.

If a specific amount needs to be collected on the final schedule date, that amount may be stated in Residual Amount field of the Payment Schedule production condition. The amount stated in this field is exclusive of any scheduled calculated amount on the final schedule and is always considered to be belonging to ACCOUNT property.

If a specific amount (residual amount) needs to be collected at the payment end date of the term, it can be achieved by either defining the residual amount or by defining an amortisation term in the Amortisation Term field.

The Payment Mode field can be set to ADVANCE for payment of advance interest. The Interest Property Class is mandatory and it is possible to input in this payment mode setup.

- Payment Freq field - indicates the frequency at which payments are made due.
- Start Date field - indicates the actual payment start date. If the start date is mentioned, then the payment frequency is applied on the start date. Else, the system defaults it from the base date. Ad-hoc payment dates can be defined by expanding the multi-value sets and defining the dates in the Start Date field. Payment and Due Frequency fields have to be null. Additionally, an End Date or Number of Payments can be specified to indicate when the payments should terminate.
- End Date field - indicates the actual payment end date.
- Either an End Date or Number of Payments can be specified to indicate when the payments should be terminated.


##### Issue Bill In Advance

Bills can be issued in advance by setting the In Adv (BILL.PRODUCED) field in the Payment Schedule product condition for all payment types.

On the bill issue date, the system considers any forward-dated changes between the issue bill and payment dates to schedule and calculate the bill amount for the current period. However, any forward-dated change between the issue bill and payment dates that is input after the bill is issued, is effective only from the next payment date.

It is not possible to modify a bill once it is issued except if the Finalise Bills field is defined in the payment schedule condition. The only approach to modify an issued bill is by using the Payment Holiday feature when the issued bill has not crossed the finalisation period.

> **⚠️ Note:** When the loan has a floating rate or a periodic rate, the corresponding Payment Schedule must have the On Activity and Recalculate set of fields, set to recalculate the payment amount. Similarly, any other forward-dated condition in interest or other components should have a corresponding forward-dated Payment Schedule for the payment amount to be recalculated. Only when the system has a corresponding payment amount recalculation setup available, it is enabled to produce the bill in advance considering the changes between issue and due dates. Read Defining the Bill Rules for more information.

Bills issued in advance are treated as current bills and can be settled in advance irrespective of the Advance Payment Restriction field defined in Payment Rules Condition.

For a Periodic Charge, bills can be issued in advance only when the Property Type is set as Defer. If the Periodic Charge is not set to defer, the system raises an override to indicate that the bills can be issued in advance only for Defer type of periodic charges.

The assessment period for the Defer type of periodic charges are from previous issue bill to current issue bill date. The system triggers LENDING-ISSUEBILL-PERIODIC.CHARGES* in accordance to the value defined in In Adv (BILL.PRODUCED) field in Payment Schedule condition.

- The bill generated on the advance date includes all the deferred charges from previous issue bill date to the current issue bill date. Periodic Charges of Defer type should include all the deferred charges only. Other features like activity-based charges with free counts are not possible in Defer type of periodic charges.
- Any charge raised after the current issue bill date is included in the next assessment period and in the next billing cycle.
- The periodic charges are be made due on the payment date and can be repaid thereafter.

During an advance payment between the issue bill date and the payment date, the payment is appropriated against periodic charges based on the Payment Rules condition. Advance repayments of loan installment is possible for all payment types excluding the payment types based on transaction amount and routines.

For a product with Periodic Charges set to Defer and with issue bill in advance, the system validates if the Periodic Charges property is found in the advance payment rule configured for the product. If it is missing, then the system raises a validation error (at proofing or arrangement level).

The order repayment should be: Periodic Charges, Charges, Interest and then the Principal.

In the example given below, the AGEINGFEE and DISBURSEMENTFEE activity charges are set to Defer Application Method .

These two charges are collected using a PCDEFER periodic charge property which is set to Defer property type . Therefore, this PCDEFER property can be set to generate bills in advance.

The periodic charge property which is set to Defer property type should have its corresponding product condition as follows:

The Payment Schedule should have bills issued in advance for the PCDEFER Property.


###### Extend Cycle

Periodic charges, interest and scheduled charges can be extended and collected beyond the loan maturity date or the loan payment end date by setting the Extend Cycle field to the corresponding property class for the payment type.

In the example given below, the EXTENDPC Payment type has Extend Cycle field set to PERIODIC.CHARGES.

The EXTENDPC payment type has the Extend Cycle field set to PERIODIC.CHARGES. Thus, the AGEINGFEE which is charged after the loan maturity or the loan payment end date can be extended and collected as a part of the PCDEFER periodic charge property as Extend Cycle is set.

The PCDEFER periodic charge is set to be made-due every month with the bill to be issued 10 days in advance.

Thus, the system can be configured for:

- Only a Periodic Charge with Defer property type
- Only a Payment Type which has Extend Cycle set
- A Periodic Charge with Defer property type and a payment type with Extend Cycle set to collect the deferred charge. The system raises an error if the loan’s maturity date has a defer type periodic charge’s due date (bill issued and made due on the maturity date) indicating Payment Type is not set as Extend Cycle . Thus it ensures that all deferred charges are made due till the loan is closed.

Read the Payment Schedule Property Class user guide for more information on other options available for setting up schedules.


##### Minimum Payment Amount

A minimum payment amount is required to be defined by some financial markets. AA supports to capture a minimum payment amount based on the bill type. This gives the flexibility for the users to group properties by bill type and assign a minimum payment amount for them.

- It is possible to setup minimum payment amount based on the bill type – Note that it is applicable only if Account Property and on Actual Payment Type.
- The Group Min Property field is a part of the Minimum Payment set of fields to capture the Minimum Invoice Component (MIC). This field is mutually exclusive with Group Min Amount .
- Bill Type wtise MIC can be defined using the Group Bill Type and Group Min Property set of fields.

In the Group Bill Type field, only Payment type records are allowed.

> **⚠️ Note:** Any bill type defined in this attribute should not be set against the system calculated payment types namely Linear, Constant and Progressive. In the Group Min Amount field, a minimum payment amount should be indicated for the bill type mentioned.

The Minimum Payment Type field is applicable only when the payment type for Account Property displays the CalculationType field set to Actual and the Type field set to Calculated.

- If the calculated payment amount for the given bill type is less than the minimum payment amount, then the bill is raised of the minimum payment amount. The difference is billed as principal (Account Property).
- This is allowed only for scheduled payments and not for Activity-based charges or break rule charges.
- Minimum payment amount calculation can be considered during payment schedule projections and during simulations.
- The following attributes indicate the minimum amount for an arrangement. Group Bill Type field - indicates the bill type for which the minimum amount has to be applied. Group Min Amount field - indicates the minimum bill amount.
- On the scheduled payment date, when a bill is raised for the bill type mentioned in the Group Bill Type field, the system evaluates the calculated payment amount against the minimum amount specified. When the calculated amount is greater than or equal to the minimum amount, then the calculated amount is billed. When the calculated amount is lesser than the minimum amount, then the minimum amount is billed. The differential amount is billed as Account (Property).
- Minimum payment amount can be applied only to Actual payment types and does not apply for Constant, Linear or Progressive payment types.

When the bills are set to combine, the system raises a consolidated bill for all payment type lines that has a scheduled bill getting due on the same date.

BT.MINIMUM.AMOUNT is considered only when the Account Property is part of the combined bill.

- If the Account Property is not available, then the calculated property amounts are billed at actuals.
- If the Account Property is available, the system checks if the sum of the calculated amount per property (including Account) is greater than or equal to the minimum amount.
- If there is a short fall, the difference amount is increased in the Account Property to match the minimum amount specified.

When the bills are not set to combine, the system raises separate bills for each payment type. When there is at least one bill for an Account Property, the system compares the calculated amount of all bills scheduled for the date sharing the same bill type to see if it is greater than or equal to the minimum amount specified.

If the condition satisfies, the system issues the bill for the calculated amount. If the condition fails, the system issues the bill for the minimum amount specified.

When the system tries to adjust the account portion of the bill to match the minimum payment amount and the adjustment amount is more than what is outstanding in the CURACCOUNT, then the system restricts the adjustment to what is available in the CURACCOUNT.

> **⚠️ Note:** Minimum payment amount is considered even when recalculating the payment schedule.


##### Fixed Equal Repayment

- Arrangement loans can generate the Fixed Equal Repayment (FEP) Schedule.
- AA.PAYMENT.TYPE - FIXED.EQUAL is used in loan arrangements to indicate an FEP schedule. This payment type displays the Calculation Type field as manual. The mandatory Property Classes are Account (Principal) and Interest.
- The user can manually input the repayment amount during arrangement creation in the Actual Amount attribute in the Payment Schedule. The schedule projection is based on this user input FEP amount. The value in the Term field is optional for this Payment Type.
- When the Term field is not captured, it is calculated based on the FEP amount given by the user.


##### Zero Payments

Regular payment can be skipped completely once or for a regular period. Remaining payments adjust the skipped installment. Zero payment can be done either by skipping the month(s) in Pay Freq field or by giving only start and end date and skipping the interim payment(s).


##### Progressive Payments

The PROGRESSIVE payment type is used to increase the repayment amount by a pre-defined frequency captured in the Pay Freq field.

- When the Pay Freq attribute is 0%, the system behaves like an Annuity contract. If it has a percentage defined for example 2%, it means, the repayment amount increases by 2% for every repayment and the entire principal is settled on the payment end date.
- The Prog Pay Perc attribute in the Payment Schedule component accepts the progressive rate at which the repayment amount can be incremented for every repayment


##### Future Dated Conditions

The user can introduce a new date at the arrangement level using the FORWARD.DATED value in the Type attribute in the AA.PROPERTY.CLASS record. Once captured with a future date, the system automatically schedules this, and during close of business, the scheduled activity is processed applying the new condition to the Arrangement.


##### Payments Linked with Disbursement

- The consumer loan business segment would require a down payment (of principal) along with each disbursement. This is calculated as percentage of the net movement on CUR balance.
- Such a payment calculation requires the following information The disbursement event, in order to configure a payment calculation whenever a disbursement event occurs. The source on which the (down) payment has to be calculated. Optionally, a configuration to generate the bill online.
- DISBURSEMENT, is a relative date option that is used to identify the disbursement event and triggers a payment calculation. This should be specified in the Start Date field.
- Payment type with Calc Type as TRANSACTION is to calculate the payment based on net movement.
- Schedule Type has to be set as ONLINE, if the bill has to be generated online along with the disbursement.

For instance, if there is a disbursement of 1000, with a charge of 200 (set to cap) that is linked, the payment amount can be defined as a % of 1200. If the % is defined as 25%, then the system calculates a payment of 300. The condition is shown below.


##### Special Payments

Special payment is the actual amount specified by the user to substitute the regular instalment amount for the specific period, either single or regular. This amount should be specified in the Actual Amt attribute.

For example, the instalment amount needs to be different (user defined) for every March and the system calculates the value in the Calc Amount field for the remaining instalments by considering the specific payment for the given instalment(s).


##### Deferred Payments

The Defer Period attribute in the Payment Schedule Property Class is used to define the duration the scheduled payment should be deferred from the original cycled date.

When a value is defined in the Defer Period attribute, then the system schedules DEFER.MAKEDUE or DEFER.CAPITALISE activities on the cycled date and moves the bills to DEFER status.

On the cycled date + Defer Period, the system schedules MAKEDUE or CAPITALISE activities where the bills are be moved out from the DEFER status to their respective status.

> **⚠️ Note:** The defer period should not be more than the payment frequency defined in the payment schedule condition. In case the defer period is more than the payment frequency, the interest cycle fails and subsequent schedule of the Defer Capitalise or Defer Make-Due activities are not cycled to the next date.


##### Calculation of Annual Percentage Rate

Read the Annual Percentage Rate section in the Reporting Property Class user guide for more information on Annual Percentage Rate (APR) calculation.


##### Installment Amount for Multiple Disbursement

The Include Future Disb (INCLUDE.PRIN.AMOUNTS) attribute in Payment Schedule specifies the option for calculating the EMI considering the future installments.

When left blank, the default behavior continues. For a loan with multiple disbursements, the installment amount is calculated on the first disbursement and on further disbursement the user has to configure the system to recalculate the Term or Payment amount using On Activity, Recalculate fields. Else, the system lets the future disbursements get adjusted to repay in the final installment on the maturity date.

When the Include Future Disb field is set to Yes, the system calculates the constant installments with interest on outstanding principal and future disbursements or payments scheduled. This facility is applicable for all payment types. This feature is also applicable for fixed profit contracts.


##### Full or Partial Capitalisation of Interest/Profit

This section describes the full or partial capitalisation of interest and profit accruals in detail.

The Alt Payment Method field in AA.PAYMENT.TYPE is set to Due And Cap, to enable full or partial capitalisation of interest accruals in a loan. The actual amount indicated in the payment schedule is only made due and any remaining interest accruals are capitalised. This option can be used both in Islamic and conventional banking and it enables capitalization of profit accrued but not due for repayment in current period.

This option is available for the annuity repayment type. Hence both Account and Interest properties should be part of the payment type definition.

This option is not available for repayment types like principal only repayments, interest only payments, progressive payments, percentage payments (step up or step down), accelerated payments, transaction payment types and fixed equal repayments. The system raises an error if Due and Cap option is chosen for any of these payment types.

When a Due and Cap payment type is used in the payment schedule, the Payment Method field should be set as Due. The system raises an error when Payment Method is set as Capitalise.

> **⚠️ Note:** The system raises an error if the Interest Property used under a Due and Cap payment type is of the Residual Accrual Property Type.

When the Alt Payment Method field in AA.PAYMENT.TYPE is set to CAP AND INV, then during Charge Capitalisation, if the account has insufficient funds to capitalise a charge the pending amount is invoiced to the customer. The system retries the invoiced charge automatically at regular intervals using the Transaction Cycler facility. This indicates that the bill amount must be capitalised for the funds (based on the settlement rules) and invoiced for the unrealised balance.

When a charge like activity charge, scheduled charge, rule break charge is set to Capitalise and payment type indicates Alt Payment Method attribute as CAP AND INV, then the pending amount for settlement after capitalisation is invoiced to the customer. The pending charge amount, which is invoiced, is moved to INV .

The Settlement condition can be set as Full, Partial or None to indicate if the account is fully debited irrespective of the balance available, partially debited for the available amount or not debited at all when full funds are not available respectively.

Read Charges Property Class for more information.

> **⚠️ Note:** CAP and INV can be used only for Interest and Charges Property Class in the schedule. Periodic Charges cannot use the CAP and INV option.


#### 🔧 Working With

The following section describes the process of scheduling payments.


##### Scheduling Payments

Bills are generated on the scheduled date (or in advance based on the Inadv field in payment schedule).

The bills generated on the payment schedule is stored in AA.BILL.DETAILS record.

In the outstanding bills enquiry of the loan, the outstanding amount is inclusive of the tax amount on accrued penalty interest only when Tax Inclusive field is set as Yes in a payment rule of the product. The details can be read through the drilldown as shown below.

The bill details include the billed components. The tax related components for the bill are listed in the drilldown next to the bill details.

An illustration of another contract where a bill is settled is shown below. The details of the principal, interest and the tax settled are seen in the AA.BILL.DETAILS .

When a bill is deferred for a specific payment type, the defer date is updated in the AA.BILL.DETAILS record based on the Defer Period in the Payment Schedule.

The property specific original amount that is the outstanding property amount is indicated in the bill. Any adjustments are also seen in the record.

The bill details displays three sets of fields:

- Bill Status field - takes the values ISSUED, DUE, AGING and SETTLED based on the life-cycle of the bill. For example, when the bill is deferred, the Bill Status has the value DEFER after being issued and before becoming DUE.
- Settle Status field - updates as UNPAID and then as REPAID when the bill is settled.
- Aging Status field - takes the values GRACE, DEL, NAB, etc., and finally SETTLED. Note that GRACE, DEL, and NAB values are given based on the overdue

When the bill is paid or made due in advance and the payment bill is generated but paid after the cooling period if any, the MAKEDUE.ADVANCE Activity is scheduled one day after the cooling period. Any interest or principal changes through the Activity affects the interest and the final interest in the Tot Due Amt field of AA.INTEREST.ACCRUALS . The difference is paid or made due immediately.

The AA.BILL.DETAILS record stores the Property wise outstanding balances and ageing status. Read the Payment Schedule Property Class user guide for more information.

The below screen shot displays the bill details that contain multiple properties, billed amount and outstanding amount.

The below screenshot displays the ageing information, bill status and settle status.

The aging references are stored along with bill references and payment indicator.


##### Pre - Notification and Finalisation of Payment

Loan customers are advised N number of days in advance of an upcoming payment. From the notification date, the customers can choose to make changes to their upcoming payment till the bill amount is finalised . Upon reaching the finalisation date, no further changes are allowed for the upcoming payment and system triggers settlement processing for claiming funds from clearing. In case of no finalisation date, then the upcoming payment amount can be modified until the day before the payment date.

This functionality is achieved through Payment Schedule Property Class through the Bill Produced and Finalise Bills attributes. The period defined in Finalise Bills should be less than Bill Produced .

Scenario: Consider the following conditions.

| Attribute | Value |
|---|---|
| Payment date for a scheduled payment | 14-May-2020 |
| Bill Produced | 10D |
| Finalise Bills | 2D |

Ten working days (10D) prior to the payment date of 14-May-2020 is 30-Apr-2020 and the bill is issued on 30th Apr 2020 and the payment amount can be modified either by way of increasing or decreasing it until 12-May-2020

> **⚠️ Note:** The finalised payments are not shown during change activity where the user can modify the holiday amount.


##### Minimum Payment Amount

The user can setup bill type wise minimum payment amount using the Group Bill Type and Group Min Amount fields.

- Create an LOC Product with 3% principal repayment, monthly Monthly minimum payment of 1000
- Create an arrangement with 3% principal repayments with monthly frequency.
- View the Payment Schedule projection when the loan is not disbursed.
- Make a disbursement of 34T as of arrangement start date.
- View the Payment Schedule projection after the disbursement is authorised.
- View in detail the 04/25 bill.
- The outstanding amount was 34,000 and the interest percentage is 3%, which is 1,020. The calculated amount is greater than the minimum payment amount of 1,000 and hence the calculated amount is billed.
- View in detail the 05/25 bill.
- Here, the calculated amount is 989. The calculated amount is less than the minimum payment amount of 1000 and hence the minimum amount is billed.

- Create a LOC Product with 3% principal repayment, monthly Actuals of interest accrued, quarterly. Interest rate is 6% Monthly minimum payment of 1500
- View the Payment Schedule projection when the loan is not disbursed.
- Make a disbursement for 20T as of arrangement start date.
- View the Payment Schedule projection after the disbursement is authorised.
- View in detail the 05/30 bill.
- View the actual bill raised for 05/30.
- View in detail the 07/30 bill.
- Here, 3% of outstanding principal is 510 (17,000 * 3%). The interest balance is 299.18. The cumulated amount is 809.18. Since this is less than the minimum payment amount of 1,500, the bill is produced for the minimum amount. The difference amount of 690.82 is added to the Account Property.

- Create a LOC Product with 3% principal repayment, payable monthly, with bill type as INSTALLMENT. Actuals of interest accrued, payable quarterly, with bill type as PAYMENT. Interest rate is 6%. Minimum payment amount for INSTALLMENT bill type and PAYMENT is 1,000 and 500, respectively.
- View the Payment Schedule projection before the loan is disbursed.
- Loan is disbursed for 30T as of arrangement start date.
- View the Payment Schedule projection after the disbursement transaction is authorised.
- View in detail the 04/25 bill.
- Here, the calculated amount is 900 (30,000 * 3%) and hence the bill is raised for the minimum amount of 1,000.
- View in detail 06/25 bills
- There are two bills, one for INTEREST and the other for ACCOUNT.
- Interest Bill: Although minimum amount of 500 was defined for interest, the billing has happened only for the actual accrued amount. This is because, there was no account Property defined for the bill type.
- Account bill: The calculated amount is less than the minimum amount of 1,000 and hence the bill is made due for a 1,000.


##### Fixed Equal Repayment

For the loan arrangements with Fixed Equal Payments(FEP), a Minimum Invoice Component (MIC) can be configured at the Product definition level or at the arrangement level. At the loan agreement stage, it is possible to indicate that though loan is of FEP type, certain mandatory component(s) (such as interest and charges) are invoiced fully.

MIC is used to define the components that are to be invoiced fully. The Account Property cannot be defined as an MIC. The Interest Property can be defined as an MIC. When the charge is part of the FEP amount, but interest alone is defined in MIC, an override is raised.

- When the FEP amount is less than the total MIC amount (sum of the Property amounts defined in MIC), the total MIC amount is billed.
- When the FEP amount is more than the total MIC amount (sum of the Property amounts defined in MIC), the FEP amount is billed. For example, Interest component is alone specified as MIC component.
- When the FEP amount is less than the accrued interest, the accrued interest is billed.
- When the FEP amount is greater than the accrued interest, the original FEP amount is billed.

If FEP is unable to cover the components in the Payment Schedule, then the order of invoicing is charge, interest and principal.

- Any charge amount that cannot be billed, is foregone if the charge is not part of MIC.
- Any interest amount that is accrued but not billed, gets carried forward to the next period.

In certain activities, recalculate options affect FEP schedules as follows:

The term is calculated based on the FEP amount. If the term cannot be calculated, then it is updated as blank resulting in the contract becoming a call contract.

> **⚠️ Note:** Every time term is recalculated, the system calculates the annuity amount, if available, is cleared.

Annuity amount is calculated. If Term is not available, it raises an error.

Residual amount is calculated using the FEP amount defined in the Actual Amount attribute and current term. If Term is not available, an error pop ups.

For a Product with Maximum Term Cap defined, when the term is recalculated based on the FEP amount captured or it breaches the cap, the system caps maturity date to the maximum term and calculates the annuity amount. The annuity amount gets updated.

Even if the term cannot be calculated, the system caps the maturity date to the maximum term and calculates the annuity amount.


##### Recalculation on Arrangements with Forward Dated Conditions

When there are forward dated conditions in a loan contract and the user triggers an activity such as prepayment or disbursement or change in the interest and so on, the system allows the recalculation of ‘Term’ or ‘Payment’ or ‘Maturity then payment’ based on the setup in the Recalculate attribute of the Payment Schedule condition.

| Column 1 | Column 2 |
|---|---|
| Loan Details |  |
| Created on | Jul 10, 2020 |
| Amount | 36,000 |
| Term | 3Y |
| Payment | Monthly |
| Interest Rate |  |
| Jul 10, 2020 to Jul 9, 2021 | 2% |
| Jul 10, 2021 to Jul 10, 2023 | 3% (variable rate) |
| Payment Amount |  |
| For the first year | 1000 |
| From the second year, until maturity | 1100 |

| Column 1 | Column 2 |
|---|---|
| Loan Details |  |
| Created on | Apr 1, 2022 |
| Term Amount |  |
| Amount | USD 100,000 |
| Maturity date | May 1, 2023 |
| Cap on the maturity date | 2 years (that is, it cannot exceed beyond April 1, 2024). |
| Payment Schedule |  |
| Payment | Monthly |
| Payment amount | USD 8149.33 |
| The disbursement, change schedule, apply rate and change interest activities are set to recalculate the “Maturity then payment” in the payment schedule condition. |  |
| Interest Rate |  |
| Apr 1, 2022 to May 1, 2023 | 10% |
| Day basis | E |


##### Zero Payment

During zero payment, either the payment frequency can be skipped of the end date mentioned in the End Date field or date in the Start Date field can be defined for skipping interim payments. In both the cases, the system calculates the amount in the Calc Amount field after considering the skipped installments (zero payments).

For an Annuity arrangement having a payment term of one year, if two regular payments are skipped in the middle of the payment period, the system calculates the payment amount for the remaining 10 payments considering the two zero payments and calculation logic equates the payment amount for the arrangement.

In the following example, payments are skipped on 6th, 7th, 9th and 11th month. However, the system projects the schedule for the arrangement by adjusting the skipped installment amounts for the rest of the payment period using its calculation logic. The below screen shot displays the AA.PRD.DES.PAYMENT.SCHEDULE record. The below screen shot displays the Enquiry schedule projection Disbursement Linked Payments When a loan product has to collect principal (down) payments along with disbursement, it can be set-up using the DISBURSEMENT relative date option and a TRANSACTION based Payment type. The consumer loan product in model bank illustrates this set-up where a downpayment of 25% is collected for each disbursement and the rest of the payments are collected on 30, 60 & 90th day. Case 1: Downpayment with Automatic Full Disbursement An arrangement is created for USD 1000 and is fully disbursed (automatically) The disbursement fee is calculated on each disbursement and is capitalised. 20% for loans upto 500 16% for loans above 500 but less than1000 8% for loans above 1000 25% of the disbursed amount plus the charge is collected as downpayment and is billed online. The net CUR account movement is 1160 25% of the movement ,that is, 290 is calculated as a payment bill and is raised along with this disbursement. Case 2: Downpayment with Partial Disbursement An arrangement created for USD 5000 The disbursement fee is calculated on each disbursement and is capitalised. 20% for loans upto 500 16% for loans above 500 but less than1000 8% for loans above 1000 25% of the disbursed amount plus the charge is collected as downpayment and is billed online. The disbursements are done manually First Disbursement for 3000 Net movement in CUR balance is 3,240 25% of the movement, that is, 810 is calculated as a payment bill and is raised along with this disbursement. Second and final disbursement for 2000 New movement in CUR balance is 2160 25% of the movement, that is, 540 is calculated as a payment bill and is raised along with the second disbursement.


##### Progressive Payments

The repayment amount in the Calc Amount field can be recalculated upon every repayment. The PROGRESSIVE.PAYMENT value in the Recalculate attribute increments the Calc Amount by the progressive percentage. The On Activity attribute in the Payment Schedule should include the LENDING-MAKEDUE-PAYMENT.SCHEDULE Activity to recalculate the PROGRESSIVE.PAYMENT.

In the example AA.ARR.PAYMENT.SCHEDULE , the Payment Freq attribute is set to 1M and the rate is 2%. This results in the amount calculated each month to increase by 2% every month.

The below ENQ AA.SCHEDULES.FULL enquiry shows the calculated amount for future payments for the above arrangement. This has been increased every month. Percentage Calculation for Principal-only Payments The total granted loan amount can be linearly distributed as Principal-only repayment for the percentage defined for the amortisation period as per the repayment frequency. When a percentage is defined in the Max Percentage attribute, the repayment percentage of original loan principal definition is restricted to maximum of percentage defined. Amortisation Schedule is 100% but the calculation percentage is restricted to the defined percentage. For example, if loan offered to customer was an Interest Subsidy loan, then it is convenient to collect the Principal-only repayments. Illustration Consider the following example. Loan Amount = USD 100,000 on 17 April 2020 Term = 1year Payments = Principal-only CALC Type = Percentage Repayment Frequency = Monthly Max Percentage = 100 Amortisation Schedule is as follows: 15% of 100,000 on the first three payments - 15,000 / 3 = 5000 20% of 100,000 on the next three - 20,000 / 3 = 6666.67 25% of 100,000 on the next three - 25,000/3 = 8333.33 40% of 100,000 on the last three - 40,000 / 3 = 13,333.33 Amortization date Total amount per period Repayment Percentage of original loan principal, % per period 17 May 2020 15000 15 17 June 2020 17 July 2020 17 Aug 2020 20000 20 17 Sep 2020 17 Oct 2020 17 Nov 2020 25000 25 17 Dec 2020 17 Jan 2021 17 Feb 2021 40000 40 17 Mar 2021 17 Apr 2021 The above amortisation conditions can be defined as follows in Payment Schedule product conditions. The payment amount calculation is always based on the outstanding balance and the remaining total percentage. Overriding the Capitalisation Amount The capitalisation process can make an account overdrawn, but such a scenario can optionally be restricted to the extent of available balance on the account. However, this functionality cannot be extended to user-defined checks, for example, a minimum amount definition that might be required for the customer for his living, like a sustenance amount. The system considers the entire available balance during capitalisation. In order to overcome this, an option is provided to validate any other user defined conditions that might be required during capitalisation. During capitalisation of bills, the system validates if the payment type is set as Cap and Inv Alt Payment Method and a user routine is attached in Alt Payment Routine . When both these conditions are satisfied, the available balance and the capitalisation amount are handed over by the core routine to the user attached API. The API further validates and decides if the bill should be capitalised or invoiced. Illustration Consider the pre-conditions listed above are met. A customer has a credit balance of Rs 5000. There is a user definition to have a balance Rs 7000 and above for his sustenance. A debit interest bill is processed for Rs 500. In the above scenario since the sustenance balance is greater than the available balance, the entire billed amount is moved to Inv.


##### Defining Future Conditions at the Arrangement Level

The Type field with FORWARD.DATED value in the AA.PROPERTY.CLASS record allows the user to introduce a new definition at the arrangement level, it will be dated. Once captured with a future date, the system automatically schedules this and during close of business the Scheduled Activity is processed by applying the new condition to the arrangement.

A Show tabs for expansion icon is provided in the tool bar of AA.ARRANGEMENT.ACTIVITY and AA.SIMULATION.CAPTURE screens. It helps the user to identify the property for which the future dated condition can be added.

Future dated condition can either be given by specifying the date of required change or by specifying relative date like ARRANGEMENT / START + 1 month.

1. Click the Show tabs for expansion icon in the tool bar. The Show tabs for expansion icon is disabled after displaying Current tab for the property to which Future Date Conditions are allowed.
2. Click Expand icon from Current tab to add Future Date Conditions. An Option for selecting Fixed Date and Relative Date pops up on the screen.
3. Select month and year for Fixed Date and Arrangement or Start date, offset by day(s), week(s), month(s) and year(s) for Relative Date.
4. Click to confirm the selection. The selected options will be displayed as the description of the Future Date Conditions tab.

> **⚠️ Note:** Multi-Tabs added to a FORWARD.DATE set AA property can be displayed. But there is no option of hiding the Future Date Conditions Tabs.


##### Additional Payments

Additional scheduled payments can be included in the PAYMENT.SCHEDULE Property. Additional payment is defined as the payment scheduled over and above the regular payments.

Additional payments can be given by adding a payment type, and it can be either ad hoc (single) or regular and the amount should be specified in the Actual Amt attribute. The system calculates the Calc Amount field taking into account the additional payment(s) specified.

It is possible to have

- Regular additional payment- An additional payment amount is specified on a recurring basis, such as annually. This amount applies over and above the regular installment amount.
- Regular special payment - An actual payment amount is specified for a regular installment. This amount replaces the regular installment amount.
- The additional amount is paid over and above the normal loan installment. When an additional amount is set in a repayment schedule, the remaining instalments are automatically calculated by the system.
- These payments can be in the middle of an Annuity schedule, or a Single Line Amortisation (SLA) schedule (equivalent to Linear payment type). When the payments are added to such a schedule, the payment amount is calculated to take into account the additional payment(s). The below screen shot displays the AA.PRD.DES.PAYMENT.SCHEDULE . The below screen shot displays additional payments every 3 months in the Payment Schedule.


##### Special Payments

Special payment is the actual amount specified by the user to substitute the regular installment amount for the specific period, either single or regular. This amount has to be specified in the Actual Amt attribute. In the example below, it is possible to schedule the Actual Amt for the specified periods, which substitutes the system Calc Amount . In this case, the system calculates the Calc Amount considering the user scheduled Actual Amt .

The below screen shot displays the AA.PRD.DES.PAYMENT.SCHEDULE record.


##### Deferred Payments

The Defer Period attribute in the Payment Schedule Property Class is used to define deferred payments. It defines how long the scheduled payment should be deferred from original cycled date.

- Date Convention - Forward
- Date Adjustment - Period
- Bill is raised on 2nd Feb with Payment Date as 2nd Feb, Actual Pay Date as 1st Feb, Financial Date as 2nd Feb and Defer Date as 8th Feb.
- Defer Date is calculated as 5 days from Actual Pay Date , which is 6th Feb. As it is holiday, the system again applies Date Convention on top of this date. Hence, the value of Defer date in this case is 8th Feb.
- For Defer Activity (processed on 2nd Feb), accounting entries are raised with Value date as Financial Date.
- The MAKEDUE or CAPITALISE Activity is processed on the Defer Date, which is 8th Feb. Here, the accounting entries are moved to nullify DEF entries and raise real statement entries.

- Date Convention - Forward
- Date Adjustment - Value
- Bill is raised on 2nd Feb with Payment Date as 2nd Feb, Actual Pay Date as 1st Feb, Financial Date as 2nd Feb and Defer Date as 8th Feb.
- Defer Date is calculated as 5 days from Actual Pay Date, which is 6th Feb. As it is holiday, it will again apply Date Convention on top of this date. Hence, Defer date in this case is 8th Feb.
- For Defer Activity (processed on 2nd Feb), accounting entries will be raised with Value date as Financial Date.
- The MAKEDUE or CAPITALISE Activity is processed on the Defer Date which is 8th Feb. Here, accounting entries will be moved to nullify DEF entries and raise real statement entries.


##### Installment Amount for Multiple Disbursement

Loans can have the calculated installment amount as a constant (same) amount based on the full principal amount and the accrued interest on the outstanding principal balance. This constant installment amount is the same amount from the first to the final installment amount as per the payment schedule. The Include Future Disb (INCLUDE.PRIN.AMOUNTS) field is set to Yes only when the installment amount is required to be constant from start date until the maturity date of the contract. Any principal disbursement or repayment scheduled in the future is taken into consideration for the calculation of installment.

Given below is an illustration of the loan that has scheduled disbursements with loan installments set for annuity repayment. Here the user has opted for installment calculations to consider future disbursements.

The schedules are built considering the future disbursements as well.

In the below illustration, the scheduled disbursement is planned, but the total outstanding is repaid before the second disbursement. Hence the second installment is a reduced amount to repay the outstanding and third installments is zero. Regular repayments start after the next disbursement is carried out.

When the flag for considering future disbursements is set, the system adjusts the installment amount automatically during loan life cycle stages. For example, change in disbursement dates, disbursement amount or disbursement percentage, interest rate revisions, maturity date change, payment holiday, change in schedules, prepayments, special payments, special schedules like interest only or principal only, tax or charge included installments, capitalisation of dues during overdue, charge-off, write-off.

During the loan takeover from legacy system, the users set this field as yes to calculate the installment amount considering the future disbursements.


##### Residual Principal in Payment Schedule

The residual amount can be set over the life of a loan contract. When set, it is included in the Principal component of the last installment and the Total Due amount is also adjusted to reflect the residual amount along with other scheduled payments.

The schedule projector includes the residual amount against the Total Due and Principal components and the payment schedule enquiry displays the details of each component.

Consider a loan contract with residual amount ($20000) setup. The effective date of the loan is 17-Apr-2019 and the maturity date is 17-Apr-2020.

The Payment Schedule projector is updated with the residual amount against the last installment and it is included in the Total Due amount as well as the Principal component of the installment.

The drill down on the installment detail shows the break-up of the Total Due amount and it includes the residual amount as a separate line item. Further, as the Principal component also includes the residual amount, the same is seen as a separate entry against the Account Property as shown below.

Read the Payment Schedule Property Class for information on the Residual Amount attribute.


##### Adjust Balance for Upfront Profit

For a finance in which upfront profit is collected, when the customer indicates his inability to repay a loan, the user can adjust the balance and recalculate the upfront profit using the LENDING-RESTRUCUTRE-BALANCE.MAINTENANCE Activity Class. The system raises the accounting entries and updates the interest files. The system recalculates the profit after the restructure. This functionality is currently limited to Account and Interest (upfront profit) Property Class alone.

| Event | Balance type | ECB amount |
|---|---|---|
| Disbursement | RECINTEREST | -$713.61 |
|  | ACCINTEREST | $713.61 |
| During Issue Bill | RECINTEREST | -$654.31 |
|  | ACCINTEREST | $654.31 |
|  | DUEINTEREST | $59.3 |
| Restructure activity - New outstanding amount is $20 instead of $59.3 | RECINTEREST | -$693.61 |
|  | ACCINTEREST | $693.61 |
|  | DUEINTEREST | $20 |


##### Partial Capitalisation of Interest Accruals

In an interest bearing arrangement with Annuity payment type, with Due and Cap setup, the actual amount indicated in the Payment Schedule is only made due and any remaining interest accruals is capitalised. This can be a partial or full capitalisation of interest accrual for that period.

For this kind of repayment patterns, The Alt Payment Method field in AA.PAYMENT.TYPE should be set as Due and Cap. In such Payment Types, in the Payment Schedule, the Payment Method should be set as Due and an Actual Amt can be specified. This Actual Amt is made due on the schedule date.

- When the Actual Amt is zero, all the accruals for that period is capitalised.
- When the Actual Amt is more than zero, that amount is made due and any remaining accruals for that period is automatically capitalised due to the principal.

Two separate bills are raised when the accruals are made due and capitalised. The Actual Amt mentioned is made due and follows the overdue cycle for non-repayments. The remaining accruals are capitalised and a capitalised bill is raised for this part.

When the system automatically calculates the instalment amount by itself, a separate set of associated multi-value fields should be defined with the same Payment Type and the Actual Amt should be left blank.


###### Illustration of a Mortgage Loan

In this illustration, there is a mortgage loan with the first two instalments as full capitalisation ( Actual Amt is 0), the next two instalments make the amount as 100 and remaining is capitalised ( Actual Amt is 100).

For this arrangement, there is a schedule built and the interest component with tax is fully capitalised for the first two schedules. The next two schedules have partial capitalisation. The amount 100, mentioned in the Payment Schedule is made due for interest accruals and the corresponding tax is also made due. The remaining accruals for the period and their respective tax component is capitalised to the principal of the arrangement.

When the Payment Type has Tax Inclusive set to No, the tax component is not included in the amount.

Separate bills are raised for the capitalised and the due component of the instalment. The capitalisation component is immediately settled and the actual amount component is made due. The actual amount component is made due for the instalment amount and If the instalment bill is not settled, this instalment bill undergoes ageing based on the overdue configuration

This arrangement also has fully capitalised interest for the first two schedules. The next two schedules have partial capitalisation. In this Payment Type, the Tax Inclusive attribute is set as Yes.

The Payment Schedule is shown below:

When the Payment Type has Tax Inclusive set to Yes, the actual amount mentioned is inclusive of tax as seen below:


##### Assigning Default Values to Payment Schedule Conditions

It is possible to pre-construct the schedule configurations and set defaults in the Payment Schedule conditions of the arrangement. Banks can offer a unique amortisation plan to customers to repay a specific different percentage of the principal-only repayment over a certain period, for the granted loan amount. This could be tedious to define it every time at the arrangement creation. The option of setting default values to Payment Schedule feature minimises the overwhelming operations maintenance overhead when a unique percentage has to be populated for arrangements without having to repeat them for every arrangement.

Consider the following example. Create an AA.PAYMENT.TYPE record called AMORT.PLAN.3 for a Personal Loan product as follows.

A new arrangement is created and the above configured AMORT.PLAN.3 is chosen for Payment Type for Schedule conditions.

The amortisation plan configured in the AA.PAYMENT.TYPE is assigned as default to the respective attributes in the Schedule conditions using an API at validate .


> **Related Applications:** `AA.ARR.PAYMENT.SCHEDULE`, `AA.ARRANGEMENT.ACTIVITY`, `AA.BILL.DETAILS`, `AA.INTEREST.ACCRUALS`, `AA.PAYMENT.TYPE`, `AA.PRD.DES.PAYMENT.SCHEDULE`, `AA.PROPERTY.CLASS`, `AA.SIMULATION.CAPTURE`, `EB.CONTRACT`

---


### 1.24  Weighted Average Rate


> **📇 Quick Reference Card**
> 
> **Purpose:** *When loans are being disbursed in multiple tranches, each having its own interest rate a Weighted Average Rate (WAR) for the arrangement has to be calculated and applied to the contract after each disbursement .*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

When loans are being disbursed in multiple tranches, each having its own interest rate a Weighted Average Rate (WAR) for the arrangement has to be calculated and applied to the contract after each disbursement .

A weighted average interest rate is an average that is adjusted to reflect the contribution of each loan to the total debt. The weighted average multiplies each loan’s disbursement interest rate by the loan balance and divides the sum by the total loan balance. Each loan’s disbursement interest rate contributes to the weighted average in proportion to the loan’s percentage of the total debt.

The Weighted Average Rate Type of Interest condition enables the calculation of the weighted average rate, which determines the actual effective rate of the arrangement.

---


### 1.25  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Transaction Recycler provides the ability to retry failed financial transactions again at regular intervals. This is a generic retry mechanism which can be consumed by any Temenos Transact application. The Transaction Recycler is available for Arrangement Architecture (AA) and Interest and Charg...*
> 
> **Applications:** `AA.PARAMETER`, `MS.PARAMETER`, `RC.CONTRACT.PRIORITY`
> 
> **Key Fields:** *Aa Product*, *Aa Product Group*, *Attribute Type*, *Attribute Value*, *Create Retry Trigger*, *Custom Priority Rank*, *Date Convention*, *Def Prev Settle* ... +33 more
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- Temenos Transact Services

The Transaction Recycler provides the ability to retry failed financial transactions again at regular intervals. This is a generic retry mechanism which can be consumed by any Temenos Transact application. The Transaction Recycler is available for Arrangement Architecture (AA) and Interest and Charged (IC) modules (R13 release and above). Read Transaction Cycler section under Settlement Property Class for more information related to Arrangement Architecture.

The Transaction Recycler service handles the retry of failed transactions. This service will run as a COB job at a specific stage during both End of Day (EOD) and online phases. This job will retry the transactions on scheduled dates until the transaction is settled or number of retry attempts allowed have been exhausted or retry end date is reached.

During each retry, the Transaction Recycler will take the amount available in the settlement account for settling the transaction amount in full or partial, based on the Transaction Recycler retry configuration. The RC can retry the settlement based on pre-defined priority order as defined by the bank. In case of an AA loan repayment, the RC.CONTRACT.PRIORITY application allows the user to define sorting priority criteria based on custom values - the bill type or the aging status of bill.

The transactions handed over to Recycler (RC), if settled outside the RC framework are not excluded from further processing by RC and is marked with a specific status.

The following chart shows the transaction recycler process:

The Transaction Recycler acts as a framework and the processing required for retrying an AA payment or IC charges is built as a plug-in. In the above flow chart, the core plug-ins are generally represented as the payment processor, and the RC processes further, when there is an AA payment or an IC payment pending. The Transaction Recycler recognises that two different types of payments should be processed and the respective payment processor invoked is parameterised. This design enables the addition of new activity types (including any client-specific local activities) to be retried while using the same Transaction Recycler framework to orchestrate the recycling.


##### Product Configuration

The following chart shows the Transaction Recycler module components:

| Core Routine Fields | Description | Routine Name |
|---|---|---|
| Pre processor | Used to define whether a message specific core routine needs to be called to pre-process a message. | RC.PREP.RC.TYPE – For example, RC.PREP.IC.CHARGE |
| Prioritise | Used to define the message-specific core routine called by the Transaction Recycler to perform transaction grouping and sorting. | RC.PRTY.RC.TYPE – For example, RC.PRTY.IC.CHARGE |
| Processor | Used to define the message-specific core routine called by the Transaction Recycler to process the Transaction Recycler transaction, or transactions if they are grouped. | RC.PROC.RC.TYPE – For example, RC.PROCE.IC.CHARGE |
| Post process | Defines the message-specific API routine called by the Transaction Recycler to perform processing after the transaction has been completed. | RC.POST.RC.TYPE – For example, RC.POST.IC.CHARGE |

The RC.PRIORITY application is a highest level prioritisation parameter that allows to setup priority of transactions at the company level by EB.SYSTEM.ID or AA.PRODUCT.GROUP . This application is used in conjunction with RC.PRODUCT.PRIORITY and RC.CONTRACT.PRIORITY to create the rules regarding which type of transaction takes priority when there is more than one outstanding transaction against a settlement account. It ranks by EB.SYSTEM.ID , by AA.PRODUCT.GROUP or by a custom RC.PRODUCT.PRIORITY record and the ID to this application can be either a master or a lead company.

In the RC.PRIORITY application, the order of priorities are defined in the descending order (for example, the first definition has the highest priority and so on).

- In the above screenshot, the system is set up to consider the transactions in the following order, if multiple retry requests are posted against the same account:First: Products defined in the RC.PRODUCT.PRIORITY application in the PRIORITY+ONE record (direct debits sent by TPH with transaction code 125).

- Second: Products defined in the RC.PRODUCT.PRIORITY application in the MORTAGES record (MORTGAGE AA Product and then MORTGAGE.CASHBACK AA Product).

- Third: Products defined in the RC.PRODUCT.PRIORITY application in the PRIORITY +TPH record (direct debits sent by TPH with transaction code 213).

- Fourth: Request posted by the PAYMENT.ORDER application, irrespective of the request type.

When using as a priority, either a System ID (an EB.SYSTEM.ID record), the system does not require a correspondent RC.PRODUCT.PRIORITY record. If the RC.PRODUCT.PRIORITY record is not defined, it will process all retry transaction requests posted by the application in a default order, considering the oldest one received by the recycler first.

> **⚠️ Note:** The system allows only one option for each priority to be entered. This can either be an EB.SYSTEM.ID, an AA.PRODUCT.GROUP or a Product Priority (custom RC.PRODUCT.PRIORITY ID ).

Def Prev Settle is a filtering rule that means if, out of a list of ‘n’ pending transactions, one of transactions could not be settled (during retry), then all subsequent pending transactions in that list will be abandoned. It could be set to either Yes or No or left blank. If selected, it is applicable for EB.SYSTEM.ID , AA.PRODUCT.GROUP or Product Priority. This field is mutually exclusive with Prev Settle field.

The Prev Settle field can be set as Yes or No. If set to Yes, during retry of ‘n’ transactions, all transactions must be settled. Even if one of the transactions fail for some reason, then none of the remaining transactions will be considered for settlement.

The RC.CONTRACT.PRIORITY application is used in conjunction with RC.PRIORITY and RC.PRODUCT.PRIORITY to create the rules regarding the type of transaction that takes priority when there is more than one outstanding transaction against a settlement account. The RC.CONTRACT.PRIORITY is used to set the ranks at transaction level for the same type of retry request. It is used to set priority by value date, transaction amount or by a custom setting, for example by bills overdue status sent to Recycler by Arrangement Architecture (AA).

For example, if there are several transactions for the same product type against the settlement account, then the transactions have to be prioritised.

- The oldest transactions are processed first.
- If there are more than one transaction due for the same date and type, then prioritise by the largest amount first.

The RC.CONTRACT.PRIORITY application allows the user to define sorting priority criteria based on custom values. For example, based on the bills’ status issued by AA in case of loans repayments. To perform this, set:

- Due Type - Sort By Priority Attribute
- Due Rule - Custom

The Priority Rank Type field in RC.CONTRACT.PRIORITY accepts the following three options:

- Aging Status - Enables prioritisation based on the aging status of bills generated for each arrangement.
- Bill Type - Enables prioritisation of bill ( RC.DETAIL ) records based on the bill type of the arrangements.
- Blank – The value is used if the prioritization is by Aging Status of the bills.

It is not possible to set the prioritization by both Aging Status /Blank and Bill Type in the same record.

The multi-valued Custom Priority Rank field must contain custom values in the order which they must be sorted. Based on the Custom Priority Rank the Custom Priority Rank field must contain valid EB.LOOKUP record values from AA.OVERDUE.STATUS or from AA.BILL.TYPE .

In the example below, the custom values represent the overdue bill’s status based on aging / bill type as they are sent by AA to Recycler, to process the retry requests.

> **⚠️ Note:** It is not possible to set the prioritization by both Aging Status / Blank and Bill Type in the same record.

The overdue status is shown in the RC.DETAIL record after the request is settled.

> **⚠️ Note:** The AA Payment Rules setup must be in sync with the setup done in the Recycler priority setup tables. For example, if the oldest bill setup is done in AA Payment Rules, the same setup must be done in the recycler.

For example, if the Payment Rules are setup to consider the oldest bill first for an AA Product, and for the same AA Product, the contract priority rule is setup to consider the largest amount first (different setup than in Payment Rules), the system works as follows:

- If two bills are issued for the same contract on the same date, the system settles the bills by date (oldest one first) ignoring the ‘By amount’ setup in the recycler.
- If two bills are issued for the same contract on different dates, the system settles the bills considering the ‘By amount’ setup in the recycler.
- If two bills are issued for different contracts on different dates, the system settles the bills considering the ‘By amount’ setup in the recycler.
- If two bills are issued for different contracts on the same date, the system settles the bills by date (oldest one first) ignoring the ‘By amount’ setup in the recycler.

The user can define product priorities based on contract custom criteria using the RC.PRODUCT.PRIORITY application. If the user wants to define such priority, the Rank Based Priority field must be defined with the RC.CONTRACT.PRIORITY custom name. If this is set, the order defined in RC.CONTRACT.PRIORITY is applied to all products setup in RC.PRODUCT.PRIORITY . For example, it is possible to define custom priority criteria based on bills overdue status and based on product type. The bills overdue status should be setup first in the RC.CONTRACT.PRIORITY application as a custom record (read the RC.CONTRACT.PRIORITY for more details).

In order to sort the retry request based on the setup in RC.CONTRACT.PRIORITY and the one in the product order defined in RC.PRODUCT.PRIORITY , Priority Execution field must be defined. The values in this field are ’Rank Then Product’ and ’Product Then Rank’.

If the value ’Rank Then Product’ is selected, if more than one retry request is posted against the same account, the system orders requests based on the rank (status) defined in RC.CONTRACT.PRIORITY first and then by the product as defined in RC.CONTRACT.PRIORITY . If the value ’Product Then Rank’ is selected, the system orders the requests by product first and then by their rank from the RC.CONTRACT.PRIORITY application.

The following screenshot shows the RC.PRODUCT.PRIORITY is created with the value ’Rank Then Product’.

The RC.CONTRACT.PRIORITY custom record ‘MORTGAGELOANS’ has the setup as shown in the below screenshot.

The RC.PRODUCT.PRIORITY record is setup to order the requests according to the rank (status) first and then according to the product order (MORTGAGE.LOANS.USD and then MORTGAGE.LOANS.1Y), if more than one request has the same rank (status).

In case the RC.PRODUCT.PRIORITY record has a custom ID and if the Priority Execution field is defined with the value ’Rank Then Product’, the Aa Product Group field will become multivalued, allowing the definition of priorities based on products which are part of different AA PRODUCT GROUPS in the same record.

The input of Aa Product Group field is mandatory in case any Aa Product are defined. The Aa Product definition is not mandatory if the Aa Product Group is entered. If only the Aa Product Group is defined, the system considers all the retry requests posted by any product type within the product group and orders them by date (the oldest one is considered first). It is not possible to define a duplicate combination of Aa Product Group and Aa Product of the same type in the same record.

The online recycler checks for the following:

- New triggers on the accounts with active retry requests.
- Retry request for which the cut off time has passed.

The RC.PARAMETER application controls the retry trigger and the Create Retry Trigger field can have one of the following options:

- Any Credit – The system creates a retry trigger ( RC.RETRY.TRIGGER table application) for any credit posted on the account.
- Credit Balance – The system creates a retry trigger only if the new credit makes the account balance positive.

In the OVERRIDE record, ACCT.UNAUTH.OD, the Susp Appln field and Fwd Acct Mode should to be configured, as shown in the example below:

| Scenario 1 Schedule Initiation on Holiday parameter is configured | Scenario 2 Schedule Initiation on Holiday parameter is not configured |
|---|---|
| Transaction Recycler retries the transaction to settle the bill. System checks the value date when the settlement account received the funds. As it is backdated, RC settles the bill with value date on Saturday. Penalty interest accrued for Saturday and Sunday is reversed, and only one day of penalty interest is applied to the contract. Bill is settled & Contract status = Current, as of Saturday. | Transaction Recycler retries the transaction to settle the bill. System checks the value date when the settlement account received the funds. As it is backdated, RC settles the bill with the value date on Saturday. Age Overdue activity is reversed and not replayed. Total amount for which the customer is charged = Instalment amount + One day’s penalty. Due to the reversal of the ageing activities, the penalty interest is posted to UNC/remainder activity. |


##### Business Events

When the Emit Business Event field in MS.PARAMETER is set as ‘Yes’, the business events representing the state change are emitted.

The following business events are emitted for Transaction Recycler.

| Business Event | Description |
|---|---|
| settlementService.transactionRetry.currentRetry | Event to be emitted when the transaction retry is moved to current status |
| settlementService.transactionRetry.fundRecovered | Event to be emitted for a transaction retry when the funds are recovered successfully |
| settlementService.transactionRetry.fundReserved | Event to be emitted for a transaction retry when the funds are reserved successfully |
| settlementService.transactionRetry.manuallyApproved | Event to be emitted when a transaction is manually approved |
| settlementService.transactionRetry.retryCancelled | Event to be emitted when the transaction retry is cancelled |
| settlementService.transactionRetry.retryCompleted | Event to be emitted when the transaction retry is completed |
| settlementService.transactionRetry.retryCreated | Event to be emitted when the transaction retry is created |


> **Related Applications:** `AA.PARAMETER`, `MS.PARAMETER`, `RC.CONTRACT.PRIORITY`

---


---


## Chapter 2: Islamic_Banking - IS


Islamic_Banking - IS module of Temenos Transact


### Features in Islamic_Banking - IS


| # | Feature | Sections |
|---|---------|----------|
| 2.1 | Account Statements | Intro |
| 2.2 | ProductBuilder | Intro |
| 2.3 | Charges and Commissions | Worki |
| 2.4 | Hybrid Pooling | Worki |
| 2.5 | Upfront Profit in Club Finance | Worki |
| 2.6 | Asset Capture | Intro, Confi, Tasks, Outpu |
| 2.7 | Asset Review | Intro, Confi, Tasks, Outpu |
| 2.8 | Commodity Delivery and Sale | Intro, Confi, Tasks, Outpu |
| 2.9 | CreatingFacility for IslamicFinanceProducts | Intro, Confi, Worki, Tasks, Outpu |
| 2.10 | Finance Profit Accrual Product | Intro, Confi, Tasks, Outpu |
| 2.11 | Finance Profit Upfront Sale Product Group | Intro, Confi, Tasks, Outpu |
| 2.12 | Islamic Contract | Intro, Confi, Tasks, Outpu |
| 2.13 | IslamicSyndicateFinance | Intro, Confi, Worki, Tasks, Outpu |
| 2.14 | Misc | Intro |
| 2.15 | Payment Management | Intro, Confi, Tasks, Outpu |
| 2.16 | PaymentManagementUsingPO | Intro, Confi, Worki, Tasks, Outpu |
| 2.17 | ProfitDeclaration | Intro, Confi, Worki, Tasks, Outpu |
| 2.18 | Charges | Worki |
| 2.19 | SubAccounts | Confi |
| 2.20 | Limit Balance | Intro |
| 2.21 | Misc | Intro |
| 2.22 | Chargeoff | Worki |
| 2.23 | Charges | Worki |
| 2.24 | LendingRule78 | Intro |
| 2.25 | Loan Commitment | Confi |
| 2.26 | Migration of LendingArrangements | Worki |
| 2.27 | Misc | Intro |
| 2.28 | Payment Holiday | Intro, Confi, Worki |
| 2.29 | Scheduling Payments | Confi, Worki |
| 2.30 | Weighted Average Rate | Intro |
| 2.31 | Misc | Intro |


### 2.1  Account Statements


> **📇 Quick Reference Card**
> 
> **Purpose:** *Statement Property Class is used to specify the account level statement settings such as Stmt Frequency , Start Date , No Activity Indicator etc. For arrangements without Statement Property Class, the Account Statement functionality continues.*
> 
> **Key Fields:** *Frequency*, *No Activity Indicator*, *Start Date*, *Stmt*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Statement Property Class is used to specify the account level statement settings such as Stmt Frequency , Start Date , No Activity Indicator etc. For arrangements without Statement Property Class, the Account Statement functionality continues.

---


### 2.2  ProductBuilder


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Arrangement Architecture (AA) module provides a flexible framework that allows to create new Temenos Transact modules. The application provides a business component based architecture for managing products. Arrangements is part of the Retail Banking suite of products.*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

The Arrangement Architecture (AA) module provides a flexible framework that allows to create new Temenos Transact modules. The application provides a business component based architecture for managing products. Arrangements is part of the Retail Banking suite of products.

The main features of the AA module are:

- Ability to build families of products
- Ability to inherit properties from the product family structure
- Ability to determine the properties that a product is comprised of
- Control of default values to be applied for product arrangements
- Dated conditions for products
- Full control of scope of negotiation between product and arrangement conditions
- Control of negotiation of attributes over time
- Design or Proof or Publish life-cycle for product management

Read the Property Classes user guide for more details on individual classes.

---


### 2.3  Charges and Commissions


> **📇 Quick Reference Card**
> 
> **Sections:** 🔧 Working With


#### 🔧 Working With

The users can configure the charges to be due on the first, next, or last payment. The charges are triggered on occurrence of a specific activity and it is due to the customer as per the configuration.

If a user has set the charge collection on the next payment, but the system levies the charge on creation of the contract, it is still due only on the next payment date, that is, it is not due immediately. It is scheduled to be collected on the first payment date as per the schedule configuration.

Alternatively, if a user configures the collection of charge on the first payment, but the first payment date lapses when the customer triggers an activity, the system raises an override and schedules the charge along with the next upcoming payment.


##### Collecting Fee for External Event

The Record Event activity class registers an external event manually in the system. In asset financing, the financial institution can collect a delivery fee when the asset is delivered to the lessee or customer. This is an external event and not connected to the system. The user can manually register the event in the system using ASSET.FINANCE-RECORD.EVENT-ARRANGEMENT. Similarly, below activities are used for collecting charges for external events:

- Failed collection of the asset: At the end of the term, if the lessor is unable to collect the asset, the financial institution levies a charge for the failure of collection of assets. The activity can be registered in the system using ASSET.FINANCE-RECORD.FAILED.COLLECTION-ARRANGEMENT activity. A failed collection fee is levied on the arrangement when the user triggers this activity manually.
- Payment return fee: Lease payments scheduled for collection from an external system might fail due to various reasons like account unavailability or insufficient funds. System triggers ASSET.FINANCE-RECORD.DD.RETURN-ARRANGEMENT activity to register the payment failure. The user can configure a payment return fee on occurrence of this activity.

User creates an arrangement with the condition that the system collects the delivery fee when the ASSET.FINANCE-RECORD.EVENT-ARRANGEMENT activity is triggered.

Delivering the asset to the lessee is an external event. The user triggers ASSET.FINANCE-RECORD.EVENT-ARRANGEMENT in the system to register this external event. System prompts an alert message that a fee is levied for the activity.

System schedules the delivery fee to be collected along with the first payment.

---


### 2.4  Hybrid Pooling


> **📇 Quick Reference Card**
> 
> **Key Fields:** *AA Bundle ID*, *Align Dates*, *Alt Acct Id*, *Alt Acct Type*, *Alt Id Type*, *Alternate Id*, *Alternate Id Type*, *Back-to-Back FX* ... +27 more
> 
> **Sections:** 🔧 Working With


#### 🔧 Working With

The below are the different process to create a hybrid cash pool:

| Process | Activity | System/User |
|---|---|---|
| Create pool in pending live | BUNDLE-NEW.OFFER-ARRANGEMENT | Orchestration service |
| Create accounts in pending live | ACCOUNTS-NEW.OFFER-ARRANGEMENT | Orchestration service |
| Set go live date for pool | BUNDLE-UPDATE.LIVE.DATE-PRODUCT.BUNDLE | User |
| Set go live date for accounts in pool (be spoke) | BUNDLE-RESTRUCTURE-BUNDLE.HIERARCHY | User |
| Bring accounts to Live | ACCOUNTS-NEW-ARRANGEMENT | Scheduled by orchestration service and processed by COB orchestration process |
| Bring pool to live | BUNDLE-NEW-ARRANGEMENT | User/CB Orchestration process |
| Add standalone account | ACCOUNTS-TRANSFORM-ARRANGEMENT | Scheduled by orchestration service and processed by COB orchestration process |
| Remove pool account | ACCOUNTS-TRANSFORM-ARRANGEMENT | Scheduled by orchestration service and processed by COB orchestration process |
| Close pool account | ACCOUNTS-SETTLE-PAYOFF | Scheduled by orchestration service and processed by COB orchestration process |

This section describes the steps and sequences to be followed, to manually create the various account part of a BN pool structure.

The navigation is as follows,

- Product Catalog.
- Select Product Catalog from the User Menu

> **⚠️ Note:** These accounts (including the master account bundle arrangement) can be created forward dated. They are activated by the system at SOD on that date.

Create CT accounts in the desired currencies.

- Switch off settlement instructions on pay-in and pay-out sides.

Create a new bundle arrangement under the master account product.

- Attach the CTs to the product bundle.
- Identify the currency of the master account and choose the corresponding CT account to be the recipient of the bundle.

Create summary or transaction account in the order of the hierarchy.

- The parent must be created first before creating the child.
- If TR1 has its parent as CS1, which has its parent as SA1, then SA1 is created, followed by CS1 and then TR1.
- Once an account is created, its parent can only be set or changed through the purpose built internal restructuring activity.
- Normal Update-Account activity cannot be used.
- Similarly, once an account is created, the bundle arrangement (master account) and link account number (CT account) can be updated through the purpose built External Restructuring Activity.
- Switch off settlement instructions on pay-in and pay-out sides.
- Once the accounts are created, the normal workflow on updating their conditions are to be followed through the arrangement overview. The new activity drilldown links to setup, Bank interest or fees or schedule and settlement Internal interest or fees or schedule and settlement conditions.


###### Generating IBAN

When the Bundle for the master account product is created in Draft status and when it is subsequently moved to the New Offer status, the IBAN is generated based on the values defined for Generate Iban and Alt Id Type . The IBAN can be seen in the AA.ARRANGEMENT record of the underlying contract.

As displaying the entire IBAN Value on the card is not feasible, it displays few characters of IBAN and appends it with three dots , for example, GB12DEMO60161300087537 is displayed as GB12DEMO6061…; on hovering over the text it displays the full string value.

The Alternate Id Type and Alternate Id of the Alt Id Types can be viewed in the expand header of each card. For the accounts other than master, T24.IBAN value gets displayed on the card instead of Account ID. If T24.IBAN value is available, the Alt Acct Type and Alt Acct Id get displayed on the expand card header.

When creating the CT accounts except for Limit (in case of MCCFor SCCF or MCF or SCF) is updated, no other special attribute needs to be specified to attach it to a master account, since it is done through the UPDATE-PRODUCT.BUNDLE activity. The user does this activity directly on the bundle arrangement (master account).

Once the CTs and MAs are created, when creating SA or CS or TR or MTR, it is important to capture the pool and hierarchy details via the purpose built attributes in Account property.

The following is a screenshot of a TR being created new, attached to an existing Pool under SA1 as its parent. The navigation for this could either be from the Product Catalog or the Master Account Overview.

The Master account is the bundle arrangement.

- If the account added or created is in a different Temenos Transact company than the master account, then the master account reference must be captured suffixed with its company mnemonic. In the example above, since the master account is in Temenos Transact Company BNK, it must be captured as AA1710732QS1/BNK for the system to recognise it.
- Linked Account number is the CT Account. If left blank and if a valid CT in this currency exists, then the system would default it. If a value is entered, the system validates that it is a valid participant in this Bundle Arrangement and that its currency matches this account’s currency.

- Parent account is used to capture the parent in the hierarchy. It is an optional field and when left blank, it mean the account being created would be added to the pool directly under the master account level.
- If a value is entered, the system would validate that it is, A valid member of the Bundle Hierarchy An allowed parent of this account Enabled for multi-currency if its currency is different from that of this account’s currency

In case of opening CS or SA, the above rules hold true except for the Linked Account Number (for which input is allowed).

The accounts in the BN pool can be internally moved (at any point). To facilitate this, the ACCOUNTS-CHANGE.PARENT-ARRANGEMENT activity is initiated from the New Activity menu.

During this process happens, the balances from the previously linked parent account is also transferred.

The above screenshot shows a TR account linked to SA account 2000003347. The SA and linked TR account’s balances are the same.

From the New Activity menu in the TR account, the User activity ACCOUNTS-CHANGE.PARENT-ARRANGEMENT is initiated.

For a restructuring, this activity runs at COB, hence, the Effective Date needs to be day + 1. The new parent account is changed to 2000003355, which is the new SA account. After authorisation and a COB is run, the restructure process is initiated.

The above screenshot shows that the balance (USD 88,592.08) is moved from (2000003347) to (2000003355) account.

This section enables the user to understand creation of BN pool.

BN structure creation process starts from creating a master arrangement in a draft status. The user can provide the necessary details to create the master arrangement by selecting the NEW STRUCTURE tab in Graphical User Interface (GUI). Mandatory information is Product Name, Country (on which the Master arrangement is created), Currency (master account) and Structure Name (optional).

To create a new BN structure, from the GENERAL TRADING screen,

1. Click NEW STRUCTURE .
2. Enter the mandatory information and then click CREATE . The master arrangement is created in view mode.
3. Click to add new accounts to BN structure. The symbol is enabled.
4. Click to add new accounts to the BN structure. The Add Account to Structure pop-up window opens.
5. Select the respective account type to add a new accounts to the pool. Standalone accounts can be selected and added to the BN structure by filtering the accounts by Currency.
6. Click to add multiple accounts to the pool. Example: To add two SA accounts, select the currency and company from the drop-down list. Once the account placed holder is created, click OK to create the placeholder card in GUI.
7. Click Save to save the BN pool structure in GUI. GUI passes the information to Temenos Transact to store the placeholder details. The user can save the changes in GUI after the BN pool structure is approved by corporate. When the user saves the Master arrangement in GUI, Temenos Transact does not any validation.

The BN structure can be edited and updated with new accounts and removal account by selecting the edit options. The Draft BN structure can be edited with the following details.

- Adding new placeholders
- Removing placeholder accounts
- Changing Parent details
- Adding Standalone accounts
- Adding a new parent placeholder for child accounts

Click Validate and Commit . The CT placeholders are created automatically. CT account is opened in Master account company for each currency of TR accounts.

To disconnect account placeholder, Click on each cards. The account card is removed immediately from the BN pool structure. When the Summary Account (SA) or Currency Summary (CS) placeholders are removed from BN pool, the child accounts are linked to the immediate parent. The parent accounts can be removed along with the child accounts from BN pool.

> **⚠️ Note:** Account number is not generated in Temenos Transact, hence the conversion of TR account to standalone is not possible.

To add standalone accounts to BN pool, click on the respective cards.

> **⚠️ Note:** This icon is enabled only for Master or SA or CS accounts.

Standalone accounts can be added under SA and CS account or directly under the master arrangement without any parent. Until the BN pool becomes live, the standalone account terms and conditions remains the same. Once the live date reaches, the account is converted to TR and the new product conditions applies. The account number remains the same as standalone account and only the change product activity is triggered.

Export. The BN structure can be exported as PDF, HTML, Excel, Power Point and Word. The exported BN structure is produced with the corporate customer for any modifications or changes in the structure. BN structure can be exported during Draft, Preliminary and Live status.

Go Preliminary to move the pool to preliminary. To move the pool to Preliminary status, the Pool Orchestration Service is run after committing the Activity. Once the Go Preliminary is triggered on a particular BN pool, the user can click on top-left and GUI displays the GUI landing page.

Once the preliminary process completed, the status of BN pool structure is moved and updated as Preliminary. Account number is generated on each placeholder and appears on each cards. Temenos Transact generates CT account automatically for each currency of TR accounts.

Click Edit to update the Terms and Conditions.

This section enables maintenance of cover control

This option is available in Tools menu. Click Edit to update the cover control setup. Accounts part of BN pool are listed as tree view and the changes can be updated in each account. Cover control on CT accounts are not applicable and hence the options are not enabled. Enable Apply settings to sub-structure to copy the cover control setup to child accounts.

Credit check is set for internal or external transactions or both. When the options is Null, the credit is applied during the transaction processing. Click Save to update the changes in Temenos Transact.

Click Edit to add new SA,CS,TR or MTR accounts in preliminary BN structure. The similar process is followed in Draft to add new accounts in preliminary. The user can commit the changes once the placeholders are created. Once the BN pool is committed in GUI, account number is generated immediately in Temenos Transact and appears on each card. The user can update the terms and conditions for the new account created in BN Pool.

To sets the Global Go Live Date from CARD VIEW Click Go Live on top-right of the BN Pool structure in GUI.

In the below screen, the Global Go Live is set for Bundle arrangements and the custom Go Live date option is for individual accounts part of BN Pool structure. Set the Global Go Live Date first and then the customer go live date, else an error message is displayed. Custom Go Live date is an optional input, participant accounts in BN pool goes live with the same date as Master or Bundle go live. When the go live date is set for individual accounts, then the accounts are live only on that particular date. Transactions are not allowed until the accounts are moved to LIVE.

The Custom go live date can be the same as Master live date as or later than Master live date. Temenos Transact displays an error message when the customer go live date is before Master live date.

This section enables maintenance of CT Accounts

CT Account

CT accounts provides static information of accounts such as CUSTOMER NAME, CUSTOMER ID, ACCOUNT NUMBER, STATUS and SCHEDULED CHANGES. CT expand card also has an option to setup or amend the interest conditions. When the limit is available for the CT account, GUI allows editing of limit on CT accounts.

CT Account Transactions

CT Account balances

Limit Conditions

To update or amend the limit records, click Edit. Once the changes and amendments are done, click Commit to submit the changes in Temenos transact.

Interest Conditions

Click Interest conditions on CT account in expand view, the version of Interest calculations are launched. The interest activity can be set with immediate effort or for a future effective date. On committing the changes, GUI passes the information to Temeons Transact to update interest details.

Summary Account/Currency Summary

SA account provides the static information of accounts such as CUSTOMER NAME , CUSTOMER ID , ACCOUNT NUMBER , STATUS and SCHEDULE CHANGES . It provides the combined balances of all the child accounts linked under the SA accounts. It is multi-currency accounts; hence, any allowed currencies can be linked to SA. When the SA account is having a multi-currency child accounts, then the balance is combined to SA account currency. SA expand card can setup or amend interest conditions and internal cover control.

When the user clicks on Interest condition, the respective version is launched to update the internal interest conditions. Manage Limit option allows the user to setup the internal and external cover control. Manage limit version is launched and the GUI allows to update and commit the changes.

TR Account

Expanded view of TR account provides the static information of accounts such as CUSTOMER NAME , CUSTOMER ID , ACCOUNT NUMBER , STATUS and Schedule Changes. TR account provides the balances and transactions of the respective TR accounts. The user can view the transactions by providing the start and end date. TR expand card can setup or amend interest conditions and internal cover control.

When the user clicks on Interest condition, the respective version is launched to update the internal interest conditions. Manage Limit option allows the user to setup the internal and external cover control. Manage limit version is launched and the GUI allows to update and commit the changes.

TR Account Transfer Services

Setting Future Internal STO/Sweeps

On selecting the Transfer services, the process remains the same. Refer Transact process flow.

When the CT Accounts are created (except for Limit in case of MCCF or SCCF or MCF or SCF) are updated, no other special attribute is specified to attach it to a master account using the UPDATE-PRODUCT.BUNDLE activity. The user does it directly on the bundle arrangement (master account).

When the CTs and MAs are created and when creating (SA or CS or TR or MTR), the pool and hierarchy details should be captured using the purpose built attributes in Account property.

The below screenshot shows a new TR attached to an existing pool under SA1 as its parent. The navigation for this is from the Product Catalog or the Master Account Overview.

The master account is the bundle arrangement.

When the account added or created is in a Temenos Transact company different from the master account, the master account reference should be captured and suffixed with its company mnemonic. In the above screenshot, since the master account is in Temenos Transact company BNK, it must be captured as AA1710732QS1/BNK for the system to identify.

Linked Account Number is the CT account. If this field is left blank and when a valid CT in this currency exists, then the system defaults it.

- When a value is entered in this field, the system checks if it is a valid participant in the bundle arrangement and currency matches the account’s currency.

Parent Account is used to capture the parent in the hierarchy. It is an optional field and when left blank, the account created is added to the pool directly under the master account level. When a value is entered in this field, the system validates if it is,

- A valid member of the bundle hierarchy
- An allowed parent of this account
- Enabled for multi-currency (if the currency is different from that of the account’s currency)

> **⚠️ Note:** The above rules hold true when opening CS or SA, (except for the Linked Account Number for which input is not allowed).

The AA.BUNDLE.HIERARCHY.DETAILS (system maintained table) is used for any investigation or analysis purposes or to know the pool structure on a given date.

85308 is the top most summary account and the grand parent of 85332, 85348, 85359 and 85367 (all from the same company) and also a parent of 2000003266 (from a different company). This illustrates that the pool hierarchy can contain accounts across borders ( Temenos Transact companies or books).

Posting transactions on a BN pool is possible through the transaction account (that has External Posting set as Yes).

> **⚠️ Note:** The system blocks any direct posting on CS or SA or CT.

Whenever a transaction is posted in a TR account, the core accounting engine does the following:

- Makes a posting on the TR as a memo posting and diverts it as a real entry in the corresponding CT account (specified in Link AC Number field in Account Property)
- Replicates the same memo entry in the parent of the TR (specified in the Parent Account field in Account Property) and its parent and so on up to the top level parent.

Internal or external transactions are controlled by the Transaction Type attribute in TRANSACTION table. This and the internal cover control attributes in Limit property class drives the validations on these transactions for TR or CS and SA accounts.

| Account Type | Company Name | System Date |
|---|---|---|
| CT account (100001) | Temenos core banking Norway company | 25/10/2017 |
| TR account (100002) | Temenos core banking Norway Sweden | 23/10/2017 |
| TR account (100003) | Temenos Core Banking Norway Finland | 24/10/2017 |

To make a bundle go live, enter the current or future date in the Master Live Date field.

- If the current date is given, run the AA.POOL.ORCHESTRATION.SERVICE service to make the pool go live online.
- If the current date is given but service is not run, the bundle does not go live during the End of Day processes. In this case, to make the bundle go live, enter the current date, the following day (and run the service), or a future date in the Master Live Date field .
- If a future date is given, the bundle goes live during the SOD process of the given date.

When a pool structure (bundle arrangement) is created, subsequent maintenance activities either at Pool or individual account level can be carried out from the bundle arrangement overview.

Find Bundle Arrangement

The spectacles icon takes the user to the arrangement overview

Bundle Arrangement Overview

The New Activity lists the user activities that are performed at the bundle level. This is used to launch the Update Product Bundle activity to add more CTs to the master account.

The Bundle Participants section lists the CT accounts that are part of the master account. The spectacles icon drills down to the respective CT account arrangement overview

The Hierarchy section of the bundle arrangement overview lists the various accounts that are part of the hierarchy. The spectacles icon drills down to the respective account arrangement overview.

The Add A/C to Pool tab allows user to add different types of accounts to the pool. This is to provide easy access from the bundle overview and requires customisation of the enquiry based on the products displayed.

The settlement property specifies the default settlement (in the case of CS/SA/CT) and counter booking account (in the case of TR/CS/SA). Navigate from the bundle overview into the respective account overview, the user can launch Update-Settlement activity from the New Activity List.

For example, counter booking for a TR account.

New Activity List

The below screenshot shows a default settlement account for a CS

When the settlement account is specified, the relevant pay in or pay out settlement instructions need to be switched on by setting the value to Yes.

The user navigates to the respective account arrangement overview and New Activity List to launch the Update Limit activity to set internal limit for a TR/CS/SA.

The below screenshot shows an internal limit on a TR

Setting the Internal Limit to 1,000.00 results in the maximum debit balance on this account to be 5,000.00.

Even though the Group Balance is close to 1 Million USD + 10 Million in Credit Facility, debiting USD 6,000.00 from this Account would result in the following override message.

To set a restriction of limit utilisation by a CT on shared limit, the user can navigate to the respective Account Arrangement Overview and select the New Activity List to launch the Update Limit activity.

The below screenshot shows Bundle Participants in bundle overview:

The below screenshot shows a New Activity on CT Account Overview

Update limit to restrict maximum utilisation of the available balance by the EUR CT to EUR 15,000.00.

The financial summary of the EUR CT is shown below:

The account balance of the EUR TR is shown below:

Debiting EUR 20,000.00 from TR results in this limit excess message on the EUR CT account 85294.

| Column 1 | Column 2 |
|---|---|
| Interest all types (credit or debit or special) | The system calculates an up-to-date accrual of each individual interest property. Makes required adjustments to any of these interest properties. Honours adjusted periods, that is, a forward dated effective date. |
| Tax on interest | When defined, the system calculates all tax up to this point on each individual property. |
| Charges all types (periodic or scheduled or activity) | The system calculates all types of charges up to the effective date. Makes up-to-date accrual of the individual charge properties. Evaluates all activity charges. |
| Tax on charges | The system calculates all tax up to this point on all charge properties. |
| Evaluate all activity restrictions | Per product definition, any defined rules need to be honoured. |
| Evaluate and generate any associated messaging | Per product definition activity messaging generates the appropriate advice. |
| Evaluate all current core services attached | A validation report is generated. |
| When the calculated balance is negative, validation shows an error. | Manual steps are needed to bring the balance into credit. The process can then be run again. |

The accounts in the BN pool can be internally moved at any point. To facilitate this, the activity ACCOUNTS-CHANGE.PARENT-ARRANGEMENT is initiated from the New Activity menu.

When this process happens, the balances from the previously linked parent account is also be transferred.

The above screenshot sows a TR is linked to SA account (2000003347) and this SA account has the same balance as the linked TR account.

New Activity menu from the TR account, the User activity ACCOUNTS-CHANGE.PARENT-ARRANGEMENT can be initiated.

For restructuring, this activity happen during COB, hence, the Effective Date should be day +1.

The new parent account is changed to 2000003355, which is a new SA account.

After authorisation and a COB is run, the restructure process is initiated.

A balance of USD 88,592.08 is moved from (2000003347) to (2000003355) account.

BN Pool accounts can be moved from one parent account to another parent accounts. To move an account, select the respective account, click and click Move account . Once the account is selected to move, select the target account and click Paste . When the account is already in Draft or Preliminary, the account is moved to the target parent immediately.

Select the target parent account and click Paste . When the account is in preliminary, the account is moved to the target parent account immediately.

Account 2000003328 is moved to the new parent, that is, bundle arrangement.

If the account is in Live, then the account is moved on the next working day or with a future business date. The account remains with the existing parent, terms and conditions remains the same. Once the system reaches the schedule date, the account is moved to the new parent.

Intra-cash pool movement of the Sub-structure (GUI)

To move the sub-structure from one parent to another parent account, right-click the account that needs to be moved the new parent. New dialog box appears with confirmation, whether the account wants to be moved with sub-structure or only with the selected account. By clicking on Also move sub-structure , the entire sub-structure is moved to the new parent.

Temenos Transact scheduled a new activity and the account is moved on the scheduled date. Hover on the card to view the change parent details.

Financial institutions collect charges on master cash pool account, which is the master arrangement for the pool hierarchy, even when master cash pool account is a non-financial product.

Temenos core banking suite levies charges on master cash pool account (non-financial product) by extending the functionality of some of the property class to the bundle product line.

The charges levied on master cash pool account is posted to the nominated financial settlement account.

- Bundle account /master account detail = Arrangement No AA17132HJ8T0
- Settlement account detail = Arrangement No AA171323JK92, account no 85073
- CT account detail = Arrangement NO AA17131SVQ33, account no 85057
- For the above master account following charges are configured
- Subscription and setup fees are fixed as USD 1000 and EUR 500 respectively.

The below screenshot shows the Master Account overview:

The setup fee is configured as fixed amount of EUR 500 for this bundle accouent.

Subscription fee is configured as fixed amount of USD 10000 for this bundle account.

Schedule for collection of subscription fees is 3 days.

Defined default settlement account is 85073.

Defined settlement account 85073

Charges are levied on master account, debited to default settlement account as shown below:

> **⚠️ Note:** Difference in the charge amount for setup fee is due to the currency difference.

| Column 1 | Column 2 | Column 3 |
|---|---|---|
| Account Number | DR/CR | Amount |
| 12345 | DR | EUR 1,000 |
| 67899 | CR | USD 1,0811.77 |
| 22333 | CR | EUR 1,000 |
| 44555 | DR | USD 1,0811.77 |

When the user updates rate through Preferential Pricing FX condition, (with a date effective in the future), the new rates are available to all TRs from that date.

When the user updates rate in Preferential Pricing FX condition, with a date effective in the past (T-3),

- Existing transfers are not recalculated.
- New internal FX transactions takes rates effective as of the booking date.

The system automatically closes the pricing arrangement on static review, if the customer is no longer eligible for this pricing arrangement

- This would happen as the Eligibility rules for the Internal FX Pricing arrangement are the same as that of the Master Account.
- When a customer is not eligible to open a master account, the customer is not eligible to have an internal FX pricing arrangement either.

| DR | CR |
|---|---|
| EUR TR 1,000.00 | Contra EUR TR 1,000.00 |
| Contra USD TR 1,250.00 | USD TR 1,250.00 |

In the CUSTOMER.MASS.BLOCK application, the user can provide the AA Bundle Arrangement ID in the AA Bundle ID field to block all the accounts, which are part of that bundle for transaction processing.

In case of BN, by entering the AA Bundle Arrangement ID and committing the record, all currency top accounts, which are part of that bundle is blocked for transaction processing (posted against transaction accounts, which are part of the same BN structure).

Example: A BN structure is created in the system with master account arrangement bundle ID as AA171075RFH6.

This bundle arrangement has two currency top accounts: AA17107RHMWK (EUR) and AA17107BB6H6 (USD).


###### Block Entire Cashpool structure (GUI)

To block the entire BN structure, select Emergency Block from Tools menu. Select SUSPEND CASHPOOL to block all accounts, which are part of the respective bundle for transaction processing.

> **⚠️ Note:** To block the BN pool, Start date is a mandatory field. Expiry date is an optional field.

Suspend can be done with future start date and expiry date. Once the Temenos Transact reaches the particular Start of Day (SOD), all the accounts which are part of that Bundle are blocked for Transactions. Fund transfer, standing order and sweeping scheduled (between the accounts in the bundle structure) are also suspended.

Once the BN pool structure is blocked, further maintenance on accounts is also suspended and the structure blocked message is displayed.

To unblock the BN structure, select Unblock Structure from the Tools menu. Enter the date in the Expiry date field and provide the reason and click UNBLOCK STRUCTURE button.

> **⚠️ Note:** The date in Expiry date can be current or future date and when,

- Current date is provided, the structure is unblocked immediately and the user can perform transactions on BN accounts.
- Future date is provide, Temenos Transact removes the blocked status during the start of day of the particular end date.

To block the sub-structure, Select Emergency Block from Tools menu and click BLOCK ACCOUNT OR SUB- STRUCTURE . By selecting the parent accounts GUI blocks the child accounts linked under the parent account. In Temenos Transact child accounts are not blocked and only parent account is blocked. When the user initiates the transaction on TR accounts, Temenos Transact displays an error message and further transactions are not allowed. Enter date in Start date and Expiry date fields to block the sub-structure and a particular account. Temenos Transact allows to block the sub-structure or an account with future start date and end date.

When the user selects the parent account, the child accounts linked under the parent are selected automatically and in GUI, the status is shown as blocked.

Once the sub-structure and accounts are blocked, the status is updated on each account and the tool tip is shown on each card with the date on which the account is blocked. When the parent is blocked, the child account details are also updated as blocked in GUI.

Block details are updated in card and tree view.

To unblock sub-structure or an account, select Unblock Account or Sub Structure . The blocked accounts are selected by default. The user can deselect an account when there is no need to unblock. Enter the Expiry date and click UNBLOCK ACCOUNTS to commit the changes in Temenos Transact. Expiry date can be current or future dated. When current date is used to unblock the account, it is unblocked immediately and Temenos Transact allows to initiate transactions.

BN pool GUI structure is refreshed with the changes in Temenos Transact and the blocked status is updated in GUI. Once the account is unblocked, the strike line on an account is removed immediately.

A CUSTOMER.MASS.BLOCK record is created to block the two CT accounts starting 18 April 2017, until 19 April 2017.

By giving the bundle arrangement ID and committing this record, the CT accounts are blocked and no transactions are posted against any transaction accounts linked to these currency top accounts.

The accounts are unblocked by giving the expiry date and an unblocking code.

A BN structure is created in the system, having a master account arrangement bundle ID as AA171075RFH6.

This bundle arrangement has two currency top accounts: AA17107RHMWK (EUR) and AA17107BB6H6 (USD).

A TR account can be disconnected from a BN pool and then it can be ultimately closed. In such cases, the balances, capitalised interest and charges are transferred to another account.

The general process to disconnect and close an account from the BN structure is as follows:

- The user switches the TR account from off balance sheet to on balance sheet. This is done when user executes an activity to remove the TR account from the pool, a change product is also executed.

> **⚠️ Note:** When closure is attempted, validation is done to confirm that link to the BN pool is removed. If not, a related error is displayed.

Click here to refer Arrangement Closure.

These reports are accessible through the Corporate Single Customer View (SCV) of corporate user menu under balance netting or in the role based home page for balance netting administrator.

The key reports are explained below.

This report provides an overview on the latest terms and conditions registered in the account. The details include cover control, internal or external credit limits, payment restrictions and blocked amounts.

The details provided in this report are:

- Account type
- Account number
- Currency
- Date for latest modifications
- Cover control (on/off)
- Capitalisation account
- Frequency of capitalisation
- Settlement account
- Deposit interest (margin and base rate used)
- Deposit fee (negative interest as a fee)
- Lending interest
- Lending fee
- Unauthorised overdraft interest
- Unauthorised overdraft fee
- Penalty fee (in regards unauthorised overdraft)
- Day method
- Inheritance
- Thresholds
- Blocked amounts
- Unable to check if conditions and terms seen are internal or external

When the user selects several accounts, the search can be limited to comprise only accounts in a certain currency.

The below screenshot shows the terms and condition of master account - Interest:

The below screenshot shows the terms and condition of master account – Charge:

The below screenshot shows the terms and condition of master account – Schedule:

The basic account information per current day for a BN cash pool account are shown below:

- Account type
- Activation date
- Disconnected date
- Date for latest modifications
- Scheduled event(s) and the date for it
- Account number both BBAN and IBAN format
- Account country (that is, the country in which the account is located)
- Currency
- Balance reporting (which type, for example, account statements such as MT940, MT941)
- Frequency of the statement (for transaction accounts only)
- Parent account
- Settlement account
- Capitalisation account
- Customer name
- Customer ID

> **⚠️ Note:** The closure date is also displayed for closed accounts.

The below screenshot shows that a search on master account displays the summary and currency summary account and transaction account in the hierarchy.

The user Credit report for BN accounts is available with the below details:

- Account number and account type
- Limit attached to accounts within the structure
- Type of limit
- The size of the limit
- Currency of the limit
- Interest and fees linked to the limit
- Automatic renewal
- Placed securities (type of collateral)
- Registration date
- End date
- Renewal date

The below screenshot shows that a search on master account displays the summary and currency summary account and transaction account in the hierarchy.

This report displays all the internal cash pool services that are linked to the accounts in the hierarchy.

- Automated balance transfer
- Internal automated balance zeroing
- Internal FX balance transfer
- Internal standing order

The below screenshot shows that a search on master account displays the summary and currency summary account and transaction account in the hierarchy.

The following details are found for a selected balance netting account:

- Account number and account type
- Interest type
- Accrued interest
- Capitalised interest current year
- Capitalised interest previous year
- Capitalised interest latest period
- Date for latest capitalisation
- Specification of accrued interest
- Internal interest calculated but requested not to be capitalised for the current year
- Internal interest calculated but requested not to be capitalised for the previous year
- Internal interest calculated but requested not to be capitalised for the latest period

The below screenshot shows that a search on master account displays, the summary and currency summary account and transaction account in the hierarchy. The results can be exported to an excel.

The user can extract information on structural changes in a hierarchy at account closed and accounts moved level. The latter is within a structure or to another BN structure in a bank. Only live structures apply for structural changes (not draft or preliminary).

A below report on structural changes of all MA bundles in Temenos Transact are:

- The list is sorted by MA bundle owner and not by the change.
- Specify the account type taking part in the structural change
- Specify the type of structural change (add, delete and move)
- Specify if the structural change is conducted by a bank user or the customer
- Specify the ID of the user who registered or entered the change
- Account number and customer ID of account involved in the structural change
- If account is moved, then the user should specify the parent account number to which the account is moved ( MA /SA/ CS)
- The go live date of the structural change
- The date the structural change was registered
- Total number of structural changes (aggregate of added, closed and moved respectively) in each MA bundle. This can be used to simplify charging the customer of the structural changes.

A report on structural changes in a specific MA bundle:

- State the MA bundle the structural changes are extracted from
- Specify the account type taking part in the structural change
- Account number and customer ID of account involved in the structural change
- Specify the type of structural change (add, delete and move)
- Specify if the structural change is conducted by a bank user or the customer
- Specify the ID of the user who registered/entered the change
- If account is moved, specify to which parent account number the account is moved ( MA /SA/ CS)
- The go live date of the structural change
- The date the structural change was registered
- Total number of structural changes (aggregate of added, closed and moved respectively) in the specific MA bundle. This is done to simplify charging the customer of the structural changes.

This report displays all transactions (booked during the given period of dates) and transfer details (such as, reference number) if attached to the payment.

If a TR is moved from one structure to another and the search date is before start date in new structure, the system displays the historical transactions only for searches on TR account.

Transactions can be filtered by:

- Transactions within a certain currency
- Customer internal transactions
- Intra-cash pool transactions
- Transactions between certain amounts
- All debit and credit transactions

A search on master account displays the summary and currency summary account and transaction account in the hierarchy

The Integrity Check Days attribute in Bundle Hierarchy Property Class is used to schedule an evaluation on ‘n’ number of days before an event is triggered in the bundle.

The first integrity check is run ‘n’ number of days before go live date for a pool in preliminary status.

This validation runs on continuous basis ‘n’ number of days before every event in the Bundle.

> **⚠️ Note:** Integrity check days are calculated as ‘n’ working days.

- Integrity check orchestrates the validations from MA level to the underlying accounts in the hierarchy.
- The system triggers the Activity Class BUNDLE-INTEGRITY.CHECK-ARRANGEMENT to run the integrity check.
- The user can trigger ad-hoc integrity checks by manually running the activity class for integrity check. The system automatically runs the pool orchestration service and generates integrity report.

- Validations are run on the bundle and results are recorded in AA.POOL.EXCEPTION.LOG. The record ID is Arrangement Number-INTEGRITY.REPORT.

- It is possible to query on this table using the bundle (arrangement) number. This displays a single screen that contains all the validations related to all the accounts in the bundle, especially the failures

- Drilldown to the individual accounts are available to take correction actions.

The below are the validations based on pool events.

A complete scan is carried out when go live date is set.

When the live date is given (not null), the scan is carried out at the pool level.

- Pool cannot go live without even a single CT.
- CT cannot exist without MA and TR.

The system validates,

- If the bank is working on the dates in which pool has tasks scheduled at SOD
- If previous calendar date is a working day

- A warning message giving the childless CS or SA or CT is closed automatically
- Currency availability in weighted rate calculation (CT and SA) CT: When 4 CTs are in bundle but only three currencies are specified in custom type in Recipient CT Interest property, then exception message is raised for the missing custom type in that currency SA: Validates if all the currencies for which balance is maintained in ECB, are specified in the custom type

- Currency market rate for currencies in secondary currency market Takes recipient’s secondary currency market, and scan through CURRENCY table in recipient CT company for each allowed currency of the bundle and see if there is a rate definition for this secondary currency market. An exception is recorded for the missing rate definition

- Settlement account validation All properties, payment types have settlement accounts (payment schedule, activity charges and rule break charges) Settlement and counter booking belong to the same pool and currency, the status of those accounts for the date (this account’s go live date atleast) required Settlement account specified in bundle settlement Settlement instruction switched on (if not, warning message) Settlement and counter booking account should be available for the go live date of the CS or SA or TR During new offer of SA or CS, a new offer TR can be attached as a settlement account but it must be set to go live for the SA or CS Go live date

When an account is linked to the pool, the below validations are performed:

- External sweeps are set for the account
- External STOs are set for the account
- Account with negative balance (error is raised when TR account is linked)
- AC pre closure validations are performed
- Account is scheduled for closure TR has external sweep or STO

When an account is delinked from the pool, the below validations are performed:

- Internal sweeps are set for the account
- Internal STOs are set for the account
- AC Pre closure validations
- Account scheduled for closure TR has internal sweep or STO

During the closure of an account, the below validations are performed:

- Negative balance in account
- Sweeps setup in account
- Accounts has a record already in AC block closure


###### Closure of entire pool structure (GUI)

BN pool can be closed during Draft, Preliminary and Live status. To close the BN pool structure, right-click the 3 dots on Master card and select Close Entire Pool . Closure of live BN pool online is not possible. It is possible on the next business day or on a future date.

Closing the preliminary BN pool is done online and future scheduling is not possible. Master arrangement and SA, CS, TR or MTR accounts linked to the pool is closed online and Tree or Card view is updated accordingly. GUI displays a warning message to the user before closing the entire BN pool. When the user clicks on YES, GUI passes the information to Temenos Transact and the accounts are closed.

Cross pool event go live date against destination pool go live date and parent go live date is validated and exceptions are logged in case of breach.

> **⚠️ Note:** When these validations are not met, exception log is updated with a warning message.

Cross-pool movements of the Sub-structure

When arrangement is part of a hierarchy of accounts such as, a cash pool hierarchy, the arrangement interest, charge and capitalisation frequencies need to be set (not at product level but at another arrangement higher up in the hierarchy). In a cash pool structure, this means setting conditions for inheritance at the (parent or grandparent) or (pool or currency specific concentration level).This helps in easy maintenance of these conditions in a single place instead of having to deal with the individual arrangements at the lowest level, which also happen to be the normal transaction accounts.

---


### 2.5  Upfront Profit in Club Finance


> **📇 Quick Reference Card**
> 
> **Applications:** `AA.INTEREST.ACCRUALS`
> 
> **Key Fields:** *Accounting Mode*, *Participant Accounting Type*
> 
> **Sections:** 🔧 Working With


#### 🔧 Working With

When a bank sets the upfront profit calculation method for a club finance, the system calculates the upfront profit receivable for borrower and for each participant based on each participant’s share.

A club finance of USD 20,000,000 for a term of 2Y is provided to the borrower. It is funded by two participants, own bank and a participant bank (Abn Amro Securities). The own bank which is also the Agent bank funds USD 12,000,000 (60%) whereas Abn Amro funds USD 8,000,000 (40%).

The bank has the following setup:

- Profit Condition - 5% fixed rate with upfront profit setup
- Rate type – Flat type

The screenshot below shows the principal interest (accrued) of the contract 124605 in the Arrangement Overview page.

The profit amount is split among the participant banks based on their share in the club finance. The profit rate for accrual is same as the borrower’s.

Own bank’s share: Profit amount = 150,000.00* 60% = USD 90,000

Abn Amro’s share: Profit amount = 150,000.00* 40% = USD 60,000

The system calculates the profit rate and profit receivable from the borrower as shown in the screenshot below.

The profit amount is raised as receivable profit in each participant and borrower’s ECB and the profit rate is updated in AA.INTEREST.ACCRUALS records of the respective participants.

REC and ACC balance of the borrower is USD 150,000. The borrower’s receivable is raised as memo entries as shown in the screenshot below.

REC and ACC balance of own bank’s share is USD 90,000, raised as real entries as shown in the screenshot below.

REC and ACC balance of participant bank’s share is USD 60,000 as shown in the screenshot below. It is raised as either memo or contingent entries based on the Participant Accounting Type field setup.

> **⚠️ Note:** The Offline Processing of participant balances setup in Participant product condition is preferred for club finance with upfront profit receivable.

The following are the scenarios based on which the bank can calculate the upfront profit with the respective accounting entries.

- Due for Repayment When the profit is made due to the borrower based on the Payment Schedule, the system generates a bill with the profit accrued till that date for the borrower. The system issues a separate bill for each participant with the profit accrued on the participant’s books, based on their share. Refer for Upfront Profit for Club Finance more information about the detailed accounting enteries.
- Advance repayment – Cash basis and Amort basis In case of advance repayment of profit bills, with issuing and settling by producing the bills, the system recalculates the profit rate based on their advance interest accounting method – ‘Cash Basis’ or ‘Amort Basis’. Refer for Upfront Profit for Club Finance more information about the detailed accounting enteries.
- Recalculation of Upfront Profit If the user sets the Interest condition to recalculate the upfront profit amount when there is a change in profit condition or disbursement activity, then the upfront profit amount of the borrower and the participants are recalculated. The system then updates the upfront profit amount and profit rate of borrower and each participants in its respective AA.INTEREST.ACCRUALS records.
- Share Transfer When a bank participating in a club finance is transferring its share to another bank at any time during its lifetime, then the system recalculates upfront profit receivable of the selling bank and the buying bank, based on their share from the day of transfer. The receivable profit will be transferred to the selling bank to buying bank. If an own bank transferring 20% of its share to its participant bank, then the system transers 20% of own bank’s receivable profit to the buying bank. Therefore, the upfront profit receivable of the buying bank increases to USD 76,627.56 and the upfront profit receivable of the own bank adjusts to USD 70,733.14.

> **⚠️ Note:** During takeover of a club finance with upfront profit from legacy system, the user must enter the outstanding receivable profit amount as flat profit amount receivable. Defining flat rate or reducing rate is not supported.


##### Restrictions in Enabling Upfront Profit

The following features are restricted for club finance with upfront profit.

- Advance or Receivable type of interest in Accounting Mode - The system raises the accounting entries based on the values in the Accounting Mode field. In the upfront profit mode of club finance, the upfront profit collected in advance before the interest periods and receivable type of interest are not supported.
- Skims for Participants - Skim is the difference between the interest received from the borrower and the interest paid to the participant by the owning bank. In upfront profit method for club finance, skim margins rates are not supported.
- Highest or Lowest type of interest - Compare rates option is used by banks to choose the highest or lowest rate among multiple interest rates defined to calculate the interest. This is not supported for club finance with upfront profit.
- RFR type of interest - Risk free rates tied to RFR index for interest is not supported in club finance with upfront profit.
- Splits and Merges of loans - Spliting and merging of club finance with upfront profit is not supported.
- Risk fees and risk margin (interest properties) collection - Risk fees and risk margin to be paid to Risk Participants cannot be defined using upfront profit mode.
- Loan Securitization - Upfront profit for club finance concept does not include loan securitization which allows the bank to sell the outstanding amount of the loan principal (or a part of it) to an investor (who is part of the pool).
- Pricing Grid - Pricing Grid is used to determine the eligible interest rate or margin for a loan based on these pre-defined criterion values which is not supported for club finance with upfront profit.
- Secondary Loan Trading of loan - Trading of club finance with upfront profit through loan trade application is not supported.


##### Rebate of Upfront Profit

When the customer initiates the pay-off (Early closure of loan) on a loan, a certain amount is rebated as part of the early payoff instead of paying this amount to the borrower, there is an option into adjust this amount to the profit amount to be repaid to encourage the borrower for early payoff or closure of loan.

There are multiple ways in which the system can rebate the amount to the customer. They are as follows:

- Effective date – The profit accrued till that date is marked as bank's profit and remaining receivable profit is rebated.
- Period end date – The profit that is accrued till the current repayment period is marked as bank's profit and remaining receivable profit is rebated.
- Payment end date – The profit amount fixed upfront is marked as bank's profit and no amount is rebated.
- Context – During the rebate activity, the bank user gives the amount that should be collected from the borrower. The remaining upfront profit amount is rebated back to the customer.
- Percentage – Certain percentage of receivable profit is rebated back to the customer during early closure.

The borrower gets a club loan of USD 10,00,000 for a term of 1Y. Two participants, Own bank and a Participant bank (Abn Amro Securities) funds the loan on 1st March 2024. The own bank, also the Agent cum participant bank funds USD 8,00,000 (80%), whereas Abn Amro funds USD 200,000 (20%).

The bank has setup profit condition with 50,000 as fixed amount with upfront profit setup. The bank has setup to collect it as Flat rate. During early closure rebate, 5% of receivable profit is configured.

After repaying due bills,

Customer ECB is shown in the screenshot below :

Participant ECB is shown in the screenshot below :

Own book ECB is shown in the screenshot below:

The system updates the participant and own bank bills on pro rate basis as shown in the screenshot below.

Pay off bill is shown in the screenshot below:

Own Book Pay off bill is shown in the screenshot below:

Participant pay off bill is shown in the screenshot below:

Based on the pay-off amount, payment order can be initiated, and all balances would be closed.

> **⚠️ Note:** Rebate feature applies only to Loan pay off. Rule 78 is restricted to club loans with upfront profit interest.


> **Related Applications:** `AA.INTEREST.ACCRUALS`

---


### 2.6  Asset Capture


> **📇 Quick Reference Card**
> 
> **Purpose:** *Asset capture is the starting step for Islamic finance process and is used to maintain the asset inventory to be sold. Asset request is made when there is a requirement from a customer or client.*
> 
> **Applications:** `EB.LOOKUP`, `EB.TABLE.DEFINITION`, `IS.ASSET`, `IS.BROKER`, `IS.COMMODITY`, `IS.REALESTATE`
> 
> **Key Fields:** *Address*, *Allowed Unit*, *Area*, *Asset Description*, *Asset Short Title*, *Asset Table*, *Asset Type*, *Builder Code* ... +46 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Asset capture is the starting step for Islamic finance process and is used to maintain the asset inventory to be sold. Asset request is made when there is a requirement from a customer or client.

Asset types are divided into two:

| Named asset | Quantified asset |
|---|---|
| Specifies or captures individual specifications for each asset. | Does not specify individual asset-specific characteristics |
| A vehicle has specific features and characters that is captured such as, chassis number, engine number, etc. A house has specific features and characters like dimensions. | Oil, rice, vegetables, metals, etc. |

Asset capture defines the following table and fields for named assets:

- User-specific tables.
- Additional fields to existing table to capture additional details


#### ⚙️ Configuration

This topic helps the user to understand the configuration required for asset capture.


##### UnderstandingIS.COMMODITY

The following fields in IS.COMMODITY govern the asset capture functionality for named assets and quantified assets.

| Field Name | Description |
|---|---|
| Commodity Status | Indicates whether commodity is active. Valid values are defined in the EB.LOOKUP table with prefix IS.STATUS*. |
| Asset Type | Indicates the asset type. Valid values are Named and Quantified. |
| Asset Table | The application in which the asset is defined. This application could be a regular or dynamic table. Applicable for named asset types. |
| Allowed Unit | The units in which commodity is transacted. Valid values are defined in the EB.LOOKUP table with prefix IS.UNIT*. |
| Decimal Qty | Identifies the number of decimals the asset quantity can be transacted. Mandatory for quantified asset types. |
| Buy Broker | Lists the brokers who can transact as buy broker for the commodity. Must be a valid record from the table IS.BROKER . The broker allowed should be eligible for buy or both. Applicable for quantified asset types. |
| Sell Broker | Lists the brokers who can transact as sell broker for the commodity. Must be a valid record from the table IS.BROKER . The broker allowed should be eligible for sell or both. Applicable for quantified asset types. |


##### ConfiguringIS.COMMODITY(Asset Table)

Asset table is user-definable and the user has fields to capture the required information for asset. The following steps are used to create a table and link it to IS.COMMODITY table:

1. Define a unique named asset table record and fields required to collect the required information using EB.TABLE.DEFINITION application. For example, IS.REALESTATE is named asset table.
2. IS.ASSET * IS.REALESTATE .
3. When the named asset table is added to EB.LOOKUP table, it is available for user selection in Asset Table field in IS.COMMODITY .


#### 📋 Tasks

Asset capture is used to specify or capture individual specifications for each named assets, such as, vehicle, real estate, equipment, miscellaneous and movable equipment, so that the bank can purchase these assets on behalf of customer or client.


##### Workflow

In Asset Capture, the user can perform the following activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Capture Asset Details . |
| List of Assets | Click the New icon corresponding to the equipment asset type. |
| Equipment | Enter values in the required fields: Customer Currency Vendor Unit Price Asset Description Asset Short Title Seller Customer ID Seller Customer Name Seller Settlement Ac In the Equipment Specific Details tab, enter values in the following fields: Equipment Name Equipment Type Year of Manufacture Make Model Origination Country In the Dealer Details tab, enter values in the following fields: Dealer Code Dealer Name Equipment Located at Invoice No Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Authorise/Delete/View Asset Capture . |
| Unauthorised Assets | Enter a value in the Commodity or Customer field. Click the FIND button. Select the Authorise option from the drop-down corresponding to a record. Click the Launch icon. |
| Vehicle/Real Estate/Equipment/Movable Equipment/Miscellaneous Asset | Click the Authorise icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Amend – Asset Capture Details . |
| IS.ASSET.AMD | Enter a value in the Commodity or Customer field. Click the FIND button. |
| Amend Asset Detail | Click the Amend icon corresponding to a record. |
| Vehicle/Real Estate/Equipment/Movable Equipment/Miscellaneous Asset | Enter values in the required fields. Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

There are no Outputs available for Asset Capture feature.


> **Related Applications:** `EB.LOOKUP`, `EB.TABLE.DEFINITION`, `IS.ASSET`, `IS.BROKER`, `IS.COMMODITY`, `IS.REALESTATE`

---


### 2.7  Asset Review


> **📇 Quick Reference Card**
> 
> **Purpose:** *Asset Review ( IS.ASSET.REVIEW ) application captures the review particulars of the asset. An appraiser or reviewer provides opinion on the value of the asset or commodity for a fee.*
> 
> **Applications:** `CUSTOMER`, `IS.ASSET.REVIEW`, `IS.REVIEWER`
> 
> **Key Fields:** *Asset Reference*, *Asset Value by Appraiser*, *Bank Share (Amount)*, *Commodity*, *Currency*, *Customer*, *Customer Account*, *Customer Share (Amount)* ... +13 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Asset Review ( IS.ASSET.REVIEW ) application captures the review particulars of the asset. An appraiser or reviewer provides opinion on the value of the asset or commodity for a fee.

The asset review feature allows the following:

- Record fee for service
- Split fee into customer and bank fee
- Setup project status and next review meeting dates
- Record profit or loss amount


#### ⚙️ Configuration

The reviewer ID should be a valid customer ID in the CUSTOMER application and this customer should be maintained in the IS.REVIEWER application.


#### 📋 Tasks

Related topics:

- Perform Asset or Commodity Review (IF)
- Islamic Financing processes
- Manage Reviewer (IF)

Asset Review is the process of reviewing or verifying the asset or commodity involved in the purchase. This can be carried out by appraiser, surveyor or reviewer based on the type of asset or commodity.


##### Workflow

This section allows the user to perform the below activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Input – Asset Review . |
| Input Asset Review | Click the Review Asset icon. |
| Input Asset Review | Enter values in the following fields: Reviewer Reviewer Name Reviewer Type Reviewer Account Purchase Reference Customer Customer Account Commodity Asset Reference Currency Effective Date Review Date Description Asset Value by Appraiser Progress Percentage Status Valuation Fees Bank Share (Amount) Customer Share (Amount) Notes Upcoming Review Date Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

| SCREENS | WORKFLOW |
|---|---|
|  | Authorise/Delete/View - Asset Review . |
| Unauthorised Asset Review | Click the Authorise icon. |
| Input Asset Review | Click the Authorise icon. |


#### 📊 Outputs

There are no Outputs available for Asset Review feature.


> **Related Applications:** `CUSTOMER`, `IS.ASSET.REVIEW`, `IS.REVIEWER`

---


### 2.8  Commodity Delivery and Sale


> **📇 Quick Reference Card**
> 
> **Purpose:** *Commodity delivery and sale functionality is used for Bai Salam products, where advance payment is made to the vendor for goods to be delivered at a future date. Quantity and quality of the goods or commodities intended to purchase at future date are recorded.*
> 
> **Applications:** `IS.COMMODITY.POSITION`, `IS.COMMODITY.SALE`, `IS.CONTRACT`, `IS.CONTRACT.DELIVERY`, `IS.PARAMETER`
> 
> **Key Fields:** *Asset Delivery Tracking*, *Delivery Date*, *Delivery Quantity*, *Purchase Reference*, *Sale Quantity*, *Sale Unit Price*, *Sell Quantity*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Commodity delivery and sale functionality is used for Bai Salam products, where advance payment is made to the vendor for goods to be delivered at a future date. Quantity and quality of the goods or commodities intended to purchase at future date are recorded.

Commodity delivery and sale can be used to,

- Record the commodities delivered in partial or full
- Sell the delivered commodities in partial or full
- Track the requested, delivered and sold details of the commodities
- Record the profit or loss amount

The following applications can be used to create and manage delivery and sale of commodities:

| Application | Description |
|---|---|
| Commodity delivery ( IS.CONTRACT.DELIVERY ) | Tracks the delivery of commodities or assets. |
| Commodity sale ( IS.COMMODITY.SALE ) | Sells the delivered commodities to clients either partially or fully. |
| Commodity position ( IS.COMMODITY.POSITION ) | Tracks the commodities requested, delivered and sold details. |


#### ⚙️ Configuration

This topic enables the user to understand the configuration required for commodity deliver and sale.


##### Configuring Commodity Delivery

The Asset Delivery Tracking field in IS.PARAMETER is set to Yes, for the product code used in Islamic Contracts ( IS.CONTRACT ).


#### 📋 Tasks

Related topics:

- Manage Commodity Delivery (IF)
- Islamic Financing processes

Commodity delivery and sale functionality captures the delivery or sale of assets or commodities which are purchased, also tracks the requested, delivered and sold details of assets or commodities.


##### Workflow

This section helps the user to perform the below tasks:

| SCREENS | WORKFLOW |
|---|---|
|  | Input - Asset Delivery Details . |
| Delivery Tracking of Assets | Click the Delivery Asset icon of a corresponding record. |
| Asset Delivery | Enter values in the following fields: Delivery Date Delivery Quantity Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

| SCREENS | WORKFLOW |
|---|---|
|  | Amend - Asset Delivery Details . |
| Amend Unauthorised Records | Click the Amend icon of a corresponding record. |
| Asset Delivery | Enter the field values which require amendment. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

| SCREENS | WORKFLOW |
|---|---|
|  | Authorise - Asset Delivery . |
| Unauthorised Records | Click the Authorise icon of a corresponding record. |
| Authorise – Contract Delivery | Click the Authorise icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Input - Commodity Sale . |
| Commodity / Asset Sale | Click the Input Sale icon of a corresponding record. |
| Input Commodity/Asset Sale | Enter a value in the Sell Quantity field. In the Sale Detail tab, enter values in the following fields: Purchase Reference Sale Unit Price Sale Quantity Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

| SCREENS | WORKFLOW |
|---|---|
|  | Amend – Commodity Sale Details . |
| Amend Commodity Sale | Click the Amend icon of a corresponding record. |
| Input Commodity/Asset Sale | Enter values in the fields which require amendment. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

| SCREENS | WORKFLOW |
|---|---|
|  | Authorise - Commodity Sale . |
| Unauthorised Commodity Sale | Click the Authorise icon of a corresponding record. |
| Authorise Commodity/Asset Sale | Click the Authorise icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Reverse - Commodity Sale . |
| Reversal Commodity Sale | Click the Reverse icon of a corresponding record. |
| Reverse Commodity / Asset Sale | Click the Reverse icon. |


#### 📊 Outputs

There are no Outputs available for Commodity Delivery and Sale feature.


> **Related Applications:** `IS.COMMODITY.POSITION`, `IS.COMMODITY.SALE`, `IS.CONTRACT`, `IS.CONTRACT.DELIVERY`, `IS.PARAMETER`

---


### 2.9  CreatingFacility for IslamicFinanceProducts


> **📇 Quick Reference Card**
> 
> **Purpose:** *A facility or commitment is a lender's promise to offer finance or credit line for a specified amount to a customer. It can be a revolving or non-revolving facility for a definite period of years or months upon which the customer can utilise the commitment extended by the bank through drawings. The ...*
> 
> **Applications:** `AA.PRD.DES.XIS.DRAWING`, `AA.PRD.DES.XIS.FACILITY`, `IS.PARAMETER`
> 
> **Key Fields:** *Amount*, *Currency*, *Customer*, *Decl Level*, *Declaration At*, *Effective Date*, *Fixed*, *IS Product ID* ... +8 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

A facility or commitment is a lender's promise to offer finance or credit line for a specified amount to a customer. It can be a revolving or non-revolving facility for a definite period of years or months upon which the customer can utilise the commitment extended by the bank through drawings. The user can create multiple drawings under the facility.

The bank has to license a FL product code to use the Facility module. Creation of facility for Islamic finance products is similar to the creation of facility for conventional finance products. Read Facility user guide for more information.


#### ⚙️ Configuration

A user can create a facility arrangement for any Islamic finance arrangement depending upon the bank’s need. Multiple drawings can be made under the facility to disburse funds to the customer. It is possible to customise different profit rates for each drawing and the bank can collect the repayment at the facility or drawings level.

This topic explains the creation of a Mudaraba facility arrangement and single or multiple drawings in detail.

Mudaraba is a partnership agreement whereby the bank provides the capital amount, and the customer provides labour, work, or experience. The profit is shared between the capital provider and the customer on a predefined ratio, which is mutually agreed upon and explicitly stated at the time of the contract agreement. The customer declares the actual profit amount at the end of the contract period and then the bank decides whether the profit or loss has to be paid to customer or should be considered as the bank’s income.

The customer can declare the realised profit amount multiple times during the Mudaraba financing period. The user can configure profit-sharing percentage details at the facility or drawings levels as mentioned below:


##### Configuring Eligible Profit Properties for Profit Declaration

The bank can attach multiple profit properties into the facility or drawings arrangement product used to create Mudaraba finance for the customer. To identify the eligible profit properties allowed for profit declaration, the property type ( Type ) of the Profit property needs to be configured as Profit and Profit declaration.


##### Defining Product Condition at Facility Level

While creating a facility arrangement, the user can define the default profit-sharing ratio agreed between the bank and customer can be defined at the facility level using the AA.PRD.DES.XIS.FACILITY product condition which has to be attached to the facility product.

The user can configure the default profit declaration related details at the facility level using the following fields:

- Declaration At – Helps to choose if the realised profit amount has to be declared at the facility or drawings level. Allowed values are Facility, Drawings.
- Mudaraba Profit Share % – Helps to setup the default profit declaration share percentage between bank and the customer. In most of the cases, it is defined at the facility or drawings level.
- IS Product ID – Helps to identify the product parameter reference number created in IS.PARAMETER .


##### Defining Product Condition at Drawing Level

The user can configure the default profit sharing percentage at the drawings level by setting up the values for below fields using AA.PRD.DES.XIS.DRAWING :

- Mudaraba Profit Share % – Helps to setup the default profit declaration share percentage between bank and the customer. In most of the cases, it is defined at the facility or drawings level.
- IS Product ID – Helps to identify the product parameter reference number created in IS.PARAMETER .


#### 🔧 Working With

The following sections describe the creation of facility and drawings arrangements in detail.


##### Creating Facility Arrangement

The user can create a Mudaraba facility for the customer by capturing the customer ID, currency, and an effective date of the facility. After validating the facility transaction, it is required to capture the facility amount, term, declaration level, profit sharing percentage agreed between bank and customer . The system can default the product code from the product condition level. Upon authorisation, the Mudaraba facility is created for the customer.


##### Creating Drawings Arrangement

The user can create a drawings arrangement under the facility by linking it to the facility arrangement. It can also be created without linking it to the facility (finance creation without facility).

The user can create a Mudaraba drawings arrangement by capturing the customer ID, currency, facility reference number, and an effective date. It is required to capture the effective date greater than or equal to the Mudaraba facility arrangement. During validation, the amount, term, expected profit rate, repayment schedule details, settlement account details, profit-sharing percentage and product code can be captured.

- The user can create multiple drawings under the facility to utilise the commitment extended to the customer.
- If the profit declaration details are already defined at the facility level, then the system defaults it automatically into the drawings and the Profit Declaration Percentage can be amended.
- Profit amount is accrued based upon the expected profit rate setup at the drawings level.
- The user can collect the repayment at the facility level and apportion it to the underlying Mudaraba drawings arrangement based upon the configuration.


#### 📋 Tasks

The Mudaraba facility is created for the customer by capturing the Customer ID, Currency, and the effective date of the Facility.


##### Workflow

In Facility Creation, the user can perform the following activities:

| SCREENS | WORKFLOW |
|---|---|
|  | AA – Product Catalog . |
| Product Group | Click the Islamic Facility section to expand. Click the Products icon corresponding to the Islamic Facility product group. |
| Products | In the Islamic facility product screen, click the New Arrangement icon corresponding to the Mudaraba Facility product. |
| New Arrangement (Islamic) | Enter values in the required fields: Customer Currency Effective Date Click the Validate icon to check for errors and overrides. In the Commitment section, enter values in the following fields: Amount Term In the Islamic Facility details, enter values in the following fields: Decl Level Profit Share Perc In the Schedule section, enter values in the required fields. In the Pool ID section, enter a value in the Pool Id field. Click the Validate icon to check for errors and overrides. Click the Commit icon. Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
|  | Find Facility . |
| Product Group | Click the Overview Icon corresponding to the respective Facility. Click on New Drawing icon from the Overview screen. |
| Products | In the product Catalog screen, click the New Arrangement icon corresponding to the Mudaraba drawings product. |
| New Arrangement (Islamic) | Enter values in the required fields: Customer Click the Validate icon to check for errors and overrides. In the Commitment section, enter values in the following fields: Amount Term In the Principal Profit Details section, enter values in the following fields: Fixed (Expected profit rate) In the Mudaraba drawings details, enter or modify values in the following fields: Mudarib Profit Share % In the Schedule section, enter values in the required fields. In the Pool ID section, enter a value in the Pool Id field. Click the Validate icon to check for errors and overrides. Click the Commit icon. Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
|  | AA – Product Catalog . |
| Product Group | Click the Islamic Financing section to expand. Click the Products icon corresponding to the Mudaraba Drawings product group. |
| Products | In the Profit accrual sale product group screen, click the New Arrangement icon corresponding to the Mudaraba drawings product. |
| New Arrangement (Islamic) | Enter values in the required fields: Customer Currency Effective Date IS Product Click the Validate icon to check for errors and overrides. In the Commitment section, enter values in the following fields: Amount Term In the Principal Profit Details section, enter values in the following fields: Fixed (Expected profit rate) In the Mudaraba drawings details, enter or modify values in the following fields: Mudarib Profit Share % In the Schedule section, enter values in the required fields. In the Pool ID section, enter a value in the Pool Id field. Click the Validate icon to check for errors and overrides. Click the Commit icon. Accept the overrides, if any. |


#### 📊 Outputs

There are no Outputs available for Facility Creation for Islamic Finance Products feature.


> **Related Applications:** `AA.PRD.DES.XIS.DRAWING`, `AA.PRD.DES.XIS.FACILITY`, `IS.PARAMETER`

---


### 2.10  Finance Profit Accrual Product


> **📇 Quick Reference Card**
> 
> **Purpose:** *The finance products for which the profit amount is accrued based on the outstanding finance principal amount is grouped under the Profit Accrual Product Group.*
> 
> **Key Fields:** *Bank Share*, *Commodity Sale Ref*, *Currency*, *Customer*, *Customer Share*, *Effective Date*, *Fixed*, *I* ... +6 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The finance products for which the profit amount is accrued based on the outstanding finance principal amount is grouped under the Profit Accrual Product Group.

The following products are grouped under the Profit Accrual Sale Product Group.

- Bai Salam Finance
- Construction Finance
- Diminishing Musharaka Finance
- Forward Ijara Finance
- Mudaraba Financing
- Qard Hassan Finance (Profit-free Finance)


#### ⚙️ Configuration

The below screenshot displays the Product Condition setup for Profit, with Rate Type field set as Reducing Rate.

Refer to, Retail Lending user guide for more information on AA lending configuration setup.


#### 📋 Tasks

Related topics:

- Create and Disburse Baisalam Finance (Manual) (IF)
- Create and Disburse Diminishing Musharaka Finance (Scheduled) (IF)
- Create and Disburse Mudaraba Finance (Manual) (IF)
- Create and Disburse Forward Ijara Finance (Scheduled) (IF)
- Islamic Financing processes

The finance products for which the profit amount is accrued based on the outstanding finance principal amount is grouped under the Profit Accrual Sale Product Group.

During sale process, Islamic contract uses the Retail Lending module to create a finance contract.


##### Workflow

The user can create a new arrangement for any of the Islamic finance products listed under the profit accrual sale product group.

The following products are grouped under the multi structured products product group.

| SCREENS | WORKFLOW |
|---|---|
|  | AA – Product Catalog . |
| Product Group | Click the Islamic Financing section to expand. Click the Products icon corresponding to the Profit Accrual Sale product group. |
| Products | In the Profit Accrual Sale screen, click the New Arrangement icon corresponding to the Bai Salam Finance product. |
| New Arrangement(Islamic) | Enter values in the following fields: Customer Currency IS Product Commodity Sale Ref Effective Date Click the Validate icon to check for errors and overrides. In the Commitment section, enter a value in the Term field. In the Principal Profit section, enter a value in the Fixed field. In the Schedule section, enter values in the required fields. In the Pool ID section, enter a value in the Pool Id field. Click the Validate icon to check for errors and overrides. Click the Commit icon. Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
|  | AA – Product Catalog . |
| Product Group | Click the Islamic Financing section to expand. Click the Products icon corresponding to the Profit Accrual Sale product group. |
| Products | In the Profit Accrual Sale screen, click the New Arrangement icon corresponding to the Construction Finance product. |
| New Arrangement(Islamic) | Enter values in the following fields: Customer Currency IS Product IS Contract Ref Effective Date Click the Validate icon to check for errors and overrides. In the Commitment section, enter a value in the Term field. In the Principal Profit section, enter a value in the Fixed field. In the Schedule section, enter values in the required fields. In the Pool ID section, enter a value in the Pool Id field. Click the Validate icon to check for errors and overrides. Click the Commit icon. Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
|  | AA – Product Catalog . |
| Product Group | Click the Islamic Financing section to expand. Click the Products icon corresponding to the Profit Accrual Sale product group. |
| Products | In the Profit Accrual Sale screen, click the New Arrangement icon corresponding to the Diminishing Musharaka Finance product. |
| New Arrangement(Islamic) | Enter values in the following fields: Customer Currency I S Product IS Contract Ref Effective Date Click the Validate icon to check for errors and overrides. In the Commitment section, enter a value in the Term field. In the Principal Profit section, enter a value in the Fixed field. In the Schedule section, enter values in the required fields. In the Musharaka details section, enter values in the Bank Share (or) Customer Share field. In the Pool ID section, enter a value in the Pool Id field. Click the Validate icon to check for errors and overrides. Click the Commit icon. Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
|  | AA – Product Catalog . |
| Product Group | Click the Islamic Financing section to expand. Click the Products icon corresponding to the Profit Accrual Sale product group. |
| Products | In the Profit Accrual Sale screen, click the New Arrangement icon corresponding to the Forward Ijara Finance product. |
| New Arrangement(Islamic) | Enter values in the following fields: Customer Currency IS Product IS Contract Ref Effective Date Click the Validate icon to check for errors and overrides. In the Commitment section, enter a value in the Term field. In the Deferred Profit section, enter a value in the Fixed field. In the Principal Profit section, enter a value in the Fixed field. In the Schedule section, enter values in the required fields. In the Pool ID section, enter a value in the Pool Id field. Click the Validate icon to check for errors and overrides. Click the Commit icon. Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
|  | AA – Product Catalog . |
| Product Group | Click the Islamic Financing section to expand. Click the Products icon corresponding to the Profit Accrual Sale product group. |
| Products | In the Profit Accrual Sale screen, click the New Arrangement icon corresponding to the Mudaraba Financing product. |
| New Arrangement(Islamic) | Enter values in the following fields: Customer Currency IS Product Effective Date Click the Validate icon to check for errors and overrides. In the Commitment section, enter values in the following fields: Amount Term In the Profit Declaration section, enter values in the following fields: Currency Fixed Amount In the Schedule section, enter values in the required fields. In the Pool ID section, enter a value in the Pool Id field. Click the Validate icon to check for errors and overrides. Click the Commit icon. Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
|  | AA – Product Catalog . |
| Product Group | Click the Islamic Financing section to expand. Click the Products icon corresponding to the Profit Accrual Sale product group. |
| Products | In the Profit Accrual Sale screen, click the New Arrangement icon corresponding to the Qard Hassan Finance product. |
| New Arrangement(Islamic) | Enter values in the following fields: Customer Currency IS Product Effective Date Click the Validate icon to check for errors and overrides. In the Commitment section, enter values in the following fields: Amount Term In the Schedule section, enter values in the required fields. In the Pool ID section, enter a value in the Pool Id field. Click the Validate icon to check for errors and overrides. Click the Commit icon. Accept the overrides, if any. |


#### 📊 Outputs

There are no Outputs available for Finance – Profit Accrual Product feature.

---


### 2.11  Finance Profit Upfront Sale Product Group


> **📇 Quick Reference Card**
> 
> **Purpose:** *The purchased asset is sold to the client for which payment is made through deferred installments. Different modes of financing are available in Islamic banking. During sale process, Islamic contract uses the Retail Lending module to create a finance contract.*
> 
> **Applications:** `AA.PAYMENT.TYPE`
> 
> **Key Fields:** *AA Reference*, *Active Y/N*, *Actual profit amount*, *Advance Payment*, *Advance Profit Accounting*, *Alt Payment Method*, *Amount*, *Arrangement* ... +41 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The purchased asset is sold to the client for which payment is made through deferred installments. Different modes of financing are available in Islamic banking. During sale process, Islamic contract uses the Retail Lending module to create a finance contract.

The following products are grouped under the Profit Upfront Sale Product Group.

- Murabaha Finance
- Ijara (Service Ijara – Murabaha Based)
- Commodity Murabaha


#### ⚙️ Configuration

The configuration settings (Interest product condition) required for Islamic – Profit Upfront Sale product are shown in the screenshot below:

The settings are mentioned in the following table along with a description.

| Field | Value and Description |
|---|---|
| Mode | Upfront Profit - The interest amount is collected at the beginning of the contract |
| Profit Method | Fixed - The total profit amount is fixed. |
| Rate Type | Reducing Rate, Flat Rate or Flat Amount. |
| Recalculate | Profit Amount - All activities that result in payment schedule recalculation can be configured to Profit Amount. |
| Actual profit amount | It is used to capture the upfront profit amount. Applicable only if Rate Type is set as Flat Amount. |
| Original profit amount | It is used to capture the upfront profit amount realised in the legacy system. Applicable only during a take-over activity (migration). |
| Advance Profit Accounting | Amort – Applicable only for flat rate and flat amount of profit contracts. The profit received in advance is booked to PL over the respite period. Cash Basis - The profit received in advance is booked to PL immediately on the respite date. Blank – If no option is selected , the functionality works similar to Cash Basis. |

In order for the respite to work as per the option selected for Advance Profit Accounting , the corresponding Payment Rules setup need to have Settle Unearned Profit as Yes and Advance Payment set as Full.


###### Key Features of Advance Profit Accounting

- Once a contract is moved to or set to have Amort option, it is not possible to move back to or change to Cash Basis option or leave blank.
- The Advance Profit Accounting can be set as Amort at the time of creating an arrangement or during the life of the arrangement. But this field cannot be changed when the contract is currently in a respite period.
- When the Profit Property is set as: Non-Tracking A Change interest condition / Change Product condition can change the Advance Profit Accounting option from Cash Basis or Null to Amort but not vice versa. The Advance Profit Accounting can be set as Amort at the time of creating an arrangement or during the life of the arrangement. But this field cannot be changed when the contract is currently in a respite period. Once a contract is moved to or set to have Amort option, it is not possible to move back to or change to Cash Basis option or leave blank. Tracking If a new product condition is released to change the Advance Profit Accounting from blank to Amort, the change should be tracked. The contracts that are in an existing respite period cannot be set to amort by the system and should be handled as an exception manually. If a new product condition is released to change the Advance Profit Accounting from Amort to Cash Basis, this attribute change does not impact the existing contracts.
- When the Default Attribute Option is set as Resetting for Advance Profit Accounting, and when the Advance Profit Accounting is changed from blank or Cash Basis to Amort, during change product, for all associated contracts all properties and attributes are reset except Advance Profit Accounting .
- During a respite period, if there a change in profit due to rate or principal change: The profit receivable has to be recalculated accordingly and adjustment entries for the difference have to be posted. The profit amount collected during the respite payment should continue to accrue to PL till the respite period end date.
- During the respite period: Another respite can be triggered, and the profit rate is recalculated by the system accordingly. Rate Change can be triggered: The profit amount is calculated and the adjustment is posted to REC (an increase or decrease to the profit amount) But the profit collected during respite period in advance has not changed, so the system continues to amortise this income to the PL. After the respite period, the accrual rate restores to the new accrual rate in order to collect the profit after recalculation. Another respite before the end of current respite: If a second respite is triggered before the end of current respite, then the profit rate is automatically recalculated till the end of the second respite period and accrual continues on the new the profit rate. Prepayment of principal is possible: The profit rate for the respite period and the period after the respite is recalculated for the reduced principal after the prepayment. Payoff can be triggered: The pending receivable income is collected from the customer. The profit amount collected during the respite payment is accrued to the PL immediately. Payment holiday is setup: Respite during Payment Holiday During a payment holiday it is possible to recalculate the term or repayment amount. As a result of the payment holiday if there is a change in term and a respite is triggered, the system respites the respective bills after payment holiday. If the repayment amount is calculated or changed when a respite is triggered, the system respites for the repay amount (installment) before the payment holiday was declared. This is because of the Forward Recalculate Activity being reversed or replayed when a respite is triggered. Any excess fund / shortage paid based on the repay amount in the payment schedule as per payment holiday is treated per the Remainder Activity setup in the Payment Rules. After the respite period: If the Payment Holiday is set up after the end of the current respite period, either the profit rate is recalculated or term is recalculated. This is based on the choice given in recalculation option while declaring payment holiday. Compression can be triggered: The payment amount is recalculated as per the compression amount. The remaining profit after compression is amortised to the P/L until the respite end at the recalculated rate. Change Term can be triggered: The profit receivable have to be recalculated accordingly and entries be reversed and replayed. The apply payment activity for respite is also replayed. The difference amount (excess) after the respite, if any, has to be settled as per the remainder activity in the payment rules for respite. Change term between disbursements Change Payment Schedule can be triggered: The bills generated based on the previous frequency is reversed and new bills are generated as per the latest repayment schedule. The apply payment activity for the respite is also replayed. The remaining funds after the respite will be apportioned as per the payment allocation rules, and, any excess payment will be settled as per the reminder activity in the payment rules for respite. Disbursement can be triggered: The profit rate is recalculated based on the balance after the next disbursement If the system is set to recalculate the profit on disbursement, then the adjustment entries are booked to the P/L immediately After the respite period, the accrual restores to an accrual rate based on the new balance updated after the second disbursement and based on the recalculated profit.
- A respite cannot be triggered in the contract: During the partial or full capitalisation of the contract When a Reset Arrangement Activity is scheduled in the arrangement. When a Change Product Activity is scheduled in the arrangement. When a scheduled Renegotiate arrangement is scheduled in the arrangement.
- In Payment Schedule condition,the user has a choice to decide on the annuity amount based on the disbursements. The Include Future Disb attribute is used to indicate if the future disbursements scheduled must be considered for calculating the constant installment amount. This is applicable for CONSTANT or LINEAR payment type. The attributes Include All Payments and Include Future Disb are mutually exclusive.


##### Capitalisation of Profit

In upfront profit contracts, profit-only schedules can be set to capitalise to the principal. When the profit accruals of a property is set to capitalise, then any other payment type in the same contract using the same property can only be set as Due and Cap. For example, a contract can have

1. Profit set to capitalise with linear payment of principal
2. Profit set to capitalise with bullet payment of principal
3. Profit set to capitalise for few months and then annuity payment types with Due and Cap set (irrespective of an actual amount being used).

> **⚠️ Note:** A regular annuity payment type without Due and Cap option cannot be used for the profit property capitalised in that contract.


###### Partial Capitalisation of Profit

The Alt Payment Method field in AA.PAYMENT.TYPE is set to Due And Cap to enable full or partial capitalisation of interest accruals in a loan. The actual amount indicated in the Payment Schedule is only made due and any remaining interest accruals are capitalised. To read further click here .

Refer Retail Lending user guide for more information on AA Lending configuration setup.


#### 📋 Tasks

Related topics:

- Create and Disburse Murabaha Finance (Scheduled) (IF)
- Perform Repayment (IF)
- Manage Prepayment (IF)
- Manage and Decide on Amendments (IF)
- Islamic Financing processes
- Create and Disburse Commodity Murabaha Finance (Scheduled) (IF)
- Create and Disburse Murabaha Finance (Scheduled) (IF)
- Create Commodity Murabaha Contract (IF)
- Create Murabaha Contract (IF)

The purchased asset or commodity is sold to the client for which payment is made through deferred installments and different modes of financing are available in Islamic banking.

During sale process, Islamic contract uses the Retail Lending module to create a finance contract.


##### Workflow

The user can create a new arrangement for any of the Islamic finance products listed under the profit upfront sale product group.

The following products are grouped under the profit upfront sale product group:

- Murabaha Finance
- Ijara Finance
- Commodity Murabaha Finance

| SCREENS | WORKFLOW |
|---|---|
|  | AA – Product Catalog . |
| Product Groups | In the Islamic Financing section, click the Products icon corresponding to the Profit Upfront Sale product group. |
| Products | In the Profit Upfront Sale section, click the New Arrangement icon corresponding to the Murabaha Finance or Commodity Murabaha Finance or Ijara Finance product. |
| New Arrangement(Islamic) | Enter values in the following fields: Customer Currency IS Product IS Contract Ref Effective Date Click the Validate icon to check for errors and overrides. In the Commitment section, enter a value in the Term field. In the Deferred Profit section, enter a value in the Fixed field. In the Penalty Profit section, enter a value in the Fixed field. In the Schedule section, enter values in the required fields. In the Pool ID Section, enter a value in the Pool Id field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

User can perform the disbursement either as full or in part. The disbursement can be made to a specified Legacy Account or AA Account or Internal account or it can be in cash.

During finance arrangement creations, if Active Y/N field is set with the No option in Disbursements and Other Payouts screen, then the finance arrangements will be disbursed manually.

To initiate a manual disbursement through FUNDS.TRANSFER application, perform the following steps:

1. AA Disbursement .
2. Enter values in the following fields: Arrangement Id Debit Value Date Debit Currency Debit Amount
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon.

To initiate a manual disbursement via TELLER application, perform the following steps:

1. AA Disbursement .
2. Enter values in the following fields: LCY Amount Arrangement Id Value Date Narrative
3. In the Cash Denom tab, enter a value in the Units field.
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon.

| SCREENS | WORKFLOW |
|---|---|
|  | Find Finance . |
| Find Lending Arrangements | Enter a value in the Arrangement field. Click the FIND button. |
| AA Arrangement | Click the Overview icon. |
| Arrangement Overview (Lending) | Click the New Activity option. |
| New Activities | Click the Do Activity Today icon corresponding to Change Activity for Schedule activity. |
| Arrangement Activity | In the Schedule section, amend the value in the Due Freq field for respective property field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Find Finance . |
| Find Lending Arrangements | Enter a value in the Arrangement field. Click the FIND button. |
| AA Arrangement | Click the Overview icon. |
| Arrangement Overview (Lending) | Click the Run icon corresponding to Request Payment Holiday activity. |
| Future Schedules | Click the Simulate icon. |
| Capture Activity to Simulate | Click the Validate icon to check for errors and overrides. In the Payment Holiday section, enter a value in the Number of Installments field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |
| Simulation Status | This screen displays the simulation status of the arrangement. Run the BNK/AA.SIMULATION.SERVICE Simulation Service. |

The below are the different types of Partial Payments:

- Partial Payment - Respite
- Partial Payment – Compression
- Partial Payment – Principal Decrease

To initiate a respite payment, perform the following steps:

1. AA - Respite Payment .
2. Enter values in the following fields: Customer AA Reference Installments to Pay Credit Value Date Debit Account Debit Value Date
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon.

To initiate a compression payment, perform the following steps:

1. AA - Compression Payment .
2. Enter values in the following fields: Customer AA Reference Installments to Pay Credit Value Date Debit Account Debit Value Date
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon.

To initiate a principal decrease, perform the following steps

1. AA Principal Decrease .
2. Enter values in the following fields: Arrangement Id Credit value Date Credit Currency Credit Amount Debit Account Debit Value Date
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon.

| SCREENS | WORKFLOW |
|---|---|
|  | Find Finance . |
| Find Lending Arrangements | Enter a value in the Arrangement field. Click the FIND button. |
| AA Arrangement | Click the Overview icon. |
| Arrangement Overview (Lending) | Click the Run icon corresponding to Request Payoff activity. |
| Calculate Payoff | Enter values in the following fields: Payoff Date Closure Reason Click the Validate icon to check for errors and overrides. In the Payoff Rules section, enter a value in the Expiry Days field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |
| Simulation Status | This screen displays the simulation status of the arrangement. Run the BNK/AA.SIMULATION.SERVICE simulation service. Click the Details icon for payoff statement. |

This enquiry displays the unauthorised transactions performed on finance arrangement initiated via FUNDS.TRANSFER application. The user can authorise or delete the unauthorised transactions.

To authorise an unauthorised transaction, perform the following steps:

1. Authorise/Delete Arrangements (FT) .
2. Click the Authorise icon of a corresponding record.
3. In the Authorise/Delete Funds Transfer screen, click the Authorise icon.

To delete an unauthorised transaction, perform the following steps:

1. Authorise/Delete Arrangements (FT) .
2. Click the Delete icon of a corresponding record.
3. In the Authorise/Delete Funds Transfer screen, click the Delete icon.

This enquiry displays the unauthorised transactions performed on finance arrangement initiated through Teller application. The user can authorise or delete the unauthorised transactions.

To authorise an unauthorised transaction, perform the following steps:

1. Authorise/Delete Arrangements (TT)S .
2. Click the Authorise icon of a corresponding record.
3. In the AA Loan Disbursement screen, click the Authorise icon.

To delete an unauthorised transaction, perform the following steps:

1. Authorise/Delete Arrangements (TT)S .
2. Click the Delete icon of a corresponding record.
3. In the AA Loan Disbursement screen, click the Delete icon.


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to finance arrangements.


##### Enquiries and Reports

This section allows the user to view the below list of enquiries and reports:

Finance Booked Today

This enquiry displays the list of finance arrangements booked on any given system day.

Expiring Finance

This enquiry displays the list of finance arrangements that expires in the next seven days.

Overdue Finance

This enquiry displays the list of finance arrangements for which payments are overdue.

Finance Report

This enquiry displays the complete report of finance arrangement.

Schedule

This enquiry displays the payment schedule details of the arrangement.


##### SWIFT Messages

NA


##### Advices

The below mentioned are the few sample advices:

This advice specifies the customer details, account details and principal interest details.

This advice specifies the charges and bill details for the new arrangement fee.

This advice specifies the principal decrease fee.


##### Alerts

NA


> **Related Applications:** `AA.PAYMENT.TYPE`

---


### 2.12  Islamic Contract


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Islamic Contract ( IS.CONTRACT ) application is used to purchase Islamic contracts. Islamic banking is asset based banking where the bank buys the asset and sells it to the client. The client in turn pays the bank on deferred basis.*
> 
> **Applications:** `EB.LOOKUP`, `IS.CONTRACT`, `IS.PARAMETER`, `IS.STATUS`
> 
> **Key Fields:** *Account*, *Action*, *Action Completed*, *Action Success*, *Asset Delivery Tracking*, *Asset Reference*, *Beneficiary*, *Br Fee BS Acctg* ... +78 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The Islamic Contract ( IS.CONTRACT ) application is used to purchase Islamic contracts. Islamic banking is asset based banking where the bank buys the asset and sells it to the client. The client in turn pays the bank on deferred basis.

This functionality,

- Supports the use of named or quantified assets and also controls the credit work flow for Islamic products.
- Captures the asset definition reference.
- Defaults the values in relevant fields. The vendor ID defaults the vendor account.

The user can enter the quantity of the asset for purchase along with customer settlement account. It supports definition of down payment and capturing cost related information. The accounting entries are generated based on workflow and accounting status.


##### Workflow Status

The following workflow statuses are released by Temenos as part of Model bank (MB). Additional workflow statuses are setup based on client requirement. A brief description of Temenos released Islamic workflow status is given below:

| Status | Description |
|---|---|
| Request | Asset details are auto populated from the existing named or quantified assets during Islamic contract creation. The user, Enters the required details. Captures client details, Islamic product, currency and value date details during request stage. Captures other static information specific to the asset or commodity. |
| Approval | During this stage, client and bank enters into an agreement called promise to purchase agreement Supplier or vendor details, asset costs, number of units and customer requested finance amount (for quantified assets) can be entered. Customer contribution in the project as down payment can be specified. Similarly, additional cost incurred on the asset to be purchased can be specified. This cost is paid either by the client or bank. It is possible to add the cost to the finance amount and repayment scheduled. |
| Purchase | During this stage, the asset is purchased by the bank and accounted in their books of accounts. Modifies down payment contribution and additional costs. It is possible to link multiple assets under the same purchase. |
| Down Payment | Modifies down payment contribution amount. During this stage, down payment amount can be collected automatically from the customer account or third party account. It is possible to collect down payment amount from multiple accounts. |
| Resale | During this stage, the asset is purchased from the seller and payment is made directly to the seller settlement account number. |

Islamic contract enables the user to perform the following actions:

- Update workflow status automatically during contract processing.
- Create user defined workflow status.
- Support capturing the named asset definition reference for vendor and defaults the values in the relevant fields.
- Support quantified assets for vendor and broker.
- Support the down payment functionality.
- Support capturing cost related information.
- Generate accounting entries based on workflow status.
- Support multiple assets linking to a particular contract.
- Support to capture Wakala references
- Define and account the dealer rebate
- Support sell commodity to sell broker and credit proceeds to customer account.
- Support the return commodity to buy broker or sell broker.
- Option to mark whether commodity is in the possession of the customer.


#### ⚙️ Configuration

This topic enables the user to understand the configuration for Islamic Contract.


##### UnderstandingIS.PARAMETER

This table defines the features of Islamic product. When a new Islamic parameter is created, Finance Product field is mandatory. This field displays the list of records from IS.PARAMETER table for user selection.

The following fields in IS.PARAMETER govern the asset capture functionality for named and quantified assets.

| Field Name | Description |
|---|---|
| Finance Product | Identifies the AA lending or deposit products, which can be used in Islamic contract. |
| Eligible Status for Finance | Indicates the status after which contract is eligible to enter finance stage. |
| Company | The company for which asset restriction is placed. |
| Restricted Asset | Identifies the list of assets or commodities that are restricted for a particular company. |
| Status | Defines the list of statuses in a sequential order, which defines the workflow status for the product. A work flow status generates any one of the following accounting events or it does not generate accounting entry. Allowed accounting events are: Approval Reverse Approval Purchase Resale Cost Down Payment Sell commodity to sell broker and credit customer account Return commodity Broker settlement |
| Asset Delivery Tracking | Enables delivery tracking for assets. |


##### Configuring Workflow Status

The workflow status defines the product workflow. Banks can define credit work flow status records in EB.LOOKUP table with IS.WF.STATUS as prefix.

IS.WF.STATUS*REQUEST. Here, REQUEST is a workflow status.

PRODUCT), status defined in IS.PARAMETER table is auto populated at the time of contract input. The order of the status in IS.PARAMETER table defines the contract workflow status. Status movement (to the next status) happens automatically during authorisation of the previous stage. New workflow status is defined in EB.LOOKUP table. Accounting entries for the defined workflow status is configured in IS.STATUS . It is not required to define all the workflow status belongs to the product in IS.PARAMETER .

In commodity Murabaha, based upon the customer request, the bank purchases commodity from buy broker. This commodity is then handed over to the customer after booking finance contract. Customer then directs the bank to sell the commodity and credit the proceeds to his account. Bank can setup purchase, sell commodity to sell broker and credit proceeds to customer account and broker settlement as part of the general workflow.

It is also possible that the customer changes his mind and not willing to go ahead with his request. In that case, the commodity needs to return to the Broker by Bank. It is exceptional workflow, need not be setup in the generic workflow, and can handle as part of the transaction.


#### 📋 Tasks

Related topics:

- Manage Vendor (IF)
- Manage Reviewer (IF)
- Manage Broker (IF)
- Create Murabaha Contract (IF)
- Create Commodity Murabaha Contract (IF)
- Islamic Financing processes
- Perform Commodity Murabaha Contract Status Change (IF)
- Perform Murabaha Contract Status Change (IF)

Islamic Contract ( IS.CONTRACT ) application is used to create contracts for named assets or quantified assets and controls the credit work flow for Islamic products.


##### Workflow

This section allows the user to perform the below tasks:

| SCREENS | WORKFLOW |
|---|---|
|  | Vendor Setup . |
| Vendors | Click the Input New Vendor icon. |
| Vendor Setup | Ensure the record id of this screen is an existing customer record. Enter values in the following fields: Name Status Company Currency Account Beneficiary Commodity Rebate Currency Default Rebate Type Default Rebate Value Start Date Rebate Type Rebate Value End Date Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

| SCREENS | WORKFLOW |
|---|---|
|  | Reviewer Setup . |
| List of Reviewers | Click the Input New Reviewer icon. |
| Reviewer Setup | Ensure the record id of this screen is an existing customer record. Enter values in the following fields: Name Status Reviewer Type Company Currency Account Beneficiary Comments abt Reviewer Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

| SCREENS | WORKFLOW |
|---|---|
|  | Broker Setup . |
| Brokers | Click the Input New Broker icon. |
| Broker Setup | Ensure the record id of this screen is an existing customer record. Enter values in the following fields: Name Status Broker Type Br Settle Wash Categ Company Currency Broker Acct Beneficiary Br Fee Type Br Fee Currency Br Fee Settlement Br Fee Share Perc Br Fee Tax Base Amt Br Fee Wash Categ Br Fee Pay Frequency Br Last Payment Date Move to History Days Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

| SCREENS | WORKFLOW |
|---|---|
|  | New Contract – Named Asset . |
| Input Contract | Enter value in the Commodity or Customer field and click the FIND button. Click the Create Contract icon corresponding to a record. |
| Input New contract | Enter values in the required fields: Customer IS Product Status Value Date Currency Value Date GB Asset Description Commodity Asset Reference Vendor Vendor Name Units Unit Price Purchase Quantity Customer Account Units Equivalent of Purchase Simulation Reference Seller Customer ID Seller Customer Name Seller Settlement Ac In the Down Payment tab, enter values in the following fields: Down Payment Commodity Down Pay Asset ref Down Payment type Down Payment Amount Down Payment Account Down Payment Rec Amount Down Pay Percentage Contribution Type Contribution Counterparty Contribution Amount In the Rebate tab, enter values in the following fields: Rebate Allowed Rebate Action In the Wakala Reference tab, enter values in the following fields: Wakala Finance Ref In the Cost tab, enter values in the following fields: Cost Type Cost Payment Type Cost Amount Cost Debit Account Cost Credit Account Description abt the Cost In the Action tab, enter values in the following fields: Action Action Completed Action Success Notes Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

| SCREENS | WORKFLOW |
|---|---|
|  | New Contract – Quantified Asset – Vendor . |
| Commodities with Quantified Assets | Click the Create Contract icon. |
| Input New Contract | Enter values in the following fields: Customer IS Product Status Value Date Currency Value Date GB Asset Description Request Amount Commodity Asset Reference Vendor Vendor Name Units Unit Price Purchase Quantity Customer Account Units Equivalent of Purchase Simulation Reference In the Down Payment tab, enter values in the following fields: Down Payment Commodity Down Pay Asset ref Down Payment type Down Payment Amount Down Payment Account Down Payment Rec Amount Down Pay Percentage Contribution Type Contribution Counterparty Contribution Amount In the Cost tab, enter values in the following fields: Cost Type Cost Payment Type Cost Amount Cost Debit Account Cost Credit Account Description abt the Cost In the Action tab, enter values in the following fields: Action Action Completed Action Success Notes Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

| SCREENS | WORKFLOW |
|---|---|
|  | New Contract – Quantified Asset – Broker . |
| Commodities with Quantified Assets | Click the Create Contract icon. |
| Input New Contract | Enter values in the following fields: Customer IS Product Status Value Date Currency Value Date GB Asset Description Request Amount Commodity Asset Reference Buy Broker Buy Broker Acct Buy Broker Wash Acct Sell Broker Sell Broker Acct Sell Broker Wash Acct Units Unit Price Purchase Quantity Customer Account Simulation Reference In the Down Payment tab, enter values in the following fields: Down Payment Commodity Down Pay Asset ref Down Payment type Down Payment Amount Down Payment Account Down Payment Rec Amount Down Pay Percentage Contribution Type Contribution Counterparty Contribution Amount In the Broker Fee Details tab, enter values in the following fields: Br Fee Debit Type Br Fee BS Acctg Br Fee BS Cr Acct In the Cost tab, enter values in the following fields: Cost Type Cost Payment Type Cost Amount Cost Debit Account Cost Credit Account Description abt the Cost In the Action tab, enter values in the following fields: Action Action Completed Action Success Notes Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

| SCREENS | WORKFLOW |
|---|---|
|  | Amend Unauthorised Contracts . |
| Amend Unauthorised Records | Click the Update icon. |
| Amend Contract | Enter values in the fields which require amendment. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

| SCREENS | WORKFLOW |
|---|---|
|  | Workflow change / Modification of Contract . |
| Amend Contract | Click the Next Action icon. |
| Next Action | Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

| SCREENS | WORKFLOW |
|---|---|
|  | Sell Comm and Cr Cust Ac / Return Commodity . |
| Amend Contract | Click the Amend Status icon. |
| Amend Status of Contract | Enter the values in the following fields which are to be amended: Status set as Return Commodity Return Unit Price Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

| SCREENS | WORKFLOW |
|---|---|
|  | Authorise/Delete/View Contract . |
| Unauthorised Contracts | Enter a value in the Contract Reference or Customer field and then click the FIND button. |
| Unauthorised Transaction | Click the Authorise icon. |
| Authorise/Delete/View Contract | Click the Authorise icon. |


#### 📊 Outputs

The user can view the below list of enquiries related to Islamic contracts in the core banking system.


##### Enquiries and Reports

This section allows the user to view the below enquiries and reports:

List of Contracts

This enquiry displays the list of Islamic Contracts created in the system.

Contractwise Customer Position

This enquiry displays the list of the customer position with respect to the number of units in hand after the Purchase of Asset.

Commodity Limit Details

This enquiry displays the commodity limits for a particular Commodity and Date.

Broker Fee Details

This enquiry displays the reconciliation for Broker share of Broker Fee.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA


> **Related Applications:** `EB.LOOKUP`, `IS.CONTRACT`, `IS.PARAMETER`, `IS.STATUS`

---


### 2.13  IslamicSyndicateFinance


> **📇 Quick Reference Card**
> 
> **Purpose:** *Islamic Syndicate Finance is a mode of Islamic finance where a group of financial institutions offer finance to a single borrower. Under the syndication structure, one of the banks acts as the lead bank and manages the finance on behalf of the other investors. Islamic syndicate finance is like the c...*
> 
> **Key Fields:** *Amount*, *Arrangement*, *Currency*, *Customer*, *Effective*, *Effective Date*, *Fixed*, *IS Contract Ref* ... +5 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Islamic Syndicate Finance is a mode of Islamic finance where a group of financial institutions offer finance to a single borrower. Under the syndication structure, one of the banks acts as the lead bank and manages the finance on behalf of the other investors. Islamic syndicate finance is like the conventional one except that it uses the structures accepted by Sharia principles.

Islamic syndication plays a significant role in buying assets which require huge investments that cannot be handled by a single bank. In Islamic syndicate finance profit or loss is borne by all the investors.

Key Islamic finance structures in syndication are:

- Murabaha Syndication: A cost-plus-profit structure where the lead bank buys an asset and sells it to the borrower at a marked-up price. Syndication allows multiple banks to contribute to the financing of the asset.
- Ijara Syndication: Here the banks jointly provide funding for the purchase of an asset. The borrower leases the asset back with payments structured according to the agreed terms.


##### Bank Roles

In syndicate finance, the concept of upfront profit refers to the calculation of profit amount during creation of a syndicate finance arrangement. These profits can be allocated among the different roles that the banks play in the arrangement, which include:

1. Participating Agent In an Islamic syndication, when a lead bank functions as an Agent cum Participant, it combines the dual role of managing the syndication while also contributing funds to the pool of financing. This hybrid role is a distinctive feature in some large syndicated Islamic finance transactions. As an agent, the bank takes on the responsibility of managing the syndicate, structuring the financing, monitoring the transaction, and acting as the central point of contact for communication between the borrower and the syndicate members. In addition to these management duties, the lead bank also takes on the role of a Participant. It contributes a portion of the financing itself, alongside other members of the syndicate. Apart from the key activities as an agent, the Participating agent is involved in below key activities: Participating in the Financing - The lead bank contributes funds to the syndication along with the other syndicate members. It shares the financial risk of the syndication in proportion to its contribution, alongside other participant. Advantages for the Lead bank acting as an Agent cum Participant: Aligned Interests - By contributing to the financing, this role ensures that the interests are aligned with the other syndicate members. This can enhance trust and cooperation among the parties involved, as the Lead bank shares in the risks and rewards of the financing. Expertise and Control - In this role, the Lead Bank typically brings significant expertise to the transaction. It has a strong understanding of the financial structure, Sharia compliance, and the operational details to manage the syndicate. By taking on this dual role, the Lead bank maintains a central position of control while ensuring that its financial stake in the deal gives a vested interest in the success of the project. Market Confidence - The involvement of the Lead bank as a Participant can instill confidence in other banks and investors in the syndicate, as it demonstrates the bank’s commitment to the success of the transaction. This may make it easier to attract other participants to join the syndicate. Risk Sharing - The Lead bank sharing in the financing alongside other participants helps distribute the risk more evenly among all parties. It ensures that the bank does not carry all the financial exposure and reduces its risk profile in large syndications.
2. Agent The lead bank is the primary party responsible for organising and managing the syndication process. In Islamic syndicate finance, the lead bank as Agent has expertise in structuring Sharia-compliant financing arrangements. Agent often takes on the largest portion as fee due to its comprehensive responsibilities. As the agent bank, the lead bank acts as the primary point of contact for all communication between the borrower and the syndicate members. It is responsible for distributing funds, receiving payments from the borrower, and then distributing it to the other syndicate members in accordance with their share of participation in financing. The lead bank is involved in several key activities: Structuring the Financing - The lead bank works to structure the financing according to Sharia principles, using Islamic finance products such as Murabaha and Ijara. Syndication - The lead bank initiates the syndication process by reaching out to potential syndicate participants, who are other Islamic banks or financial institutions. Documentation - The lead bank ensures that all necessary legal documentation with sharia-compliance is in place. This includes the Syndication Agreement and other documents like Facility Agreements, Murabaha and Ijara agreements. These contracts outline the terms and conditions, obligations, and rights of each participant in the syndicate and provide guidance on how disputes can be resolved according to Islamic principles. Monitoring and Reporting - After the syndication is finalised, and funds are disbursed, the lead bank assumes the role of ongoing monitoring of the project’s progress, financial status, and compliance with the agreed-upon terms. It also handles the reporting and communication between the borrower and the syndicate members.
3. Participant In an Islamic syndication, a Participant bank refers to a financial institution that joins the syndicate to contribute capital to the financing pool. It does not take on the primary organisational or management roles. The Participant bank's role is limited to providing funds in exchange for a share of the profits or returns generated by the Islamic financing transaction, with Sharia compliance. Key activities of participant bank are: Capital Contribution - The Participant bank contributes a portion of the total funding required for the transaction. This funding is pooled with contributions from other participating banks, including the lead bank. The share of the Participant Bank in the financing is proportional to its investment, and its share of profits or returns is also based on the amount contributed. Risk Sharing - The Participant bank shares the risks and rewards of the financing according to its contribution. This means the Participant bank receives a portion of the profits in Murabaha, Ijara structures. It also assumes the financial risks if the borrower defaults or the project fails. Documentation - The Participant bank signs the syndication agreements and other legal documents. It is bound by the terms of the Syndication agreement and other related contracts. These agreements detail participants' rights, responsibilities, and obligations in relation to the financing

The agent’s fee can vary depending on the role the agent plays in the syndication. As per Islamic finance principles, the agent in a syndicate finance is compensated through two distinct types of fees. Both fees can be negotiated and agreed upon at the outset of the deal, depending on the role the agent is expected to play in managing the facility.

Mudarib Fee

The Mudarib role comes from the concept of Mudaraba in Islamic finance. Mudaraba is a partnership in which one party provides capital (the Rab al-Maal) and the other party (the Mudarib) provides expertise and management in conducting a business or investment. This is a performance-based fee, compensating the agent for successfully managing the syndicate agreement and ensuring the objectives are met. This fee is linked to the success of the finance and calculated as a percentage of any profits generated.

Wakeel Fee

The Wakeel role comes from the concept of Wakala (agent) in Islamic finance. It refers to an agency agreement where one party (the Wakeel) is appointed to act on behalf of another party (the principal) to carry out specific tasks or services. This fee compensates the Wakeel for its administrative and managerial duties that are critical in ensuring the smooth operation of the syndicate and the Sharia-compliant nature of the transaction. This is collected from both borrowers and investors as a predetermined amount. This is collected upfront and not dependent on facility's profitability.


#### ⚙️ Configuration

This section enables the user to understand the configuration for Islamic Syndicate Finance. Apart from IS and AL, PRTPNT, and other modules licenses are required to enable the syndicate financing.


##### Participant Property Class

The Participant Property Class is used to include multiple participants in an Islamic syndicate facility and drawing. In an Islamic Syndicate finance arrangement, the bank can take on different roles, such as Agent, Participating Agent, and Participant. Participant details are captured at the facility level and are defaulted in the drawing arrangement. These details cannot be modified at the drawing level. While most participant details are captured at the arrangement level, only a few specific attributes can be input at the product level. All other Participant property class attributes are not allowed for input at the product level.

When the Participant property class is linked to a facility or finance product, the Balance Treatment attribute in the Account property class must be set to Participation. Participant accounting is raised based on this configuration for different own bank roles. If this is not configured, the system triggers an error at the arrangement creation level. The accounting entries generated are determined based on two key criteria:

1. Role of the Agent Bank The role of the owning bank in the system is defined within the Participant property class at arrangement level. Based on this, if the agent bank’s role is: Agent - Then no accounting entries for commitment are required for the bank. Only accounting entries related to fees and charges are generated. Participating Agent - Then non-contingent accounting entries are generated for the bank. The customer balances are always treated as memo balances, which are maintained under balance types with the ‘PARTINF’ suffix.
2. Participation Accounting Type The participant balances are categorised based on the Participation Accounting Type, which can either be: Memo - The participant balances are maintained as memo balances, identified with the ‘PARTINF’ suffix. Contingent - The participant balances are maintained as contingent balances, marked with the ‘PART’ suffix, and are reported as contingent liabilities in the off-balance sheet general ledger.

- Lead Bank as a Wakeel – The lead bank receives the agency fees for administrating the syndicate finance. This is collected as a flat fee and is configured as a fixed type of charge. It is only possible to configure the collection of fees from the customer and not from the participants. This fee is applicable for the bank roles as Agent and Participating Agent.
- Lead Bank as a Mudarib – The agent bank receives agency fees as percentage of the Participants’ profits for this role. Any loss is solely borne by the participating banks. This charge is calculated on the profit generated out of the syndication finance. This needs to be handled outside the system as the fee to be calculated on the profit generated by each participant. Wakeel fee is collected as a fixed amount and configured as ‘Agent Fee’ at the Finance level. Mudarib fee is collected as a percentage of Profit from the Participants. This is to be handled separately outside Transact as collecting fee from participants is not enabled.

Read this Working with Upfront Profit in Club Finance for more details on Upfront profit in Syndicate Finance.


#### 🔧 Working With

Islamic Syndication in Transact is supported for both:

- Profit upfront products, where the profit amount is calculated upfront.
- Profit accrual products, where the profit is accrued throughout the life of the arrangement.

The accounting entries for the Islamic syndicate finance are raised based on the configuration of below attributes in the Participant property class:

1. Participant Accounting type - Decides whether the accounting must be raised as memo or contingent
2. Own Bank Role defined - Entries are raised based on the roles as Agent, Agent cum Participant and Participant
3. Profit Method set as Fixed in Profit PC (For Syndicate Murabaha finance) - The system raises upfront profit receivable entries for the drawings created under the facility.


##### Workflow - Own Bank as Participating Agent

As a lead bank, Transact is responsible for organising and managing the syndication process. As the agent bank, the lead bank acts as the primary point of contact for all communication between the borrower and the syndicate members. It is responsible for distributing funds, receiving payments from the borrower, and then distributing it to the other syndicate members in accordance with their share of participation in financing. Accounting entries are raised as real entries for the own bank portion and info entries for the participants. In case of Syndicate Murabaha finance, receivable entries are raised upfront for the profit portion of the finance.

The user can create an Islamic syndicate facility by capturing the commitment amount and the participant details. Balance Treatment in Account property class must be configured as Participation to enable participant accounting for Islamic Syndicate Facility. It is mandatory to capture the beneficiary details of the participating banks to enable transferring money to and from the participating banks.

The screenshot below shows an Islamic syndicate facility, where the Transact bank acts as Agent cum Participant. The commitment amount is shared by the own bank and two participating banks in 40, 40 and 20 ratios.

The commitment entries raised for the above Facility arrangement has three different types of balances.

- Customer Balances - For information purpose and are single leg entries. It stores all the balance types with INF suffix. These entries are raised for the entire commitment amount and utilised when drawings are created under a facility.
- Own Book Balances - Show the real statement entries for an Islamic syndicate facility arrangement. It stores the balances related to the own bank’s share. It is recorded in the bank’s accounting books.
- Participant Balances - It is necessary for the agent bank to record the share percentage or amount and balances of the participants to ensure smooth processing of syndicate arrangement. The participant balances can either be stored as just an informational memo or as contingent balances, based on Accounting Type attribute in the Participant property class. As the Account Type is configured as Memo in the below enquiry, the participant balances are updated with a PARTINF suffix.

When the own bank acts as an Agent cum Participant, the asset is procured using Islamic workflow configuration. Asset request is initiated where the user can enter the specifications of the asset and the vendor details. Once the asset request is created and authorised, an Islamic contract is created to capture details of the number of assets to be purchased, customer account details, down payment amount, any additional costs, asset review fee, and so on.

Workflow for a specific Syndicate Finance (Syndicate Ijara and Syndicate Murabaha) is parameterised in the system and the workflow steps must be completed before creating a Finance arrangement using AA.

The screenshot below shows the Islamic contract for Syndicate Ijara (IS Product 14) is created and marked as purchased in the system.


###### Syndicate Ijara Finance

The user can create a Syndicate Ijara finance using the New Drawings option in Facility overview screen. Only the finance products configured under Sub arrangement rules property class of the Facility product can be created using this option. Syndicate Ijara finance can also be created as a standalone finance without a facility.

While creating a Syndicate Ijara drawing under a Facility, the system defaults the facility reference in the finance arrangement creation screen. The user must enter the Islamic product reference and Islamic contract reference when the syndication is managed by the own bank (Agent bank). Creation of asset request, asset purchase is not expected if the bank role is Participant.

The system defaults the Participant details from Islamic syndicate facility arrangement. The system also defaults the commitment amount with the asset price and settlement account for disbursement with multi-supplier wash account. If the customer account is provided at the time of creating asset purchase, then the system defaults the settlement account for repayments and fees. The user can capture the Term, profit rate and agent fee if applicable to create the Syndicate Ijara finance arrangement.

The screenshot below shows the Syndicate Ijara finance overview which has the facility linked to it. The drawings created under a Facility are shown in the Facility overview screen as well.

Accounting entries are raised as below for Syndicate Ijara finance. The system raises:

- Own book balance as info entries.
- Customer balances as real entries as the bank acts as agent cum participant.
- Participant balances with a PARTINF suffix.

UTL balances are raised for the utilised balance of the finance, and this is based on the configuration in Term Amount property class.


###### Syndicate Murabaha Finance

In Syndicate Murabaha finance, the agent bank buys the asset and sells it the customer at a cost-plus-profit price. Members of the syndication shares the asset purchase price and the corresponding profit amount. As the profit amount is decided and agreed upfront, the system raises receivable entries for a Syndicate Murabaha finance. For a Murabaha contract with the same asset price and term, below accounting entries are generated.

For the finance amount USD 200,000, the agreed profit is USD 101,472.22. In this, 50% of the profit is for the agent bank and 30% for Participating bank1 and 20% for the Participating bank2. The profit amount calculated upfront is split among the participants based on their participation.

Read Working with Upfront Profit in Club Finance for more details on Upfront profit in Syndicate Finance.


##### Workflow - Own bank as Agent

As a lead bank, Transact is responsible for organising and managing the syndication process. As the agent bank, the lead bank acts as the primary point of contact for all communication between the borrower and the syndicate members. It is responsible for distributing funds, receiving payments from the borrower, and then distributing it to the other syndicate members in accordance with their share of participation in financing. Accounting entries are raised as info entries for the own bank portion and info entries for the participants. In case of Syndicate Murabaha finance, the receivable entries are raised upfront for the profit portion of the finance.

The user can create a Islamic Syndicate Facility by capturing the commitment amount and the participant details. Balance Treatment in the Account property class has to be configured as Participation to enable participant accounting for Islamic Syndicate Facility. It is mandatory to capture the beneficiary details of the participating banks to enable money transfer to and from the participating banks.

The screenshot below shows an Islamic syndicate facility, where the Transact bank acts as 'Agent'. The commitment amount is shared by two participating banks in 60, and 40 ratios.

When the own bank acts as an Agent, the asset is procured using Islamic workflow configuration. Asset request is initiated where the user can enter the specifications of the asset and the vendor details. Once the asset request is created and authorised, an Islamic contract is created to capture details of the number of assets to be purchased, customer account details, down payment amount, any additional costs, asset review fee, and so on. Workflow for a specific Syndicate Finance (Syndicate Ijara and Syndicate Murabaha) are parameterised in the system and the workflow steps to be completed before creating a Finance arrangement using AA.


###### Syndicate Ijara finance

Syndicate Ijara finance can be created under the Facility with the IS contract reference.

Accounting entries for the Syndicate Ijara Finance with Bank role as 'Agent' is generated as below. The system raises:

- Own book balance as info entries.
- Customer balances are not raised (except for Fee), As the Bank acts only as an agent and not invest in the syndication.
- Participant balances with a PARTINF suffix.


###### Syndicate Murabaha Finance

For a Syndicate Murabaha finance with Bank role as Agent, upfront profit entries are generated for the profit portion, and it is split into customer and participant balances.

Read Working with Upfront Profit in Club Finance for more details on Upfront profit in Syndicate Finance.


##### Workflow - Own Bank as Participant

As a participant bank, Transact joins the syndicate to contribute capital to the financing pool. It does not take on the primary organisational or management roles. This syndication is managed by another bank. The participant bank's role is limited to providing funds in exchange for a share of the profits or returns generated by the Islamic financing transaction.

The user can create an Islamic Syndicate Facility by capturing the commitment amount and own bank amount. Participant details need not be input. It is mandatory to capture the beneficiary details of the agent bank to enable money transfer to and from the agent bank.

The screenshot below shows an Islamic syndicate facility, where the Transact bank acts as 'Participant'.

When the Transact bank acts as Participant, the asset purchase is handled by the agent bank. Creation of asset purchase and Islamic contract workflow is not required for this role. Syndicate finance arrangements can be created without the Islamic contract reference.


###### Syndicate Ijara Finance

As the bank acts as participant, the system allows the user to create a syndicate finance without the Islamic contract reference. In this case, the finance amount is disbursed to the agent bank using beneficiary details captured at the time of finance or facility creation. Payment schedule is updated with disbursement schedule and settlement instructions for Payout is set as Yes without an account number/DD/Beneficiary reference. The system triggers the LENDING-APPLYPAYMENT-PO.WITHDRAWAL activity to disburse the amount and update the finance status as current. Agent fee is not applicable for the 'Participant' role.

Accounting entries are raised as below for the Syndicate Ijara finance for the 'Participant' role. Real entries are raised for the own bank.


###### Syndicate Murabaha Finance

Similar workflow is followed for Murabaha finance where the system raises receivable entries for the profit portion of the finance.

Read Working with Upfront Profit in Club Finance for more details on Upfront profit in Syndicate Finance.


###### Rebate on Payoff

In a Murabaha finance, a rebate refers to a reduction in the total profit amount to be repaid if the total finance amount is settled before the maturity date. It is given to the borrowers to provide them benefit of paying the fixed markup (profit margin) agreed at the beginning of the contract earlier than the scheduled maturity date. This rebate is usually calculated as a portion of the remaining profit. When the customer initiates early closure of an upfront profit finance, a certain amount can be rebated as part of the early payoff.

This is configured in the Profit product condition and calculated when early payoff activity is triggered. There are few options available on how this rebate is provided to the customer.

- Effective date – The accrued profit till the effective date is collected from the customer, the remaining receivable profit is given up as rebate.
- Period end date – The accrued profit till the current payment period is collected from the customer, remaining receivable profit is given up as rebate.
- Payment end date – The accrued profit till the Maturity date is collected from the customer, no rebate is given to the customer.
- Context – During the rebate activity, the bank user gives the amount that should be collected from the borrower. The remaining upfront profit amount is given up as rebate.
- Percentage – Certain percentage of receivable profit is rebated back to the customer during early closure.


###### Split, Merge and Rollover

In a profit accrual finance under a deal or facility, can be rolled over and repriced multiple times in synchronous with the profit periods. When transitioning into a contract with new terms and conditions, the workflow is like creating a new drawing. The new arrangement can be set up either as an offer or directly as an agreement. The terms and conditions, profit rate, and other details are established in advance.

A corporate borrower may make multiple drawdowns under a commitment. These drawdowns can be consolidated into one or divided into several, depending on the borrower's request. During the split or merger process, any unamortised upfront fee from the original drawdowns, held in a suspense account, is transferred to the newly created drawing on a pro-rata basis. This transfer of the fee impacts the cash flow of the drawings involved. If the facility commitment is not fully utilised, the upfront fee is recognized in the profit and loss statement upon the facility's expiration or maturity.


###### Share Transfer

The Share Transfer Transaction class is used to transfer a participants share percentage to another participant. This can be initiated from arrangement overview and the transfer is possible to a new or an existing participant of the Syndicate Finance. When the buyer is a new participant and not an existing participant in the contract, then the user should update the role of the buyer under the Participant Role field and his beneficiary details in the Settlement Instructions tab as part of the share transfer activity.


#### 📋 Tasks

Islamic Syndicate Finance is a mode of Islamic finance where a group of financial institutions offer finance to a single borrower. Under the syndication structure, one of the banks acts as the lead bank and manages the finance on behalf of the other investors. Islamic syndicate finance is like the conventional one except that it uses the structures accepted by Sharia principles.


##### Workflow

This section allows the user to perform the below activities:

| SCREENS | WORKFLOW |
|---|---|
|  | AA – Product Catalog . |
| Product Group | Islamic Syndicate Facility . Click the Products icon corresponding to the Islamic Syndicate Facility product group. |
| Products | In the Islamic facility product screen, click the New Arrangement icon corresponding to the Islamic Syndicate Facility product. |
| New Arrangement (Islamic) | Enter values in the following fields: Customer Currency Effective Date Click the Validate icon to check for errors and overrides. In the Commitment section, enter values in the following fields: Amount Term In the Schedule section, enter values in the required fields. In the Pool ID section, enter a value in the Pool Id field. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
|  | Find Facility . |
| Product Group | Enter the Facility ID and click the Overview Icon corresponding to the respective Facility. Click the New Drawing icon from the Overview screen. |
| Products | In the Islamic facility product screen, click the New Arrangement icon corresponding to the Syndicate Murabaha drawings product. |
| New Arrangement (Islamic) | Enter values in the following fields: Customer IS Contract Ref Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. In the Commitment section, enter values in the following fields: Amount Term In the Principal Profit Details section, enter values in the following fields: Fixed (expected profit rate) In the Schedule section, enter values in the required fields. In the Pool ID section, enter a value in the Pool Id field. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
|  | AA – Product Catalog . |
| Product Group | Islamic Syndicate Finance . Click the Products icon corresponding to the Syndicate Murabaha Drawings product group. |
| Products | Click the New Arrangement icon corresponding to the Syndicate Murabaha finance product. |
| New Arrangement (Islamic) | Enter values in the following fields: Customer Currency IS Contract Ref Effective IS Product Click the Validate icon to check for errors and overrides. In the Commitment section, enter values in the following fields: Amount Term In the Principal Profit Details section, enter values in the following fields: Fixed (expected profit rate) In the Schedule section, enter values in the required fields. In the Pool ID section, enter a value in the Pool Id field. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
|  | Find Facility . |
| Product Group | Click the Overview Icon corresponding to the respective Facility. Click the New Drawing icon from the Overview screen. |
| Products | In the Islamic facility product screen, click the New Arrangement icon corresponding to the Syndicate Ijara drawings product. |
| New Arrangement (Islamic) | Enter values in the following fields: Customer IS Contract Ref IS Product Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. In the Commitment section, enter values in the following fields: Amount Term In the Principal Profit Details section, enter values in the following fields: Fixed (expected profit rate) In the Schedule section, enter values in the required fields. In the Pool ID section, enter a value in the Pool Id field. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
|  | AA – Product Catalog . |
| Product Group | Islamic Syndicate Finance . Click the Products icon corresponding to the Islamic Syndicate Finance product group. |
| Products | Click the New Arrangement icon corresponding to the Syndicate Ijara finance product. |
| New Arrangement (Islamic) | Enter values in the following fields: Customer Currency IS Contract Ref Effective IS Product Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. In the Principal Profit Details section, enter values in the following fields: Fixed (expected profit rate) In the Schedule section, enter values in the required fields. In the Pool ID section, enter a value in the Pool Id field. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Find Facility Arrangements | Enter facility arrangement ID in the Arrangement field and then click the FIND button. Click the Overview icon corresponding to the record. |
| Arrangement Overview (Facility) | Click the Share Transfer Simulation option corresponding to the participant. |
| Share Transfer Simulation | In the Share Transfer tab, enter the values in the required fields. When share transfer is made to a new participant, in the settlement instructions, enter values in the required fields. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Find Facility Arrangements | Enter facility arrangement ID in the Arrangement field and then click the FIND button. Click the Overview icon corresponding to the record. |
| Arrangement Overview (Facility) | Click the Share Transfer Simulation option corresponding to the participant. |
| Share Transfer Simulation | In the Share Transfer tab, enter the values in the required fields. When share transfer is made to a new participant, in the settlement instructions, enter values in the required fields. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Authorised | Enter facility arrangement ID in the Arrangement field and then click the FIND button. Click the Overview icon corresponding to the record. |
| Arrangement Overview (Facility) | Click the New Activity option. |
| New Activities | Click the Do Activity Today icon corresponding to Capture Merge or Split. |
| Split & Merges Rollover | Select a value in the Rollover Type field as required. Enter values in the required fields according to the option chosen under Rollover Type . Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. Accept the overrides, if any. Run the BNK/AA.SPLITS.MERGES service. |


#### 📊 Outputs

There are no Outputs available for Islamic Syndicate Finance.

---


### 2.14  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *Islamic banking refers to a system of banking or banking activity that is consistent with the principles of the Shari'ah (Islamic rulings) and its practical application through the development of Islamic economics. It started during the late 20th century when a number of Islamic banks were formed to...*
> 
> **Applications:** `AA.PRODUCT.DESIGNER`, `AA.PRODUCT.GROUP`, `AA.PRODUCT.LINE`, `AA.PROPERTY`, `AA.PROPERTY.CLASS`, `IS.ASSET.REVIEW`, `IS.BROKER`, `IS.COMMODITY` ... +15 more
> 
> **Key Fields:** *Status*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- Temenos Transact Services

Islamic banking refers to a system of banking or banking activity that is consistent with the principles of the Shari'ah (Islamic rulings) and its practical application through the development of Islamic economics. It started during the late 20th century when a number of Islamic banks were formed to provide an alternative banking system. Islamic banking has the same purpose as conventional banking except that it operates in accordance with the rules of Shari’ah.

Shari'ah prohibits payment or acceptance of interest charges (riba) for lending and accepting money, as well as carrying out trade and other activities that provide goods or services considered contrary to its principles. To ensure adherence to these underlying Islamic principles, most Islamic banks have a Shari'ah board comprising Islamic scholars that scrutinises proposed transactions and maintains an overall review of the bank’s Islamic financing methods and operations

The following are the basic concepts of Islamic banking:

- Interest – Cannot be charged for the mere use of money. Islamic financial institutions must trade in real assets or services.
- Uncertainty – Does not allow any contract based occurrence or non-occurrence of a future uncertain event.
- Speculation or gambling – Does not allow trading or investment transactions, which involve the risk of incurring losses as well as earning profits.
- Prohibited activities or commodities – Does not finance enterprises involved in, Financial services (Interest-based) Gambling Alcoholic liquor
- Mobilisation of funds – Does not mobilise funds by paying interest to their depositors.

| Work-flow Stages | Description |
|---|---|
| Asset Request | Asset request is used for maintaining asset inventory to be sold based on requirement. This request is made, when there is a requirement from the customer or client. Asset can be classified into: Named ( for example, vehicle, machinery, equipment) Quantified (for example, agricultural produce, minerals) During this stage the below details are captured: Client Supplier Vendor/Resale Customer ID, Resale Customer Name, Resale Settle Account Asset cost and number of units Currency Other static information specific to the asset |
| Asset Approval | During this stage, the agreement of promise to purchase is entered into between the client and the bank. Specifies customer contribution in the project as down payment. Specifies any additional cost incurred on the asset to be purchased. This cost can paid either by the client or bank. Adds the cost to the finance amount and repayment scheduled. |
| Asset Purchase | During this stage, the asset is purchased by the bank and accounted in their books of accounts. Down payment contribution and additional costs can be modified. It is possible to link multiple assets under the same purchase. |
| Payment Management | Vendor payments, payment to cost counterparty, reviewer payments, broker payments (for treasury transactions) are made. Payments are consolidated vendor wise and can be made ad-hoc or scheduled. A certain percentage of the payment can be retained by the bank and paid subsequently as retention amount payment. |
| Sale or Finance | The purchased asset is sold to the client for which the payment is made as deferred installments. In a lease (Ijara) contract where the client is a lessee, lease rentals are paid to the bank. The modes of financing in Islamic banking are defined as different products, such as Murabaha, Musharaka, Ijara, Istisna, Salam, Mudaraba, and Wakala. |

| Finance Products | Groups |
|---|---|
| Profit Upfront Sale | Murabaha finance Ijara finance (service Ijara – Murabaha based) Commodity Murabaha finance |
| Profit Accrual Sale | Forward Ijara finance Qard Hassan finance (profit free finance) Diminishing Musharaka finance Bai Salam finance Construction finance Mudaraba financing |
| Multi-structured Products | Musawama finance Wakala finance |


##### Configuring Islamic Banking

This section orients the user on asset purchase and finance management related activities. Asset management comprises of,

- Asset creation
- Asset purchase
- Asset tracking or delivery
- Asset review and payment activities
- Finance management activities

| Application Name | Description |
|---|---|
| Asset Capture | Used to create, Asset or inventory. Own application tables to capture asset specifications. For example, IS.VEHICLE IS.REALESTATE IS.EQUIPMENT IS.MOVEQUIPMENT IS.MISCASSET |
| IS.CONTRACT | Used to, Purchase assets. Control credit workflow for Islamic assets. Define flexible workflow status based on requirements Raise flexible accounting entries based on defined workflow status. |
| IS.CONTRACT.DELIVERY | Used to track the delivery of commodities or assets. |
| IS.COMMODITY.SALE | Used to sell the delivered commodities to clients either partially or fully. |
| IS.ASSET.REVIEW | Used to manage the review activities for assets |
| IS.PAYMENT | Used to manage Islamic banking payment activities. |

| Column 1 | Column 2 | Column 3 |
|---|---|---|
| ACCOUNT ACCOUNTING ACTIVITY.API ACTIVITY.CHARGES ACTIVITY.MAPPING ACTIVITY.MESSAGING ACTIVITY.PRESENTATION ACTIVITY.RESTRICTION ALERTS AGENT COMMISSION BALANCE.MAINTENANCE | CHANGE.PRODUCT CHARGE CHARGE.OVERRIDE CHARGEOFF CLOSURE CONSTRAINT CUSTOMER ELIGIBILITY INTEREST LIMIT OFFICERS OVERDUE | PAYMENT.RULES PAYMENT.SCHEDULE PAYOFF PAYOUT.RULES PERIODIC.CHARGES PRICING.RULES REPORTING SETTLEMENT TERM.AMOUNT STATEMENT TAX XIS.POOLID XIS.FACILITY XIS.DRAWING XIS.FINANCE |


##### Illustrating Model Parameters

Parameter files and system tables need to be setup to support the Islamic banking operations. This section provides a brief overview of the system and parameter setup for holding the static data for Islamic asset management operations. Refer to, Retail Lending (AL) user guide for information on parameter setup for finance management operations.

| Application Name | Features |
|---|---|
| IS.PARAMETER | This table defines, Islamic product features. AA products that can be used for finance. Workflow status and also the status, which enables the sale process. Restrictions on contract creation for specific companies. Category codes and transaction types used at the time of credit workflow accounting. Stage at which customer contribution or down payment can be declared. Delivery tracking for specific type of assets Broker or reviewer category codes and transaction types. Allowed Product code range is from 1 to 9999 |
| IS.STATUS | This table defines, Applicable accounting entries for each of the defined workflow statuses are parameterised in the IS.PARAMETER table. The following accounting events related workflow statuses are defined in Status field of IS.PARAMETER table. Approval Rev Approval Purchase Cost Down Payment Return com to Broker Sell com to Sell Broker Broker Settlement Resale Applicable accounting entries for workflow status that can be used manually as and when required using IS.CONTRACT application. The following accounting events related workflow statuses are used in the IS.CONTRACT application. Sell Com To Sell Broker, Broker Settlement Return Com To Broker, Broker Settlement Broker Settlement accounting event entries are always generated along with either Return To Com To Broker or Sell Com To Sell Broker accounting events. |
| IS.COMMODITY | This table defines, Details of asset or commodity. Support named assets and quantified assets. Commodity active or inactive. Buy broker and sell broker for commodities. Allowed units and decimal quantity. Definition of unit price for commodity for each buy and sell broker combination. Daily allowed amount at commodity level Daily allowed quantity and amount for commodity-broker combination |
| IS.CONTRACT.TASK | This table defines, User-specific tasks and actions. Task or actions during asset purchase as checklist and tracks the same. Tasks that can be either generic or verification type. The ID of the table, which can be any text in alphanumeric format. |
| IS.COST.TYPE | This table defines, Costs incurred during purchase of asset or commodity. Status active or inactive. This parameter also specifies the charge code to default the charge amount for the cost in purchase contract. |
| IS.BROKER | This table defines, Broker related details specific to Islamic Treasury operations. Status active or inactive. Company to which broker belongs to. Broker account and beneficiary details per currency for a particular company. Broker type (Buy, Sell or Both). Broker fee collection related setup and broker share of fee payment frequency. |
| IS.VENDOR | This table defines, Vendor details. Status as 'Active' or 'Inactive' Company wise configuration of vendor account Vendor account and beneficiary details for each currency Commodity wise rebate configuration General rebate details and rebate currency, rebate type (amount or percentage) Special rebate details applicable for specific period with rebate currency, rebate type (amount or percentage) |
| IS.REVIEWER | This table defines, Reviewer related details with the name of the reviewer. Reviewer can be anyone involved in the project and does the service for a fee. Appraiser Project cost evaluator Project Auditor Advisor Legal Consultant Reviewer status whether 'Active' or 'Inactive' Company wise configuration of reviewer account Reviewer account and beneficiary details for each currency |


##### Illustrating Model Products

Islamic finance provides the asset management and finance management functionalities for Temenos Transact .

| Product Group | Product Name | Product Attributes |
|---|---|---|
| NA | Asset Capture | Named assets creation. New asset tables are created when required by user. New field names are added when required by user. |
| NA | Islamic Contract | Vendor purchase contract for named assets and quantified assets. Broker purchase contract for quantified assets. Automatic purchase contract workflow status update. Accounting entries generation based on workflow status. Down payment functionality. Capture cost-related information. |
| NA | Commodity Delivery and Sale | Track delivery of commodities. Sell the delivered commodity to different customers. Record profit or loss amount. |
| NA | Asset Review | Capture review details and collect fee for review. Split fee into customer fee and bank fee. Update project status and next review date. |
| NA | Payment Management | Use multiple payment applications. Support different payment types. |
| Finance - Profit Up-front Sale | Commodity Murabaha | It is a Murabaha based short term placement operation that involves the purchase and sale of commodities in the international exchange. Used for liquidity management purposes. |
| Ijara Finance | One party purchases and leases out the equipment required by the client for a rental fee. The duration of the rental and fee are agreed in advance and ownership of the asset remains with the lessor. At the time of contract maturity ownership. Alternatively, the lessee can agree at the outset to buy the asset at the end of the lease period. Profit collected at the beginning of the contract. Fixed profit method and profit amount is constant. |  |
| Murabaha Finance | Profit is collected at beginning of the contract. Fixed profit method and profit amount is constant. Commodity is sold for cost plus profit, and both the buyer and seller knows the cost and the profit involved. |  |
| Finance - Multi Structured Products | Musawama Finance Wakala Finance | Two types of finances are booked as a part of this product. Purchase cost is disbursed through Wakala contract with zero profit till shipment is in possession of seller. Later, Musawama contract is booked from Wakala start date with agreed profit amount. Profit is collected at the beginning of the contract. Fixed profit method and profit amount is constant. |
| Finance - Profit Accrual Sale | Bai Salam | An Islamic contract in which full payment is made in advance for specific goods (often agricultural products) to be delivered at a future date. Conventional profit bearing product. |
| Construction Finance | Islamic finance in which a manufacturer agrees to complete a construction project on a future date for a fixed, agreed-upon price and with product specifications that both parties agree to. |  |
| Diminishing Musharaka Finance | A partnership in which one of the partners promises to buy the equity share of the other partner gradually until the equity is completely transferred to him. |  |
| Forward Ijara Finance | Lease contract with sale of a clearly specified underlying asset, which is currently being produced or constructed, for a future delivery. With forward ijara, a financier undertakes payment during the construction period, while customer's payments will start within a specific period after completion |  |
| Mudaraba Finance | A partnership in profit whereby the bank provides capital as (Rab Al-maal) and the customer provides labour or work or experience as Mudarib |  |
| Qard Hassan Finance | A contract involving a finance with two parties on the basis of social welfare. During the finance process, the repayment amount must be the same as the amount borrowed. Profit rate to be defined as zero percentage. |  |


> **Related Applications:** `AA.PRODUCT.DESIGNER`, `AA.PRODUCT.GROUP`, `AA.PRODUCT.LINE`, `AA.PROPERTY`, `AA.PROPERTY.CLASS`, `IS.ASSET.REVIEW`, `IS.BROKER`, `IS.COMMODITY`, `IS.COMMODITY.SALE`, `IS.CONTRACT`, `IS.CONTRACT.DELIVERY`, `IS.CONTRACT.TASK`, `IS.COST.TYPE`, `IS.EQUIPMENT`, `IS.MISCASSET`, `IS.MOVEQUIPMENT`, `IS.PARAMETER`, `IS.PAYMENT`, `IS.REALESTATE`, `IS.REVIEWER`, `IS.STATUS`, `IS.VEHICLE`, `IS.VENDOR`

---


### 2.15  Payment Management


> **📇 Quick Reference Card**
> 
> **Purpose:** *Payment management system manages all Islamic banking payment activities. Payment activities such as payments to vendor, broker, cost counterparty, reviewer and retention amounts are handled by using payment management applications.*
> 
> **Applications:** `FUNDS.TRANSFER`, `IS.PAYMENT`, `TELLER`
> 
> **Key Fields:** *Asset Reference*, *Ben Bank*, *Ben Cust*, *Ben Customer*, *Ben. Acct. No*, *Ben. Cust*, *Beneficiary*, *Booking Date* ... +31 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Payment management system manages all Islamic banking payment activities. Payment activities such as payments to vendor, broker, cost counterparty, reviewer and retention amounts are handled by using payment management applications.

The following applications are used for Islamic payments:

- IS.PAYMENT
- FUNDS.TRANSFER
- TELLER

Payment management system allows the user or system to perform the several actions. This system:

- Allows to use multiple payment applications
- Supports different payment types, such as vendor, broker and cost
- Allows ad hoc and scheduled payment
- Allows single payment for multiple purchases
- Allows input and reversal of payment transactions


#### ⚙️ Configuration

Payment management feature has no specific configuration to be setup. The parameter tables are setup at the implementation stage.


#### 📋 Tasks

Related topics:

- Decide on Payment Types (IF)
- Execute Broker Settlement (IF)
- Islamic Financing processes

Payment management manages all Islamic banking payment activities, such as, vendor payments (ad hoc or schedule basis), payments to cost counterparty (ad hoc or schedule basis), retention amount payments, reviewer payments, broker payments, rebate payments and down payments through the following applications:

- IS.PAYMENT
- FUNDS.TRANSFER
- TELLER


##### Workflow

This section allows the user to perform the below tasks:

| SCREENS | WORKFLOW |
|---|---|
|  | Authorise – Payment Transactions . |
| Unauthorised Payments | Click the Authorise icon of a corresponding record. |
| Authorise Payment | Click the Authorise icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Authorise – Payment Transactions . |
| Unauthorised Payments | Click the Authorise icon of a corresponding record. |
| Authorise Payment | Click the Authorise icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Authorise – Payment Transactions . |
| Unauthorised Payments | Click the Authorise icon of a corresponding record. |
| Authorise Payment | Click the Authorise icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Authorise – Payment Transactions . |
| Unauthorised Payments | Click the Authorise icon of a corresponding record. |
| Authorise Payment | Click the Authorise icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Input – Down Payment . |
| Down Payment Transactions | Click the Down Payment icon of a corresponding record. |
| Down Payment | Enter values in the following fields: Customer No Commodity Reference Asset Reference Commodity Sale Reference Debit Account Debit Currency Down Payment Amount Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

| SCREENS | WORKFLOW |
|---|---|
|  | Authorise – Payment Transactions . |
| Unauthorised Payments | Click the Authorise icon of a corresponding record. |
| Authorise Payment | Click the Authorise icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Rebate Payment – Adhoc . |
| Rebate Payment | Click the Input Rebate Payment icon of a corresponding record. |
| Rebate | Enter values in the following fields: Rebate Payment Option Payment Amount Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |


#### 📊 Outputs

There are no Outputs available for the Payment Management feature.


> **Related Applications:** `FUNDS.TRANSFER`, `IS.PAYMENT`, `TELLER`

---


### 2.16  PaymentManagementUsingPO


> **📇 Quick Reference Card**
> 
> **Purpose:** *The payment management manages all the Islamic banking payment activities. Payment Order (PO) is used for handling Islamic payments such as payments to vendor, retention, rebate and cost payments. The payment management system:*
> 
> **Applications:** `IS.ASSET.REVIEW`, `IS.CONTRACT`, `IS.COST.PAYMENT.BALANCES`, `IS.DOWN.PAYMENT.BALANCES`, `IS.PP.STATUS.CODE`, `IS.REVIEWER.PAYMENT.BALANCES`, `IS.VENDOR`, `IS.VENDOR.PAYMENT BALANCES` ... +8 more
> 
> **Key Fields:** *Allow BIC*, *Allow Future Date*, *Allow IBAN*, *Allow Sort
 code*, *Asset
 Reference*, *Asset Reference*, *Beneficiary*, *Booking Date* ... +28 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The payment management manages all the Islamic banking payment activities. Payment Order (PO) is used for handling Islamic payments such as payments to vendor, retention, rebate and cost payments. The payment management system:

- Supports different payment types, such as vendor, retention, rebate and cost payments.
- Allows single payment or multiple payments for a single purchase.
- Allows input, amend and reversal of payment transactions.


#### ⚙️ Configuration

Some specific parameters and configuration for Islamic payment activities such as Vendor and Retention payments are described below.

PAYMENT.ORDER.PARAMETER is a company wise record and Islamic payments uses the Payment Connection Method as Temenos Payment System (TPS). The Payment Connection Method field defines the connection method between the payment order and the payment processing system. Temenos Payment Hub is used for processing the Islamic payments initiated through Payment order.

Islamic payments can be made to an internal vendor or to a vendor who is not registered in the Transact system. To facilitate this, there are different payment order products configured for internal and external Islamic payments.

- The Allow Future Date field in PAYMENT.ORDER.PRODUCT is used for processing a payment with a future date. This is configured as Yes for all Islamic payments.
- The Warehouse Required field is used to define whether the future dated payments are to be processed on the processing date during Start of Day processing in COB (Close of Business) or immediately. This is configured as No for all Islamic payments.
- The Pay through beneficiary field in PAYMENT ORDER PRODUCT is used for enabling payment to an external customer.

PP.MSGPAYMENTTYPE is configured for Islamic payments with IDs same as that of the Payment order product.

PP.NODA.LIST defines the list of messages for which Debit Authority Check to be skipped. This is configured for all Islamic payments. The Startdate and Enddate fields represent the period when the debit authority check has to be skipped.

The PAYMENT.ORDER.PRODUCT , PP.MSGPAYMENTTYPE , PP.NODA.LIST configurations for internal, external vendor payment and retentions are described below:

| Table Name | Internal Vendor | Internal Retention | External Vendor | External Retention |
|---|---|---|---|---|
| PAYMENT.ORDER.PRODUCT | Pay Through Beneficiary = No | Pay Through Beneficiary = No | Pay Through Beneficiary = Yes Allow IBAN , Allow BIC and Allow Sort code fields = Allowed. | Pay Through Beneficiary = Yes |
| PP.MSGPAYMENTTYPE |  |  |  |  |
| PP.NODA.LIST |  |  |  |  |

The following common parameters are used for identification of Islamic payments.

The ISL record in PP.SOURCE is created for Islamic payments and linked to Order initiation type in a payment for easy identification of Islamic payments.

Actions to be performed for the corresponding status codes of Islamic payments are configured in this table as below.


#### 🔧 Working With

The following section describes in detail how the payment management is used to handle vendor, retention, rebate, cost , down and broker payments.

Start

- Vendor
- Retention
- Rebate
- Cost
- Down
- Broker
- Reviewer


##### Vendor Payments

An Islamic bank procures assets or commodities from the vendors and sells these goods/services to a customer with an agreed profit. The bank needs to make payments to the vendor for the goods bought. These vendors can be registered within Transact and external to Transact with beneficiary details updated within Transact. Vendor payments in Islamic banking can be managed through payment order. Transact supports internal and external vendor payments.

Payment to the vendor can be made as a single payment or multiple times till the full amount for a particular goods/service is paid. IS.VENDOR.PAYMENT.BALANCES captures the payments made and maintains the payment balances for Islamic contracts. This is a system-maintained table and is updated when an Islamic contract is created using the IS.CONTRACT application.


##### Retention Payments

Retention is used to hold a percentage or amount to be paid to the vendor. This retained amount is paid using a separate payment called Retention payment. Retention percentage or amount is defined as part of vendor payment initiation to retain a specific amount and pay the remaining to the vendor. For example, while initiating a vendor payment for 8,000, the user can retain 10% of this payment and pay this separately to the vendor as retention payment. Like vendor payments, retention payments can be made to an internal vendor or any external vendors using different clearing methods.

> **⚠️ Note:** Retention payment can only be made as a single payment for the entire retention amount. The system raises an error while creating retention payment in PO with partial retention amount.


##### Key Highlights ofIS.VENDOR.PAYMENT.BALANCES

The IS.VENDOR.PAYMENT.BALANCES table contains the vendor payment details such as total vendor payment, outstanding vendor payment, and payment order ID along with the payment status.

- The ID format of this table is - for any asset purchase and - for commodity purchase.
- The system refers the outstanding amount in this table to keep track of the pending payments to the vendor for a specific asset. It raises an error when a payment order is initiated for vendor payment with an amount greater than the outstanding amount in this table.
- The Vendor Payment Status field in IS.VENDOR.PAYMENT.BALANCES is used for tracking the status of the payment. This payment status is based on the status field in IS.PP.STATUS.CODE . ID of this table is PP.STATUS.CODE. The outstanding balances of the vendor payments is updated based this status field.

The IS.VENDOR.PAYMENT.BALANCES table is updated in the following scenarios:

- When the user creates an IS contract and subsequently updated whenever there is a payment to the vendor.
- In scenarios, where there are multiple assets linked to a same IS contract, a unique record is created in this table for every asset. For a Ijarah contract under construction, ID of the vendor payment balances is updated with only the contract reference.
- When a payment order is input and not authorized. This table is updated with the payment details. When a payment order record is deleted from unauthorised status, the payment balance details in vendor payment balances are updated accordingly. For example, consider a vendor payment for an asset purchase of 10,000. If the user makes two vendor payments for 2,000 and 2,500, the outstanding vendor payment is updated as 5,500 in IS.VENDOR.PAYMENT BALANCES record. When the user deletes the payment order for 2,500 in unauthorised status, the total outstanding vendor payment is updated as 8,000.
- It is possible for a payment order record to go into repair queue due to some errors while processing the payment. Also, it is possible to cancel a payment order transaction when warehousing is enabled at payment product level. In such scenarios, the outstanding and paid amount in this table are updated based on the cancelled transaction amount. This update is enabled for vendor and retention payments.
- The Payment Order system uses the POR.POSTING.REVERSAL application for reversing a payment order transaction which is in completed status. When the user cancels a processed vendor or retention payment using PO reversal, the outstanding and paid amount in the IS.VENDOR.PAYMENT BALANCES table are updated based on cancelled transaction amount.

Read Payment Inititation for more details on Payment order.


##### Rebate Payments

A vendor rebate is a discount the vendor offers for purchasing the asset. The bank receives the rebate from the manufacturers or dealers. It is possible to share the rebate amount with the finance customer or bank's PL account using the Rebate Payment option. Accounting entries are generated for the rebate payment from the multi-supplier account on the bill date and the payment balances file is updated.

Rebates can be configured in IS.VENDOR for a specific commodity. Different percentages or flat amounts can be configured as rebates for different commodities. When the user creates an asset purchase transaction, if Rebate Allowed is enabled, the system defaults the rebate details from the IS.VENDOR configuration and the rebate amount is calculated.

When a rebate is allowed for an asset and the Rebate Type is:

- Finance - The system reduces this amount from vendor payment amount while updating IS.VENDOR.PAYMENT.BALANCES . For example, if 50,000 is the price of the asset and the vendor rebate percentage is set as 10%, then the outstanding amount in vendor payment balances is updated as 49,500 during the asset purchase. This rebate amount can be amortised into the PL category from the finance arrangement throughout the tenor.
- Payment -The system updates IS.VENDOR.PAYMENT.BALANCES with the rebate details like, rebate action, rebate payment reference and rebate balance details. This amount can be paid using a Payment order to the finance customer having a Transact account or to an account in a different bank using an external beneficiary.

The Internal Rebate PL Category option is used to pay the rebate amount to the PL category (recognised as an income for the bank).


##### Cost Payments

Cost payment is used to pay any additional cost incurred during the asset purchase. Apart from the purchase price of the asset, there are other costs such as money spent on freight, custom duties, packaging, documentation, taxes, and so on that may be involved in bringing the asset to a usable condition. Cost payment is used to make payments to cost counter-party. Cost payment can be made to a registered cost counter-party in Transact or to an external beneficiary. The accounting entries are generated for cost payments from the multi-supplier account on the payment date.

IS.COST.PAYMENT.BALANCES is updated while generating an accounting entry for the cost payment. The system creates this table with ID as IS.CONTRACT.REFERENCE.NUMBER-COST.TYPE-COST.PAYMENT.TYPE. For a particular cost payment type the cost payment can only be made in full. Part payments are not allowed. Payment order transaction details are updated in this table for tracking purposes.


##### Down Payment

Down payment is an initial, one-time payment the customer makes to reflect their financial status and credibility.

The down payment amount paid by the customer can be captured in the purchase contract and can be collected by changing the status of IS.CONTRACT . It is also possible to collect the down payment amount using a payment order. The down payment amount captured in the purchase contract can be validated against the amount paid by the customer.

In the Down Payment page, it is required to capture the Customer ID, Purchase reference number, Asset reference number or Commodity, Debit Account number, and Debit currency. Also, it is required to capture the down payment amount in the Request Amount field. The system defaults the down payment settlement account number in the Credit Account Number field.

During validation,

- If the down payment amount is defined in the purchase contract using cash - bank combination, then it is validated and it is not possible to collect the down payment amount greater than the amount defined.
- Otherwise, the down payment amount can be collected up to 99% of the total purchase amount.

While authorising the down payment transaction accounting entries are posted.

The down payment amount can be collected from the customer either as a single payment or in multiple installments. IS.DOWN.PAYMENT.BALANCES captures the down payment related details and keeps track of the down payment made by the customer.


##### Broker Payments

For commodity Murabaha finance contracts, the user can execute the broker settlement transactions to post the required accounting entries. Below broker settlement transactions can be executed using a payment order.

- Broker Payment - External
- Sell commodity and Credit customer account
- Sell broker settlement
- Broker settlement

This option is used to settle the buy broker account outside Transact. As per the business flow, the bank purchases the commodity from the buy broker based upon the customer request. During a commodity purchase, if the buy broker does not have a Transact account , then the purchase amount is credited into the buy broker wash account using the Broker Payment - External option. The user can debit the buy broker wash account and credit the buy broker account with the external bank.

The user can capture Customer ID, Purchase reference number, Debit account number, Debit currency, and Request amount. During authorisation, the broker payment accounting entries are generated.

Consider the scenario where on behalf of the customer request, the bank buys the commodity from the buy broker. The bank can create a finance arrangement against the customer by handing over the commodity to him. Then, the customer can handover the commodity to the bank requesting to sell the commodity to another broker and credit the proceeds to his settlement account. This transaction can be handled using the sell commodity and credit customer account Payment Order page.

The user can capture the Customer ID, Purchase reference number, Debit account number, Debit currency, and Request amount . Also, the customer account needs to be captured as credit account number to credit the sold proceeds to his account number. During authorisation, the settlement accounting entries are posted.

While executing the sell commodity and credit customer account transaction, in case, if the sell broker does not have the Transact account, then it is possible debit the amount received in the nostro account of the sell broker and credit the sell broker wash account.

The user can capture the Customer ID, Purchase reference number, Debit account number, Debit currency, and Request amount. The sell broker wash account needs to be captured as credit account number to settle the outstanding balances.

The broker account belonging to buy broker and sell broker can be settled using the Broker Settlement page . The user can capture the Customer ID, Purchase reference number, Debit account number, Debit currency, and request amount. During authorisation, the buy broker and sell broker account balances are settled.


##### Reviewer Payments

Asset review is the process of evaluating and inspecting the asset while it is under construction or manufacturing. IS.ASSET.REVIEW captures the review particulars of the asset and asset inspection related information such as, date of review, result of review and project status. A fee for the services rendered by the reviewer can be captured in the system. Reviewer payment transaction is used for paying this fee to the reviewer.

It is possible to split the fee amount between the customer and the bank while capturing Asset review details. Once the payment transaction is completed, the accounting entries are generated from multi supplier account to the reviewer account. It is possible to make payments to a reviewer registered in the system or to an external vendor by using their beneficiary details.

IS.REVIEWER.PAYMENT.BALANCES captures asset review payment related details and used for tracking reviewer balance.


##### Business Workflow

The business workflow for an internal vendor payment is illustrated below.

IS.VENDOR.PAYMENT.BALANCES is updated on an Islamic contract creation.

The payment order is initiated for a partial payment to an internal vendor as shown below.

IS.VENDOR.PAYMENT.BALANCES is updated as below.

At this stage, if the user tries to make another payment for 50,000, this transaction amount is compared to the outstanding amount and a validation is raised as shown below.

The IS.VENDOR.PAYMENT.BALANCES table is updated for external vendor payments, internal retention payment, and external retention payments similarly.


#### 📋 Tasks

Related topics:

- Manage Cost Payment Using Payment Order (IF)
- Manage Down Payment Using Payment Order (IF)
- Manage Rebate Payment Using Payment Order (IF)
- Manage Reviewer Payment Using Payment Order (IF)
- Manage Vendor Payment Using Payment Order (IF)
- Manage Retention Payment Using Payment Order (IF)

Payment management manages all Islamic banking payment activities, such as, vendor payments (adhoc or schedule basis), payments to cost counterparty (adhoc or schedule basis), retention amount payments, reviewer payments, broker payments, rebate payments and down payments using Payment Order.

To initiate payment to a vendor account that available within the bank through Payment Order application, perform the following steps.

1. Vendor Payment .
2. To make payment to a vendor account available within the bank, enter values in the following fields: Customer No Contract Reference Commodity Asset Reference Debit Amount Credit Account
3. Click the Validate a deal icon to check for errors and overrides.
4. Click the Commit the deal icon to submit the record.

To initiate payment to a vendor account that available within the bank through Payment Order application, perform the following steps.

1. Retention Payment .
2. To make payment to a vendor account available within the bank, enter values in the following fields: Customer No Contract Reference Commodity Asset Reference Debit Amount Credit Account
3. Click the Validate a deal icon to check for errors and overrides.
4. Click the Commit the deal icon to submit the record.

To initiate rebate payment to a vendor account that available within the bank through Payment Order application, perform the following steps.

1. Rebate Payment .
2. To make payment to a vendor account available within the bank, enter values in the following fields: Customer No Contract Reference Commodity Asset Reference Rebate Pay (Customer/ PL Category) Payment Amount Credit Account
3. Click the Validate a deal icon to check for errors and overrides.
4. Click the Commit the deal icon to submit the record.

To initiate a cost payment to counterparty that available within the bank through Payment Order application, perform the following steps.

1. Cost Payment .
2. To make payment to a vendor account available within the bank, enter values in the following fields: Customer No Contract Reference Commodity Asset Reference Cost Pay Type Payment Amount Credit Account
3. Click the Validate a deal icon to check for errors and overrides.
4. Click the Commit the deal icon to submit the record.

To initiate a payment to a reviewer in ad hoc basis through Payment Order, perform the following steps:

1. Reviewer Payment
2. Enter Contract reference or Asset reference to get the Reviewer payment details.
3. To make a payment to a reviewer account available within the bank, enter values in the following fields: Reviewer Account Payment Currency Payment Amount Payment Date Purchase Reference Commodity Asset Reference Review Reference Payment Date
4. To make a payment to a reviewer account available in other banks, enter values in the following fields using ‘External Reviewer PO’ option: Reviewer Beneficiary Payment Currency Booking Date Purchase Reference Commodity Asset Reference Review Reference Payment Date Payment Amount
5. Click Validate to check for errors and overrides.
6. Click Commit to submit the record.

| SCREENS | WORKFLOW |
|---|---|
|  | Down Payment . |
| Down Payment Transactions | Click the Down Payment icon of a corresponding record. |
| Down Payment | Enter values in the following fields: Customer No Purchase Reference Asset Reference Commodity Debit Account Debit Currency Down Payment Amount Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

To initiate a payment to a broker in ad hoc basis through the Payment Order application, perform the following steps:

1. Broker Payment
2. To make a payment to a broker account available within the bank, enter values in the following fields: Broker Broker Account Payment Currency Booking Date Purchase Reference Commodity Payment Date Payment Amount
3. To make a payment to a broker account available in other banks, enter the values in the following fields using ‘Broker Payment - External’ option: Broker Beneficiary Payment Currency Booking Date Purchase Reference Commodity Payment Date Payment Amount
4. Click Validate to check for errors and overrides.
5. Click Commit to submit the record.


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to Payment Management using PO.


##### Enquiries and Reports

This section allows the user to view the below list of enquiries and reports.

Vendor Payment and click FIND .

This enquiry displays the details of vendor and retention payment for specific asset reference.

Rebate Payment and click FIND .

This enquiry displays the details of rebate payment for specific asset reference.

Cost Payment and click FIND .

This enquiry displays the details of cost payment for specific asset reference.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA


> **Related Applications:** `IS.ASSET.REVIEW`, `IS.CONTRACT`, `IS.COST.PAYMENT.BALANCES`, `IS.DOWN.PAYMENT.BALANCES`, `IS.PP.STATUS.CODE`, `IS.REVIEWER.PAYMENT.BALANCES`, `IS.VENDOR`, `IS.VENDOR.PAYMENT BALANCES`, `IS.VENDOR.PAYMENT.BALANCES`, `PAYMENT ORDER PRODUCT`, `PAYMENT.ORDER.PARAMETER`, `PAYMENT.ORDER.PRODUCT`, `POR.POSTING.REVERSAL`, `PP.MSGPAYMENTTYPE`, `PP.NODA.LIST`, `PP.SOURCE`

---


### 2.17  ProfitDeclaration


> **📇 Quick Reference Card**
> 
> **Purpose:** *Mudaraba is for the fixed period, the customer (Mudarib or fund manager) must return the Mudaraba capital and the bank (Rab Ul Mal or fund provider) share of the realised Mudaraba profit at the end of the Mudaraba term.*
> 
> **Applications:** `AA.ARR.XIS.DRAWING`, `AA.ARR.XIS.FACILITY`, `CURRENCY`, `IS.PARAMETER`, `IS.PAYMENT.DECLARATION`
> 
> **Key Fields:** *Acc Difference Amount*, *Acc Difference Amt*, *Accrual
 End Date*, *Accrual End Date*, *Accrual Start Date*, *Amount*, *Arrangement*, *Arrangement Status* ... +41 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Mudaraba is for the fixed period, the customer (Mudarib or fund manager) must return the Mudaraba capital and the bank (Rab Ul Mal or fund provider) share of the realised Mudaraba profit at the end of the Mudaraba term.

- The Mudaraba capital invested by the bank through Mudaraba is not in the nature of a fixed receivable loan type. It is like an investment subject to increase in case of profitability or decrease in case of loss. The customer (Mudarib) has to invest the Mudaraba capital in business activities to fulfil the objectives of the investment during the fixed period.
- The Mudaraba capital in a business project under a Mudaraba agreement has to allow for partial return (to the extent intact) of the Mudaraba capital during the Mudaraba term period. The parties to the Mudaraba agreement may agree based on the partial return (to the extent intact) of the Mudaraba capital either in the Mudaraba agreement or may mutually agree on the same at any time during the Mudaraba term period, if such an arrangement has not been covered in the relevant Mudaraba agreement.
- In case of partial return during the Mudaraba term period, if upon the determination (for example, by constructive liquidation) the Mudaraba capital is still intact, then the company may be required to return part of the agreed Mudaraba capital along with the entire profit entitlement of the bank, on the date of such determination. The company may then reinvest the balance of the Mudaraba capital on Mudaraba basis for the rest of the Mudaraba term period.
- If upon the determination (for example, by constructive liquidation) the Mudaraba capital has occasioned a loss due to market considerations without the negligence or misconduct of the company or customer, then the bank has to bear the extent of the loss and the Mudaraba capital will decrease accordingly. In such a situation, the basis for determination either for partial (during the Mudaraba term period) or total return (at the end of the Mudaraba term period) is the actual remaining Mudaraba capital and not the original Mudaraba capital which was invested at the time of creating the Mudaraba partial liquidation will be applied on the current Mudaraba capital amount and not the original Mudaraba capital amount.
- It is not a binding contract, and each party has the right to terminate the contract on its own discretion. However, if a Mudaraba period has been agreed upon between the parties, then the Mudaraba binding for such period and no party can terminate it on its own till the completion of such Mudaraba period. The ratio of profit distribution does not change due to early termination of Mudaraba, that is, if the profit sharing percentage was agreed to be distributed 50% for the bank and 50% for the customer, then the same forms the basis for the determination and distribution of the Mudaraba profit even in the case of early termination.
- The Mudarib can realise the Mudaraba investment with the desirable profit within the extended period in the following cases: If the Mudaraba contract is extended by the required period The Mudaraba capital remains invested The redemption is delayed due to reasons beyond Mudarib’s control
- If there is a delay in liquidating the Mudaraba due to breach, misconduct, or negligence of the customer (as Mudarib) then the entire Mudaraba capital gets transformed into a debt on the customer. Resultantly, the bank would not continue to be Rab Ul Mal but a creditor to the customer. However, the amount is frozen, and the bank cannot claim any amount over and above the originally invested Mudaraba capital. The Rab Ul Mal also adds the expected profit which was projected by the Mudarib at the time of receiving the Mudaraba funds. Still if the customer does not pay its obligation, the bank may give relaxation in time or can liquidate the collaterals provided by the customer (if any) and realise its claim for the Mudaraba amount.

The customer (as Mudarib) can declare the realised profit amount for Mudaraba finance arrangement at the facility or drawings level based upon the Mudaraba agreement. Based upon the difference between the expected and actual profit amounts, the system posts the accounting entries.


#### ⚙️ Configuration

The expected profit rate setup at the Mudaraba drawings level is used collect the profit amount from the customer based upon agreed repayment schedule. The expected profit amount is calculated based upon the Mudaraba capital invested by the bank in the business run by the customer. The actual profit amount can be declared by the customer as per the agreed terms with the bank. It is possible to declare the actual profit amount multiple times during finance term (or) it can be declared once upon maturity.


##### Configuring Product Parameter

Income or Expense categories related to Profit declaration for the Mudaraba finance product can be configured in IS.PARAMETER .

| Field | Description |
|---|---|
| Income PL | It is used to setup the PL category to credit the bank portion of the realised profit received from the customer. |
| Profit decl Expense PL | It is used to setup the PL category to settle the shortage profit amount declared by the customer (Expected profit amount – Actual profit amount). |
| Profit Decl Txn | It is used to setup the FT.TXN.TYPE.CONDITION record to raise the realised profit declaration accounting entries. |


##### Declaring Profit

The customer (Mudarib) can declare the realised profit amount from the business during any time in the Mudaraba finance life cycle. It can be declared at the facility or drawings level depending upon the relevant arrangement level setup. It is possible to declare the profit amount multiple times for the period to post the accounting entries.

| Field | Description |
|---|---|
| ID | The facility or drawings reference number used for declaring the realised profit amount and a sequence number to handle the multiple profit declarations from the customer. AA131231312-001, where AA131231312 is the facility or drawings reference number and 001 is the sequence number. |
| Decl Level | It is used to identify the profit declaration level. It can be selected as Facility or Drawings and the system defaults these from the facility or drawings. |
| Arrangement | The system defaults the facility or drawings reference number captured in the ID automatically and it cannot be edited. |
| Accrual Start Date | The system defaults it automatically as Value date. If the realised profit amount is declared already, then it defaults the (previous accrual end date + 1) and it cannot be edited. |
| Accrual End Date | It is required to input the date up to which the profit amount is declared by the customer. |
| Customer | The system defaults the customer ID of the arrangement and it cannot be edited. |
| Product | The system defaults the arrangement product name and it cannot be edited. |
| Value date | The system defaults the arrangement value date and it cannot be edited. |
| Maturity date | The system defaults the arrangement maturity date and it cannot be edited. |
| Amount | The system defaults the arrangement amount and it cannot be edited. |
| Arrangement Status | The system defaults the arrangement status and it cannot be edited. |
| Booking Date | The user can input the value date for posting profit declaration accounting entries. |
| Drawing ID | If Decl level is set as Facility, then the system defaults the drawings (single or multiple) created under the facility automatically and it cannot be edited. |
| Drawings Arr Currency | It is used to display the currency of the Drawing ID . |
| Profit Acc Type | The system defaults the profit properties linked to the Facility or Drawings product marked with profit property type as Profit, Profit declaration and it cannot be edited. |
| Profit Acc Start Date | The starting date from which the profit amount accrued in the profit property populated in Profit Acc type . |
| Profit Acc End Date | The ending date up to which the profit amount accrued in the profit property populated in Profit Acc type . |
| Profit Acc Amount | Accrued profit amount from Profit Acc Start Date to Profit Acc End Date . |
| Profit Acc Amount Facility Ccy | In case if drawings are made in any other currency than facility currency then the Profit Acc Amount is converted and displayed in facility currency. |
| Total Accrual Profit Amount | Total accrued profit amount from multiple profit properties or multiple drawings populated in Profit Acc Amount Facility Ccy. |
| Declared Profit Amt | The user can input the realised profit amount declared by the customer in facility currency. |
| Acc Difference Amt | Difference between Total Accrual Profit Amt and Declared Profit Amt is updated. It is not allowed to edit the populated value. |
| Profit Share Perc | The system defaults the profit share percentage captured at the facility or drawings level automatically and it can be amended. |
| Profit Share Calc Amt | It is calculated by multiplying the Acc Difference Amt with the Profit Share Percentage . The un-rounded calculated amount is displayed in the field. |
| Profit Share Amt | It is used to display the rounded-off value of the Profit Share Calc Amt . It is rounded by considering the number of decimals configured in CURRENCY . |
| Settlement Account | This account is used to debit the bank share of the realised profit amount (or) and is used to credit the bank share of the shortage profit amount into the customer account which can be used to settle the Mudaraba finance outstanding amount. |


#### 🔧 Working With

The following section describes declaring profit at facility and drawing levels in detail.


##### Declaring Profit at Facility Level

The customer can declare the profit amount at the facility level. For this, it is required to capture the facility reference number as the ID of the IS.PAYMENT.DECLARATION application. If there is a previous profit amount declaration for the facility reference, then the system automatically creates the next record. Otherwise, it appends “001” along with the facility reference number separated by “– hyphen”.

The system defaults the conditions setup at the facility level using AA.ARR.XIS.FACILITY into declaration level. The other details related to the facility reference number are populated automatically into the relevant fields.

| Field | Description |
|---|---|
| Accrual Start Date | It is the value date of the facility reference number. If the profit amount is already declared for the facility reference number, then the system defaults the ( Accrual End Date + 1) of the previous profit declaration record into this field. |
| Accrual End Date | The user inputs this, and it has to be less than or equal to the maturity date of the facility reference number. |
| Profit Share Perc | The system defaults this value from the facility level condition and it can be amended. |
| Customer , Product , Contract Currency , Value Date , Maturity Date , Amount , Arrangement Status | The system defaults these values from the facility reference number. |
| Booking Date | It is used to capture the value date of the profit declaration. The system defaults it as the current date and it cannot be edited. |
| Drawing ID | The system populates the drawings created under the facility reference number automatically into this field. If the profit amount is declared at the facility level, then it is not possible to remove any drawings ID getting included in the profit declaration calculation. |
| Drawings Arr Currency | The system defaults this value from Drawing ID. |
| Profit Acc Type | The system defaults the profit properties associated with the Drawing product marked with property Type as Profit and Profit declaration into this field. It is not possible to remove the defaulted profit properties during profit declaration calculation. |
| Profit Acc Start Date , Profit Acc End Date , Profit Acc Amt , Profit Acc Amount Facility Ccy | These are used to default the accrued profit amount between “date from” and “date to” dates using the expected profit rate setup at the drawing level. The accrued profit amount is converted to facility currency and displayed in Profit Acc Amt Facility Ccy . The profit amount accrued between multiple dates are populated automatically for the relevant profit property. |
| Total Accrual Profit Amt | It displays the sum of the accrued profit amount from multiple profit properties linked to multiple drawings arrangement. |
| Declared Profit Amt | It is used to capture the profit amount declared by the customer. |
| Acc Difference Amount | It displays the difference between Total Accrual Profit Amt and Declared Profit Amt . |
| Profit Share Amt | The Profit Share Perc value is applied on the Acc Difference Amount to calculate it. |
| Settlement Account | It is used to capture the account number. |

If Declared Profit Amt is greater than Total Accrued Profit Amt by using the expected profit rate, then the customer has earned more profit from the business. The bank has to recover its share of the profit amount from the customer during profit declaration.

- DR Customer Account (Bank share of profit share amount)
- CR Income PL (Bank share of profit share amount)

If Declared Profit Amt is less than Total Accrued Profit Amt by using the expected profit rate, then the customer has earned less profit amount from the business. The bank pays the shortage profit amount from the Expenses PL to the customer account. It can be used to settle the Mudaraba finance outstanding amount (principal + profit).

- DR Expenses PL (Bank share of shortage profit share amount)
- CR Customer Account (Bank share of shortage profit share amount)


##### Declaring Profit at Drawings Level

The customer can declare the profit amount at the drawings level. For this, it is required to capture the drawing reference number as the ID of the IS.PAYMENT.DECLARATION application. If there is a previous profit amount declaration for the drawing reference, then the system automatically creates the next record. Otherwise, appends “001” along with the inputted drawing reference number separated by “– hyphen”.

The system defaults the conditions setup at the drawing level using AA.ARR.XIS.DRAWING into Declaration level. The other details related to the Drawings reference number are populated into the relevant fields.

| Field | Description |
|---|---|
| Accrual Start Date | It is the value date of the drawing reference number. If the profit amount is already declared for the drawing reference number, then the system defaults the ( Accrual End Date + 1) of the previous profit declaration record into the Accrual Start Date . |
| Accrual End Date | The user inputs this, and it is required to be less than or equal to the maturity date of the drawing reference number. |
| Profit Share Perc | The system defaults this from the drawing level condition. |
| Customer , Product , Contract Currency , Value Date , Maturity Date , Amount , Arrangement Status | The system defaults these from the drawing reference number. |
| Booking Date | It is used to capture the value date of the profit declaration. The system defaults it as current date and it cannot be edited. |
| Drawings ID | The system populates it from the ID. |
| Drawings Arr Currency | The system defaults it from Drawing ID. |
| Profit Acc Type | The system defaults the profit properties associated with the Drawing product marked with property Type as “Profit” and “Profit declaration” into this field. It is not possible to remove the defaulted profit properties during profit declaration calculation. |
| Profit Acc Start Date , Profit Acc End Date , Profit Acc Amount , Profit Acc Amt Facility Ccy | These are used to default the accrued profit amount between “date from” and “date to” dates using the expected profit rate setup at the Drawing level. The accrued profit amount is converted to facility currency and displayed in Profit Acc Amt Facility Ccy . The profit amount accrued between multiple dates are populated automatically for the relevant profit property. |
| Total Accrual Profit Amount | It displays the sum of the accrued profit amount from multiple profit properties linked to drawings arrangement. |
| Declared Profit Amt | It used to capture the profit amount declared by the customer. |
| Acc Difference Amount | It displays the difference between Total Accrual Profit Amt and Declared Profit Amt. |
| Profit Share Amt | Profit Share Percentage is applied on Acc Difference Amount to calculate this value. |
| Settlement Account | It is used to capture the account number. |

If Declared Profit Amt is greater than Total Accrued Profit Amt using the expected profit rate, then the customer has earned more profit from the business. The bank has to recover its share of the profit amount from the customer during profit declaration.

- DR Customer Account (Bank share of profit share amount)
- CR Income PL (Bank share of profit share amount)

If Declared Profit Amt is less than the Total Accrued Profit Am t by using the expected profit rate, then the customer has earned less profit from the business. Bank pays the shortage profit amount from the Expenses PL to the customer account. It can be used to settle the Mudaraba finance outstanding amount (principal + profit).

- DR Expenses PL (Bank share of shortage profit share amount)
- CR Customer Account (Bank share of shortage profit share amount)


##### Amending Profit Declaration

It is possible to amend the profit declaration by selecting the required profit declaration record. It is not possible to reverse the profit declaration.

During amendment, the accounting entries are posted again by reversing the old accounting entries. The history of previously posted accounting entries are stored for future reference.


#### 📋 Tasks

Profit Declaration can be amended by selecting the required profit declaration record. Profit Declaration cannot be reversed.

| SCREENS | WORKFLOW |
|---|---|
| Input - Profit Declaration | Input - Profit Declaration . |
|  | Facility and Drawings arrangements are grouped in separate tabs for ease to declare the profit amount. |
|  | Enter values in the required fields: Declared Profit Amt Settlement Account |
|  | Click the Validate icon to check for errors and overrides. Click the Commit icon. Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
| Input - Profit Declaration | Authorise/Delete/View - Profit declaration. . |
|  | List of un-authorised profit declaration records are displayed. |
|  | Click the Authorise button to authorise the profit declaration. Click the Delete button to delete the profit declaration. Click the Modify button to modify the profit declaration. |
|  | Click the Commit icon. Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
| Input - Profit Declaration | Amend - Profit Declaration . |
|  | List of Authorised Profit Declaration records are displayed. |
|  | Click the Amend button to modify the record details. |
|  | Modify the Declared Profit Amt (or) Settlement Account . Click the Validate icon to check for errors and overrides. Click the Commit icon. Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
| View - Profit Declaration | View - Profit Declaration . List of Authorised Profit Declaration records are displayed. |
|  | Click the View button to see the record details. |


#### 📊 Outputs

There are no Outputs available for Profit Declaration feature.


> **Related Applications:** `AA.ARR.XIS.DRAWING`, `AA.ARR.XIS.FACILITY`, `CURRENCY`, `IS.PARAMETER`, `IS.PAYMENT.DECLARATION`

---


### 2.18  Charges


> **📇 Quick Reference Card**
> 
> **Key Fields:** *Def Account*, *Method*
> 
> **Sections:** 🔧 Working With


#### 🔧 Working With

Financial institutions can impose charges at the multi-currency arrangement on occurrence of a specific activity (activity charge) or on a specific frequency (scheduled charge).

These charges can be debit charges collected from customer or credit charges that can be paid to the customer. Only a flat amount can be collected or paid as a charge. The Issue Bill activity is triggered on the settlement arrangement for the activity or scheduled charge to get processed. The defined charge will only be capitalised against the defined settlement account. The Generate Charges Activity is used by the system to capitalise these charges to the liquidation account mentioned in the Settlement condition.

The system updates the base currency sub-account as the default settlement account of the MCY arrangement. During MCY account creation, the base currency sub-account may be created automatically by the system or manually by the user subject to product configuration .

When the base currency sub-account is created:

- Automatically ( by the system) – The system defaults the base currency sub-account as the Def Account . This Def Account cannot be changed during MCY arrangement opening. The charges like new arrangement fees can be collected from the base currency sub account. Post creation of the MCY Account, the user can amend the default settlement account which could be any sub-account within the MCY structure or an AR (Retail Account) account outside MCY structure.
- Manually (by the user) – The system defaults the base currency as the default settlement account Def Account during base currency sub-account opening if the field is blank.

It is possible to specify a Payment Type specific settlement account for different type of charges. When an account is updated in Def Account or other settlement accounts, the system ensures that the accounting condition is available for the Charge Property Class in that account.

> **⚠️ Note:** When a charge is defined at time of arrangement opening, if automatic creation of sub-account is not defined, the settlement account should be updated by the user. Else, charges cannot be collected.


##### Illustrations

The following section illustrates how a scheduled or an activity charge can be set up during MCY creation, raised and settled from liquidation account.


###### Activity Charges

It is possible to collect an account opening fee as an activity charge at the time of MCY arrangement opening. As the base currency account has to be opened automatically, the charge is collected from the base currency sub-account. In the below example a MCY arrangement is created with a debit and credit charge defined during MCY account creation. The following are defined:

- A new arrangement activity charge of USD10 (debit charge)
- A bonus charge of USD 20 (credit charge) is defined during MCY account creation.
- Method is set as Capitalise.

These charges are capitalised to the base currency sub-account.

In the MCY arrangement, the charge and bill info details are shown below.

The debit and credit Bill Details Overview display the charge amount, corresponding settlement account ID and charge property name.

The charges are created at the MCY arrangement level and collected from the liquidation account level using the Generate Charges Activity as seen below:


###### Scheduled Charge

Consider a USD10 annual administrative fee scheduled in the MCY arrangement.

The settlement account gets automatically updated with base currency sub-account.

The Payment Schedule condition gets updated.

---


### 2.19  SubAccounts


> **📇 Quick Reference Card**
> 
> **Applications:** `AA.PRODUCT.DESIGNER`
> 
> **Key Fields:** *Activity Link*, *Allowed Product*, *Base Ccy Product*, *Master Arrangement*, *Product Only*
> 
> **Sections:** ⚙️ Configuration


#### ⚙️ Configuration

The sub-accounts are account arrangements created in the product defined in the Allowed Product field of Sub-Arrangement Rules of the MCY product. The linkage between sub-arrangements and a parent arrangement within a multi-currency (MCY) account is supported using the Master Arrangement field of AAA. In addition, information related to the connection between the two arrangements is updated in the Activity Link type field .

Refer to Configuration of AR Accounts for more details on the configuration of Sub-Accounts.

Refer to Configuration of AR Accounts for more details on the configuration of Sub-Accounts.

Further, the arrangement account product for the sub-account should have the Product Only field set as ‘Mcy’ in the AA.PRODUCT.DESIGNER . This setup specifies that this product is for MCY sub-accounts only and it allows the bank to differentiate between the features of regular current, savings and MCY sub-accounts.


##### Automatic Creation of Base Currency Sub-Account

When the MCY arrangement is created, the system can be configured to create the base currency sub-account automatically. The automatic account creation can be configured by setting up the Base Ccy Product field in Sub-arrangement Rules condition of the MCY arrangement. The product should be a MCY only Product in AR product line. When the user gives this (Base Ccy Product) product in the Sub-arrangement of the MCY product configuration (or at MCY arrangement level), the base currency sub-account creates automatically in this product as part of MCY account creation.


> **Related Applications:** `AA.PRODUCT.DESIGNER`

---


### 2.20  Limit Balance


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Limit Property Class can maintain the balance information of total sanctioned, utilised, unutilised and excess.*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

The Limit Property Class can maintain the balance information of total sanctioned, utilised, unutilised and excess.

- In case of a single limit, the information is maintained on the same account that is linked with the limit.
- In case of a shared limit, the user can maintain this information in one of the accounts that is linked with the limit (or) can make use of a dedicated account.

The Limit Property Class holds the account information that maintains the limit balance information.

When a limit is defined based on a time code, it is possible to maintain balance information based on time code definition. The user can choose to maintain time code balances in addition to the summary balances.

Since limit balance information is maintained as balance types, the user can calculate fees or charges corresponding to each balance. For instance, the user can calculate

- A charge on the total limit amount
- An interest on the utilised and unutilised amount
- A penalty interest on the overdrawn limit amount.

---


### 2.21  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *&#9432; Content migrated from existing User Guide. Was earlier available as lore ipsum.*
> 
> **Applications:** `AA.PAYMENT.TYPE`, `AA.PRODUCT.DESIGNER`, `AA.PRODUCT.GROUP`, `AA.PRODUCT.LINE`, `AA.PROPERTY`, `AA.PROPERTY.CLASS`, `EB.EVENTS`, `LIMIT` ... +1 more
> 
> **Key Fields:** *Mandatory*, *Optional*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- APIs
- Temenos Transact Services

&#9432; Content migrated from existing User Guide. Was earlier available as lore ipsum.

Retail Accounts (AR) is one of the modules under Arrangement Architecture (AA) umbrella of products and is part of the Temenos Retail Banking suite of products.

The AR module provides financial account functionality and its maintenance for a financial institution. The module allows the user to create current or checking and savings accounts using the AA framework, under the Accounts product line, and perform a series of related activities on it.

A few of the key functionality included are:

- Create a new account arrangement
- Perform credit or debit activity or transactions for the account
- Accrue credit or debit interest accruals
- Capitalise interest to account balances
- Monitor charges and commissions
- Monitor inactivity or dormancy
- Issue cheque book or passbook
- Issue mandates


##### Configuring Retail Accounts

The AA.PRODUCT.LINE application provides a high-level definition of the business components (property classes), required to construct a product belonging to that line.

A product line is described by the property classes which constitute it. A financial institution can use these building blocks (property classes) to construct individual products, which can then be made available for sale to its customers.

AR has the following property classes.

| Column 1 | Column 2 | Column 3 |
|---|---|---|
| ACCOUNT ACCOUNTING ACTIVITY.API ACTIVITY.CHARGES ACTIVITY.MAPPING ACTIVITY.MESSAGING ACTIVITY.PRESENTATION ACTIVITY.RESTRICTION ALERTS AGENT COMMISSION BALANCE.AVAILABILITY | BALANCE.MAINTENANCE CHANGE.PRODUCT CHARGE CHARGE.OVERRIDE CLOSURE CONSTRAINT CUSTOMER DORMANCY ELIGIBILITY FACILITY INTEREST INHERITANCE | LIMIT OFFICERS PAYMENT.RULES PAYMENT.SCHEDULE PAYOFF PAYOUT.RULES PERIODIC.CHARGES PRICING.RULES REPORTING SETTLEMENT STATEMENT TAX |

The AA.PROPERTY is an instance of AA.PROPERTY.CLASS and these components constitute an account product. The property classes and properties are made Mandatory or Optional based on the AA.PRODUCT.GROUP level but subject to the Product Line definition. The AA.PRODUCT.DESIGNER is used to create the Account Products required.


##### Illustrating Model Parameters

The product conditions of a property class are evaluated to bring out the features of the property class. The system defaults the values in the product condition in an arrangement during its creation. The negotiability or default values and other restrictions are also defined in the product condition. These product conditions along with the properties derived from the property classes are grouped together to build products.

The product conditions are dated and some of the product conditions have currency as part of their ID. When the currency forms a part of the product condition ID, the user needs to create different conditions for each currency in which the product is available. When a new condition is created or an existing one is amended, the product to which the condition is linked has to be proofed and published.

| S.NO | Parameters | Description |
|---|---|---|
| 1 | Account | The Account property class is used by all the products which are account based. This property class primarily controls the description of the account. The ACCOUNT property allows the user to define and control balance treatment, posting restriction, linked account number (for memo accounts), currency market, date convention related setup for the account. Although the account names are account specific, generic titles can be defaulted from the product and can be replaced or given additional detail at the arrangement level. Each product defined and processed in AA can have a single ACCOUNT Property defined. |
| 2 | Activity Charges | The Activity Charges property class defines the charges that have to be applied when a particular activity is triggered on the arrangement. The charges so applied can be made due, capitalised or deferred. The user can enable auto settle the charges made due from unallocated credit balance by setting this to Yes. In accounts, charges are enabled for dormancy, settle payoff and ageing. This property class is also extensively used for all AA related modules, charges are set for various other activities. |
| 3 | Activity Restriction | The Activity Restriction property class is used to specify a restriction on a particular transaction. The restriction rules including the relevant periodic attributes and activities are defined in the product condition. These rules are then used to define activity based or property based restrictions. A rule if broken can be set to result in an override or error. A charge can be attached for this and can be set to be made due, capitalised or deferred. For the AR module, activity restriction is extensively used for restricting transactions by number, type, and so on. This is also extensively used in other modules to restrict the user from doing various user activity based on the life cycle status of contracts. |
| 4 | Balance Availability | The Balance Availability property class allows the user to control the following features pertaining to AR module: Notice amount and period, which needs to be given by a customer for withdrawing money from his account. Default Credit Check and Available Balance update related set up. Activity class or Activity specific credit check, and NSF related fees pertaining to it Tolerance Amount or Tolerance Currency - To indicate the grace amount, which is the allowed overdraft before the bank imposes NSF or OD fees. Overdraft Grace Period - To waive the NSF fee levied on the account, if the customer clears the debit balance within the stipulated grace period. |
| 5 | Dormancy | The Dormancy property class allows the user to control the parameterisation of inactive or dormant accounts and movement of the same into various buckets at the arrangement or product level. The same can be controlled based on period, and some exceptions or rules also can be added for evaluation and movement. The user can include or exclude certain activity or activity class for the evaluation. It is possible to, Configure different Dormancy status based on the period of inactivity Specify different charges and charging frequency for each Dormancy status Apply some exception rule filtering at an individual arrangement level (for example, account is in debit balance) and such rules can either be an API or a rule created using the Rules Engine Specify notices and notice frequency for each Dormancy status Specify Activities or Activity Classes or Activity Initiation Types which are qualified to keep an account active. Auto Reset can be enabled based on status or on Activity Type. |
| 6 | Facility | The Facility is a service component for financial products designed using arrangement architecture. The Facility property class controls the list of available services for an arrangement account. When an external activity (financial or non-financial) is triggered and the corresponding service group is mapped to an activity through Activity Mapping and EB.EVENTS . And the same came allowed or restricted or charged corresponding error message is raised to stop the activity. |
| 7 | Inheritance | The Inheritance property class is used for BN pool structure for inheriting the product conditions set at Parent level arrangement to the Child level arrangement accounts. The product conditions that are set for inheritance are attached to Property records with type as Inheritance Only. The properties to be inherited can be controlled both at source and target level. |
| 8 | Interest | The Interest property class is used for all interest definition and processing in AA. A product defined and processed in AA can have multiple interest properties defined (for example, principal interest, penalty interest, commission, etc. Interest rates can be defined as fixed , floating , periodic or linked rate (referring an INTEREST property from other arrangement), routine based calculation. Tiered interest can also be defined. Further it is possible to define a negative rate, minimum interest amount and waive the interest. Interest adjustment can be done in run time, and adjustment related detail or values can be captured in adjustment related fields. |
| 9 | Limit | The Limit property class primarily controls the use of LIMIT module by the product. We can set up single or shared limit. We can define the LIMIT.REFERENCE applicable for a specific product such that the system defaults the same in an arrangement. For a new limit, at the arrangement level, the LIMIT.SERIAL has to be given as NEW. The AR module can have self-contained secondary limit without having actual limit attached to it. Overdraft status or notice for AR module is handled inside the Limit Property class. Further Limits can be set to use the LIMIT module (AL and AD) or it can be managed only within the arrangement architecture framework. |
| 10 | Payment Schedule | The Payment Schedule property class is used by all products which have amounts billed (that is,made due) or capitalised or Pay. A Payment Schedule can be comprised of one or more payment definitions with conditions such as payment Type and Method, arrangement properties, dates and amounts. The AA.PAYMENT.TYPE application is used to define the standard payment types such as constant, linear, actual and fixed equal and so on, that can be used by a product. This payment type is then attached to each payment schedule definition. The start and end date can be specified, the user can specify the repayment of arrangement to commence after ‘n’ months from the arrangement date or ‘n’ months before the maturity or ‘n’ months after the change product or reset and rollover has happened. |
| 11 | Periodic Charges | The Periodic Charges property class acts as a container to group different charge properties and calculate a periodic charge amount. The Payment Schedule property class drives this property class. A periodic charge property can be attached in payment schedule and on schedule date periodic charge amount is calculated. At the arrangement level adjustment can be done by the user on whole periodic charge. |
| 12 | Statement | The Statement property class is used to define the legacy ACCT.STATEMENT feature at the AA level. Statements may be produced daily (every working day), every 1-9 weeks, twice a month (on the 15th and the last day of the month) or every 1-12 months on any day of the month. Up to nine statement cycles may be specified for each account, and each statement cycle is independent. In addition to this, special interim statements can be enabled. This property class also controls whether or not advices are to be produced when interest and charges are applied, and whether detailed interest statements (interest scale) should be produced. Within a statement cycle, it is possible to define multiple frequencies with a combination of weekly and monthly, such that statements are produced on the dates specified by both frequencies, but only contain details of entries since the last statement in that cycle. |


##### Illustrating Model Products

The AR product line provides current and savings account functionalities. The module allows the user to create savings or current accounts using the AA framework under the Accounts product line.

| S.No | Product Name | Product Attributes |
|---|---|---|
| 1 | Current Accounts | Corporate account with fixed debit interest Regular current account with floating Interest for both debit and credit interest, amount based capping of NSF Charges and waivers during account closure Current account with periodic charge Current account limit secured by deposit Current account for staff with additional interest Account with predefined overdraft limit of USD 250 Premium current account with some restriction on balance, and activities Current with some SME related features enabled Current account for SME - self service account Current account for students Current account for bundling, and gaining additional benefit through bundle Fully negotiable account Master account collects the interest from the Sub account and pays the interest accordingly Sub account pays the interest to the master account according to the maintained balance Payroll Account with cashback and count based capping of NSF Charges. Current Account for elite customers where the cheque issue fee is waived based on the relationship of the customer with the bank. The pricing evaluation runs on multiple arrangements of the customer which are fetched from Holdings MS and only those arrangements which are not in Non-accrual basis status is selected for pricing. Transact must be integrated with Holdings MS and the extension data mapping for this criteria set is to be configured locally to use this feature in the model product. |
| 2 | Savings Accounts | Regular saving account with basic features Regular saving account with restriction in Interest capitalisation Savings account for child Savings account for non resident Regular salary savings account Traditional notice savings account Savings account for staff |
| 3 | Summary Accounts | Summary account Currency summary account |


> **Related Applications:** `AA.PAYMENT.TYPE`, `AA.PRODUCT.DESIGNER`, `AA.PRODUCT.GROUP`, `AA.PRODUCT.LINE`, `AA.PROPERTY`, `AA.PROPERTY.CLASS`, `EB.EVENTS`, `LIMIT`, `LIMIT.REFERENCE`

---


### 2.22  Chargeoff


> **📇 Quick Reference Card**
> 
> **Applications:** `AA.ACCOUNT.DETAILS`, `AA.ACTIVITY.HISTORY`, `AA.BILL.DETAILS`, `AA.INTEREST.ACCRUALS`, `CATEG.ENTRY`, `RE.CONSOL.SPEC.ENTRY`
> 
> **Key Fields:** *Bill Type*, *Charge Off Amount*, *Charge Off Percentage*, *Charge off Amount*, *Charge off Percentage*, *Full Chargeoff*, *New Property Amount*, *Or Prop Amt* ... +8 more
> 
> **Sections:** 🔧 Working With


#### 🔧 Working With

Working with Loan Charge-off Key Features Charge-off is different from writing off the arrangement. The key features of charge-off are: A full or multiple partial charge-off transaction is possible. The interest on the charge-off balance should accrue, but is not passed to income. Reversal of charge-off transactions is possible Removal from charge-off or partial removal from charge-off (that is, a lessening of the charge-off amount) is possible as well. Dual accounting –that is, having two sets of books, the customer record vs. the bank record and applying payments independently to the two records. The charge-off feature is available for the Lending Product Line. The Charge-off Property has to be included in the product for charging off an account. Activity Class - Charge-off Full/Complete Charge-off The LENDING-CHARGEOFF-ARRANGEMENT Activity Class is used for charge-off of an arrangement. The complete outstanding in the loan is charged off. Partial Charge-off or Charge-off in Parts It is possible to charge off a loan, in parts. The LENDING-CHARGE-OFF-ACCOUNT Activity Class is used to charge-off the Account Property balance, based on the charge-off order. This is used to both charge-off an amount of principal (that is, increase charge-off amount) and to reduce the charge-off (that is, decrease the charge-off amount) if required. If a loan is being charged-off for the first time, this Activity is responsible for creating the charge-off balances as well as the customer’s shadow balances. Handling Charge-off under FASB Regulations For handling charge-off under certain specific regulations (FASB), the bank user uses the CHARGEOFF-REPORTING activity. Dual Accounting For loan contracts, apart from the customer balances, it is possible to store two separate balances, the bank balances along with the charge-off balances. When a Lending Product with Charge-off Property is proofed and published, the system automatically creates the balance type records to maintain charge-off balances along with the customer and bank balances. For a loan that is charged off, for CUR , the balances prior to the Charge-off Activity is stored as a shadow CUR CUST. The charge-off amount is stored in CUR CO and the amount under banks book is stored as CUR . The CUR CO charge-off balance, is the contingent balance and CUR CUST is a balance used for internal purpose and CUR is only non-contingent in nature. When the LENDING-CREDIT-ARRANGEMENT activity is processed, the amount credited to UNC is also credited to UNC CUST. When the LENDING-DEBIT-ARRANGEMENT activity is processed, the amount debited from UNC is also be debited from UNC CUST. Shadow Balances When a loan is charged-off, the borrower is unaware of this action, and continues to receive regular billing notices. As a result, when a loan is fully or partially charged off there is a situation to maintain two sets of books: A customer record (that is, the customer’s view of the balances and bills) A bank record (that is, the bank’s view of the balances). Prior to the charge-off, the customer and the bank records are the same (and therefore there is only one set of books). However once a loan is partially or fully charged off, the views are different. Customer Record Banks generally don’t communicate charge-off decision to the customers. So, a customer is unaware of a charge-off. Copying the balances prior to the Charge-off Activity creates a shadow record. This now becomes the customer record and does not include any of the effects of the charge-off. The bills and payments continue to be processed normally against this customer record. The payments received have to be apportioned as per the Payment Rules according to the customer. The customer balances are apportioned in this repayment order. Bank Record Full/Complete Charge-off For a full or complete charge-off using the LENDING-CHARGEOFF-ARRANGEMENT activity, there are no bank balances. The BNK balances are zero in this case. Charge-off in Parts/Partial Charge-off A charge-off creates the shadow balances for the customer record that do not include the effects of the charge-off (that is, the customer is completely unaware). As a result, the existing balances (customer balance less charge-off amount) continue to be referred to as the bank record and includes the effects of the charge-off (for example, the charged-off balance). As the arrangement advances, it also contains the interest accrual on the bank balance and charged-off balance separately. Additionally payments to the loan are allocated in a different manner on the bank record than on the customer record. This is based upon the value of the book balances and the status of the loan (for example, partially charged-off, fully charged-off or non-accrual). Internal inquiry screens display both the customer and the bank record, once a loan is partially or fully charged off. Reports breakdown the information this way as well – including both the bank balances and the customer balances. Charge-Off Balances The CUR CO and each ACC CO balance corresponds to the charge-off balance for the principal and the interest respectively. The system creates these balances by appending a CO at the end of each balance type. Multiple Interest Accruals For a full charge-off, the system accrues interest for charge-off and the customer balances namely CO and CUST balances. There is no bank balance to accrue interest for the BNK balances. For a partial charge-off (charge-off in parts), the system accrues interest for bank balance (for example, CUR ), charge-off and the customer balances. The system also accrues interest for the chargeoff and customer balances namely CO and CUST balances. It is necessary to accrue both charge-off and customer interest on the corresponding balances separately. Full/Complete Charge-off During a full charge-off, the arrangement balances are moved to the Chargeoff PL. As part of shadow accounting, CUR CUST and CUR CO balances are maintained during a full Chargeoff. This results in the accrual of balances per Interest Property for each of this principal balance. Each of them accrues interest at the same rate but based upon their balance. ACC CUST is accrued on CUR CUST and ACC CO is accrued on CUR CO. Though multiple interest accruals are done based on different balances, definition of source balance for each type of accrual is not required. Product configuration contains: Property Source INTEREST CURACCOUNT Corresponding Accruals in a full charge-off loan are: Balance Source ACCINTERESTCO CURACCOUNTCO ACCINTERESTCUST CURACCOUNTCUST Partial Charge-off or Charge-off in Parts In a partial charge-off, there are three balances: CUR , CUR CUST, CUR CO. Hence, there are three accrual balances per Interest Property and each accrues interest at the same rate but based upon their balance. ACC is accrued on CUR then ACC CUST is accrued on CUR CUST. Though multiple interest accruals are done based on different balances, definition of source balance for each type of accrual is not required. The interest is calculated on: Property Source INTEREST CURACCOUNT Corresponding accruals in a partial charge-off loan are: Balance Source ACCINTEREST CURACCOUNT ACCINTERESTCO CURACCOUNTCO ACCINTERESTCUST CURACCOUNTCUST Product Setup and Charge-off Balances When a Lending Product with Charge-off Property is proofed and published, the system automatically creates the below balance type records to maintain customer, bank and charge-off balances. Except bank balances, other balance type records which are created by system are contingent in nature. Bank Balances Charge-off Balances Customer Balances CUR CUR CO CUR CUST DUE DUE CUST CUST UNC UNC CUST ACC ACC CO ACC CUST DUE DUE CUST CUST CUR CO balance type holds the cumulative amount that’s been charged-off against an account. ACC CO balance type is used for posting the accrued interest on charged-off balances namely CUR CO. Dual Billing In the case where a loan is in Charge-Off status, AA.BILL.DETAILS is updated with both the customer and the bank due amounts. For a complete charge-off, the reflection of the charge-off billing is found in the billed balances. The bank amount is zero For a partial charge-off, two sets of figures (the customer and bank amounts) are calculated and stored on the bill. The customer and the bank amounts differ due to the effect of the charged-off principal as well as the alternate way of applying credits to the arrangement. Illustration of Partial Charge-off The changes that happen in an arrangement when a charge-off is performed is illustrated with the help of the below example. The arrangement is in delinquent status and is being charged off using the LENDING-CHARGEOFF-ACCOUNT Activity giving the transaction amount as 80,000 USD. This means 80,000 USD of principal is charged off. The Loan Arrangement Overview is displayed below. The Charge-off Activity is shown below. The Loan Arrangement Overview After Charge-off is shown below. Comparison of Arrangement Balances Before And After Charge-off The ECB balances before charge-off of 80,000 is shown below. The ECB balances after charge-off of 80,000 is shown below. Note that the arrangement balances have changed as a result of the charge-off. Bill Generated Before/After Charge-off On bill generation, AA.BILL.DETAILS is updated with both the customer and the bank due amounts for each of these accruals. AA.BILL.DETAILS stores the bank related fields that get updated on and after the charge-off of an arrangement. Once the charge-off is done, then the customer balances are stored in existing amount related fields and bank balances are stored in the BNK (bank) fields. Overdue processing is triggered based on the bills getting aged. The Os Prop Amt and Or Prop Amt fields of the bill are based on the customer balances(original amount) and regular overdue processing is triggered for the same. Balance type AA.BILL.DETAILS CUR Os Prop Amt Bnk Or Prop Amt Bnk CUR CUST Os Prop Amt Or Prop Amt Key Features of Full/Complete Charge-off A complete charge-off is done using the LENDING-CHARGEOFF-ARRANGEMENT activity. After a complete charge-off is made in the arrangement, the Full Chargeoff field in the AA.ACCOUNT.DETAILS application displays Yes. During charge-off, the loan principal is charged off to the PL Category assigned to the Account property class. The interest is charged off to the PL Category assigned to the Interest property class. Any tax is charged-off to the PL Category assigned to the Tax property class. Validations During a Complete Charge-off When this activity is executed, the system performs the below validations and results in error in below scenarios: The bank performs the charge off after clearing any outstanding credit balances of the loan (like UNC/INV/AVL). Hence if there are any credit balances available during a charge-off, the system raises the following error. When there is a charge with outstanding pay balance, the arrangement cannot be charged off. The pay balance must be cleared and then charge-off should be triggered in the system. Post charge-off, the banks do not prefer to disburse any further loans or increase the loan commitment further. Hence, the disbursement activity is not allowed after the charge off. During the cooling and cancel period, the loan charge-off is not allowed. Any income to the arrangement is booked to the Chargeoff PL of that Property An arrangement that has undergone partial charge-off can undergo full charge-off, but an arrangement that is completely charged off cannot be charged off further. Loans cannot go to negative rate when loan is in charge-off. Dormant loans cannot be charged off. When an arrangement has a charge set to amortise, the charge cannot be charged off. The system raises an error when the user tries to do a full charge-off when there is a charge amortisation in progress. During charge-off, the system calculates the penalty interest if this has been configured and this helps the bank to access the real charge-off amount for all the property. Illustration of Charge-off Consider a loan that has few bills outstanding and is delinquent. Perform a charge-off. The charged-off arrangement is shown below. The charge-off information in AA.ACCOUNT.DETAILS is as shown below. Arrangement Balances Movement The loan principal balances and billed interest balances are moved to Chargeoff PL and are stored in CO and CUST balances as off-balance sheet items. Here, the sum is: ACCPRINCIPALINTCO=ACCPRINCIPALINTCUST+DELPRINCIPALINTCUST CURACCOUNTCO=DELACCOUNTCUST+CURACCOUNTCUST Bills A bill that was already generated is also updated with the charge-off information. In a full charge-off, the BNK balances for the Property after charge-off is zero. The billed amount and outstanding balance here represents the CUST balance, as shown below Interest Accruals After a charge-off, the interest accruals are under CUST and CO balances. Charge Bills Charge-Off An arrangement with interest and charge bills is being fully charged off, including all interest and charges in the bills along with outstanding principal. Any Activity Charge, Periodic Charge and Rule break charge are also charged off. This is subject to certain evaluation: The system evaluates if there are any pay charges outstanding and raises an error to indicate that the same must be settled. The system evaluates if there is charge collected that is undergoing amortisation, then the system doesn’t allow to charge off that arrangement. Consider an arrangement that has been charged off. During a charge-off, charge bills are also charged off. A rule break that is being charged off is shown below. The balances after the charge-off, also reflects the charges being charged off. Accounting for Charges in Charge-off RE.CONSOL.SPEC.ENTRY is generated during the charge-off of the principal decrease fee, a rule break fee. For charge-off books it is as shown below. For customer books it is as shown below. Activity Charge for charge-off books is shown below. Activity Charge for customer books is shown below The charge-off entries for the charge debited in the banks PL are as follows: For the Rule break fee: For the Activity Charge: Charge-off of Upfront Profit Contracts It is possible to setup upfront profit in loan arrangements. For such a loan, the interest is collected upfront and is booked to the PL over a period as accruals. Read Islamic Finance-Upfront Sale for more information. The below arrangement has upfront bills with outstanding bills. This arrangement has a profit amount of 10,000 USD that is collected for a year’s tenure. The upfront profit is booked between RECDEFERREDPFT and ACCDEFERREDPFT at the time of booking the arrangement. DR RECDEFERREDPFT -10,000 CR ACCDEFERREDPFT 10,000 During accruals, the profit is booked between ACCDEFERREDPFT and PL DR ACCDEFERREDPFT -48.84 CR PL 48.84 The accruals for the month are -1513.79 and the balance in ACCDEFERREDPFT is 8486.21 at the end of month. On the due date of the profit, the accruals of the month are posted to the RECDEFERREDPFT from DUEDEFERREDPFT DR DUEDEFERREDPFT -1513.79 CR RECDEFERREDPFT 1513.79 As a result of this, RECDEFERREDPFT has a balance of -8486.21 Time Head Movement Balances Creation RECDEFERREDPFT -10,000 -10,000 Creation ACCDEFERREDPFT 10,000 10,000 Monthly Accrual ACCDEFERREDPFT -1513.79 8486.21 Due date RECDEFERREDPFT 1513.79 8486.21 Illustration of Charge-off Upfront Profit The arrangement is now charged off. The balances from CURACCOUNT have moved to CURACCOUNTCO. A part of the principal amount is billed already. So CURACCOUNTCUST+DELACCOUNTCUST amounts to the total principal. The bill is in delinquent status from the customer perspective and the balance is stored in DELDEFERREDPFTCUST as -1513.79. The RECDEFFEREDPFTCUST gives the outstanding amount as per customer, -8,486.21 that is pending receivable. There are four days accrual after the last bill date for 180.38 that has resulted in the ACCDEFERREDPFTCUST is 8305.83 (8,486.21-180.38). Time Head Movement Balances Creation RECDEFERREDPFT -10,000 -10,000 Creation ACCDEFERREDPFT 10,000 10,000 Monthly Accrual ACCDEFERREDPFT -1513.79 8486.21 Due date RECDEFERREDPFT 1513.79 8486.21 4 days accruals after due date ACCDEFERREDPFT -180.37 8305.83 Repayment in the Charge-Off Loan A repayment received in the upfront profit loan arrangement is allocated as per the payment rule given below. The balances of the same loan arrangement after a couple of days are; Time Head Movement Balances Creation RECDEFERREDPFT -10,000 -10,000 Creation ACCDEFERREDPFT 10,000 10,000 Monthly Accrual ACCDEFERREDPFT -1513.79 8486.21 Due date RECDEFERREDPFT 1513.79 8486.21 6 days accruals after due date ACCDEFERREDPFT -270.56 8215.64 The same update is in the AA.INTEREST.ACCRUALS as shown below. A payment of 5000 on the arrangement and this is apportioned against the CUST and CO balances as per the Payment Rules and Chargeoff Rules respectively. In customer perspective, the Payment Rules apportions the payment towards to DEFFEREDPFT first and then the ACCOUNT Property as seen below. The same is reflected in arrangement balances as shown below. In charge-off perspective, the repayment works as explained below. The Charge-off condition governs the repayment rule for charge off balances. The Charge-off condition for the upfront profit loan is given below. In this arrangement, the loan is fully charged off. So the Billed and Current Balance Type options do not have any impact and the system apportions the payment for the CHARGEOFF balance type. Thus, the full payment of 5000 is apportioned to the ACCOUNT balance. This can be seen in the screenshot below. In banks’ books repayment is as explained below. The repayment is received in the banks’ book against the CHARGEOFF PL as indicated in Accounting Condition. The repayment of 5000 is credited to the PL indicated in this accounting condition as seen below. Charge-off in Charge Component - Upfront Profit Contract In the contract below, a charge booked at the time of arrangement creation is shown. The impact on the charge bill during a charge-off is shown in the subsequent screenshots The arrangement balances before a charge-off are shown below. The arrangement balances after charge-off as shown below. A comparison of the bill details before and after the charge-off is shown below: The accounting entries in charge-off are as follows: The charge-off entry in the PL, is a debit to the banks PL as seen in CATEG.ENTRY . The charge-off entries to bank and customer books are as RE.CONSOL.SPEC.ENTRY . In the charge-off books, the CO entry is as shown below. In the customer books, the CUST entry is as shown below.

In a business situation where the bank user must capture a bill in a loan that has undergone charge-off, the user can do so with the capture bill (LENDING-CAPTURE.BILL-BALANCE.MAINTENANCE) activity on such a loan. This activity can be used only for the arrangement that has undergone a full charge-off (LENDING-CHARGEOFF-ARRANGEMENT). As a result of this bill capture activity, the system releases the bill and balances in the customer books and the charge-off books.

Consider a scenario of dispute with the customer and the contract is charged off. The bank prefers to collect some charges or re-raise a bill that was previously paid, due to a customer dispute. In this case, the bank user can capture the bill and record it as an outstanding amount with the customer.

Consider a loan that is fully charged off using the LENDING-CHARGEOFF-ARRANGEMENT activity. The balances charged-off include the principal and interest as highlighted below.

- Charge-off principal - 46,369.61 (Outstanding principal).
- Charge- off interest - 31.62 (Accrued interest amount after the first installment).

This loan has only one installment bill which is already settled.

In this example, the client has raised a dispute with the bank on the 3871.49 bill dated Apr 12, 2023. So, the bank decides to refund the bill. At a later date, the claim is proved false and the bank wanted to raise the bill with the same amount for the customer.

The user captures the bill in this charged-off loan using the LENDING-CAPTURE.BILL-BALANCE.MAINTENANCE activity. The details of Bill Type , Payment Type , Payment Method , Payment amount , Property , Original Property Amount , and New Property Amount are entered based on the first installment bill details.

Though the bill is to claim the dues that were refunded earlier, the capture bill can be raised only for the current value date (not forward or back-valued) for the required payment type, bill type, and the bill amount for the components required. The bill date must also be the current date (not forward or back-valued).

Post capture bill activity, a due bill is created, and the system automatically updates the respective charge-off balances and customer balances in ECB.

Post capture bill activity:

- The charge-off principal is updated as 50000 (46169.61 + 3830.39)
- The charge-off interest is updated as 72.72 (31.62 + 41.10).

When an activity is triggered back-valued after this capture bill activity, the capture bill activity is also effectively reversed and replayed. As the bill is a manually created bill, the components of the bill do not undergo a change but the bill is reversed and replayed staying unaffected.


##### Handling Charge-off under FASB Regulations

In order to provision loan under FASB, the user can trigger the LENDING-CHARGEOFF-REPORTING activity and specify the required charge-off amount or percentage.

Consider a delinquent loan with the balances stated below.

The user triggers the Charge Off Reporting activity from the New Activities menu on the loan overview screen.

The user inputs the required Charge off Amount for partial charge-off of the loan.

> **⚠️ Note:** To achieve partial charge-off, either the Charge Off Amount or Charge Off Percentage attribute can be used. In case a percentage is specified, the percentage is converted into amount and stored.

Charge off details updated in AA.ACTIVITY.HISTORY are shown below:

Charge off details updated in AA.ACCOUNT.DETAILS are shown below:

Consider a delinquent loan with the balances stated below.

The user prefers to fully charge-off the loan and provides the Charge off Percentage as 100.

The charge off details updated in AA.ACTIVITY.HISTORY are shown below.

The percentage is converted to amount by an API and stored.

Charge off details updated in AA.ACCOUNT.DETAILS are shown below:

> **⚠️ Note:** Only during a full charge-off the Full Chargeoff attribute is updated as Yes.

| AA Activity | IFRS Operation | Description |
|---|---|---|
| LENDING-IFRS.CHARGEOFF-REPORTING | CHARGE OFF | Indicates the loan is charged-off for the first instance. |
|  | CHARGE OFF INCREASE | Indicates loan is charged- off for an additional amount from earlier levels. |
|  | CHARGE OFF DECREASE | Indicates loan charge-off amount is decreased by specifying a negative amount. |
| LENDING-APPLYPAYMENT-PAYMENT.RULES ENDING- | RECOVERY | Indicates a repayment made on the loan. |
| LENDING-WRITE.OFF-BALANCE.MAINTENANCE | WRITE OFF | Indicates loan has been completely written off |
|  | WRITE OFF PARTIAL | Indicates a partial write off scenario which instead of entire loan only certain bills and/or balances are written off on contract. |
|  | ADJUSTMENT | Indicates any bill and/or balance adjustments made on the contract. |
| LENDING-MATURE-ARRANGEMENT | MATURE | Indicates loan has matured |
| LENDING-RESUME-ARRANGEMENT | RESUME | Indicates loan is resumed |

The following section provides examples of using SUSPEND.STATUS and CHARGEOFF.STATUS periodic attributes

The SUSPEND.STATUS periodic attribute allows the user to evaluate if loan is suspended or not and suitably configures any activity restrictions based on the suspense status of the loan. The evaluation is done based the suspend information stored in AA.ACCOUNT.DETAILS and allows the bank user to configure an error/override in the Activity Restriction condition.

Consider an example in which user needs to restrict a charge-off operation on a performing loan which is not suspended. If this periodic attribute is configured at product or arrangement level, then a user cannot trigger the charge off activity on a loan which is not suspended.

A rule is configured to check if the loan is in suspended status or not.

The rule is evaluated when an activity (charge off activity is considered in the case below) is triggered and based on the evaluation result an override (or error) is raised. Additionally, a rule break charge is applied if necessary.

This periodic attribute allows the user to evaluate and place activity restrictions based on the charge off status of the loan. This evaluates the charge off information in AA.ACCOUNT.DETAILS and allows the bank user to configure an error/override in Activity Restriction condition, based on the charge off status of the loan.

Consider an example in which user needs to restrict a resume operation on a charged-off loan. If this periodic is configured at product or arrangement level, then the user cannot trigger resume on a loan which is fully and/or partially charged-off.

A rule is configured to check if the contract is in suspended status or not. The rule can be configured to evaluate if loan is fully or partially charged-off.

The rule is evaluated when an activity (resume activity is considered in the case below) is triggered and based on the evaluation result an override (or error) is raised. Additionally, a rule break charge is applied if necessary.


> **Related Applications:** `AA.ACCOUNT.DETAILS`, `AA.ACTIVITY.HISTORY`, `AA.BILL.DETAILS`, `AA.INTEREST.ACCRUALS`, `CATEG.ENTRY`, `RE.CONSOL.SPEC.ENTRY`

---


### 2.23  Charges


> **📇 Quick Reference Card**
> 
> **Applications:** `EB.ACCRUAL`
> 
> **Key Fields:** *Start Date*
> 
> **Sections:** 🔧 Working With


#### 🔧 Working With

The following are different scenarios encountered while processing loan charges.


##### Charge Currency Different from Arrangement Currency

When the charge currency is different from arrangement currency , an override message is displayed as below.


##### Rule Break Charges

The below screenshot displays the Arrangement Overview.

The Term Amount increases AA activity and the associated override message is seen when the activity is committed.

Changes can be seen in the Total Commitment and the charges that were associated with the increase in Term Amount can be seen.


##### Amortisation of Charges

Once an arrangement has been created, an EB.ACCRUAL record is created per configuration for the amortisation process. Each record shows certain information, such as the daily accrual to date and the start and the end date of accrual.

The below screenshot displays EB.ACCRUAL record.


##### Stop Suspend / Resume Amortisation of Charges

Consider a loan product with Processing Fee (Debit charge) of $100 fee collected from customer upfront and amortised from the loan creation date until maturity. Loan Term is 100 days. The daily amortised fee amount is $1.

The fee amortisation is set to Stop Suspend from the day the loan is moved to non-performing stage. The amortisation of the said Processing Fee when the charge is Stop Suspend is tabulated below. The amortisation of the fee for Suspend charge type is also illustrated to draw comparison between the accounting entries booked against both charge types.

| TERM DAYS | SUSPEND | STOP.SUSPEND |
|---|---|---|
| Day 1 | Dr ACC 100 Cr P/L 0 | Dr ACC 100 Cr P/L 0 |
| Day 5 (COB) | Dr ACC 95 Cr P/L 5 | Dr ACC 95 Cr P/L 5 |
| Day 60 (COB) | Dr ACC 40 Cr P/L 60 | Dr ACC 40 Cr P/L 60 |
| Day 61 | Loan moved to ‘Non-Performing’ status |  |
| Day 61 (COB) | Dr ACC 39 Cr P/L 60 Cr ACC SP 1 | Amortization is stopped until Resume is triggered. |
| Day 80 (COB) | Dr ACC 20 Cr P/L 60 Cr ACC SP 20 | Amortization is stopped until Resume is triggered. |
| Day 81 | Loan Resumes to 'Performing' status |  |
| Day 81 (COB) | Dr ACC 19 Cr P/L 81 Cr ACC SP 0 | Dr ACC 38 Cr P/L 62 |
| Day 91 (COB) | Dr ACC 9 Cr P/L 91 | Dr ACC 18 Cr P/L 82 |
| Day 100 (COB) | Dr ACC 0 Cr P/L 100 | Dr ACC 0 Cr P/L 100 |


##### Suspend or Resume Accrual or Amortisation of Credit Charge

Consider an example where a loan product is set with a Charge property that is payable (Credit type) and set to Suspend. The charge is set to be amortized until maturity.

For illustration, the arrangement created for this loan product with Agent Expense (Credit charge) with a Pay bill for $100. The amortisation is configured for $1 daily and set to happen from the loan creation date until maturity. Loan Term is 100 days. Assume the charges are booked upfront and amortized over the term.

Further, the amortisation of the charge is set to Suspend from the day the loan becomes non-performing.

The below illustration tabulates the amortisation of the said ‘Agent Expense’ when the charge is Suspend. The amortisation of a debit charge with property type Suspend is also illustrated to draw comparison between the accounting entries booked against both credit and debit charge.

- ACC represents unamortized fee balance.
- ACC SP represents suspended fee balance.
- Income P/L represents the income account/head into which fee income is amortized.
- ACC represents unamortized agent expense balance.
- ACC SP represents suspended expense balance.
- Expense P/L represents the expense account/head into which expense is amortized.

All amounts in the table below indicate closing balances under the respective heads. Assume income and expense heads are zero to begin with.

| TERM DAYS | AMORTISATION OF CREDIT CHARGE[BG1] [SN2] | AMORTISATION OF DEBIT CHARGE |
|---|---|---|
| Day 1 | Expense P/L 0 ACC -100 | ACC 100 Income P/L 0 |
| Day 5 (COB) | Expense P/L -5 ACC -95 | ACC 95 Income P/L 5 |
| Day 60 (COB) | Expense P/L -60 ACC -40 | ACC 40 Income P/L 60 |
| Day 61 | Loan Suspended due to ‘Non-Performing’ status |  |
| Day 61 (COB) | Expense P/L -60 ACC -39 ACC SP -1 | ACC 39 Income P/L 60 ACC SP 1 |
| Day 95 (COB) | Expense P/L -60 ACC -5 ACC SP -35 | ACC 5 Income P/L 60 ACC SP 35 |
| Day 96 | Loan Resumes to 'Performing' status |  |
| Day 96 (At Resume) | Expense P/L -95 ACC -5 ACC SP 0 | ACC 5 Income P/L 95 ACC SP 0 |
| Day 96 (COB) | Expense P/L -96 ACC -4 ACC SP 0 | ACC 4 Income P/L 96 ACC SP 0 |
| Day 100 (COB) | Expense P/L -100 ACC 0 ACC SP 0 | ACC 0 Income P/L 100 ACC SP 0 |


##### Income Recognition Using Cost-Recovery Method

Read Income Recognition Under Cost Recovery Method section in Interest property class for more information on the underlying configuration.

Consider the following example where a contract is booked with the following details.

- Tenure -150 Days.
- Per-day daily accrual in the account - 1.
- Interest property type for PRINCIPALINT - SUSPEND,SUSPENDOVERDUE,AMORT RECOVERY SUSPEND.
- Interest property type for PENALINT - SUSPEND, AMORT RECOVERY SUSPEND.

The following table shows how the income recognition works under Cost-Recovery method:

| Activity | Principal Interest (Set to Suspend Overdues) | Remarks for Principal Interest balance movement | Penal Interest (Set to Suspend) | Remarks for Penal Interest balance movement |
|---|---|---|---|---|
| Day 1 | Accrued Principal Interest [ACC PRINCIPAL INT] – 0 P/L - 0 | Daily Accruals happen from Day 1 to day 90 | Accrued Penalty Interest [ACC PENALINT] – 0 P/L - 0 |  |
| Day 10 | ACC PRINCIPALINT – 10 Dr P/L – 10 Cr |  | ACC PENALINT – 0 P/L - 0 |  |
| Day 90 | ACC PRINCIPALINT – 90 Dr P/L – 90 Cr |  | ACC PENALINT – 0 P/L - 0 |  |
| Day 91 – Loan suspend due to prolonged delinquency | ACC PRINCIPALINT – 90 Dr Suspended Principal Interest ACC PRINCIPALINT SP – 90 Cr P/L - 0 | On Day 91, the loan is suspended. The balance from P/L is moved to ACCPRINCIPALINTSP | ACC PENALINT – 0 Suspended Penalty Interest ACC PENALINT SP – 0 P/L - 0 |  |
| Day 100 | ACC PRINCIPALINT – 100 Dr ACC PRINCIPALINT SP – 100 Cr |  | ACC PENALINT – 10 Dr ACC PENALINT SP – 10 Cr | Daily Accruals for PENALINT happen from Day 100 |
| Day 101 – Repayment 35 | ACC PRINCIPALINT – 70 Dr Repayment applied as per payment rule to due interest ACC PRINCIPALINT SP – 70 Cr Based on repayment amount 30 debited from SP and credited to IAP Interest applied to principal [RSP PRINCIPALINT] – 30 Cr P/L - 0 | Repayment of principal interest is done on Day 101. The balance from ACCPRINCIPALINTSP is moved to RSP PRINCIPALINT | ACC PENALINT – 5 Dr Repayment applied as per payment rule to due interest ACC PENALINT SP – 5 Cr Repayment amount of 5 debited from SP and credited to IAP Interest applied to principal [RSP PENALINT] – 5 Cr P/L - 0 | Repayment of penal interest is done on Day 101. The balance from ACC PENALINTSP is moved to RSP PENALINT |
| Day 110 EOD | ACC PRINCIPALINT – 80 Dr ACC PRINCIPALINT SP – 80 Cr RSP PRINCIPALINT – 30 Cr P/L - 0 |  | ACC PENALINT – 15 Dr ACC PENALINT SP – 15 Cr RSP PENALINT – 5 Cr P/L - 0 |  |
| Day 111 – Repayment 95 (principal interest – 80 and penal interest - 15) | ACC PRINCIPALINT – 0 ACC PRINCIPALINT SP – 0 RSP PRINCIPALINT – 110 Cr P/L – 0 |  | ACC PENALINT – 0 ACC PENALINT SP – 0 RSP PENALINT – 20 Cr P/L - 0 |  |
| Day 111 – RESUME | ACC PRINCIPALINT – 0 ACC PRINCIPALINT SP – 0 RSP PRINCIPALINT – 0 Amortization record (ACR) generated for RSP balance. ACR PRINCIPALINT – 110 Cr Straight line amount calculated at 110/40 = 2.75 per day P/L – 0 | On day 111 the loan is resumed. Amortization record is generated for RSP. The balance is moved from RSP PRINCIPALINT to ACR PRINCIPALINT | ACC PENALINT – 0 ACC PENALINT SP – 0 RSP PENALINT – 0 Amortization record (ACR) generated for RSP balance ACR PENALINT – 20 Cr Straight line amount calculated at 20/40 = 0.50 per day P/L - 0 | On day 111 the loan is resumed. Amortization record is generated for RSP. The balance is moved from RSP PENALINT to ACR PENALINT |
| Day 111 EOD | ACC PRINCIPALINT – 1 Dr ACC PRINCIPALINT SP – 0 RSP PRINCIPALINT – 0 ACR PRINCIPALINT – 107.25 Cr P/L – 3.75 Cr [1 from daily accrual and 2.75 from recovery interest] | Straight line amount calculated at 110/40 = 2.75 per day ACR PRINCIPALINT is debited by 2.75 and Income a/c is credited. | ACC PENALINT – 0 ACC PENALINT SP – 0 RSP PENALINT – 0 ACR PENALINT – 19.50 Cr P/L – 0.50 Cr [from recovery interest] | Straight line amount calculated at 20/40 = 0.50 per day ACR PENALINT is debited by 0.50 and Income a/c is credited |
| Day 120 EOD | ACC PRINCIPALINT – 10 Dr ACC PRINCIPALINT SP – 0 RSP PRINCIPALINT – 0 ACR PRINCIPALINT – 82.5 P/L – 37.5 [10+27.50] |  | ACC PENALINT – 0 ACC PENALINT SP – 0 RSP PENALINT – 0 ACR PENALINT – 15 P/L – 5 |  |
| Day 130 EOD | ACC PRINCIPALINT – 20 Dr ACC PRINCIPALINT SP – 0 RSP PRINCIPALINT – 0 ACR PRINCIPALINT – 55 P/L – 75 [37.50+10+27.50] |  | ACC PENALINT – 0 ACC PENALINT SP – 0 RSP PENALINT – 0 ACR PENALINT – 10 P/L – 10 |  |
| Day 131 – Loan Suspend due to market conditions – EOD | ACC PRINCIPALINT – 21 Dr ACC PRINCIPALINT SP – 21 Cr [20+1] RSP PRINCIPALINT – 0 ACR PRINCIPALINT – 52.25 ACR PRINCIPALINT SP – 2.75 P/L – 55 (20 reversed to ACC SP) | Loan is suspended from day 131. The property PRINCIPALINT is configured as “SUSPEND OVERDUES”. The income which is booked so for is reversed to ACCSP. P/L is debited and ACC PRINCIPALINT SP IS credited. | ACC PENALINT – 1 Dr ACC PENALINT SP – 1 Cr RSP PENALINT – 0 ACR PENALINT – 9.50 ACR PENALINT SP – 0.50 P/L – 10 | Here the PENALINT property is configured as ‘SUSPEND’. Here no income is booked so far and hence reversal is not required. |
| Day 140 EOD | ACC PRINCIPALINT – 30 Dr ACC PRINCIPALINT SP – 30 Cr RSP PRINCIPALINT – 0 ACR PRINCIPALINT – 27.5 ACR PRINCIPALINT SP – 27.5 P/L – 55 |  | ACC PENALINT – 10 Dr ACC PENALINT SP – 10 Cr RSP PENALINT – 0 ACR PENALINT – 5 ACR PENALINT SP – 5 P/L – 10 |  |
| Day 141 – Repayment – 40 (30 repaid towards Principal Interest+10 repaid towards Penal Interest) | ACC PRINCIPALINT – 0 ACC PRINCIPALINT SP – 0 RSP PRINCIPALINT – 30 Cr ACR PRINCIPALINT – 27.5 Cr ACR PRINCIPALINT SP – 27.5 Cr P/L – 55 |  | ACC PENALINT – 0 ACC PENALINT SP – 0 RSP PENALINT – 10 Cr ACR PENALINT – 5 Cr ACR PENALINT SP – 5 Cr P/L – 10 |  |
| Day 141 – Resume 2nd time | ACC PRINCIPALINT – 0 Dr ACC PRINCIPALINT SP – 0 Cr RSP PRINCIPALINT – 0 ACR PRINCIPALINT – 85 Cr (27.5+27.5+30) ACR PRINCIPALINT SP – 0 P/L – 55 | Each time resume is triggered, based on RSP and ACRSP balance a new amortization record is generated in EB Accrual application. | ACC PENALINT – 0 Dr ACC PENALINT SP – 0 Cr RSP PENALINT – 0 ACR PENALINT – 20 (5+5+10) ACR PENALINT SP – 0 P/L – 10 |  |
| Day 141 EOD | ACC PRINCIPALINT – 1 Dr ACC PRINCIPALINT SP – 0 Cr RSP PRINCIPALINT – 0 ACR PRINCIPALINT – 76.5 Cr Amortization resumed at 85/10 =8.50 per day ACR PRINCIPALINT SP – 0 P/L – 64.50 [55+8.50+1] |  | ACC PENALINT – 0 Dr ACC PENALINT SP – 0 Cr RSP PENALINT – 0 ACR PENALINT – 18 Amortization resumed at 20/10 = 2 per day ACR PENALINT SP – 0 P/L – 12[10+2] |  |
| Day 145 EOD | ACC PRINCIPALINT – 5 Dr ACC PRINCIPALINT SP – 0 RSP PRINCIPALINT – 0 ACR PRINCIPALINT – 32.5 Cr ACR PRINCIPALINT SP – 0 P/L – 102.5 [64.50+(8.50*4)+(1*4)] |  | ACC PENALINT – 0 Dr ACC PENALINT SP – 0 RSP PENALINT – 0 ACR PENALINT – 10 Cr ACR PENALINT SP – 0 P/L – 20 [12+(2*4)] |  |
| Day 150 EOD – Loan Maturity | ACC PRINCIPALINT – 10 Dr ACC PRINCIPALINT SP – 0 RSP PRINCIPALINT – 0 ACR PRINCIPALINT – 0 A CR PRINCIPALINT SP – 0 P/L – 150 [102.50+(8.50*5)+(1*5)] |  | ACC PENALINT – 0 Dr ACC PENALINT SP – 0 RSP PENALINT – 0 ACR PENALINT – 0 ACR PENALINT SP – 0 P/L – 30 [20+(2*5)] |  |
| Day 150 – Payoff |  | After loan is payoff |  |  |
| After payoff |  | ACC PRINCIPALINT – 0 ACC PRINCIPALINT SP – 0 RSP PRINCIPALINT – 0 ACR PRINCIPALINT – 0 ACR PRINCIPALINT SP – 0 P/L – 150 | ACC PENALINT – 0 ACC PENALINT SP – 0 RSP PENALINT – 0 ACR PENALINT – 0 ACR PENALINT SP – 0 P/L – 30 |  |

> **⚠️ Note:** Each time a resume is triggered, based on RSP and ACRSP balance a new amortization record is generated in the EB.ACCRUAL application.


##### Preferential Pricing

The below screenshot displays the New Arrangement Fee waived off because the arrangement has been created as a Valued Customer.


##### Rebate Processing

The below screenshot displays the rebate processing.

For some loan products, the customers protect their loan commitment with the help of insurance covers against risks such as death and disability. The insurance policy can be for the entire loan term or particular period such as yearly and then it is renewed at the end of every period. Rebate processing provides a facility to rebate the outstanding amount of premium for loan insurance on pre-closure or on cancellation at a later stage or cancellation within a certain grace period.

The aim of the rebate processing feature is, to render the ability to use a local routine for certain types of amortisation calculation. However, in AA, the generic accrual processing mechanism allows the user to amortise or accrue fixed amounts supplied by applications through a direct API or accounting entries. The standard method of processing is to straight line the amount on a daily basis.

It is possible to post to an internal account category (instead of PL) in the Accounting version.

The user can define the start date of accrual calculation. From that day, the accrual and account postings begin. On the first day, the calculation is based on the beginning of the accrual period – Start Date in the EB.ACCRUAL record. The changes to the grace period is considered only if the record is reversed, and if the record is reversed, no accounting activity takes place.

This feature provides an option to rebate the outstanding amount of premium for loan insurance on pre-closure or on cancellation at a later stage or cancellation within a certain grace period.

Home loan insurance, or any mortgage redemption insurance plan, is part of a banker's sales pitch when extending sizable long-term credit, such as a home loan. These plans hedge the risk of loss in case the borrower dies or becomes disabled during the loan term, especially an unsecured loan. The banks fund the insurance portion as part of the loan amount, which is repaid by the customers as part of the loan. The insurance policy can be done for the entire loan term or particular period.

The solution deals with the option to define the grace period, rebate on cancellation of an insurance contract and insurance rebate on pre-closure of a loan.


##### Pre-Closure and Dues Settlement

The below arrangement has a start date of 18 Apr with cooling date set as 23 Apr. As the customer opted not to proceed with the loan, the user closes the arrangement before the cooling date and the system displays the error message that the dues are not settled. Unless the dues are either settled or waived, the system does not allow the user to close the arrangement.


##### Tax on Charges

It is possible to levy a tax on charge if necessary. The below screenshot displays the Tax on Charges.


##### Pre-Closure of a Loan and Rebate Processing

An arrangement is created with Insurance Property as shown in the below screenshot.

The charge percentage is negotiable at arrangement level to add or less value based on the customer’s credibility.


> **Related Applications:** `EB.ACCRUAL`

---


### 2.24  LendingRule78


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Rule of 78 is a method used by lenders to calculate interest on a loan. It gives greater weight to months in the earlier part of a borrower’s loan cycle when calculating interest, which increases the profit for the lender.*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

The Rule of 78 is a method used by lenders to calculate interest on a loan. It gives greater weight to months in the earlier part of a borrower’s loan cycle when calculating interest, which increases the profit for the lender.

The Rule of 78 (R78) is a sum-of-the-digits method, summing up of the digits one through 12 - the number of months in a year =78 as a basis for profit accrual distribution . R78 is a method regardless of the finance tenor if it is exactly one year loan with 12 instalments. For applying Rule 78, the total interest collected from the customer is pre-calculated using the Fixed profit rate or fixed interest rate and distributes the interest over the loan life according to the R78 calculation. The interest portion charged for the prior month is much higher than the later one. By using R78, if customer does not terminate the finance before maturity, the interest amount calculated by using flat rate and Rule of 78 finance is equivalent.

Customers can pay the same amount in total. However, if customers pay off the finance early, they end up paying more than the flat rate method.

It is possible to configure and use Rule78 arrangements for both Profit bearing and upfront profit arrangements (Murabaha).

---


### 2.25  Loan Commitment


> **📇 Quick Reference Card**
> 
> **Applications:** `AA.ACCOUNT.DETAILS`, `AA.PERIODIC.ATTRIBUTE`, `AC.ALLOCATION.RULE`, `AC.ALLOCATION.RULES`, `AC.EVENT`
> 
> **Key Fields:** *Amount*, *Change Amount*, *Commitment Drawdown*, *Commitment Reversal*, *Cooling Date Adj*, *Cooling Period*, *Full Commitment Activity*, *Pre Notice Activity* ... +10 more
> 
> **Sections:** ⚙️ Configuration


#### ⚙️ Configuration

The Term Amount Property Class is used to define the commitment given to a contract.

- The Amount attribute in the Term Amount Property Class is used to define the commitment (maximum) amount of the Arrangement.
- The Term attribute in the Term Amount Property Class is used to define the commitment term of the Arrangement. The Amount attribute is currency specific, that is, the user must have one instance of each Product Condition for each currency of the product (or products) that use the Product Condition.
- The Commitment Drawdown attribute in the Term Amount Property class is used to define the disbursement method for the arrangement with options as Manual, Auto or Schedule. While the Schedule option disburses funds based on the schedule definitions in Payment Schedule property conditions, the Auto option disburses the funds through Term Amount property conditions with no dependency on Payment Schedule.

- The Change Amount attribute in the Term Amount Property Class is used to increase or decrease the commitment amount of the arrangement during the life cycle using the INCREASE or DECREASE action.
- The Change Amount attribute represents the amount to be increased or decreased on the original amount.
- To increase, the input in this attribute has to be greater than zero.
- To decrease, the input in this attribute has to be lesser than zero.

- The Change Term Activity allows the user to modify (that is, increase or decrease) the term of an arrangement, subject to the negotiation rules.

The Commitment Reversal attribute in the Term Amount condition enables the user to configure the reversal of the total commitment balance either at maturity or during the pending closure process. This attribute has the following options :

- None or On Maturity - The system reverses the total commitment balance at term maturity.
- On Closure - It reverses the total commitment balance only during pending closure process.

> **⚠️ Note:** Both the commitment amount and the term can be modified during the life cycle of the arrangement, subject to negotiation rules, periodic rules and the current outstanding amount.

When a loan is pre closed (early matured) within the Cooling Period defined for the product, its interest and charges can be waived. This cooling period can be defined as the number of calendar days in the Closure and Term Amount Property Classes. These features are mutually exclusive.

The Cooling Period attribute in the Term Amount Property Class determines the time period during which the amount can be redeemed without making due any accrued interest in the case of pre-closure of an arrangement. In the case of interest already made due, redeem Arrangement Activity during the cooling period only stops paying the accrued interest and due interest paid is not reversed back.

With respect to the pre-closure charges, the charges have to be configured as Rule Break Charges with Rule Start attribute set to Cooling-off.

In AA.PERIODIC.ATTRIBUTE , the value for the Rule Start attribute set as Cooling-off calculates the start date from which restriction has to be applied. If Cooling-off is opted, then the periodic restriction starts from the cooling date as specified in the AA.ACCOUNT.DETAILS .

The below screen shot displays the Periodic Attribute setup for charge trigger after the cooling period.

The following AC.EVENT records are used in AC.ALLOCATION.RULES .

The below screen shot displays INTEREST-ADJUST.REDEEM-PAY.

The below screen shot displays the INTEREST-ADJUST.REDEEM-PAY-CM record.

The below screen shot displays the INTEREST-ADJUST.REDEEM-PAY-PM record.

The below screen shot displays INTEREST-ADJUST.REDEEM-PAY-PY event type in the AC.ALLOCATION.RULE .

The AC.ALLOCATION.RULE set up should be as done as indicated in the above screenshots for the AC.EVENT records.

The Closure Property Class is used to define the cooling period for loan pre-closure without interest and charges. The Cooling Period field of a loan is defined as number of days (calendar) and in case it is a holiday, the Cooling Date Adj field can be used to adjust the cooling period to the next working day.

Property Class wise or Property wise choice is available for waiving or retaining the charge or interest applied during the cooling period using the Waive Class, Waive Prop and Waive Bill Type attributes. The Waive Bill Type attribute can be set to waive accrued amount, billed amount or both.

> **⚠️ Note:** For interest, only the current interest (accrued) can be waived. For charges, the waiver has to be applied on both billed and current (accrued) charges. The Cooling Period attribute in the Term Amount Property Class is mutually exclusive of the Cooling Period attribute in the Closure Property Class. If found in both the places, the system raises an error at the proofing stage.

The Loan Cancellation functionality allows a loan to be automatically cancelled if the commitment amount is not fully availed by the customer in the stipulated time period. The stipulated time is defined as the number of days under Term Amount Property Class.

The system schedules the LENDING-CANCEL-ARRANGEMENT Activity, which triggers the cancellation if the loan is not fully disbursed by that cancel period.

The banks can configure a pre-advice to be sent to the customer to indicate the cancellation that would come up due to the pending disbursement. The pre-advice configuration is achieved through the Activity Messaging Property which has associated multi-value attributes, such as Pre Notice Activity and Pre Notice Days . The Pre Notice Activity attribute has to be LENDING-CANCEL-ARRANGEMENT and Pre Notice Days attribute controls the time in advance when the notification has to be sent.

Certain type of loan products require the loan to be made available in tranches over multiple time frames, this enables the borrowers to withdraw the loan amount in a phased manner to meet the periodic requirement of cash flows.

The Full Commitment Activity attribute in the Term Amount Property Class when set to Yes triggers the LENDING-FULL.DISBURSE-ARRANGEMENT Activity when the loan is fully disbursed.


##### Overdrawn Commitment

The update to commitment balances is controlled by two attributes in the Term Amount Property Class.

- Update Utilised Commitment - indicates whether to raise utilized commitment balance or not.
- Update Commit on Capitalisation - indicates how capitalisation impacts various the commitment balances.

For Retail Loans, the setup of the two attributes below can be configured in two ways

| Scenario | Update Utilised Commitment | Update Commit On Capitalisation | System Behavior |
|---|---|---|---|
| A | No | Current | Follows existing behavior and capitalised charges are maintained in CUR balance of TERM.AMOUNT. |
| B | Yes | Overdraw | Utilisation and Capitalised amounts are maintained in new balances, UTL and OVD respectively.OVD represents the capitalised amounts while UTL represents the utilised commitment amount, excluding the capitalised amount. |


##### Scenario A

Impact of Loan Commitment Balances during Multiple Disbursements and Fee Capitalization

A loan is disbursed in multiple tranches with a linked disbursement fee that is capitalised. The impact on commitment balance is described below.

The configuration in Term Amount product condition for Scenario A is presented below.

- Update Utilised Commitment - No
- Update Commit on Capitalisation - Current

| Step | Nature of Activity (or) Transaction | Transaction Amount (USD) | TOT (Total Commitment) (USD) | CUR (Unutilised Commitment) (USD) | CUR Account (Current Account Principal) (USD) | Due Outstanding (Due Account) (USD) |
|---|---|---|---|---|---|---|
| 1 | New Loan | 1,000,000 | 1,000,000 | 1,000,000 | - | - |
| 2 | Disbursement | 1,000,000 | 1,000,000 | - | 1,000,000 | - |
| 3 | Due | 200,000 | 1,000,000 | - | 800,000 | 200,000 |
| 4 | Repayment | 200,000 | 1,000,000 | 200,000 | 800,000 | - |
| 5 | Disbursement | 100,000 | 1,000,000 | 100,000 | 900,000 | - |
| 6 | Capitalisation | 500,000 | 1,000,000 | - | 1,400,000 | - |
| 7 | Repayment | 300,000 | 1,000,000 | 300,000 | 1,100,000 | - |
| 8 | Repayment | 300,000 | 1,000,000 | 600,000 | 800,000 | - |

| Step | Nature of Activity (or) Transaction | Transaction Amount (USD) | TOT (Total Commitment) (USD) | CUR (Unutilised Commitment) (USD) | CUR Account (Current Account Principal) (USD) |
|---|---|---|---|---|---|
| 1 | New Loan | 100,000 | 100,000 | 100,000 | - |
| 2 | Disbursement | 60,000 | 100,000 | 40,000 | 60,000 |
| 3 | Capitalisation | 2,000 | 100,000 | 38,000 | 62,000 |
| 4 | Disbursement | 38,000 | 100,000 | - | 100,000 |
| 5 | Capitalisation | 2,000 | 100,000 | - | 102,000 |
| 6 | Repayment | 10,000 | 100,000 | - | 92,000 |


##### Scenario B

In certain Lending businesses, especially in Consumer Lending scenarios, when the loan disbursement happens in multiple stages, requirement is that commitment is not to be affected when the fees are capitalised during disbursement and is handled separately without affecting the available commitment for future disbursement . This allows the bank to fully disburse the sanctioned loan amount to the customer.

A loan of USD 100 is sanctioned with two disbursements (USD 70 and USD 30). A disbursement fee of USD 5 is capitalised each time a disbursement happens. Assume there are no other interest, fees or charges.

When 70 USD is disbursed, a fee of USD 5 is capitalised on the loan and the commitment reduces from 100 USD to USD 25 . This means, only 25 USD is available for subsequent disbursement against a required amount of 30 USD.

Similar to the above scenario, when a loan is Revolving, say a loan of 100 USD is fully disbursed and subsequently an activity charge is capitalised for 5 USD. At this point the principal outstanding is 105 USD and when a repayment is triggered for say 5 USD towards the fee portion, the available commitment gets reinstated by 5 USD. This means that against a 100 USD loan, 105 could be drawn since commitment was reinstated for the repaid amount towards the capitalised fees.

For loans in which the bank wants to overcome the above behaviour, the Term Amount product condition is configured with Update Utilised Commitment field set as Yes and Update Commit on Capitalisation set as Overdraw.

> **⚠️ Note:** When the Update Utilised Commitment field is set as Yes, the Update Commit on Capitalisation field must be set to either Overdraw or Current And Overdraw. These are the only combinations allowed at this point of time for the Lending product line when the Update Utilised Commitment field is set as Yes. For other combinations the system raises a validation or proofing error.

The UTL and OVD commitment balance types are used for the above configuration.

Impact of Loan Commitment Balances during Multiple Disbursements and Fee Capitalization

A loan is disbursed in multiple tranches with a linked disbursement fee that is capitalised. Impact on commitment balance is described below.

The configuration in Term Amount product condition for Scenario B is presented below.

- Update Utilised Commitment - Yes
- Update Commit on Capitalisation - Overdraw

|  |  |  | Total Commitment | Unutilised Commitment | Utilised Commitment | Overdraw Commitment | Current Outstanding | Due Outstanding |
|---|---|---|---|---|---|---|---|---|
|  | Activity | Txn Amount (USD) | TOT (USD) | CUR (USD) | UTL (USD) | OVD (USD) | CUR (USD) | DUE (USD) |
| 1 | New Loan | 1,000,000 | 1,000,000 | 1,000,000 | - | - | - | - |
| 2 | Disbursement | 1,000,000 | 1,000,000 | - | 1,000,000 | - | 1,000,000 | - |
| 3 | Due | 200,000 | 1,000,000 | - | 1,000,000 | - | 800,000 | 200,000 |
| 4 | Repayment | 200,000 | 1,000,000 | 200,000 | 800,000 | - | 800,000 | - |
| 5 | Disbursement | 100,000 | 1,000,000 | 100,000 | 900,000 | - | 900,000 | - |
| 6 | Capitalisation | 500,000 | 1,000,000 | 100,000 | 900,000 | 500,000 | 1,400,000 | - |
| 7 | Repayment | 300,000 | 1,000,000 | 100,000 | 900,000 | 200,000 | 1,100,000 | - |
| 8 | Repayment | 300,000 | 1,000,000 | 100,000 | 800,000 | - | 800,000 | - |

|  |  |  | Total Commitment | Unutilised Commitment | Utilised Commitment | Overdraw Commitment | Current Outstanding | Due Outstanding |
|---|---|---|---|---|---|---|---|---|
|  | Activity | Txn Amount (USD) | TOT (USD) | CUR (USD) | UTL (USD) | OVD (USD) | CUR (USD) | DUE |
| 1 | New Loan | 100,000 | 100,000 | 100,000 | - | - | - | - |
| 2 | Disbursement | 60,000 | 100,000 | 40,000 | 60,000 | - | 60,000 | - |
| 3 | Capitalisation | 2,000 | 100,000 | 40,000 | 60,000 | 2,000 | 62,000 | - |
| 4 | Disbursement | 40,000 | 100,000 | - | 100,000 | 2,000 | 102,000 | - |
| 5 | Capitalisation | 2,000 | 100,000 | - | 100,000 | 4,000 | 104,000 | - |
| 6 | Repayment | 10,000 | 100,000 | - | 94,000 | - | 94,000 | - |

> **⚠️ Note:** For Scenario B, the Overdrawn Commitment functionality for a loan which has Revolving field set to 'Prepayment' is currently not available.

A validation is introduced to restrict the below configuration.

- Update Utilised Commitment - Yes
- Update Commit on Capitalisation - Overdraw
- Revolving - Prepayment


> **Related Applications:** `AA.ACCOUNT.DETAILS`, `AA.PERIODIC.ATTRIBUTE`, `AC.ALLOCATION.RULE`, `AC.ALLOCATION.RULES`, `AC.EVENT`

---


### 2.26  Migration of LendingArrangements


> **📇 Quick Reference Card**
> 
> **Applications:** `AA.ACTIVITY.CLASS`, `AA.ARRANGEMENT.ACTIVITY`, `AA.CONTEXT TYPE`, `ACCOUNT`, `CUSTOMER`, `EB.CASHFLOW`, `LIMIT`, `PERIODIC.RATE`
> 
> **Key Fields:** *AMC*, *Activity*, *Arrangement*, *Context Name*, *Context Value*, *Context name*, *Currency*, *Customer* ... +25 more
> 
> **Sections:** 🔧 Working With


#### 🔧 Working With

This section deals with the migration of lending arrangements.


##### General Approach

The following general approach is recommended:

- Analyse existing products and create equivalent products using the AL module.
- Determine requirements for historic data in Temenos' system.
- Prepare extract of legacy loan contract data and balances.
- Create new arrangements from the legacy loan contract data.
- Create the outstanding legacy bills.
- Update the penalty balances.

To takeover legacy loans to AL, the following activities must already have taken place before creating the arrangements:

Each loan arrangement has to be linked to a customer in the CUSTOMER application. Every loan has to be captured in the Temenos' Lending module to ensure that the associated client data is made available in our system and the legacy loan data can be associated with the customer number in the Temenos' system.

For each customer in a loan arrangement, a corresponding LIMIT record is created in our system before creating the arrangement.

A loan can be a long-term contract in the legacy system, which can be ongoing for several years. The usual practice for the takeover of financial contracts is for the contract to be takeover to take place with an effective date that is equal to a scheduled date (for example, interest or principal due date).

The contract is created with principal balance and interest rates at the selected event date as a new contract. Interest rate and principal changes after the event date are loaded into our system as future-dated activities. Details of previous history and balances are not used in the contract processing in our system.

The date chosen can be the last payment date, which can be a past date.

> **⚠️ Note:** It is possible to takeover a contract in the middle of an interest period, but this adds additional complexity to the process. Interest calculations are split in the two systems with associated profit and loss being accrued partly in the legacy system and Temenos' system.

Existing contracts are analysed to identify the earliest date that can be used to create an arrangement.

The existing products in the legacy system has to be analysed and products have to be created for the Lending Product Line that provides the same functionality.

The legacy system is unlikely to provide functionality in exactly the same way as Temenos' system and data may not map directly from the legacy system to our system.

Properties, Product Property Conditions and Products have to be created with an effective date that is on or earlier than the earliest contract date for takeover identified in the legacy data.

Products have to be published, including any known future conditions and made available for sale before arrangements can be created.

It is unlikely that the legacy system has the concepts of product inheritance and negotiable attributes as our system so the legacy products are likely to be supported best by:

- Not using any inheritance in the product structure.
- Making the majority of attributes negotiable for arrangements.

The AA module supports the ability to record arrangement level conditions for information purposes only. Once the arrangement is created, it is possible to load historic conditions if required. Any data loaded prior to the creation date in our system are not used for processing and is not a mandatory requirement.

Temenos' system cannot process the adjustment to loan contracts with an effective date prior to the takeover date. The usual approach is to make the amendment in the legacy system if still available, or manually calculate the adjustment. The adjustment can then be applied to the arrangement in our system effective the takeover date.

The value of outstanding bills have to be taken over into Temenos' system with an effective date equal to the start date of the arrangement in our system or the takeover date. Data has to be made available for overdue bills.

The value of penalty interest and charges calculated (accrued) by the legacy system has to be made available at the takeover date (that is, effective date of arrangement creation in our system). It provides the ability to take these balances over.

The following data should be made available (or be able to be derived) in Temenos' system:

- Customer number.
- Product name.
- Effective Date for the takeover of the contract.
- Currency of Arrangement.
- Outstanding principal balance as at the Effective Date.

> **⚠️ Note:** A possible scenario is that a contract that has passed its maturity date in the legacy system but has outstanding bills and has a current principal of zero at the effective date of takeover.

A separate extract of overdue bills for existing arrangements has to be prepared. It includes,

- The bill due date.
- The breakdown of properties and outstanding amount for the bill.
- A legacy contract identifier that should be possible to link to the created arrangement number after takeover.

Any outstanding penalty interest or charge accrual balances for loans should be prepared and should identify

- The Property name (for example, PENALTYINT)
- The balance amount for the Property.

| Field | Content | Description |
|---|---|---|
| Arrangement | NEW | Requests New ID for the arrangement |
| Activity | LENDING-TAKEOVER-ARRANGEMENT | Create a new arrangement for takeover |
| Effective Date | Period Start Date | The date on which the legacy contract starts in our system, usually the start of an interest period. |
| Customer | Customer | The customer number allocated to the customer of the legacy loan contract. |
| Product | Product | The name of the product created as an equivalent to the legacy product. |
| Currency | Currency | Currency of the legacy loan. |
| Orig Contract Date | Legacy Start Date | The original start date of the legacy contract for information purposes |
| Legacy War Rate | Legacy War Rate | To retrieve the data provided in Context Name and Context Value fields and update the PERIODIC.RATE . |

| Field | Content | Description |
|---|---|---|
| Arrangement | Arrangement No | Indicates the arrangement number allocated by the takeover activity. |
| Activity | LENDING-CAPTURE.BILL-BALANCE.MAINTENANCE | Indicates the activity name which creates the new bill for an existing arrangement. |
| Effective Date | Period Start Date | Indicates the date when the legacy contract starts in our system. This is usually the start of an interest period. |
| Property.1 | Balance Maintenance Property Name | Indicates the name of the Balance Maintenance Property. |
| Field Name.1.1 | Bill Date | Indicates the name of the field to be updated in the balance maintenance property. |
| Field Value.1.1 | Bill Date | Indicates the original date the bill was created in the legacy system |
| Field Name.1.2 | PAYMENT.DATE | Indicates the name of the field to update in the Balance Maintenance Property. |
| Field Value.1.2 | Due Date | Indicates the original due date of the bill in the legacy system. |
| Field Name.1.3 | OR.BILL.AMOUNT | Indicates the name of the field to update in the Balance Maintenance Property. |
| Field Value.1.3 | Original amount | Indicates the original total amount of the bill issued in the legacy system. |
| Field Name.1.4 | PROPERTY-N | Indicates the name of the field to update in the Balance Maintenance Property. |
| Field Value.1.4 | Name of property | Indicates the name of the billed Property. |
| Field Name.1.5 | OR.PROP.AMT-N | Indicates the name of the field to update in the Balance Maintenance Property. |
| Field Value.1.5 | Original property amount | Indicates the original billed amount of the Property billed. |
| Field Name.1.6 | NEW.PROP.AMT-N | Indicates the name of the field to update in the Balance Maintenance Property. |
| Field Value.1.6 | Current outstanding property amount | Indicates the current outstanding billed amount for the associated Property to be taken over. |

| Field | Content | Description |
|---|---|---|
| Arrangement | Arrangement No | Indicates the arrangement number allocated by the takeover activity |
| Activity | LENDING-CAPTURE.BALANCE-BALANCE.MAINTENANCE | Indicates the activity that creates new balance for an existing arrangement |
| Effective Date | Period Start Date | Indicates the date at which the legacy contract starts in Temenos' system, usually the start of an interest period |
| Property 1 | Balance Maintenance Property Name | Indicates the name of the Balance Maintenance Property. |
| Field Name.1.1 | ADJUST.PROP-N | Indicates the name of the field used to update in the Balance Maintenance Property. |
| Field Value.1.1 | Penalty property | Indicates the name of the Penalty Interest or Charge Property to adjust. |
| Field Name.1.2 | ADJ.BAL.TYPE-N.N | Indicates the name of the field to update in the Balance Maintenance Property. |
| Field Value.1.2 | Balance name | Indicates the name of the penalty balance for the Associated Property, for example, CURPENINT. |
| Field Name.1.3 | NEW.BAL.AMT-N.N | Indicates the name of the field used to update in the Balance Maintenance Property. |
| Field Value.1.3 | Original amount | Indicates the balance amount for the associated property to takeover. |

During migration or takeover activity the TAKEOVER.CASHFLOW-REPORTING Cashflow type activity class allows the user to specify the EIR or carry cost which is handed off to the Cashflow engine.

Read Capturing EIR/AMC during Migration in Reporting Property Class for further information.

The following section describes the methods used in triggering TAKEOVER CASH FLOW REPORTING Activity


###### Using AMC Method

1. The following screenshot is Lending Arrangement overview after Takeover is completed
2. The TAKEOVER CASHFLOW REPORTING activity is triggered .The Takeover method is “AMC” and EIR is input as 5.
3. EB.CASHFLOW is updated with the following details Event Type updated as TAKEOVER-PERFORMING for the performing loan


###### Using EIR Method

1. The following screenshot is Lending Arrangement overview after the takeover activity. This loan is in Suspend Status.
2. The TAKEOVER CASHFLOW REPORTING activity is triggered .The Takeover method is “EIR” and AMC is input as 70.
3. EB.CASHFLOW is updated with the following details AMC value is updated in the Takeover Npv field. Event Type is updated as “TAKEOVER-SUSPEND” for the suspended loan


###### Takeover Sequence

The following section describes the takeover sequence in detail.


###### Takeover process – AA Contract with Reporting PC (in IFRS standard)

This process is for existing bank with AA loans & IFRS reporting in their system but switching to FASB standards (from IFRS).

1. Update Reporting condition for the loan product.
2. Proof and Publish the product.
3. Trigger IFRS activity.
4. Update EIR or AMC as required and commit.
5. EB Cashflow gets updated.


###### Takeover process – AA Contract without Reporting PC (without IFRS standard)

This process is for existing bank with AA loans without IFRS module initially but later comply.

1. Add Reporting condition for the loan product.
2. Proof and Publish the product.
3. Trigger IFRS activity.
4. Update EIR or AMC as required and commit.
5. EB Cashflow gets updated.


###### Full Takeover from legacy (Non AA, Non IFRS case)

This process involves migration of loans from legacy system into Temenos' solution with AA & IFRS functionality.

1. Create Loan product with Reporting condition
2. Complete loan Takeover sequence to migrate the outstanding loan bills and balances.
3. Trigger IFRS activity.
4. Update EIR or AMC as required and commit.
5. EB Cashflow gets updated.


> **Related Applications:** `AA.ACTIVITY.CLASS`, `AA.ARRANGEMENT.ACTIVITY`, `AA.CONTEXT TYPE`, `ACCOUNT`, `CUSTOMER`, `EB.CASHFLOW`, `LIMIT`, `PERIODIC.RATE`

---


### 2.27  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Retail Lending (AL) module is part of the Retail Banking suite of products, providing various lending functionalities that a financial institution can offer to its customer.*
> 
> **Applications:** `AA.PAYMENT.TYPE`, `AA.PRODUCT.LINE`, `EB.CONTEXT`, `EB.RULES`, `EB.RULES.VERSION`, `PRODUCT.BUILDER`
> 
> **Key Fields:** *Counter Booking Account*, *Cr Counter Booking Activity*, *Dr Counter Booking Activity*, *Limit Reference*, *Limit Serial*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- APIs
- Temenos Transact Services

The Retail Lending (AL) module is part of the Retail Banking suite of products, providing various lending functionalities that a financial institution can offer to its customer.

It supports an entire range of lending features with configurable conditions. It allows flexibility within which new lending products can be added to it to meet the bank’s ongoing requirements.

It supports the complete lifecycle of loan account from creation of loan, disbursement of loan, maintenance of lending activities - such as amendment of interest rate, capitalise interest to principal amount, change product, repayment of loans and closure of loans at maturity.

Regulatory requirements such as eligibility for opening and operating loan accounts, tax on interest, and restriction of operations are also covered in the module.

The AL module provides a flexible retail lending functionality that allows retail products to be created with the following features:

- Support for commitment processing.
- Unlimited interest types including penalty interest and charge types.
- Fully integrated rules-based overdue and ageing processing.
- Ability to amend, reverse or update arrangements back dated with full automatic recalculation and adjustment of contract.
- Ability to pay in and disburse the arrangement through any application in the system and channel that allows the specification of any customer account. As a result, disbursal and repayment can be from accounts in any currency.
- Flexible repayment schedule and flexible production of bills when repayments are due.
- Ability to overpay, underpay, pay late or early based on issued bills.
- Utilises rules-based accounting, allowing flexible configuration of entry or balance generation in the system.
- Fully supports Risk Free Rates(RFR) processing using the Lookback market convention based on lookback days.

and Product), which is available in the Product Builder application supports product designing and configuration. This application helps the financial institution to deliver the product on time. Temenos’ robust arrangement architecture helps to minimise the time consumed to go to market with the product and modify the characteristics of the product as and when required, with flexible configuration and with minimal customisation approach.

This product equips the banks:

- To define various product conditions for term loans and create different type of loans based on target customer requirements
- To provide a very powerful and user-friendly framework that supports diverse interest, fee and transaction charges setup
- To integrate with Temenos’ pricing and offers a very efficient preferential pricing tool, configurable based on customer segmentation
- With the ability to amend, reverse or update arrangements with effective date as back date with recalculation and adjustment, if required
- With the ability to settle the disbursement of loan amount to multiple accounts (and can be in multi-currency as well)
- With role-based home pages for users - with an option for custom set of screens, enquiries or menus as required by a user to carry on with the day-to-day operations


##### Configuration

The following section describes the AL configuration

| Account | Accounting | Activity Api |
|---|---|---|
| Activity Charges | Activity Mapping | Activity Messaging |
| Activity Presentation | Activity Restriction | Agent Commission |
| Alerts | Balance Maintenance | Change Product |
| Charge | Charge Override | Chargeoff |
| Closure | Constraint | Customer |
| Dormancy | Eligibility | Facility |
| Interest | Limit | Officers |
| Overdue | Payment Rules | Payment Schedule |
| Payout Rules | Periodic Charges | Pricing Rules |
| Reporting | Settlement | Statement |
| Tax | Term Amount |  |

The application provides the ability to allow the user to construct banking products by combining different business components. The Product Lines, which provide functionality for different banking areas are licensed by Temenos; each Product Line utilises a number of Property Classes (business components) that are configurable.

The main features of the product builder are given below:

- Ability to build families of products
- Ability to inherit properties from the product family structure
- Ability to determine the properties that a product is comprised of
- Control of default values to be applied for product arrangements
- Dated conditions for products
- Full control of scope of negotiation between product and arrangement conditions
- Control of negotiation of attributes over time
- Design, proof and publish lifecycle for product management
- The product builder can be used to create and maintain existing application (Mortgage, Account, Loans and Deposits and AZ) product parameters

Read AA Product Builder user guide for details on Product Construction and Configuration process.

Read AA Property Classes user guide for detailed information on Property Classes.


##### Illustrating Model Parameters

Product Conditions of a Property Class are evaluated to bring out the features of the Property Class. The values in the Product Condition are made default in an arrangement during its creation. The negotiability or default values and other restrictions are also defined in the Product Condition. These Product Conditions with the Properties derived from the Property Classes are grouped together to build products.

Product Conditions are dated and some of them have currency as part of their ID. When currency forms part of the Product Condition ID, then the user has to create different conditions for each currency in which the product is available. When a new condition is created or an existing condition is amended, the user has to proof and publish the product to which the condition is linked.

Model parameters consists of:

The Accounting Property Class is used by all products. Arrangement Architecture (AA) uses activity-based accounting. Each Property has different actions, which require accounting. For each action, a corresponding allocation rule definition is required. Allocation rules can be defined either at Property or Property Class level. The categories to which the interest or charges have to be posted are also defined in this Product Condition. In Model Bank, the charges are amortised.

The Activity Charge Property Class defines the charges that has to be applied when a particular activity is triggered on the arrangement. The charges so applied can be made due, capitalised or deferred. In the model bank, for a Mortgage loan product a principal decrease fee is applied for a principal decrease activity and a new arrangement fee is applied when a new arrangement is created.

The Activity Mapping Property Class provides the link between external applications and arrangement activities when a transaction is performed on an arrangement account. A debit or credit to an arrangement account triggers the applications such as Funds Transfer, Teller, Clearing, etc., which are linked by relevant transaction codes using this Product Condition.

The Agent Commission property class is possible to record the agent and the agent arrangement for a given financial arrangement and monitor what are the default events that trigger commissions and ability to provide a spread over the default commission rates and give the ability to provide an overriding amount, as against the predefined commission calculation.

The Alerts Property Class is used by all products. It enables alerts to be sent to the customer for various activities in an arrangement. Alerts can be subscribed at the arrangement level by using EB.ALERT.REQUEST . Multiple owners of the arrangement are allowed to subscribe different alerts on that arrangement. The subscription of alerts can be restricted based on the role of the customer in that arrangement.

The Activity Presentation is an optional Property Class that allows to define versions used for various Properties during arrangement activities. The versions can be defined at Property Class, Property and Activity levels.

The Activity Restriction Property Class is used to specify the restriction on a particular transaction. The restriction rules including the relevant periodic attributes and activities are defined in the product condition. These rules are then used to define activity based or property based restrictions. A rule if broken can be set to result in an override or error. A charge can be attached for this and can be set to be made due , capitalised or deferred.

The Activity Messaging Property Class links the Soft Delivery module to Arrangement Architecture module. Messages are sent based on the role and activity performed on an arrangement. This record allows either specific Activities or Activity Classes to be defined and linked to the records of EB.ADVICES .

The Balance Maintenance Property Class allows the user to capture bills and balances, and adjust the balances of the bill for the contracts, which have been taken over from existing legacy system or Temenos' Lending module into the AA module.

The actions such as CAPTURE.BILL, ADJUST.BILL and so on., help in capturing the bill and its balances into the new system.

The Charge Property Class is used for all charge calculations in AA. The charge can be a scheduled , periodic or an activity based charge. It can be fixed or calculated based on band or level. The currency in which the charge has to be applied can also be defined. It is possible to define a minimum charge and also to waive the charge.

The Charge Off property class enables the customer to charge off various properties financial balances in arrangements. This can be a partial charge-off, a series of partial charge-off transactions, or a total charge-off. Feature Dual Accounting – i.e. having two sets of books; the Customer Record vs. the Bank Record and applying payments “independently” to the two records is enabled.

The Charge Override Property Class enables the customer to modify the ad-hoc charges triggered by an Activity. The user can either waive or modify the activity charge or rule break charge.

The Change Product property class defines the rules and behaviour for allowing arrangements of one product to be changed to another product. The CHANGE.PRODUCT property can be included in a product if arrangements are allowed to be changed to another product during its lifetime. The Property Class allows the definition of restrictions on products that change can be made to and when a scheduled change should be applied. It can also be used to define the roll over conditions for an arrangement.

The Closure Property Class is used to close an arrangement account. An arrangement account can be closed automatically or manually. This is defined in the product condition. On reversal of a new arrangement, closure is triggered automatically.

Cooling period functionality is available in the Closure Property Class (PC), for Accounts, Deposits, Lending, Rewards and Safe Deposit Box. If the customer chooses to cancel (that is, payoff) the loan within the cooling period, any charges and interest are waived off based on the product condition setup.

The Constraint Property Class is used to define constraints on the arrangement. The constraint indicates the maximum period an arrangement that can be backdated with an error or override.

The Customer Property Class is used by all products. This property class is used to define all the parties involved in an arrangement. The customer is always defined at the arrangement level. Each arrangement can have one or more legal owners defined in OWNER

The Eligibility Property Class is used to evaluate eligibility of a customer for a specific product based on a set of rules. Here, first the EB.CONTEXT has to be created. Based on this, rules are defined using Rules Engine. Once these rules are validated, the EB.RULES.VERSION and EB.RULES are created in the system.

This Facility Property Class controls the list of available services for an arrangement account. When an external activity (financial/non-financial) is triggered and the corresponding service group is identified as blocked for this account, then an error message appears to stop the activity.

The Interest Property Class is used for all interest definition and processing in AA. A product defined and processed in AA can have multiple interest properties defined (for example, principal interest, penalty interest, commission, etc.) Interest rates can be define as Fixed , Floating, Periodic or Linked Rate (referring an interest property from other arrangement). Tiered interest can also be defined. Further it is possible to define a Negative Rate, Minimum interest amount and waive the interest.

The Limit Property Class primarily controls the use of Limit module by the product. The user can set up single or shared limit and can define Limit Reference applicable for a specific product such that the same is set as default in an arrangement. For a new limit, at the arrangement level, the user should provide New in the Limit Serial field. Further limits can be set to use the Limit module or it can be managed only within the arrangement architecture framework.

The Officers Property Class enables the user to define:

- Product
- Arrangement specific officers
- Officer’s roles
- Primary officer
- Additional officer

The Overdue Property Class controls the ageing process of the bills raised in arrangement. The ageing period, statuses and accounting treatment of the outstanding balance can be defined. It is possible to define penalty interest to be applied on the overdue amounts and/or current balances. Bills can be aged based on the number of outstanding bills or days. It is also possible to define that all bills of an arrangement have to be aged to the present status. Accounting entries can be made to raise for every status movement and chaser advices can be scheduled.

The Payoff Property Class is used to produce a payoff statement, which is given to a customer when a loan payoff is considered. It shows the current status of the account, including the updated accrued interest and penalty applicable, if any. An expiry date can be defined for the payoff statement and the loan statement shows the additional daily interest to be charged till the expiry date.

The payoff amount is calculated by using the simulation framework.

The Payment Rules Property Class controls the sequence and order in which the bills or outstanding balances that required to be settled. An arrangement can contain several outstanding bills and each bill can be comprised of multiple amounts (for example, principal, principal interest, penalty, tax, charges, etc.). When a customer makes a payment, the entire due amount cannot be satisfied. This Property Class is used to define the method by which a single payment is applied to multiple bills and multiple amount types.

The Payment Schedule Property Class is used by all products which have amounts billed (that is, made due or capitalized or pay). A Payment Schedule can be comprised of one or more payment definitions with conditions such as payment type and method, arrangement properties, dates and amounts. The AA.PAYMENT.TYPE file is used to define the standard payment types such as Constant, Linear, Actual and Fixed Equal, etc., that can be used by a product. This payment type is then attached to each payment schedule definition. The start and end date can be specified. The user can specify the repayment of arrangement to commence after ‘n’ months from the arrangement date or ‘n’ months before the maturity or ‘n’ months after the change product or reset and rollover has happened.

The Payout Rules Property Class is used by various Product Lines, which have amounts billed and made due for payment to the customer. It is used to define the method by which a single payment is applied to multiple bills and multiple amount types.

The Periodic Charges Property Class is used to define a charge to be applied in relation to a period of time. The charge currency can be specified and the charge can be set to be deferred. A minimum and maximum charge amount can be defined.

The Reporting Property Class defines parameter for IFRS compliance of AA. It is also used to configure position management reporting.

The Statement Property class is used to define the legacy ACCT.STATEMENT feature at Arrangement Architecture level. Statements may be produced daily (every working day), every 1-9 weeks, twice a month (on the 15th and the last day of the month) or every 1-12 months on any day of the month. Up to nine statement cycles may be specified for each Account, and each statement cycle is independent. In addition to this, special interim statements can be enabled. This property class also controls if advices are to be produced or not, when interest and charges are applied, and whether detailed interest statements (interest scale) should be produced.

The Settlement Property Class is used for various Product Lines to control the settlement related functions of all the Product Lines. Settlement can be handled by linking any customer account within the system, the account and bank details of another bank by using Direct Debit and beneficiary of the customer.

The Settlement Property Class specifies the counter booking details with the Counter Booking Account , Dr Counter Booking Activity and Cr Counter Booking Activity fields. The Default Settlement Account is considered as the default account for both Pay-in and Pay-out Activities, if the Pay in or Pay out account is not specified. But, if the accounts are specified for the Pay in or Pay out, then those accounts precedes over the specified default settlement account.

The Dormancy Property Class allows the user to control the parameterisation of inactive or dormant accounts and movement of these accounts into various buckets at arrangement or product level. It can control based on period, and some exceptions or rules also can be added for evaluation and movement. The user can include or exclude certain activity or activity class for the evaluation.

The Tax Property Class allows the user to control and define tax that has to be calculated for various financial property. Tax definition can be done at both Property Class and Property Tax level. The tax can be attached both at TAX and TAX.GEN.CONDITION level.

The Term Amount Property Class is used by financial products which involve an amount of money that is lent or deposited for a specified period of time. This property class controls the commitment made by the bank and the customer.


##### Illustrating Model Products

Lending Product Line provides Home Equity, Line of Credit, Mortgages, Personal Loans and Small Business Loans functionality. This module allows the user to create Home Equity, Line of Credit, Mortgages, Personal Loans and Small Business Loans by using the AA framework under the Lending Product Line.

| Product Name | Product Attributes |
|---|---|
| Home Equity | CEL Loan Home Equity Line of Credit Home Equity with LOC with Floating interest initially for 9 years and then periodic interest with annuity type of repayments. Home Equity Loan Home Equity without LOC for 25 Years term. Interest only payments for the first 9 years and with annuity type of repayments. |
| Line of Credit (LOC) | LOC with 3% Principal Repayment LOC with 3% Principal Repayment with revolving credit facility. LOC with Interest Only Payments LOC with interest only payments and revolving limit that reinstates on repayments. LOC with credit line product with default term as 10 years and Revolving as Payment. LOC with interest only payments and revolving limit that reinstates on repayments. |
| Mortgages | Bridge Mortgage A bridge loan to connect two mortgages with a term of around 1 year (the maximum term is 5 years). Repayment of Interest amount is scheduled on monthly basis and principal amount is scheduled on the maturity date. Mortgage Mortgage loan with automatic disbursement configured and annuity type of repayments with periodic interest. Any advance payments get a benefit from both principal and interest components. Mortgage (Adjustable Rate) Mortgage loan with periodic rate resets for every year. Escrow charges are included in the monthly constant payment schedule. Mortgage (Fixed Equal Repayment) The schedule has a Fixed Equal Repayment . On events like advance repayment, change in components like interest, schedule, and so on, the Term is recalculated till the maximum possible (based on the term) and capped with the maximum term. Thereafter, the payment amount is calculated. Mortgage (Seasonal Repayments) Seasonal constant repayments configured in schedule. For example, 1, 3, 7, 10, month. Mortgage (Special Offer) Interest offset advantage for the initial period. Mortgage (Cash Back) Mortgage loan Bonus for prompt repayment Advance repayment with principal benefit only Mortgage (Linked Rate) A Mortgage loan any advance repayment does not have any benefits. Penalty interest is adopted from a linked principal interest rate. Mortgage (Fixed 2 year Product) Fixed two-year mortgage that allows loan with overpayment on adhoc or regular basis based on a fixed amount. Mortgage (Fixed 5 year Product) Loan with overpayment on Adhoc or Regular basis based on a current balance percentage. |
| Personal Loans | Personal Loan Personal Loan (Biweekly Repayment) Personal Loan (Linked Rate) Student Loan (Loans to student aged between 15 to 25 years) Vehicle Loan Forward dated personal loan is specifically created for the repayment calculator Payroll Loan Loan for people under payrolls FASB Loan Financial Accounting Standards Based Loan |
| Small Business Loans | Small Business Loan Small Business loan with loan revolving as prepayment and a preferential pricing Commercial Loan (Interest Upfront) Small Business loan with interest upfront with loan revolving as prepayment Fully Negotiable Loan Default (For Failed Eligibility) War Loan The calculation of a weighted average interest rate for the loans, which have multiple legs (tranches). |
| Consumer Loan | Single or Multiple Disbursement loan with the cancel period of 7 Days. No Interest Definition. Instead a DISBURSEMENTFEE is added based on the current disbursement amount. DISBURSEMENTFEE is a Tiered charge with a Cap of 250. REFUNDFEE is given as Credit Type to the customer on doing a repayment. |
| Technical Loan | Term amount with a Minimum value as 1000 and Maximum value as 25000 with multiples of 100. Category is set as 3112 in the ACCOUNT property class. Repay current balance is set for ACCPRINCIPALINTINF and CURACCOUNTINF in Payment. Rule property class. |
| Instalment Loan | Instalment loan for 12 month Instalment loan for 6 month Instalment loan for 3 month |
| War Loan | It is created to enable the calculation of a weighted average interest rate for the loans, which have multiple legs (tranches). |
| Digi Mortgages | Digi Mortgage 2Y Fixed+Constant Pay Constant Repayment Type, Fixed Interest Rate is applicable for first 2 years and Periodic Interest Rate thereafter. On a principal decrease, either the loan term or the loan repayment amount can be recalcuated based on the user choice. Digi Mortgage 2Y Tracker+Int Only Interest only Repayment Type, Floating Interest Rate is applicable for first 2 years and Periodic Interest Rate thereafter. On a principal decrease, either the loan term or the loan repayment amount can be recalculated based on the user choice. Digi Mortgage 5Y Fixed+Constant Pay Constant Repayment type, Fixed Interest Rate is applicable for first 5 years and Periodic Interest Rate thereafter. On a principal decrease, either the loan term or the loan repayment amount can be recalculated based on the user choice. Digi Mortgage 5Y Track+Constant Pay Constant Repayment type, Floating Interest Rate is applicable for first 5 years and Periodic Interest Rate thereafter. On a principal decrease, either the loan term or the loan repayment amount can be recalculated based on the user choice. |


> **Related Applications:** `AA.PAYMENT.TYPE`, `AA.PRODUCT.LINE`, `EB.CONTEXT`, `EB.RULES`, `EB.RULES.VERSION`, `PRODUCT.BUILDER`

---


### 2.28  Payment Holiday


> **📇 Quick Reference Card**
> 
> **Purpose:** *Banks offer convenient repayment options for lending products in order to please the customers. To facilitate such flexibility, the system should allow banks to skip or modify (increase or decrease) some of their scheduled repayments based on certain rules defined at multiple levels (such as Product...*
> 
> **Applications:** `AA.ACCOUNT.DETAILS`, `AA.PERIODIC.ATTRIBUTE`
> 
> **Key Fields:** *Bill Type*, *Calc Type*, *Combine Bill At Parent*, *Comparison Type*, *Hol Restrict Item*, *Hol Restrict Type*, *Modify/Cancel Payment Holidays*, *New Payment Amount* ... +20 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With


#### 📖 Introduction

Banks offer convenient repayment options for lending products in order to please the customers. To facilitate such flexibility, the system should allow banks to skip or modify (increase or decrease) some of their scheduled repayments based on certain rules defined at multiple levels (such as Product or Arrangement). Payment Holiday is one of the features offered by banks that allow customers to skip payments based on some rules of the bank and within a prescribed limit, which is also controlled.


#### ⚙️ Configuration

The system can be configured to allow modifications to the scheduled payments by either skipping or modifying the payment amount. This type of flexible repayment is achieved by using the Payment Holiday Transaction Class. There are no product conditions required and each time the conditions have to be captured afresh by the user.

Flexible repayment instructions are captured using the LENDING-UPDATE-PAYMENT.HOLIDAY activity and any subsequent changes to the flexible repayment are made through the LENDING-CHANGE-PAYMENT.HOLIDAY activity.


##### Defining Payment Holiday

Using the LENDING-UPDATE-PAYMENT.HOLIDAY activity, the user can define a payment holiday based on the Payment Type or Bill Type . The user, further has to define the Number of Instalments and the New Payment Amount (if the New Payment Amount is a Reduced Payment Amount than the Original Payment Amount).

- New Payment Amount - Determines the reduced repayment amount (the field is optional, if left blank the entire payment is considered)
- Number of Instalments - Determines the installments that need to be skipped or should have a reduced repayment amount.
- Recalculation – Allows the user to define the type of recalculations on the schedule, due to the payment holiday definition. The Recalculation options are Payment, Residual, Term, Progressive Payment and Maturity Then Payment (Read Recalculation Based on Activities in Payment Schedule)

In the screenshot below, the options to recalculate during the payment holiday and defer holiday interest period are illustrated.


##### Defining Multiple Payment Holiday

When the user defines multiple holiday payments with multiple start dates, then the payment schedule projection honours all the payment holidays.

> **⚠️ Note:** There may be few payments between holiday start dates.


##### Amending Payment Holiday

Amendments to the existing holiday payments definition can be made using the LENDING-CHANGE-PAYMENT.HOLIDAY Activity.


##### Restricting Items from Payment Holiday

If some payment type or bills types have to be restricted, it can be defined in the Payment Schedule conditions using the Hol Restrict Type and Hol Restrict Item set of fields. The user has to choose the restriction on holiday processing based on either the property class, property, bill type or payment type.

Consider a scenario, if the Charge property class is selected for restriction, then flexible repayment is not allowed for any of the scheduled charges. This can be achieved by setting Hol Restrict Type as Property Class and Hol Restrict Item as CHARGE.

Read Restriction in Flexible Repayment in Payment Holiday for more information.


##### Repayment of Holiday Interest

During a payment holiday, the system continues to accrue interest as per the original configuration. The holiday interest accrued during the payment holiday period is collected in the first upcoming schedule post holiday. When the accrued interest breaches the permissible amount of the first upcoming schedule post holiday, the accrued interest is moved to the subsequent bills.

When the payment holiday is declared, the system can be configured to collect the accrued interest during the holiday period as a separate schedule by setting Repay Type as Deferred.

- When Repay Type is left blank, the accrued interest is collected in upcoming schedules as a priority but when it is set as Deferred, the holiday period’s accrued interest is billed as a separate item in the payment schedule. The system automatically moves the holiday interest accrued to a separate balance type and starts billing it in a separate payment type after the payment holiday.
- Repay Period - Specifies the number of billing cycles required to collect the accrued holiday interest. When left blank, the holiday interest is collected as schedules till maturity.
- Refer Settlement Type - Reuses the settlement instructions of another existing payment type.

Read Repayment of the Accrued Holiday Interest for more information.


###### Balance Type for Holiday Interest

It is possible to collect the interest accrued during the payment holiday as a separate schedule. Read Flexible Repayment Definition in Payment Holiday Property Class for more information.

When the system is configured to collect the payment holiday interest in a specific schedule, the system should bill the holiday interest separately. It automatically moves the interest accrued during the payment holiday to a separate balance type to achieve this separate billing. The unbilled accrual during the payment holiday is moved from ACC to HOL (that is, from Accrued Interest Balance Type to Holiday Interest Balance Type).

The holiday interest accrued during the holiday is moved to the HOL balance type using the LENDING-DEFER-PAYMENT.HOLIDAY activity.


###### Payment Type for Holiday Interest

The HOL holiday interest is billed as a separate component in the payment schedule automatically under the Payment Type that has the Calc Type as Holiday.

> **⚠️ Note:** Ensure that the Combine Bill At Parent field is set to Yes for HOLIDAY.INTEREST Payment type for combining the holiday interest and other payment types.

When a holiday is declared for more than one interest property, separate payment types are scheduled for each of the interest property. The holiday interest is scheduled in the same frequency in which the original interest is collected and the number of schedules are based on the Repay Period specified. When left blank the schedules continue till maturity. This interest can be collected from the same settlement instruction as that of Payment Type given in Refer Settlement Type .

The system schedules the Forward Recalculate Activity at the end of the holiday period to update the Payment Schedule for the holiday interest component.

The repayment of the interest accrued during the payment holiday starts immediately after payment holiday or grace period ends. The system schedules an activity for changing the payment schedule to accommodate the HOLIDAY.INTEREST payment type on the last day of the defined payment holiday. The HOLIDAY.INTEREST Payment Type is set up in such a way that the Start Date of the HOLIDAY.INTEREST Payment Type is the immediate next due date (as that of the Payment Type or Bill Type defined in the Payment Holiday) after the payment holiday.

The user can amend the details of the holiday interest payment that is automatically scheduled after the holiday interest schedule is updated in the arrangement (after the holiday period).


##### Defining Payment Holiday Limit

When the customer opts for a flexible payment, the bank may choose to place a control on the amount of flexibility used by the customer. The bank can control the repayment amount that is being skipped or reduced during a payment holiday. This control can be configured in the Payment Schedule condition at the product or arrangement levels.


###### Periodic Attribute Class

The HOLIDAY.LIMIT and the HOLIDAY.LIMIT.REVOLVING periodic attribute classes are used to define the flexible payment limit.

- HOLIDAY LIMIT - Calculates the maximum amount or maximum percentage of amount taken as payment holiday when utilising a flexible payment.
- HOLIDAY LIMIT REVOLVING - Calculates the maximum amount or percentage that can be taken as a payment holiday where the holiday limit available is reinstated during further ad hoc payments.


###### Periodic Attribute

The banks or FIIs can define periodic attributes from the Periodic Attribute Classes. The periodic attribute controls the rule and its impact on the product through fields like:

- Periodic Type - Determines the period for which the Rule should be active on the Product. The options are Life, Initial, Repeating, Rolling, Current and Assessment Period.
- Comparison Type – Evaluates rules by comparing the values captured by the user against the arrangement values with the comparison type defined here. This should be a valid record in EB.COMPARISON.TYPE .
- Rule Start Date - Determines the date from which the Rule should be made effective. The options are Arrangement, Agreement, Start, Anniversary and Cooling Off.

Other attributes are not mandatory. Read Periodic Rules for more information.

The PAYMENT.LIMIT.REVOLVING periodic attribute is configured in the Payment Schedule condition to restrict the Payment Holiday Limit to a maximum amount or maximum percentage defined by the banks or FIIs. This rule is configured to be effective on an arrangement from the Arrangement Effective date throughout the life of the arrangement.

This rule allows to reinstate the Payment Holiday Limit during any adhoc or excess payment over and above the due amount.

The FLEXIBLE.PAYMENT.LIMIT periodic attribute is configured in the Payment Schedule condition to restrict the Payment Holiday Limit to a maximum amount or maximum percentage defined by the banks or FIIs. This rule is configured to be effective on an arrangement from the Arrangement Effective date throughout the life of the arrangement.

The periodic attribute defined in the Payment Schedule condition is evaluated every time a new payment holiday is declared. These periodic attributes can also allow banks to create period-based rules (for example USD 1000 Flexible Payment Amount Limit per year) by configuring the Periodic Type (in the Periodic Attribute) and the available flexible payment limit gets checked every time a payment holiday or flexible payment is requested for the given period (the Period can be Life, Initial, Repeating, Rolling, Current and Assessment Period). For a revolving Holiday Limit, any excess repayment over and above the due amount replenishes the flexible payment limit (to the extent of the initial limit value defined).

The utilisation of the Payment Holiday Limit, is based on scheduled bill and how much the customer has paid for the Scheduled Bill. Read Payment Holiday Limit for more information. The Payment Holiday limit is evaluated whenever there is a change in Payment Schedule like a change in the repayment amount due to the change in the interest rate.

> **⚠️ Note:** As it is possible to break the limit during standard system processing and not only during a user activity (like change in payment amount due to change in interest change in term or cancelling the declared holiday and so on), it is recommended to configure the Periodic Rule to generate an override rather an error so that during system processing any changes are automatically approved. However, during a user-initiated activity an approval is required to exceed the limit.


##### Configuring Payment Holiday Limit

The Payment Holiday Limit can be any of the following:

- Fixed amount - When the Payment Holiday limit is configured as a fixed amount, the system allows the banks or FIIs to provide payment holiday to the customer upto the defined Fixed Payment Holiday Limit.
- Percentage based on a balance type

For configuring a Fixed Payment Holiday Limit, the FLEXIBLE.PAYMENT.LIMIT/PAYMENT.LIMIT.REVOLVING periodic attribute is set up as follows, in the Periodic Rule Tab of Payment Schedule Product Condition of the product.

As per the above setup, the system is configured to raise an override for Payment Holiday Limit above USD 50,000.

For configuring a Payment Holiday Limit based of a Balance Type (that is, a percentage of the Balance Type), the FLEXIBLE.PAYMENT.LIMIT/PAYMENT.LIMIT.REVOLVING periodic attribute is set up as follows in the Periodic Rule tab of Payment Schedule Product Condition of the product.

Then in the Negotiation Rule tab, the following configuration is followed to set up a Payment Holiday Limit, which is 10% of the Total Commitment (TOTCOMMITMENT) Limit.

Any Payment Holiday limit above the defined value raises an override.

It has to be noted that, the Payment Limit Revolving periodic attribute is used to reinstate the payment holiday limit balance, during the adhoc or excess payment over and above the due amount. The banks or the FIIs can configure:

- Different percentage in the Nr Value
- Different evaluation source balance in the Nr Value Source (for example, CURACCOUNT)

That is, in the Negotiable Rules tab the Value Source , Options , Type , Value , and Message controls the Payment Holiday Limit and the related message to be displayed if the limit is breached.

> **⚠️ Note:** ’Balance Name’.


##### Controlling Payment Holidays Count

Banks/FIIs can implement a control on the number of payment holidays, for a given Bill type or Payment type defined in an arrangement for a period by configuring the periodic attribute of the HOLIDAY.COUNT periodic attribute class in the Payment Schedule condition at the product or arrangement levels.


###### Defining Periodic Attribute Class

The HOLIDAY.COUNT periodic attribute class is used to define the number of payment holidays within a period.

It evaluates the number of holidays defined in an arrangement from AA.ACCOUNT.DETAILS and there by implements the restriction on the definition of payment holidays. During a rule evaluation, the system excludes any cancelled payment holiday, while ascertaining the overall payment holiday count for the period.


###### Defining Periodic Attribute

Banks/FIIs can define periodic attribute from the periodic attribute classes and these periodic attributes control the rule and its impact on the products. Read Periodic Rules for more information.

The user configures the HOLIDAY.COUNT.YEARLY periodic attribute in the Payment Schedule condition to restrict the number of payment holidays defined in a year, as required by the banks or FIIs. This rule is configured to be effective on an arrangement from the Arrangement Effective date and the rule repeats every year.


###### Configuring Holiday Count

For restricting the number of payment holidays for a particular year, HOLIDAY.COUNT.YEARLY is set up as follows in the Periodic Rule tab of Payment Schedule product condition.


##### Defining Restriction on Consecutive Payment Holidays

Parallel payment holiday (that is, if an arrangement is within a payment holiday period and the user tries to further define a payment holiday, before the current payment holiday period is completed) is restricted when the Repay Type field is set as Deferred in the Payment Holiday Transaction Class. When Repay Type is set blank, the user can define a parallel payment holiday.

However, the banks/FIIs can implement restrictions on the definition of parallel payment holiday when Repay Type is blank, through the periodic attribute of the HOLIDAY.RESTRICT periodic attribute class.


###### Defining Periodic Attribute Class

The HOLIDAY.RESTRICT periodic attribute class is used to restrict payment holidays defined in parallel to an existing payment holiday.

The HOLIDAY.RESTRICT periodic attribute class evaluates the existing defined payment holiday dates from AA.ACCOUNT.DETAILS with that of the current activity date of payment holiday definition and there by implements the restriction, if required.


###### Defining Periodic Attribute

The user configures the HOLIDAY.RESTRICT.LIFE periodic attribute in the Payment Schedule condition to restrict any parallel payment holiday, that is, if an arrangement is within a payment holiday period the system restricts defining further payment holiday, unless the existing payment holiday period is completed. This rule is configured to be effective on an arrangement from the arrangement effective date, throughout the life of the arrangement.

The periodic attribute defined in the Payment Schedule condition evaluates the current system date and existing holiday dates in AA.ACCOUNT.DETAILS when a new payment holiday is declared. These restrictions on applying the payment holiday can be configured for different periods (for example, the life of arrangement, a period from renewal of the arrangement, repeating for period and so on) by configuring the Periodic Type and Rule Start Date in the AA.PERIODIC.ATTRIBUTE .

However, configuring the Periodic Type as Initial, doesn’t impose any restriction of definition of consecutive payment holiday as defined above.


###### Configuring Holiday Restriction

For restricting the parallel payment holidays throughout the life of the arrangement, HOLIDAY.RESTRICT.LIFE is set up as follows in the Periodic Rule tab of Payment Schedule product condition.

> **⚠️ Note:** The Pr Value for the Periodic Attribute should be Null. The system restricts definition of parallel payment for payment holidays having Repay Type as Deferred, without the configuration of the Periodic Attribute in the Payment Schedule product condition.


##### Cancelling Skipped Schedules

It allows the user to cancel the skipped schedules, through the LENDING-CHANGE-PAYMENT.HOLIDAY activity. However, cancellation is only allowed, when the upcoming holidays post cancellation is consecutive and it cannot be on an ad-hoc basis.

Read Cancellation of Holidays Declared for more information.


##### Paying-off during Payment Holiday

It is possible to payoff a loan in a holiday or grace period and/or a loan carrying the unbilled holiday interest. The payoff statement is generated for the entire loan outstanding including the accrued holiday interest and due holiday amount.

The Payment Rules used for payoff should include the holiday interest component. This enables the system to include the pending HOL . Read Payment Rules for more information.


#### 🔧 Working With

This section explains about the payment holiday definitions and processing of the same under various circumstances.

Payment Holiday for scheduled payments can be declared by triggering the UPDATE-PAYMENT.HOLIDAY activity (the same can be achieved from the Arrangement Overview page through Request Payment Holidays) and by setting the relevant holiday related attributes as explained in Configuring Payment Holiday . The above said UPDATE-PAYMENT- HOLIDAY activity can be simulated and also be converted to live.

The flexible repayment achieved using a payment holiday is explained in the below workflow:

A loan is created on 1st Jan, 2020 for one year having payments due every month. Assume the customer decides to skip the schedules for the month of April, May and June. The system achieves this flexible repayment through the below flow of activities.


##### Defining Holiday

Banks or FIIs can define the payment holiday on an arrangement for Instalment Deferral or Decrease, by using the LENDING-UPDATE-PAYMENT.HOLIDAY activity or accessing the Request Payment Holiday field in the Arrangement Overview page and there by providing the Payment Type or Bill Type , Number of Installments and the New Payment Amount fields as required.

The payment holiday is defined based on the Payment Type or Bill Type , so that, all the components of the specified Bill Type or Payment Type are subjected to the Payment Holiday, unless a restriction is defined though the Payment Schedule product condition. Read Restriction in Flexible Repayment in Payment Holiday for more information.

Banks or FIIS can reduce the repayment amount for a particular period by capturing the New Payment Amount and Number of Installments .

The below screenshot displays the payment holiday that can be declared by enabling the Request Payment Holidays field in the Arrangement Overview page. Here, the user has selected to apply Payment Holiday for three installments from the schedule due on Jul 15, 2021.

The payment holiday details are captured in AA.ACCOUNT.DETAILS , whenever a payment holiday is defined as shown below for the specified example.

The details of the holiday is evident in the Payment Holiday drill down in the Arrangement Overview page.


##### Simulating Payment Holiday

The system allows simulation of a payment holiday, to understand the impact of the payment holiday on the arrangement and then execute the same (instead of directly executing the same). In the below screenshot the user selects the Request Payment Holiday option in the Arrangement Overview page, from where Apply Payment Holiday simulation for the installment of the month Aug 2021 was selected.

The payment holiday simulation results are available under the Simulation tab in the Arrangement Overview page. The details of the simulation are stored in the $SIM files that can be used for further actions. The simulation results are printable and helps the banks to take the holiday execution forward.


##### Repayment of Holiday Interest

The system continues to accrue interest even during a payment holiday. This accrued interest is automatically collected in the upcoming installment/s immediately after the regular payment resumes.

The user has an option to repay the holiday interest as an additional schedule over a specific period or until maturity. This is achieved by using the Payment Holiday attributes, Repay Type , Repay Period and Refer Settlement (Read Payment Holiday Attributes for more information)

This section describes the Payment Holiday to reduce the repayment amount and defer the interest over a period.

- Consider a payment in which the monthly instalment is 120 (70 principal and 50 interest) and the payment rule is set to service the interest first. If the payment is decreased from 120 to 70, the interest is billed fully and remaining towards the principal or any other component as defined. Thus, there is no accrued holiday interest for processing and trying to defer the holiday interest raises an error. If the instalment is decreased from 120 to 40, the interest is partially billed for 40 against accrual of 50. The system tracks the unbilled interest portion for the entire holiday period and considers the same for processing holiday interest after the payment holiday period, based on the Repay Type , Repay Period and Refer Settlement fields in Payment Holiday Transaction Class.

- Consider a payment in which the monthly instalment is 120 (70 principal and 50 interest) and the payment rule is set to service the principal first. If the instalment is decreased from 120 to 60, the interest is billed fully and remaining towards the principal or any other component as defined. Thus, there is no accrued holiday interest for processing and trying to defer the holiday interest raises an error.

> **⚠️ Note:** Whenever, a new payment amount is defined while declaring a Payment Holiday, the new amount adjusts the repayment (during the Payment Holiday) in the order of charge, interest and principal components, irrespective of the Payment Rule condition. The remaining amount of the repayment amount, that gets postponed due to the Payment Holiday, is adjusted after the payment holiday period, as per the configuration in Payment Holiday Transaction Class condition.

When a payment holiday is declared for May, June and July installment with Repay Type left blank (that is, the system first adjusts the accrued holiday interest, before the adjusting the normal interest due and principal) the system adjusts the interest accrued during the holiday period, immediately after the defined Payment Holiday.

In the above example, it can be observed that the instalments due for the months May, Jun and Jul are skipped and as per the schedule it is observed that the interest component is adjusted first, from the month of Aug 2022 (instalment date immediately after the Payment Holiday) to Feb 2023.

> **⚠️ Note:** In Constant or Fixed Equal repayment Payment type, the monthly instalment is recalculated to be a fixed amount till the maturity of the loan. In such scenarios, the instalment, immediately after the Payment Holiday, may not clear the entire accrued holiday interest. In such cases, the system apportions the entire repayment to the accrued interest, till the holiday interest is completely paid off and thus the initial few instalments might only adjust the interest component.

Consider a payment holiday for the months of Mar, Apr and May installments with Repay type set as Deferred and Repay Period left blank. The system collects the interest accrued during the payment holiday namely the Holiday Interest, scheduled equally throughout the life of the loan.

Here, it can be observed that the instalments due for the months Mar, Apr and May 2022 are skipped and as per the schedule it is observed that the holiday interest is equally collected throughout the life of the arrangement.

The interest accrued during the holiday period is USD 6095.89 (as seen in AA.ACCOUNT.DETAILS ) and the remaining number of instalment is 297 (that is, (25*12) months – 3 Months= 297 Months). Thus, the Holiday Interest is 6095.89/297 = USD 20.52 per month, till maturity.

| Schedule Months | TOTAL Repayment | Instalment | Principal | Interest | Payment Holiday Interest | Payment Holiday Accrued Interest | Payment Holiday Accrued Interest Cumulative | Outstanding |
|---|---|---|---|---|---|---|---|---|
| 12/2020 | 428.07 | 428.07 | 407.24 | 20.83 |  |  |  | 4592.76 |
| 01/2021 | 0 | 0 | 0 | 0 |  | 19.14 | 19.14 | 4592.76 |
| 02/2021 | 0 | 0 | 0 | 0 |  | 19.14 | 38.28 | 4592.76 |
| 03/2021 | 0 | 0 | 0 | 0 |  | 19.14 | 57.42 | 4592.76 |
| 04/2021 | 592.18 | 585 | 565.86 | 19.14 | 7.18 |  | 50.24 | 4026.9 |
| 05/2021 | 592.18 | 585 | 568.22 | 16.78 | 7.18 |  | 43.06 | 3458.68 |
| 06/2021 | 0 | 0 | 0 | 0 | 0 | 14.41 | 57.48 | 3458.68 |
| 07/2021 | 0 | 0 | 0 | 0 | 0 | 14.41 | 71.89 | 3458.68 |
| 08/2021 | 0 | 0 | 0 | 0 | 0 | 14.41 | 86.3 | 3458.68 |
| 09/2021 | 1191.37 | 1162.6 | 1148.19 | 14.41 | 28.77 |  | 57.53 | 2310.49 |
| 10/2021 | 1191.37 | 1162.6 | 1152.97 | 9.63 | 28.77 |  | 28.76 | 1157.52 |
| 11/2021 | 1191.10 | 1162.34 | 1157.52 | 4.82 | 28.76 |  | 0 | 0 |


##### IFRS Contract with EB Cashflow having Payment Holiday

Consider a scenario where the loan has a monthly interest accrual of 30 and bank has defined a holiday for three instalments. The holiday interest is set to be collected over the four subsequent cycles.

| Scenario | ACC | HOL | DUE Regular | DUE Holiday | Total DUE Interest |
|---|---|---|---|---|---|
| Holiday granted for 3 months at the beginning of the month |  |  |  |  |  |
| Day 1 | 1 Dr | 0 | 0 | 0 | 0 |
| Day 30 | 30 Dr | 0 | 0 | 0 | 0 |
| End of 1st month/Day 30 | 30 Dr | 0 | 0 | 0 | 0 |
| End of 2nd Month | 60 Dr | 0 | 0 | 0 | 0 |
| End of 3rd Month | 90 Dr | 0 | 0 | 0 | 0 |
| SOD of 3rd Month End | 0 | 90 Dr | 0 | 0 | 0 |
| End of Holiday |  |  |  |  |  |
| End of 4th Month | 30 Dr | 90 Dr | 0 | 0 | 0 |
| Bill raised at the SOD of 4th month | 0 | 67.5 Dr | 30 Dr | 22.5 (holiday interest is calculated based as Tot Residual Balance/ 4) | 52.5 Dr |
| Bill raised at the SOD of 5th month | 0 | 45 Dr | 30 Dr | 22.5 Dr | 52.5 Dr |
| Bill raised at the SOD of 6th month | 0 | 22.5 Dr | 30 Dr | 22.5 Dr | 52.5 Dr |
| Bill raised at the SOD of 7th month | 0 | 0 | 30 Dr | 22.5 Dr | 52.5 Dr |

The LENDING-UPDATE-PAYMENT.HOLIDAY is a cashflow type activity. Thus, when Update Holiday is triggered, in the above scenario the cashflow handoff happens as projected below.

| Timeline | Cashflow handoff (Overall Interest) |
|---|---|
| In the above illustration consider that the PH was sanctioned on Apr 1 for three instalments |  |
| 30th Mar | 0 |
| 30th Apr | 0 |
| 30th May | 0 |
| 30th June | 52.5 |
| 30th July | 52.5 |
| 30th Aug | 52.5 |
| 30th Sept | 52.5 |


##### Impact of Change Schedule in Payment Holiday

When the bank/FIIs defines the Repay Period as Deferred, the holiday interest linked to Payment Type or Bill Type gets deferred for the specified period as mentioned in the Repay Period . At the end of holiday period, the system generates a holiday interest payment type automatically for the holiday interest balances associated with the loan and schedule the holiday interest Payment Type by mirroring the schedule associated with the Interest Property in the Payment Type or Bill Type (as defined during UPDATE-PAYMENT.HOLIDAY Activity). Read Payment Type for Holiday Interest for more information.

Once the Payment Holiday is defined, any change in the schedule (frequency change, bill type change, payment type change, start/end dates), cancels or voids all the future Payment Holiday defined (cancels the existing payment holiday). That is, if an arrangement is in a Payment Holiday Period or has defined a Payment Holiday Period for a future date, the change in schedule cancels all the payment holidays from the date of change of schedule.

An override is raised by the system for modification in the schedule of loan carrying Payment Holiday or having a future date Payment Holiday. Fresh holiday instructions need to be declared, if necessary for additional bills.

> **⚠️ Note:** The change in schedule affects the Payment Holiday, irrespective of the usage of the Repay Type field, while defining the Payment Holiday.

For example, during a payment holiday, if the user tries to change the future schedule dates of the loan, then the existing payment holiday from the current date is cancelled by the system and user should request a fresh payment holiday for the recent holiday.

The same holds good when there is payment holiday scheduled in future and the payment schedule is changed prior to that scheduled payment holiday.

A mortgage arrangement of USD 300,000 for 25 years, is opened and disbursed as on Apr 15, 2021. Repayment is set as monthly, and Payment Type set as Constant.

As per the customer request, the bank/FIIs applied for a Payment Holiday, from May to Sep. Now the customer requests a change in the repayment schedule of the arrangement from monthly to bi-weekly, before the payment holiday gets exhausted. This results in raising an override stating 'Change in payment schedule will ignore payment holiday requests if available' and there by makes all the existing Payment Holiday defined as void.


##### Payment Holiday Dates

The following section describes backdated and future dated payment holidays with illustrations.


###### Back Dated Payment Holidays

When a customer is unable to repay his loan and has missed few installments, it is possible that the bank declares those missed installments as payment holidays and restructures the loan. In this scenario, the holiday start date cannot be less than the Activity effective date. For the holiday start to be backdated, the Activity has to be run backdated. This means that, the bank or FIIs can provide a Back Dated Payment Holiday, if the LENDING-UPDATE-PAYMENT.HOLIDAY activity is also back dated.

Consider a mortgage that is in NAB status due to outstanding bills.

Now the customer approaches the bank/FII requesting for a back dated payment holiday, from Feb 1, 2022 to May 1, 2022 and the same gets approved. Accordingly, bank/FIIs agrees for the same.

After the payment holiday is declared, the customer does not miss any payment and his overdue status is reassessed based on the new schedule. The loan is not in NAB status after this restructure of declaring a back value dated payment holiday.


###### Future Dated Payment Holiday

If the start date is in the future, then the base date for holiday payment calculation, is the previous payment date of the holiday start date.


##### Amending Payment Holiday

Payment holiday definition can be reversed, by reversing the actual activity. Any amendments to the existing holiday payments definition can be made by using the CHANGE-PAYMENT.HOLIDAY activity. This functionality helps the bank/FIIs to modify or cancel an already defined Payment Holiday.


##### Payment Holiday Limit

Payment Holiday Limits allow the bank/FIIs to provide flexible payment or payment holiday options to the customer, by either reducing the repayment amount or by skipping the same, upto a defined limit agreed by the bank/FIIs and the customer. The Payment Holiday limit can be defined by configuring the Payment Schedule Condition as explained in Payment Holiday Limit.

When the repayment obligation is reduced or skipped for a customer, the system compares the amount reduced from the original repayment and with that of the available payment limit defined. An error or an override can be defined, if the limit is breached as per the banks/FIIs convenience.

There can be situations, when the schedule payment amount may change due to changes in rate of interest, term or cancelling the declared holiday in the loan. In such circumstances, the system automatically updates the Payment Holiday limit based on the new payment amount and triggers an alert to the customer when the limit is breached.

Consider the following conditions:

- The maximum limit for flexible repayment is USD 30000
- Every month instalment is due for USD 10000.

Consider a contract, having a term of one year for USD 120000 as on Jan 1,2020. The customer now requests for a payment holiday of the entire installment, for the months of Apr, May and Jun. Accordingly bank sanctions the payment holiday. Thus the Payment Holiday Limit now is USD 30000 and the Utilised Payment Holiday Limit is USD 30000.

Later the customer approaches the bank requesting for cancelation of the Payment Holiday, for Jun. This is approved by the bank and thereby the Available Payment Holiday limit becomes USD 10000 and Utilised Payment Holiday Limit now is USD 20000.

Now, the bank decides to increase the interest for the said contract, after Apr. This results in increasing the payment amount from USD 10000 to USD 11000 for the month of May. Since the month of May is within the defined Payment Holiday, the Utilised Payment Holiday Limit increases to USD 21000 and the Available Payment Holiday limit becomes USD 9000.

A mortgage arrangement of USD 500,000 for 25 years, is opened and disbursed as on Jan 1, 2022. The Payment Holiday Limit for the arrangement is set at USD 50,000.

A Payment Holiday is applied on the arrangement, for the months of Feb to Jun 2022, for the Payment Type Constant, Repay type Deferred and Repay Period left blank (that is, the system collects the interest accrued during the Payment Holiday or Holiday Interest, equally throughout the life of the loan).

The bank as on Apr 19, 2022 decides to increase the margin of the interest from 0.50 to 25.00.

This in turn affects the scheduled payments from Apr 19,2022 and the same can be seen in the schedule of the arrangement. However as the arrangement is in the Payment Holiday Period (that is, from Feb to Jun 2022), the said increase in the interest, is adjusted with Payment Holiday limit. The same can be observed, by the reduction of Available Payment Holiday limit from USD 35.381.95 to USD 34.113.45 as shown below.

Consider a loan having a Payment Holiday Limit of USD 3000 and monthly installment of USD 4500. In this scenario, while placing a Payment Holiday request, the system displays an error message, as the available Payment Holiday Limit is less than the monthly instalment and thus the New Payment Amount field should be entered maximum to the extent of 3000 USD.


##### Revolving Payment Holiday Limit

A Payment Holiday Limit can be configured to reinstate to its initial defined Payment Holiday limit, due to adhoc or excess repayments, over and above the due amount. This can be configured as defined in the Payment Holiday Limit in Payment Holiday configuration. Upon creation of an arrangement, the customer can request for a repayment holiday. The system evaluates the Repayment Holiday Limit for the product and accordingly reduces or skips the repayment obligation, as per the Flexible Payment Limit available. For revolving Payment Holiday Limit, any excess payment towards the principal, results in the evaluation of the Available Payment Holiday Limit with that of the Payment Holiday Limit defined and there by restoring the Payment Holiday limit to the extend of the defined Payment Holiday Limit (This is termed as Limit Restoration). The Available Holiday Limit is updated online and the same is evident in the Arrangement Overview page. This process can be understood from the scenarios below.

Consider a one year loan, starting from Jan 1, 2021, for an amount of USD 120000. The monthly repayment is say USD 10000 and Payment Holiday Limit USD 30000.

After settling the bills of Jan, Feb and March, the customer requests for a payment holiday on Mar 20 for next two bills. As the payment holiday is given for USD 20000, the holiday limit is reduced to USD 10000. When the customer makes a repayment of USD 50000 towards the principal of the loan on Mar 25, it reinstates the Payment Holiday Limit to its initial defined Payment Holiday Limit of USD 30000.

Consider a loan account in overdue status for USD 4500. The Payment Holiday Limit for the said loan is defined as USD 5000 and the Available Payment Holiday Limit for the loan as of now, is USD 2000.

The customer now approaches the bank for an excess payment of USD 6000.

The system adjusts excess payment, against the overdue amount of USD 4500 and the remaining amount of USD 1500 is used to replenish the Available Payment Holiday Limit (maximum to the extend of the initial defined Payment Holiday Limit of USD 5000). The New Available Payment Holiday Limit is USD 3500.

Consider a loan having Payment Holiday Limit of USD 5000 and monthly installment amount of USD 4500. The customer holds an excess amount of USD 6000 in his loan account.

Now the customer requests a Payment Holiday for the coming two months, summing to an amount of USD 9000 (that is, 2*USD 4500=USD 9000). The customer expects the same to be approved (as he holds an excess amount of USD 6000 in his loan account and has a Payment Holiday limit of USD 5000), however the system raises an error, as the system while defining the Payment Holiday checks the Payment Holiday limit and the customer only has a Payment Holiday Limit of USD 5000.

> **⚠️ Note:** The system does not consider the excess amount during repayment holiday request evaluation.


##### Controlling Payment Holidays Count

Banks/FIIs can control the number payment holidays allowed in an arrangement by configuring the HOLIDAY.COUNT periodic attribute in the Payment Schedule product condition. (Read Controlling Payment Holidays Count Configuration for more information)

Consider a mortgage arrangement in Lending product line, where the number of payment holidays that can be defined in a year is restricted to five (using the HOLIDAY.COUNT.YEARLY periodic attribute). If the user defines more than the stipulated payment holidays, the system raises an override.

When the customer tries to define a payment holiday for six instalments, the system displays the following override message: Maximum negotiable value of 5 has been exceeded by 1 in field SCHEDULE.


##### Defining Restriction on Consecutive Payment Holidays

The system supports restriction of payment holiday in parallel (that is, if an arrangement is within a payment holiday, further definition of a payment holiday is restricted, unless and until the current payment holiday period has expired), through the HOLIDAY.RESTRICT.LIFE periodic attribute, configured in the Payment Schedule product condition (Read Payment Holiday Configuration for more information).

> **⚠️ Note:** The system restricts definition of parallel payment for payment holidays having Repay Type as Deferred, without the configuration of the Periodic Attribute in the Payment Schedule product condition.

Consider a mortgage arrangement in Lending product line with HOLIDAY.RESTRICT.LIFE periodic attribute configured to raise an error, while defining a parallel payment holiday. Payment Holiday is already defined for the months of February, March, April, May, June and July.

The system’s current date is April 19, 2022 and the user tries to define a payment holiday for the month of August. The system displays the following error: Multiple Holiday requests are restricted in same holiday period.


##### Paying-off during Payment Holiday

Payoff Simulation and Direct Payoff of the loan arrangement, in a holiday or grace period, as well as, the loan arrangement carrying the unbilled holiday interest, is possible. The payoff statement is generated for the entire loan outstanding including the accrued holiday interest and due holiday amount.

Consider that a user triggers a payoff on a loan which is within the payment holiday period. The principal is 1000, due interest amount is 200, accrued interest is 50 and holiday interest balance is 20 (holiday balance represents accrued holiday interest which is yet to be billed).

The loan payoff simulation generates a payoff statement reflecting the holiday interest property along with the property like principal, interest and any fees or charges.

For the above example a payoff statement is generated with the components below.

- Payoff amount = 1270
- Account = 1000
- Interest = 270 (that is, Due Interest Amount=200, Accrual Interest=50 and Holiday Interest= 20)

Payoff bill includes the holiday interest accrual as part of the overall payoff bill.

Consider a user triggers payoff on a loan after payment holiday period ends. The principal is 1000, due interest is 205 (that is, Due interest for the current bill is 200 and the due Holiday Interest is 5), accrued interest is 50 and holiday interest balance is 15 (holiday balance represents accrued holiday interest which is yet to be billed).

The loan payoff simulation generates a payoff statement reflecting the holiday interest property along with the property like principal, interest and any fees or charges.

For the above example a payoff statement will be generated with the components below.

- Payoff amount = 1270
- Account = 1000
- Interest = 270 (that is, Due Interest Amount=205, Accrued Interest=50 and Holiday Interest=15)

Payoff bill includes the due holiday interest amounts and holiday interest accrual as part of the overall payoff bill.


##### Cancelling Holidays Declared

The user has an option to cancel or shorten the holidays declared, through Modify/Cancel Payment Holidays field in the Arrangement Overview page. The system triggers LENDING-CHANGE-PAYMENT.HOLIDAY when a payment holiday is modified or cancelled.

The payment holiday can be fully cancelled or modified to cancel specific number of holidays. But this cancellation should be consecutive. Out of four schedules marked as holiday, it is possible to:

- Cancel first
- Cancel last
- Cancel first few
- Cancel last few

But it is not possible to cancel the holidays in between or in a random order.

Change in schedule after cancel of payment holiday for Jul is:

Cancellation or shortening of holidays can be done only for consecutive schedules and error is raised when the user attempts to cancel the non – consecutive holidays.


##### Payment Holiday During Migration

The system allows migrations of loans under active Payment Holiday definitions. There are possibly two scenarios to be considered during migration or upgrade of loans.

- Loan under payment holiday period at the time of migration
- Loan completed grace or holiday period repaying holiday interest at the time of migration


###### Legacy Migration

The migration sequence in case of legacy loans with payment holiday is as follows:

1. Takeover arrangement
2. Capture outstanding loan bills and balances
3. If the loan is migrated during the holiday period, capture accrued interest (Holiday Interest).
4. Capture any future holidays using ‘Update Holiday’ and recalculate options can be configured suitably.


###### Upgrading Clients

For a customer upgrade to a loan product having payment holiday functionality,

1. Cancel existing holiday instructions
2. Re-configure fresh holiday instruction with defer option.


###### Legacy Migration

The migration sequence in case of legacy loans with payment holiday are as follows.

1. Takeover Arrangement
2. Capture outstanding loan bills and balances including the Holiday Interest due and accrued
3. Update ‘Schedule’ for ‘Holiday Interest’ and specify start and end dates based on the period over which the holiday interest is billed


###### Upgrading Clients

For a customer upgrade to a loan product having Payment Holiday,

1. The accrue interest is billed fully at the end of the Holiday Period
2. The holiday Instructions are performed if needed with Holiday functionality in the New Loan Product.
3. If bank perform upgrade after the end of holiday period and before billing of accrued holiday interest and wishes to use deferred functionality, then they can reverse the earlier holiday requests and reconfigure fresh holiday instructions with defer option.

The Update Holiday activity allows Payment Holiday to be defined for a repayment scheduled on loan takeover or migration date.

Consider a scenario where the loan takeover or migration date - May 1, 2021, as per the original schedule, and last repayment date is Nov 1, 2021

The user triggers Payment Holiday on May 1, 2021 for the repayment scheduled on the same day (May 1, 2021) with recalculation option as Term. The repayment due for May 1 is considered as a holiday by the system and extends the schedule to Dec 1, 2021 (as term is recalculated).

| Timeline | Accrual | Handoff |
|---|---|---|
| Month 1 | 30 | NA |
| Migration triggered with holiday accrual booked under MIGRPHINT property. This property is set to exclude from EIR calculation. Post migration interest is booked under PHINT property. Holiday declared for month 2 & 3 and repay period set as ‘4’ cycles. |  |  |
| Month 2 (Holiday) | PHINT – 30 MIGRPHINT -30 | NA |
| Month 3 (Holiday) | PHINT – 60 MIGRPHINT -30 | NA |
| End of Holiday period. Here both pre and post migration interest portion are assumed to set as deferred and repaid over 4 billing cycles. The overall pre migrated holiday interest (MIGRPHINT) is split across 4 cycles at 30/4=7.50 The overall post migrated holiday interest (PHINT) is split across 4 cycles at 60/4 = 15 |  |  |
| Month 4 |  | PHINT – 15; MIGRPHINT – 7.50 (Exclude from EIR) |
| Month 5 |  | PHINT – 15; MIGRPHINT – 7.50 (Exclude from EIR) |
| Month 6 |  | PHINT – 15; MIGRPHINT – 7.50 (Exclude from EIR) |
| Month 7 |  | PHINT – 15; MIGRPHINT – 7.50 (Exclude from EIR) |


> **Related Applications:** `AA.ACCOUNT.DETAILS`, `AA.PERIODIC.ATTRIBUTE`

---


### 2.29  Scheduling Payments


> **📇 Quick Reference Card**
> 
> **Applications:** `AA.ARR.PAYMENT.SCHEDULE`, `AA.ARRANGEMENT.ACTIVITY`, `AA.BILL.DETAILS`, `AA.INTEREST.ACCRUALS`, `AA.PAYMENT.TYPE`, `AA.PRD.DES.PAYMENT.SCHEDULE`, `AA.PROPERTY.CLASS`, `AA.SIMULATION.CAPTURE` ... +1 more
> 
> **Key Fields:** *Actual Amount*, *Actual Amt*, *Actual Pay Date*, *Advance Payment Restriction*, *Aging Status*, *Alt Payment Method*, *Alt Payment Routine*, *Amortisation Term* ... +49 more
> 
> **Sections:** ⚙️ Configuration | 🔧 Working With


#### ⚙️ Configuration

The following section describes the configuration required for scheduling payments.


##### Scheduling Payments

The Payment Schedule Property Class is used to schedule the payments for a loan arrangement. The user can input Payment Schedule values. Payment Type is a mandatory information and can be created by users. The available Payment Types are stored in AA.PAYMENT.TYPE table, which can be accessed through the AA Product Builder. Some of the payment types supported by AA are listed below:

- Constant: This results in constant repayments, that is, the principal and interest repayment are constant. It is used for Annuity arrangements. It requires both account and interest properties to be specified in the Payment Schedule Property Class. The Charge Property can be optionally added.
- Linear: Here, the principal repayment remains fixed over the lifetime of the arrangement. Optional properties such as Interest, Charge and Tax may be included. The actual amounts calculated by these properties are added to the fixed principal amount repayment. For a bill to be generated for Linear Payment Type on the arrangement creation date, Schedule Type must be set as Online and during the arrangement creation in Payment Schedule, set the Start Date field as the arrangement start date.
- Actual: When the Type is Manual, then the allowed Calculation Type is Actual, in which case, the user has to specify an amount in the arrangement for the Payment Type. When the Type is Calculated, Actual is normally used for repayment of the calculated property classes (for example, Interest, Charge and Tax) and the amount is determined on each payment schedule date. It can also be used in conjunction with the Account Property Class, such as, Principal, when a percentage need to be specified in the Payment Schedule Property Class.
- Transaction: This makes use of the disbursement transaction amount and capped charges linked with the activity as the source to calculate the payment amount.
- Percentage: In this calculation type, the repayment is linearly distributed for the percentage defined over the period. This is allowed for both Principal and Interest properties together for blended payments and just the Account property for Principal only payments.
- Fixed Equal Repayment: Payment Type Fixed Equal defines a manual repayment amount for the loan. As the name indicates, it is a fixed repayment amount given by the user. In addition it is also possible to specify the component that has to be fully invoiced which could supersede the fixed equal repayment amount defined by the user. Please refer to scheduling payment types
- Progressive: On choosing this type, a progressive percentage should be defined in the Prog Pay Perc field . The system calculates an amount which is progressing by the rate specified in Prog Pay Perc . Exactly same as CONSTANT type when Prog Pay Perc is defined as 0. Optionally user routine could be attached for this type.
- Other: It is a user routine attached to the Calculation Routine field.
- Rule 78 Routine based calculation: The lending arrangement can have payment schedules built on Rule 78 calculation. A Routine based Payment Type can be used to achieve this. The Cal Routine in those payment types should use the AA.CALCULATE.RULE78.PRIN.AMOUNT and AA.CALCULATE.RULE78.INTEREST.AMOUNT routines to build the principal and interest schedules respectively. Read Rule78 payment setup for more information.

- Payment Method : Once the Payment Type has been specified, the user can specify whether the amount is Due (to or from the customer), Pay (for rebates and automatic scheduled disbursement) or Capitalised.Interest only bills of loans can be capitalised to the principal for Islamic finance contracts and conventional loans.
- Max Percentage: Restricts the percentage definition in Percentage attribute in Payment Schedule product conditions. The repayment percentage of original loan principal definition is restricted to maximum of percentage defined in this attribute. Amortisation Schedule always covers 100% of total granted loan amount but the calculation percentage is based on the maximum percentage defined.

Payment Schedule conditions can be pre-constructed through AA.PAYMENT.TYPE and default values can be assigned to Payment Schedule conditions during the arrangement creation using an API validation.

Read AA.PAYMENT.TYPE in Payment Schedule property class for further details.

If a specific amount needs to be collected on the final schedule date, that amount may be stated in Residual Amount field of the Payment Schedule production condition. The amount stated in this field is exclusive of any scheduled calculated amount on the final schedule and is always considered to be belonging to ACCOUNT property.

If a specific amount (residual amount) needs to be collected at the payment end date of the term, it can be achieved by either defining the residual amount or by defining an amortisation term in the Amortisation Term field.

The Payment Mode field can be set to ADVANCE for payment of advance interest. The Interest Property Class is mandatory and it is possible to input in this payment mode setup.

- Payment Freq field - indicates the frequency at which payments are made due.
- Start Date field - indicates the actual payment start date. If the start date is mentioned, then the payment frequency is applied on the start date. Else, the system defaults it from the base date. Ad-hoc payment dates can be defined by expanding the multi-value sets and defining the dates in the Start Date field. Payment and Due Frequency fields have to be null. Additionally, an End Date or Number of Payments can be specified to indicate when the payments should terminate.
- End Date field - indicates the actual payment end date.
- Either an End Date or Number of Payments can be specified to indicate when the payments should be terminated.


##### Issue Bill In Advance

Bills can be issued in advance by setting the In Adv (BILL.PRODUCED) field in the Payment Schedule product condition for all payment types.

On the bill issue date, the system considers any forward-dated changes between the issue bill and payment dates to schedule and calculate the bill amount for the current period. However, any forward-dated change between the issue bill and payment dates that is input after the bill is issued, is effective only from the next payment date.

It is not possible to modify a bill once it is issued except if the Finalise Bills field is defined in the payment schedule condition. The only approach to modify an issued bill is by using the Payment Holiday feature when the issued bill has not crossed the finalisation period.

> **⚠️ Note:** When the loan has a floating rate or a periodic rate, the corresponding Payment Schedule must have the On Activity and Recalculate set of fields, set to recalculate the payment amount. Similarly, any other forward-dated condition in interest or other components should have a corresponding forward-dated Payment Schedule for the payment amount to be recalculated. Only when the system has a corresponding payment amount recalculation setup available, it is enabled to produce the bill in advance considering the changes between issue and due dates. Read Defining the Bill Rules for more information.

Bills issued in advance are treated as current bills and can be settled in advance irrespective of the Advance Payment Restriction field defined in Payment Rules Condition.

For a Periodic Charge, bills can be issued in advance only when the Property Type is set as Defer. If the Periodic Charge is not set to defer, the system raises an override to indicate that the bills can be issued in advance only for Defer type of periodic charges.

The assessment period for the Defer type of periodic charges are from previous issue bill to current issue bill date. The system triggers LENDING-ISSUEBILL-PERIODIC.CHARGES* in accordance to the value defined in In Adv (BILL.PRODUCED) field in Payment Schedule condition.

- The bill generated on the advance date includes all the deferred charges from previous issue bill date to the current issue bill date. Periodic Charges of Defer type should include all the deferred charges only. Other features like activity-based charges with free counts are not possible in Defer type of periodic charges.
- Any charge raised after the current issue bill date is included in the next assessment period and in the next billing cycle.
- The periodic charges are be made due on the payment date and can be repaid thereafter.

During an advance payment between the issue bill date and the payment date, the payment is appropriated against periodic charges based on the Payment Rules condition. Advance repayments of loan installment is possible for all payment types excluding the payment types based on transaction amount and routines.

For a product with Periodic Charges set to Defer and with issue bill in advance, the system validates if the Periodic Charges property is found in the advance payment rule configured for the product. If it is missing, then the system raises a validation error (at proofing or arrangement level).

The order repayment should be: Periodic Charges, Charges, Interest and then the Principal.

In the example given below, the AGEINGFEE and DISBURSEMENTFEE activity charges are set to Defer Application Method .

These two charges are collected using a PCDEFER periodic charge property which is set to Defer property type . Therefore, this PCDEFER property can be set to generate bills in advance.

The periodic charge property which is set to Defer property type should have its corresponding product condition as follows:

The Payment Schedule should have bills issued in advance for the PCDEFER Property.


###### Extend Cycle

Periodic charges, interest and scheduled charges can be extended and collected beyond the loan maturity date or the loan payment end date by setting the Extend Cycle field to the corresponding property class for the payment type.

In the example given below, the EXTENDPC Payment type has Extend Cycle field set to PERIODIC.CHARGES.

The EXTENDPC payment type has the Extend Cycle field set to PERIODIC.CHARGES. Thus, the AGEINGFEE which is charged after the loan maturity or the loan payment end date can be extended and collected as a part of the PCDEFER periodic charge property as Extend Cycle is set.

The PCDEFER periodic charge is set to be made-due every month with the bill to be issued 10 days in advance.

Thus, the system can be configured for:

- Only a Periodic Charge with Defer property type
- Only a Payment Type which has Extend Cycle set
- A Periodic Charge with Defer property type and a payment type with Extend Cycle set to collect the deferred charge. The system raises an error if the loan’s maturity date has a defer type periodic charge’s due date (bill issued and made due on the maturity date) indicating Payment Type is not set as Extend Cycle . Thus it ensures that all deferred charges are made due till the loan is closed.

Read the Payment Schedule Property Class user guide for more information on other options available for setting up schedules.


##### Minimum Payment Amount

A minimum payment amount is required to be defined by some financial markets. AA supports to capture a minimum payment amount based on the bill type. This gives the flexibility for the users to group properties by bill type and assign a minimum payment amount for them.

- It is possible to setup minimum payment amount based on the bill type – Note that it is applicable only if Account Property and on Actual Payment Type.
- The Group Min Property field is a part of the Minimum Payment set of fields to capture the Minimum Invoice Component (MIC). This field is mutually exclusive with Group Min Amount .
- Bill Type wtise MIC can be defined using the Group Bill Type and Group Min Property set of fields.

In the Group Bill Type field, only Payment type records are allowed.

> **⚠️ Note:** Any bill type defined in this attribute should not be set against the system calculated payment types namely Linear, Constant and Progressive. In the Group Min Amount field, a minimum payment amount should be indicated for the bill type mentioned.

The Minimum Payment Type field is applicable only when the payment type for Account Property displays the CalculationType field set to Actual and the Type field set to Calculated.

- If the calculated payment amount for the given bill type is less than the minimum payment amount, then the bill is raised of the minimum payment amount. The difference is billed as principal (Account Property).
- This is allowed only for scheduled payments and not for Activity-based charges or break rule charges.
- Minimum payment amount calculation can be considered during payment schedule projections and during simulations.
- The following attributes indicate the minimum amount for an arrangement. Group Bill Type field - indicates the bill type for which the minimum amount has to be applied. Group Min Amount field - indicates the minimum bill amount.
- On the scheduled payment date, when a bill is raised for the bill type mentioned in the Group Bill Type field, the system evaluates the calculated payment amount against the minimum amount specified. When the calculated amount is greater than or equal to the minimum amount, then the calculated amount is billed. When the calculated amount is lesser than the minimum amount, then the minimum amount is billed. The differential amount is billed as Account (Property).
- Minimum payment amount can be applied only to Actual payment types and does not apply for Constant, Linear or Progressive payment types.

When the bills are set to combine, the system raises a consolidated bill for all payment type lines that has a scheduled bill getting due on the same date.

BT.MINIMUM.AMOUNT is considered only when the Account Property is part of the combined bill.

- If the Account Property is not available, then the calculated property amounts are billed at actuals.
- If the Account Property is available, the system checks if the sum of the calculated amount per property (including Account) is greater than or equal to the minimum amount.
- If there is a short fall, the difference amount is increased in the Account Property to match the minimum amount specified.

When the bills are not set to combine, the system raises separate bills for each payment type. When there is at least one bill for an Account Property, the system compares the calculated amount of all bills scheduled for the date sharing the same bill type to see if it is greater than or equal to the minimum amount specified.

If the condition satisfies, the system issues the bill for the calculated amount. If the condition fails, the system issues the bill for the minimum amount specified.

When the system tries to adjust the account portion of the bill to match the minimum payment amount and the adjustment amount is more than what is outstanding in the CURACCOUNT, then the system restricts the adjustment to what is available in the CURACCOUNT.

> **⚠️ Note:** Minimum payment amount is considered even when recalculating the payment schedule.


##### Fixed Equal Repayment

- Arrangement loans can generate the Fixed Equal Repayment (FEP) Schedule.
- AA.PAYMENT.TYPE - FIXED.EQUAL is used in loan arrangements to indicate an FEP schedule. This payment type displays the Calculation Type field as manual. The mandatory Property Classes are Account (Principal) and Interest.
- The user can manually input the repayment amount during arrangement creation in the Actual Amount attribute in the Payment Schedule. The schedule projection is based on this user input FEP amount. The value in the Term field is optional for this Payment Type.
- When the Term field is not captured, it is calculated based on the FEP amount given by the user.


##### Zero Payments

Regular payment can be skipped completely once or for a regular period. Remaining payments adjust the skipped installment. Zero payment can be done either by skipping the month(s) in Pay Freq field or by giving only start and end date and skipping the interim payment(s).


##### Progressive Payments

The PROGRESSIVE payment type is used to increase the repayment amount by a pre-defined frequency captured in the Pay Freq field.

- When the Pay Freq attribute is 0%, the system behaves like an Annuity contract. If it has a percentage defined for example 2%, it means, the repayment amount increases by 2% for every repayment and the entire principal is settled on the payment end date.
- The Prog Pay Perc attribute in the Payment Schedule component accepts the progressive rate at which the repayment amount can be incremented for every repayment


##### Future Dated Conditions

The user can introduce a new date at the arrangement level using the FORWARD.DATED value in the Type attribute in the AA.PROPERTY.CLASS record. Once captured with a future date, the system automatically schedules this, and during close of business, the scheduled activity is processed applying the new condition to the Arrangement.


##### Payments Linked with Disbursement

- The consumer loan business segment would require a down payment (of principal) along with each disbursement. This is calculated as percentage of the net movement on CUR balance.
- Such a payment calculation requires the following information The disbursement event, in order to configure a payment calculation whenever a disbursement event occurs. The source on which the (down) payment has to be calculated. Optionally, a configuration to generate the bill online.
- DISBURSEMENT, is a relative date option that is used to identify the disbursement event and triggers a payment calculation. This should be specified in the Start Date field.
- Payment type with Calc Type as TRANSACTION is to calculate the payment based on net movement.
- Schedule Type has to be set as ONLINE, if the bill has to be generated online along with the disbursement.

For instance, if there is a disbursement of 1000, with a charge of 200 (set to cap) that is linked, the payment amount can be defined as a % of 1200. If the % is defined as 25%, then the system calculates a payment of 300. The condition is shown below.


##### Special Payments

Special payment is the actual amount specified by the user to substitute the regular instalment amount for the specific period, either single or regular. This amount should be specified in the Actual Amt attribute.

For example, the instalment amount needs to be different (user defined) for every March and the system calculates the value in the Calc Amount field for the remaining instalments by considering the specific payment for the given instalment(s).


##### Deferred Payments

The Defer Period attribute in the Payment Schedule Property Class is used to define the duration the scheduled payment should be deferred from the original cycled date.

When a value is defined in the Defer Period attribute, then the system schedules DEFER.MAKEDUE or DEFER.CAPITALISE activities on the cycled date and moves the bills to DEFER status.

On the cycled date + Defer Period, the system schedules MAKEDUE or CAPITALISE activities where the bills are be moved out from the DEFER status to their respective status.

> **⚠️ Note:** The defer period should not be more than the payment frequency defined in the payment schedule condition. In case the defer period is more than the payment frequency, the interest cycle fails and subsequent schedule of the Defer Capitalise or Defer Make-Due activities are not cycled to the next date.


##### Calculation of Annual Percentage Rate

Read the Annual Percentage Rate section in the Reporting Property Class user guide for more information on Annual Percentage Rate (APR) calculation.


##### Installment Amount for Multiple Disbursement

The Include Future Disb (INCLUDE.PRIN.AMOUNTS) attribute in Payment Schedule specifies the option for calculating the EMI considering the future installments.

When left blank, the default behavior continues. For a loan with multiple disbursements, the installment amount is calculated on the first disbursement and on further disbursement the user has to configure the system to recalculate the Term or Payment amount using On Activity, Recalculate fields. Else, the system lets the future disbursements get adjusted to repay in the final installment on the maturity date.

When the Include Future Disb field is set to Yes, the system calculates the constant installments with interest on outstanding principal and future disbursements or payments scheduled. This facility is applicable for all payment types. This feature is also applicable for fixed profit contracts.


##### Full or Partial Capitalisation of Interest/Profit

This section describes the full or partial capitalisation of interest and profit accruals in detail.

The Alt Payment Method field in AA.PAYMENT.TYPE is set to Due And Cap, to enable full or partial capitalisation of interest accruals in a loan. The actual amount indicated in the payment schedule is only made due and any remaining interest accruals are capitalised. This option can be used both in Islamic and conventional banking and it enables capitalization of profit accrued but not due for repayment in current period.

This option is available for the annuity repayment type. Hence both Account and Interest properties should be part of the payment type definition.

This option is not available for repayment types like principal only repayments, interest only payments, progressive payments, percentage payments (step up or step down), accelerated payments, transaction payment types and fixed equal repayments. The system raises an error if Due and Cap option is chosen for any of these payment types.

When a Due and Cap payment type is used in the payment schedule, the Payment Method field should be set as Due. The system raises an error when Payment Method is set as Capitalise.

> **⚠️ Note:** The system raises an error if the Interest Property used under a Due and Cap payment type is of the Residual Accrual Property Type.

When the Alt Payment Method field in AA.PAYMENT.TYPE is set to CAP AND INV, then during Charge Capitalisation, if the account has insufficient funds to capitalise a charge the pending amount is invoiced to the customer. The system retries the invoiced charge automatically at regular intervals using the Transaction Cycler facility. This indicates that the bill amount must be capitalised for the funds (based on the settlement rules) and invoiced for the unrealised balance.

When a charge like activity charge, scheduled charge, rule break charge is set to Capitalise and payment type indicates Alt Payment Method attribute as CAP AND INV, then the pending amount for settlement after capitalisation is invoiced to the customer. The pending charge amount, which is invoiced, is moved to INV .

The Settlement condition can be set as Full, Partial or None to indicate if the account is fully debited irrespective of the balance available, partially debited for the available amount or not debited at all when full funds are not available respectively.

Read Charges Property Class for more information.

> **⚠️ Note:** CAP and INV can be used only for Interest and Charges Property Class in the schedule. Periodic Charges cannot use the CAP and INV option.


#### 🔧 Working With

The following section describes the process of scheduling payments.


##### Scheduling Payments

Bills are generated on the scheduled date (or in advance based on the Inadv field in payment schedule).

The bills generated on the payment schedule is stored in AA.BILL.DETAILS record.

In the outstanding bills enquiry of the loan, the outstanding amount is inclusive of the tax amount on accrued penalty interest only when Tax Inclusive field is set as Yes in a payment rule of the product. The details can be read through the drilldown as shown below.

The bill details include the billed components. The tax related components for the bill are listed in the drilldown next to the bill details.

An illustration of another contract where a bill is settled is shown below. The details of the principal, interest and the tax settled are seen in the AA.BILL.DETAILS .

When a bill is deferred for a specific payment type, the defer date is updated in the AA.BILL.DETAILS record based on the Defer Period in the Payment Schedule.

The property specific original amount that is the outstanding property amount is indicated in the bill. Any adjustments are also seen in the record.

The bill details displays three sets of fields:

- Bill Status field - takes the values ISSUED, DUE, AGING and SETTLED based on the life-cycle of the bill. For example, when the bill is deferred, the Bill Status has the value DEFER after being issued and before becoming DUE.
- Settle Status field - updates as UNPAID and then as REPAID when the bill is settled.
- Aging Status field - takes the values GRACE, DEL, NAB, etc., and finally SETTLED. Note that GRACE, DEL, and NAB values are given based on the overdue

When the bill is paid or made due in advance and the payment bill is generated but paid after the cooling period if any, the MAKEDUE.ADVANCE Activity is scheduled one day after the cooling period. Any interest or principal changes through the Activity affects the interest and the final interest in the Tot Due Amt field of AA.INTEREST.ACCRUALS . The difference is paid or made due immediately.

The AA.BILL.DETAILS record stores the Property wise outstanding balances and ageing status. Read the Payment Schedule Property Class user guide for more information.

The below screen shot displays the bill details that contain multiple properties, billed amount and outstanding amount.

The below screenshot displays the ageing information, bill status and settle status.

The aging references are stored along with bill references and payment indicator.


##### Pre - Notification and Finalisation of Payment

Loan customers are advised N number of days in advance of an upcoming payment. From the notification date, the customers can choose to make changes to their upcoming payment till the bill amount is finalised . Upon reaching the finalisation date, no further changes are allowed for the upcoming payment and system triggers settlement processing for claiming funds from clearing. In case of no finalisation date, then the upcoming payment amount can be modified until the day before the payment date.

This functionality is achieved through Payment Schedule Property Class through the Bill Produced and Finalise Bills attributes. The period defined in Finalise Bills should be less than Bill Produced .

Scenario: Consider the following conditions.

| Attribute | Value |
|---|---|
| Payment date for a scheduled payment | 14-May-2020 |
| Bill Produced | 10D |
| Finalise Bills | 2D |

Ten working days (10D) prior to the payment date of 14-May-2020 is 30-Apr-2020 and the bill is issued on 30th Apr 2020 and the payment amount can be modified either by way of increasing or decreasing it until 12-May-2020

> **⚠️ Note:** The finalised payments are not shown during change activity where the user can modify the holiday amount.


##### Minimum Payment Amount

The user can setup bill type wise minimum payment amount using the Group Bill Type and Group Min Amount fields.

- Create an LOC Product with 3% principal repayment, monthly Monthly minimum payment of 1000
- Create an arrangement with 3% principal repayments with monthly frequency.
- View the Payment Schedule projection when the loan is not disbursed.
- Make a disbursement of 34T as of arrangement start date.
- View the Payment Schedule projection after the disbursement is authorised.
- View in detail the 04/25 bill.
- The outstanding amount was 34,000 and the interest percentage is 3%, which is 1,020. The calculated amount is greater than the minimum payment amount of 1,000 and hence the calculated amount is billed.
- View in detail the 05/25 bill.
- Here, the calculated amount is 989. The calculated amount is less than the minimum payment amount of 1000 and hence the minimum amount is billed.

- Create a LOC Product with 3% principal repayment, monthly Actuals of interest accrued, quarterly. Interest rate is 6% Monthly minimum payment of 1500
- View the Payment Schedule projection when the loan is not disbursed.
- Make a disbursement for 20T as of arrangement start date.
- View the Payment Schedule projection after the disbursement is authorised.
- View in detail the 05/30 bill.
- View the actual bill raised for 05/30.
- View in detail the 07/30 bill.
- Here, 3% of outstanding principal is 510 (17,000 * 3%). The interest balance is 299.18. The cumulated amount is 809.18. Since this is less than the minimum payment amount of 1,500, the bill is produced for the minimum amount. The difference amount of 690.82 is added to the Account Property.

- Create a LOC Product with 3% principal repayment, payable monthly, with bill type as INSTALLMENT. Actuals of interest accrued, payable quarterly, with bill type as PAYMENT. Interest rate is 6%. Minimum payment amount for INSTALLMENT bill type and PAYMENT is 1,000 and 500, respectively.
- View the Payment Schedule projection before the loan is disbursed.
- Loan is disbursed for 30T as of arrangement start date.
- View the Payment Schedule projection after the disbursement transaction is authorised.
- View in detail the 04/25 bill.
- Here, the calculated amount is 900 (30,000 * 3%) and hence the bill is raised for the minimum amount of 1,000.
- View in detail 06/25 bills
- There are two bills, one for INTEREST and the other for ACCOUNT.
- Interest Bill: Although minimum amount of 500 was defined for interest, the billing has happened only for the actual accrued amount. This is because, there was no account Property defined for the bill type.
- Account bill: The calculated amount is less than the minimum amount of 1,000 and hence the bill is made due for a 1,000.


##### Fixed Equal Repayment

For the loan arrangements with Fixed Equal Payments(FEP), a Minimum Invoice Component (MIC) can be configured at the Product definition level or at the arrangement level. At the loan agreement stage, it is possible to indicate that though loan is of FEP type, certain mandatory component(s) (such as interest and charges) are invoiced fully.

MIC is used to define the components that are to be invoiced fully. The Account Property cannot be defined as an MIC. The Interest Property can be defined as an MIC. When the charge is part of the FEP amount, but interest alone is defined in MIC, an override is raised.

- When the FEP amount is less than the total MIC amount (sum of the Property amounts defined in MIC), the total MIC amount is billed.
- When the FEP amount is more than the total MIC amount (sum of the Property amounts defined in MIC), the FEP amount is billed. For example, Interest component is alone specified as MIC component.
- When the FEP amount is less than the accrued interest, the accrued interest is billed.
- When the FEP amount is greater than the accrued interest, the original FEP amount is billed.

If FEP is unable to cover the components in the Payment Schedule, then the order of invoicing is charge, interest and principal.

- Any charge amount that cannot be billed, is foregone if the charge is not part of MIC.
- Any interest amount that is accrued but not billed, gets carried forward to the next period.

In certain activities, recalculate options affect FEP schedules as follows:

The term is calculated based on the FEP amount. If the term cannot be calculated, then it is updated as blank resulting in the contract becoming a call contract.

> **⚠️ Note:** Every time term is recalculated, the system calculates the annuity amount, if available, is cleared.

Annuity amount is calculated. If Term is not available, it raises an error.

Residual amount is calculated using the FEP amount defined in the Actual Amount attribute and current term. If Term is not available, an error pop ups.

For a Product with Maximum Term Cap defined, when the term is recalculated based on the FEP amount captured or it breaches the cap, the system caps maturity date to the maximum term and calculates the annuity amount. The annuity amount gets updated.

Even if the term cannot be calculated, the system caps the maturity date to the maximum term and calculates the annuity amount.


##### Recalculation on Arrangements with Forward Dated Conditions

When there are forward dated conditions in a loan contract and the user triggers an activity such as prepayment or disbursement or change in the interest and so on, the system allows the recalculation of ‘Term’ or ‘Payment’ or ‘Maturity then payment’ based on the setup in the Recalculate attribute of the Payment Schedule condition.

| Column 1 | Column 2 |
|---|---|
| Loan Details |  |
| Created on | Jul 10, 2020 |
| Amount | 36,000 |
| Term | 3Y |
| Payment | Monthly |
| Interest Rate |  |
| Jul 10, 2020 to Jul 9, 2021 | 2% |
| Jul 10, 2021 to Jul 10, 2023 | 3% (variable rate) |
| Payment Amount |  |
| For the first year | 1000 |
| From the second year, until maturity | 1100 |

| Column 1 | Column 2 |
|---|---|
| Loan Details |  |
| Created on | Apr 1, 2022 |
| Term Amount |  |
| Amount | USD 100,000 |
| Maturity date | May 1, 2023 |
| Cap on the maturity date | 2 years (that is, it cannot exceed beyond April 1, 2024). |
| Payment Schedule |  |
| Payment | Monthly |
| Payment amount | USD 8149.33 |
| The disbursement, change schedule, apply rate and change interest activities are set to recalculate the “Maturity then payment” in the payment schedule condition. |  |
| Interest Rate |  |
| Apr 1, 2022 to May 1, 2023 | 10% |
| Day basis | E |


##### Zero Payment

During zero payment, either the payment frequency can be skipped of the end date mentioned in the End Date field or date in the Start Date field can be defined for skipping interim payments. In both the cases, the system calculates the amount in the Calc Amount field after considering the skipped installments (zero payments).

For an Annuity arrangement having a payment term of one year, if two regular payments are skipped in the middle of the payment period, the system calculates the payment amount for the remaining 10 payments considering the two zero payments and calculation logic equates the payment amount for the arrangement.

In the following example, payments are skipped on 6th, 7th, 9th and 11th month. However, the system projects the schedule for the arrangement by adjusting the skipped installment amounts for the rest of the payment period using its calculation logic. The below screen shot displays the AA.PRD.DES.PAYMENT.SCHEDULE record. The below screen shot displays the Enquiry schedule projection Disbursement Linked Payments When a loan product has to collect principal (down) payments along with disbursement, it can be set-up using the DISBURSEMENT relative date option and a TRANSACTION based Payment type. The consumer loan product in model bank illustrates this set-up where a downpayment of 25% is collected for each disbursement and the rest of the payments are collected on 30, 60 & 90th day. Case 1: Downpayment with Automatic Full Disbursement An arrangement is created for USD 1000 and is fully disbursed (automatically) The disbursement fee is calculated on each disbursement and is capitalised. 20% for loans upto 500 16% for loans above 500 but less than1000 8% for loans above 1000 25% of the disbursed amount plus the charge is collected as downpayment and is billed online. The net CUR account movement is 1160 25% of the movement ,that is, 290 is calculated as a payment bill and is raised along with this disbursement. Case 2: Downpayment with Partial Disbursement An arrangement created for USD 5000 The disbursement fee is calculated on each disbursement and is capitalised. 20% for loans upto 500 16% for loans above 500 but less than1000 8% for loans above 1000 25% of the disbursed amount plus the charge is collected as downpayment and is billed online. The disbursements are done manually First Disbursement for 3000 Net movement in CUR balance is 3,240 25% of the movement, that is, 810 is calculated as a payment bill and is raised along with this disbursement. Second and final disbursement for 2000 New movement in CUR balance is 2160 25% of the movement, that is, 540 is calculated as a payment bill and is raised along with the second disbursement.


##### Progressive Payments

The repayment amount in the Calc Amount field can be recalculated upon every repayment. The PROGRESSIVE.PAYMENT value in the Recalculate attribute increments the Calc Amount by the progressive percentage. The On Activity attribute in the Payment Schedule should include the LENDING-MAKEDUE-PAYMENT.SCHEDULE Activity to recalculate the PROGRESSIVE.PAYMENT.

In the example AA.ARR.PAYMENT.SCHEDULE , the Payment Freq attribute is set to 1M and the rate is 2%. This results in the amount calculated each month to increase by 2% every month.

The below ENQ AA.SCHEDULES.FULL enquiry shows the calculated amount for future payments for the above arrangement. This has been increased every month. Percentage Calculation for Principal-only Payments The total granted loan amount can be linearly distributed as Principal-only repayment for the percentage defined for the amortisation period as per the repayment frequency. When a percentage is defined in the Max Percentage attribute, the repayment percentage of original loan principal definition is restricted to maximum of percentage defined. Amortisation Schedule is 100% but the calculation percentage is restricted to the defined percentage. For example, if loan offered to customer was an Interest Subsidy loan, then it is convenient to collect the Principal-only repayments. Illustration Consider the following example. Loan Amount = USD 100,000 on 17 April 2020 Term = 1year Payments = Principal-only CALC Type = Percentage Repayment Frequency = Monthly Max Percentage = 100 Amortisation Schedule is as follows: 15% of 100,000 on the first three payments - 15,000 / 3 = 5000 20% of 100,000 on the next three - 20,000 / 3 = 6666.67 25% of 100,000 on the next three - 25,000/3 = 8333.33 40% of 100,000 on the last three - 40,000 / 3 = 13,333.33 Amortization date Total amount per period Repayment Percentage of original loan principal, % per period 17 May 2020 15000 15 17 June 2020 17 July 2020 17 Aug 2020 20000 20 17 Sep 2020 17 Oct 2020 17 Nov 2020 25000 25 17 Dec 2020 17 Jan 2021 17 Feb 2021 40000 40 17 Mar 2021 17 Apr 2021 The above amortisation conditions can be defined as follows in Payment Schedule product conditions. The payment amount calculation is always based on the outstanding balance and the remaining total percentage. Overriding the Capitalisation Amount The capitalisation process can make an account overdrawn, but such a scenario can optionally be restricted to the extent of available balance on the account. However, this functionality cannot be extended to user-defined checks, for example, a minimum amount definition that might be required for the customer for his living, like a sustenance amount. The system considers the entire available balance during capitalisation. In order to overcome this, an option is provided to validate any other user defined conditions that might be required during capitalisation. During capitalisation of bills, the system validates if the payment type is set as Cap and Inv Alt Payment Method and a user routine is attached in Alt Payment Routine . When both these conditions are satisfied, the available balance and the capitalisation amount are handed over by the core routine to the user attached API. The API further validates and decides if the bill should be capitalised or invoiced. Illustration Consider the pre-conditions listed above are met. A customer has a credit balance of Rs 5000. There is a user definition to have a balance Rs 7000 and above for his sustenance. A debit interest bill is processed for Rs 500. In the above scenario since the sustenance balance is greater than the available balance, the entire billed amount is moved to Inv.


##### Defining Future Conditions at the Arrangement Level

The Type field with FORWARD.DATED value in the AA.PROPERTY.CLASS record allows the user to introduce a new definition at the arrangement level, it will be dated. Once captured with a future date, the system automatically schedules this and during close of business the Scheduled Activity is processed by applying the new condition to the arrangement.

A Show tabs for expansion icon is provided in the tool bar of AA.ARRANGEMENT.ACTIVITY and AA.SIMULATION.CAPTURE screens. It helps the user to identify the property for which the future dated condition can be added.

Future dated condition can either be given by specifying the date of required change or by specifying relative date like ARRANGEMENT / START + 1 month.

1. Click the Show tabs for expansion icon in the tool bar. The Show tabs for expansion icon is disabled after displaying Current tab for the property to which Future Date Conditions are allowed.
2. Click Expand icon from Current tab to add Future Date Conditions. An Option for selecting Fixed Date and Relative Date pops up on the screen.
3. Select month and year for Fixed Date and Arrangement or Start date, offset by day(s), week(s), month(s) and year(s) for Relative Date.
4. Click to confirm the selection. The selected options will be displayed as the description of the Future Date Conditions tab.

> **⚠️ Note:** Multi-Tabs added to a FORWARD.DATE set AA property can be displayed. But there is no option of hiding the Future Date Conditions Tabs.


##### Additional Payments

Additional scheduled payments can be included in the PAYMENT.SCHEDULE Property. Additional payment is defined as the payment scheduled over and above the regular payments.

Additional payments can be given by adding a payment type, and it can be either ad hoc (single) or regular and the amount should be specified in the Actual Amt attribute. The system calculates the Calc Amount field taking into account the additional payment(s) specified.

It is possible to have

- Regular additional payment- An additional payment amount is specified on a recurring basis, such as annually. This amount applies over and above the regular installment amount.
- Regular special payment - An actual payment amount is specified for a regular installment. This amount replaces the regular installment amount.
- The additional amount is paid over and above the normal loan installment. When an additional amount is set in a repayment schedule, the remaining instalments are automatically calculated by the system.
- These payments can be in the middle of an Annuity schedule, or a Single Line Amortisation (SLA) schedule (equivalent to Linear payment type). When the payments are added to such a schedule, the payment amount is calculated to take into account the additional payment(s). The below screen shot displays the AA.PRD.DES.PAYMENT.SCHEDULE . The below screen shot displays additional payments every 3 months in the Payment Schedule.


##### Special Payments

Special payment is the actual amount specified by the user to substitute the regular installment amount for the specific period, either single or regular. This amount has to be specified in the Actual Amt attribute. In the example below, it is possible to schedule the Actual Amt for the specified periods, which substitutes the system Calc Amount . In this case, the system calculates the Calc Amount considering the user scheduled Actual Amt .

The below screen shot displays the AA.PRD.DES.PAYMENT.SCHEDULE record.


##### Deferred Payments

The Defer Period attribute in the Payment Schedule Property Class is used to define deferred payments. It defines how long the scheduled payment should be deferred from original cycled date.

- Date Convention - Forward
- Date Adjustment - Period
- Bill is raised on 2nd Feb with Payment Date as 2nd Feb, Actual Pay Date as 1st Feb, Financial Date as 2nd Feb and Defer Date as 8th Feb.
- Defer Date is calculated as 5 days from Actual Pay Date , which is 6th Feb. As it is holiday, the system again applies Date Convention on top of this date. Hence, the value of Defer date in this case is 8th Feb.
- For Defer Activity (processed on 2nd Feb), accounting entries are raised with Value date as Financial Date.
- The MAKEDUE or CAPITALISE Activity is processed on the Defer Date, which is 8th Feb. Here, the accounting entries are moved to nullify DEF entries and raise real statement entries.

- Date Convention - Forward
- Date Adjustment - Value
- Bill is raised on 2nd Feb with Payment Date as 2nd Feb, Actual Pay Date as 1st Feb, Financial Date as 2nd Feb and Defer Date as 8th Feb.
- Defer Date is calculated as 5 days from Actual Pay Date, which is 6th Feb. As it is holiday, it will again apply Date Convention on top of this date. Hence, Defer date in this case is 8th Feb.
- For Defer Activity (processed on 2nd Feb), accounting entries will be raised with Value date as Financial Date.
- The MAKEDUE or CAPITALISE Activity is processed on the Defer Date which is 8th Feb. Here, accounting entries will be moved to nullify DEF entries and raise real statement entries.


##### Installment Amount for Multiple Disbursement

Loans can have the calculated installment amount as a constant (same) amount based on the full principal amount and the accrued interest on the outstanding principal balance. This constant installment amount is the same amount from the first to the final installment amount as per the payment schedule. The Include Future Disb (INCLUDE.PRIN.AMOUNTS) field is set to Yes only when the installment amount is required to be constant from start date until the maturity date of the contract. Any principal disbursement or repayment scheduled in the future is taken into consideration for the calculation of installment.

Given below is an illustration of the loan that has scheduled disbursements with loan installments set for annuity repayment. Here the user has opted for installment calculations to consider future disbursements.

The schedules are built considering the future disbursements as well.

In the below illustration, the scheduled disbursement is planned, but the total outstanding is repaid before the second disbursement. Hence the second installment is a reduced amount to repay the outstanding and third installments is zero. Regular repayments start after the next disbursement is carried out.

When the flag for considering future disbursements is set, the system adjusts the installment amount automatically during loan life cycle stages. For example, change in disbursement dates, disbursement amount or disbursement percentage, interest rate revisions, maturity date change, payment holiday, change in schedules, prepayments, special payments, special schedules like interest only or principal only, tax or charge included installments, capitalisation of dues during overdue, charge-off, write-off.

During the loan takeover from legacy system, the users set this field as yes to calculate the installment amount considering the future disbursements.


##### Residual Principal in Payment Schedule

The residual amount can be set over the life of a loan contract. When set, it is included in the Principal component of the last installment and the Total Due amount is also adjusted to reflect the residual amount along with other scheduled payments.

The schedule projector includes the residual amount against the Total Due and Principal components and the payment schedule enquiry displays the details of each component.

Consider a loan contract with residual amount ($20000) setup. The effective date of the loan is 17-Apr-2019 and the maturity date is 17-Apr-2020.

The Payment Schedule projector is updated with the residual amount against the last installment and it is included in the Total Due amount as well as the Principal component of the installment.

The drill down on the installment detail shows the break-up of the Total Due amount and it includes the residual amount as a separate line item. Further, as the Principal component also includes the residual amount, the same is seen as a separate entry against the Account Property as shown below.

Read the Payment Schedule Property Class for information on the Residual Amount attribute.


##### Adjust Balance for Upfront Profit

For a finance in which upfront profit is collected, when the customer indicates his inability to repay a loan, the user can adjust the balance and recalculate the upfront profit using the LENDING-RESTRUCUTRE-BALANCE.MAINTENANCE Activity Class. The system raises the accounting entries and updates the interest files. The system recalculates the profit after the restructure. This functionality is currently limited to Account and Interest (upfront profit) Property Class alone.

| Event | Balance type | ECB amount |
|---|---|---|
| Disbursement | RECINTEREST | -$713.61 |
|  | ACCINTEREST | $713.61 |
| During Issue Bill | RECINTEREST | -$654.31 |
|  | ACCINTEREST | $654.31 |
|  | DUEINTEREST | $59.3 |
| Restructure activity - New outstanding amount is $20 instead of $59.3 | RECINTEREST | -$693.61 |
|  | ACCINTEREST | $693.61 |
|  | DUEINTEREST | $20 |


##### Partial Capitalisation of Interest Accruals

In an interest bearing arrangement with Annuity payment type, with Due and Cap setup, the actual amount indicated in the Payment Schedule is only made due and any remaining interest accruals is capitalised. This can be a partial or full capitalisation of interest accrual for that period.

For this kind of repayment patterns, The Alt Payment Method field in AA.PAYMENT.TYPE should be set as Due and Cap. In such Payment Types, in the Payment Schedule, the Payment Method should be set as Due and an Actual Amt can be specified. This Actual Amt is made due on the schedule date.

- When the Actual Amt is zero, all the accruals for that period is capitalised.
- When the Actual Amt is more than zero, that amount is made due and any remaining accruals for that period is automatically capitalised due to the principal.

Two separate bills are raised when the accruals are made due and capitalised. The Actual Amt mentioned is made due and follows the overdue cycle for non-repayments. The remaining accruals are capitalised and a capitalised bill is raised for this part.

When the system automatically calculates the instalment amount by itself, a separate set of associated multi-value fields should be defined with the same Payment Type and the Actual Amt should be left blank.


###### Illustration of a Mortgage Loan

In this illustration, there is a mortgage loan with the first two instalments as full capitalisation ( Actual Amt is 0), the next two instalments make the amount as 100 and remaining is capitalised ( Actual Amt is 100).

For this arrangement, there is a schedule built and the interest component with tax is fully capitalised for the first two schedules. The next two schedules have partial capitalisation. The amount 100, mentioned in the Payment Schedule is made due for interest accruals and the corresponding tax is also made due. The remaining accruals for the period and their respective tax component is capitalised to the principal of the arrangement.

When the Payment Type has Tax Inclusive set to No, the tax component is not included in the amount.

Separate bills are raised for the capitalised and the due component of the instalment. The capitalisation component is immediately settled and the actual amount component is made due. The actual amount component is made due for the instalment amount and If the instalment bill is not settled, this instalment bill undergoes ageing based on the overdue configuration

This arrangement also has fully capitalised interest for the first two schedules. The next two schedules have partial capitalisation. In this Payment Type, the Tax Inclusive attribute is set as Yes.

The Payment Schedule is shown below:

When the Payment Type has Tax Inclusive set to Yes, the actual amount mentioned is inclusive of tax as seen below:


##### Assigning Default Values to Payment Schedule Conditions

It is possible to pre-construct the schedule configurations and set defaults in the Payment Schedule conditions of the arrangement. Banks can offer a unique amortisation plan to customers to repay a specific different percentage of the principal-only repayment over a certain period, for the granted loan amount. This could be tedious to define it every time at the arrangement creation. The option of setting default values to Payment Schedule feature minimises the overwhelming operations maintenance overhead when a unique percentage has to be populated for arrangements without having to repeat them for every arrangement.

Consider the following example. Create an AA.PAYMENT.TYPE record called AMORT.PLAN.3 for a Personal Loan product as follows.

A new arrangement is created and the above configured AMORT.PLAN.3 is chosen for Payment Type for Schedule conditions.

The amortisation plan configured in the AA.PAYMENT.TYPE is assigned as default to the respective attributes in the Schedule conditions using an API at validate .


> **Related Applications:** `AA.ARR.PAYMENT.SCHEDULE`, `AA.ARRANGEMENT.ACTIVITY`, `AA.BILL.DETAILS`, `AA.INTEREST.ACCRUALS`, `AA.PAYMENT.TYPE`, `AA.PRD.DES.PAYMENT.SCHEDULE`, `AA.PROPERTY.CLASS`, `AA.SIMULATION.CAPTURE`, `EB.CONTRACT`

---


### 2.30  Weighted Average Rate


> **📇 Quick Reference Card**
> 
> **Purpose:** *When loans are being disbursed in multiple tranches, each having its own interest rate a Weighted Average Rate (WAR) for the arrangement has to be calculated and applied to the contract after each disbursement .*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

When loans are being disbursed in multiple tranches, each having its own interest rate a Weighted Average Rate (WAR) for the arrangement has to be calculated and applied to the contract after each disbursement .

A weighted average interest rate is an average that is adjusted to reflect the contribution of each loan to the total debt. The weighted average multiplies each loan’s disbursement interest rate by the loan balance and divides the sum by the total loan balance. Each loan’s disbursement interest rate contributes to the weighted average in proportion to the loan’s percentage of the total debt.

The Weighted Average Rate Type of Interest condition enables the calculation of the weighted average rate, which determines the actual effective rate of the arrangement.

---


### 2.31  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Transaction Recycler provides the ability to retry failed financial transactions again at regular intervals. This is a generic retry mechanism which can be consumed by any Temenos Transact application. The Transaction Recycler is available for Arrangement Architecture (AA) and Interest and Charg...*
> 
> **Applications:** `AA.PARAMETER`, `MS.PARAMETER`, `RC.CONTRACT.PRIORITY`
> 
> **Key Fields:** *Aa Product*, *Aa Product Group*, *Attribute Type*, *Attribute Value*, *Create Retry Trigger*, *Custom Priority Rank*, *Date Convention*, *Def Prev Settle* ... +33 more
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- Temenos Transact Services

The Transaction Recycler provides the ability to retry failed financial transactions again at regular intervals. This is a generic retry mechanism which can be consumed by any Temenos Transact application. The Transaction Recycler is available for Arrangement Architecture (AA) and Interest and Charged (IC) modules (R13 release and above). Read Transaction Cycler section under Settlement Property Class for more information related to Arrangement Architecture.

The Transaction Recycler service handles the retry of failed transactions. This service will run as a COB job at a specific stage during both End of Day (EOD) and online phases. This job will retry the transactions on scheduled dates until the transaction is settled or number of retry attempts allowed have been exhausted or retry end date is reached.

During each retry, the Transaction Recycler will take the amount available in the settlement account for settling the transaction amount in full or partial, based on the Transaction Recycler retry configuration. The RC can retry the settlement based on pre-defined priority order as defined by the bank. In case of an AA loan repayment, the RC.CONTRACT.PRIORITY application allows the user to define sorting priority criteria based on custom values - the bill type or the aging status of bill.

The transactions handed over to Recycler (RC), if settled outside the RC framework are not excluded from further processing by RC and is marked with a specific status.

The following chart shows the transaction recycler process:

The Transaction Recycler acts as a framework and the processing required for retrying an AA payment or IC charges is built as a plug-in. In the above flow chart, the core plug-ins are generally represented as the payment processor, and the RC processes further, when there is an AA payment or an IC payment pending. The Transaction Recycler recognises that two different types of payments should be processed and the respective payment processor invoked is parameterised. This design enables the addition of new activity types (including any client-specific local activities) to be retried while using the same Transaction Recycler framework to orchestrate the recycling.


##### Product Configuration

The following chart shows the Transaction Recycler module components:

| Core Routine Fields | Description | Routine Name |
|---|---|---|
| Pre processor | Used to define whether a message specific core routine needs to be called to pre-process a message. | RC.PREP.RC.TYPE – For example, RC.PREP.IC.CHARGE |
| Prioritise | Used to define the message-specific core routine called by the Transaction Recycler to perform transaction grouping and sorting. | RC.PRTY.RC.TYPE – For example, RC.PRTY.IC.CHARGE |
| Processor | Used to define the message-specific core routine called by the Transaction Recycler to process the Transaction Recycler transaction, or transactions if they are grouped. | RC.PROC.RC.TYPE – For example, RC.PROCE.IC.CHARGE |
| Post process | Defines the message-specific API routine called by the Transaction Recycler to perform processing after the transaction has been completed. | RC.POST.RC.TYPE – For example, RC.POST.IC.CHARGE |

The RC.PRIORITY application is a highest level prioritisation parameter that allows to setup priority of transactions at the company level by EB.SYSTEM.ID or AA.PRODUCT.GROUP . This application is used in conjunction with RC.PRODUCT.PRIORITY and RC.CONTRACT.PRIORITY to create the rules regarding which type of transaction takes priority when there is more than one outstanding transaction against a settlement account. It ranks by EB.SYSTEM.ID , by AA.PRODUCT.GROUP or by a custom RC.PRODUCT.PRIORITY record and the ID to this application can be either a master or a lead company.

In the RC.PRIORITY application, the order of priorities are defined in the descending order (for example, the first definition has the highest priority and so on).

- In the above screenshot, the system is set up to consider the transactions in the following order, if multiple retry requests are posted against the same account:First: Products defined in the RC.PRODUCT.PRIORITY application in the PRIORITY+ONE record (direct debits sent by TPH with transaction code 125).

- Second: Products defined in the RC.PRODUCT.PRIORITY application in the MORTAGES record (MORTGAGE AA Product and then MORTGAGE.CASHBACK AA Product).

- Third: Products defined in the RC.PRODUCT.PRIORITY application in the PRIORITY +TPH record (direct debits sent by TPH with transaction code 213).

- Fourth: Request posted by the PAYMENT.ORDER application, irrespective of the request type.

When using as a priority, either a System ID (an EB.SYSTEM.ID record), the system does not require a correspondent RC.PRODUCT.PRIORITY record. If the RC.PRODUCT.PRIORITY record is not defined, it will process all retry transaction requests posted by the application in a default order, considering the oldest one received by the recycler first.

> **⚠️ Note:** The system allows only one option for each priority to be entered. This can either be an EB.SYSTEM.ID, an AA.PRODUCT.GROUP or a Product Priority (custom RC.PRODUCT.PRIORITY ID ).

Def Prev Settle is a filtering rule that means if, out of a list of ‘n’ pending transactions, one of transactions could not be settled (during retry), then all subsequent pending transactions in that list will be abandoned. It could be set to either Yes or No or left blank. If selected, it is applicable for EB.SYSTEM.ID , AA.PRODUCT.GROUP or Product Priority. This field is mutually exclusive with Prev Settle field.

The Prev Settle field can be set as Yes or No. If set to Yes, during retry of ‘n’ transactions, all transactions must be settled. Even if one of the transactions fail for some reason, then none of the remaining transactions will be considered for settlement.

The RC.CONTRACT.PRIORITY application is used in conjunction with RC.PRIORITY and RC.PRODUCT.PRIORITY to create the rules regarding the type of transaction that takes priority when there is more than one outstanding transaction against a settlement account. The RC.CONTRACT.PRIORITY is used to set the ranks at transaction level for the same type of retry request. It is used to set priority by value date, transaction amount or by a custom setting, for example by bills overdue status sent to Recycler by Arrangement Architecture (AA).

For example, if there are several transactions for the same product type against the settlement account, then the transactions have to be prioritised.

- The oldest transactions are processed first.
- If there are more than one transaction due for the same date and type, then prioritise by the largest amount first.

The RC.CONTRACT.PRIORITY application allows the user to define sorting priority criteria based on custom values. For example, based on the bills’ status issued by AA in case of loans repayments. To perform this, set:

- Due Type - Sort By Priority Attribute
- Due Rule - Custom

The Priority Rank Type field in RC.CONTRACT.PRIORITY accepts the following three options:

- Aging Status - Enables prioritisation based on the aging status of bills generated for each arrangement.
- Bill Type - Enables prioritisation of bill ( RC.DETAIL ) records based on the bill type of the arrangements.
- Blank – The value is used if the prioritization is by Aging Status of the bills.

It is not possible to set the prioritization by both Aging Status /Blank and Bill Type in the same record.

The multi-valued Custom Priority Rank field must contain custom values in the order which they must be sorted. Based on the Custom Priority Rank the Custom Priority Rank field must contain valid EB.LOOKUP record values from AA.OVERDUE.STATUS or from AA.BILL.TYPE .

In the example below, the custom values represent the overdue bill’s status based on aging / bill type as they are sent by AA to Recycler, to process the retry requests.

> **⚠️ Note:** It is not possible to set the prioritization by both Aging Status / Blank and Bill Type in the same record.

The overdue status is shown in the RC.DETAIL record after the request is settled.

> **⚠️ Note:** The AA Payment Rules setup must be in sync with the setup done in the Recycler priority setup tables. For example, if the oldest bill setup is done in AA Payment Rules, the same setup must be done in the recycler.

For example, if the Payment Rules are setup to consider the oldest bill first for an AA Product, and for the same AA Product, the contract priority rule is setup to consider the largest amount first (different setup than in Payment Rules), the system works as follows:

- If two bills are issued for the same contract on the same date, the system settles the bills by date (oldest one first) ignoring the ‘By amount’ setup in the recycler.
- If two bills are issued for the same contract on different dates, the system settles the bills considering the ‘By amount’ setup in the recycler.
- If two bills are issued for different contracts on different dates, the system settles the bills considering the ‘By amount’ setup in the recycler.
- If two bills are issued for different contracts on the same date, the system settles the bills by date (oldest one first) ignoring the ‘By amount’ setup in the recycler.

The user can define product priorities based on contract custom criteria using the RC.PRODUCT.PRIORITY application. If the user wants to define such priority, the Rank Based Priority field must be defined with the RC.CONTRACT.PRIORITY custom name. If this is set, the order defined in RC.CONTRACT.PRIORITY is applied to all products setup in RC.PRODUCT.PRIORITY . For example, it is possible to define custom priority criteria based on bills overdue status and based on product type. The bills overdue status should be setup first in the RC.CONTRACT.PRIORITY application as a custom record (read the RC.CONTRACT.PRIORITY for more details).

In order to sort the retry request based on the setup in RC.CONTRACT.PRIORITY and the one in the product order defined in RC.PRODUCT.PRIORITY , Priority Execution field must be defined. The values in this field are ’Rank Then Product’ and ’Product Then Rank’.

If the value ’Rank Then Product’ is selected, if more than one retry request is posted against the same account, the system orders requests based on the rank (status) defined in RC.CONTRACT.PRIORITY first and then by the product as defined in RC.CONTRACT.PRIORITY . If the value ’Product Then Rank’ is selected, the system orders the requests by product first and then by their rank from the RC.CONTRACT.PRIORITY application.

The following screenshot shows the RC.PRODUCT.PRIORITY is created with the value ’Rank Then Product’.

The RC.CONTRACT.PRIORITY custom record ‘MORTGAGELOANS’ has the setup as shown in the below screenshot.

The RC.PRODUCT.PRIORITY record is setup to order the requests according to the rank (status) first and then according to the product order (MORTGAGE.LOANS.USD and then MORTGAGE.LOANS.1Y), if more than one request has the same rank (status).

In case the RC.PRODUCT.PRIORITY record has a custom ID and if the Priority Execution field is defined with the value ’Rank Then Product’, the Aa Product Group field will become multivalued, allowing the definition of priorities based on products which are part of different AA PRODUCT GROUPS in the same record.

The input of Aa Product Group field is mandatory in case any Aa Product are defined. The Aa Product definition is not mandatory if the Aa Product Group is entered. If only the Aa Product Group is defined, the system considers all the retry requests posted by any product type within the product group and orders them by date (the oldest one is considered first). It is not possible to define a duplicate combination of Aa Product Group and Aa Product of the same type in the same record.

The online recycler checks for the following:

- New triggers on the accounts with active retry requests.
- Retry request for which the cut off time has passed.

The RC.PARAMETER application controls the retry trigger and the Create Retry Trigger field can have one of the following options:

- Any Credit – The system creates a retry trigger ( RC.RETRY.TRIGGER table application) for any credit posted on the account.
- Credit Balance – The system creates a retry trigger only if the new credit makes the account balance positive.

In the OVERRIDE record, ACCT.UNAUTH.OD, the Susp Appln field and Fwd Acct Mode should to be configured, as shown in the example below:

| Scenario 1 Schedule Initiation on Holiday parameter is configured | Scenario 2 Schedule Initiation on Holiday parameter is not configured |
|---|---|
| Transaction Recycler retries the transaction to settle the bill. System checks the value date when the settlement account received the funds. As it is backdated, RC settles the bill with value date on Saturday. Penalty interest accrued for Saturday and Sunday is reversed, and only one day of penalty interest is applied to the contract. Bill is settled & Contract status = Current, as of Saturday. | Transaction Recycler retries the transaction to settle the bill. System checks the value date when the settlement account received the funds. As it is backdated, RC settles the bill with the value date on Saturday. Age Overdue activity is reversed and not replayed. Total amount for which the customer is charged = Instalment amount + One day’s penalty. Due to the reversal of the ageing activities, the penalty interest is posted to UNC/remainder activity. |


##### Business Events

When the Emit Business Event field in MS.PARAMETER is set as ‘Yes’, the business events representing the state change are emitted.

The following business events are emitted for Transaction Recycler.

| Business Event | Description |
|---|---|
| settlementService.transactionRetry.currentRetry | Event to be emitted when the transaction retry is moved to current status |
| settlementService.transactionRetry.fundRecovered | Event to be emitted for a transaction retry when the funds are recovered successfully |
| settlementService.transactionRetry.fundReserved | Event to be emitted for a transaction retry when the funds are reserved successfully |
| settlementService.transactionRetry.manuallyApproved | Event to be emitted when a transaction is manually approved |
| settlementService.transactionRetry.retryCancelled | Event to be emitted when the transaction retry is cancelled |
| settlementService.transactionRetry.retryCompleted | Event to be emitted when the transaction retry is completed |
| settlementService.transactionRetry.retryCreated | Event to be emitted when the transaction retry is created |


> **Related Applications:** `AA.PARAMETER`, `MS.PARAMETER`, `RC.CONTRACT.PRIORITY`

---


---


## Appendix A: Glossary of T24 Applications & Fields


This glossary lists all T24/Transact application names and field names referenced throughout this document, with descriptions where available.


### Applications


| Application | Description |
|------------|-------------|
| `AA.ACCOUNT.DETAILS` | T24 application: AA.ACCOUNT.DETAILS |
| `AA.ACCRUAL.FREQUENCY` | T24 application: AA.ACCRUAL.FREQUENCY |
| `AA.ACTIVITY` | T24 application: AA.ACTIVITY |
| `AA.ACTIVITY.CLASS` | T24 application: AA.ACTIVITY.CLASS |
| `AA.ACTIVITY.HISTORY` | T24 application: AA.ACTIVITY.HISTORY |
| `AA.ARR.PAYMENT.SCHEDULE` | T24 application: AA.ARR.PAYMENT.SCHEDULE |
| `AA.ARR.XIS.DRAWING` | T24 application: AA.ARR.XIS.DRAWING |
| `AA.ARR.XIS.FACILITY` | T24 application: AA.ARR.XIS.FACILITY |
| `AA.ARRANGEMENT` | T24 application: AA.ARRANGEMENT |
| `AA.ARRANGEMENT.ACTIVITY` | T24 application: AA.ARRANGEMENT.ACTIVITY |
| `AA.BILL.DETAILS` | T24 application: AA.BILL.DETAILS |
| `AA.CONTEXT TYPE` | T24 application: AA.CONTEXT TYPE |
| `AA.DECISION.PARAMETER` | T24 application: AA.DECISION.PARAMETER |
| `AA.INTEREST.ACCRUALS` | T24 application: AA.INTEREST.ACCRUALS |
| `AA.NEXT.ACTIVITY` | T24 application: AA.NEXT.ACTIVITY |
| `AA.PARAMETER` | T24 application: AA.PARAMETER |
| `AA.PAYMENT.TYPE` | T24 application: AA.PAYMENT.TYPE |
| `AA.PERIODIC.ATTRIBUTE` | T24 application: AA.PERIODIC.ATTRIBUTE |
| `AA.PRD.DES.PAYMENT.SCHEDULE` | T24 application: AA.PRD.DES.PAYMENT.SCHEDULE |
| `AA.PRD.DES.XIS.DRAWING` | T24 application: AA.PRD.DES.XIS.DRAWING |
| `AA.PRD.DES.XIS.FACILITY` | T24 application: AA.PRD.DES.XIS.FACILITY |
| `AA.PRODUCT.DESIGNER` | T24 application: AA.PRODUCT.DESIGNER |
| `AA.PRODUCT.GROUP` | T24 application: AA.PRODUCT.GROUP |
| `AA.PRODUCT.LINE` | T24 application: AA.PRODUCT.LINE |
| `AA.PROPERTY` | T24 application: AA.PROPERTY |
| `AA.PROPERTY.CLASS` | T24 application: AA.PROPERTY.CLASS |
| `AA.SCHEDULED.ACTIVITY` | T24 application: AA.SCHEDULED.ACTIVITY |
| `AA.SIMULATION.CAPTURE` | T24 application: AA.SIMULATION.CAPTURE |
| `AC.ALLOCATION.RULE` | T24 application: AC.ALLOCATION.RULE |
| `AC.ALLOCATION.RULES` | T24 application: AC.ALLOCATION.RULES |
| `AC.EVENT` | T24 application: AC.EVENT |
| `ACCOUNT` | T24 application: ACCOUNT |
| `ACCR.REV.PARAM` | T24 application: ACCR.REV.PARAM |
| `BASIC.INTEREST` | T24 application: BASIC.INTEREST |
| `CATEG.ENTRY` | T24 application: CATEG.ENTRY |
| `CATEGORY` | T24 application: CATEGORY |
| `CURRENCY` | T24 application: CURRENCY |
| `CURRENCY.MARKET` | T24 application: CURRENCY.MARKET |
| `CUSTOMER` | T24 application: CUSTOMER |
| `EB.ACCRUAL` | T24 application: EB.ACCRUAL |
| `EB.API` | T24 application: EB.API |
| `EB.CASHFLOW` | T24 application: EB.CASHFLOW |
| `EB.CONTEXT` | T24 application: EB.CONTEXT |
| `EB.CONTRACT` | T24 application: EB.CONTRACT |
| `EB.EVENTS` | T24 application: EB.EVENTS |
| `EB.LOOKUP` | T24 application: EB.LOOKUP |
| `EB.RULES` | T24 application: EB.RULES |
| `EB.RULES.VERSION` | T24 application: EB.RULES.VERSION |
| `EB.TABLE.DEFINITION` | T24 application: EB.TABLE.DEFINITION |
| `FUNDS.TRANSFER` | T24 application: FUNDS.TRANSFER |
| `ID.ACCOUNT.CONDITION` | T24 application: ID.ACCOUNT.CONDITION |
| `ID.CATEG.ENT.DETAILS` | T24 application: ID.CATEG.ENT.DETAILS |
| `ID.CATEG.ENT.UPDATE` | T24 application: ID.CATEG.ENT.UPDATE |
| `ID.CUSTOMER.PREFERENCES` | T24 application: ID.CUSTOMER.PREFERENCES |
| `ID.DEPOSIT.BALANCES` | T24 application: ID.DEPOSIT.BALANCES |
| `ID.PDS.ACTION` | T24 application: ID.PDS.ACTION |
| `ID.PDS.CATEGORY` | T24 application: ID.PDS.CATEGORY |
| `ID.PDS.WEIGHT` | T24 application: ID.PDS.WEIGHT |
| `ID.POOL.CONDITION` | T24 application: ID.POOL.CONDITION |
| `ID.POOL.PARAMETER` | T24 application: ID.POOL.PARAMETER |
| `ID.PRECLOSE.CUSTOMISE` | T24 application: ID.PRECLOSE.CUSTOMISE |
| `ID.SYSTEM.PARAMETER` | T24 application: ID.SYSTEM.PARAMETER |
| `INTEREST.BASIS` | T24 application: INTEREST.BASIS |
| `IS.ASSET` | T24 application: IS.ASSET |
| `IS.ASSET.REVIEW` | T24 application: IS.ASSET.REVIEW |
| `IS.BROKER` | T24 application: IS.BROKER |
| `IS.COMMODITY` | T24 application: IS.COMMODITY |
| `IS.COMMODITY.POSITION` | T24 application: IS.COMMODITY.POSITION |
| `IS.COMMODITY.SALE` | T24 application: IS.COMMODITY.SALE |
| `IS.CONTRACT` | T24 application: IS.CONTRACT |
| `IS.CONTRACT.DELIVERY` | T24 application: IS.CONTRACT.DELIVERY |
| `IS.CONTRACT.TASK` | T24 application: IS.CONTRACT.TASK |
| `IS.COST.PAYMENT.BALANCES` | T24 application: IS.COST.PAYMENT.BALANCES |
| `IS.COST.TYPE` | T24 application: IS.COST.TYPE |
| `IS.DOWN.PAYMENT.BALANCES` | T24 application: IS.DOWN.PAYMENT.BALANCES |
| `IS.EQUIPMENT` | T24 application: IS.EQUIPMENT |
| `IS.MISCASSET` | T24 application: IS.MISCASSET |
| `IS.MOVEQUIPMENT` | T24 application: IS.MOVEQUIPMENT |
| `IS.PARAMETER` | T24 application: IS.PARAMETER |
| `IS.PAYMENT` | T24 application: IS.PAYMENT |
| `IS.PAYMENT.DECLARATION` | T24 application: IS.PAYMENT.DECLARATION |
| `IS.PDS.WEIGHT` | T24 application: IS.PDS.WEIGHT |
| `IS.PP.STATUS.CODE` | T24 application: IS.PP.STATUS.CODE |
| `IS.REALESTATE` | T24 application: IS.REALESTATE |
| `IS.REVIEWER` | T24 application: IS.REVIEWER |
| `IS.REVIEWER.PAYMENT.BALANCES` | T24 application: IS.REVIEWER.PAYMENT.BALANCES |
| `IS.STATUS` | T24 application: IS.STATUS |
| `IS.VEHICLE` | T24 application: IS.VEHICLE |
| `IS.VENDOR` | T24 application: IS.VENDOR |
| `IS.VENDOR.PAYMENT BALANCES` | T24 application: IS.VENDOR.PAYMENT BALANCES |
| `IS.VENDOR.PAYMENT.BALANCES` | T24 application: IS.VENDOR.PAYMENT.BALANCES |
| `LD.LOANS.AND.DEPOSITS` | T24 application: LD.LOANS.AND.DEPOSITS |
| `LETTER.OF.CREDIT` | T24 application: LETTER.OF.CREDIT |
| `LIMIT` | T24 application: LIMIT |
| `LIMIT.REFERENCE` | T24 application: LIMIT.REFERENCE |
| `MM.MONEY.MARKET` | T24 application: MM.MONEY.MARKET |
| `MS.PARAMETER` | T24 application: MS.PARAMETER |
| `PAYMENT ORDER PRODUCT` | T24 application: PAYMENT ORDER PRODUCT |
| `PAYMENT.ORDER.PARAMETER` | T24 application: PAYMENT.ORDER.PARAMETER |
| `PAYMENT.ORDER.PRODUCT` | T24 application: PAYMENT.ORDER.PRODUCT |
| `PERIODIC.INTEREST` | T24 application: PERIODIC.INTEREST |
| `PERIODIC.RATE` | T24 application: PERIODIC.RATE |
| `POR.POSTING.REVERSAL` | T24 application: POR.POSTING.REVERSAL |
| `PP.MSGPAYMENTTYPE` | T24 application: PP.MSGPAYMENTTYPE |
| `PP.NODA.LIST` | T24 application: PP.NODA.LIST |
| `PP.SOURCE` | T24 application: PP.SOURCE |
| `PRODUCT.BUILDER` | T24 application: PRODUCT.BUILDER |
| `RC.CONTRACT.PRIORITY` | T24 application: RC.CONTRACT.PRIORITY |
| `RE.CONSOL.SPEC.ENTRY` | T24 application: RE.CONSOL.SPEC.ENTRY |
| `SEC.TRADE` | T24 application: SEC.TRADE |
| `TELLER` | T24 application: TELLER |
| `TSA.SERVICE` | T24 application: TSA.SERVICE |


### Fields Referenced


| Field | Field | Field |
|-------|-------|-------|
| `AA Bundle ID` | `AA Reference` | `AMC` |
| `Aa Product` | `Aa Product Group` | `Acc Difference Amount` |
| `Acc Difference Amt` | `Account` | `Account Cat` |
| `Account Seq` | `Accounting Mode` | `Accrual End Date` |
| `Accrual End Date` | `Accrual Rate` | `Accrual Start Date` |
| `Acct weightage` | `Action` | `Action Completed` |
| `Action Reference` | `Action Success` | `Active Y/N` |
| `Activity` | `Activity Link` | `Activity Type` |
| `Actual Amount` | `Actual Amt` | `Actual Pay Date` |
| `Actual profit amount` | `Addl Reserve Rtn` | `Addl reserve Rtn` |
| `Address` | `Advance Payment` | `Advance Payment Restriction` |
| `Advance Profit Accounting` | `Aging Status` | `Align Dates` |
| `Allow BIC` | `Allow Future Date` | `Allow IBAN` |
| `Allow Sort code` | `Allowed Product` | `Allowed Unit` |
| `Alt Acct Id` | `Alt Acct Type` | `Alt Id Type` |
| `Alt Payment Method` | `Alt Payment Routine` | `Alternate Id` |
| `Alternate Id Type` | `Amortisation Term` | `Amount` |
| `Amount From` | `Amount To` | `Amount from` |
| `Amount to` | `Appl Field Name` | `Application Method` |
| `Apply PDS Profit Rate` | `Apply as Tier Rate` | `Area` |
| `Arrangement` | `Arrangement Id` | `Arrangement Status` |
| `Asset Reference` | `Asset Delivery Tracking` | `Asset Description` |
| `Asset Reference` | `Asset Short Title` | `Asset Table` |
| `Asset Type` | `Asset Value by Appraiser` | `Attribute Type` |
| `Attribute Value` | `Auto Settle` | `Available Date` |
| `Back-to-Back FX` | `Back-to-back FX` | `Band or Level` |
| `Bank Share` | `Bank Share (Amount)` | `Base Ccy Product` |
| `Ben Bank` | `Ben Cust` | `Ben Customer` |
| `Ben. Acct. No` | `Ben. Cust` | `Beneficiary` |
| `Bill Produced` | `Bill Produced` | `Bill Status` |
| `Bill Type` | `Booking Date` | `Br Fee BS Acctg` |
| `Br Fee BS Cr Acct` | `Br Fee Currency` | `Br Fee Debit Type` |
| `Br Fee Pay Frequency` | `Br Fee Settlement` | `Br Fee Share Perc` |
| `Br Fee Tax Base Amt` | `Br Fee Type` | `Br Fee Wash Categ` |
| `Br Last Payment Date` | `Br Settle Wash Categ` | `Broker` |
| `Broker Account` | `Broker Acct` | `Broker Type` |
| `Builder Code` | `Builder Name` | `Bundle Arrangement` |
| `Buy Broker` | `Buy Broker Account` | `Buy Broker Acct` |
| `Buy Broker Wash Acct` | `Cal Routine` | `Calc Amount` |
| `Calc Balance Type` | `Calc Type` | `Calculation Routine` |
| `Calculation Type` | `CalculationType` | `Cash Dep Amt` |
| `Change Amount` | `Charge Off Amount` | `Charge Off Percentage` |
| `Charge off Amount` | `Charge off Percentage` | `Chassis No` |
| `Closure Reason` | `Color` | `Combine Bill At Parent` |
| `Comments abt Reviewer` | `Commitment Drawdown` | `Commitment Reversal` |
| `Commodity` | `Commodity Reference` | `Commodity Sale Ref` |
| `Commodity Sale Reference` | `Commodity Status` | `Company` |
| `Comparison Type` | `Conditions Evaluation Period` | `Context Name` |
| `Context Value` | `Context name` | `Contract Currency` |
| `Contract Reference` | `Contribution Amount` | `Contribution Counterparty` |
| `Contribution Type` | `Cooling Date Adj` | `Cooling Period` |
| `Cost Amount` | `Cost Counter Party` | `Cost Credit Account` |
| `Cost Debit Account` | `Cost Pay Type` | `Cost Payable Account` |
| `Cost Payment Type` | `Cost Reference` | `Cost Type` |
| `Counter Booking Account` | `Cr Counter Booking Activity` | `Create Retry Trigger` |
| `Credit Account` | `Credit Amount` | `Credit Currency` |
| `Credit Value Date` | `Credit value Date` | `Currency` |
| `Currency & Min Balance` | `Currency Market` | `Custom Priority Rank` |
| `Customer` | `Customer No` | `Customer Account` |
| `Customer Acct` | `Customer No` | `Customer Share` |
| `Customer Share (Amount)` | `Date Convention` | `Dealer Code` |
| `Dealer Name` | `Debit Account` | `Debit Currency` |
| `Debit Account` | `Debit Amount` | `Debit Currency` |
| `Debit Value Date` | `Decimal Qty` | `Decl Level` |
| `Decl level` | `Declaration At` | `Declared Profit Amt` |
| `Declared Profit Amt` | `Declared Profit Amt.` | `Def Account` |
| `Def Prev Settle` | `Default Attribute Option` | `Default Ol Accrual` |
| `Default Pool` | `Default Rebate Type` | `Default Rebate Value` |
| `Defer Date` | `Defer Period` | `Define Pool ID` |
| `Delivery Date` | `Delivery Quantity` | `Deposit Cat` |
| `Deposit Currency` | `Description` | `Description abt the Cost` |
| `Direct Pay Profit` | `Dist Balance Type` | `Distrib Freq` |
| `Down Payment Amount` | `Down Pay Asset ref` | `Down Pay Percentage` |
| `Down Payment Account` | `Down Payment Amount` | `Down Payment Commodity` |
| `Down Payment Rec Amount` | `Down Payment type` | `Dr Counter Booking Activity` |
| `Drawing ID` | `Drawings Arr Currency` | `Due Freq` |
| `Due Frequency` | `Due Rule` | `Due Type` |
| `EIR` | `Effective` | `Effective Date` |
| `Eligible Status for Finance` | `Emit Business Event` | `End Date` |
| `Enddate` | `Engine No` | `Engine Power (in CC)` |
| `Equipment Located at` | `Equipment Name` | `Equipment Type` |
| `Event Type` | `Exclude/Include Activity` | `Exclude/Include Indicator` |
| `Exclusion Evaluation Cycle` | `Expense Cat` | `Expense Product` |
| `Expense Product Cat` | `Expiry Days` | `Expiry date` |
| `Extend Cycle` | `External Posting` | `Field Name.1.1` |
| `Field Name.1.2` | `Field Name.1.3` | `Field Name.1.4` |
| `Field Name.1.5` | `Field Name.1.6` | `Field Operation` |
| `Field Operator` | `Field Value.1.1` | `Field Value.1.2` |
| `Field Value.1.3` | `Field Value.1.4` | `Field Value.1.5` |
| `Field Value.1.6` | `Finalise Bills` | `Finalise Bills` |
| `Finance Product` | `Financial Date` | `Fixed` |
| `Fixed Rate` | `Frequency` | `Full Chargeoff` |
| `Full Commitment Activity` | `Fwd Acct Mode` | `GB Asset Description` |
| `Generate Iban` | `Group Bill Type` | `Group Min Amount` |
| `Group Min Property` | `Hiba Pay Cat` | `Hol Restrict Item` |
| `Hol Restrict Type` | `I` | `ID` |
| `IS Contract Ref` | `IS Product` | `IS Product ID` |
| `IS Product` | `Id` | `In Adv` |
| `Inadv` | `Include All Payments` | `Include Future Disb` |
| `Income Cat` | `Income PL` | `Income Product` |
| `Income Product Cat` | `Initiation Type` | `Installments to Pay` |
| `Internal Limit` | `Internal Rebate PL Category` | `Investment Strategy` |
| `Invoice No` | `Irr Categ` | `Irr Percent` |
| `LCY Amount` | `Last Update Date` | `Legacy War Rate` |
| `Limit Reference` | `Limit Serial` | `Link AC Number` |
| `Link Account` | `Linked Ac Number` | `Linked Account Number` |
| `Loc Cap Chk Rtn` | `Loc Processor` | `Loc post process` |
| `Loc pre process` | `Loc prioritise` | `Loc processor` |
| `Location Of The Property` | `Make` | `Mandatory` |
| `Master Arrangement` | `Master Live Date` | `Maturity Date` |
| `Maturity Dist Adjust` | `Maturity date` | `Max Percentage` |
| `Maximum Amt.1` | `Maximum Term Cap` | `Method` |
| `Migration Mode` | `Min Balance Amount` | `Min Balance Evaluation Start Date` |
| `Min Dep Period` | `Min. Tfr Cr 1` | `Min. Tfr Dr 1’` |
| `Minimum Amt.1` | `Minimum Payment Type` | `Mode` |
| `Model` | `Modify/Cancel Payment Holidays` | `Move to History Days` |
| `Mud Share` | `Mudaraba Profit Share %` | `Mudarib Adjust Cat` |
| `Mudarib Fee Cat` | `Mudarib Profit Share %` | `Name` |
| `Narrative` | `Net Profit Recalc Rtn` | `New Activity` |
| `New Payment Amount` | `New Property Amount` | `No Activity Indicator` |
| `Notes` | `Nr Value` | `Nr Value Source` |
| `Number of Installments` | `Number of Instalments` | `Number of Payments` |
| `Number of Rooms` | `On Activity` | `On Activity, Recalculate` |
| `Online Retry Attempts` | `Optional` | `Or Prop Amt` |
| `Or Prop Amt Bnk` | `Ordering Customer` | `Orig Contract Date` |
| `Original Property Amount` | `Original profit amount` | `Origination Country` |
| `Os Prop Amt` | `Os Prop Amt Bnk` | `Oth Income Cat` |
| `Oth Acct Pct` | `Oth Exp Acct Pct` | `Oth Expense Acct` |
| `Oth Expense Cat` | `Oth Expense Pct` | `Oth Inc Acct Pct` |
| `Oth Income Acct` | `Oth Income Pct` | `PDS Category I` |
| `Parent Account` | `Participant Accounting Type` | `Pay Freq` |
| `Pay Through Beneficiary` | `Pay through beneficiary` | `Payment` |
| `Payment Amount` | `Payment Connection Method` | `Payment Currency` |
| `Payment Date` | `Payment Freq` | `Payment Method` |
| `Payment Mode` | `Payment Type` | `Payment amount` |
| `Payment type` | `Payoff Date` | `Pds Action Id` |
| `Per Categ` | `Per Percent` | `Percentage` |
| `Periodic Type` | `Place of EC Issue` | `Plot Id` |
| `Pool` | `Pool Id` | `Pool Objective` |
| `Pool Ref` | `Pool Sweep` | `Post process` |
| `Pr Value` | `Pre Cob Check` | `Pre Notice Activity` |
| `Pre Notice Days` | `Pre processor` | `Prev Settle` |
| `Prft Acctng Value Date` | `Principal` | `Prioritise` |
| `Priority Execution` | `Priority Rank Type` | `Processing Date` |
| `Processor` | `Prod Cat End` | `Prod Cat Start` |
| `Prod Prop Ol Accrual` | `Product` | `Product Only` |
| `Profit Acc Amount` | `Profit Acc Amt Facility Ccy` | `Profit Acc type` |
| `Profit Method` | `Profit Acc Amount` | `Profit Acc Amount Facility Ccy` |
| `Profit Acc Amount Facility Ccy.` | `Profit Acc Amt` | `Profit Acc Amt Facility Ccy` |
| `Profit Acc End Date` | `Profit Acc End Date` | `Profit Acc Start Date` |
| `Profit Acc Type` | `Profit Acc type` | `Profit Basis` |
| `Profit Calc Order` | `Profit Capitalisation` | `Profit Decl Txn` |
| `Profit Declaration Percentage` | `Profit Pay Method` | `Profit Property` |
| `Profit Share Amt` | `Profit Share Calc Amt` | `Profit Share Perc` |
| `Profit decl Expense PL` | `Prog Pay Perc` | `Progress Percentage` |
| `Prop Ol Accrual` | `Property` | `Property 1` |
| `Property Ol Accrual` | `Property Type` | `Property.1` |
| `Purchase Reference` | `Purchase Quantity` | `Purchase Reference` |
| `Rank Based Priority` | `Rate Type` | `Rc Condition` |
| `Rc Type` | `Rebate Action` | `Rebate Allowed` |
| `Rebate Currency` | `Rebate Pay` | `Rebate Payment Option` |
| `Rebate Type` | `Rebate Value` | `Recalc Profit` |
| `Recalc category` | `Recalc profit adjustment percentage` | `Recalculate` |
| `Recalculate Method` | `Recalculation` | `Refer Settlement` |
| `Refer Settlement Type` | `Registered at` | `Registration Expired on` |
| `Registration No` | `Remainder Activity` | `Repay Period` |
| `Repay Type` | `Repay type` | `Request Amount` |
| `Request Payment Holiday` | `Request Payment Holidays` | `Resale Customer ID, Resale Customer Name, Resale Settle Ac` |
| `Reserve Util Order` | `Residual Amount` | `Rest period` |
| `Restricted Asset` | `Retry Attempts` | `Retry Fqu` |
| `Retry Options` | `Retry Period` | `Return Unit Price` |
| `Review Date` | `Review Reference` | `Reviewer` |
| `Reviewer Account` | `Reviewer Name` | `Reviewer Type` |
| `Revolving` | `Ro Dist Adjust` | `Rollover Type` |
| `Rule Start` | `Rule Start Date` | `Rule.1` |
| `S Product` | `Sale Quantity` | `Sale Unit Price` |
| `Schedule Type` | `Seating Capacity` | `Sell Broker` |
| `Sell Broker Account` | `Sell Broker Acct` | `Sell Broker Wash Acct` |
| `Sell Quantity` | `Seller Customer ID` | `Seller Customer Name` |
| `Seller Settlement Ac` | `Settle Status` | `Settle Unearned Profit` |
| `Settlement A/c` | `Settlement Account` | `Settlement Type` |
| `Sh Account` | `Sh Add Early Mat Bal` | `Sh Add Excl Acct Bal` |
| `Sh Add Wak Dep Bal` | `Sh Add Wt Deposit Bal` | `Sh Balance Type` |
| `Sh Calc Type` | `Sh Category` | `Sh Currency` |
| `Sh Currency Option` | `Sh Expense Cat` | `Sh Recalc Rtn` |
| `Simulation Reference` | `Spcl Spread Rate` | `Spl Hiba Adj Pl Categ` |
| `Spl Hiba Expense Categ` | `Spl Hiba Income Categ` | `Spread Rate` |
| `Start Date` | `Start date` | `StartDt Option` |
| `Startdate` | `Status` | `Status Value Date` |
| `Status set as Return Commodity` | `Status set as Sell Commodity to Sell Customer` | `Stmt` |
| `Susp Appln` | `Susp End Date` | `Susp Start Date` |
| `Sweep Cancel Date` | `System Id` | `Takeover Npv` |
| `Takeover method` | `Target Rate` | `Tax Inclusive` |
| `Term` | `Title Deed Date` | `Title Deed From Date` |
| `Title Deed Number` | `Title Deed To Date` | `Tot Due Amt` |
| `Total Accrual Profit Amt` | `Total Accrual Profit Amount` | `Total Accrual Profit Amt` |
| `Total Accrued Profit Am` | `Total Accrued Profit Amt` | `Total Due` |
| `Tran Threshold Count` | `Txn Code` | `Txn Type` |
| `Type` | `Unit Price` | `Units` |
| `Units Equivalent of Purchase` | `Up to Amount.1` | `Upcoming Review Date` |
| `Update Commit On Capitalisation` | `Update Commit on Capitalisation` | `Update Rate` |
| `Update Utilised Commitment` | `Update Utilised Commitment` | `Usability` |
| `Use Profit Basis from Currency` | `User Activity` | `Valuation Fees` |
| `Valuation Id` | `Value` | `Value Date` |
| `Value Dtd Acctng Y/N` | `Value From` | `Value Of The property` |
| `Value To` | `Value date` | `Vehicle Status` |
| `Vendor` | `Vendor Account` | `Vendor Name` |
| `Vendor Pay Amount` | `Vendor Payment Status` | `Waive Bill Type` |
| `Waive Class, Waive Prop and Waive Bill Type` | `Wakala Adjust Cat` | `Wakala Adjust Option` |
| `Wakala Cat` | `Wakala Fee Amount` | `Wakala Fee Cat` |
| `Wakala Finance Ref` | `Wakala Incentive Cat` | `Warehouse Required` |
| `Weightage` | `Year of Construction` | `Year of Manufacture` |
| `property` | `xx` | `xx` |
| `Field.Value` |  |  |


---


## Appendix B: Consolidated Field Reference


This appendix consolidates all field description tables from across the documentation, grouped by sub-module. This provides a single reference for all field definitions.


### Islamic_Banking - ID (ID)


**Hybrid Pooling**

| Account Type | Company Name | System Date |
|---|---|---|
| CT account (100001) | Temenos core banking Norway company | 25/10/2017 |
| TR account (100002) | Temenos core banking Norway Sweden | 23/10/2017 |
| TR account (100003) | Temenos Core Banking Norway Finland | 24/10/2017 |

**Arrangement Pool Linking**

| Field Name | Description/Usage |
|---|---|
| Default Pool | Captures the default pool ID. If the conditions mentioned in the below fields do not satisfy, then the pool ID mentioned is defaulted. Allows a valid record from ID.POOL.PARAMETER . |
| Pool | Captures the pool ID to be defaulted, if the conditions mentioned in Appl Field Name , Field Operator , Value From , and Value To fields are satisfied. Allows a valid record from ID.POOL.PARAMETER . |
| Appl Field Name | symbol. |
| Field Operator | Captures the operator used during evaluation. Allows valid operators such as, Eq, Ge, Gt, Le, Lt, Lk, Ne, Nr, Rg, and UI. |
| Value From | Captures the starting value used for evaluation in Appl Field Name along with condition mentioned in Field Operator . |
| Value To | Captures the ending value used for evaluation in Appl Field Name along with condition mentioned in Field Operator . |
| Field Operation | Joins multiple condition for evaluation using and/or operators. |

**Misc**

| Field | Description |
|---|---|
| Income Cat | This field is used to define the income accrual PL category. It is a multi-value field used along with Income Product Cat for mapping the product income. PL categories set in the Accounting product condition of the respective product, needs to be mapped in this field. Allowed values are from the CATEGORY table . |
| Income Product Cat | This field is used to set the income product category. The finance product categories required for the pool calculation are set in this field . Allowed values are from the CATEGORY table. |
| Income Product | This field is reserved for future use. |
| Oth Income Cat | This field is used to set the income PL category for capturing the non–product related income. It is a multi-value field used along with Oth Income Pct for calculating the pool income. Allowed values are from the CATEGORY table. |
| Oth Acct Pct | This field is used to capture the percentage of other income to be consider in the pool calculation. Allowed values are from 0 -100. |
| Oth Income Acct | This field is used to set the income from the internal accounts. It is a multi-value field used along with Oth Inc Acct Pct for calculating the pool income. Allowed values are from the ACCOUNT table. |
| Oth Inc Acct Pct | This field is used to capture the percentage of other income from accounts to be used during the pool calculation. Allowed values are from 0 – 100. |

**Misc**

| Product Group | Product Name | Features |
|---|---|---|
|  | Pool Linking | Linking finance or deposit or account to pool with manual or automatic process |
| Islamic Deposits | 1 Month Mudaraba Deposit 12 Month Mudaraba Deposit 2 Year Mudaraba Deposit 3 Month Mudaraba Deposit 6 Month Mudaraba Deposit Long Term Mudaraba Deposit | Creates Mudaraba deposit for different currency or tenor using AA - Deposits product line. Books deposits for different tenor with or without rollover. The user defined property class and product condition features are used to capture the pool ID, deposit conditions, and early maturity recalculation options. Mudaraba deposit can be booked with the notional profit rate setup in ID.PDS.WEIGHT . |
| Advanced profit fixed Mudaraba Deposit | Mudaraba deposit can be booked with the notional profit rate setup in ID.PDS.WEIGHT . Profit amount is paid to the deposit customer on the deposit booking date. |  |
| Mudaraba Savings Plan | This is a recurring deposit product based upon Mudaraba. It can be opened for various tenor, currency and funding can be made based upon different frequency. It is possible to capitalise the profit amount calculated during PDS calculation. |  |
| Wakala Deposit | Wakala deposit for different currency or tenor is created by using AA – Deposits product line. Books deposits for different tenor with or without rollover. The user defined property class and product condition features are used to capture the pool ID. Wakala deposit can be booked with the notional profit rate setup in ID.PDS.WEIGHT . |  |
| Islamic Savings Accounts | Mudaraba Accounts Mudaraba Daily Product Savings Accounts | Mudaraba accounts for different currency can be opened by using AA – Accounts product line. Profit rate used for daily accruals defaulted from the notional profit rate setup in ID.PDS.WEIGHT . It is possible to setup the Tier balance-based calculation with Band or Level profit rate setup. The user defined property class and product condition features are used to capture the pool ID. |
|  | PDS Process – Simulation | The net profit amount is calculated from the income or expenses of the pool during the specified period. When net profit amount is derived, it is split based on the weighted average balance, (which takes into account the contributions to the pool, from each Mudaraba Deposit, Mudaraba Account, Wakala Deposit and share holder contribution). The weighted average calculation is based on the weightage setup during the parameter configuration. Applies IRR%, PER%, Mudarib share% calculation to reduce the net profit for each deposit before arriving at the distributable profit amount. Distributable profit rate is calculated from the profit amount. |
|  | PDS Process – Distribution | Applies identified profit rate to the underlying Mudaraba deposits or Mudaraba accounts. Based on the profit pay method available in Mudaraba deposits, profit amount is paid to the customer account on distribution date or at later date. For Mudaraba accounts profit amount is paid by using profit distribution frequency. For Wakala deposits profit adjustment accounting entries are generated. |
|  | Reverse – PDS Process – Distribution | After distributing the profit amount to the Mudaraba deposits or Mudaraba account or Wakala deposits, it is possible to reverse the PDS distribution. During the reversal, the accounting entries raised during old PDS distribution are reversed. New PDS distribution accounting entries are generated based upon the calculated adjustment amount. New PDS profit rate is distributed to the Deposits or Accounts, which posts the adjustment accounting entries for the profit amount calculated during old PDS distribution. |

**PDS Distribution**

| Field Name | Description |
|---|---|
| Action | This field is used to setup the list of actions and activities linked to the action. It is a mandatory field. Valid values are: Accounts Change Schedule Accounts rate Change Deposits Change Schedule Deposits rate Change Accounts Apply Changes To Close at PDS The above listed valid values are setup in EB.LOOKUP table with record ID as ID.DIST ACTION |
| User Activity | This field is used to setup the AA.ACTIVITY ID linked to Action field. |

**PDS Simulation**

| Process | Description |
|---|---|
| Simulation | The net profit amount is calculated from the income or expenses of the pool during the specified period. When the net profit amount is derived, it is split based on the weighted average method, which takes into account the contributions to the pool from each (Mudaraba deposit, Mudaraba account, Wakala deposit and shareholder equity). The weighted average balance calculation is based on the percentages and weights setup during the parameter configuration. The IRR%, PER%, Mudarib share% setup in ID.PDS.WEIGHT is used to reduce the split net profit for each deposit before arriving at the distributable profit amount. The profit amount is converted into profit rate. |
| Targetupdate | The user can amend the profit rate calculated to match the market expectations. Such amendment results in recalculation of the distributable profit amount. |
| Distribution | When the profit rate is finalised, it is applied to the underlying Mudaraba deposits or Mudaraba accounts. Based on the profit pay method available in Mudaraba deposits, profit is paid to the customer account on (distribution or at later date). For Mudaraba accounts, profit is paid by using profit distribution frequency setup in the ID.POOL.PARAMETER . For Wakala deposits, based on the parameter setup, profit adjustment accounting entries are generated. Otherwise, it is added to the shareholder equity. |
| Projection | This option is used to run the simulation from the simulation start date till the simulation end date. Simulation end date can be a future date. The net profit amount is calculated from the income or expenses of the pool during the specified period from simulation start date till the last working day. Net profit amount is projected from Last working day + 1 till the simulation end date by using the pro-rata calculation. When the projected net profit amount is derived, it is split based on the weighted average method, which considers the contributions to the pool from each (Mudaraba deposit, Mudaraba account, Wakala deposit and shareholder equity). The weighted average balance calculation is based on the percentages and weights setup during the parameter configuration. The IRR%, PER%, Mudarib share% setup in ID.PDS.WEIGHT is used to reduce the split net profit for each deposit before arriving at the distributable profit amount. The profit amount is converted into profit rate. It is not possible to distribute the projected simulation calculation. |
| Reverse Distribution | This option is used to reverse the last PDS distribution performed by user for a Pool on any day before running the subsequent PDS distribution. The PDS distribution accounting entries raised during old PDS distribution is reversed. But, the arrangement activities triggered as part of old PDS distribution to Mudaraba deposits or Mudaraba savings accounts is not reversed. Since, AA – Deposits module has the capability to reverse and replay the activities happened in the past, it uses the functionalities: Reversal request for old PDS distribution [Last] can be initiated. New simulation request for the old PDS distribution period is triggered. Target rate update is used to modify the profit rate calculated during simulation. During PDS distribution, the accounting entries generated for the old PDS distribution is reversed. New PDS distribution accounting entries are generated. |

**Misc**

| S.NO | Parameters | Description |
|---|---|---|
| 1 | Account | The Account property class is used by all the products which are account based. This property class primarily controls the description of the account. The ACCOUNT property allows the user to define and control balance treatment, posting restriction, linked account number (for memo accounts), currency market, date convention related setup for the account. Although the account names are account specific, generic titles can be defaulted from the product and can be replaced or given additional detail at the arrangement level. Each product defined and processed in AA can have a single ACCOUNT Property defined. |
| 2 | Activity Charges | The Activity Charges property class defines the charges that have to be applied when a particular activity is triggered on the arrangement. The charges so applied can be made due, capitalised or deferred. The user can enable auto settle the charges made due from unallocated credit balance by setting this to Yes. In accounts, charges are enabled for dormancy, settle payoff and ageing. This property class is also extensively used for all AA related modules, charges are set for various other activities. |
| 3 | Activity Restriction | The Activity Restriction property class is used to specify a restriction on a particular transaction. The restriction rules including the relevant periodic attributes and activities are defined in the product condition. These rules are then used to define activity based or property based restrictions. A rule if broken can be set to result in an override or error. A charge can be attached for this and can be set to be made due, capitalised or deferred. For the AR module, activity restriction is extensively used for restricting transactions by number, type, and so on. This is also extensively used in other modules to restrict the user from doing various user activity based on the life cycle status of contracts. |
| 4 | Balance Availability | The Balance Availability property class allows the user to control the following features pertaining to AR module: Notice amount and period, which needs to be given by a customer for withdrawing money from his account. Default Credit Check and Available Balance update related set up. Activity class or Activity specific credit check, and NSF related fees pertaining to it Tolerance Amount or Tolerance Currency - To indicate the grace amount, which is the allowed overdraft before the bank imposes NSF or OD fees. Overdraft Grace Period - To waive the NSF fee levied on the account, if the customer clears the debit balance within the stipulated grace period. |
| 5 | Dormancy | The Dormancy property class allows the user to control the parameterisation of inactive or dormant accounts and movement of the same into various buckets at the arrangement or product level. The same can be controlled based on period, and some exceptions or rules also can be added for evaluation and movement. The user can include or exclude certain activity or activity class for the evaluation. It is possible to, Configure different Dormancy status based on the period of inactivity Specify different charges and charging frequency for each Dormancy status Apply some exception rule filtering at an individual arrangement level (for example, account is in debit balance) and such rules can either be an API or a rule created using the Rules Engine Specify notices and notice frequency for each Dormancy status Specify Activities or Activity Classes or Activity Initiation Types which are qualified to keep an account active. Auto Reset can be enabled based on status or on Activity Type. |
| 6 | Facility | The Facility is a service component for financial products designed using arrangement architecture. The Facility property class controls the list of available services for an arrangement account. When an external activity (financial or non-financial) is triggered and the corresponding service group is mapped to an activity through Activity Mapping and EB.EVENTS . And the same came allowed or restricted or charged corresponding error message is raised to stop the activity. |
| 7 | Inheritance | The Inheritance property class is used for BN pool structure for inheriting the product conditions set at Parent level arrangement to the Child level arrangement accounts. The product conditions that are set for inheritance are attached to Property records with type as Inheritance Only. The properties to be inherited can be controlled both at source and target level. |
| 8 | Interest | The Interest property class is used for all interest definition and processing in AA. A product defined and processed in AA can have multiple interest properties defined (for example, principal interest, penalty interest, commission, etc. Interest rates can be defined as fixed , floating , periodic or linked rate (referring an INTEREST property from other arrangement), routine based calculation. Tiered interest can also be defined. Further it is possible to define a negative rate, minimum interest amount and waive the interest. Interest adjustment can be done in run time, and adjustment related detail or values can be captured in adjustment related fields. |
| 9 | Limit | The Limit property class primarily controls the use of LIMIT module by the product. We can set up single or shared limit. We can define the LIMIT.REFERENCE applicable for a specific product such that the system defaults the same in an arrangement. For a new limit, at the arrangement level, the LIMIT.SERIAL has to be given as NEW. The AR module can have self-contained secondary limit without having actual limit attached to it. Overdraft status or notice for AR module is handled inside the Limit Property class. Further Limits can be set to use the LIMIT module (AL and AD) or it can be managed only within the arrangement architecture framework. |
| 10 | Payment Schedule | The Payment Schedule property class is used by all products which have amounts billed (that is,made due) or capitalised or Pay. A Payment Schedule can be comprised of one or more payment definitions with conditions such as payment Type and Method, arrangement properties, dates and amounts. The AA.PAYMENT.TYPE application is used to define the standard payment types such as constant, linear, actual and fixed equal and so on, that can be used by a product. This payment type is then attached to each payment schedule definition. The start and end date can be specified, the user can specify the repayment of arrangement to commence after ‘n’ months from the arrangement date or ‘n’ months before the maturity or ‘n’ months after the change product or reset and rollover has happened. |
| 11 | Periodic Charges | The Periodic Charges property class acts as a container to group different charge properties and calculate a periodic charge amount. The Payment Schedule property class drives this property class. A periodic charge property can be attached in payment schedule and on schedule date periodic charge amount is calculated. At the arrangement level adjustment can be done by the user on whole periodic charge. |
| 12 | Statement | The Statement property class is used to define the legacy ACCT.STATEMENT feature at the AA level. Statements may be produced daily (every working day), every 1-9 weeks, twice a month (on the 15th and the last day of the month) or every 1-12 months on any day of the month. Up to nine statement cycles may be specified for each account, and each statement cycle is independent. In addition to this, special interim statements can be enabled. This property class also controls whether or not advices are to be produced when interest and charges are applied, and whether detailed interest statements (interest scale) should be produced. Within a statement cycle, it is possible to define multiple frequencies with a combination of weekly and monthly, such that statements are produced on the dates specified by both frequencies, but only contain details of entries since the last statement in that cycle. |

**Misc**

| S.No | Product Name | Product Attributes |
|---|---|---|
| 1 | Current Accounts | Corporate account with fixed debit interest Regular current account with floating Interest for both debit and credit interest, amount based capping of NSF Charges and waivers during account closure Current account with periodic charge Current account limit secured by deposit Current account for staff with additional interest Account with predefined overdraft limit of USD 250 Premium current account with some restriction on balance, and activities Current with some SME related features enabled Current account for SME - self service account Current account for students Current account for bundling, and gaining additional benefit through bundle Fully negotiable account Master account collects the interest from the Sub account and pays the interest accordingly Sub account pays the interest to the master account according to the maintained balance Payroll Account with cashback and count based capping of NSF Charges. Current Account for elite customers where the cheque issue fee is waived based on the relationship of the customer with the bank. The pricing evaluation runs on multiple arrangements of the customer which are fetched from Holdings MS and only those arrangements which are not in Non-accrual basis status is selected for pricing. Transact must be integrated with Holdings MS and the extension data mapping for this criteria set is to be configured locally to use this feature in the model product. |
| 2 | Savings Accounts | Regular saving account with basic features Regular saving account with restriction in Interest capitalisation Savings account for child Savings account for non resident Regular salary savings account Traditional notice savings account Savings account for staff |
| 3 | Summary Accounts | Summary account Currency summary account |

**Misc**

| S.No | Product Name | Product Attributes |
|---|---|---|
| 1 | Bonds | Bonds with Fixed term as 1 year Bonds with Fixed term as 3 year Bonds with Fixed term as 6 Months |
| 2 | Term Deposits | Term deposits for 3 months Term deposits for 6 months Term deposits for 9 months Term deposits for 12 months Term deposits for 18 months 2 year Term deposits 3 year Term deposits Long Term deposits Short Term deposits Call Deposits Fully Negotiable deposits |
| 3 | Savings Plan | Commitment Savings Plan |
| 4 | Retirement Plan Deposits | Term Deposits with tax condition defined to calculate withholding tax on the following activities: Deposit Withdraw Deposit Redemption Issue Bill for Deposit Interest The withholding taxes can be overwritten at the arrangement activity level by passing values using the context set of fields. |

**Chargeoff**

| AA Activity | IFRS Operation | Description |
|---|---|---|
| LENDING-IFRS.CHARGEOFF-REPORTING | CHARGE OFF | Indicates the loan is charged-off for the first instance. |
|  | CHARGE OFF INCREASE | Indicates loan is charged- off for an additional amount from earlier levels. |
|  | CHARGE OFF DECREASE | Indicates loan charge-off amount is decreased by specifying a negative amount. |
| LENDING-APPLYPAYMENT-PAYMENT.RULES ENDING- | RECOVERY | Indicates a repayment made on the loan. |
| LENDING-WRITE.OFF-BALANCE.MAINTENANCE | WRITE OFF | Indicates loan has been completely written off |
|  | WRITE OFF PARTIAL | Indicates a partial write off scenario which instead of entire loan only certain bills and/or balances are written off on contract. |
|  | ADJUSTMENT | Indicates any bill and/or balance adjustments made on the contract. |
| LENDING-MATURE-ARRANGEMENT | MATURE | Indicates loan has matured |
| LENDING-RESUME-ARRANGEMENT | RESUME | Indicates loan is resumed |

**Migration of LendingArrangements**

| Field | Content | Description |
|---|---|---|
| Arrangement | NEW | Requests New ID for the arrangement |
| Activity | LENDING-TAKEOVER-ARRANGEMENT | Create a new arrangement for takeover |
| Effective Date | Period Start Date | The date on which the legacy contract starts in our system, usually the start of an interest period. |
| Customer | Customer | The customer number allocated to the customer of the legacy loan contract. |
| Product | Product | The name of the product created as an equivalent to the legacy product. |
| Currency | Currency | Currency of the legacy loan. |
| Orig Contract Date | Legacy Start Date | The original start date of the legacy contract for information purposes |
| Legacy War Rate | Legacy War Rate | To retrieve the data provided in Context Name and Context Value fields and update the PERIODIC.RATE . |

**Migration of LendingArrangements**

| Field | Content | Description |
|---|---|---|
| Arrangement | Arrangement No | Indicates the arrangement number allocated by the takeover activity. |
| Activity | LENDING-CAPTURE.BILL-BALANCE.MAINTENANCE | Indicates the activity name which creates the new bill for an existing arrangement. |
| Effective Date | Period Start Date | Indicates the date when the legacy contract starts in our system. This is usually the start of an interest period. |
| Property.1 | Balance Maintenance Property Name | Indicates the name of the Balance Maintenance Property. |
| Field Name.1.1 | Bill Date | Indicates the name of the field to be updated in the balance maintenance property. |
| Field Value.1.1 | Bill Date | Indicates the original date the bill was created in the legacy system |
| Field Name.1.2 | PAYMENT.DATE | Indicates the name of the field to update in the Balance Maintenance Property. |
| Field Value.1.2 | Due Date | Indicates the original due date of the bill in the legacy system. |
| Field Name.1.3 | OR.BILL.AMOUNT | Indicates the name of the field to update in the Balance Maintenance Property. |
| Field Value.1.3 | Original amount | Indicates the original total amount of the bill issued in the legacy system. |
| Field Name.1.4 | PROPERTY-N | Indicates the name of the field to update in the Balance Maintenance Property. |
| Field Value.1.4 | Name of property | Indicates the name of the billed Property. |
| Field Name.1.5 | OR.PROP.AMT-N | Indicates the name of the field to update in the Balance Maintenance Property. |
| Field Value.1.5 | Original property amount | Indicates the original billed amount of the Property billed. |
| Field Name.1.6 | NEW.PROP.AMT-N | Indicates the name of the field to update in the Balance Maintenance Property. |
| Field Value.1.6 | Current outstanding property amount | Indicates the current outstanding billed amount for the associated Property to be taken over. |

**Migration of LendingArrangements**

| Field | Content | Description |
|---|---|---|
| Arrangement | Arrangement No | Indicates the arrangement number allocated by the takeover activity |
| Activity | LENDING-CAPTURE.BALANCE-BALANCE.MAINTENANCE | Indicates the activity that creates new balance for an existing arrangement |
| Effective Date | Period Start Date | Indicates the date at which the legacy contract starts in Temenos' system, usually the start of an interest period |
| Property 1 | Balance Maintenance Property Name | Indicates the name of the Balance Maintenance Property. |
| Field Name.1.1 | ADJUST.PROP-N | Indicates the name of the field used to update in the Balance Maintenance Property. |
| Field Value.1.1 | Penalty property | Indicates the name of the Penalty Interest or Charge Property to adjust. |
| Field Name.1.2 | ADJ.BAL.TYPE-N.N | Indicates the name of the field to update in the Balance Maintenance Property. |
| Field Value.1.2 | Balance name | Indicates the name of the penalty balance for the Associated Property, for example, CURPENINT. |
| Field Name.1.3 | NEW.BAL.AMT-N.N | Indicates the name of the field used to update in the Balance Maintenance Property. |
| Field Value.1.3 | Original amount | Indicates the balance amount for the associated property to takeover. |

**Scheduling Payments**

| Attribute | Value |
|---|---|
| Payment date for a scheduled payment | 14-May-2020 |
| Bill Produced | 10D |
| Finalise Bills | 2D |

**Misc**

| Core Routine Fields | Description | Routine Name |
|---|---|---|
| Pre processor | Used to define whether a message specific core routine needs to be called to pre-process a message. | RC.PREP.RC.TYPE – For example, RC.PREP.IC.CHARGE |
| Prioritise | Used to define the message-specific core routine called by the Transaction Recycler to perform transaction grouping and sorting. | RC.PRTY.RC.TYPE – For example, RC.PRTY.IC.CHARGE |
| Processor | Used to define the message-specific core routine called by the Transaction Recycler to process the Transaction Recycler transaction, or transactions if they are grouped. | RC.PROC.RC.TYPE – For example, RC.PROCE.IC.CHARGE |
| Post process | Defines the message-specific API routine called by the Transaction Recycler to perform processing after the transaction has been completed. | RC.POST.RC.TYPE – For example, RC.POST.IC.CHARGE |

**Misc**

| Business Event | Description |
|---|---|
| settlementService.transactionRetry.currentRetry | Event to be emitted when the transaction retry is moved to current status |
| settlementService.transactionRetry.fundRecovered | Event to be emitted for a transaction retry when the funds are recovered successfully |
| settlementService.transactionRetry.fundReserved | Event to be emitted for a transaction retry when the funds are reserved successfully |
| settlementService.transactionRetry.manuallyApproved | Event to be emitted when a transaction is manually approved |
| settlementService.transactionRetry.retryCancelled | Event to be emitted when the transaction retry is cancelled |
| settlementService.transactionRetry.retryCompleted | Event to be emitted when the transaction retry is completed |
| settlementService.transactionRetry.retryCreated | Event to be emitted when the transaction retry is created |


### Islamic_Banking - IS (IS)


**Hybrid Pooling**

| Account Type | Company Name | System Date |
|---|---|---|
| CT account (100001) | Temenos core banking Norway company | 25/10/2017 |
| TR account (100002) | Temenos core banking Norway Sweden | 23/10/2017 |
| TR account (100003) | Temenos Core Banking Norway Finland | 24/10/2017 |

**Asset Capture**

| Field Name | Description |
|---|---|
| Commodity Status | Indicates whether commodity is active. Valid values are defined in the EB.LOOKUP table with prefix IS.STATUS*. |
| Asset Type | Indicates the asset type. Valid values are Named and Quantified. |
| Asset Table | The application in which the asset is defined. This application could be a regular or dynamic table. Applicable for named asset types. |
| Allowed Unit | The units in which commodity is transacted. Valid values are defined in the EB.LOOKUP table with prefix IS.UNIT*. |
| Decimal Qty | Identifies the number of decimals the asset quantity can be transacted. Mandatory for quantified asset types. |
| Buy Broker | Lists the brokers who can transact as buy broker for the commodity. Must be a valid record from the table IS.BROKER . The broker allowed should be eligible for buy or both. Applicable for quantified asset types. |
| Sell Broker | Lists the brokers who can transact as sell broker for the commodity. Must be a valid record from the table IS.BROKER . The broker allowed should be eligible for sell or both. Applicable for quantified asset types. |

**Asset Capture**

| Named asset | Quantified asset |
|---|---|
| Specifies or captures individual specifications for each asset. | Does not specify individual asset-specific characteristics |
| A vehicle has specific features and characters that is captured such as, chassis number, engine number, etc. A house has specific features and characters like dimensions. | Oil, rice, vegetables, metals, etc. |

**Commodity Delivery and Sale**

| Application | Description |
|---|---|
| Commodity delivery ( IS.CONTRACT.DELIVERY ) | Tracks the delivery of commodities or assets. |
| Commodity sale ( IS.COMMODITY.SALE ) | Sells the delivered commodities to clients either partially or fully. |
| Commodity position ( IS.COMMODITY.POSITION ) | Tracks the commodities requested, delivered and sold details. |

**Finance Profit Upfront Sale Product Group**

| Field | Value and Description |
|---|---|
| Mode | Upfront Profit - The interest amount is collected at the beginning of the contract |
| Profit Method | Fixed - The total profit amount is fixed. |
| Rate Type | Reducing Rate, Flat Rate or Flat Amount. |
| Recalculate | Profit Amount - All activities that result in payment schedule recalculation can be configured to Profit Amount. |
| Actual profit amount | It is used to capture the upfront profit amount. Applicable only if Rate Type is set as Flat Amount. |
| Original profit amount | It is used to capture the upfront profit amount realised in the legacy system. Applicable only during a take-over activity (migration). |
| Advance Profit Accounting | Amort – Applicable only for flat rate and flat amount of profit contracts. The profit received in advance is booked to PL over the respite period. Cash Basis - The profit received in advance is booked to PL immediately on the respite date. Blank – If no option is selected , the functionality works similar to Cash Basis. |

**Islamic Contract**

| Field Name | Description |
|---|---|
| Finance Product | Identifies the AA lending or deposit products, which can be used in Islamic contract. |
| Eligible Status for Finance | Indicates the status after which contract is eligible to enter finance stage. |
| Company | The company for which asset restriction is placed. |
| Restricted Asset | Identifies the list of assets or commodities that are restricted for a particular company. |
| Status | Defines the list of statuses in a sequential order, which defines the workflow status for the product. A work flow status generates any one of the following accounting events or it does not generate accounting entry. Allowed accounting events are: Approval Reverse Approval Purchase Resale Cost Down Payment Sell commodity to sell broker and credit customer account Return commodity Broker settlement |
| Asset Delivery Tracking | Enables delivery tracking for assets. |

**Islamic Contract**

| Status | Description |
|---|---|
| Request | Asset details are auto populated from the existing named or quantified assets during Islamic contract creation. The user, Enters the required details. Captures client details, Islamic product, currency and value date details during request stage. Captures other static information specific to the asset or commodity. |
| Approval | During this stage, client and bank enters into an agreement called promise to purchase agreement Supplier or vendor details, asset costs, number of units and customer requested finance amount (for quantified assets) can be entered. Customer contribution in the project as down payment can be specified. Similarly, additional cost incurred on the asset to be purchased can be specified. This cost is paid either by the client or bank. It is possible to add the cost to the finance amount and repayment scheduled. |
| Purchase | During this stage, the asset is purchased by the bank and accounted in their books of accounts. Modifies down payment contribution and additional costs. It is possible to link multiple assets under the same purchase. |
| Down Payment | Modifies down payment contribution amount. During this stage, down payment amount can be collected automatically from the customer account or third party account. It is possible to collect down payment amount from multiple accounts. |
| Resale | During this stage, the asset is purchased from the seller and payment is made directly to the seller settlement account number. |

**Misc**

| Work-flow Stages | Description |
|---|---|
| Asset Request | Asset request is used for maintaining asset inventory to be sold based on requirement. This request is made, when there is a requirement from the customer or client. Asset can be classified into: Named ( for example, vehicle, machinery, equipment) Quantified (for example, agricultural produce, minerals) During this stage the below details are captured: Client Supplier Vendor/Resale Customer ID, Resale Customer Name, Resale Settle Account Asset cost and number of units Currency Other static information specific to the asset |
| Asset Approval | During this stage, the agreement of promise to purchase is entered into between the client and the bank. Specifies customer contribution in the project as down payment. Specifies any additional cost incurred on the asset to be purchased. This cost can paid either by the client or bank. Adds the cost to the finance amount and repayment scheduled. |
| Asset Purchase | During this stage, the asset is purchased by the bank and accounted in their books of accounts. Down payment contribution and additional costs can be modified. It is possible to link multiple assets under the same purchase. |
| Payment Management | Vendor payments, payment to cost counterparty, reviewer payments, broker payments (for treasury transactions) are made. Payments are consolidated vendor wise and can be made ad-hoc or scheduled. A certain percentage of the payment can be retained by the bank and paid subsequently as retention amount payment. |
| Sale or Finance | The purchased asset is sold to the client for which the payment is made as deferred installments. In a lease (Ijara) contract where the client is a lessee, lease rentals are paid to the bank. The modes of financing in Islamic banking are defined as different products, such as Murabaha, Musharaka, Ijara, Istisna, Salam, Mudaraba, and Wakala. |

**Misc**

| Application Name | Description |
|---|---|
| Asset Capture | Used to create, Asset or inventory. Own application tables to capture asset specifications. For example, IS.VEHICLE IS.REALESTATE IS.EQUIPMENT IS.MOVEQUIPMENT IS.MISCASSET |
| IS.CONTRACT | Used to, Purchase assets. Control credit workflow for Islamic assets. Define flexible workflow status based on requirements Raise flexible accounting entries based on defined workflow status. |
| IS.CONTRACT.DELIVERY | Used to track the delivery of commodities or assets. |
| IS.COMMODITY.SALE | Used to sell the delivered commodities to clients either partially or fully. |
| IS.ASSET.REVIEW | Used to manage the review activities for assets |
| IS.PAYMENT | Used to manage Islamic banking payment activities. |

**Misc**

| Application Name | Features |
|---|---|
| IS.PARAMETER | This table defines, Islamic product features. AA products that can be used for finance. Workflow status and also the status, which enables the sale process. Restrictions on contract creation for specific companies. Category codes and transaction types used at the time of credit workflow accounting. Stage at which customer contribution or down payment can be declared. Delivery tracking for specific type of assets Broker or reviewer category codes and transaction types. Allowed Product code range is from 1 to 9999 |
| IS.STATUS | This table defines, Applicable accounting entries for each of the defined workflow statuses are parameterised in the IS.PARAMETER table. The following accounting events related workflow statuses are defined in Status field of IS.PARAMETER table. Approval Rev Approval Purchase Cost Down Payment Return com to Broker Sell com to Sell Broker Broker Settlement Resale Applicable accounting entries for workflow status that can be used manually as and when required using IS.CONTRACT application. The following accounting events related workflow statuses are used in the IS.CONTRACT application. Sell Com To Sell Broker, Broker Settlement Return Com To Broker, Broker Settlement Broker Settlement accounting event entries are always generated along with either Return To Com To Broker or Sell Com To Sell Broker accounting events. |
| IS.COMMODITY | This table defines, Details of asset or commodity. Support named assets and quantified assets. Commodity active or inactive. Buy broker and sell broker for commodities. Allowed units and decimal quantity. Definition of unit price for commodity for each buy and sell broker combination. Daily allowed amount at commodity level Daily allowed quantity and amount for commodity-broker combination |
| IS.CONTRACT.TASK | This table defines, User-specific tasks and actions. Task or actions during asset purchase as checklist and tracks the same. Tasks that can be either generic or verification type. The ID of the table, which can be any text in alphanumeric format. |
| IS.COST.TYPE | This table defines, Costs incurred during purchase of asset or commodity. Status active or inactive. This parameter also specifies the charge code to default the charge amount for the cost in purchase contract. |
| IS.BROKER | This table defines, Broker related details specific to Islamic Treasury operations. Status active or inactive. Company to which broker belongs to. Broker account and beneficiary details per currency for a particular company. Broker type (Buy, Sell or Both). Broker fee collection related setup and broker share of fee payment frequency. |
| IS.VENDOR | This table defines, Vendor details. Status as 'Active' or 'Inactive' Company wise configuration of vendor account Vendor account and beneficiary details for each currency Commodity wise rebate configuration General rebate details and rebate currency, rebate type (amount or percentage) Special rebate details applicable for specific period with rebate currency, rebate type (amount or percentage) |
| IS.REVIEWER | This table defines, Reviewer related details with the name of the reviewer. Reviewer can be anyone involved in the project and does the service for a fee. Appraiser Project cost evaluator Project Auditor Advisor Legal Consultant Reviewer status whether 'Active' or 'Inactive' Company wise configuration of reviewer account Reviewer account and beneficiary details for each currency |

**Misc**

| Product Group | Product Name | Product Attributes |
|---|---|---|
| NA | Asset Capture | Named assets creation. New asset tables are created when required by user. New field names are added when required by user. |
| NA | Islamic Contract | Vendor purchase contract for named assets and quantified assets. Broker purchase contract for quantified assets. Automatic purchase contract workflow status update. Accounting entries generation based on workflow status. Down payment functionality. Capture cost-related information. |
| NA | Commodity Delivery and Sale | Track delivery of commodities. Sell the delivered commodity to different customers. Record profit or loss amount. |
| NA | Asset Review | Capture review details and collect fee for review. Split fee into customer fee and bank fee. Update project status and next review date. |
| NA | Payment Management | Use multiple payment applications. Support different payment types. |
| Finance - Profit Up-front Sale | Commodity Murabaha | It is a Murabaha based short term placement operation that involves the purchase and sale of commodities in the international exchange. Used for liquidity management purposes. |
| Ijara Finance | One party purchases and leases out the equipment required by the client for a rental fee. The duration of the rental and fee are agreed in advance and ownership of the asset remains with the lessor. At the time of contract maturity ownership. Alternatively, the lessee can agree at the outset to buy the asset at the end of the lease period. Profit collected at the beginning of the contract. Fixed profit method and profit amount is constant. |  |
| Murabaha Finance | Profit is collected at beginning of the contract. Fixed profit method and profit amount is constant. Commodity is sold for cost plus profit, and both the buyer and seller knows the cost and the profit involved. |  |
| Finance - Multi Structured Products | Musawama Finance Wakala Finance | Two types of finances are booked as a part of this product. Purchase cost is disbursed through Wakala contract with zero profit till shipment is in possession of seller. Later, Musawama contract is booked from Wakala start date with agreed profit amount. Profit is collected at the beginning of the contract. Fixed profit method and profit amount is constant. |
| Finance - Profit Accrual Sale | Bai Salam | An Islamic contract in which full payment is made in advance for specific goods (often agricultural products) to be delivered at a future date. Conventional profit bearing product. |
| Construction Finance | Islamic finance in which a manufacturer agrees to complete a construction project on a future date for a fixed, agreed-upon price and with product specifications that both parties agree to. |  |
| Diminishing Musharaka Finance | A partnership in which one of the partners promises to buy the equity share of the other partner gradually until the equity is completely transferred to him. |  |
| Forward Ijara Finance | Lease contract with sale of a clearly specified underlying asset, which is currently being produced or constructed, for a future delivery. With forward ijara, a financier undertakes payment during the construction period, while customer's payments will start within a specific period after completion |  |
| Mudaraba Finance | A partnership in profit whereby the bank provides capital as (Rab Al-maal) and the customer provides labour or work or experience as Mudarib |  |
| Qard Hassan Finance | A contract involving a finance with two parties on the basis of social welfare. During the finance process, the repayment amount must be the same as the amount borrowed. Profit rate to be defined as zero percentage. |  |

**PaymentManagementUsingPO**

| Table Name | Internal Vendor | Internal Retention | External Vendor | External Retention |
|---|---|---|---|---|
| PAYMENT.ORDER.PRODUCT | Pay Through Beneficiary = No | Pay Through Beneficiary = No | Pay Through Beneficiary = Yes Allow IBAN , Allow BIC and Allow Sort code fields = Allowed. | Pay Through Beneficiary = Yes |
| PP.MSGPAYMENTTYPE |  |  |  |  |
| PP.NODA.LIST |  |  |  |  |

**ProfitDeclaration**

| Field | Description |
|---|---|
| Income PL | It is used to setup the PL category to credit the bank portion of the realised profit received from the customer. |
| Profit decl Expense PL | It is used to setup the PL category to settle the shortage profit amount declared by the customer (Expected profit amount – Actual profit amount). |
| Profit Decl Txn | It is used to setup the FT.TXN.TYPE.CONDITION record to raise the realised profit declaration accounting entries. |

**ProfitDeclaration**

| Field | Description |
|---|---|
| ID | The facility or drawings reference number used for declaring the realised profit amount and a sequence number to handle the multiple profit declarations from the customer. AA131231312-001, where AA131231312 is the facility or drawings reference number and 001 is the sequence number. |
| Decl Level | It is used to identify the profit declaration level. It can be selected as Facility or Drawings and the system defaults these from the facility or drawings. |
| Arrangement | The system defaults the facility or drawings reference number captured in the ID automatically and it cannot be edited. |
| Accrual Start Date | The system defaults it automatically as Value date. If the realised profit amount is declared already, then it defaults the (previous accrual end date + 1) and it cannot be edited. |
| Accrual End Date | It is required to input the date up to which the profit amount is declared by the customer. |
| Customer | The system defaults the customer ID of the arrangement and it cannot be edited. |
| Product | The system defaults the arrangement product name and it cannot be edited. |
| Value date | The system defaults the arrangement value date and it cannot be edited. |
| Maturity date | The system defaults the arrangement maturity date and it cannot be edited. |
| Amount | The system defaults the arrangement amount and it cannot be edited. |
| Arrangement Status | The system defaults the arrangement status and it cannot be edited. |
| Booking Date | The user can input the value date for posting profit declaration accounting entries. |
| Drawing ID | If Decl level is set as Facility, then the system defaults the drawings (single or multiple) created under the facility automatically and it cannot be edited. |
| Drawings Arr Currency | It is used to display the currency of the Drawing ID . |
| Profit Acc Type | The system defaults the profit properties linked to the Facility or Drawings product marked with profit property type as Profit, Profit declaration and it cannot be edited. |
| Profit Acc Start Date | The starting date from which the profit amount accrued in the profit property populated in Profit Acc type . |
| Profit Acc End Date | The ending date up to which the profit amount accrued in the profit property populated in Profit Acc type . |
| Profit Acc Amount | Accrued profit amount from Profit Acc Start Date to Profit Acc End Date . |
| Profit Acc Amount Facility Ccy | In case if drawings are made in any other currency than facility currency then the Profit Acc Amount is converted and displayed in facility currency. |
| Total Accrual Profit Amount | Total accrued profit amount from multiple profit properties or multiple drawings populated in Profit Acc Amount Facility Ccy. |
| Declared Profit Amt | The user can input the realised profit amount declared by the customer in facility currency. |
| Acc Difference Amt | Difference between Total Accrual Profit Amt and Declared Profit Amt is updated. It is not allowed to edit the populated value. |
| Profit Share Perc | The system defaults the profit share percentage captured at the facility or drawings level automatically and it can be amended. |
| Profit Share Calc Amt | It is calculated by multiplying the Acc Difference Amt with the Profit Share Percentage . The un-rounded calculated amount is displayed in the field. |
| Profit Share Amt | It is used to display the rounded-off value of the Profit Share Calc Amt . It is rounded by considering the number of decimals configured in CURRENCY . |
| Settlement Account | This account is used to debit the bank share of the realised profit amount (or) and is used to credit the bank share of the shortage profit amount into the customer account which can be used to settle the Mudaraba finance outstanding amount. |

**ProfitDeclaration**

| Field | Description |
|---|---|
| Accrual Start Date | It is the value date of the facility reference number. If the profit amount is already declared for the facility reference number, then the system defaults the ( Accrual End Date + 1) of the previous profit declaration record into this field. |
| Accrual End Date | The user inputs this, and it has to be less than or equal to the maturity date of the facility reference number. |
| Profit Share Perc | The system defaults this value from the facility level condition and it can be amended. |
| Customer , Product , Contract Currency , Value Date , Maturity Date , Amount , Arrangement Status | The system defaults these values from the facility reference number. |
| Booking Date | It is used to capture the value date of the profit declaration. The system defaults it as the current date and it cannot be edited. |
| Drawing ID | The system populates the drawings created under the facility reference number automatically into this field. If the profit amount is declared at the facility level, then it is not possible to remove any drawings ID getting included in the profit declaration calculation. |
| Drawings Arr Currency | The system defaults this value from Drawing ID. |
| Profit Acc Type | The system defaults the profit properties associated with the Drawing product marked with property Type as Profit and Profit declaration into this field. It is not possible to remove the defaulted profit properties during profit declaration calculation. |
| Profit Acc Start Date , Profit Acc End Date , Profit Acc Amt , Profit Acc Amount Facility Ccy | These are used to default the accrued profit amount between “date from” and “date to” dates using the expected profit rate setup at the drawing level. The accrued profit amount is converted to facility currency and displayed in Profit Acc Amt Facility Ccy . The profit amount accrued between multiple dates are populated automatically for the relevant profit property. |
| Total Accrual Profit Amt | It displays the sum of the accrued profit amount from multiple profit properties linked to multiple drawings arrangement. |
| Declared Profit Amt | It is used to capture the profit amount declared by the customer. |
| Acc Difference Amount | It displays the difference between Total Accrual Profit Amt and Declared Profit Amt . |
| Profit Share Amt | The Profit Share Perc value is applied on the Acc Difference Amount to calculate it. |
| Settlement Account | It is used to capture the account number. |

**ProfitDeclaration**

| Field | Description |
|---|---|
| Accrual Start Date | It is the value date of the drawing reference number. If the profit amount is already declared for the drawing reference number, then the system defaults the ( Accrual End Date + 1) of the previous profit declaration record into the Accrual Start Date . |
| Accrual End Date | The user inputs this, and it is required to be less than or equal to the maturity date of the drawing reference number. |
| Profit Share Perc | The system defaults this from the drawing level condition. |
| Customer , Product , Contract Currency , Value Date , Maturity Date , Amount , Arrangement Status | The system defaults these from the drawing reference number. |
| Booking Date | It is used to capture the value date of the profit declaration. The system defaults it as current date and it cannot be edited. |
| Drawings ID | The system populates it from the ID. |
| Drawings Arr Currency | The system defaults it from Drawing ID. |
| Profit Acc Type | The system defaults the profit properties associated with the Drawing product marked with property Type as “Profit” and “Profit declaration” into this field. It is not possible to remove the defaulted profit properties during profit declaration calculation. |
| Profit Acc Start Date , Profit Acc End Date , Profit Acc Amount , Profit Acc Amt Facility Ccy | These are used to default the accrued profit amount between “date from” and “date to” dates using the expected profit rate setup at the Drawing level. The accrued profit amount is converted to facility currency and displayed in Profit Acc Amt Facility Ccy . The profit amount accrued between multiple dates are populated automatically for the relevant profit property. |
| Total Accrual Profit Amount | It displays the sum of the accrued profit amount from multiple profit properties linked to drawings arrangement. |
| Declared Profit Amt | It used to capture the profit amount declared by the customer. |
| Acc Difference Amount | It displays the difference between Total Accrual Profit Amt and Declared Profit Amt. |
| Profit Share Amt | Profit Share Percentage is applied on Acc Difference Amount to calculate this value. |
| Settlement Account | It is used to capture the account number. |

**Misc**

| S.NO | Parameters | Description |
|---|---|---|
| 1 | Account | The Account property class is used by all the products which are account based. This property class primarily controls the description of the account. The ACCOUNT property allows the user to define and control balance treatment, posting restriction, linked account number (for memo accounts), currency market, date convention related setup for the account. Although the account names are account specific, generic titles can be defaulted from the product and can be replaced or given additional detail at the arrangement level. Each product defined and processed in AA can have a single ACCOUNT Property defined. |
| 2 | Activity Charges | The Activity Charges property class defines the charges that have to be applied when a particular activity is triggered on the arrangement. The charges so applied can be made due, capitalised or deferred. The user can enable auto settle the charges made due from unallocated credit balance by setting this to Yes. In accounts, charges are enabled for dormancy, settle payoff and ageing. This property class is also extensively used for all AA related modules, charges are set for various other activities. |
| 3 | Activity Restriction | The Activity Restriction property class is used to specify a restriction on a particular transaction. The restriction rules including the relevant periodic attributes and activities are defined in the product condition. These rules are then used to define activity based or property based restrictions. A rule if broken can be set to result in an override or error. A charge can be attached for this and can be set to be made due, capitalised or deferred. For the AR module, activity restriction is extensively used for restricting transactions by number, type, and so on. This is also extensively used in other modules to restrict the user from doing various user activity based on the life cycle status of contracts. |
| 4 | Balance Availability | The Balance Availability property class allows the user to control the following features pertaining to AR module: Notice amount and period, which needs to be given by a customer for withdrawing money from his account. Default Credit Check and Available Balance update related set up. Activity class or Activity specific credit check, and NSF related fees pertaining to it Tolerance Amount or Tolerance Currency - To indicate the grace amount, which is the allowed overdraft before the bank imposes NSF or OD fees. Overdraft Grace Period - To waive the NSF fee levied on the account, if the customer clears the debit balance within the stipulated grace period. |
| 5 | Dormancy | The Dormancy property class allows the user to control the parameterisation of inactive or dormant accounts and movement of the same into various buckets at the arrangement or product level. The same can be controlled based on period, and some exceptions or rules also can be added for evaluation and movement. The user can include or exclude certain activity or activity class for the evaluation. It is possible to, Configure different Dormancy status based on the period of inactivity Specify different charges and charging frequency for each Dormancy status Apply some exception rule filtering at an individual arrangement level (for example, account is in debit balance) and such rules can either be an API or a rule created using the Rules Engine Specify notices and notice frequency for each Dormancy status Specify Activities or Activity Classes or Activity Initiation Types which are qualified to keep an account active. Auto Reset can be enabled based on status or on Activity Type. |
| 6 | Facility | The Facility is a service component for financial products designed using arrangement architecture. The Facility property class controls the list of available services for an arrangement account. When an external activity (financial or non-financial) is triggered and the corresponding service group is mapped to an activity through Activity Mapping and EB.EVENTS . And the same came allowed or restricted or charged corresponding error message is raised to stop the activity. |
| 7 | Inheritance | The Inheritance property class is used for BN pool structure for inheriting the product conditions set at Parent level arrangement to the Child level arrangement accounts. The product conditions that are set for inheritance are attached to Property records with type as Inheritance Only. The properties to be inherited can be controlled both at source and target level. |
| 8 | Interest | The Interest property class is used for all interest definition and processing in AA. A product defined and processed in AA can have multiple interest properties defined (for example, principal interest, penalty interest, commission, etc. Interest rates can be defined as fixed , floating , periodic or linked rate (referring an INTEREST property from other arrangement), routine based calculation. Tiered interest can also be defined. Further it is possible to define a negative rate, minimum interest amount and waive the interest. Interest adjustment can be done in run time, and adjustment related detail or values can be captured in adjustment related fields. |
| 9 | Limit | The Limit property class primarily controls the use of LIMIT module by the product. We can set up single or shared limit. We can define the LIMIT.REFERENCE applicable for a specific product such that the system defaults the same in an arrangement. For a new limit, at the arrangement level, the LIMIT.SERIAL has to be given as NEW. The AR module can have self-contained secondary limit without having actual limit attached to it. Overdraft status or notice for AR module is handled inside the Limit Property class. Further Limits can be set to use the LIMIT module (AL and AD) or it can be managed only within the arrangement architecture framework. |
| 10 | Payment Schedule | The Payment Schedule property class is used by all products which have amounts billed (that is,made due) or capitalised or Pay. A Payment Schedule can be comprised of one or more payment definitions with conditions such as payment Type and Method, arrangement properties, dates and amounts. The AA.PAYMENT.TYPE application is used to define the standard payment types such as constant, linear, actual and fixed equal and so on, that can be used by a product. This payment type is then attached to each payment schedule definition. The start and end date can be specified, the user can specify the repayment of arrangement to commence after ‘n’ months from the arrangement date or ‘n’ months before the maturity or ‘n’ months after the change product or reset and rollover has happened. |
| 11 | Periodic Charges | The Periodic Charges property class acts as a container to group different charge properties and calculate a periodic charge amount. The Payment Schedule property class drives this property class. A periodic charge property can be attached in payment schedule and on schedule date periodic charge amount is calculated. At the arrangement level adjustment can be done by the user on whole periodic charge. |
| 12 | Statement | The Statement property class is used to define the legacy ACCT.STATEMENT feature at the AA level. Statements may be produced daily (every working day), every 1-9 weeks, twice a month (on the 15th and the last day of the month) or every 1-12 months on any day of the month. Up to nine statement cycles may be specified for each account, and each statement cycle is independent. In addition to this, special interim statements can be enabled. This property class also controls whether or not advices are to be produced when interest and charges are applied, and whether detailed interest statements (interest scale) should be produced. Within a statement cycle, it is possible to define multiple frequencies with a combination of weekly and monthly, such that statements are produced on the dates specified by both frequencies, but only contain details of entries since the last statement in that cycle. |

**Misc**

| S.No | Product Name | Product Attributes |
|---|---|---|
| 1 | Current Accounts | Corporate account with fixed debit interest Regular current account with floating Interest for both debit and credit interest, amount based capping of NSF Charges and waivers during account closure Current account with periodic charge Current account limit secured by deposit Current account for staff with additional interest Account with predefined overdraft limit of USD 250 Premium current account with some restriction on balance, and activities Current with some SME related features enabled Current account for SME - self service account Current account for students Current account for bundling, and gaining additional benefit through bundle Fully negotiable account Master account collects the interest from the Sub account and pays the interest accordingly Sub account pays the interest to the master account according to the maintained balance Payroll Account with cashback and count based capping of NSF Charges. Current Account for elite customers where the cheque issue fee is waived based on the relationship of the customer with the bank. The pricing evaluation runs on multiple arrangements of the customer which are fetched from Holdings MS and only those arrangements which are not in Non-accrual basis status is selected for pricing. Transact must be integrated with Holdings MS and the extension data mapping for this criteria set is to be configured locally to use this feature in the model product. |
| 2 | Savings Accounts | Regular saving account with basic features Regular saving account with restriction in Interest capitalisation Savings account for child Savings account for non resident Regular salary savings account Traditional notice savings account Savings account for staff |
| 3 | Summary Accounts | Summary account Currency summary account |

**Chargeoff**

| AA Activity | IFRS Operation | Description |
|---|---|---|
| LENDING-IFRS.CHARGEOFF-REPORTING | CHARGE OFF | Indicates the loan is charged-off for the first instance. |
|  | CHARGE OFF INCREASE | Indicates loan is charged- off for an additional amount from earlier levels. |
|  | CHARGE OFF DECREASE | Indicates loan charge-off amount is decreased by specifying a negative amount. |
| LENDING-APPLYPAYMENT-PAYMENT.RULES ENDING- | RECOVERY | Indicates a repayment made on the loan. |
| LENDING-WRITE.OFF-BALANCE.MAINTENANCE | WRITE OFF | Indicates loan has been completely written off |
|  | WRITE OFF PARTIAL | Indicates a partial write off scenario which instead of entire loan only certain bills and/or balances are written off on contract. |
|  | ADJUSTMENT | Indicates any bill and/or balance adjustments made on the contract. |
| LENDING-MATURE-ARRANGEMENT | MATURE | Indicates loan has matured |
| LENDING-RESUME-ARRANGEMENT | RESUME | Indicates loan is resumed |

**Migration of LendingArrangements**

| Field | Content | Description |
|---|---|---|
| Arrangement | NEW | Requests New ID for the arrangement |
| Activity | LENDING-TAKEOVER-ARRANGEMENT | Create a new arrangement for takeover |
| Effective Date | Period Start Date | The date on which the legacy contract starts in our system, usually the start of an interest period. |
| Customer | Customer | The customer number allocated to the customer of the legacy loan contract. |
| Product | Product | The name of the product created as an equivalent to the legacy product. |
| Currency | Currency | Currency of the legacy loan. |
| Orig Contract Date | Legacy Start Date | The original start date of the legacy contract for information purposes |
| Legacy War Rate | Legacy War Rate | To retrieve the data provided in Context Name and Context Value fields and update the PERIODIC.RATE . |

**Migration of LendingArrangements**

| Field | Content | Description |
|---|---|---|
| Arrangement | Arrangement No | Indicates the arrangement number allocated by the takeover activity. |
| Activity | LENDING-CAPTURE.BILL-BALANCE.MAINTENANCE | Indicates the activity name which creates the new bill for an existing arrangement. |
| Effective Date | Period Start Date | Indicates the date when the legacy contract starts in our system. This is usually the start of an interest period. |
| Property.1 | Balance Maintenance Property Name | Indicates the name of the Balance Maintenance Property. |
| Field Name.1.1 | Bill Date | Indicates the name of the field to be updated in the balance maintenance property. |
| Field Value.1.1 | Bill Date | Indicates the original date the bill was created in the legacy system |
| Field Name.1.2 | PAYMENT.DATE | Indicates the name of the field to update in the Balance Maintenance Property. |
| Field Value.1.2 | Due Date | Indicates the original due date of the bill in the legacy system. |
| Field Name.1.3 | OR.BILL.AMOUNT | Indicates the name of the field to update in the Balance Maintenance Property. |
| Field Value.1.3 | Original amount | Indicates the original total amount of the bill issued in the legacy system. |
| Field Name.1.4 | PROPERTY-N | Indicates the name of the field to update in the Balance Maintenance Property. |
| Field Value.1.4 | Name of property | Indicates the name of the billed Property. |
| Field Name.1.5 | OR.PROP.AMT-N | Indicates the name of the field to update in the Balance Maintenance Property. |
| Field Value.1.5 | Original property amount | Indicates the original billed amount of the Property billed. |
| Field Name.1.6 | NEW.PROP.AMT-N | Indicates the name of the field to update in the Balance Maintenance Property. |
| Field Value.1.6 | Current outstanding property amount | Indicates the current outstanding billed amount for the associated Property to be taken over. |

**Migration of LendingArrangements**

| Field | Content | Description |
|---|---|---|
| Arrangement | Arrangement No | Indicates the arrangement number allocated by the takeover activity |
| Activity | LENDING-CAPTURE.BALANCE-BALANCE.MAINTENANCE | Indicates the activity that creates new balance for an existing arrangement |
| Effective Date | Period Start Date | Indicates the date at which the legacy contract starts in Temenos' system, usually the start of an interest period |
| Property 1 | Balance Maintenance Property Name | Indicates the name of the Balance Maintenance Property. |
| Field Name.1.1 | ADJUST.PROP-N | Indicates the name of the field used to update in the Balance Maintenance Property. |
| Field Value.1.1 | Penalty property | Indicates the name of the Penalty Interest or Charge Property to adjust. |
| Field Name.1.2 | ADJ.BAL.TYPE-N.N | Indicates the name of the field to update in the Balance Maintenance Property. |
| Field Value.1.2 | Balance name | Indicates the name of the penalty balance for the Associated Property, for example, CURPENINT. |
| Field Name.1.3 | NEW.BAL.AMT-N.N | Indicates the name of the field used to update in the Balance Maintenance Property. |
| Field Value.1.3 | Original amount | Indicates the balance amount for the associated property to takeover. |

**Misc**

| Product Name | Product Attributes |
|---|---|
| Home Equity | CEL Loan Home Equity Line of Credit Home Equity with LOC with Floating interest initially for 9 years and then periodic interest with annuity type of repayments. Home Equity Loan Home Equity without LOC for 25 Years term. Interest only payments for the first 9 years and with annuity type of repayments. |
| Line of Credit (LOC) | LOC with 3% Principal Repayment LOC with 3% Principal Repayment with revolving credit facility. LOC with Interest Only Payments LOC with interest only payments and revolving limit that reinstates on repayments. LOC with credit line product with default term as 10 years and Revolving as Payment. LOC with interest only payments and revolving limit that reinstates on repayments. |
| Mortgages | Bridge Mortgage A bridge loan to connect two mortgages with a term of around 1 year (the maximum term is 5 years). Repayment of Interest amount is scheduled on monthly basis and principal amount is scheduled on the maturity date. Mortgage Mortgage loan with automatic disbursement configured and annuity type of repayments with periodic interest. Any advance payments get a benefit from both principal and interest components. Mortgage (Adjustable Rate) Mortgage loan with periodic rate resets for every year. Escrow charges are included in the monthly constant payment schedule. Mortgage (Fixed Equal Repayment) The schedule has a Fixed Equal Repayment . On events like advance repayment, change in components like interest, schedule, and so on, the Term is recalculated till the maximum possible (based on the term) and capped with the maximum term. Thereafter, the payment amount is calculated. Mortgage (Seasonal Repayments) Seasonal constant repayments configured in schedule. For example, 1, 3, 7, 10, month. Mortgage (Special Offer) Interest offset advantage for the initial period. Mortgage (Cash Back) Mortgage loan Bonus for prompt repayment Advance repayment with principal benefit only Mortgage (Linked Rate) A Mortgage loan any advance repayment does not have any benefits. Penalty interest is adopted from a linked principal interest rate. Mortgage (Fixed 2 year Product) Fixed two-year mortgage that allows loan with overpayment on adhoc or regular basis based on a fixed amount. Mortgage (Fixed 5 year Product) Loan with overpayment on Adhoc or Regular basis based on a current balance percentage. |
| Personal Loans | Personal Loan Personal Loan (Biweekly Repayment) Personal Loan (Linked Rate) Student Loan (Loans to student aged between 15 to 25 years) Vehicle Loan Forward dated personal loan is specifically created for the repayment calculator Payroll Loan Loan for people under payrolls FASB Loan Financial Accounting Standards Based Loan |
| Small Business Loans | Small Business Loan Small Business loan with loan revolving as prepayment and a preferential pricing Commercial Loan (Interest Upfront) Small Business loan with interest upfront with loan revolving as prepayment Fully Negotiable Loan Default (For Failed Eligibility) War Loan The calculation of a weighted average interest rate for the loans, which have multiple legs (tranches). |
| Consumer Loan | Single or Multiple Disbursement loan with the cancel period of 7 Days. No Interest Definition. Instead a DISBURSEMENTFEE is added based on the current disbursement amount. DISBURSEMENTFEE is a Tiered charge with a Cap of 250. REFUNDFEE is given as Credit Type to the customer on doing a repayment. |
| Technical Loan | Term amount with a Minimum value as 1000 and Maximum value as 25000 with multiples of 100. Category is set as 3112 in the ACCOUNT property class. Repay current balance is set for ACCPRINCIPALINTINF and CURACCOUNTINF in Payment. Rule property class. |
| Instalment Loan | Instalment loan for 12 month Instalment loan for 6 month Instalment loan for 3 month |
| War Loan | It is created to enable the calculation of a weighted average interest rate for the loans, which have multiple legs (tranches). |
| Digi Mortgages | Digi Mortgage 2Y Fixed+Constant Pay Constant Repayment Type, Fixed Interest Rate is applicable for first 2 years and Periodic Interest Rate thereafter. On a principal decrease, either the loan term or the loan repayment amount can be recalcuated based on the user choice. Digi Mortgage 2Y Tracker+Int Only Interest only Repayment Type, Floating Interest Rate is applicable for first 2 years and Periodic Interest Rate thereafter. On a principal decrease, either the loan term or the loan repayment amount can be recalculated based on the user choice. Digi Mortgage 5Y Fixed+Constant Pay Constant Repayment type, Fixed Interest Rate is applicable for first 5 years and Periodic Interest Rate thereafter. On a principal decrease, either the loan term or the loan repayment amount can be recalculated based on the user choice. Digi Mortgage 5Y Track+Constant Pay Constant Repayment type, Floating Interest Rate is applicable for first 5 years and Periodic Interest Rate thereafter. On a principal decrease, either the loan term or the loan repayment amount can be recalculated based on the user choice. |

**Scheduling Payments**

| Attribute | Value |
|---|---|
| Payment date for a scheduled payment | 14-May-2020 |
| Bill Produced | 10D |
| Finalise Bills | 2D |

**Misc**

| Core Routine Fields | Description | Routine Name |
|---|---|---|
| Pre processor | Used to define whether a message specific core routine needs to be called to pre-process a message. | RC.PREP.RC.TYPE – For example, RC.PREP.IC.CHARGE |
| Prioritise | Used to define the message-specific core routine called by the Transaction Recycler to perform transaction grouping and sorting. | RC.PRTY.RC.TYPE – For example, RC.PRTY.IC.CHARGE |
| Processor | Used to define the message-specific core routine called by the Transaction Recycler to process the Transaction Recycler transaction, or transactions if they are grouped. | RC.PROC.RC.TYPE – For example, RC.PROCE.IC.CHARGE |
| Post process | Defines the message-specific API routine called by the Transaction Recycler to perform processing after the transaction has been completed. | RC.POST.RC.TYPE – For example, RC.POST.IC.CHARGE |

**Misc**

| Business Event | Description |
|---|---|
| settlementService.transactionRetry.currentRetry | Event to be emitted when the transaction retry is moved to current status |
| settlementService.transactionRetry.fundRecovered | Event to be emitted for a transaction retry when the funds are recovered successfully |
| settlementService.transactionRetry.fundReserved | Event to be emitted for a transaction retry when the funds are reserved successfully |
| settlementService.transactionRetry.manuallyApproved | Event to be emitted when a transaction is manually approved |
| settlementService.transactionRetry.retryCancelled | Event to be emitted when the transaction retry is cancelled |
| settlementService.transactionRetry.retryCompleted | Event to be emitted when the transaction retry is completed |
| settlementService.transactionRetry.retryCreated | Event to be emitted when the transaction retry is created |


---
