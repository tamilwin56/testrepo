
# Temenos Transact — Deposits Module Documentation


> **Comprehensive User Guide**
> Generated: 13 April 2026
> Content: Configuration | Reference | Field Descriptions | Glossary


## Table of Contents

  - [Deposits Module Overview](#deposits-module-overview)
    - [Sub-Module Summary](#sub-module-summary)
    - [How to Use This Guide](#how-to-use-this-guide)
  - [Chapter 1: Deposits - AD](#chapter-1-deposits---ad)
    - [Features in Deposits - AD](#features-in-deposits---ad)
    - [1.1  Account Statements](#11-account-statements)
    - [1.2  COB Processing](#12-cob-processing)
    - [1.3  Charges and Commissions](#13-charges-and-commissions)
    - [1.4  Hybrid Pooling](#14-hybrid-pooling)
    - [1.5  Misc](#15-misc)
    - [1.6  Charges](#16-charges)
    - [1.7  SubAccounts](#17-subaccounts)
    - [1.8  Limit Balance](#18-limit-balance)
    - [1.9  Misc](#19-misc)
    - [1.10  Accounting in Deposits](#110-accounting-in-deposits)
    - [1.11  Cancel Period](#111-cancel-period)
    - [1.12  Charges](#112-charges)
    - [1.13  Cooling Period](#113-cooling-period)
    - [1.14  Customer Ownership and Eligibility](#114-customer-ownership-and-eligibility)
    - [1.15  Deposit Closure](#115-deposit-closure)
    - [1.16  Deposit Creation](#116-deposit-creation)
    - [1.17  Deposit Simulation](#117-deposit-simulation)
    - [1.18  Dormancy](#118-dormancy)
    - [1.19  Early Redemption of Deposit](#119-early-redemption-of-deposit)
    - [1.20  Funding of Deposit](#120-funding-of-deposit)
    - [1.21  Future Dated Conditions](#121-future-dated-conditions)
    - [1.22  Interest](#122-interest)
    - [1.23  Interest Adjustments](#123-interest-adjustments)
    - [1.24  Migration Process](#124-migration-process)
    - [1.25  Migration RFR LIBOR](#125-migration-rfr-libor)
    - [1.26  Misc](#126-misc)
    - [1.27  Notice for Redemption of Funds](#127-notice-for-redemption-of-funds)
    - [1.28  Preclosure of Deposits](#128-preclosure-of-deposits)
    - [1.29  ProductVariations](#129-productvariations)
    - [1.30  Risk Free Rates](#130-risk-free-rates)
    - [1.31  Rollover of Deposits](#131-rollover-of-deposits)
    - [1.32  Savings Plan Product](#132-savings-plan-product)
    - [1.33  Statements](#133-statements)
    - [1.34  Swift Messages for Deposit](#134-swift-messages-for-deposit)
    - [1.35  Tax](#135-tax)
    - [1.36  Valuations and Interface to Securities Module](#136-valuations-and-interface-to-securities-module)
    - [1.37  Withdrawal from a Deposit](#137-withdrawal-from-a-deposit)
    - [1.38  Chargeoff](#138-chargeoff)
    - [1.39  Charges](#139-charges)
    - [1.40  LendingRule78](#140-lendingrule78)
    - [1.41  Limit Facility for Loan](#141-limit-facility-for-loan)
    - [1.42  Loan Commitment](#142-loan-commitment)
    - [1.43  Migration of LendingArrangements](#143-migration-of-lendingarrangements)
    - [1.44  Payment Holiday](#144-payment-holiday)
    - [1.45  Scheduling Payments](#145-scheduling-payments)
    - [1.46  Weighted Average Rate](#146-weighted-average-rate)
    - [1.47  Misc](#147-misc)
  - [Chapter 2: Deposits - FD](#chapter-2-deposits---fd)
    - [Features in Deposits - FD](#features-in-deposits---fd)
    - [2.1  Fiduciaries Workflow](#21-fiduciaries-workflow)
    - [2.2  Misc](#22-misc)
  - [Appendix A: Glossary of T24 Applications & Fields](#appendix-a-glossary-of-t24-applications-fields)
    - [Applications](#applications)
    - [Fields Referenced](#fields-referenced)
  - [Appendix B: Consolidated Field Reference](#appendix-b-consolidated-field-reference)
    - [Deposits - AD (AD)](#deposits---ad-ad)
    - [Deposits - FD (FD)](#deposits---fd-fd)

---


## Deposits Module Overview


This document provides comprehensive documentation for the **Deposits** module of Temenos Transact. It covers **2 sub-modules** with a total of **49 feature areas**.


### Sub-Module Summary


| # | Sub-Module | Code | Features | Description |
|---|-----------|------|----------|-------------|
| 1 | **Deposits - AD** | `AD` | 47 | Deposits - AD module of Temenos Transact |
| 2 | **Deposits - FD** | `FD` | 2 | Deposits - FD module of Temenos Transact |


### How to Use This Guide


Each feature in this document is organized into the following sections:

- 📖 **Introduction** — Overview and purpose of the feature
- ⚙️ **Configuration** — How to set up and configure the feature
- 🔧 **Working With** — Operational usage and field descriptions
- 📋 **Tasks** — Step-by-step procedures
- 📊 **Outputs** — Reports, enquiries, and generated outputs

Each feature includes a **Quick Reference Card** at the top with application names, key fields, prerequisites, and a summary. Appendices provide a full glossary, consolidated field tables, and end-to-end use-case scenarios.

---


## Chapter 1: Deposits - AD


Deposits - AD module of Temenos Transact


### Features in Deposits - AD


| # | Feature | Sections |
|---|---------|----------|
| 1.1 | Account Statements | Intro |
| 1.2 | COB Processing | Worki |
| 1.3 | Charges and Commissions | Worki |
| 1.4 | Hybrid Pooling | Worki |
| 1.5 | Misc | Intro |
| 1.6 | Charges | Worki |
| 1.7 | SubAccounts | Confi |
| 1.8 | Limit Balance | Intro |
| 1.9 | Misc | Intro |
| 1.10 | Accounting in Deposits | Intro, Confi, Worki, Tasks, Outpu |
| 1.11 | Cancel Period | Intro, Confi, Worki, Tasks, Outpu |
| 1.12 | Charges | Intro, Tasks, Outpu |
| 1.13 | Cooling Period | Intro, Confi, Worki, Tasks, Outpu |
| 1.14 | Customer Ownership and Eligibility | Intro, Confi, Worki, Tasks, Outpu |
| 1.15 | Deposit Closure | Intro, Confi, Worki, Tasks, Outpu |
| 1.16 | Deposit Creation | Intro, Confi, Worki, Tasks, Outpu |
| 1.17 | Deposit Simulation | Intro, Confi, Worki, Tasks, Outpu |
| 1.18 | Dormancy | Intro, Confi, Worki, Tasks, Outpu |
| 1.19 | Early Redemption of Deposit | Intro, Confi, Worki, Tasks, Outpu |
| 1.20 | Funding of Deposit | Intro, Confi, Worki, Tasks, Outpu |
| 1.21 | Future Dated Conditions | Intro, Confi, Worki, Tasks, Outpu |
| 1.22 | Interest | Intro, Tasks, Outpu |
| 1.23 | Interest Adjustments | Intro, Confi, Worki, Tasks, Outpu |
| 1.24 | Migration Process | Intro, Confi, Worki, Tasks, Outpu |
| 1.25 | Migration RFR LIBOR | Intro, Confi, Worki, Tasks, Outpu |
| 1.26 | Misc | Intro |
| 1.27 | Notice for Redemption of Funds | Intro, Confi, Worki, Tasks, Outpu |
| 1.28 | Preclosure of Deposits | Intro, Confi, Worki, Tasks, Outpu |
| 1.29 | ProductVariations | Intro, Confi, Worki, Tasks, Outpu |
| 1.30 | Risk Free Rates | Intro, Confi, Worki, Tasks, Outpu |
| 1.31 | Rollover of Deposits | Intro, Confi, Worki, Tasks, Outpu |
| 1.32 | Savings Plan Product | Intro, Confi, Worki, Tasks, Outpu |
| 1.33 | Statements | Intro, Confi, Worki, Tasks, Outpu |
| 1.34 | Swift Messages for Deposit | Intro, Confi, Worki, Tasks, Outpu |
| 1.35 | Tax | Intro, Confi, Worki, Tasks, Outpu |
| 1.36 | Valuations and Interface to Securities Module | Intro, Confi, Worki, Tasks, Outpu |
| 1.37 | Withdrawal from a Deposit | Intro, Confi, Worki, Tasks, Outpu |
| 1.38 | Chargeoff | Worki |
| 1.39 | Charges | Worki |
| 1.40 | LendingRule78 | Intro |
| 1.41 | Limit Facility for Loan | Intro |
| 1.42 | Loan Commitment | Confi |
| 1.43 | Migration of LendingArrangements | Worki |
| 1.44 | Payment Holiday | Intro, Confi, Worki |
| 1.45 | Scheduling Payments | Confi, Worki |
| 1.46 | Weighted Average Rate | Intro |
| 1.47 | Misc | Intro |


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


### 1.5  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *In the payment landscape, payment processing is a complex process, where booking is just one of the steps. The Temenos Payments Hub (TPH) orchestrates the payment execution. The account status check, funds reservation and booking can take place at different stages of payment processing.*
> 
> **Applications:** `AC.ENTRY.PARAM`, `AC.INWARD.ENTRY`, `CATEG.ENTRY`, `EB.SYSTEM.ID`, `EXTERNAL.SEPA.DETAILS`, `GENERIC.ACCOUNTING.REQUEST`, `MS.PARAMETER`, `RE.CONSOL.SPEC.ENTRY` ... +1 more
> 
> **Key Fields:** *A*, *Attribute*, *Contra Acc*, *Contra Acct Categ*, *Contra Cr Txn Code*, *Contra Currency*, *Contra Dr Txn Code*, *Contra Entry* ... +25 more
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- Temenos Transact Services

In the payment landscape, payment processing is a complex process, where booking is just one of the steps. The Temenos Payments Hub (TPH) orchestrates the payment execution. The account status check, funds reservation and booking can take place at different stages of payment processing.

TPH uses the internal Temenos Transact Deposit Demand Account interface to check the account status, reserve funds and raise bookings in an embedded manner. However, when a bank implements a third party payment system, these APIs must be invoked from that system or an ESB, and possibly from other solutions implemented by the bank like online channels, cards interfaces, and so on.

Depending on their enterprise architecture, banks can have multiple systems or interfaces to invoke the APIs for:

- Checking if a transaction can be applied on an account (cover request).
- Reserving funds on an account (reservation request).
- Booking an entry or entries on an account (booking request).

Temenos Generic Accounting Interface (GAI), also known as OFS clearing, accepts cover, reservation and booking requests sent by other banks’ systems to Temenos Transact.

Depending on the type of processing, a synchronous and/or asynchronous response(s) is sent by the GAI. Then, this response is forwarded by the Enterprise Service Bus (ESB) back to the request source system to take a decision on the payment processing.

The request messages are received through queues in the Temenos OFS Clearing proprietary format. The formatting to the Temenos request format, from the Temenos response format and routing are done in ESB.

The GENERIC.ACCOUNTING.REQUEST application allows the user to manually reverse a transaction that is successfully posted through GAI. This creates a booking reversal request, which is processed using the GAI mechanism.


##### Product Configuration

The main processing rules related to Generic Accounting Interface (GAI) messages are described in the AC.ENTRY.PARAM application and cover the following:

- System ID associated with the bookings
- Message layout – the header and the data items provided in the message
- Entry and fields separator
- Default transaction codes
- Contra-related options
- Accounting mode for exceptions handling
- Additional validations
- Duplicate check rule
- Suspense details
- Fund Transfer (FT) transaction type used in suspense posting
- Response options

A record must be created in the EB.SYSTEM.ID application for the System id indicated in AC.ENTRY.PARAM , AC.INWARD.ENTRY .

This appears in the accounting entries raised by GAI (populated in the STMT A dd D etail V alue field associated with the Add Detail Name PARENT.TXN.SYS.ID in STMT.ENTRY ) and indicates that the entries have been generated through GAI.

| Values in the Data Item field | Description |
|---|---|
| CONTROL TOTAL | Displays the total number of items in the request. If this is provided in the message, it is checked against the number of actual entries in the message. |
| SIGN | When the sign is not supplied in the request, the value in the header is used by default. |
| CURRENCY | When the currency is not supplied in the request, the value in the header is used by default. |
| LOCAL REF | Supplied at the header level and stored in the AC.INWARD.ENTRY record, which stores the header of the CSMBATCH message. |
| EXT.BATCH.REF | The batch reference provided in the batch message (if any) is not only populated in the batch entry in AC.INWARD.ENTRY , but also in the individual ones. For CSM and CSMBULK, this is populated in the accounting entries raised on the contra account and on the accounts specified in the request message; it will be stored in STMT.ENTRY / CATEG.ENTRY / RE.CONSOL.SPEC.ENTRY , in the ADD.DETAIL.VALUE field associated with the ADD.DETAIL.NAME field, which has the value “EXT.BATCH.REF”. |

The default entry delimiter is ‘_’ and the default field delimiter is ‘,’. In some markets or regions, these characters are included in the allowed character set and are used by customers when making payments. So, the banks must provide a different character than the default one.

The values can be specified in the Entry Delim iter and Field Delim fields in AC.ENTRY.PARAM . The characters used as delimiters are ` ! @ # $ % & * ( ) _ - + = [ ] { } ; / \ |

The Dr Txn Code and Cr Txn Code fields indicate the default transaction codes that are used if transaction code is not supplied in the request entry.

| Values in the Contra Entry field | Description |
|---|---|
| ENTRY | The balancing entry is raised for each entry indicated in the request. |
| CURRENCY.NET | Balance by currency, netting debit and credit entries, irrespective of the value date. If the entries that are part of an online posting message are netting for each currency to zero, a balancing entry is not raised. |
| CURRENCY | Balance by currency and sign, irrespective of the value date. A consolidated entry is created for all debit/credit entries, per each currency. |
| CCY.VAL.NET | Balance by value date and currency, irrespective of sign netting debits and credits. If the entries that are part of an online posting message are netting to zero per currency and per value date, a balancing entry is not raised. |
| CURRENCY.VAL.NET | Balance by currency, sign and value date. A consolidated entry is created for all debit/ credit entries, per each currency, sign and value date. |
| LOCAL | To raise balancing entries in the local currency irrespective of request currency. Balancing happens by value date, processing date, accounting date, and netting the debit and credit entries irrespective of sign. |
| CCY.PROC.NET | To allow balancing using currency, processing date, and netting debit and credit entries irrespective of sign. |

| Accounting Mode | In case of Error During Processing | In case of Override During Processing | No Error or Override During Processing |
|---|---|---|---|
| SAO | Posted to suspense account | Posted to target account or PL | Posted to target account or PL |
| SSS | Posted to suspense account | Posted to suspense account | Posted to target account or PL |
| SNP | No posting - rejected (Read Note | No posting –- rejected | Posted to target account or PL |

For CSM, CSMBULK and CSMBATCH, it is mandatory to be set as unique and implies that a record is created and stored for each entry in AC.INWARD.ENTRY .

The following type of responses are supported by GAI:

- Detail – Synchronous response, it returns the result and the type ID of the entry.
- Summary – Synchronous response, it returns the result only.
- ExtDetail – Asynchronous response through Integration Framework, it returns all the details available in the entry.
- ExtBatch – Asynchronous response through Integration Framework, it returns all the header details.

In AC.ENTRY.PARAM , the Interface Type field is set to Internal.


##### Business Events

When the Emit Business Event field in MS.PARAMETER is set as ‘Yes’, the business events representing the state change are emitted.

The following business events are emitted for Generic Accounting Interface tables.

| Business Event | Description |
|---|---|
| settlementService.checkFunds.fundAvailable | Event for a cover request when sufficient funds are available in the account |
| settlementService.checkFunds.fundNotAvailable | Event for a cover request when sufficient funds are not available in the account |
| settlementService.creditRequest.accountCredited | Event for a book request when the account is credited successfully |
| settlementService.creditRequest.creditFailed | Event for a book request when credit transaction to an account fails |
| settlementService.creditRequest.creditSubmittedForRetry | Event for a book request when credit transaction to an account submitted for a retry |
| settlementService.creditRequest.creditSuspended | Event for a book request when credit transaction to an account gets suspended |
| settlementService.debitRequest.accountDebited | Event for a book request when the account is debited successfully |
| settlementService.debitRequest.debitFailed | Event for a book request when debit transaction to an account fails |
| settlementService.debitRequest.debitSubmittedForRetry | Event for a book request when debit transaction to an account submitted for a retry |
| settlementService.debitRequest.debitSuspended | Event for a book request when debit transaction to an account gets suspended |
| settlementService.reserveRequest.fundReserved | Event for a reserve request when the funds are reserved successfully |
| settlementService.reserveRequest.reserveFundFailed | Event for a reserve request when the funds reserve fails |
| settlementService.transactionRetry.fundRecovered | Event for a transaction retry when the funds are recovered successfully |
| settlementService.transactionRetry.fundReserved | Event for a transaction retry when the funds are reserved successfully |


##### Illustrating Model Parameters

This section covers the high-level specifications required for Generic Accounting Interface.

| S.No. | Parameters | Description |
|---|---|---|
| 1. | AC.ENTRY.PARAM | The processing rules related to Generic Accounting Interface (GAI) messages are described in the AC.ENTRY.PARAM application. Nonfinancial option in the Attribute field indicates the non-financial clearing messages and its respective responses updated in the AC.INWARD.ENTRY.NONFIN table. If this attribute is not set, all messages continue to update in existing way, that is, in the AC.INWARD.ENTRY table. |


> **Related Applications:** `AC.ENTRY.PARAM`, `AC.INWARD.ENTRY`, `CATEG.ENTRY`, `EB.SYSTEM.ID`, `EXTERNAL.SEPA.DETAILS`, `GENERIC.ACCOUNTING.REQUEST`, `MS.PARAMETER`, `RE.CONSOL.SPEC.ENTRY`, `STMT.ENTRY`

---


### 1.6  Charges


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

The charges levied on a multi-currency (MCY) account can be settled to:

- The base currency sub-account (under the MCY structure).
- Another account within the MCY structure.
- Another account (which is not under the MCY structure but within the Deposits TBC).


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


### 1.7  SubAccounts


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

Further, the arrangement account product for the sub-account should have the Product Only field set as ‘Mcy’ in the AA.PRODUCT.DESIGNER . This setup specifies that this product is for MCY sub-accounts only and it allows the bank to differentiate between the features of regular current, savings and MCY sub-accounts.


##### Automatic Creation of Base Currency Sub-Account

When the MCY arrangement is created, the system can be configured to create the base currency sub-account automatically. The automatic account creation can be configured by setting up the Base Ccy Product field in Sub-arrangement Rules condition of the MCY arrangement. The product should be a MCY only Product in AR product line. When the user gives this (Base Ccy Product) product in the Sub-arrangement of the MCY product configuration (or at MCY arrangement level), the base currency sub-account creates automatically in this product as part of MCY account creation.


> **Related Applications:** `AA.PRODUCT.DESIGNER`

---


### 1.8  Limit Balance


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

Limit Balances related feature is currently not available in TBC. The user can update the limit amount for an account in TBC using only secondary limits. Read here to read more on overdraft accounts in TBC.

---


### 1.9  Misc


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


### 1.10  Accounting in Deposits


> **📇 Quick Reference Card**
> 
> **Purpose:** *The AA Deposit module utilises the rule-based accounting framework to generate the accounting movements. The accounting functionality is used by all the financial products, and controls the link between the accounting events and allocation rules to be applied to these events. The adjustments in Inte...*
> 
> **Applications:** `AA.ACTIVITY`, `EB.CONTRACT.BALANCES`
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The AA Deposit module utilises the rule-based accounting framework to generate the accounting movements. The accounting functionality is used by all the financial products, and controls the link between the accounting events and allocation rules to be applied to these events. The adjustments in Interest and Charges Activities across accounting periods can be booked in a different Profit and Loss head, for better accounting. It is possible to report the Income and expense arising out of negative rates in a different Profit and Loss head. The system accounts for the charges collected or paid to the customer either in customer’s home branch or in the deposit-opening branch. The waivers or discounts in charges can be accounted separately or as a net entry.

The accounting related features and processing are handled by an external GL system for deposits in TBC.

When a transaction (that is, a withdrawal or funding or repayment) is posted to a deposit in TBC,

- The request is passed through the GAI (Generic Accounting Interface)
- An event is emitted which can be captured by the connected external GL system for the balance updates or accounting to be completed.

Read here to know more about TBC for deposits.


#### ⚙️ Configuration

In Deposits, the funds are settled using rule based accounting. The funding of deposits can be achieved using the Settlement and the Payment Rules Property Classes and payout of maturity proceeds from deposits uses the Settlement and Payout Rules Property Classes.

For transactions within the AA framework, soft accounting drives the accounting setup and the transaction codes for accounting entries. It is possible to have debit and credit transactions posted to the deposit using account-based applications, such as Teller or Funds Transfer. The transaction codes of the respective application is mapped with the AA.ACTIVITY in the Activity Mapping Property Class. Further accounting is based on the Activity triggered using the Payment or Payout Rules for payments made in and out of the deposit, respectively.


#### 🔧 Working With

The below illustration details the accounting in deposits.


##### Illustration

The account overview screen of a four-year deposit is shown below.

The Financial Summary section displays the commitment, live balance and the accrued interest information.

The Payment Schedule gives the principal, interest and charge schedules for the arrangement.

Any financial transaction is part of the activity log as seen below.

A sample screenshot of EB.CONTRACT.BALANCES is shown below.

The balances in the deposit can be viewed using the EB.CONTRACT.BALANCES.BALANCE enquiry.


##### Enquiries

Some of the standard enquiries used are as follows:

| Enquiries | Description |
|---|---|
| AA.DETAILS.ACCOUNT | Displays the Product, Account Number, Arrangement Date, Customer Name and Arrangement Status of an Arrangement |
| AA.DETAILS.ACTIVITY.LOG.FIN | Displays the activity log of an Arrangement |
| AA.DETAILS.ACTIVITY.LOG.FIN ARRANGEMENT.ID | Displays the financial activity log of an Arrangement |
| AA.DETAILS.ACTIVITY.LOG.FIN.HISTORY | Displays the financial activities log maintained in the history table such as Date, Activity, Type, Transaction Amount and Status of an Arrangement |
| AA.DETAILS.ACTIVITY.LOG.FINANCIAL.FIN | Displays the Activity Type, Status and Transaction Amount of an Arrangement |
| AA.DETAILS.ACTIVITY.LOG.USER.FIN | Displays the User Activities, Status, and Transaction Amount of an Arrangement |
| AA.DETAILS.ACTIVITY.LOG.PENDING.FIN | Displays the pending financial activities of an Arrangement |
| AA.DETAILS.ACTIVITY.LOG.SYSTEM.FIN | Displays the financial activity initiated by the system of an Arrangement |
| AA.DETAILS.ACTIVITY.LOG.TOTAL | Displays the total activity log details of an Arrangement |
| AA.DETAILS.ACTIVITY.LOG.USER.FIN | Displays the financial activities initiated by the user of an Arrangement |


#### 📋 Tasks

There are no tasks available for Accounting in Deposits feature.


#### 📊 Outputs

There are no Outputs available for Accounting in Deposits feature.


> **Related Applications:** `AA.ACTIVITY`, `EB.CONTRACT.BALANCES`

---


### 1.11  Cancel Period


> **📇 Quick Reference Card**
> 
> **Purpose:** *The bank can fund a deposit arrangement on a date that is different from the creation date and fund it partially.*
> 
> **Applications:** `AA.ACCOUNT.DETAILS`, `AA.PAYMENT.RULE.TYPE`, `AA.PRODUCT.DESIGNER`, `EB.ADVICES`
> 
> **Key Fields:** *Advice*, *Application Type*, *Bill Type*, *Cancel Date*, *Cancel Period*, *Payment Method*, *Pre Notice Activity*, *Pre Notice Days*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The bank can fund a deposit arrangement on a date that is different from the creation date and fund it partially.

The bank waits for the agreed period for the full funding of the deposit arrangement. The bank can choose to,

- Close the arrangement when not funded or only partially funded.
- Close the arrangement and give back the proceeds to the customer when partially funded.

This period can be configured at product level, so that the Cancel Activity is scheduled and triggered automatically if the deposit arrangement is not funded or partially funded.

There are no specific limitations with regards to the cancel period functionality for deposits in TBC.


#### ⚙️ Configuration

The Cancel Period field, in the Term Amount Property Class, is a generic attribute across the Deposits and Lending Product Lines. The period set in this field denotes the number of days from the arrangement creation date, after which the bank can trigger cancellation of the arrangement.

At the time of creation of the deposit arrangement, the system schedules the DEPOSITS-CANCEL-ARRANGEMENT, after the expiry of the value set in the Cancel Period field in the Term Amount Property Condition.

After expiry of the cancellation period, the system triggers the cancellation of the arrangement, if it is not funded or it is partially funded. If the account is not fully funded, within the cancel period, the system reverses any accrued interest.

In case of partial funding, the deposit can be closed after paying out the deposit amount to the customer account:

- As part of the cancellation activity, the deposit amount is reversed and credited to the UNC balances. That is, the system moves the funds available in the CUR to the UNC balance, after the Cancellation Activity and the arrangement moves to Cancelled status. The amount in the UNC balance must be paid out to close the deposit. For this, the user must initiate a payout transaction which triggers a DEPOSITS-APPLYPAYMENT- activity where the Payout Rule condition is configured with the Application Type set as PAY and only ACCOUNT property in the sequence. The AA.PAYMENT.RULE.TYPE configuration for the PAY record must have Payment Rule Type set to Pay in Advance, Payment Method set as Pay and Bill Type set to Payment. The below screenshot shows the Payout rule configuration required to pay out the UNC balance to the customer.

Once the amount is fully paid out from the UNC balance, the status of the deposit moves to Pending Closure and the system schedules the Close Arrangement activity for the deposit based on the Closure condition setup.

If the deposit arrangement is not fully funded, a pre-notification message can be generated in advance to indicate the impending cancellation of the arrangement.

The Pre Notice Activity field controls the DEPOSITS-CANCEL-ARRANGEMENT Activity by generating the pre-notification message. The system generates the alert message based on the value available in the Pre Notice Days field.

In the TBC, the pre-notifications are not applicable and, if required, they should be handled by external solutions.


#### 🔧 Working With

The Cancel Period field is available in Term Amount Property Condition. This is a generic field, which can also be used for other Product Lines.

The user can update the Cancel Period field in the below formats:

- Days (calendar) (nnnnD)
- Weeks (nnnnW)
- Months (nnnnM)
- Years (nnY)

Once a deposit arrangement is created, the system updates the Cancel Date field for the arrangement, based on the value in the Cancel Period field.

The system schedules the Cancel Activity, based on the value in the Cancel Period field. At close of business on the cancel date, the system compares the Expected balance and the CUR balance in the deposit arrangement. If the EXP balance is not equal to zero, then the system triggers the cancellation process.

The below screenshot displays the bill for deposit arrangement.

Cancel Period can be amended or removed after the initial creation of an arrangement through Change Term and Renegotiate Arrangement Activities, when the Cancel Period attribute is set as Negotiable and Accounting Mode in Interest Property Class is not set as Advance or Upfront Profit.

When the Cancel Period value is amended, the system calculates the Cancel Period End Date and stores the value in AA.ACCOUNT.DETAILS table. If the Cancel Period value is removed, then no Cancel Period End Date is stored in the table or displayed in the arrangement. Also, it removes or updates any scheduled activity for cancelling the arrangement.


##### Notification of Pending Cancellation of an Arrangement

The user can set the number of days, before the cancellation date, where a pre-notification advice is generated and sent to the customer.

A workflow example is shown below for Deposits. The same process can also be used for the other Product Lines.

The screenshot below displays the EB.ADVICES record and orients the user to attach to the Advice field (which is the Activity Messaging Condition field).

The Activity Messaging Product Condition specifies the pre-notification activity and the specific number of days before the cancellation period by when the pre-notification advice can be sent. These activities are then included in the AA.PRODUCT.DESIGNER .

The below screenshot displays the Activity Messaging Product Conditions.

The below screenshot displays the scheduled Activity of pre-notification and cancellation of arrangement.

In the TBC, the pre-notifications are not applicable and, if required, they should be handled by external solutions.


#### 📋 Tasks

Related topics:

- Open Deposit (AA)

The bank waits for the agreed period for the full funding of the deposit arrangement. The bank can choose to,

- Close the arrangement when not funded or only partially funded.
- Close the arrangement and give back the proceeds to the customer when partially funded.


##### Workflow

This section allows the user to perform the below activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Product Catalog . |
| Product Catalogue | Click the New Arrangement icon corresponding to Fully Negotiable deposit. |
| New Arrangement | Enter values in the following fields: Customer Currency Effective Date Click the Validate icon. Click the Commitment tab and then enter values in the following fields: Amount Term Cancel Period Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to Cancel Period in the core banking system.


##### Enquiries and Reports

NA


##### SWIFT Messages

NA


##### Advices

The below list of advices are generated by the core banking system pertaining to Cancel Period.

This advice specifies the details to customer as a Pre-notification for the cancellation of deposit on account of non-funding or partial funding .


##### Alerts

NA


> **Related Applications:** `AA.ACCOUNT.DETAILS`, `AA.PAYMENT.RULE.TYPE`, `AA.PRODUCT.DESIGNER`, `EB.ADVICES`

---


### 1.12  Charges


> **📇 Quick Reference Card**
> 
> **Purpose:** *The banks have the option to levy charges for opening a deposit account or on the individual transaction or activities triggered by the customer. The activities such as creation of a new deposit arrangement fee, any specific customer request (request for change of interest rate), etc., attract charg...*
> 
> **Key Fields:** *Arrangement*, *Flat Charge*, *GB Narrative*
> 
> **Sections:** 📖 Introduction | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The banks have the option to levy charges for opening a deposit account or on the individual transaction or activities triggered by the customer. The activities such as creation of a new deposit arrangement fee, any specific customer request (request for change of interest rate), etc., attract charges. These are due charges that are collected from the customer. There are charges which may be payable to the customer such as bonus, in case the deposit is not pre-closed for the full period, the bank may provide additional interest of 1 % as bonus on the deposit amount.

The banks may choose to amortise due or capitalise charges over a period, to spread the cost of expenses or income over a period. Though the charges levied on deposit products are less than that of the loan products, the accounting process remains the same for both deposit and lending.

There are no specific limitations for processing of deposit charges in TBC.

In TBC, the accounting related features and processing are handled by an external GL system for deposits. Therefore, to complete the accounting related to deposit charges, the TBC generates an event which can be captured by the connected external GL (General Ledger) system.


#### 📋 Tasks

Related topics:

- Open Deposit (AA)

Banks have the option to levy charges for opening a deposit account or on the individual transaction or activities triggered by the customer. The activities, such as, creation of a new deposit arrangement fee, any specific customer request (request for change of interest rate), Early redemption fee and so on, attract charges.


##### Workflow

This section allows the user to perform the below activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Find Deposit Arrangements | Enter an account arrangement ID in the Arrangement field and then click the FIND button. Click the Overview icon corresponding to a record. |
| Arrangement Overview (Deposit) | Click the New Activity option. |
| New Activities | Click the Do Activity Today icon corresponding to Change Redemption Fee Condition (User) activity. |
| Arrangement Activity | Enter a value in the GB Narrative field. Click the Validate icon. Click the Early Redemption Fee section and then click the Calculation tab. Enter a value in the Flat Charge field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

There are no Outputs available for Charges feature.

---


### 1.13  Cooling Period


> **📇 Quick Reference Card**
> 
> **Purpose:** *In certain cases, if the customer prefers to redeem their deposit within a certain period from deposit opening date (usually within a few days of deposit), then the bank may not charge any penalties as a normal pre-closure of the deposit would attract. This is an option to the customer and the depos...*
> 
> **Applications:** `AA.ACCOUNT.DETAILS`, `AA.PERIODIC.ATTRIBUTE`
> 
> **Key Fields:** *Base Date Type*, *Cooling Convention*, *Cooling Date*, *Cooling Date Adj*, *Cooling Period*, *Cooling Waive Class*, *Cooling Waive Prop*, *Rule Start* ... +3 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

In certain cases, if the customer prefers to redeem their deposit within a certain period from deposit opening date (usually within a few days of deposit), then the bank may not charge any penalties as a normal pre-closure of the deposit would attract. This is an option to the customer and the deposit arrangement does not get any interest for the pre-closed term deposit as well. This is a facility extended to the customer and the customer is required to initiate closure proceeding.

There are no specific limitations with regards to the cooling period functionality for deposits in TBC.


#### ⚙️ Configuration

In some countries, regulatory requirements mandate that a customer should be allowed to close the arrangement, within a stipulated time after the deposit start date, without any charges or request to waive any accrued interest for that period. This time is called the cooling period.

At any point of time, during the tenure of the deposit, a term deposit can be pre-closed. The banks levy pre-closure charges or pay lesser interest for such early withdrawals. Charges are automatically levied using the Activity Restriction Property Class.

The bank allows the customer to withdraw the deposit within a specified period (Cooling Period) without levying any charges to the deposit arrangement. If the customer withdraws the entire deposit amount within the cooling period, then the bank does not have to pay any interest on the deposit, for the period it remained with the bank. In this case, any charges collected during the cooling period are also reversed.

There may be cases where the bank defines the interest payment schedule and processes before the expiry of the cooling period. Any interest or principal amounts, already paid from the deposit arrangement within the cooling period, are not included in the redemption calculation and the amount already paid is not reversed. An override is populated at the arrangement level, if a schedule is configured within the cooling period and at the funds transfer stage to notify the user.

Banks can configure the cooling period using the Term Amount or the Closure property class.

Using the Cooling Period attribute in the Term Amount property class, banks can calculate the cooling date based on the calendar days. The user can close a deposit arrangement within this cooling date, without any pre-closure charges, and banks do not have to pay any interest to the customer.

Banks can configure the cooling period attributes such as Cooling Period , Cooling Date Adj , Cooling Convention , Waive Class , Waive Prop , and Waive Bill Type , using the Closure property class.

The advantages of using the Cooling Period attributes, in the Closure property class, are the following:

- Banks have the option to specify property class or property (Interest or Charge) for which waiver or refund is to be done.
- Banks can calculate the cooling period on working days instead of calendar days using the Cooling Convention attribute.
- The Cooling Date Adj attribute allows the bank to adjust the cooling date to the next working day if the cooling date falls on holiday.

> **⚠️ Note:** It is recommended to configure cooling period attributes in the Closure property class, as it has enriched functionality, compared to the cooling period configuration in the Term Amount property class.

The cooling off period is applicable for rollovers only if the Base Date Type field is set to Agreement in the Account property class. The customer can withdraw the money after rollover, within the defined cooling period. In this case, no interest is paid for the deposit from the date of rollover.

When a term deposit is pre-closed, within the cooling period, only the Current Balance (CUR ) can be considered and not the interest that is already paid to the customer. Any PAY balances available in the deposit arrangement are not reversed at the time of pre-closure, but the accruals from last make-due date are reversed at the time of pre-closure.


##### Product Condition - Term Amount

For a deposit, the Cooling Period field in the Term Amount Product Condition is set to seven days. This allows the customer to pre-close or withdraw the arrangement within this period of seven days.


##### Product Condition - Closure

The Closure property class defines the Cooling Period attributes for the deposit product.

- The Cooling Period attribute is defined as the number of days from the deposit creation date within which the deposit can be closed without any charges and accrued interest can be waived
- If the cooling period date falls on a holiday, configuring the Cooling Date Adj attribute as ‘Forward’ adjusts the cooling period date to the next working day.
- The user can configure the Cooling Convention attribute as ‘Working Days’ to calculate the cooling period in working days. If the user selects the Null option, the system calculates the cooling period based on the calendar days.
- Property class level or property level choices are available for waiving or retaining the charge or interest applied during the cooling period using the Waive Class , Waive Prop and Waive Bill Type attributes.
- The user should configure the Waive Bill Type as Current if interest property class or property is selected All if charge property class or property is selected

Refer to the Closure section for more information.

- Only the current interest (accrued) can be waived. The interest that is already paid or capitalized cannot be waived or refunded.
- Due or Pay charges can be waived or refunded only at the time of redemption and the same needs to be settled.
- Capitalized Charges (Debit or Credit) cannot be waived or refunded.
- The Cooling Period attribute in the Term Amount property class is mutually exclusive of the Cooling Period attribute in the Closure property class. If found in both places, the system raises an error at the proofing stage.

In the AA.PERIODIC.ATTRIBUTE , the Rule Start field, when set as Cooling-off, decides the start date from which the periodic restriction is to be applied. If Cooling-off is opted, then the periodic restriction can start from the date of Cooling Date as specified in the AA.ACCOUNT.DETAILS .


#### 🔧 Working With

This section orients the user to create cooling period.


##### Creation of the Cooling Period

Banks can define the cooling period either in the Term Amount or the Closure property class. If defined in both the places, then the system raises an error at the proofing stage.

The Term Amount Property Class has the Cooling Period field where the user defines the period within which the customer can withdraw the deposit amount without interest and charges for the arrangement.

The Closure property class has the cooling period attributes such as Cooling Period , Cooling Date Adj , Cooling Convention Waive Class , Waive Prop , and Waive Bill Type where the user defines the period and property class or property for which waiver or refund is to be applied in case if the deposit is to be closed within cooling date.


##### Cooling Period using Term Amount

Consider a deposit product with a cooling period defined as seven days using the Term Amount property class. When an arrangement is created on 15 Apr, 2022, the system calculates the cooling date by considering the seven calendar days. Hence, the cooling date for the arrangement is 22 Apr, 2022. The user can check if the Cooling Date field is updated in AA.ACCOUNT.DETAILS table to confirm the end date of the cooling period.

At the time of closure, the arrangement has the accrued interest as 9.30. If the arrangement is closed on 19 Apr, 2002, that is, before the cooling date, the accrued interest is waived.

The ECB before the closure is displayed in the screenshot below.

The ECB after the closure is displayed in the screenshot below.


##### Cooling Period using Closure

The cooling period allows the user to close a deposit within a stipulated time after the deposit start date. The stipulated time is defined as the number of calendar days in the Closure property class.

When customer chooses to close or cancel the deposit within the cooling period, the interest and charges are handled based on the parameter defined in the Closure property class.

The Cooling Period can also be defined in the Term Amount property class. The Term Amount property class does not provide the interest and charges option to the users.

The Closure product condition is defined as shown in the screenshot below for a deposit product. The Cooling Period is defined for seven days. The Interest property class is defined in the Cooling Waive Class field. Only the MAINTENENACEFEES property is specified in the Cooling Waive Prop field.

The below image shows that the arrangement is created on 15 Apr, 2022 and the cooling date for the arrangement is 22 Apr, 2022.

At the time of arrangement creation, the below charges are raised and the same has been collected.

- MAINTENANCEFEES – 100 USD (Debit charge raised and settled on 15 Apr, 2022)
- DEPOPENINGFEE – 250 USD (Debit charge raised and settled on 15 Apr, 2022)

At the time of closure, the deposit has below balances.

- Deposit balance – 40,000 USD
- Accrued Interest – 11.88 USD

When a deposit is closed before the cooling date, the accrued interest portion is waived (The Interest property class is specified in closure product condition) and, only the MAINTENANCEFEES charge is refunded. Other charges, if any incurred, are not waived or refunded during closure since only the MAINTENANCEFEES property is specified in closure product condition.

Deposit redemption is triggered before the cooling date. During the closure, the system performs the following.

- Deposit balance – Paid to customer
- DEPOPENINGFEE – Debit charge collected from customer is not refunded
- MAINTENANCEFEES – Refunded to customer by creating equivalent PAY bill (Since MAINTENANCEFEES property is configured in Closure condition for waiver)
- Accrued Interest – Reversed to the Banks PL account (Since Interest property class is configured in Closure condition for waiver)

In this case, the system pays back to the customer 41,000 USD (40,000 – Deposit balance + 100 – MAINTENANCEFEES).


#### 📋 Tasks

Related topics:

- Perform Pre-Closure of Deposit (AA)

The bank allows the customer to withdraw the deposit within a specified period (Cooling Period) without levying any charges to the deposit arrangement. If the customer withdraws the entire deposit amount within the cooling period, then the bank does not have to pay any interest on the deposit for the period it remained with the bank. In this case, any charges collected during the cooling period is also reversed.


##### Workflow

This section allows the user to perform the below activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Product Catalog . |
| Product Catalogue | Click the New Arrangement icon corresponding to Fully Negotiable deposit. |
| New Arrangement | Enter values in the following fields: Customer Currency Effective Date Click the Validate icon. Click the Commitment tab and then enter values in the following fields: Amount Term Cooling Period Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

There are no Outputs available for Cooling Period feature.


> **Related Applications:** `AA.ACCOUNT.DETAILS`, `AA.PERIODIC.ATTRIBUTE`

---


### 1.14  Customer Ownership and Eligibility


> **📇 Quick Reference Card**
> 
> **Purpose:** *Banks offer Term Deposit accounts to their customers. There can be a single or multiple owners for a deposit account and in case of multiple owners, there is one primary beneficial owner.*
> 
> **Applications:** `AA.ARR.CUSTOMER`, `AA.ARR.OFFICER`
> 
> **Key Fields:** *Arrangement*, *Beneficial Owner*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Banks offer Term Deposit accounts to their customers. There can be a single or multiple owners for a deposit account and in case of multiple owners, there is one primary beneficial owner.

Apart from being the owner of a deposit account, the customers related to the deposit account can have different roles. During the tenure of the deposit, it is possible to amend the customers related to the arrangement and their roles.

Banks can set eligibility on their deposit products that is evaluated when the deposit is created. For example, age validation of the customer at the time of opening a senior citizen deposit product.

In the TBC, it is possible to define that certain deposit products require meeting the configured eligibility criteria. The eligibility of the customer for a deposit, can be defined and evaluated at the Enterprise layer, that is TEP (Temenos Enterprise Pricing).


#### ⚙️ Configuration

At the time of account creation, it is mandatory for the user to enter at least one customer as the owner of the arrangement. If there is only one customer, then the role is automatically set to the Beneficial Owner.

Once the deposit arrangement is committed, the customer details are automatically set to the Customer Property Condition of the deposit arrangement. The customer details are stored in the AA.ARR.CUSTOMER record for the particular deposit arrangement. The system enables the user to add a customer and corresponding roles of a deposit arrangement using the Change Customer Activity.

The information related to customers and other parties in a deposit must be existing entries in the Party TBC. The system evaluates this customer information against the records found in this system. Also, in the TBC, the Change Customer Activity can be executed through the use of the respective API.


##### Eligibility

A customer’s eligibility for a particular deposit arrangement product is checked at the time of account creation. The eligibility rules can be defined based on customer attributes, such as age, business or occupation, residence, etc. There can be multiple eligibility conditions for a particular product.

The rules are set at product level and are validated at the time of creation and at periodic intervals, or when there is a change in customer details. The system validates these rules for all customers related to the deposit arrangement.

Whenever there is a rollover of deposit arrangement and the user has defined change product, the system checks if all the customers satisfy the eligibility rules defined for the new product. If the rules are not satisfied during the eligibility review process, the arrangement moves to the default product as per the configuration.

The eligibility of the customer for a deposit can be defined and evaluated at the Enterprise layer, that is TEP (Temenos Enterprise Pricing).


##### Account Officer

The system defaults the Account Officer responsible for the deposit arrangement relationship at product level and can be amended at the arrangement level, if allowed. Details of the account officer related to the deposit arrangement are available in AA.ARR.OFFICER record of the arrangement.


#### 🔧 Working With

This topic enables the user to perform multiple actions in a deposit arrangement.


##### Owner

The owner is specified in the Beneficial Owner field for the deposit arrangement. There can be multiple customers with different roles. Each customer should have a specified role and the role defined should be a valid record in the AA.CUSTOMER.ROLE table. The customer roles can be joint owner, power of attorney, guarantor, etc. and each role describes the responsibilities and rights of the customer in the arrangement.

The Retail Deposits system allows the user to:

- Add or remove a customer to the deposit ownership.
- Modify the customer details related to the arrangement, using the Change Customer Activity.
- Change the role of the customer already related to the arrangement.
- Update details of the customer already related to the deposit arrangement, using the Update Customer Activity.

The information related to customers and other parties should be existing entries in Party TBC. The system evaluates this customer information against the records found in this system.

When the customer of a deposit is changed in the TBC, the eligibility of the customer for that deposit product is evaluated at the Enterprise layer, for example, TEP (Temenos Enterprise Pricing).


##### Eligibility

To check the eligibility of a customer requesting a particular deposit product, rules are set up to validate the conditions at the time of creation of deposit arrangement. If a deposit product is eligible only for a customer over 18 years, then the system validates the customer’s date of birth in the customer’s record with the system's accounting date and provides the customers’ eligibility for the product.

Read the Eligibility Property Class user guide for further information.

The bank can form different rules to validate several conditions for various deposit products, such as the occupation of the customer, residence, portfolio with the bank. The eligibility conditions can be complex if the bank requires so, such as checking the age, nationality, net worth, and duration of relationship with the bank to arrive at a decision, can be created as rule for eligibility validation.

The eligibility of the customer for a deposit can be defined and evaluated at the Enterprise layer, for example, the product management like TEP (Temenos Enterprise Pricing).


##### Account Officer

The system allows the addition of an account officer who is responsible for the deposit arrangement relationship at the time of creation. In addition, it is possible to amend the officer information related to the deposit arrangement using the Deposits Update Officer Activity.


#### 📋 Tasks

Related topics:

- Open Deposit (AA)

The system enables the user to add a customer and corresponding roles of a deposit arrangement using the Change Customer Activity.


##### Workflow

This section allows the user to perform the below activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Find Deposit Arrangements | Enter an account arrangement ID in the Arrangement field and then click the FIND button. Click the Overview icon corresponding to a record. |
| Arrangement Overview (Deposit) | Click the New Activity option. |
| New Activities | Click the Do Activity Today icon corresponding to the Change Customer activity. |
| Arrangement Activity | Enter values in the following fields: Customer Effective Date Click the Validate icon. Click the Customer section and then enter values in the following fields: Tax Liab% GL Alloc% Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

There are no Outputs available for Customer, Ownership and Eligibility feature.


> **Related Applications:** `AA.ARR.CUSTOMER`, `AA.ARR.OFFICER`

---


### 1.15  Deposit Closure


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Deposit Account Arrangement is closed by the system when,*
> 
> **Applications:** `AA.ARRANGEMENT`, `AA.CUSTOMER.ARRANGEMENT`, `AA.CUSTOMER.ARRANGEMENT.HIST`, `AA.CUSTOMER.ARRANGMENT.HIST`, `ACCOUNT.CLOSURE`
> 
> **Key Fields:** *Active Y/N*, *Arrangement*, *Arrangement Id*, *Arrangement Status*, *Balance Type*, *Closure Method*, *Closure Notes*, *Closure Period* ... +17 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The Deposit Account Arrangement is closed by the system when,

- The customer redeems the deposit.
- The balance amount available is settled to the customer.
- There are no other outstanding balances.

The closure process of the Close Activity, of a specific deposit arrangement, can be triggered manually by the user or automatically by the system, when all the balances of the arrangement become zero or when the arrangement matures, provided all the balances are settled to the customer. The automatic triggering can be scheduled after a specific period, mentioned in the Closure Property Condition.

There are no specific differences for closure of deposits in the TBC. When a deposit is closed, the deposit proceeds can be settled to an account within the TBC. If the account or beneficiary is outside the TBC, the system forwards a settlement request to the account or beneficiary, by publishing an event, which should be consumed by an external payments system for further processing.


#### ⚙️ Configuration

The automatic closure is defined in the Closure Type field, which allows the following values.

- Balance -If this value is selected, the account is closed on the same day the account's balance becomes zero.
- Maturity - If this value is selected, when all balances are settled to the customer, the Arrangement Status field is updated to PENDING.CLOSURE and the Account Closure Activity is scheduled on the date of maturity of the arrangement.
- None - This value can be selected, only when the Closure Method field is set to Manual.

The Closure Period field defines the period, after which an arrangement will be closed, once it is identified as ready for closure, based on the above-mentioned configuration. The system schedules the Closure Activity, based on the period indicated in the field.

The Closure Type field has to be set as either Maturity or Balance. In case of using the Manual closure method, the user triggers the Closure Activity manually.

The bank restricts all transactions into the account, once the account is marked for closure. This is mentioned in the Posting Restrict field, with a value in the range of 90–99.


#### 🔧 Working With

This section orients the user to initiate deposit closure.

In the below scenario, the

field is set to AUTOMATIC with the

field as Maturity and the

as 20 days.

After all the balances are settled well before maturity, the Arrangement Status field is updated to PENDING.CLOSURE in the AA.ARRANGEMENT record as shown in the below screenshot.

On maturity, the arrangement status is updated as CLOSE.

Now the ACCOUNT.CLOSURE record is created with the Posting Restriction field set to 90.


##### Closed Arrangements

The AA.CUSTOMER.ARRANGEMENT.HIST table maintains the records of closed arrangements with attributes similar to AA.CUSTOMER.ARRANGEMENT table.

Upon closure of an account, the arrangement records are moved from AA.CUSTOMER.ARRANGEMENT table to the AA.CUSTOMER.ARRANGEMENT.HIST table.

All the closed arrangements are available in the AA.CUSTOMER.ARRANGMENT.HIST table.

> **⚠️ Note:** During history restoration, the records are moved from the AA.CUSTOMER.ARRANGEMENT.HIST table to the AA.CUSTOMER.ARRANGEMENT table.


#### 📋 Tasks

Related topics:

- Perform Pre-Closure of Deposit (AA)
- Account and Deposit Processes (Retail)

The Deposit module provides deposits functionality for Core Banking. This module allows the user to perform various deposit related activity such as, update the settlement, partial withdrawal, and so on.


##### Workflow

This section allows the user to view the below list of tasks:

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Find Deposit Arrangements | Enter the required field values and click the FIND button. |
| AA Arrangement | Click the Overview icon. |
| Arrangement Overview (Deposits) | Click the New Activity option. |
| New Activities | Click the Do Activity Today icon corresponding to the Update Settlement Instructions activity. |
| Arrangement Activity | Enter a value in the Narrative field. Click the Settlement Instruction section to expand. In the Initial Funding, Charges Settlement screen, enter values in the following fields: Active Y/N Settlement A/c In the Interest & Redemption Settlement screen, enter values in the following fields: Active Y/N Settlement A/c Click the Validate icon to check for errors and overrides. Click the Commit icon. Accept the overrides, if any. |

This option is used to repay the pay balances from Deposits Arrangement. Repayment can be done through cash or funds transfer. It is used when settlement account for pay-out is not provided in the Deposit Arrangement.

To repay a Deposit, follow the below steps:

1. AA Pay-out .
2. Enter values for the following fields: Arrangement Id Debit Value Date Debit Currency Debit Amount Credit Account Credit Value Date Credit Amount Treasury Rate Customer Spread Customer Rate
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon.

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Find Deposit Arrangements | Enter a value in the Arrangement field and click the FIND button. |
| AA Arrangement | Click the Overview icon. |
| Arrangement Overview (Deposits) | Click the Run icon corresponding to Redeem Deposit activity . |
| Redeem Deposit | Enter values in the following fields: Closure Reason Redemption Date Closure Notes Click the Validate icon to check for errors and overrides. Click the Commit icon. Run the BNK/AA.SIMULATION.SERVICE simulation service . |
| Arrangement Overview (Deposits) | Click the Redemption Statement icon. |
| Redemption Statements | Click the Redemption Statement Details icon. Click the Redeem Deposit icon. Enter values in the following fields: Closure Reason GB Closure Notes Click the Validate icon to check for errors and overrides. Click the Settlement Instruction section to expand. In the Initial Funding, Charges Settlement screen, enter values in the following fields: Active Y/N Settlement A/c In the Interest & Redemption Settlement, enter values in the following fields: Active Y/N Settlement A/c Click the Validate icon to check for errors and overrides. Click the Commit icon. Accept the overrides, if any. |


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to Deposit Closure in the core banking system.


##### Enquiries and Reports

This section allows the user to view the below list of enquiries and reports:

Mature in 7 days

This enquiry displays the details of deposits that are maturing in the next seven days. The user can view the Deposits Overview screen from this enquiry by clicking the Over View icon.


##### SWIFT Messages

NA


##### Advices

The below list of advices are generated by the core banking system pertaining to Deposit Closure.

This advice specifies the details such as, Customer details, Account details and Repayment details.


##### Alerts

NA


> **Related Applications:** `AA.ARRANGEMENT`, `AA.CUSTOMER.ARRANGEMENT`, `AA.CUSTOMER.ARRANGEMENT.HIST`, `AA.CUSTOMER.ARRANGMENT.HIST`, `ACCOUNT.CLOSURE`

---


### 1.16  Deposit Creation


> **📇 Quick Reference Card**
> 
> **Purpose:** *The banks offer Term Deposit accounts for its customers to encourage investments. These accounts can be in any currency. Typically, a deposit arrangement has a fixed tenure but it is possible to create call deposits, which does not require the user to define the term period or notice deposits, where...*
> 
> **Applications:** `AA.PRODUCT`
> 
> **Key Fields:** *Alt Id*, *Alternate ID*, *Amount*, *Arrangement*, *Currency*, *Customer*, *Linked Appl*, *Linked Appl Id* ... +3 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The banks offer Term Deposit accounts for its customers to encourage investments. These accounts can be in any currency. Typically, a deposit arrangement has a fixed tenure but it is possible to create call deposits, which does not require the user to define the term period or notice deposits, where a notice should be given before making a withdrawal.

Term deposits accounts can have single or multiple owners. The system generates the deposit account number, which the customer can use as reference number for transactions, using channels.

When the user tries to create a deposit from the front-end, the system triggers the corresponding activity in the TBC to complete the deposit creation process. The deposit for the customer is opened in one of the products selected from the list of products available.

There are no specific limitations for creating and handling different types of deposits (such as term deposits, call deposits, and so on) in the TBC.


#### ⚙️ Configuration

To create a deposit arrangement, the user requires customer information along with Product information and the currency of the arrangement. The user assigns a reference number for the deposit arrangement. Every arrangement has an underlying account associated with it. The deposit arrangement’s corresponding account number is updated in Linked Appl Id with Linked Appl as ACCOUNT.

The user can create deposit arrangements using the below products:

| Column 1 | Column 2 |
|---|---|
| Savings Account Plan | Term Deposits Plan |
| Customer deposits a specific amount in regular intervals for a particular period. Such savings plan arrangements can be created for recurring dates (usually monthly intervals) of deposits for purpose of saving. AA supports Recurring deposits or Saving Plan products. | Customers can deposit a fixed amount for a specific period using deposit products to earn a specific interest. The interest earned can be paid on regular intervals or capitalised to arrangement and paid at maturity. It is possible to automatically renew the deposits on maturity. |

The user adds or modifies the following details when creating deposit arrangements:

| Column 1 | Column 2 | Column 3 | Column 4 | Column 5 |
|---|---|---|---|---|
| Customer | Eligibility | Agent | Preferential Pricing | Alternate Account ID |
| Deposit owner is the beneficial owner of the deposit arrangement account. There can be multiple owners to deposit accounts at the time of deposit account opening. The system can add and maintain joint owners at any time during the entire tenure of the deposit. It is mandatory to assign customer roles when there are more than one owner. | Banks can configure to validate the customer’s eligibility for availing a deposit product at the time of opening of the term deposit. Read the Eligibility Property Class user guide for more information. | As a business practice, banks may have prior agreements with agents to source deposit accounts. At the time of creation of these deposits, the user can enter the agent information. The bank pays the agent either full commission, when there is full funding of the deposit or periodic commission, as and when interest is paid to the deposit customer. However, this is not a mandatory detail required for creation of deposit arrangement. Read the Agent user guide for more details. | Pricing is not mandatory for creating a deposit arrangement, but a Pricing Plan adds value to the deposit. It provisions better interest and charge application to the customer based on the relationship arrangements. If the pricing option is set to Automatic, then the system automatically determines the ideal pricing plan for the customer. If it is set to Manual, then the system manually updates the pricing plan. Read the Preferential Pricing user guide for more information. | The Alt Id field on the Account Property Class Condition displays the updated system ID for deposit accounts migrated from legacy systems or taken over from another system. The value in this field is used as an identifier and the user can use the alternate system ID for enquiry purpose. |

- The information related to customers and other parties in a deposit can be input from an external system such as Party TBC. The system evaluates this customer information against the records found in the external system.
- For a deposit in TBC, the eligibility criteria and the preferential pricing options can be defined and evaluated at the Enterprise layer such as TEP (Temenos Enterprise Pricing).
- The Agent Commission property class and its related functionality are not applicable for deposits in TBC. The TBC generates an event when the deposit is funded fully, or the interest is paid to the customer. These events can be consumed by external systems for further processing (such as payment of commission to an agent) as per the bank’s requirement.


#### 🔧 Working With

This topic enables the user to create deposit arrangements.


##### Activity for Deposit Arrangement Creation

The DEPOSITS-NEW-ARRANGEMENT Activity is triggered to create a new deposit arrangement. To create a new arrangement, the system requires the user to enter information on the below details:

| Column 1 | Column 2 | Column 3 | Column 4 |
|---|---|---|---|
| Customer | Product | Currency | Effective Date |
| The user can input details of multiple customers with different roles. Read the Customer Property Class user guide for more information. | The user must ensure to enter a valid record name in AA.PRODUCT record and available for the corresponding company or branch. | The user must ensure to validate the currency entered for the deposit arrangement with the existing currencies of the product, as the system allows the user to create the deposit arrangement. Only if the product is available in the particular currency then the system allows the creation of the deposit arrangement. | The effective date for creation of a deposit can be the current system date, back date or a future date. |

In addition, the user can provide the pricing options when creating the new deposit arrangement.

To create a new deposit arrangement,

1. Retail Operations and click Product Catalog .
2. In the Term Deposits section, click of the corresponding Product.
3. Enter the customer information along with currency, agent, and pricing details.
4. Validate the initial creation of the arrangement.
5. Commit and authorise the deposit arrangement.

When the user tries to create a deposit from the front end and the API to the TBC is called, the system triggers the corresponding activity in the TBC to complete the deposit creation process. The above-mentioned (points 1-5) are not applicable to the TBC.

- The deposit for the customer is opened in one of the products selected from the list of products available.
- The customer related information in a deposit can be input from an external system such as Party TBC. The system evaluates this customer information against the records found in the external system.
- The currency in which the deposit is opened is evaluated against the list of currencies in which the product is available. It is to be noted that the currency details can be evaluated from an external system like Market or Reference Data TBC.
- The pricing options for a deposit in TBC can be defined and evaluated at the Enterprise layer such as TEP (Temenos Enterprise Pricing).

The Agent Commission property class and its related functionality are not applicable for deposits in the TBC. The TBC generates an event when the deposit is funded fully, or the interest is paid to the customer. These events can be consumed by external systems for further processing (such as payment of commission to an agent) as per the bank’s requirement.


#### 📋 Tasks

Related topics:

- Amend Deposit (AA)
- Core Banking Open Deposit (AA)
- Account and Deposit Processes (Retail)

The Deposit Arrangement administration can be performed by triggering various activities in a Deposit Arrangement through which various conditions can be updated as per the requirement.


##### Workflow

In Deposit Creation, the user can open the following types of Deposit Arrangements.

| SCREENS | WORKFLOW |
|---|---|
|  | Product Catalog . |
| Product Catalogue | Click the New Arrangement icon corresponding to the product 3 Months Deposit. |
| AA Arrangement Activity | Enter values in the following fields: Customer Currency Click the Validate icon to check for errors and overrides. Click the Commitment section. Enter a value in the Amount field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Product Catalog . |
| Product Catalogue | Click the New Arrangement icon corresponding to the product Commitment Savings Plan. |
| AA Arrangement Activity | Enter values in the following fields: Customer Currency Click the Validate icon to check for errors and overrides. Click the Commitment section. Enter a value in the Amount field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Product Catalog . |
| Product Catalogue | Click the New Arrangement icon corresponding to the product 12 Months Deposit. |
| AA Arrangement Activity | Enter values in the following fields: Customer Currency Click the Validate icon to check for errors and overrides. Click the Commitment section. Enter a value in the Amount field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Find Deposit Arrangements | Enter a deposit arrangement ID in the Arrangement field. Click the FIND button. Click the Overview icon. |
| Arrangement Overview (Deposits) | Click the New Activity option. |
| New Activities | Click the Do Activity Today icon corresponding to the Update Account Details activity. |
| Arrangement Activity | Enter a value in the Narrative field. Click the Account section. Enter a value in the Alternate ID multi-value field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Find Deposit Arrangements | Enter a deposit arrangement ID in the Arrangement field. Click the FIND button. Click the Overview icon. |
| Arrangement Overview (Deposits) | Click the New Activity option. |
| New Activities | Click the Do Activity Today icon corresponding to the Change Commitment Term activity. |
| Arrangement Activity | Enter a value in the Reason field. Click the Commitment section. Enter a value in the Term field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to Deposit Creation in the core banking system.


##### Enquiries and Reports

The user can view the below list of enquiries and reports:

Deposit Overview

This screen has the different set of enquires displays the Account Dates, Arrangement details, Linked arrangements, Additional details and so on.


##### SWIFT Messages

NA


##### Advices

The below list of advices are generated by the core banking system pertaining to Deposit Creation.

This advice specifies the details such as, Account Number, Product, Amount, Start Date and Maturity Date for a new arrangement deposit.

This advice specifies the details such as, Account details, Customer details, Interest details and repayment schedule details.


##### Alerts

NA


> **Related Applications:** `AA.PRODUCT`

---


### 1.17  Deposit Simulation


> **📇 Quick Reference Card**
> 
> **Purpose:** *The simulation engine helps in ascertaining the actual results of certain activities such as creation of deposit, change of interest rate on a live deposit account and pre-closure of a term deposit without actually executing the transaction. Simulation provides results for the user to check and deci...*
> 
> **Applications:** `AA.ACTIVITY.HISTORY`, `AA.ACTIVITY.HISTORY.SIM`, `AA.ARR.CUSTOMER`, `AA.ARR.INTEREST`, `AA.ARRANGEMENT.ACTIVITY`, `AA.ARRANGEMENT.SIM`, `AA.SIM.CUSTOMER`, `AA.SIM.INTEREST` ... +6 more
> 
> **Key Fields:** *Auto Run*, *Calc Amount*, *Execute Simulation*, *Run Activity*, *Sim Currency*, *Sim Date*, *Sim End Date*, *Sim Reference* ... +3 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The simulation engine helps in ascertaining the actual results of certain activities such as creation of deposit, change of interest rate on a live deposit account and pre-closure of a term deposit without actually executing the transaction. Simulation provides results for the user to check and decide whether to proceed with actual execution of the transaction. It helps the customer understand the impact and decide whether to proceed with the particular activity.

The simulation of deposits in TBC are performed through the usage of the provided APIs.


#### ⚙️ Configuration

The simulation engine provides the method of running various combinations of activities in the system. The effective date for the simulation is set to the current accounting date or to a future date, to see the effect of these without having any impact on live data. This simulation helps the user and the customer to check for possible solutions like (but not limited to),

- New deposit illustrations
- Impact on change of interest on the deposit arrangement
- Partial withdrawal or pre-closure calculation

The Arrangement Architecture (AA) provides a simulation tool that helps the customer with the decision-making process, during the creation of deposit or at the time of pre-closure of a term deposit.

This tool enables the user for,

- Simulation of deposits for prospective and existing customers
- Viewing payment schedule for simulated deposits
- Making changes to existing arrangement due to specific dated activities

It is possible to convert the simulated deposits into live deposits. All the products within AA framework support simulation.

The simulation within AA requires the following sub-systems.

The simulation of deposits in TBC are performed through the usage of the provided APIs.


##### Simulation Data Capture

Simulation Data Capture captures the information in the AA.SIMULATION.CAPTURE application, which is similar to AA.ARRANGEMENT.ACTIVITY . This captures data as part of the simulation activity for new arrangements or simulations in live arrangements.


##### Simulation Runner

The information captured is first fed to the runner, which is supported by the AA.SIMULATION.RUNNER application. In this application, the user provides the arrangement ID of the simulation capture and the end date of the simulation. If no end date is given, then the maturity date of the arrangement is defaulted as end date.

- Run simulation for the captures is done with the help of service.
- The simulated arrangement can be used for information purpose or be converted to a live arrangement.

AA simulation performs all the activities, updates respective files and stores the details in separate tables.

Enquiries can be written to process the data in these files to provide a pleasing user interface.


##### Information Storage and Retrieval

Run the simulation using a service that stores information till the date specified by the user.


#### 🔧 Working With

This topic enables the user to perform multiple actions in a deposit arrangement.

The simulation of deposits in TBC are performed through the usage of the provided APIs.


##### Simulation Capture

The simulation capture process is similar to the process used when creating a new arrangement using the AA.ARRANGEMENT.ACTIVITY application.

Depending on the setup of the product, the Conditions are defaulted at the time of simulation and the conditions can be modified, if negotiable, to suit the simulation requirements. For example, modification of interest rate or maturity details of the contract and changes to forward dated conditions.

The AA.SIMULATION.CAPTURE application captures the defaulted and negotiated condition information. The captured information is stored in individual SIM files for each property such as AA.SIM.INTEREST , AA.SIM.CUSTOMER , and so on. These files are similar to live files such as AA.ARR.INTEREST , AA.ARR.CUSTOMER , and so on.

Other SIM files that are created as part of simulation are as follows:

- AA.ARRANGEMENT.SIM — Stores the arrangement details for the simulation.
- AA.SIMULATION.CAPTURE —Clones the AA.ARRANGEMENT.ACTIVITY to state the basic details. The Sim Reference field stores the customer simulation reference for future use.
- AA.ACTIVITY.HISTORY.SIM —Clones the AA.ACTIVITY.HISTORY that holds all the Activities captured through AA.SIMULATION.CAPTURE .


##### Amend Simulation Capture

The user can amend the simulation capture. The Update Prod Condition attribute in AA.SIMULATION.CAPTURE defines whether or not to refresh the property conditions in the simulation capture record using the latest product conditions.

Additionally, while amending the simulation capture, the effective date can be changed to the required date and the Update Prod Condition attribute can be defined to use the product condition or the SIM records for the new effective date.

If the effective date needs to be changed, the Auto Run attribute needs to be manually set to Simulate.

Read Amend Simulation Capture for more information.


##### Simulation Runner

The AA.SIMULATION.RUNNER application runs the simulation once the details are captured in the AA.SIMULATION.CAPTURE record.

Additional information are added to the Sim End Date , Sim Currency , Sim Run Date , Sim Date and the Sim Reference fields, which are added to the AA.SIMMULATION.RUNNER record.


##### Information Storage and Retrieval

Once the AA.SIMULATION.RUNNER record is authorised, the user can run the service for simulation in the AA.SIMULATION.SERVICE application. The service stores the required data to different files for retrieval later.

Few examples for $SIM files are as follows:

- FBNK.AA.BILL.DETAILS$SIM
- FBNK.AA.SCHEDULED.ACTIVITY$SIM
- FBNK.AA.ACCOUNT.DETAILS$SIM
- FBNK.AA.INTEREST.ACCRUALS$SIM and others

The F.SIMULATION.DETAILS file displays information of all the $SIM files and also updates them on running the simulation service.

The record in the AA.SIMULATION.RUNNER application displays the complete information of the Activities performed on running simulation.

After running the AA.SIMULATION.RUNNER service, the user can amend the record for further simulation by adding more Activities, such as pre-payment, payment rules change, and so on, to be run on specific dates.

If ad hoc activities are added, the date on which the Activity is to be run is specified and the Run Activity field is set to Yes.

After the storage of information to different files, the user can opt to have a live arrangement in the system depending on the client’s decision.

To achieve this, the user can set the Execute Simulation field as Yes in the AA.SIMULATION.RUNNER .


##### Simulation—New Deposit Modelling

Deposit modelling calculates the simulation scenarios by combining variables and fixed values and pass them to the system.

In deposits, the parameters values that play the vital role are the principal amount, interest rate, number of payments (either number of years or months) and payment amount (payment to be made, scheduled payment).

Customers that are interested for a Deposit product may prefer to know the interest rate for the given deposit product, as well as the interest payment amount to be received on a specified period (for example, every month, every week and so on.) for the specified rate and periods. The simulation results give the customers a direct comparison and help them choose the most suitable product for them.

Deposit modelling uses the simulation engine functionality.

The user can feed the fixed parameter using the AA.SIMULATION.CAPTURE application and can view the variable parameter in the same application.

The Auto Run field in the AA.SIMULATION.CAPTURE application decides whether to model the deposits or apply the deposits modelled on to the live system.

A customer requires information regarding the interest pay out that will get credited every month for a specific principal amount, term and interest rate.

Once the simulation run is completed, a simulation record is created in the AA.SIMULATION.RUNNER with the AA.SIMULATION.CAPTURE reference stored in it.

The AA.SIMULATION.SERVICE is a batch service run, which,

- Reads the message written in the AA.SIMULATION.SERVICE.LIST file.
- Calculate the variable parameter.
- Write the payment amount calculated in the respective $SIM file.

The ENQ AA.SIMULATION.MONITOR monitors the progress of the simulation. This enquiry then returns a status of either processing or completed.

In the enquiry output, there is a link to return to the AA.SIMULATION.CAPTURE application where the user can view the variable parameter. If the user has requested for calculating the payment amount, the Calc Amount field in the Payment Schedule is updated with the payment amount. If a request for the Term field (given the principal amount, payment amount and interest rate), then the system updates the term in the Term Amount Property record.

At this stage, the user can amend the same simulation capture and modify the values to find the variable parameter by changing the fixed parameter.

Unlike the simulation engine, the modelling is a step process where the user enters the fixed parameters and the system returns the variable parameter.

The simulation creates a property for each element.


##### Simulation Monitor—Enquiry

By running the ENQ AA.SIMULATION.MONITOR, the user can view the status of the service.

This enquiry takes the simulation runner ID as input and returns the status of the service (whether the service has completed processing). On authorising, the simulation capture, the system writes a record in the AA.SIMULATION.RUNNER application with the details of the simulation capture as shown in the below screenshot.


##### Activity Split

The activities listed in the simulation runner are grouped based on the activity types, such as Scheduled, User or Transaction.


#### 📋 Tasks

Related topics:

- Amend Deposit (AA)
- Open Deposit (AA)

The simulation engine helps in ascertaining the actual results of certain activities, such as:

- Creation of deposit
- Change of interest rate on a live deposit account
- Pre-closure of a term deposit without actually executing the transaction


##### Workflow

This section allows the user to perform the below activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Product Catalog . |
| Product Catalogue | Click the Simulate icon corresponding to Fully Negotiable deposit. |
| Simulate New Arrangement | Enter values in the following fields: Customer Currency Effective Date Click the Validate icon. Click the Commitment tab and then enter values in the following fields: Amount Term |
| New Arrangement | Enter values in the following fields: Customer Currency Effective Date Click the Validate icon to check for errors and overrides. Click the Commit icon. Run the BNK/AA.SIMULATION.SERVICE simulation service. |


#### 📊 Outputs

There are no Outputs available for Deposit Simulation feature.


> **Related Applications:** `AA.ACTIVITY.HISTORY`, `AA.ACTIVITY.HISTORY.SIM`, `AA.ARR.CUSTOMER`, `AA.ARR.INTEREST`, `AA.ARRANGEMENT.ACTIVITY`, `AA.ARRANGEMENT.SIM`, `AA.SIM.CUSTOMER`, `AA.SIM.INTEREST`, `AA.SIMMULATION.RUNNER`, `AA.SIMULATION.CAPTURE`, `AA.SIMULATION.RUNNER`, `AA.SIMULATION.SERVICE`, `AA.SIMULATION.SERVICE.LIST`, `F.SIMULATION.DETAILS`

---


### 1.18  Dormancy


> **📇 Quick Reference Card**
> 
> **Purpose:** *A deposit arrangement has a fixed tenure. On maturity, the deposit can be renewed or redeemed and paid to the customer. If the deposit remains without going through Renewal or Redemption Activity, then the deposit remains in Matured status. The bank can decide to mark deposit accounts in matured sta...*
> 
> **Applications:** `AA.ACCOUNT.DETAILS`
> 
> **Key Fields:** *Arrangement*, *GB Narrative*, *Last Activity Date*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

A deposit arrangement has a fixed tenure. On maturity, the deposit can be renewed or redeemed and paid to the customer. If the deposit remains without going through Renewal or Redemption Activity, then the deposit remains in Matured status. The bank can decide to mark deposit accounts in matured status for a long time, as dormant. A dormant deposit can be closed automatically, after transferring the balance to an internal account. A notice can be sent to the customer prior to its closure. In order to send a notice to the customer and move the balance to internal account, the rules are defined in the Product Qualifier and Activity Restriction Product Conditions.

The dormancy details of the arrangement can be handed off to the Customer Dormancy Monitor (CDM) system for customer level dormancy processing.

- Customer Dormancy Monitoring is not supported in the Deposits TBC and must be handled through an external customer management solution. The dormancy information can be handed-off to the external customer capability as required to monitor the customer dormancy status.
- The exception processing for dormancy can be configured using routines in Deposits TBC. The option to configure a rule-based exception processing, on the rules engine, is not applicable for the Deposits TBC.


#### ⚙️ Configuration

A deposit account is declared as dormant when the deposit account remains without any transaction or activity after the deposit has matured. The Dormancy Property Class holds the conditions to be validated for marking a deposit arrangement as dormant.

Read the Dormancy Property Class user guide for more information.

There may be certain processes or activities that would not prevent the system from marking the deposit arrangement dormant, for example, business process such as system-initiated activities, like periodic charges levied on the account.

Generally, if there is no user-initiated transaction or Activity triggered for a certain period, then the deposit arrangement can be marked as dormant. The period of inactivity to mark the deposit as dormant may vary from bank to bank. The Dormancy Property Class is common for deposits, accounts, loans and safe deposit boxes.

System-driven transactions, for example, activities related to the interest application on the deposit account, which are scheduled AA Activities, are not considered for dormancy purposes.


##### Dormancy Processing

The Dormancy Property Condition displays the list of AA Activities that are included to check the last customer-initiated Activity.

The dormancy process supports different statuses, based on the different inactivity periods in deposits. A sample screenshot is provided below and it displays the charge that can be configured when marking or revoking the dormancy status. If multiple stages of dormancy are configured, then the system schedules the next dormancy check based on the period of the next dormancy status.

In order to determine if a deposit is active, the deposit is checked for any qualifying activity in the evaluation period. A qualifying activity can be a transaction, such as cash payment, or a user driven activity, such as changing Settlement instructions. During configuration, banks can decide which activity to include or exclude from qualifying Activities in a deposit, during dormancy evaluation.

There may be a request from the customer to change the settlement instructions. Although this is an activity, which can prevent the bank to defer marking dormancy to the deposit account, the activity is not a financial one. That is, the system considers both financial and non-financial activities for dormancy assessment.

Read the Dormancy Property Class user guide for more information.

The Dormancy Property Class can be used to indicate the exception rules to be run, in order to exclude certain deposits from dormancy processing. If the system runs the exception rules (user configured) to get the final decision and once confirmed, it marks the account as Dormant. If the exception rule returns a No, then the system does not mark the Account as Dormant and reschedules the Check for Dormancy.


##### Customer Dormancy Processing

Customer Dormancy Monitor (CDM) allows to calculate, manage and report dormancy at the customer level with an option to parameterise inactivity periods at both the customer and product levels.

The Dormancy condition can be configured to handoff the dormancy details to Customer Dormancy Monitor when the arrangement reaches that specific dormancy status. CDM Handoff can be set for one of the dormancy statuses which has to considered for the customer level dormancy processing. The system hands off the dormancy date and the value of Last Activity Date stored in AA.ACCOUNT.DETAILS of the arrangement. When the condition doesn’t have a CDM handoff configured for any of their statuses, then the very first status of the Dormancy condition is considered for the CDM handoff.

Once the CDM handoff is triggered for an arrangement, the CDM requests for the details of the other arrangements held by this particular customer. The CDM system evaluates the dormancy status of the customer based on this information and marks the customer as dormant when all the related accounts and contracts (within the system including AA framework, and outside of the system) are already dormant.

Customer Dormancy Monitoring is not supported in Deposits TBC and must be handled through an external customer management solution. The dormancy information can be handed-off to the external customer capability as required to monitor the customer dormancy status.


##### Auto Closure of Dormant Deposits

Deposits without any customer-initiated transactions for a defined period is moved to dormancy. On reaching the dormancy milestone (as per the period defined in Product Conditions), the balances are automatically transferred to the bank's internal account and the deposit account is closed. The rule sets for the automatic closure of the account are configured through the Activity Restriction Product Condition. The Dormancy Status Condition passes through the rules defined in the Activity Restriction Product Condition - Product Qualifiers to make a decision on whether to close the dormant account.

The exception processing for dormancy can be configured using routines in Deposits TBC. The option to configure a rule-based exception processing, on the rules engine, is not applicable for Deposits TBC.


#### 🔧 Working With

The dormancy information is updated in the Long Term Deposit Overview screen as displayed in the below screenshot.

Dormancy Activity History and Dormancy History can be seen from the drilldown enquiries available in arrangement overview.


##### Customer Level Dormancy Processing

When customer level dormancy processing is configured, for a particular dormancy status, the AA framework hands-off the value of Last Activity Date updated in AA.ACCOUNT.DETAILS , along with the dormancy status of the arrangement, to Customer Dormancy Monitor (CDM).

Customer Dormancy Monitoring is not supported in Deposit TBC and must be handled through an external customer management solution. The dormancy information can be handed-off to the external customer capability as required to monitor the customer dormancy status.


##### Automatic Closure of Dormant Deposits

Auto closure of deposits can be configured using the Activity Restriction Product Qualifiers.

A short-term deposit, which is matured and expired is ready for auto closure as shown below.

A notice is sent to the customer, before auto transferring the balance and closing the deposit.

Read the Dormancy Property Class user guide for illustration of Arrangement Dormancy and Retail Accounts user guide for more information on Inactivity and Dormancy. Differences in TBC In the TBC, the pre-notifications are not applicable and, if required, they should be handled by external solutions. The exception processing for dormancy can be configured using routines in Deposit TBC. The option to configure a rule based on the rules engine is not applicable for Deposit TBC.


#### 📋 Tasks

Related topics:

- Set or Reset Dormancy (AA)

A deposit arrangement has a fixed tenure. On maturity, the deposit can be renewed or redeemed and paid to the customer. If the deposit remains without going through Renewal or Redemption activity, then the deposit remains in Matured status. The bank can decide to mark deposit accounts in matured status for a long time, as dormant.


##### Workflow

This section allows the user to perform the below activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Find Deposit Arrangements | Enter an account arrangement ID in the Arrangement field then click the FIND button. Click the Overview icon corresponding to a record. |
| Arrangement Overview (Deposit) | Click the New Activity option. |
| New Activities | Click the Do Activity Today icon corresponding to the Set Dormancy (Manual) activity. |
| Set Dormancy | Enter values in the following fields: Activity Effective Date Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Find Deposit Arrangements | Enter an account arrangement ID in the Arrangement field then click the FIND button. Click the Overview icon corresponding to a record. |
| Arrangement Overview (Deposit) | Click the New Activity option. |
| New Activities | Click the Do Activity Today icon corresponding to the Reset Dormancy (Manual) activity. |
| Arrangement Activity | Enter a value in the GB Narrative field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

There are no Outputs available for Dormancy feature.


> **Related Applications:** `AA.ACCOUNT.DETAILS`

---


### 1.19  Early Redemption of Deposit


> **📇 Quick Reference Card**
> 
> **Purpose:** *A term deposit interest rate is based on the term that was agreed, for the funds to be held in the deposit. If the customer makes a partial or full redemption, ahead of the agreed term, the bank can reduce the interest rate paid to the customer for the redeemed amount.*
> 
> **Applications:** `AA.BILL.DETAILS`, `AA.CHARGE.DETAILS`, `AA.INTEREST.ACCRUAL`, `AA.INTEREST.ACCRUALS`, `AC.ALLOCATION.RULE`, `AC.EVENTS`, `CUSTOMER.CHARGE`, `PAYMENT.ORDER` ... +1 more
> 
> **Key Fields:** *Active Y/N*, *Actual Group*, *Adj Int Prop*, *Adjust Rate*, *Closure Reason*, *Internal Booking*, *Method*, *Proportional Calc* ... +4 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

A term deposit interest rate is based on the term that was agreed, for the funds to be held in the deposit. If the customer makes a partial or full redemption, ahead of the agreed term, the bank can reduce the interest rate paid to the customer for the redeemed amount.

The system calculates the difference between the original rate (for the full term) and the actual rate, due to early redemption, as a break cost fee and adjusts the same from the accrued interest balance. If the break cost fee is more than the accrued interest, then the remaining amount, after accrued interest adjustment, is reduced from the principal, else this makes the interest accrual overdrawn or negative, based on the Method attribute configuration in Activity Charge or Activity Restriction.

This feature helps the banks to pay the interest amount for the period when the customer holds deposits with the bank.

There are no specific differences for the calculation and processing of break cost fee when a deposit in the TBC is redeemed prior to its maturity.


#### ⚙️ Configuration

The Payout Rules property class along with the Settlement condition governs the early withdrawal from deposits. It lists the properties and the sequence to be settled during a redemption activity. Read Configuring Withdrawal from a Deposit for more information.

The user can trigger an early redemption activity using one of the following:

- PAYMENT.ORDER application
- Arrangement Overview page
- API

A break cost fee can be calculated for a full or partial early redemption, by configuring an activity charge or a rule break charge on:

- DEPOSITS-APPLYPAYMENT-PO.EARLY.WITHDRAWAL
- DEPOSITS-WITHDRAW-PO.EARLY.WITHDRAWAL
- DEPOSITS-REDEEM-ARRANGEMENT

When any one of the activities are triggered, the system calculates the break cost fee. This is adjusted against the accrued interest and the remaining fee, if any, makes the interest accrual to become overdrawn or capitalised against the principal, depending upon the Method attribute configuration in Activity Charge or Activity Restriction.

To enable break cost fee calculation, the following have to be in place.

The features related to triggering an early redemption of a deposit, using a payment order and the arrangement overview screen, are not applicable for deposits in the TBC.


##### Reduced Rate Calculation

The system calculates a charge and collects it as a break cost fee, during a partial or full redemption of term deposit. This charge is configured by specifying the details in Type , Adj Int Prop and Adjust Rate attributes. The user can specify the credit interest property in Adj Int Prop attribute and, based on this property, a break cost fee is calculated and adjusted against the interest accruals.

The user must attach an API routine in Adjust Rate attribute and this routine must locally calculate the adjustment or penalty rates for the early redemption. The routine returns the details of the adjustment or the penalty rate, along with date from which the interest accrual has to be calculated and this enables the system to calculate the break cost fee. The local API routine must return the reduced rate along with the date on which a rate change takes place for the product.

During the life of a term deposit, the interest rate may change. During every change in the interest rate, the system stores the interest rates for the corresponding period in a dated manner. For example,

| Arguments in API | Values |
|---|---|
| Int Dates | 20211201\|20211210\|20220117\|20220225 |
| Int Rates | 10\|7\|12\|5 |

Whenever the interest rate of the deposit is revised, the API has to return the corresponding Penalty Rate explicitly to the core system. For example,

| Arguments in API | Values |
|---|---|
| Adjust Dates | 20211201\|20211210\|20220117\|20220225 |
| Penalty Rates | 9\|5\|10\|4 |

If the Penalty Rate is not returned for a period that has the rate change in the deposit interest, the system automatically considers the original deposit interest rate as the Penalty Rate. This means the entire interest rate is considered as Penalty Rate for that particular period. For example: In the below case, the system considers 12 as the Penalty Rate from Jan 17, 2022 to Feb 22, 2022.

| Arguments in API | Values |
|---|---|
| Adjust Dates | 20211201\|20211210\|20220117\|20220225 |
| Penalty Rates | 9\|5\| \|4 \| |

> **⚠️ Note:** Banks can pass Adjust Rates instead of Penalty Rates in the APIs to calculate the break cost fee.

For a roll over contract, the renewal date is considered as the start date for break cost fee calculation. In case of a change in the product, the latest product-change date is considered as the start date for break cost fee calculation. The following are some example routines, available in the model bank for illustration purposes.

- AA.LOCAL.CHARGE.INT.ADJUST.RATE - Provides the rate by which the original contract rate has to be reduced.
- AA.LOCAL.CHARGE.INT.PENALTY.RATE - Provides the rate using which the new accruals have to be calculated.

Original (Actual) deposit rate - 5%,

Rate applicable due to break - 3%

For the above scenario, the rates considered for break cost fee calculation for the respective local API are shown below:

- AA.LOCAL.CHARGE.INT.ADJUST.RATE - 2%
- AA.LOCAL.CHARGE.INT.PENALTY.RATE - 3%

The AA.LOCAL.CHARGE.INT.NULL.VALUE routine does not return any rates. This routine evaluates if the interest property is fixed, floating or periodic rate.

- If it is a periodic rate, the system considers the PERIODIC.INTEREST application and returns the rate for that elapsed period to the deposit as the adjusted rate.
- In other cases, default 1% is reduced from the original rate and returns it back as the adjusted rate for interest calculation.

The user can utilise the AA.LOCAL.BREAK.COST.PENALTY.RATE routine to pass the adjust rate or penalty rate by referring the logic of the above mentioned model routines or can create a new routine as per their requirement.

The user has to attach a Charge product condition with a charge property, for which the property type is selected as ADJUST.DUE or ADJUST.

- ADJUST.DUE - Denotes that a separate due entry is raised and displayed in the account statement for break cost fee.
- ADJUST - Denotes that there will not be any entry shown in account statement for break cost fee.

Read Charge property class and Property types pages for more information.


##### Break Cost Fee Calculation

During a partial or full redemption from a term deposit, the difference between the accrued amount, based on the original rate and the accrued amount, for the reduced or adjusted rate, is calculated as the break cost fee.

- When the interest is scheduled to be paid on a periodical basis or on maturity, the calculations are based on the redeemed amount requested for partial redemption and on outstanding principal amount for full redemption.
- When the interest is capitalised on a periodical basis, the break cost fee calculation is not supported.


##### Adjustment of Break Cost Fee

The system can be configured to adjust the interest accruals with the break cost fee calculated. When the break cost fee exceeds the interest accrual amount, then the remaining break cost fee is treated as a negative balance in the accrual ( Tot Neg Accr Amt ) or simply capitalised to the deposit principal, thereby reducing the principal. This is possible through the setting of the Method attribute with Adjust or Adjust cap values, in Activity Charges or the Activity Restriction conditions, where the break cost fee is configured. When the user selects,

If the break cost fee is,

- Less than accrued interest - The system adjusts the accruals with the break cost fee amount and leaves a credit balance in the accrued interest. In this scenario, the accrued interest balance is debited and the fee income (PL) gets credited.
- More than the accrued interest - The system adjusts the accruals with the break cost fee amount and results in the interest accruals becoming negative. In this scenario, the accrued interest balance is debited and the fee income (PL) gets credited. After this, the daily accruals are adjusting the negative accrual balance. Until the interest accrual balance becomes positive, the accrued interest for the period is not made due, even though the interest capitalisation or pay-out schedule falls before that.

If break cost fee is,

- Less than accrued interest - The system adjusts the accruals with the break cost fee amount and leaves a credit balance in the accrued interest (same as Adjust option). In this scenario, the accrued interest balance is debited and the fee income (PL) gets credited.
- More than the accrued interest - The system adjusts the break cost fee to the extent of accrued interest and the excess amount is capitalised against the principal. In this scenario, the accrued interest and principal balance gets debited and the fee income (PL) gets credited..

However, if the principal capitalisation makes the account balance negative, the system raises a validation and prohibits the transaction, thus resulting in its failure.

If a partial or full redemption activity is triggered when the interest accrual balance is already negative, the break cost fee is adjusted against the deposit balance and the interest accrual balance remains as is.

> **⚠️ Note:** If an interest amount calculated based on the adjustment rate is more than the actual accrued interest amount (that is, the sum of the accrued interest paid to the customer and the accrued interest yet to be paid) during an early redemption activity for the current cycle, the break cost fee is not calculated and the adjustment of interest accrual does not take place. If the Internal Booking attribute is selected in the Charge product condition, the break cost fee is credited to the internal category specified in the Accounting condition, instead of the fee income (PL) category. The user can configure more than one break cost fee (charge) for a product. For example, it is possible to have one break cost fee configured for DEPOSITS-APPLYPAYMENT-PO.EARLY.WITHDRAWAL activity and another break cost fee configured for DEPOSITS-REDEEM-ARRANGEMENT activity. Although the system does not restrict it, if more than one break cost fee is configured for the same activity, the break cost fee adjustment does not work in such scenarios.

The accounting related features and processing are handled by an external GL system for deposits in the TBC. Therefore, to complete the accounting related to adjustment of accruals or deposit principal with the break-cost fee in a deposit, the TBC generates an event which can be captured by the connected external GL (General Ledger) system.


##### Tax Amount Recalculation during Early Redemption

Various types of tax such as withholding tax, income tax and so on can be calculated on the interest amount, in the term deposit product. Read Introduction to Tax for more information.

During a partial or full redemption from a deposit, the calc routine recalculates the interest, based on the reduced rate applicable for the period, when a break cost fee is configured. Similarly, the tax amount is recalculated based on the recalculated interest amount.

When the interest amount is not paid on a regular basis (interest paid at maturity), the system does not calculate the tax amount at the time of partial redemption. Tax is calculated only at the time of full redemption or maturity.

When the interest amount is paid to the customer during an early maturity or partial redemption, the system calculates the tax for the recalculated interest amount based on the adjusted interest rate.

When the interest is paid to the customer on regular intervals, the tax for such interest payments is based on the forecasted original interest rates. Due to this early redemption, full or partial, the interest amount is adjusted, and the tax amount also varies accordingly.

The details between the original tax amount collected (proportionate tax amount in case of partial redemption) and the actual applicable tax amount, after this full or partial redemption, are updated in AA.CHARGE.DETAILS .

During implementation, AA.CHARGE.DETAILS can be used to configure local enquiries and reports for this difference in tax. This detail can be shared with the deposit holder for applying a reimbursement with tax authorities.

> **⚠️ Note:** AA.CHARGE.DETAILS stores the actual amount, interest rate, actual tax amount, adjusted amount, adjusted interest rate, and adjusted tax amount. It also stores any change in interest rate or change in principal amount. All this information is stored chronologically.

If the Proportional Calc attribute is selected for the tax code, the system does not support break cost fee calculation when the particular tax code is configured for the interest property. The system raises a validation error if a break cost fee (using the Charge condition) is attached with a proportional tax in the deposit.


##### Tax on Break Cost Fee

Tax can be defined for a break cost fee. It is associated with the charge property used as break cost fee and is eventually collected by adjusting the interest accrual or the principal of term deposit along with the charge (either as Adjust or Adjust Cap). Using allocation rules ( Overview of AA Accounting Processing ), the system can be configured to collect break cost as fee income to the preferred PL and the tax amount to the preferred tax internal account.

The tax related assessments are performed based on the customer attributes and these attributes are part of an external system, that is, the Party TBC. Hence, the tax group that the customer belongs to, can be updated using an API in the Actual Group attribute of the CUSTOMER.CHARGE application in the TBC.

The accounting related features and processing are handled by an external GL system for deposits in the TBC. Therefore, to complete the accounting related to tax on the break cost fee, the TBC generates an event, which can be consumed by the connected external GL (General Ledger) system.

Read here to know more about processing of taxes for deposits in the TBC.


##### Exclusions

Although the system does not provide a restriction, the break cost fee is not supported in the following cases.

- RFR and tiered interest types.
- Term deposit products with interest capitalisation. During the life cycle of an arrangement, if an interest payment type is changed from pay to capitalise and vice versa.


##### Allocation Rules

For break cost fee calculation and adjustment, the following list of AC.EVENTS records are available in the AC.ALLOCATION.RULE for Interest, Charge, Tax and Account.

- INTEREST-ADJUST.DUE-ACC
- CHARGE-ADJUST.DUE-DUE
- INTEREST-REPAY-DUE-OS
- ACCOUNT-ADJUST.DUE-CUR
- TAX-ADJUST.DUE-DUE
- TAX-ADJUST.DUE-INT
- INTEREST-ADJUST.DUE-ACC-CM

The accounting related features and processing are handled by an external GL system for deposits in TBC. Therefore, to complete the accounting related to calculation and adjustment of accruals or deposit principal with the break-cost fee in a deposit, the TBC generates an event which can be captured by the connected external GL (General Ledger) system.


#### 🔧 Working With

It is possible to allow a partial or full redemption of a term deposit, prior to the term deposit contract end date. In this case, the banks are usually applying interest rate adjustments, for the funds held with the bank for the elapsed period, in the form of a break cost fee that is adjusting the interest accruals. Interest adjustment, due to early redemption is calculated as a charge.

Based on the adjustment or the penalty rate, the interest amount is calculated for the redeemed amount, from the start date of term deposit or the renewal date, in case of a rolled-over contract. This calculated interest amount is subtracted from the accrued interest, which was based on the original interest rate and the calculated amount is raised as a charge. This charge is termed as break cost fees.

This break cost fee is raised as a fee and is adjusting the accrued interest. If the break cost fee is more than the accrued interest, then the remaining amount is either capitalised, that is reduced from the principal, or turns the interest accrual into negative, based on the configuration.


##### Early Redemption

The user can trigger an early redemption activity using:

- PAYMENT.ORDER
- Arrangement overview page
- API

The user can run a simulation process that produces a partial or full redemption statement, based on the customer’s request. This statement provides a detailed break-up of the deposit’s current balance, the redeemed amount, any redemption charges, and in the case of partial redemptions, an interest loss comparison is given. If the user accepts the quotation, then the flow for both partial and full redemption, is the same and, at the end of the flow, the payments are made to the customer’s account. Read Introduction to Simulation of Partial or Full Closure of Deposit for more information.

The deposit product can be configured to calculate a break cost fee during an early redemption activity. In a deposit the user can trigger an early redemption using:

- DEPOSITS-APPLYPAYMENT-PO.EARLY.WITHDRAWAL
- DEPOSITS-WITHDRAW-PO.EARLY.WITHDRAWAL
- DEPOSITS-REDEEM-ARRANGEMENT

A break cost fee is calculated on these activities, using an Activity Restriction or Activity Charges configuration.

When the user performs an early redemption, the system evaluates the activity restriction on that activity or calculates the activity charge on that activity to levy the break cost fee. If Method is set as:

- Adjust - The entire break cost fee is adjusted against the accrued interest.
- Adjust cap - The available accrued interest gets adjusted against the break cost fee and the remaining fee is reducing the deposit's principal.

The features related to triggering an early redemption of a deposit using a payment order and the arrangement overview screen are not applicable for deposits in the TBC.


##### Early Redemption of Deposit without Tax Configuration in Interest - Illustration

Consider a deposit is created with below configuration:

- Principal = 100000
- Interest rate = 5%
- Deposit created for 3M on 2nd Apr
- Interest to be paid = First day of every month
- Breakcost fee = Adjust in Method attribute in Activity Charges
- During early redemption, the interest rate to be considered for the redeemed amount for the elapsed period = 4%

AA.INTEREST.ACCRUALS before early redemption, is shown below.

The ECB before early redemption is displayed below.

Now, when the user triggers an early redemption activity on Apr 19, a break cost fee is calculated and the same is adjusting the interest accrual balance.

Once the user accepts the simulation result, the break cost fee is raised and settled by adjusting the interest accrual.

Break cost fee = (100000*0.05*18)/360 –(100000*0.04*18)/360 = 250 – 200 = 50 USD

After redemption, AA.CHARGE.DETAILS and AA.BILL.DETAILS are as below.

The user can view the break cost fee details in AA.CHARGE.DETAILS and AA.BILL.DETAILS tables.

The break cost fee of 50 USD is adjusting the accrued interest balance. Interest accrual balance, after adjustment of break cost fee details, is shown in AA.INTEREST.ACCRUALS table. The user can check the Total Due Amnt field to view the interest balance.

When a break cost fee is configured, two types of scenarios are possible, during a partial or full redemption from term deposits.

- Break cost fee less than accrued interest
- Break cost fee more than accrued interest

The difference between Adjust and Adjust cap for the above scenarios is explained below.

| Method - Adjust | Method - Adjust cap |
|---|---|
| The break cost fee is less than accrued interest, and the system adjusts the interest accruals, with the calculated break cost fee. Interest accrual balance = (138.89-88.89) = 50 USD | The break cost fee is less than accrued interest, and the system adjusts the interest accruals, with the calculated break cost fee. Interest accrual balance = (138.89-88.89) = 50 USD |

| Method - Adjust | Method - Adjust cap |
|---|---|
| If the break cost fee is more than accrued interest, the system allows the fee to adjust to the extent of accrued interest and the remaining fee makes the interest accrual become overdrawn. Interest accrual balance = -152.78 USD (291.67-138.89) During the next payment cycle, the system checks whether interest accrual is in positive or negative balance. If the balance is positive, the make due activity takes place else bill is not made due. | If the break cost fee is more than accrued interest, the system allows the fee to adjust to the extent of accrued interest and the remaining fee is capitalised against the principal. Hence, Interest accrual balance of 138.89 USD is nullified in this case. Balance fee of 152.78 USD is capitalised against the principal. Principal balance after partial redemption = 25000 – 152.78 = 24847.22 USD |


##### Early Redemption of Deposit with Tax Configured in Interest - Illustration

Break cost fee calculation with tax configuration on interest is explained below.

Consider a contract configuration as below.

- Principal = 100000 USD
- Original Interest rate = 5%
- Days = 18
- WHT = 20%
- Interest paid-out = Every 14 days
- Interest accrued for 1st cycle = (100000*0.05*14)/360 = 194.44 USD
- Tax levied and collected for 1st cycle = (0.2*194.44) = 38.89 USD
- Interest paid to customer so far = 194.44 – 38.89 = 155.55 USD
- Interest accrued and yet to be paid = (100000*0.05*4)/360 = 55.56 USD

Now the customer makes a full redemption of 100000 USD on the 19th day.

- Interest accrual calculation for 100000 USD for 18 days = (100000*0.04*18)/360 = 200 USD
- Break cost fee = 250 – 200 = 50 USD

Tax recalculation based on the reduced rate

- Interest accrued for 1st cycle = (100000*0.04*14)/360 = 155.56
- Tax levied = (0.2*155.56) = 31.11 USD

When Method is set as Adjust,

AA.INTEREST.ACCRUAL balance after full withdrawal = 55.56 – 50 = 5.56 USD

The customer receives a total of 1,00,005.56 USD (1,00,000 – Principal + 5.56 Interest)

In this case, the customer has already paid 38.89 USD tax amount. However, customer’s actual tax obligation is 31.11 USD, due to full redemption done before contract expired. The user can view the original tax and the actual tax, due to early redemption, details in the AA.CHARGE.DETAILS table.

| Actual Interest Calculation | Interest calculation on 70000 USD @ 5% interest | Interest calculation on 70000 USD @ 4% interest |
|---|---|---|
| Interest accrued for 1st cycle = (100000*0.05*14)/360 = 194.44 USD Tax = (0.2*194.44) = 38.89 USD Interest paid to customer so far = 194.44 – 38.89 = 155.55 USD Interest accrued and yet to be paid = (100000*0.05*4)/360 = 55.56 USD | Interest accrual calculation for 1st cycle = (70000*0.05*14)/360 = 136.11 USD Tax = (0.2*136.11) = 27.22 USD Interest accrual calculation = (70000*0.05*18)/360 = 175 USD | Interest accrual calculation for 1st cycle = (70000*0.04*14)/360 = 108.89 USD Tax = (0.2*108.89) = 21.78 USD Interest accrual calculation = (70000*0.04*40)/360 = 140 USD Break cost fee = 175 – 140 = 35 USD |


#### 📋 Tasks

Related topics:

- Perform Partial Withdrawal of Deposit (AA)
- Perform Pre-Closure of Deposit (AA)

Break cost fee can be configured for term deposit product. During early redemption, break cost fee is calculated and collected as a fee income.


##### Workflow

In Early Redemption of Deposit, the user can perform the following activities:

User can trigger partial withdrawal activity during the term deposit lifecycle.

To initiate a Partial Withdrawal, follow the below steps.

1. Authorised .
2. Enter the required field values and click Find button.
3. Click the Overview icon.
4. Click the Run option corresponding to Redeem Deposit activity.
5. Enter values in following fields: Redemption Date Closure Reason
6. Click the Validate icon to check for errors and overrides.
7. Click the Commit icon.
8. Run the BNK/AA.SIMULATION.SERVICE simulation service.
9. Click the Withdrawal Statement icon.
10. Click the Withdrawal Details .
11. Click the Proceed Withdrawal .
12. Click the Validate icon to check for errors and overrides.
13. Click the Commit icon.
14. Click the Settlement Instruction section to expand.
15. Settlement instructions for partial withdrawal must be updated with Active Y/N to Yes.
16. Click the Validate icon to check the errors and overrides.
17. Click the Commit icon to complete the transaction.

User can trigger an early redemption of term deposit.

1. Authorised .
2. Enter the required field values and click Find button.
3. Click the Overview icon.
4. Click the Run option corresponding to Redeem Deposit activity.
5. Enter values in following fields: Redemption Date Closure Reason
6. Click the Validate icon to check for errors and overrides.
7. Click the Commit icon.
8. Run the BNK/AA.SIMULATION.SERVICE simulation service.
9. Click the View Statement option corresponding to Redemption Statement .
10. Click the Bill Details .
11. Click the Redeem Deposit .
12. Click the Validate icon to check for errors and overrides.
13. Click the Commit icon.
14. Click the Settlement Instruction section to expand.
15. Settlement instructions for partial withdrawal must be updated with Active Y/N to Yes.
16. Click the Validate icon to check the errors and overrides.
17. Click the Commit icon to complete the transaction.


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to Break Cost Fee for Early Redemption.


##### Enquiries and Reports

This section allows the user to view the below list of enquiries and reports:

Breakcost fee Adjust bill .

This enquiry displays due date, type, amount, and settled on date when adjust is configured on Charges/Restriction activity.

Breakcost fee AdjustCap bill .

This enquiry displays due date, type, amount and settled on date when adjust cap is configured on Charges/Restriction activity.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA


> **Related Applications:** `AA.BILL.DETAILS`, `AA.CHARGE.DETAILS`, `AA.INTEREST.ACCRUAL`, `AA.INTEREST.ACCRUALS`, `AC.ALLOCATION.RULE`, `AC.EVENTS`, `CUSTOMER.CHARGE`, `PAYMENT.ORDER`, `PERIODIC.INTEREST`

---


### 1.20  Funding of Deposit


> **📇 Quick Reference Card**
> 
> **Purpose:** *Term deposits are investment instruments characterised by a pre-determined period, which typically, range from seven days to ten years. The Savings Plan or Recurring Deposits allow the customer to invest a fixed amount into a deposit account for an agreed period and the amount remains with the bank ...*
> 
> **Applications:** `AA.ARR.TERM.AMOUNT`, `AA.INTEREST.ACCRUALS`, `AA.PARAMETER`, `BENEFICIARY.LINKS`, `PAYMENT.ORDER`, `TEC.ITEMS`, `TRANSACTION`
> 
> **Key Fields:** *Account Debit Rule*, *Active Y/N*, *Amount*, *Arrangement Id*, *Counterparty*, *Counterparty Type*, *Currency*, *Customer* ... +15 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Term deposits are investment instruments characterised by a pre-determined period, which typically, range from seven days to ten years. The Savings Plan or Recurring Deposits allow the customer to invest a fixed amount into a deposit account for an agreed period and the amount remains with the bank during the contract period.

The customer can choose to fund a deposit arrangement automatically, when the deposit arrangement is opened or manually at any time after the arrangement is created. Also, the customer can choose to either fund the deposit in full through a single transaction or partially through multiple transactions. Back value dated funding is possible when the settlement account is within the system. Interest accrual for the deposit starts once the arrangement is funded, either partially or fully.

The incoming payments in a deposit can be restricted from pre-defined counter accounts only which are added during deposit opening and maintenance processes.

In the TBC, the funding of a deposit can be done, either by debiting another existing account within the TBC, or through an account maintained outside the TBC, in which case, the TBC publishes an event with the settlement request that will be consumed by an external payments system for further processing.

> **⚠️ Note:** It is not possible to define and process nominated counter party restrictions in deposits using the TBC.


#### ⚙️ Configuration

The Retail Deposits module enables the bank to create a Term Deposit with different term periods. The user can define the term period in days (D), weeks (W), months (M), or years (Y).

The term period is the contract period for the deposit arrangement and generally, the interest rate provided by the bank remains the same. If the customer wants to terminate the contract and withdraw the deposit arrangement, then the bank can charge a penalty fee on the deposit arrangement.

If the user does not specify any term, then the system enables the user to create the deposit as a call deposit, where the customer can withdraw the deposit arrangement at any time.

The commitment amount is the principal amount committed, as part of the deposit arrangement contract. The deposit is funded either,

- Automatically, when creating a deposit arrangement using the settlement condition, or
- Manually, based on the customer preferences.

The maturity date of the term deposit is calculated automatically based on the term period that the user enters.

The term of the deposit is calculated from the start date till the maturity date of the deposit at the time of creation of the deposit. If the deposit is funded on a date later than the arrangement creation date, then term of the deposit is adjusted to match the start date and the maturity date in the arrangement. When the Base Date Type is set to Start instead of Agreement in the Account condition, the maturity date (and payment schedule) is recalculated at funding, thereby maintaining the term of the deposit.

If the maturity falls on a holiday, then the maturity date is modified based on the value available in the Mat Date Convention field of the Term Amount Property Condition. If the Mat Date Convention field is set to Yes, then the system validates the value populated in the Maturity Date field for holiday and adjusts the date according to the value available in the Date Convention field in the Account Property Condition.

The user can modify the threshold period value in the Term Tol Days field and can decide whether to recalculate the term based on the value in the Maturity Date field.

Once the user creates deposit arrangement, the system generates a bill for the principal amount in the Outstanding Deposits section and sets the Type field as Expected.

The user can choose to fund the deposit arrangement using funds transfer transaction or through payments hub using payment orders manually, or using the Payin settlement account defined in the Settlement Property Condition.

If the user defines the Payin Account in the Settlement Property Condition, then the deposit is funded automatically when creating the arrangement, debiting the Payin account. On full funding of the deposit, the Status field in the Deposit Overview section is set to Settled.

In the TBC, the funding of a deposit can be done, either by debiting another existing account within the TBC, or through an account maintained outside the TBC, in which case, the TBC publishes an event with the settlement request that will be consumed by an external payments system for further processing.

A deposit can be funded in one of the following ways:

- Automatically by configuring the settlement account or beneficiary using payment order in the settlement condition
- Manually by triggering the deposit funding transaction in the corresponding payment system such as PAYMENT.ORDER .

In both cases, the system triggers a DEPOSITS-APPLYPAYMENT- activity. The expected bill in the deposit is settled as per the order mentioned in the corresponding payment rules condition such as collection of the deposit principal amount and the corresponding charges that are due to the bank.

In the TBC, when the user funds the deposit or settles any due charges in the deposit, the system can either settle the funds with another account within the TBC or through an account or beneficiary outside the TBC, in which case, the system forwards a settlement request to the account or beneficiary by publishing an event that should be consumed by an external payments system for further processing.

Hence, the payment order related details are not applicable for deposits in the TBC.

The Reconstruct Settlement field in AA.PARAMETER is used in Back Dated Settlement processing.

This is a system wide parameter which controls the behavior of the system in a reverse and replay scenario. When a back dated activity is triggered on an arrangement and the Reconstruct Settlement field is set to AUTOMATIC, the system performs a reverse and replay of the backdated settlement processing to a settlement account based on the updated conditions in the arrangement.

When an arrangement is created with a back value effective date, any initial back dated settlement processing does not depend on the above-mentioned parameter setting. In this case, the system automatically performs the back dated settlement processing for the new arrangement.

> **⚠️ Note:** The upgrading clients may not choose to invoke this feature, so a system parameter controls this. This is a no-change field with an override being given to the user.

A new arrangement can be funded directly without the need of a manual process. The funding of the deposit can be effective today or backdated.

In the Settlement Instructions the Payment Type needs to be defined as DEPOSIT.PRINCIPAL and the required funding account needs to be defined.

Once completed, the defined account is debited and the deposit is funded. The status is Current and the expected bill is marked as Settled.

A new deposit arrangement backdated 1 day is created with the settlement account defined.

- A Deposit is funded and is in Current status.
- A Settlement account is debited.

A backdated deposit for 1 day is created as shown below

Amount is for USD 6,500

A settlement account is defined for funding.

After authorisation the deposit is funded.

The deposit funding amount is debited.


##### Nominated Counter Accounts

The incoming payments to a deposit can be restricted from pre-defined counter accounts only which are added during deposit opening and maintenance processes. This can be achieved using the associated multi-value set of fields - Counterparty Type and Counterparty in the Account condition.

Read here to know more about the fields related to nominated counter accounts.

Based on the Counterparty Type setup, the system can evaluate if:

- Payment is received only from those counter account/s when Counterparty Type is Payin
- Payment is sent to only those counter account/s when Counterparty Type is Payout
- Payment is sent to/received from only those counter account/s when Counterparty Type is Both
- There is no evaluation done when the Counterparty Type is Blank / not set.

The evaluation is done on any transaction such as payment or interest and charges settlement in the deposit.

In TBC, it is not possible to define, and process nominated counter party restrictions in deposits.

It is possible to notify the customer about the nominated counter account details for a deposit by configuring the Activity Messaging condition which generates an advice in the following scenarios:

- During deposit opening
- When there is an update in the nominated counter account details

In the below screenshot, the Activity Messaging condition is configured to send a notification to the customer about the nominated counter account details for the deposit arrangement. The notification is generated during deposit opening as well as when there is an update in the account condition.

The advice record for nominated counter account details is as given below.

The advice handoff details for the above-mentioned setup are as given below.

When a beneficiary is defined as nominated counter account for an arrangement, it is possible to notify the customer when there is a change in the beneficiary details (such as Beneficiary IBAN/ Account number).

When the beneficiary details are amended, the ‘COUNTERTYPE.BENEFICIARY.CHANGE’ record in the TEC.ITEMS application is mapped to trigger a non-financial activity in AA by configuring the Activity Mapping condition.

In the below screenshot, the Activity Mapping condition is defined to trigger a linked activity of the Record Event activity (that is, DEPOSITS-RECORD-BENEFICIARY.UPDATE activity) when the beneficiary details are modified.

The Activity Messaging condition is defined to send an advice to the customer whenever the non-financial AA activity is triggered in the arrangement.

The advice record for change in beneficiary details is as given below.

The advice handoff details for the above-mentioned setup are as given below.


#### 🔧 Working With

In the Retail Deposits module, the system defaults the details, such as term deposit products, term period, and the amount defined in the Term Amount Property Condition, to the new deposit arrangement created for the customer. The user can modify the details in the arrangement as per customer’s request, subject to negotiation rules set in the Term Amount Property Condition.

The Amount field displays the commitment amount credited to the deposit arrangement. Apart from standard amount input format, the field accepts values with text T and M (10T for ten thousand and 1M for one million).

The system allows modification of the term period during the tenure of the deposit arrangement, using the DEPOSITS-CHANGE.TERM-COMMITMENT Activity Class.

The screenshot below displays the fields related to the term and commitment available in the AA.ARR.TERM.AMOUNT record of the deposit arrangement.

The user has to ensure that the customer funds the deposit arrangement once created. To fund the deposit arrangement, the system triggers a bill for the deposit amount with details of the amount to be paid and sets the Type field as Expected Deposit. This is available in the Outstanding Deposits section.


##### Additional Funding of Deposit

Deposits are funded only upto the TOT committed as the deposit funding amount as specified in the customer agreement. In a loan, a top up loan can be disbursed using the Increase Commitment Activity. Increasing the commitment in a deposit is not possible. Hence that Activity/Activity Class is not released by Temenos. There may be instances where the bank chooses to fund a deposit exceeding the total committed amount. This section describes how an increase of deposit be achieved without triggering an Increase Commitment Activity.

It is possible to increase the principal amount (more than the TOTCOMMITMENT) of deposit arrangement which is already fully funded. Banks can allow the customer to make an additional deposit during the arrangement's lifecyle with interest accruing for the additional deposit amount as well.

Once the deposit is funded for the live deposit principal, any additional amount funded is mapped to funding the CURACCOUNT using the CURRENT option in Application Type. As a general rule, the Deposits Credit Arrangement is the reminder activity.

This adhoc funding activity is mapped in Activity Mapping or this can be added as a reminder activity for the regular funding activity of the deposit. The product is proofed and published.

Consider an arrangement is created on May 13, 2024. The amount is updated as 100000 in the Term Amount condition. The deposit is fully funded.

On May 15, 2024, the customer transfers or deposits an additional amount of 40,000 USD to his deposit arrangement.

From the COS overview screen, the total principal is updated as 140000 and CURACCOUNT balance is updated as 140000 in ECB.

The AA.INTEREST.ACCRUALS , shows that the interest is accrued for 140000 on May 15, 2024.


##### Settlement Conditions for Manual Settlement

This section guides the user to fund the deposit manually.

1. AA Deposit - Fund . The funding version of FT is displayed.
2. Enter the required details to complete the funding of the deposit arrangement.
3. Authorise the record. The system displays the Status field as Current in the Long Term Deposit Overview section. The Additional Details section displays the Status field as Settled.

> **⚠️ Note:** The customer can choose to fund the deposit arrangement manually, using FT, TT, or Payment Order (to TPH or external payment system) as required by the bank.

In the TBC, the manual funding of a term deposit in the TBC is performed through the appropriate API. Therefore points 1-3 described above are not applicable for the TBC.


##### Settlement Conditions for Auto Settlement

The Deposit product has the Settlement Property Class. If the customer provides a current or savings account as settlement account for the deposit arrangement, then the system updates it to the Payin Account field of the Settlement Property Condition. When authorising the deposit arrangement, the system automatically settles the bill raised for the principal amount (bill type – Expected) by debiting the amount from the savings or current account (Based on the value defined in the Account Debit Rule field). When the Payin Account has insufficient funds for funding, the system retries the transaction in regular intervals based on the RC configuration. The amount billed under the same payment date can be combined and settled as a single settlement when automatic settlement with the same account, maintained in the system, is defined.

Read the Settlement Property Class user guide for more details.

In the TBC, when the user funds the deposit, either partially or fully, the system can settle the funds with another account within the TBC or through an account or beneficiary maintained outside the TBC, in which case, the system publishes a settlement request event that can be consumed by an external payments system for further processing.

> **⚠️ Note:** The features related to recycling the failed postings can be achieved using the Transaction Recycler configured at the GAI (Generic Accounting Interface) level.


##### Nominated Counter Accounts

The incoming payments in a deposit can be limited from pre-defined counter accounts or nominated counter accounts only using the Counterparty Type and Counterparty fields in the account condition. When Counterparty Type is set to Pay.in or Both, the system validates if the beneficiary used for incoming payments is one of the beneficiaries defined in the associated Counterparty field.

Based on the scenario, the counter account can be set only for Payin or for Payout or Both.

- When the system is set to evaluate the Payin transactions using the option Payin in Counterparty Type - only the incoming payments with Validate Counter Party as Yes in TRANSACTION are monitored, and outgoing payments are not monitored. The system raises an override when the incoming payments are not received from one of the beneficiaries mentioned in the associated Counterparty field.
- When both incoming and outgoing payments should be evaluated, it is recommended to setup the Counterparty Type as Both and set Validate Counter Party as Yes in TRANSACTION code used. The system raises an override when the incoming payments are not received from or outgoing payments are not made to one of the beneficiaries mentioned in the associated Counterparty field.
- When the user prefers to ensure that Payin transactions must have a specific Beneficiary and Payout transaction must have a different Beneficiary, the Counterparty Type must be multivalued to take the values Payin and Payout and their respective Beneficiaries must be defined alongside them as Counterparty .

Once a beneficiary is defined as nominated counter account for an arrangement, the system creates a record in the BENEFICIARY.LINKS application to maintain the link between the beneficiary and the arrangement. To indicate that the beneficiary is a nominated counter account to the arrangement, the BENEFICIARY.LINKS application has the Counterparty Type field set to Yes. The BENEFICIARY.LINKS application is also updated with records of those beneficiaries that are not nominated counter accounts for the arrangement but are defined in the Settlement condition.

When a transaction is posted the system evaluates the IBAN number. In its absence, the system evaluates the account number with BIC/banks sort code to validate if the corresponding account is a nominated counterparty.

Read here to see an illustration of nominated counter accounts.

- When Counterparty Type is set but no counter accounts are defined in Counterparty , the system raises an override to indicate the same.
- When the user adds or removes beneficiaries as nominated counter accounts for an arrangement, system raises an override to intimate the user that the nominated counter account details are amended.
- The Nominated Counter Accounts feature is supported only for the payments initiated through the Payment Order application and payments processed through Temenos Payments Hub

In TBC, it is not possible to define, and process nominated counter party restrictions in deposits.


#### 📋 Tasks

Related topics:

- Open Deposit (AA)
- Account and Deposit Processes (Retail)

The funding of Deposit Arrangement can be done during the creation of Deposit Arrangement or after the creation of Deposit Arrangement.


##### Workflow

Funding of Deposit related activities are listed below:

Deposit Arrangements can be automatically funded when an Arrangement is created by giving the debit account in the settlement product condition. Once the Arrangement is authorised the amount gets credit in Deposit Arrangement and status is set as current.

This option allows the user to collect the rent, charge and periodic charges.

To initiate an automatic funding, follow the below steps:

1. Find Deposits .
2. Click the New Arrangement icon for the two year deposit.
3. Enter the values in the following fields: Customer Currency

1. Click the Validate icon to check for errors.
2. Expand the Commitment option.
3. Enter a value in the Amount field.
4. Expand the Settlement Instruction option.
5. Select the Basic tab.
6. Select the Yes option in the Active Y/N field for Initial Funding and Charge Settlement.
7. Enter a value in the Settlement A/c field for Initial Funding and Charge Settlement.
8. Click the Validate icon to check for errors and overrides.
9. Click the Commit icon to submit the record.

If the debit account number is not specified in settlement during arrangement creation, then the user has the option to manually fund the Deposit Arrangement either through payment order or teller.

Before funding, the status of Deposit Arrangement is set as “Not Funded”.

To do manual funding through TT, follow the below steps:

The user can perform the below tasks:

This option allows the user to perform AA Deposit – Fund.

1. AA Deposit-Fund .
2. Enter values in the following fields: Debit Account Number Credit Account Payment Amount
3. Click the Validate icon to check for errors.
4. Click the Commit icon and accept the overrides, if any.
5. Run the BNK/PAYMENT.STPFLOW.HEAVY service for successful transaction.

This option allows the user to perform AA Pay-out-Domestic.

1. AA Pay-out-Domestic .
2. Enter values in the following fields: Debit Account Number Credit Account Payment Amount
3. Click the Validate icon to check for errors.
4. Click the Commit icon and accept the overrides, if any.
5. Run the BNK/PAYMENT.STPFLOW.HEAVY Service for successful transaction.

This option allows the user to perform AA Pay-out-International.

1. AA Pay-out-International .
2. Enter values in the following fields: Debit Account Number Payment Currency Payment Amount Beneficiary ID
3. Click the Validate icon to check for errors.
4. Click the Commit icon and accept the overrides, if any.
5. Run the BNK/PAYMENT.STPFLOW.HEAVY service for successful transaction.

This option allows the user to authorise the Arrangements (PO).

1. Authorise/Delete Arrangements (PO) .
2. Click the Authorise icon.
3. Click the Authorise icon.

This option allows the user to delete the Arrangements (PO).

1. Authorise/Delete Arrangements (PO) .
2. Click the Delete icon.
3. Click the Delete icon.

| SCREENS | WORKFLOW |
|---|---|
|  | Search Customer . |
| Find Customer | Enter the customer ID in the Customer ID field and then click the FIND button. Click the Single Customer View icon. |
| Customer Details | Click the Deposits tab. Select the Fund Deposit(PO) option from the drop-down list and then click the Select icon. |
| AA Payoff | Enter values in the following fields: Debit Account Number Credit Account Payment Amount Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

There are no Outputs available for Funding a Deposit feature.


> **Related Applications:** `AA.ARR.TERM.AMOUNT`, `AA.INTEREST.ACCRUALS`, `AA.PARAMETER`, `BENEFICIARY.LINKS`, `PAYMENT.ORDER`, `TEC.ITEMS`, `TRANSACTION`

---


### 1.21  Future Dated Conditions


> **📇 Quick Reference Card**
> 
> **Purpose:** *The banks can introduce number of features that allow the customers to invest in deposits, which can offer to:*
> 
> **Applications:** `AA.SCEHDULED.ACTIVITY`, `AA.SCHEDULED.ACTIVITY`
> 
> **Key Fields:** *Arrangement*, *GB Narrative*, *Rate*, *Type*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The banks can introduce number of features that allow the customers to invest in deposits, which can offer to:

- Waive charges for a certain period.
- Allow additional interest, when the deposit remains with the bank for a certain time.

These features are addressed by introducing the Future Dated Conditions functionality to the deposit product. Changes to these conditions are automatically updated to the arrangement based on the relative date concept available in the AA arrangement framework.

There are no specific differences related to defining and processing future dated conditions in deposits, using the TBC.


#### ⚙️ Configuration

The Property Class includes future dated conditions only if the Type field displays the FORWARD.DATED value. It then enables the bank user to introduce a future dated condition at arrangement level.

The bank can offer different types of products to target a particular segment of customers. To facilitate this, the bank can offer options to the customer that can be made available after a specific period. For example, the bank can,

| Column 1 | Column 2 | Column 3 |
|---|---|---|
| Additional Interest | Transaction Charges | Bonus |
| Provide additional interest as an incentive for retaining deposit for a specific period. For instance, half a percent increase if the deposit remains with the bank for 6 months. A future dated interest condition is used for increasing the deposit interest rate after 6 months. | Apply no(zero) transaction charge for first month of arrangement and charge $10 for each transaction from the next month. A future dated condition can be set for Charge Property Class effective the date of required change or relative date like 'START + 6 month'. The system automatically schedules the update of new condition at arrangement level. On the schedule date during SOD of the COB the scheduled activity is processed, thereby applying the new condition to the arrangement. | Define the bonus charge payable to the customer with a future date when certain conditions are satisfied. For instance, no partial withdrawal of deposit can be awarded with a bonus |

The Arrangement Activity screen displays the current and future dated charges in the Charge Property Class.

The Future Dated Charge Condition is set to trigger on 31st May 2018 using the DEPOSITS-CHANGE-BONUS Activity. The scheduled activity displays in AA.SCEHDULED.ACTIVITY .


#### 🔧 Working With

The Future Dated Conditions feature is explained with an example of a change in the Payment Schedule of an existing deposit contract. As shown in the below screenshot, effective 24 Apr 2019, in the Rate field the user adjusted the Deposit Interest, from 2 to 1.5 percentage.

The payment due on 24 Apr 2019, reflects the recalculated interest and associated charges as displayed in the below screenshot. Further, the scheduled change in the deposit interest spread is evidenced in AA.SCHEDULED.ACTIVITY record under the DEPOSITS-CHANGE-DEPOSITIN Activity with the effective date set to 24th Apr.


#### 📋 Tasks

Related topics:

- Amend Deposit (AA)

The banks can have specific features after a specific period , which allow customers to invest in deposits and retain high profile customers.


##### Workflows

This section allows the user to perform the following activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Find Deposit Arrangements | Enter an account arrangement ID in the Arrangement field and then click the FIND button. Click the Overview icon corresponding to a record. |
| Arrangement Overview (Deposit) | Click New Activity option. |
| New Activities | Click the Do Activity Today icon corresponding to Change Deposit Interest (User) activity. |
| Arrangement Activity | Enter a value in the GB Narrative field. Click the Validate icon. Click the Deposit Interest section and then click the Calculation tab. Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

There are no Outputs available for Future Dated Conditions feature.


> **Related Applications:** `AA.SCEHDULED.ACTIVITY`, `AA.SCHEDULED.ACTIVITY`

---


### 1.22  Interest


> **📇 Quick Reference Card**
> 
> **Purpose:** *The bank pays interest on the deposit amount, for the entire tenure of the deposit account, of the customer. The rate of interest remains constant during the entire contract of the deposit and the bank can modify the interest under certain business circumstances, such as increase in deposit amount o...*
> 
> **Applications:** `AA.PARAMETER`
> 
> **Key Fields:** *Arrangement*, *GB Narrative*
> 
> **Sections:** 📖 Introduction | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The bank pays interest on the deposit amount, for the entire tenure of the deposit account, of the customer. The rate of interest remains constant during the entire contract of the deposit and the bank can modify the interest under certain business circumstances, such as increase in deposit amount or retain a high net-worth client. The customer can opt for:

- Scheduled pay out of interest
- Capitalisation of the interest amount.

In case of capitalisation, it is possible to calculate interest on the increased capital. The interest applicable for the deposit account can be tiered. It is also possible to apply negative interest rates, though on specific products.

Scheduled activities (such as MAKE DUE, CAPITALISE, and so on) are processed during start of the day (SOD) for the Deposits product line by default. In case of last day (last or both) inclusive setup, the interest is paid or capitalised at SOD which can lead to incorrect interest calculation, if there is a change in the deposit balance on the scheduled date. In such a case AA.PARAMETER can be configured to move specific scheduled activities to the end of day (EOD) processing.

For deposits in the TBC, the interest amount, as per the Payment Schedule definition, can be:

- Capitalised to the same deposit account
- Paid to another account within the TBC
- Forwarded as a settlement request, by publishing an event to an account or beneficiary outside the TBC, which should be consumed by an external payments system for further processing.


#### 📋 Tasks

Related topics:

- Amend Deposit (AA)

The bank can modify the interest under certain business considerations, such as, increase in deposit amount or retain a high net worth client.


##### Workflow

This section allows the user to perform the below activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Find Deposit Arrangements | Enter an account arrangement ID in the Arrangement field and then click the FIND button. Click the Overview icon corresponding to a record. |
| Arrangement Overview (Deposit) | Click the New Activity option. |
| New Activities | Click the Do Activity Today icon corresponding to Change Deposit Interest (User) activity. |
| Arrangement Activity | Enter a value in the GB Narrative field. Click the Validate icon. Click the Deposit Interest section and then click the Calculation tab. Enter values in the following fields: Rate Period Negative Rate Margin Type Operand Margin Rate Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

There are no Outputs available for Interests feature.


> **Related Applications:** `AA.PARAMETER`

---


### 1.23  Interest Adjustments


> **📇 Quick Reference Card**
> 
> **Purpose:** *The bank can introduce changes to a specific deposit arrangement with the current, past, or future date set as the effective date. For example, the bank can introduce changes in the interest spread, effective from a past date.*
> 
> **Applications:** `AA.INTEREST.ACCRUALS`, `AA.PARAMETER`
> 
> **Key Fields:** *Arrangement*, *Fixed*, *Narrative*, *Primary Officer*, *Reconstruct Settlement*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The bank can introduce changes to a specific deposit arrangement with the current, past, or future date set as the effective date. For example, the bank can introduce changes in the interest spread, effective from a past date.

Back value-dated changes can affect balance movement or any other activities which are already performed during this period (that is, from the back value date to the current date). In case the changes will become effective on a future date, these changes will be processed at the Start of Day (SOD) processing, of the effective date.

The Interest and Charges settlement for current or back value dated correction can be:

- Capitalised to the same deposit account
- Collected from / Paid to another account within the TBC
- Forwarded as a settlement request by publishing an event to an account or beneficiary outside the TBC, which should be consumed by an external payments system, for further processing.


#### ⚙️ Configuration

In Retail Deposits module, the system allows the user to negotiate (create, amend, or reverse) the conditions with an effective date that can be set to the current, past, or a future date.

During the back value-dated change, the corresponding calculations are triggered to effect the value-dated changes. The amendments related to the back value-dated changes, are processed in chronological order.

During the modification of the arrangement conditions, the system modifies the related balances, and re-executes the calculations, so that the arrangement status reflects the final status of the deposit arrangement, based on the activity triggered.

When a back dated activity is processed, the Reverse and Replay process performs the adjustments on the arrangement based on the back value date. For instance, the bank introduces a change in the interest rate effective on a back date, then the Update Interest Activity triggers the reverse and replay process. This, in turn, triggers the reversal of all the entries, up to the back value date and re inputs the entries (replay), after the update of Interest Activity.

The Reconstruct Settlement field in AA.PARAMETER is used in Back Dated Settlement processing.

This is a system wide parameter which controls the behavior of a reverse and replay scenario. When a back dated activity is triggered on an arrangement and the Reconstruct Settlement field is set to AUTOMATIC, the system performs a reverse and replay of the backdated settlement processing to a settlement account based on the updated conditions in the arrangement.

When an arrangement is created with a back value effective date, any initial back dated settlement processing does not depend on the above-mentioned parameter setting. In this case, the system automatically performs the back dated settlement processing for the new arrangement

> **⚠️ Note:** The upgrading clients may not choose to invoke this feature, so a system parameter controls this. This is a no-change field, with an override being provided to the user.

The Interest and Charges settlement for current or back value dated correction, can be:

- Capitalised to the same deposit account
- Collected from / Paid to another account within the TBC
- Forwarded as a settlement request by publishing an event to an account or beneficiary outside the TBC, which should be consumed by an external payments system, for further processing.


#### 🔧 Working With

The screenshot below displays interest adjustment and the associated impact on the bills generated earlier. A back-valued interest adjustment triggers the system to recalculate and adjust the bill amount depending on the effective date applicable for the change. In this particular case, the system adjusts the rate to add 0.25% spread on the base rate effective 25 Mar 2019. The current system date is 17 Apr 2019 and deposit start date is 20 Mar 2019. The system automatically recalculates and adjusts the amount on the bills generated.

The bill generated activity is reversed and replayed as seen below.

The AA.INTEREST.ACCRUALS holds the information of the interest rate that is used to accrue the interest. The change in interest rate during the interest accrual period is reflected here.


#### 📋 Tasks

Interest Adjustments allows automatic recalculation and correction of related arrangement balances when back-valued activities are processed. The correction processing takes place in real-time and is initiated by the submission of a back-dated Arrangement Activity.


##### Workflow

This section covers various types of Interest Adjustments.

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Find Deposit Arrangements | Enter a deposit arrangement ID in the Arrangement field and then click the FIND button. Click the Overview icon of a corresponding record. |
| Arrangement Overview (Deposits) | Click the New Activity option. |
| New Activities | Click the Do Activity Today icon corresponding to the Change Deposit Interest (User) activity. |
| Arrangement Activity | Enter a value in the Narrative field. Click the Deposit Interest section. Enter a value in the Fixed field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Find Deposit Arrangements | Enter a deposit arrangement ID in the Arrangement field and then click the FIND button. Click the Overview icon of a corresponding record. |
| Arrangement Overview (Deposits) | Click the New Activity option. |
| New Activities | Click the Do Activity Today icon corresponding to Renegotiate Arrangement activity. |
| Arrangement Activity | Enter a value in the Narrative field. Click the Account Officers tab. Enter a value in the Primary Officer field. Click the Deposit Interest tab. Enter values in the following fields: Rate Period Negative Rate Margin Type Operand Margin Rate Spread Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to Interest Adjustments in the core banking system.


##### Enquiries and Reports

NA


##### SWIFT Messages

NA


##### Advices

The below list of advices are generated by the core banking system pertaining to Interest Adjustments.

This advice specifies the details such as, Account details, Interest details, Interest schedule details, if there is a change in the rate of interest.


##### Alerts

NA


> **Related Applications:** `AA.INTEREST.ACCRUALS`, `AA.PARAMETER`

---


### 1.24  Migration Process


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Temenos' system, when implemented in a new site replaces the legacy system. During migration, the existing contracts in the legacy system need to be transferred to the new system, which is referred as takeover. Such migration activity is supported by AA where the legacy accounts are integrated i...*
> 
> **Applications:** `AA.ARRANGEMENT.ACTIVITY`, `ACCOUNT`, `ACCOUNT.ACCRUAL`, `CUSTOMER`, `FT.COMMISSION.TYPE`
> 
> **Key Fields:** *Activity*, *Arrangement*, *Auto Pay Acct*, *Charge Account*, *Effective Date*, *Field Name 1.1*, *Field Name 1.2*, *Field Name 1.3* ... +15 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The Temenos' system, when implemented in a new site replaces the legacy system. During migration, the existing contracts in the legacy system need to be transferred to the new system, which is referred as takeover. Such migration activity is supported by AA where the legacy accounts are integrated into the Temenos' system. The balances, such as, current and accrued can be updated using the relevant AA Activity.

Live deposits can be migrated from the legacy system to the TBC when the TBC replaces the existing system. Read here to know more on migration of deposits in TBC.


##### Retention of AZ Account Numbers for AD

The objective of this feature is to provide the ability to retain the AZ account number during the takeover of an AD arrangement. Subsequently, the account gets fully operational as an AD arrangement, so there is no customer impact for upgrading clients who chooses to move their AZ Deposit into the AA ecosystem.

This feature allows retaining the AZ account number during the takeover of an AD arrangement.

This feature does not support,

- Automatic porting AZ conditions into AD
- Automatic conversion of AZ accounts into AD arrangements.
- Automatically import the deposit’s principal balance into the AD arrangement

All steps are similar to the AZ–AR conversion covered except the below.

- Premature closure of the AZ Deposit Settle the balances to an internal account
- AZ reference gets removed from ACCOUNT record and is effectively a zero balance account
- Now, use this ACCOUNT number in the DEPOSITS-TAKEOVER-ARRANGEMENT

Once it is attached to the AD arrangement, takeover balances into the AD using normal balance takeover activities.

- Training or Services engagement during upgrade scoping to train the bank on AA and AD.
- Key points for consideration and decisions made before moving an AZ account to AD arrangement The AD Product Catalog AD Product Conditions and Negotiation Rules A decision on whether the AZ accounts taken over into AD retain their existing conditions or unified under new product conditions. It is possible to make a one-time product setup change that allows existing deposits to retain their conditions and then subsequently change the product conditions before opening up the system for production.

- AZ Deposit to be pre-closed online with its balances are settled to a nominated account. This results in the AZ account being converted into an AC account but with no balances.
- Run Close of Business.
- At start of business, use Deposits Takeover Activity to create new AD Arrangements Specify the relevant AC account number in the Account Property. Pass the AC account number once the validations are accepted Results in AC account becoming the account reference for the AD arrangement.
- The balances are taken over into the AD arrangement using normal migration tools similar to a takeover of a Deposit from a legacy system.

- Previously, when an existing account number is specified in the Account Property during Deposits Takeover Activity, the system raises an error.
- AZ Deposit account has an underlying AC account record. During the takeover as an AD arrangement, the same AC account number is specified in the AD arrangement in order to maintain continuity from the customer perspective.
- The feature allows user to attach an existing AC account to a new AD arrangement as part of Takeover Activity, provided the validations are satisfied. This is permitted only when the AC account is zero balance (No balances including accrued interest should exist). The Takeover Activity results in the arrangement ID in ACCOUNT and other relevant cross-references between account number and arrangement reference and the account becomes operational as an AD deposit. Certain other pre-conditions to be met by the AC account are discussed in the Configuring Migration Process section.
- The takeover is done at the Start of Day immediately after the AZ Pre-closure During the Takeover The Original Contract Date must be the AZ Opening Date. Takeover balances to be done as per normal migration tools and processes.
- Once the above steps are completed, no back dated transaction or activity can be done beyond the takeover date.


#### ⚙️ Configuration

The following general approach is recommended for executing takeover arrangement:

- Analyse existing products and create equivalent products using the Retail Deposits (AD) module
- Determine requirement for historic data in Temenos' system
- Prepare extract of legacy deposit contract data and balances
- Create new arrangements from the legacy deposit contract data
- Create outstanding legacy bills
- Update penalty balances

During the migration of data from the legacy system to Temenos' system, it is possible to improve the performance of the takeover process by updating certain AA tables through a background service. Read Customer Arrangement Offline Update for more information.


##### Retention of AZ Account Numbers for AD

This functionality has been built around the Deposits Takeover Activity to move the AZ Deposit as zero balance, attach it to an AD arrangement and then bring the balance back into the arrangement.

The Deposits-Takeover-Arrangement Activity now allows an existing AZ Deposit with an underlying AC number to be attached, subject to passing below validations.

The Takeover Activity results in an error during the below scenarios.

- The Orig Contract Date does not match with AZ Opening Date
- INT.NO.BOOKING is not “”)
- The account has unauthorised movement
- The account is marked for Pending Closure or in Closed status
- The account is linked with another account for Interest or Charge Liquidation Interest Liqu Acct Int Liqu Acct and Charge Account fields in the ACCOUNT record
- The account is part of Interest Compensation Pool Int Comp Acct field in ACCOUNT record
- The Account has an Auto Pay Acct field in ACCOUNT (R17)
- AA Interest validation If taking over an AC account – and if Last Day Inclusive Y in ACCOUNT.ACCRUAL , then Interest Accrual Rule must be BOTH If it is N, then Interest accrual must be FIRST
- All In One Product If this attribute is set in ACCOUNT record, then Takeover should return an Error
- Suppress Business Events Events should not be qualified because of this Debit or Credit accounting happens on the AZ Deposit and AD

Scenarios exempted from validations and error are listed below.

- Account having Locked Balance
- Account having F Entry
- Account having Charge Accruals – based on FT.COMMISSION.TYPE – not a problem
- Account having Charge Amortisation – based on FT.COMMISSION.TYPE – not a problem


#### 🔧 Working With

| Column 1 | Column 2 |
|---|---|
| ACTIVITY | DEPOSITS-TAKEOVER-ARRANGEMENT |
| Effective date | Deposit contract start date in Temenos' system |
| Customer | Customer ID as available in the Temenos' system |
| Product | The name of the product created as an equivalent to the legacy product. |
| Currency | Currency of the deposit as in the legacy system |
| ORIG.CONTRACT.DATE | Original start date of the legacy contract (only for information) |


#### 📋 Tasks

There are no Tasks available for Migration Process feature.


#### 📊 Outputs

There are no Outputs available for Migration Process feature.


> **Related Applications:** `AA.ARRANGEMENT.ACTIVITY`, `ACCOUNT`, `ACCOUNT.ACCRUAL`, `CUSTOMER`, `FT.COMMISSION.TYPE`

---


### 1.25  Migration RFR LIBOR


> **📇 Quick Reference Card**
> 
> **Purpose:** *There is a business need for banks to be able to identify which contracts would require a rate change to RFRs and migrate them away from LIBOR.*
> 
> **Applications:** `AA.ACTIVITY.HISTORY`, `AA.ARR.INTEREST`, `AA.INTEREST.DETAILS`, `AA.SCHEDULED.ACTIVITY`, `RFR.CONDIITON`, `RFR.CONDITION`, `RFR.MIGRATION`, `RFR.MIGRATION.DETAILS`
> 
> **Key Fields:** *Admin*, *Application Field Name*, *Application Field Name, Field Operand, and Value From, Value To*, *Application Name*, *Context Name Value*, *Default RFR PI Key*, *Default Spread*, *Exclude Application Field* ... +30 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

There is a business need for banks to be able to identify which contracts would require a rate change to RFRs and migrate them away from LIBOR.

The automated migration tool assists the banks to have capabilities to validate multiple contracts in one selection and convert from (L)IBOR to RFRs in one go. This tool helps in identifying the live contracts that are linked to IBOR rates based on the user selection criteria that will be eligible for conversion and convert them successfully.

The features related to Migration of LIBOR Deposit Contracts to Risk Free Rates are not applicable for deposits in TBC. Read here to know more about TBC for deposits.


#### ⚙️ Configuration

The conversion from a (L)IBOR contract to a RFR contract cannot happen mid interest period and the recommendation is to complete the task on the current interest capitalization point.

The migration conversion process is handled by the following application and service.

- RFR.MIGRATION
- RFR.CONDITION
- RFR.MIGRATION.DETAILS
- Service – RFR.MIGRATION.SERVICE

The migration process itself is performed as two-step processing.

- Preview Mode – To update the migration related tables with the expected changes for eligible contracts.
- Execute Mode – To carry out the actual migration to update the Live contracts with new RFR fields and details.


##### RFR.MIGRATION

The basic selection criteria for migration with respect to application and the logistics like version for conversion is defined to select the list of contracts that require conversion from (L)IBOR to RFR.

The RFR.MIGRATION table has the following attributes and accepts the appropriate values to it. The records are selected for conversion based on the configuration given in this table. The record ID for this table a free text field and the user can create one with any alphanumerical value.

- GB Description – Indicates the description of the record
- Application Name – Indicates the application or product name that records for conversion belong to
- IBOR Cut Off Date – Indicates the IBOR discontinuation Date. Mandatory input
- Version Name – Indicates the valid version of application to be used for migration process by the OFS Routine OFS Routine – Indicates the API to perform the RFR Migration. Currently only AA.PERFORM.RFR.MIGRATION is accepted
- Mode –Identifies the process stage of the migration. Preview – Indicates the verification process and does not update the contract at this stage. Execute – Indicates that actual contract update is carried out.
- Int Period End Date – Indicates the interest period end date of the contract. Valid Date - Indicates that the migration API would identify the contracts that are greater than or equal to this date and the next working date. Blank – The migration API would identify all the contracts that are eligible for migration with respect to other conditions.
- Application Field Name – Indicates the field name from the application to be used as a selection
- Field Operand – Indicates the operation to be performed on the field during the evaluation of the contract between the selections. Values allowed are EQ; GE; GT; LE; LK; LT; NE; NR; RG. Mandatory input for the field operand RG
- Value From – Indicates the value to be verified from the application or product with respect to Application Field Name
- Value To – Indicates the Value to be verified upto, from the application or product with respect to Application Field Name

Routine Name – Indicates user-defined API can be attached to this field to get the list of arrangements to perform the migration.

> **⚠️ Note:** Conditions defined ( Application Field Name, Field Operand, and Value From, Value To definition) and Routine Name attributes are mutually exclusive.

This record can be viewed and amended in RFR.MIGRATION.LIST enquiry.

Sample version that can be attached to RFR.MIGRATION is shown below.


##### RFR.CONDITION

The RFR.CONDITION table is used to define the exclude contract conditions and include the new Periodic Interest key and the adjustment spread information with respect to RFR. The record if of this table must be a valid AA product. The following attributes conditions are defined.

- GB Description –Indicates the description of the record
- Exclude Application Field – Defines exclude condition after the selection of records based on selection definition in RFR.MIGRATION .

To exclude contracts with PERIODIC.INDEX value as ‘11’ from Interest property class.

> **⚠️ Note:** The field name could be any valid field from any of the Property class of the arrangement.

- Exclude Field Operand – Defines the operand for selection. The values allowed are EQ; NE; LT; GT; etc.

- Exclude Value From – Defines the field value for the Exclude Application Field .
- Exclude Value To –Define the field value range that would be excluded from the migration process
- Exclude Field Operation – Defines the Operation to be used when there is more than one condition exist. Mandatory input when multiple conditions are to be processed together.
- Default RFR PI Key – When none of the conditions are satisfied, this default key value is used for conversion
- Default Spread - – When none of the conditions are satisfied, this default spread value is used as adjustment spread for conversion.The spread value can be input along with ‘+’ or ‘-‘sign and is considered as Margin Operand .
- RFR PI Key – When the conditions are satisfied, this value is used as RFR Key for contracts in conversion.
- RFR Delta Spread - When the conditions are satisfied, this value is used for conversion.The spread value can be input along with ‘+’ or ‘-‘sign and would be considered as Margin Operand .This spread value is added or subtracted to the Margin Rate.
- RFR Int Property – Identifies Multiple Interest Property.

> **⚠️ Note:** If same RFR PERIODIC.INTEREST key is used for multiple Interest properties, will still need to define all the properties separately.

- Application Field Name – Specifies a Valid name from any of the property class that is part of the arrangement.

To exclude contracts with PERIODIC.INDEX value as ‘05’ from Interest property class.

- Field Operand – Specifies the operand to be used while selecting the data from the Application Field name
- Field Value From – Indicates the value to be verified against the field value of the application during the evaluation of the contract.
- Field Value To - Defines the range of the field value
- Field Operation – Defines The operation to be performed when multiple conditions are defined.Options – And; OR This record can be viewed and amended in RFR.MIGRATION.LIST enquiry.


##### RFR.MIGRATION.DETAILS

Migration contract information is recorded in this table while processing data, based on the selection criteria of include and exclude conditions defined in RFR.MIGRATION and RFR.CONDITION .

The applicable ID to this table updated by the system are

- @ID: RFR.MIGRATION table ID – Preview
- @ID: RFR.MIGRATION table ID – Execute

Launch RFR.MIGRATION table in preview mode to initiate migration and this updates the RFR.MIGRATION.DETAILS table with selected data with id Rfr Migration Id-Preview.

The migration check can be run multiple times in preview-mode for verification without impacting the underlying contracts. The selection validates the following conditions.

- Contract is linked to Periodic Interest Key
- Contract Maturity Date is greater than the IBOR Cut-off Date and the Current Int Period End Date
- Contracts that satisfied the Exclude conditions has Exclusion Flag set as ‘Yes’ in RFR.MIGRATION.DETAILS table.
- Contracts that satisfy conditions other than the Exclude conditions are assigned with values from RFR PI Key and RFR Spread
- Contracts with none of the conditions satisfied are assigned with Default RFR PI Key and Default Spread .

RFR.MIGRATION.SERVICE should be started from TSA.SERVICE after defining the selection criteria.

The service API updates the RFR.MIGRATION.DETAILS for preview mode as below.

The selection can be viewed using MIGRATION.DETAILS enquiry for PREVIEW mode

Preview mode of RFR Migration Process – Flow Diagram

Execute mode should be triggered only after the verification of the results from the preview mode.

> **⚠️ Note:** This mode is applicable only for the Interest period end date and the inbuilt intelligence ensures that the mode is triggered only once.

Launch the RFR.MIGRATION again in Execute mode, after thorough verification of results from preview mode. Upon authorization, the data with ID as ‘-Preview’ is selected from RFR.MIGRATION.DETAILS.

The execute mode runs the following eligibility check again to ensure integrity of data.

- Contract is linked to Periodic Interest Key
- Contract Maturity Date is greater than the IBOR Cut-off Date and the current Interest Period end date
- Contracts that satisfied the Exclude conditions has ‘ Exclude Flag’ set as ‘Yes’ in RFR.MIGRATION.DETAILS table
- Contracts that satisfy conditions other than the Exclude conditions are assigned with values from RFR PI Key and RFR Spread
- Contracts with none of the conditions satisfied are assigned with Default RFR PI Key and Default Spread .

The Migration API updates the RFR.MIGRATION.DETAILS with ID as ‘-Execute’. The OFS responses for each migrated contract will be recorded in the details table for verification and reconciliation purpose.

RFR.MIGRATION.SERVICE should be started from TSA.SERVICE after defining the selection criteria.

The API updates the eligible contract by triggering Change-Interest Activity and also the execution results to the migration details table along with migration status.

> **⚠️ Note:** For contracts having multiple Interest properties have multiple respective change Interest activity triggered for the properties.

OFS Error messages if any at the time of posting the records will be captured in the attribute Migration Status and otherwise Success.

Successful Migration is updated as below.

The Migrated contract lists status can be viewed using MIGRATION.DETAILS enquiry and MIGRATION.OFS.STATUS

Execute mode of RFR Migration Process – Flow Diagram


##### Migration Types

The migration is possible only for the scheduled Interest properties on the capitalisation date. There are two types of migrations possible by using the migration tool.

- Current dated Migration – The migration happens on capitalisation date set as current date.
- Future dated Migration – The migration happens on capitalisation date set as a Future date.

> **⚠️ Note:** Back dated migration is currently restricted and not possible to perform by using RFR.MIGRATION .

The current dated migration is Int Period End Date or the capitalisation date for the given interest period is set as current date..

The below screen shot is example for the current dated migration where the Int Period End Date and the Current system date are the same. Based on this definition the system selects the list of arrangements whose current period end date is 15-April-2021. and posts the OFS message to convert the LIBOR to RFR.

The Future dated migration is when the Interest period end date or the capitalisation date is a future date and not a business date. The below screen shot is example for the future dated migration where the Int Period End Date is greater than the current system date.

Base on this definition the system selects the list of arrangements whose current period end date is 19- April-2021. The DEPOSIT -RFR.MIGRATION-INTEREST is scheduled for the Int Period End Date and is triggered during the COB for conversion.

> **⚠️ Note:** Changes executed through auto-migration cannot be rolled back and should be handled manually. Due to the fact that all RFR interest properties should be scheduled in the payment schedule definition, both Principal Interest Property and Penalty Interest Property should have same payment frequency. Interest properties with the type Accrue by Bills cannot be migrated to new RFR rates. Penalty interest property condition with open period and no schedule definitions cannot be migrated using the auto migration tool and should be handled manually. Multi-Tiers with different Interest types like Floating, Fixed and Periodic cannot be migrated using migration tool. Back dated migration cannot be performed using the auto-migration tool. Arrangements with OVERDUE balances cannot be migrated using the auto-migration tool and should be migrated manually.


#### 🔧 Working With

The following section describes the current and future dated migration with illustrations.


##### Illustration 1 – Current Dated Migration

Consider a Current dated migration of the product 6Months Term Deposit from LIBOR Periodic index to RFR Periodic Index.

In this example, the Interest Conditions for the 6months Term Deposit product is DEPOSITINT and the Int Period End Date April 15, 2021.The RFR.MIGRATION is set to select the data with Int Period End Date as April 15, 2021 and only for records with currency as USD. IBOR Cut-off date is same as system date April 15, 2021.

Using the RFR.MIGRATION.LIST enquiry, the user can view and amend the RFR.MIGRATION record.

The RFR.CONDITION is configured to exclude records that have Periodic Index as 11 for the Interest Conditions. The ‘include’ condition is set to select all records with Periodic Index as ‘05’. The records that satisfy include conditions migrate to RFR PI key 96

Using the RFR.CONDITION.LIST enquiry , the user can view and amend RFR.CONDIITON record.

Launching RFR.MIGRATION and defining conditions in preview mode updates the RFR.MIGRATION.DETAILS as below before running the TSA.SERVICE.

Run TSA.SERVICE for RFR.MIGRATION.SERVICE for the respective company (say BNK/RFR.MIGRATION.SERVICE). See the RFR.MIGRATION.DETAILS updated in preview mode with the selected contracts based on include and exclude conditions.

The user can preview the Migration Details in preview mode for verification by running the MIGRATION.DETAILS enquiry for PREVIEW mode.

Launching RFR.MIGRATION in EXECUTE mode updates RFR.MIGRATION.DETAILS as follows.

Execute TSA.SERVICE BNK/RFR.MIGRATION.SERVICE again for RFR.MIGRATION Execute mode.

The user can view the migration records by running the MIGRATION.DETAILS and MIGRATION.OFS.STATUS enquiries respectively in EXECUTE mode.

The AA.ARR.INTEREST conditions before conversion is shown below.

The AA.ARR.INTEREST conditions after conversion is shown below.

The AA.ACTIVITY.HISTORY is updated with the latest activity ‘LENDING-CHANGE-DEPOSITINT’ executed for the contract.

See the RFR MIGRATION DATE updated as Context Name Value pair in the Arrangement Activity. It can be drilled down from the Activity log.


##### Illustration – Future Dated Migration

Consider a future dated migration of the product 6 Months Term Deposit from LIBOR Periodic index to RFR Periodic Index.

In this example, the Interest Conditions for the 6 month Term Deposit product is DEPOSITINT and the Int Period End Date April 19, 2021. The RFR.MIGRATION is set to select the data with Int Period End Date as April 19, 2021 and only for records with currency as USD. IBOR Cut-off date is same as system date April 15, 2021.

Using the RFR.MIGRATION.LIST enquiry the user can view and amend the RFR.MIGRATION record.

RFR.CONDITION is configured to exclude records that have Periodic Index as 11 for the Interest Conditions.

The ‘include’ condition is set to select all records with Periodic Index as ‘05’. The records that satisfy include conditions migrate to RFR PI key 96.

Using the RFR.CONDITION.LIST enquiry the user can view and amend RFR.CONDITION record.

Launching the RFR.MIGRATION and defining conditions in preview mode updates the RFR.MIGRATION.DETAILS as below before running the TSA.SERVICE.

Run TSA.SERVICE for RFR.MIGRATION.SERVICE for the respective company. Say BNK/RFR.MIGRATION.SERVICE.

See the RFR.MIGRATION.DETAILS updated in preview mode with the selected contracts based on include and exclude conditions.

The user can preview the Migration Details in preview mode for verification by running the MIGREATION.DETAILS enquiry in PREVIEW mode.

Launching RFR.MIGRATION in EXECUTE mode updates RFR.MIGRATION.DETAILS as follows.

Execute TSA.SERVICE BNK/RFR.MIGRATION.SERVICE again for RFR.MIGRATION Execute mode.

The user can view the migration records by running the MIGRATION.DETAILS enquiry in Execute mode.

For the records with Migration Status as Success, the contracts has the activity ‘DEPOSIT-RFR.MIGRATION-DEPOSITINT’ scheduled in AA.SCHEDULED.ACTIVITY for the Int period end date.

> **⚠️ Note:** Once RFR.MIGRATION has run in EXECUTE mode, the migration related details get updated in the AA.INTEREST.DETAILS table for the arrangement. When the system reaches the future scheduled date, then the RFR.MIGRATION activity gets executed in COB and converts the LIBOR contract to RFR.

ENQ RFR.MIGRATION.LIST

The user can view and amend the RFR.MIGRATION records using this enquiry.

ENQ RFR.CONDITION.LIST

The user can view and amend the RFR.CONDITION records using this enquiry.

ENQ MIGRATION.DETAILS

This enquiry gives the view of the migrated and not migrated contracts. The selection Migration ID and the mode of execution are mandatory to execute the enquiry. The user can run the enquiry in Preview mode and Execute mode individually to verify the data.

ENQ MIGRATION.OFS.STATUS

The selection Migration ID and the Mode of execution are mandatory to execute the enquiry.

Migration Status with Error is shown as below.

Menu

The following menu item is available for easy access for the tables. RFR Migration setup menu can be accessed under Admin Menu:

- Capture Migration Request – To access RFR.MIGRATION table
- View/Amend Migration Request – To view or amend RFR.MIGRATION record
- Define RFR Conditions – To access RFR.CONDITION table
- View/Amend RFR Condition – To view or amend RFR.CONDITION record
- View Migrated Contracts – To view records from RFR.MIGRATION.DETAILS table
- View Migration OFS.STATUS – Enquiry to view the OFS Status details of the contracts.


#### 📋 Tasks

There are no Tasks available for Migration of Deposit Contracts from (L)IBOR to RFR feature.


#### 📊 Outputs

There are no Outputs available for Migration of Lending Contracts from (L)IBOR to RFR feature.


> **Related Applications:** `AA.ACTIVITY.HISTORY`, `AA.ARR.INTEREST`, `AA.INTEREST.DETAILS`, `AA.SCHEDULED.ACTIVITY`, `RFR.CONDIITON`, `RFR.CONDITION`, `RFR.MIGRATION`, `RFR.MIGRATION.DETAILS`

---


### 1.26  Misc


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


### 1.27  Notice for Redemption of Funds


> **📇 Quick Reference Card**
> 
> **Purpose:** *Notice deposit refers to a fixed-term certificate of deposits held with a financial institution that permits withdrawals without penalty only after an advance notification is given.*
> 
> **Applications:** `AA.ACTION`, `AA.ARRANGEMENT.ACTIVITY`, `AA.BILL.DETAILS`, `AA.BILL.TYPE`, `AA.PAYMENT.TYPE`, `AC.EVENTS`, `AC.LOCKED.EVENT`, `AC.LOCKED.EVENTS` ... +5 more
> 
> **Key Fields:** *Application Order*, *Avail Expiry Date*, *Avail Start Date*, *Available
 Start Date*, *Available Expiry Date*, *Available Start Date*, *Batch Stage*, *Beneficiary* ... +34 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Notice deposit refers to a fixed-term certificate of deposits held with a financial institution that permits withdrawals without penalty only after an advance notification is given.

The Notice Withdrawal functionality helps to capture the notice for term deposit breaks or withdrawal of funds from the notice deposit account.

The requested funds can be made available for withdrawal on a business or calendar date. The notice funds can be automatically settled to the customer’s account or an external beneficiary.

Financial Institutions can charge a fee for breaking the term of notice deposits without providing any notice and or when notice conditions are not met.

When the end-user captures or modifies or cancels a notice for withdrawal of funds from the front-end through an API, the system performs the corresponding activity in TBC to process the notice details for the deposit. There are no specific limitations for notice withdrawal features for deposits in TBC.


#### ⚙️ Configuration

Financial Institutions may offer notice deposit products that require customers to submit a notice in advance to break the term deposit either by a full or partial withdrawal.

The Notice Withdrawal transaction class provides the ability to initiate and maintain such break-notice withdrawal requests. The notice capturing details like Notice Period , Notice Availability and so on can be configured in the Balance Availability property condition.

Read Balance Availability and Notice Withdrawal property classes for more information.

The creation, update, and cancellation of notices within the TBC, are performed through the provided APIs. When the notice amount is made available for withdrawal on the Available Start Date or when the entire amount in the Available for Withdrawal balance is reversed on the Available Expiry Date , the TBC publishes an event, which can be consumed by an external General Ledger (GL) system, or others, for further processing.


##### Capturing Notices

To capture a new notice, the DEPOSITS-CAPTURE-NOTICE.WITHDRAWAL activity class is used to display the notice withdrawal transaction class.

> **⚠️ Note:** This activity is enabled only for the products with Balance Availability property class and can never be a forward dated activity.

A notice is captured using the Create a New Notice link or the New Activity link for Capture Notice Withdrawal from the Arrangement Overview page. The user can optionally record the reason for the notice at the time the notice is captured in the Notice Reason field. The list of reasons allowed in the Notice Reason field can be locally configured through EB.LOOKUP , where the record ID has the Notice Reason * format.

- If the customer tries to capture a notice for a non-notice deposit account (that is, Notice Account field is not set in the Balance Availability condition), the system raises an error.
- Notice Reason can be set only for notice withdrawal-related activities and the system raises an error on failure.
- Scheduled Principal Payment definition is restricted for Notice Deposits as the regular approach to redeem funds from a Notice Deposit account is only after submitting the notice request.

- The Period Type attribute is used to configure the notice withdrawal conditions within and outside of the cooling period. When the user defines ‘Cooling’, the system considers the notice withdrawal parameters such as the Notice Period and Notice Availability attributes as applicable for ‘Cooling’ when notice is captured within the defined cooling period only. Available Start Date and Available Expiry Date at the time of capturing notice are populated based on the definition in the Notice Period and Notice Availability attributes defined for Cooling. When the user defines ‘NULL’, the system considers the notice withdrawal parameters applicable for 'NULL' when the notice is captured outside the cooling period. Available Start Date and Available Expiry Date at the time of capturing notice are populated based on the definition in the Notice Period and Notice Availability attributes defined for 'NULL'. When the user defines ‘NULL’ and not ‘Cooling’, the system considers the notice withdrawal parameters as applicable for ‘NULL’ for both within and outside the cooling period. Depending on the definition in Cooling Period and Notice attributes defined in the Balance Availability property class, the system behaviour is mentioned in the below table. Cooling Period Definition Notice Parameters defined for Cooling - Within Cooling Period Notice Parameters defined for NULL - Outside Cooling Period System Behaviour Yes Yes Yes If notice is captured within the cooling period, notice conditions defined in Cooling are applicable. Else, notice conditions defined in NULL are applicable. Yes Yes No If notice is captured within the cooling period, notice conditions defined in Cooling are applicable. Yes No Yes Notice conditions defined in NULL are applicable from the arrangement creation date. Yes No No Existing system behaviour continues. No Yes Yes Notice conditions defined in NULL are applicable from the arrangement creation date. No Yes No Existing system behaviour continues. No No Yes Notice conditions defined in NULL are applicable from the arrangement creation date. No No No Existing system behaviour continues.
- The Notice Amount attribute allows user-input.
- The following are the conditions applicable for Available Start Date : The system defaults the Available Start Date value based on Balance Availability property conditions and allows user-input as well. When the user-input Available Start Date falls short of the Notice Period , then activity restriction can be defined using the NOTICE.PERIOD periodic attribute to either accept or reject the requested date. When the Available Start Date falls on a non-business date, then the system raises an override: The Available Start Date is not a working date If the number of days in between activity effective date and Available Start Date is not greater than or equal to the Notice Period , then the system raises an override: The Available Start Date is within the notice period. The above validation is not applicable if Notice Convention is set to Backward and if the date is system-calculated. When the user modifies the system-calculated Available Start Date , the system raises an override: The default availability date is modified.
- Available Expiry Date is auto-calculated based on the Notice Availability attribute configured in Balance Availability property class and does not allow user-input.
- Notice Type specifies the type of notice captured and the default option is Withdrawal Notice.

Read Withdrawal with Notice to know more on accounting entries raised when funds are withdrawn with a notice.

- When the customer captures a withdrawal notice and the withdrawal amount is the same as the deposit balance (CUR ), then system raises a validation to request for a closure type of notice.
- Notices are not relevant after the deposit maturity date. Hence, user is restricted from capturing notices once the deposit is moved to either Expired or Pending Closure status.


##### Modifying Notices

Any existing notices can be modified using the DEPOSITS-CHANGE-NOTICE.WITHDRAWAL activity class. This activity can be triggered either from the New Activity Link or through the Notice Details Enquiry from the Arrangement Overview page, which displays all the existing notices.

When the Change Notice withdrawal activity is triggered, the Notice Withdrawal transaction class displays the Notice Amount , Available Start Date and Available Expiry Date prepopulated from the withdrawal notice bill that is being modified.

- When the user triggers the Change Notice Withdrawal activity effective current date to modify the Available Start Date such that it falls on the same day, then the funds availability is processed only in COB. If the user requires the funds availability to be processed online, then the NOTICE.WITHDRAWAL record in the AA.PAYMENT.TYPE application should have the Schedule Type field set to Online.
- If the customer modifies a withdrawal notice, such that the withdrawal amount is the same as the CUR balance, then the system raises an override informing the customer to request for a closure-type notice.


##### Modification Options

The following are the modification options available for notice bills for withdrawal of funds:

- It is possible to decrease the notice amount from the captured notice bill. However, the user can choose to allow or restrict the increase in notice amount that did not serve the full notice period based on the Activity Restriction condition. The NOTICE.AMOUNT.INCREASE periodic attribute is used to check if there is an increase in the notice amount from the previously requested amount within the Notice Period and can be defined to raise an error or override.
- The system-calculated Available Start Date can be modified and it can be accepted or rejected based on the activity restriction definitions.
- Available Expiry Date is auto-calculated based on the Notice Availability configured in Balance Availability property class and is not a user-input field.


##### Cancelling Notices

Any existing notices can be cancelled using the DEPOSITS-CANCEL-NOTICE.WITHDRAWAL activity class. This activity can be triggered either from the New Activity Link or through the Notice Details Enquiry from the Arrangement Overview page, which displays all the existing notices.

When this activity is triggered, the Notice Withdrawal transaction class is displayed with all the details prepopulated from the Notice Withdrawal Bill that is being cancelled. This activity does not allow any data to be edited in the Notice Withdrawal transaction class.

Once committed and authorised, the bill is marked as Expired. When a live Notice Bill is cancelled, the following accounting takes place.

| Column 1 | Column 2 |
|---|---|
| Dr AVL | Cr AVL BL |

> **⚠️ Note:** When an arrangement is cancelled within the Cancel Period with existing active notices, the notice bills in the deposit are also set to Expired.


##### Processing Closure of Notice Deposit

A closure notice request can be given using the Capture notice activity by specifying the Notice Type field as Closure Notice in the Notice Withdrawal transaction class. An info-bill of Bill Type value set as CLOSURE.NOTICE is created, and no accounting entries are raised on capturing the notice for closure.

> **⚠️ Note:** Notice Amount cannot be lodged for a closure notice.

The screenshot below shows the CLOSURE.NOTICE record setup in the AA.BILL.TYPE application.

When the customer fully redeems the funds in the deposit through a closure notice, the funds are settled as per the pay-out rule configuration that settles the interest, charges and account balances in the deposit.


##### Minimum Balance in Notice Deposit

Banks may have a Notice Deposit product with minimum balance requirement. In this case, the Activity Restriction condition can be configured to evaluate the funds withdrawal from the notice deposit to monitor the minimum balance.

The MINIMUM.BALANCE periodic attribute is configured in Activity Restriction to raise an override when the minimum balance of USD 10,000 is not maintained.

Activity Restriction is configured to evaluate the minimum balance rule each time the customer withdraws funds from the deposit.

If the evaluation fails, the resultant action is defined to automatically close the deposit.

The resultant action which has to be triggered can be defined in the AA.ACTION table (in this case, DEPOSITS-REDEEM-ARRANGEMENT).

Activity Restriction can be configured with frequency-based definitions, to evaluate for the minimum balance in the deposit at a defined frequency and automatically close the deposit if the criteria is not met.


##### Processing Notice Withdrawal

The following sections describe the withdrawal types and related accounting entries.

| Column 1 | Column 2 |
|---|---|
| Cr AVL | Dr AVL BL |

| Column 1 | Column 2 |
|---|---|
| Dr CUR | Cr Customer Account |

| Column 1 | Column 2 |
|---|---|
| Dr AVL | Cr AVL BL |

- When a notice request is captured or modified, the system evaluates for any posting restriction (of any debit) at the account or customer level that can affect the withdrawal of funds on the funds availability date and raises an override to indicate the same.
- When posting restrictions (of any debit) are defined for the Deposit Account, the system raises an override if there is a notice request in process that will get affected. Active notices in the Notice Deposit are not evaluated when defining posting restriction at the Customer level. The system evaluates if the Available Start Date of the notice request falls between the posting restriction start date and the expiry date, to raise the validation.
- When a notice request is captured or modified, the system evaluates for any existing notices and the locked amounts in the deposit. If the available balance is less than the notice amount that can affect the withdrawal on the fund availability date, the system raises an override to indicate the same.
- When defining locked amounts for the deposit, the system raises an override if there is a notice request in process that will get affected. When the locked funds are placed manually using the AC.LOCKED.EVENT application, the system checks if the available balance post funds reservation (lock amount) is less than the notice amount of the active notice in the deposit to raise an override message. When the locked events are placed through the GAI , activity restriction can be defined to warn the user about available balance as per configuration. In this case, the CHECK.NOTICE periodic attribute is used for the evaluation. The system raises validation to warn the GAI about the existing active notices prior to the future dated AC.LOCKED.EVENTS to keep the process informed about the available balance.


##### Penalty Fee for Withdrawal without Notice

The customer can make a partial or full withdrawal from a deposit account as an early redemption.

- If the bank allows withdrawal only with a notice, then the same is configured by restricting the deposit pay-out rule activity that settles against the current account balance through the Activity Restriction condition.
- If the bank allows partial or early withdrawal but with a penalty charge, then an activity charge or break rule charge for the Deposit pay-out rule activity should be configured.

A sample configuration where a penalty notice fee is set as activity charge is shown below.

The DEPOSITS-APPLYPAYMENT-PO.EARLY.WITHDRAWAL configured in the Activity Charge property class is the deposit pay-out rule activity that gets triggered when the deposit is withdrawn without notice. That is, it is the Remainder Activity in the pay-out rule condition for withdrawal with notice.


##### Calculating Penalty Fee for Withdrawal without Notice

A charge adjustment routine is configured in the Charge property condition to calculate the penalty fee based on the below formula.

- Interest Day Basis is identified from the first interest property in the arrangement.
- If the Notice attributes are defined for ‘Cooling’ in Period Type, days defined in the Notice Period attribute in the cooling definition are used for penalty fee calculation if withdrawal is done within cooling period. Else days defined in the Notice Period attribute in NULL definition is used for the same.

The below screenshot shows the setup for the WITHDRAWALFEES charge configured as an activity charge in the Activity Charge property conditions. The charge adjustment routine is attached in the Charge Routine field with Charge percentage as 5% on the transaction amount.


##### Penalty Fee for Closure without Notice

A closure withdrawal is processed through a separate activity named DEPOSITS-REDEEM-ARRANGEMENT which is different from a regular withdrawal activity. When the customer tries to close the deposit without notice, a penalty charge can be assessed by configuring the rule break charge.

The CLOSURE.NOTICE periodic attribute is configured in the Activity restriction condition to verify the closure notice bill for the arrangement.

The below screenshot shows the activity charge and activity restriction setup to trigger a closure penalty charge when the customer has redeemed the term deposit without notice. An activity charge is configured for DEPOSITS-REDEEM-ARRANGEMENT activity.

When this charge property is triggered in Activity Restriction, the CLOSURE.NOTICE periodic attribute is evaluated to check if a closure notice exists for the arrangement or not. If there is a closure notice, then the charge is waived. If there is no closure notice, the customer is charged for redeeming the deposit without notice.

The penalty charge for closure has the following setup which is similar to that of a withdrawal penalty charge and the charge is calculated as a percentage on the deposit’s current account balance.


##### Auto Settlement of Funds for Notice Deposits

The Notice funds for withdrawal can be auto-settled on the Available Start Date based on the auto settlement instructions on the arrangement.

The TBC can settle the requested notice amount with another account within the TBC or publish an event for a settlement request to an account or beneficiary outside the TBC, which should be consumed by an external payments system for further processing on the fund availability date. Hence, the payment order related details are not applicable for deposits in TBC.

The funds are settled automatically to an account, maintained within the system, on the Available Start Date .

- The PAYOUT.RULES condition for funds withdrawal through manual transfer and or with auto settlement instructions to a customer account, maintained within the system, should have the Remainder Activity set to Deposits PAYOUT.RULE.
- The funds withdrawal with no notice request triggers the same activity too.

The system triggers the ISSUE.ORDER activity to schedule the payment order before the Available Start Date based on the Order Delivery definition in PAYMENT.ORDER.PRODUCT table and Delivery Days definition in the CURRENCY table.

During the COB of the date, on which the ISSUE.ORDER activity is processed, the payment order is executed to be placed in the warehouse with Payment Execution Date , Credit Value Date , and the Debit Value Date as the Available Start Date .

> **⚠️ Note:** The Warehouse Reqd field in PAYMENT.ORDER.PRODUCT should be set to Yes, if the payment order itself should process the payments. Otherwise, the third-party system should release the payments from the warehouse.

On the Available Start Date , based on the sequence in which the batches are processed during COB, either the withdrawal balance can get created first or the payment order.

- Different Payout Rules conditions should be configured to differentiate the Remainder Activity between funds settled through PAYMENT.ORDER and funds withdrawal without notice. The Payout Rules condition for auto-settlement through payment order in advance (that is, before the AVL balance is created) should have the Remainder Activity set to DEPOSITS-SUSP.PAYMENT-ARRANGEMENT to raise accounting against the SUSPPAYMENT balance. This is to ensure that the funds get debited from deposit account only after the AVL balance is created.
- The funds in transit can be locked in for a balance check based on the Reserve Funds configuration in PAYMENT.ORDER.PRODUCT . Yes - The locked funds are created on the payment execution date. Onsubmit - The locked funds are created on the payment generation date. This configuration makes sure that any later withdrawal on the account with or without notice between the payment generation date and Available Start Date is allowed only for the remaining funds netted to the locked funds.
- The SETTLEMENT-ADVANCE.PAY-PAY-CUR event must be configured in AC.EVENTS to perform automatic settlement of funds using payment order through SUSPPAYMENT. Read AC.EVENTS for more details.
- For auto-settlement through payment order, the Activity Mapping product condition should have the activity DEPOSITS-APPLYPAYMENT- mapped to the corresponding Transaction Code for funds settlement. The debit transaction code used by the payment order product for auto settlement through payment order is configured in Debit Book Code field of PP.HEAVYWEIGHTPRODUCTCOND application.

- When auto settlement instructions are updated after the notice is captured, then the Update Settlement Activity checks the status of the issued bills status to schedule the payout accordingly.
- If the settlement instructions are given after the issue order has been initiated for the payments, then the funds are held in AVL balance and can only be settled manually.
- In case of beneficiary acknowledgment failure, the user should create a manual Payment Order to withdraw the funds. Otherwise, the funds will continue to be available in AVL from the Available Start Date till the Available Expiry Date .


##### Autoclosure of Deposits

The system can be configured with Activity Restriction rules and conditions to automatically close the deposit. Autoclosure is based on the Closure property conditions only. A closure notice can be made mandatory to auto-close the notice deposit.

> **⚠️ Note:** The validation is raised only for user-initiated closure.

- The notice deposit with closure notice and auto-settlement instructions, has the amount scheduled to settle as per the settlement instructions followed by autoclosure (if defined). The closure condition can be defined to close the deposit online or during close of business.
- When the deposit closure is triggered manually using DEPOSITS-REDEEM-ARRANGEMENT, a rule can be defined to mandate the closure type notice as shown.


#### 🔧 Working With

Using the Notice Withdrawal Transaction Class, the user can capture withdrawal notices to withdraw funds from the Notice Deposit.

The Period Type, Notice Amount , Notice Period and Notice Availability fields are configured in the Balance Availability property class.

The amount lesser than the Notice Amount defined in the Balance Availability condition can be withdrawn without issuing a notice request. If the notice withdrawal conditions are not met during the withdrawal of funds, the system raises an override.

In the below screenshot below, the system raises an override during fund transfer, where the customer has withdrawn USD 500 from the deposit account without notice.

The creation, update, and cancellation of notices within the TBC, are performed through the provided APIs. When the notice amount is made available for withdrawal on the Available Start Date or when the entire amount in the Available for Withdrawal balance is reversed on the Available Expiry Date , the TBC publishes an event, which can be consumed by an external General Ledger (GL) system, or others, for further processing.


##### Capturing Withdrawal Notice within or after Cooling Period

The Period Type attribute in the Balance Availability property class is used to define notice conditions within and outside the cooling period.

The notice deposit with the Notice attributes are defined for both within and outside the cooling period.

Consider a deposit product, where the cooling period is defined for seven days through the Closure property class. When the user captures a notice within the cooling period, the system picks up the Available Start Date and Available Expiry Date based on the days defined in the Notice Period and Notice Availability attributes for the cooling definition in Balance Availability product condition.

An arrangement is created on 14 Apr, 2022 and cooling date is 21 Apr, 2022. Notice is captured on 19 Apr, 2022, which is before the cooling date.

- The system defaults 21 Apr, 2022 as Available Start Date by considering the two days specified in Notice Period applicable for Cooling condition
- The system considers 22 Apr, 2022 as Available Expiry Date by considering the one day specified in Notice Availability applicable for Cooling condition

If withdrawal is done without complying notice conditions before cooling date, then the penalty fee is calculated by using the days defined in the Notice Period attribute defined for ‘Cooling’ condition in Balance Availability product condition. In this case, two days are used for penalty fee calculation.

If withdrawal is done without complying notice conditions after cooling date, that is, the Notice is given before cooling date and funds requested for withdrawal after cooling date, then the penalty fee is calculated by using the days defined in the Notice Period attribute defined for ‘NULL’ condition in the Balance Availability product condition. In this case, 14 days are used for penalty fee calculation.

Consider a deposit arrangement, where the cooling period is defined for seven days through the Closure property class. When the user captures a notice outside the cooling period, the system picks up the Available Start Date and Available Expiry Date based on the days defined in the Notice Period and Notice Availability attributes for the ‘NULL’ definition in Balance Availability product condition.

In the below case, the arrangement is created on 6 Apr, 2022 and cooling date is 13 Apr, 2022. Notice is captured on 19 Apr, 2022, which is after the cooling date.

- The system defaults 3 May, 2022 as Available Start Date by considering the 14 days specified in Notice Period applicable for Null condition
- The system considers 5 May, 2022 as Available Expiry Date by considering the two days specified in Notice Availability applicable for Null condition

If withdrawal is done without complying notice conditions after cooling date, penalty fee is calculated by using the days defined in the Notice Availability attribute defined for NULL condition in Balance Availability product condition. In this case, 14 days used for penalty fee calculation.


##### Adjustment of Funds Availability Date for Withdrawal

The date on which the requested fund is available for withdrawal ( Available Start Date ) can be a business or a calendar date based on the Notice Convention configuration.

Consider the following example of a notice deposit with Notice Period set to three days in the Balance Availability product condition. When the customer captures a notice on Apr 15, 2021 for withdrawal of funds, the system calculates the Available Start Date as April 18, 2021 based on Notice Period . Since April 18 is a weekend, the system considers the setup in Notice Convention to decide if Available Start Date should be a business or calendar date.

- When Notice Convention is set to Blank/Calendar, Available Start Date is April 18, 2021 even though it is a non-business day. The system raises an override: The Available Start Date is a not a working day.
- When Notice Convention is set to Forward, Available Start Date is moved to the next working day, April 19, 2021 as shown below.
- When Notice Convention is set to Backward, Available Start Date is moved to the previous working day, April 16, 2021 as shown below.

For moving Available Start Date to the previous business day:

- When Notice Convention is set to Backward, It is not considered as a notice breach when the notice days fall short by the system-calculated previous business date. It is considered as a notice breach when the notice days fall short by the previous business date input by the user. The system raises an override to highlight the notice breach: The Arrangement Start Date is within the notice period. (The Notice Convention setup is not considered when the user manually inputs an Available Start Date .) The arrangement start date cannot be greater than the previous business date. When a notice deposit is opened on a holiday and notice for withdrawal of funds is defined such that Available Start Date is earlier to the deposit opening date, then the system defaults the deposit opening date as the Available Start Date and raises an override: The Available Start Date is not a working date.
- When Notice Convention is not set to Backward,
- When there is a manual request of Available Start Date such that the notice period is compromised, the user can accept or reject it by configuring the activity restriction using the NOTICE.PERIOD periodic attribute. The system raises a default override when the system-calculated Available Start Date is modified. Illustration The NOTICE.PERIOD periodic attribute is set to evaluate and return a value NO in case of a notice breach when the user manually inputs an Available Start Date . Consider an example in which the user is restricted from capturing or changing a notice with a notice breach. The activity restriction is set to trigger the periodic attribute evaluation during the capture or change notice activity and raise an error. A notice deposit is created with Notice Period in Balance Availability condition set to four days. When modifying an already captured notice for withdrawal of funds, the system-calculated fund availability date considering the Notice Convention setup is April 26, 2022. The user has manually changed the date to April 22, 2022 and the system raises an error restricting the user from committing the activity.


##### Capturing Withdrawal Notice in Deposit Accounts

The following illustrations explain the capturing and processing of Notice Withdrawal when the customer withdraws funds from the notice deposit with and without a notice request.

| Scenario | Result | Balance Amount |
|---|---|---|
| On Apr 16, the customer requests a notice for withdrawal of USD 10,000 with Available Start Date Apr 19. | The AVL balance is created for an amount of USD 10,000 on the Available Start Date (Apr 19). | CUR - USD 20,000 AVL - USD 10,000 |
| The user processes a back dated notice capture with value date as Apr 15 for an amount of USD 12,000 such that the Available Start Date is Apr 18. | On committing the backdated activity, the system raises the override: “Available balance 8000 is less than the notice amount 10000 as of withdrawal date 20220419”. |  |
| When the backdated notice capture for Apr 15 is triggered, the AVL is created considering the deposit balance as on Apr 18 which is USD 20,000. On Apr 18, the available balance in the deposit is USD 20,000 – USD 12,000 = USD 8000. | CUR - USD 20,000 AVL - USD 12,000 |  |
| During the replay of the Notice Capture activity on Apr 16, the system considers the deposit balance as on Apr 19 ( Available Start Date ) which is USD 8000 and raises the above-mentioned override for insufficient balance. The AVL balance is created for an amount of USD 20,000 and the bill details for the Apr 19 notice bill is also updated accordingly as 8000. | CUR - USD 20,000 AVL - USD 20,000 |  |

When the customer withdraws funds from the Notice Deposit without issuing a notice, the bank can charge the customer a penalty charge. A calculation routine available as part of core release can be used to calculate the penalty charge. However, if any modification is required for a specific bank, it can be done during implementation.

The customer requests a notice for withdrawal for an amount of USD 2000.

However, on the Available Start Date , the customer withdraws USD 3000. Therefore, the bank charges the customer a penalty fee for the USD 1000 which is withdrawn without notice.

The penalty fee is calculated based on the logic mentioned for USD 1000 withdrawn without notice.

Penalty charge = (5%*7*1000)/366= USD 0.95628.

In the above case, the Charge Percentage is 5%, Notice Period is 7 days and Interest Day Basis of the first Interest property is D = 360/366

The screenshot below shows the balances before and after the withdrawal of USD 3000.

The charge details show that the penalty charge is calculated on the Source Balance of USD 1000 which is the amount withdrawn without notice.

Consider the example where there is a captured notice for an amount of USD 1000 with payment date as April 17.

The captured notice can be modified by triggering the DEPOSITS-CHANGE-NOTICE.WITHDRAWAL activity from the Arrangement Overview page.

The customer requests to modify the withdrawal amount in the notice to USD 2000 such that the funds are available for withdrawal from April 19, onwards.

When the activity is authorised, the notice withdrawal bill is modified based on the details entered by the customer and can be viewed in the Notice enquiry on the Arrangement Overview page.

> **⚠️ Note:** If automatic settlement instructions are defined for the external beneficiary, then the user is restricted from modifying the notice request after the ISSUE.ORDER activity is processed for the payment file generation.

The user can accept or restrict an increase in the notice amount within the Notice Period by configuring the NOTICE.AMOUNT.INCREASE periodic attribute in the Activity Restriction condition.

As an example, consider that the activity restriction for a notice deposit is defined to restrict the increase in notice amount within the Notice Period .

A notice deposit is opened on April 19, 2022 and a notice is captured for withdrawal of an amount of USD 50,000.

When the user tries to modify the notice request such that there is an increase in notice amount to USD 55,000 from the previously requested amount of USD 50,000, the system raises an error to restrict the user from committing the activity.

| Column 1 | Column 2 |
|---|---|
| Dr AVL | Cr AVL BL |

The periodic rule evaluation can be configured to evaluate and check the rule for a defined Start and End period. As an example, the customer can be restricted from partially withdrawing from the notice deposit account within the cooling period.

In the example below, the Activity Restriction property condition is set to trigger the FULL.PAYOUT.DEP periodic attribute, whenever the deposit is partially withdrawn and raise an error if the evaluation returns YES.

The FULL.PAYOUT.DEP periodic attribute is defined with the Rule Start and Rule End as the rule evaluation period to check if the deposit is partially withdrawn by comparing the withdrawal amount with the current account balance of the deposit.

Consider the given notice deposit which is opened on 15th April 2021 with current deposit account balance as USD 10,000.

The Cooling Period field in the Term Amount condition is set to seven days. When the customer tries to withdraw the notice deposit for an amount of USD 500 on April 19, 2021, the system raises an error to restrict the user from partially withdrawing the deposit.

When the user triggers a Change or Cancel Notice Activity using the New Activity Link in the Arrangement Overview page or from the AA.ARRANGEMENT.ACTIVITY application, the user can input Notice Reference and/or Bill ID to indicate the Notice Withdrawal bill that has to be modified or cancelled.

Consider the following sample notice withdrawal bill in the notice deposit.

The notice withdrawal bill is captured for an amount of USD 3000 with Available Start Date as Apr 16.

On Apr 19, the customer requests for cancellation of the withdrawal notice. The user triggers the Cancel Notice activity from the New Activity link in the Arrangement Overview page. It is evident that the Bill ID field and/or the Notice Reference field can be input by the user to indicate the notice withdrawal bill that is to be cancelled.

Once the activity is authorised, the bill is moved to Expired status.

> **⚠️ Note:** When the user attempts to reverse the Capture Notice activity of a modified and/or cancelled bill, the user reverses the latest change (change or cancel activity) manually and then reverses the original captured bill to complete the process. However, it is possible to manually reverse the Change Notice activity without manually reversing the Cancel Notice activity.


##### Minimum Balance in Notice Deposit

A notice deposit can be defined to have a minimum balance requirement by configuring the Activity Restriction condition.

Consider a notice deposit is opened on April 1, 2021. The deposit balance is currently USD 20,000.

When the customer requests to withdraw an amount of USD 15,000, the system raises an override to warn the user that the minimum balance criteria is not maintained. If the user continues with the withdrawal, the Redeem transaction is followed by a payoff using the DEPOSITS-REDEEM-ARRANGEMENT activity and the closure.

If auto-settlement instructions are configured, then the system automatically pays out the deposit balances (in this case, USD 5000) and closes the deposit based on the closure condition.


##### Capturing a Closure Notice in Deposit Accounts

The following illustrations explain when the customer fully redeems a deposit account with and without a notice request.

The user can trigger the Notice Capture activity from the Arrangement Overview page and use the Closure Notice option in the Notice Type field to fully redeem a term deposit. A closure notice is generated for this and the rules regarding the Closure Notice are:

- The Notice Amount field is left blank. The system calculates the closure amount at the time of closure.
- Accounting entries are not raised. (that is, similar to an info-bill)
- At any given point of time, only one closure notice bill can exist in an arrangement.
- The system generates a warning message preventing the user from issuing regular notices when the Closure Notice is already scheduled in the system.
- The rest of the process remains the same as a regular withdrawal notice bill.

> **⚠️ Note:** For a Closure Notice, Notice Period is derived based on the first multi-value definition in the Balance Availability condition. In case of auto-closure of notice deposits, the Deposit Redeem activity is scheduled for the Available Start Date . If there is a change in the notice (only the Available Start Date can be modified) after the activity is scheduled, then the Redeem activity is re-scheduled as per the requested change.

Consider the notice deposit, in which the customer requests for a closure notice on April 15. The Notice Type field is set to Closure Notice and notice is requested for a deposit redemption on April 29.

A closure notice bill is created with Bill Type as CLOSURE.NOTICE which is an info-type of bill.

> **⚠️ Note:** The closure notice bill continues to be in ISSUED status even after the customer has redeemed the deposit fully (as it is an info type of bill).

When the customer tries to fully redeem a notice deposit without notice, a penalty charge can be configured and collected. The penalty charge for closure is calculated using the calculation routine available as part of the core release. The charge calculation routine uses the following formula to calculate the penalty charge:

Penalty Charge = (Charge percentage * Notice period days * Activity Transaction amount) / Interest Day basis.

Consider the example where customer tries to redeem a term deposit that has an account balance of USD 10,000 without issuing a closure notice.

A penalty charge for closure is levied on the customer based on the below calculation:

Penalty charge for closure = (5%*7*10,000)/366 = USD 9.5628

In this case, the Charge percentage is 5%, Notice Period is 7 days and Interest Day Basis of the first Interest property is ‘D’ = 360/366.


##### Auto Settlement of Funds for Notice Deposits

The withdrawal funds requested with notice can be automatically settled on the Available Start Date to either a settlement account, maintained within the system or to an external beneficiary through a PO based on the Settlement Instructions configured in the arrangement or the product.

The TBC can settle the requested notice amount with another account within the TBC or publish an event for a settlement request to an account or beneficiary outside the TBC, which should be consumed by an external payments system for further processing on the fund availability date.

| Column 1 | Column 2 |
|---|---|
| Cr AVL | Dr AVL BL |
| Dr AVL | Cr Customer Account |
| Dr CUR | Cr AVL BL |

| Column 1 | Column 2 |
|---|---|
| Dr SUSPPAYMENT | Cr AASUSPENSE |


##### Autoclosure of Deposits

It is possible to mandate that closure notice should exist to initiate deposit closure by defining Activity Restriction as mentioned in the configuration .

Consider a notice deposit with Activity Restriction configured to restrict deposit closure without a closure notice.

When the user tries to fully redeem the deposit, the system raises an error to warn the user that closure notice is mandatory to close the deposit.

A similar error is raised when the user simulates the deposit redemption without a closure notice.


#### 📋 Tasks

Related topics:

- Record Notice for Withdrawal (AA)
- Amend or Cancel Notice for Withdrawal (AA)
- Record Notice for Closure (AA)

Notice for Redemption of Funds feature allows the user to set up a notice for Notice Deposits Arrangement. The user must enter the amount and available start date to set up a notice. The expiry date is auto-calculated by the system based on the notice availability specified in the product. Once the notice is created, if the user tries to withdraw money before the available date, an override is generated, and a penalty fee is calculated on the withdrawn amount. Similarly, an override is displayed and a penalty fee is calculated for the amount withdrawn without notice.


##### Workflow

This section allows the user to perform the below activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Search Customer . |
| Find Customer | Enter a value in the Customer ID field and then click the Find button. |
| Customer Details | Click the Single Customer View icon corresponding to the record. Click the Products tab and then click the Deposits tab. Select the Deposit Overview option from the drop-down corresponding to a record and then click the Launch icon. |
| Arrangement Activity | Find the Create a New Notice option, under the Account Details section. Click the Create a New Notice/Change/Cancel icon and validate the activity record. Enter values for the following fields, in the Notice Withdrawal section: Notice Amount Avail Start Date Notice Type (Withdrawal Notice or Closure Notice) The Avail Expiry Date field value is defaulted based on the notice period configured in the product. The user can specify a forward value date, if necessary. Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

The user can view the below enquiries and reports related to Notice for Redemption of Funds.


##### Enquiries and Reports

This section allows the user to view the below enquiries and reports:

Account Details .

This enquiry displays details like notice amount, available from, and available till of the notice deposit arrangement.

In the Product Lines Deposits, a new enquiry is introduced for notice deposit to display the notice information in the overview screen. If data is not available for notice withdrawal, then the system displays 'No data'.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA


> **Related Applications:** `AA.ACTION`, `AA.ARRANGEMENT.ACTIVITY`, `AA.BILL.DETAILS`, `AA.BILL.TYPE`, `AA.PAYMENT.TYPE`, `AC.EVENTS`, `AC.LOCKED.EVENT`, `AC.LOCKED.EVENTS`, `CURRENCY`, `EB.LOOKUP`, `PAYMENT.ORDER`, `PAYMENT.ORDER.PRODUCT`, `PP.HEAVYWEIGHTPRODUCTCOND`

---


### 1.28  Preclosure of Deposits


> **📇 Quick Reference Card**
> 
> **Purpose:** *A partial withdrawal or a full redemption (closure) of a deposit contract is allowed as per the customer’s request. The user can run a simulation process, which produces a withdrawal or a redemption statement according to the customer’s request. This statement provides a detailed break-up of the dep...*
> 
> **Applications:** `AC.LOCKED.EVENTS`, `BENEFICIARY`, `PAYMENT.ORDER.PRODUCT`
> 
> **Key Fields:** *Active Y/N*, *Currency*, *Customer ID*, *Reserve Funds*, *Settlement A/c*, *Withdrawal Amount*, *Withdrawal Date*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

A partial withdrawal or a full redemption (closure) of a deposit contract is allowed as per the customer’s request. The user can run a simulation process, which produces a withdrawal or a redemption statement according to the customer’s request. This statement provides a detailed break-up of the deposit’s current balance, the withdrawal amount, any withdrawal or redemption charges and, in the case of a partial withdrawal, an interest loss comparison is given.

If the quotation is accepted, then, for a partial withdrawal or a full redemption, the process is the same and, at the end of the flow, the user can either make external payments, through a single or multiple payment orders, or make a credit to an account maintained within the system.

In the TBC, when the user redeems the deposit either partially or fully, the deposit proceeds can be settled to an account within the TBC. If the account or beneficiary is outside the TBC, the system forwards a settlement request to the account or beneficiary, by publishing an event which should be consumed by an external payments system for further processing. Hence, the payment order related details are not applicable for deposits in TBC.

Also, the simulations of deposits in the TBC are performed through the usage of the APIs provided.


#### ⚙️ Configuration

The simulation services need to be running to enable the process to complete. Read Configuring Deposit Simulations user guide for more information.

The simulation of deposits in TBC are performed through the usage of the APIs provided.


##### Generating a Payment Order Record

In either a full redemption or partial withdrawal flow, to generate a payment order, the user has to configure a PAYMENT.ORDER.PRODUCT as shown in the following screenshot and attach it in the relevant Settlement arrangement condition.


##### Defining a Beneficiary

To interface with the payment system, a suitable BENEFICIARY record is required. It holds the details of the receiver of the funds and ultimate beneficiary.

In the TBC, when the user redeems the deposit either partially or fully, the deposit proceeds can be settled to an account within the TBC. If the account or beneficiary is outside the TBC, the system forwards a settlement request to the account or beneficiary, by publishing an event which should be consumed by an external payments system for further processing.

Hence, the payment order related details are not applicable for deposits in the TBC.


##### CreatingAC.LOCKED.EVENTSRecords Automatically

Based on the configuration in the PAYMENT.ORDER.PRODUCT , the Reserve Funds field can be set as Yes. Contracts that make payments through a Payments Order can reserve the funds automatically and create a record in AC.LOCKED.EVENTS as shown below.


#### 🔧 Working With

This section helps the user to understand how to perform early withdrawals or full redemption (closure) of a deposit.


##### Redemption of Deposit Simulation

From the contract overview screen by clicking on the Redeem Deposit icon, the user can initiate an early redemption of the deposit. The simulation process produces a redemption statement as a quotation to the customer.

If the quotation is accepted, then a full redemption process is initiated. The process initiates the DEPOSITS-REDEEM-ARRANGEMENT Activity for full redemption.

The default settlement values are taken from the contract. As per the customers’ instructions these can be validated or changed by either defining an account, maintained within the system, or through a suitable configuration, generating a single or multiple payment orders. Once these are updated and the activity is committed, the process is completed.

The features related to the Arrangement Overview screen are not applicable in the Deposits TBC and the respective activities can be performed through the provided APIs.

In the TBC, when the user redeems the deposit, the deposit proceeds can be settled to an account within the TBC. If the account or beneficiary is outside the TBC, the system forwards a settlement request to the account or beneficiary, by publishing an event, which should be consumed by an external payments system for further processing.

To initiate and perform early redemption of a deposit contract,

1. Navigate to the deposit overview screen.
2. Select the Redeem Deposit icon. The system triggers simulation of redemption of deposit on the selected date.

The Redemption Statement is available in the Overview screen of the deposit arrangement.

The system runs multiple simulations with different dates and allows the customer to check the beneficial date to redeem the deposit. The system produces a separate Redemption Statement for each simulation run. The Redemption Statement displays the breakdown of:

- Deposit principal balance
- Accrued interest
- Tax on interest
- Charges that may be applicable for pre-closure of deposit account

The features related to the Arrangement Overview screen are not applicable in the Deposits TBC and the respective activities can be performed through the provided APIs.

If the customer accepts the quotation available in the Redemption Statement, then the user can process the customer’s request to redeem the deposit by triggering DEPOSITS-REDEEM-ARRANGEMENT Activity. The user can override and waive the charges using the Charge Override Property (if available in the product).

The deposit arrangement moves to pre-closure, once the transaction is authorised.

The system proceeds with the settlement of the deposit, either through the defaulted settlement condition available in the deposit arrangement, that is, the payout account defined, or based on the customer’s request to pay the proceeds by some other channel. Once this process is authorised, the redemption process is completed.

The example below is to illustrate the early redemption process of a deposit arrangement using simulation.

Consider a deposit is created on Jan 3, for a commitment of USD 100,000 USD with the term of one year. For an early closure, the redemption process is simulated for the date Apr 19.

After the execution of the simulation, the interest payable to the customer is calculated as USD 919.67 and the early redemption fee of 100 USD with the principal of USD 100,000 is settled based on the settlement condition.

The net payable amount to the customer is 100,819.67 USD which is calculated as follows,

Net Payable Amount = Deposit (USD 100,000) + Credit Interest Payable (USD 919.67) – Redemption fee (USD 100)

The deposit is closed as per the setup in the closure condition.

> **⚠️ Note:** When an interest payment is scheduled for a particular date but there are no settlement instructions provided, then the system parks the interest payable in the PAY balances of the deposit and this can be seen in the ECB Of deposit. In such cases, when the redemption is executed, the deposit proceeds during redemption includes the interest parked in the PAY along with other component balances. For example, consider Deposit amount - USD 10000, PAYDEPOSITINT - 500, ACCDEPOSITINT - 100, Redemption fee - 40 When the redemption is executed, the system pays out USD 10,560 (10,060 + 500 → 10,560) to the settlement account including the interest parked in PAYDEPOSITINT.

In the TBC, when the user redeems the deposit, the deposit proceeds can be settled to an account within the TBC. If the account or beneficiary is outside the TBC, the system forwards a settlement request to the account or beneficiary, by publishing an event, which should be consumed by an external payments system for further processing.


##### Partial Withdrawal Simulation

Before the natural maturity of the deposit, the user can initiate a simulated partial withdrawal (Funds are taken only from the current balance CURACCOUNT) of the deposit from the contract Overview Screen. This simulation process produces a partial withdrawal statement as a quotation to the customer. Similar to a full redemption, by selecting the Withdraw Deposit icon, the partial withdrawal flow of deposit is initiated from the Arrangement Overview screen.

The default settlement values are taken from the contract. As per the customers’ instructions these can be validated or changed by either defining an account, maintained within the system, or through a suitable configuration generating a single or multiple payment orders.

Mandatory validation is performed, in case the settlement details are not complete with either an account, maintained within the system, or beneficiary details. Once these instructions are updated and the activity is committed, the process is completed.

The features related to the Arrangement Overview screen are not applicable in the Deposits TBC and the respective activities can be performed through the provided APIs.

In the TBC, when the user withdraws the deposit partially, the deposit proceeds can be settled to an account within the TBC. If the account or beneficiary is outside the TBC, the system forwards a settlement request to the account or beneficiary, by publishing an event, which should be consumed by an external payments system for further processing.

On completion of the simulation, the system generates a Withdrawal Statement which is then made available in the Overview screen. The system can trigger multiple simulation runs with different dates. A separate Withdrawal Statement is generated for each individual simulation run.

The Withdrawal Statement contains and displays the following,

- Breakdown of deposit principal balance
- Withdrawal amount
- Any charges that may be applicable for this partial withdrawal. It also contains the interest comparison data that displays the Original interest amount at maturity based on the full principal amount. Newly projected interest amount after partial withdrawal.

Consider the below example, where a deposit is created on Apr 1, 2024 for 100,000 USD. As on 16th, the accrued interest amount is 15.43. The user triggers a withdrawal deposit option from the COS overview page and specifies the withdrawal amount of 40,000 on May 16,2024. The simulation is completed successfully.

The features related to the Arrangement Overview screen are not applicable in the Deposits TBC and the respective activities can be performed through the provided APIs.

If the customer accepts the quotation, then the partial withdrawal request is processed further, by triggering the DEPOSITS-WITHDRAW-PAYOUT.RULES Activity (related DEPOSITS-APPLYPAYMENT-PO.EARLY.WITHDRAWAL Activity Class).

The system proceeds with the settlement of the partial withdrawal, either through the settlement condition available in the deposit arrangement, that is, a payout account defined, or based on the customer’s request to pay the proceeds by some other channel. Once this process is authorised, the partial redemption process is completed.

The below screenshot displays the Deposit Overview screen that displays the Withdraw Deposit option.

The below screenshot displays the Withdrawal Statement with the current balance, withdrawal date and amount, and the interest comparison data (Interest amount (24.89 USD) applicable for the deposit due to the withdrawal of 40,000 USD) after simulation was run successfully.

The features related to the Arrangement Overview screen are not applicable in the Deposits TBC and the respective activities can be performed through the provided APIs.

When the Withdraw Deposit option is triggered from the COS overview page, the settlement instructions can be updated at this stage. In this case, the beneficiary is defined in the settlement instruction along with the payment order product.

If no settlement instructions are defined, then the system produces a validation forcing the user to enter some mandatory instructions. When the transaction is committed, the payment order is generated for 40000 on May 16, 2024.

This is illustrated in the below screenshots. After a partial redemption of 40,000 USD, the principal amount is updated as 60,000 USD in the COS overview page.

Consider an example, where the request is to pay 80 percent to Beneficiary A and 20 percent to Beneficiary B.

In this case, two beneficiary records are defined in the settlement instructions.

- For beneficiary A, payout percentage is defined as 80.
- For beneficiary B, payout percentage is defined as 20.

When the transaction is authorised, two payment orders are generated on May 16,2024.

- 80 percent to Beneficiary A - 32000 USD (80% of 40000)
- 20 percent to Beneficiary B - 8000 USD (20% of 40000)

This is illustrated in the below screenshots. After a partial redemption of 40,000 USD, the principal amount is updated as 60,000 USD in the COS overview page.

In the TBC, when the user withdraws the deposit partially, the deposit proceeds can be settled to an account within the TBC. If the account or beneficiary is outside the TBC, the system forwards a settlement request to the account or beneficiary, by publishing an event, which should be consumed by an external payments system for further processing.

Hence, the payment order related details are not applicable for deposits in the TBC.


#### 📋 Tasks

Related topics:

- Perform Partial Withdrawal of Deposit (AA)
- Perform Pre-Closure of Deposit (AA)

In partial withdrawal, the customer is bound to lose a part of the assured interest returns, which the customer may want to know before proceeding to do the transaction. Simulation process assists the customer to understand the impact of interest loss on such partial withdrawal.


##### Workflow

This section allows the user to view the below list of tasks:

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Find Deposit Arrangements | Enter the required field values and click the FIND button. |
| AA Arrangement | Click the Overview icon. |
| Arrangement Overview (Deposits) | Click the Run option corresponding to Withdraw Deposit activity. |
| Withdrawal Simulation | Enter values in the following fields: Withdrawal Date Withdrawal Amount Currency Click the Validate icon to check for errors and overrides. Click the Settlement Instruction section to expand. In the Initial Funding, Charges Settlement screen, enter values in the following fields: Active Y/N Settlement A/c In the Interest & Redemption Settlement screen, enter values in the following fields: Active Y/N Settlement A/c Click the Validate icon to check for errors and overrides. Click the Commit icon. Run the BNK/AA.SIMULATION.SERVICE simulation service . |
| Arrangement Overview (Deposits) | Click the Withdrawal Statement icon. |
| Withdrawal Statement | Click the Withdrawal Statement Details icon . Click the Withdrawal Deposit icon. Enter values in the following fields: Withdrawal Date Withdrawal Amount Currency Click the Validate icon to check for errors and overrides. Click the Settlement Instruction section to expand. In the Initial Funding, Charges Settlement screen, enter values in the following fields: Active Y/N Settlement A/c In the Interest & Redemption Settlement screen, enter values in the following fields: Active Y/N Settlement A/c Click the Validate icon to check for errors and overrides. Click the Commit icon. Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
|  | Search Customer . |
| Find Customer | Enter the customer ID in the Customer ID field and then click the FIND button. Click the Single Customer View icon. |
| Customer Details | Click the Deposits tab. Select the Partial Redemption(PO) option from the drop-down list and then click the Select icon. |
| AA Partial Withdrawel | Enter values in the following fields: Debit Account Number Credit Account Payment Amount Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Search Customer . |
| Find Customer | Enter the customer ID in the Customer ID field and then click the FIND button. Click the Single Customer View icon. |
| Customer Details | Click the Deposits tab. Select the Preclose Deposit(PO) option from the drop-down list and then click the Select icon. |
| AA Partial Withdrawel | Enter values in the following fields: Debit Account Number Credit Account Payment Amount Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

There are no Outputs available for Pre-Closure of Deposits - Partial and Full feature.


> **Related Applications:** `AC.LOCKED.EVENTS`, `BENEFICIARY`, `PAYMENT.ORDER.PRODUCT`

---


### 1.29  ProductVariations


> **📇 Quick Reference Card**
> 
> **Purpose:** *Deposit products vary in characteristics based on the duration of the deposit. Much of the product configuration remains the same while a small set of conditions differ based on the arrangement term. For instance, interest can be higher or lower depending upon the market conditions on the shorter te...*
> 
> **Applications:** `AA.ARR.<PC>`, `AA.ARR.<PROPERTY.CLASS>`, `AA.ARR.<PROPERTYCLASS>`, `AA.ARRANGEMENT.ACTIVITY`
> 
> **Key Fields:** *Change Period*, *Condition by Term*, *Default Attr Option*, *Rollover*, *Term*, *Term Type*, *Term Variation*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Deposit products vary in characteristics based on the duration of the deposit. Much of the product configuration remains the same while a small set of conditions differ based on the arrangement term. For instance, interest can be higher or lower depending upon the market conditions on the shorter term. The settlement of interest can be set to renewal or maturity for shorter terms while it can be paid on periodical basis for longer deposit contracts. To achieve this, the user can create one master product with varying interest or Payment Schedule conditions that are dynamically picked up based on the arrangement term. This helps the banks in maintaining a small set of specific products in the catalog.

> **⚠️ Note:** This functionality is available only when products are created using Temenos Product Manager (TPM).


#### ⚙️ Configuration

Temenos Product Manager (TPM) allows the users to create products that vary by term. The following sections provide an overview of how it can be defined.


##### Definition of Allowed Terms in TPM

The user can define the term options required for the deposit products. During product creation, the user can choose one or more term options that are defined. Ad hoc term options cannot be defined during product creation.

Term options must be defined using standard period options (Days, Weeks, Months, Years).


##### Product Creation in TPM

The product designer in TPM is used to create or edit the products. While defining the product,

- The user can select the Conditions by Term option only when Term Type is set as selectable.
- Once Conditions by Term option is selected, the user can select different term options that are applicable for the product.
- After the term options are selected, the system creates a tab for the default and additional tabs for the terms chosen.
- The user can define the conditions that are applicable for the respective term.

During product creation through Conditions by Term, the product is enabled and different term options are specified as per bank’s requirement.

For example, in the below scenario, 90 Days and 1 Year are selected. In that case, there are three different conditions based on the term.

- A default condition, that applies for the arrangements from the minimum term, upto 89 days.
- A 90 Days + condition, that applies for arrangements from 90 days to less than a year.
- A 1 year + condition, that applies for arrangements greater than a year.

When the user approves a product in TPM, the system sends the product details to the core system (Transact) for creating actual product records. The system updates different terms passed by TPM in the Term Variation attribute in the product designer and catalog records respectively. The product designer allows the term to be updated in the Term Variation attribute only when the term is passed by TPM.

Once the product is created, AA.PRD.CAT records for different terms are created with respective conditions for the property classes and Condition by Term attribute is updated as Yes in the product catalog record for the respective product.

In case, Condition by Product is enabled and the user configures conditions for a different term, then same number of AA.PRD.CAT. records are created for the property class.

The following three AA.PRD.CAT. records are created as per the selected term shown above.

- Default condition record (TERMDEPOSITS-USD-20110411)
- 90D condition record (TERMDEPOSITS_90D-USD-20110411)
- 1Y condition record (TERMDEPOSITS_1Y-USD-20110411)

Rollover flag in the Term Amount condition can be used to indicate if the arrangements under this product are set to be rolled over or moved to a different product.


##### Arrangement Creation

Term ). This can also be initiated using the API for creating new arrangement.

Deposits can be configured to be rolled over or matured. When the term is passed while creating new arrangements, the term can be updated in different property class attributes based on the rollover conditions.

- For a rollover contract - Term to be updated in Change Period field in Change Product condition.
- For non-rollover contract - Term to be updated in Term field in Term Amount condition.

To update the term in Change Product or Term Amount condition, the system refers the Rollover flag in the Term Amount condition.

- If the user selects the Rollover flag in the Term Amount condition, then the system defaults the term specified in AAA to the Change Period attribute in the Change Product condition. Else, the system defaults the term specified in AAA to the Term attribute in the Term Amount condition.

> **⚠️ Note:** If the Rollover attribute needs to be set, the Change Product property class should be mandatorily defined in the product. To default the Term in Term Amount or Change Product condition during new arrangement creation, the respective property class should not be kept as product-only condition. Term in Term Amount and Change Period in Change Product should not set as Non-Negotiable.


#### 🔧 Working With

This topic explains the working of product variation based on arrangement term.


##### Product by Term Variation - Catalog Updates

In deposits, arrangements are created using DEPOSITS-NEW-ARRANGEMENT activity. When a term is specified in AA.ARRANGEMENT.ACTIVITY (AAA) for a condition-based product, the system:

- Refers to the term to pick the correct condition for the respective property class.
- Defaults the term in the Term attribute in Term Amount or Change Period attribute in the Change Product condition based on the Rollover flag in the Term Amount condition.

Consider a product is enabled with the Condition by Term option and different conditions are configured based on term variations in TPM. Once the product is approved, AA.PRD.CAT records are created in Transact for the respective property classes as shown below.

For the below property classes, term variation is enabled and the respective conditions are shared below.

| Column 1 | Column 2 |
|---|---|
| Payment Schedule |  |
| Default condition | Interest is configured to be paid at the time of renewal for arrangement term upto 1 year |
| 1Y condition | Interest is configured to be paid annually for arrangement term more than a year |
| Cooling Period |  |
| Default condition | Cooling Period is defined as 1 working day for arrangement term upto 31 days |
| 1M condition | Cooling Period is defined as 10 calendar days for arrangement term more than 31 days |
| Activity Restriction |  |
| Default condition | Minimum deposit balance required is 2500 for arrangements with term upto 89 days |
| 90D condition | Minimum deposit balance required is 500 for arrangement with term more than 89 days |
| Activity Messaging |  |
| Default condition | Prenotice is not configured for reset and mature activities for arrangements with term upto 12 days |
| 13D condition | Prenotice of 13D is configured for reset and mature activities for arrangements with term 13 Days to 31 Days |
| 32D condition | Prenotice of 30D is configured for reset and mature activities for arrangements with term more than 31 days |

When creating an arrangement , the user specifies the term as 20D in AAA and selects the Rollover flag in the Term Amount condition.

Depending upon the term defined in AAA, the system considers the appropriate conditions based on the term defined in AAA.

- In this case, Term is specified as 20D in AAA, the system picks the Default condition for Payment Schedule Default condition for Closure Default condition for Activity Restriction 13D condition for Activity Messaging
- Once the arrangement is created, the system creates AA.ARR. records by loading the correct conditions from AA.PRD.CAT. records.
- Term specified in AAA is defaulted to the Change Period attribute in the Change Product condition.

When creating an arrangement, the user specifies the Term as 2Y in AAA and does not select the Rollover flag in the Term Amount condition.

Depending upon the term defined in AAA, the system considers loading the correct conditions based on the term defined in AAA.

- In this case, Term is specified as 2Y in AAA, the system picks the 1Y condition for Payment Schedule 1M condition for Closure 90D condition for Activity Restriction 32D condition for Activity Messaging
- Once the arrangement is created, the system creates AA.ARR. records by loading the correct conditions from AA.PRD.CAT. records.
- Term specified in AAA is defaulted to the Term attribute in the Term Amount product condition.

AA.ARR. table screenshots are shown below.


##### Change Product or Reset or Rollover

Deposits can be configured to be reset or rolled over or changed to a different product using the Change Product condition.

During a CHANGE.PRODUCT activity, a new product may be configured with a different set of conditions for the same term and the system refers the new product conditions based on the term passed in AAA, accordingly conditions are updated for property classes for which the Default Attr Option is set as resetting.

In case of a ROLLOVER activity, the system rolls over the deposit and the conditions considered during new arrangement activity are retained. If the conditions must be reset after every renewal term, then banks must configure RESET activity in the change product condition.

During the RESET activity, the system refers the latest conditions based on the term in AAA and accordingly conditions are updated for property classes for which the Default Attr Option is set as resetting.


##### Change in Term

The user can specify or change the deposit term using the Term attribute in AAA by using any of the below activities.

- DEPOSITS-CHANGE.PRODUCT-ARRANGEMENT
- DEPOSITS-RESET-ARRANGEMENT
- DEPOSITS-NEW-ARRANGEMENT
- DEPOSITS-TAKEOVER-ARRANGEMENT
- DEPOSITS-CHANGE.TERM-TERM.AMOUNT
- DEPOSITS-UPDATE-CHANGE.PRODUCT

If Term in AAA is updated by DEPOSITS-CHANGE.TERM-TERM.AMOUNT or DEPOSITS-UPDATE-CHANGE.PRODUCT activity, the system triggers a secondary activity namely DEPOSITS-CHANGE.TERM.VARIATION-ARRANGEMENT which in turn updates product conditions based on the revised term specified in AAA and AA.ARR. tables are updated accordingly.

> **⚠️ Note:** When the term is updated in AAA, the system fetches and updates the conditions in AA.ARR. table based on revised term for the property classes for Default Attr Option is configured as resetting.


#### 📋 Tasks

There are no Tasks available for Product Variation based on Arrangement Term feature.


#### 📊 Outputs

There are no Outputs available for Product Variation based on Arrangement Term feature.


> **Related Applications:** `AA.ARR.<PC>`, `AA.ARR.<PROPERTY.CLASS>`, `AA.ARR.<PROPERTYCLASS>`, `AA.ARRANGEMENT.ACTIVITY`

---


### 1.30  Risk Free Rates


> **📇 Quick Reference Card**
> 
> **Purpose:** *Risk Free Rates in the system support any RFR irrespective of currency and publication time. They are not equal to IBOR and have to be processed in a different way. RFRs are published with a lag, that is, the rate that is published today is applied for a date in the past. This means that transaction...*
> 
> **Applications:** `EB.CASHFLOW`, `PERIODIC.INTEREST`
> 
> **Key Fields:** *Apr Type*, *Arrangement*, *Bus Day Centre*, *Lookback Type*, *Period End Date*, *Periodic Index*, *RFR*, *RFR Flooring* ... +5 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Risk Free Rates in the system support any RFR irrespective of currency and publication time. They are not equal to IBOR and have to be processed in a different way. RFRs are published with a lag, that is, the rate that is published today is applied for a date in the past. This means that transactions, which use RFRs must reference new rates each business day for compounding Interests. Banks can choose from multiple ways of compounding interest.

The features related to Risk Free Rates are not applicable for deposits in TBC. Read here to know more about TBC for deposits.


#### ⚙️ Configuration

The RFRs stored in the PERIODIC.INTEREST application are only published rates and are compounded on a daily basis to arrive at a final interest rate for the period.

- The user enters the RFRs index in the Periodic Index field.
- Along with periodic index, market convention and spread treatment parameters are passed to call the rate calculation routine to arrive at the daily compounding interest rate for the contract.
- The calculation method defined in the Rfr Calc Method attribute is used to calculate the total accrual amount for the current interest period.
- The market convention ( Rfr Convention attribute) that AA follows is the use of historical RFRs for daily compounding and is called as Lookback.

Whenever a spread is input in a contract which is on top of the rate, there are spread treatment options that can be defined in the Rfr Spread Treatment attribute.

If the rate applies till a date in excess of the Period End Date that is, when the interest period end is a weekend and contains a real month end date, then the business day’s ( Bus Day Centre attribute) convention from the Account Property conditions takes precedence in calculating the day count.

> **⚠️ Note:** In the tier interest configurations, multiple periodic indexes are allowed, but for RFR processing, the system permits only the same index record.


##### Flooring

As per market standards, the system supports the flooring of rates at either positive or negative (not just a zero rate). The following table shows how the daily and average zero floor is applied to the rate.

Similarly, positive and negative flooring can be applied to the rate. Read Interest Property Class for more information.

Read

to understand the steps involved for

using NCCR.

- When the RFR Spread Treatment field is set as: Spread-Inclusive - The spread is included as part of the cumulative compounded rate calculations (ACR -Step 1) Spread-Exclusive – The spread is added at the end of the NCCR calculations (after Step 3)
- The RFR Spread Treatment and RFR Flooring fields do not have any impact on the UCR or NCCR calculations and are applied as part of ACR calculations (Step 1).
- UCR and NCCR should not be rounded while ACR calculation follows the configured rounding rule.
- Precision should be 16dp or higher as recommended by the Bank of England.


##### IFRS Processing

IFRS has specific rules for the RFR cashflow update. They are:

- Initial transition from IBOR to RFR updates the EIR (Effective Interest Rate) in EB.CASHFLOW using the specific DEPOSITS-UPDATE.CASHFLOW-REPORTING activity.
- Ongoing daily changes in cashflow are updated in EB.CASHFLOW using the INTEREST-CHANGE event type during the RFR rate revision process.

> **⚠️ Note:** Apr Type in the Reporting Property Condition with Source Type as INTEREST is restricted for RFR contracts, as it is relevant only for deposits with fixed rate.


#### 🔧 Working With

The following section describes the working of RFR with an example.

Consider the following example of a Deposit with linked RFR. The interest payment is scheduled for weekly payments. The attribute values are set as follows:

- Term Amount - USD 1,000,000
- Lookback Days - 3
- Lookback Type - Observation Shift

The daily interest accrual amounts for the interest period are displayed in the following table. The last column in the table shows the total interest amount. In this case, 147.83 is receivable based on the final compounded rate of 0.7708%.

| Date | RFR Applicable(in percentage) | RFR Effective Date | Day Count to be considered | Compounded Rate(in percentage) | Accrual Based on the Compounded Rate | Sum of Accrued Interest |
|---|---|---|---|---|---|---|
| 7/3/2019 | 0.7701 | 6/28/2109 | 3 | 0.7701 | 21.10 | 21.10 |
| 7/4/2019 | 0.7812 | 7/1/2019 | 1 | 0.7729 | 21.25 | 42.35 |
| 7/5/2019 | 0.7619 | 7/2/2019 | 1 | 0.7707 | 21.08 | 63.43 |
| 7/6/2019 | N/A |  |  |  | 21.08 | 84.50 |
| 7/7/2019 | N/A |  |  |  | 21.08 | 105.58 |
| 7/8/2019 | 0.7733 | 7/3/2019 | 1 | 0.7711 | 21.19 | 126.76 |
| 7/9/2019 | 0.7688 | 7/4/2019 | 1 | 0.7708 | 21.07 | 147.83 |
| 7/10/2019 | 0.7988 | 7/5/2019 | 1 |  |  |  |


###### Spread-Inclusive Scenario

The RFR is compounded together with the spread. Consider the same example (as above) but with a spread of 0.05%, which is taken into the rate compounding process:

> **⚠️ Note:** For the spread operand, only ADD and SUBTRACT are supported for the RFR functionality.

The daily interest accruals are based on the compounded rate with the spread included in the compounding. The overall receivable amount is 157.42.

| Date | RFR Applicable (in percentage) | RFR Effective Date | Day Count to be considered | Compounded Rate with Spread ( in percentage) | Accrual Based on Compounded Rate with Spread | Sum of Accrued Interest |
|---|---|---|---|---|---|---|
| 7/3/2019 | 0.7701 | 6/28/2109 | 3 | 0.8201 | 22.47 | 22.47 |
| 7/4/2019 | 0.7812 | 7/1/2019 | 1 | 0.8229 | 22.62 | 45.09 |
| 7/5/2019 | 0.7619 | 7/2/2019 | 1 | 0.8207 | 22.45 | 67.54 |
| 7/6/2019 | N/A |  |  |  | 22.45 | 89.98 |
| 7/7/2019 | N/A |  |  |  | 22.45 | 112.43 |
| 7/8/2019 | 0.7733 | 7/3/2019 | 1 | 0.8212 | 22.56 | 134.98 |
| 7/9/2019 | 0.7688 | 7/4/2019 | 1 | 0.8208 | 22.44 | 157.42 |
| 7/10/2019 | 0.7988 | 7/5/2019 | 1 |  |  |  |


#### 📋 Tasks

Related topics:

- Amend Deposit (AA)

The Risk Free Rates are the published rates and are compounded on daily basis. It is identified or calculated based on RFR field value and used for accrual calculations.


##### Workflow

This section allows the user to perform the below tasks:

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Find Deposit Arrangements | Enter the deposit arrangement ID in the Arrangement field and then click the FIND button. Click the Overview icon corresponding to a record. |
| Arrangement Overview (Deposit) | Click the View Arrangement icon in Arrangement condition tab. |
| Arrangement Activity | Click the Deposit Interest section and then click the RFR tab to view the deposit arrangement and RISK-FREE rates. |


#### 📊 Outputs

There are no Outputs available for Risk Free Rates feature.


> **Related Applications:** `EB.CASHFLOW`, `PERIODIC.INTEREST`

---


### 1.31  Rollover of Deposits


> **📇 Quick Reference Card**
> 
> **Purpose:** *The banks define rollover of deposit arrangement, as per the user’s definition in the Payment Schedule Property Condition. The rollover can be manual or automatic. A rollover of deposit is allowed, after a specific period, from the date of creation of an arrangement.*
> 
> **Applications:** `AA.ARRANGEMENT.ACTIVITY`, `AA.SCHEDULED.ACTIVITY`
> 
> **Key Fields:** *Arrangement*, *Change
 Period*, *Change Activity*, *Change Date*, *Change Date Type*, *Change Period*, *Default Attr Option*, *GB Narrative* ... +3 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The banks define rollover of deposit arrangement, as per the user’s definition in the Payment Schedule Property Condition. The rollover can be manual or automatic. A rollover of deposit is allowed, after a specific period, from the date of creation of an arrangement.

The customer can avail a better deposit product, after the first contract period, to increase the principal amount or redeem the deposit, without incurring loss.

There are no specific differences related to rollover of deposits in the TBC.


#### ⚙️ Configuration

The user defines the conditions for rollover in the Change Product Property Class. The value in the Change Period field is the period after which the system triggers Deposit Rollover Activity.

On the rollover date, it is possible to rollover the entire amount of the outstanding principal balance. In addition, it is also possible to rollover only a part of the principal amount and pay the rest of the same to the customer.

While defining the condition for Change Product Property Class,

- The user can define the rules and behaviour for allowing the arrangements of one product that can be changed to another and support rollover and reset activities.
- The user can choose when a rollover can be performed on the arrangement. The Change Date Type field defines if period or a date will be configured, based on which, the user can specify a period or date in the Change Period or Change Date fields, respectively.
- The system triggers the DEPOSITS-ROLLOVER-ARRANGEMENT Activity for the rollover of the deposit.
- The system calculates the deposit rollover trigger date, based on the date available in the Change Period field.
- The system generates prior notification advice for Rollover Activity by setting the Pre Notice Days field in the Activity Messaging Property Condition.


##### Difference between Rollover, Reset, Change Product Activity

Banks can configure any of the below activities in the Change Activity attribute in the change product condition as per their requirements.

- DEPOSITS-ROLLOVER-ARRANGEMENT
- DEPOSITS-RESET-ARRANGEMENT
- DEPOSITS-CHANGE.PRODUCT-ARRANGEMENT

The system behavior after these activities are triggered is explained in the below table.

| Rollover | Reset | Change Product |
|---|---|---|
| The system triggers the DEPOSITS-ROLLOVER-ARRANGEMENT activity based on the Change Period definition in change product condition. During the rollover activity, the system retains the conditions picked up at the time of arrangement creation for the property classes (This behavior is applicable irrespective of the Default Attr Option configuration in the respective property class). | The system triggers the DEPOSITS-RESET-ARRANGEMENT activity based on the Change Period definition in change product condition. During the reset activity, the system updates the latest conditions for the property classes for which the Default Attr Option attribute is set as Resetting. However, the system retains the conditions picked up at the time of arrangement creation for the property classes for which Default Attr Option is set as Non Resetting If the banks prefer to offer latest interest rates of the product at the time of reset activity, they can configure Default Attr Option as Resetting in the Interest product condition. | The system triggers the DEPOSITS-CHANGE.PRODUCT-ARRANGEMENT activity based on the Change Period definition in change product condition. During the Change Product activity, the system updates the latest conditions from the new product for the property classes for which Default Attr Option attribute is set as Resetting However, the system retains the conditions picked up at the time of arrangement creation for the property classes for which Default Attr Option is set as Non Resetting. |


##### Interest Payment or Capitalisation during Rollover, Reset, Change Product Activity

Interest payment or capitalisation frequency is defined using the Payment Schedule condition.

Consider a deposit is created on Jan 1. The Term is specified as 3 months. In the Change Product condition, the Change Period is specified as 15 days and Change Activity is set as DEPOSITS-ROLLOVER-ARRANGEMENT. Interest is configured to be paid every month on 5th in the Payment Schedule condition.

Based on the above configuration, the interest is paid on the following dates.

- Jan 5 (Makedue)
- Feb 5 (Makedue)
- Mar 5 (Makedue)
- Apr 1 (Maturity)

Though the rollover activity is triggered every 15 days ( Jan 16, Jan 31, Feb 15, Mar 1 , Mar 16, Mar 31), the system does not pay out the interest payment during the rollover activity since the term is specified in the term amount condition.

> **⚠️ Note:** The system behaves the same for Rollover Activity, Reset Activity and Change Product as long as the payment schedule remains unchanged for the new product.

Consider a deposit is opened on Jan 1 . Change Period is specified as 15 days and Change Activity is set as DEPOSITS-RESET-ARRANGEMENT in the Change Product condition. Term is not set in the term amount condition. Interest is configured to be capitalised every month on 5th in the payment schedule condition.

Based on the above configuration, Interest is capitalised on the following dates.

- Jan 5 (Capitalise)
- Jan 16 (Reset)
- Jan 31 (Reset)
- Feb 5 (Capitalise)
- Feb 15 (Reset)
- Mar 1 (Reset)
- Mar 5 (Capitalise)
- Mar 16 (Reset)
- Mar 31 (Reset)
- Apr 5 (Capitalise) and the cycle continues until redemption.

Since the term is not specified in the Term Amount condition, the system capitalises the interest during reset activity and refers the Payment Schedule frequency as well.

> **⚠️ Note:** The system behaves the same for Rollover Activity, Reset Activity and Change Product as long as the payment schedule remains unchanged for the new product.

In the TBC, the pre-notifications are not applicable and, if required, they should be handled by external solutions.


#### 🔧 Working With

The below screenshot displays the rollover of an AA Deposit contract. When creating the arrangement, the user can pre-define the automatic rollover with a three-month frequency. The below screenshot displays the applicable dates for a new arrangement and post rollover. The system displays the rollover date when creating the arrangement and auto-populates the dates at the time of contract rollover.

When creating the arrangement, the system updates the AA.SCHEDULED.ACTIVITY table with applicable dates for the rollover of the contract.

The user can view the scheduled pre-notice and rollover activities in the AA.ARRANGEMENT.ACTIVITY table.

In the TBC, the pre-notifications are not applicable and, if required, they should be handled by external solutions.


##### Deposit Amount during Rollover

In this scenario, 3-month deposit is set to rollover on maturity.

To modify the principal amount to be rolled over, the user must define the Method field as Maintain in the Payment Schedule Product Condition.

In this example, the system scheduled the deposit rollover for an amount of 61,000.

The system scheduled an Issue-bill Activity for this deposit for the additional bill amount during rollover.


#### 📋 Tasks

Related topics:

- Amend Deposit (AA)

The user can trigger the DEPOSITS-ROLLOVER-ARRANGEMENT activity for renewal of the deposit.


##### Workflow

This section allows the user to perform the below activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Find Deposit Arrangements | Enter an account arrangement ID in the Arrangement field and then click the FIND button. Click the Overview icon corresponding to a record. |
| Arrangement Overview (Deposit) | Click the New Activity option. |
| New Activities | Click the Do Activity Today icon corresponding to Rollover Deposits activity. |
| Arrangement Activity | Enter a value in the GB Narrative field. Click the Validate icon. Click the Commitment tab and then enter a value in the Term field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

Banks define rollover of deposit arrangement as per the user’s definition in the Payment Schedule Property Condition. Rollover can be manual or automatic. Rollover of deposit is allowed after a specific period from the date of creation of an arrangement.


##### Enquiries and Reports

NA


##### SWIFT Messages

NA


##### Advices

The user can view the below list of Advices pertaining to Roll over of Deposit:

The user can view the details of deposit rollover advice.


##### Alerts

NA


> **Related Applications:** `AA.ARRANGEMENT.ACTIVITY`, `AA.SCHEDULED.ACTIVITY`

---


### 1.32  Savings Plan Product


> **📇 Quick Reference Card**
> 
> **Purpose:** *A Savings Plan Product is a special kind of deposit, offered by banks to inculcate savings in customer. The customer can deposit a fixed amount in each interval (say monthly). This amount is locked for the term of the deposit and interest is accrued on the available principal for that accrual period...*
> 
> **Applications:** `AA.OVERDUE.STATS`, `AA.PERIODIC.ATTRIBUTE`
> 
> **Key Fields:** *Amount*, *Arrangement*, *Bill Type*, *Cancel*, *Cancel Period*, *Cooling Period*, *Flat Charge*, *Holiday Amt* ... +3 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

A Savings Plan Product is a special kind of deposit, offered by banks to inculcate savings in customer. The customer can deposit a fixed amount in each interval (say monthly). This amount is locked for the term of the deposit and interest is accrued on the available principal for that accrual period.

The customer can be offered a grace period to pay the periodic amount to be deposited and timely deposits can be encouraged, by giving a bonus for on-time deposits.

There are no specific differences, related to savings plan products (deposits) in the TBC.


#### ⚙️ Configuration

The Retail Deposits module creates a deposit product that allows the customer to deposit a sum every month for a specific period. To facilitate principal payment, the system triggers a principal bill using the Bill Type that is set to Expected. If an amount is updated in the Term Amount condition, it is treated as the initial deposit in the contract.

The customer must settle (pay) the bill within a specified grace period. If the customer pays the full principal instalment within the grace period, then a bonus amount can be configured to be paid to the customer.

The Activity Restriction Product Condition is added to the product to evaluate if the customer has met the payment condition within the grace period. The TXN.COUNT.LIFE , a AA.PERIODIC.ATTRIBUTE record validates the total transaction count during the tenure of the deposit arrangement. This is explained in the below screenshot.

The periodic attribute is attached to the Activity Restriction Product Condition.

The DEPOSITS-AGE-OVERDUE*DEL*EXPECTED Activity moves the status from Expected bill (principal amount) to Delinquent (Overdue Status). Once the principal amount bill moves from Grace to Delinquent, the above Activity is triggered.

If the

field is updated to two, then the number of times the customer can miss to pay during the entire tenure of the deposit arrangement is also two. The customer is allowed only twice to fail making the payment, before the principal amount bill is moved to Delinquent status.

If there is no payment from customer within the grace period for the third time, that is if the evaluation for the third time is 'Break', then the evaluation method is updated as 'Waive'. This means that, if the customer fails to make payment within the grace period for the third time, then the bonus amount is not paid to the customer; the bonus charge amount is waived.

Read the Activity Restriction Property Class user guide for more information on the working functionality of the Property Class.


#### 🔧 Working With

The Savings Plan product enables the customer to commit in saving a specific amount of money, on a regular frequency, for a particular period.


##### Commitment Details of Savings Plan

The Term , which can be defaulted and negotiated at arrangement level, indicates term of the savings commitment. The permissible term can be indicated, under the Negotiation tab, to include the various values. Cooling Period and Cancel Period fields are applicable for the Savings plan products, as well.

If an amount is input in the Term Amount Condition, it is considered as the initial deposit. It may be left blank if no initial deposit is required. The periodic (for example, monthly) commitment amount, is specified under the Amount field in the Payment Schedule condition.


##### Expected Payments of Savings Plan

The Payment Schedule condition is used to define the Notional payment schedule for regular payments expected from the customer. For these notional due payments, the Bill Type field is set to EXPECTED.


##### Bonus Payment

At the end of the committed period, a bonus can be paid, if certain criteria such as, the number of missed deposits, is below the agreed number.

The bonus (a payable charge) is paid when,

- There are no late payments during the term of the savings plan.
- The number of missed payments is less than a predefined tolerance.
- The average delinquency amount for a status is less than x.
- The total days in a delinquency status is less than x.

The features of the bonus payment are:

- The bonus is generally payable to the customer on the maturity date of the Savings Plan.
- The rule to evaluate the bonus criteria is defined in the Activity Restriction Product Condition.
- During the bonus payment, the Activity Restriction is used with evaluation based on either the Activity or the Property.
- To determine if a bonus can be paid, an Aging Activity is specified in the Evaluation Activity and the comparison value is specified in periodic value.

The DEPOSITS-AGE-OVERDUE*OD1 Activity specifies where OD1 is evaluated to grant a bonus or not.


##### Evaluation with Periodic Attributes

- The Periodic Attribute Class used with the Activity Restriction, evaluates the following aspects to handle different Bonus Conditions. Number of days in overdue status Average amount in overdue Number of times the bills reached overdue status
- Routines attached in Periodic Attribute Class, rebuilds the AA.OVERDUE.STATS , every time, when the rule is evaluated apart, from actual rebuilding of the file, which is done by the Aging Activity.


#### 📋 Tasks

Related topics:

- Amend Deposit (AA)
- Account and Deposit Processes (Retail)

The Deposit Arrangement administration can be done by triggering various activities in a deposit arrangement through which various conditions can be updated as per the requirement. Some of the deposit arrangement administration related activities are update charges, update activity charges, update tax and so on.

System allows customers to request for a holiday payment on their savings plan product and the user can modify or cancel the requested holiday payment.


##### Workflow

In Savings Plan Product, the user can perform the following Deposit Arrangement administration related activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Find Deposit Arrangements | Enter a value in the Arrangement field. Click the FIND button. Click the Overview icon. |
| Arrangement Overview (Deposits) | Click the New Activity option. |
| New Activities | Click the Do Activity Today icon corresponding to the Change Redemption Fee Condition (User) activity. |
| Arrangement Activity | Enter a value in the Narrative field. Click the Early Redemption Fee section. In the Calculation tab, enter a value in the Flat Charge field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Find Deposit . |
| Find Deposit Arrangements | Enter a deposit arrangement ID in the Arrangement field and then click the FIND button. Click the Overview icon corresponding to a record. |
| Arrangement Overview(Deposits) | Click the RUN icon corresponding to the Request Payment Holiday enquiry. |
| Repayment Holiday | Click the Skip Payment icon. Click the Validate icon. Enter values in the following fields: Number of Installments Holiday Amt Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Find Deposit . |
| Find Deposit Arrangements | Enter a deposit arrangement ID in the Arrangement field and then click the FIND button. Click the Overview icon corresponding to a record. |
| Arrangement Overview(Deposits) | Click the Modify/Cancel Payment icon corresponding to the Modify and Cancel Payment enquiry. |
| Arrangement Activities | Click the Validate icon. Enter a value in the Holiday Amt field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Find Deposit . |
| Find Deposit Arrangements | Enter a deposit arrangement ID in the Arrangement field and then click the FIND button. Click the Overview icon corresponding to a record. |
| Arrangement Overview(Deposits) | Click the Modify/Cancel Payment icon corresponding to the Modify and Cancel Payment enquiry. |
| Arrangement Activities | Click the Validate icon. Enter a value in the Cancel field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

There are no Outputs available for Savings Plan Product feature.


> **Related Applications:** `AA.OVERDUE.STATS`, `AA.PERIODIC.ATTRIBUTE`

---


### 1.33  Statements


> **📇 Quick Reference Card**
> 
> **Purpose:** *Customers require information about the deposit accounts maintained with the bank along with periodic information in the form of statements. This enables the customer to,*
> 
> **Applications:** `AA.ACTIVITY`, `AA.ARRANGEMENT.ACTIVITY`, `AA.PROPERTY`, `AC.POSTING.DETAIL`, `AC.POSTING.DETAILS`, `PRINTER.ID`, `REPORT.CONTROL`, `STMT.ENTRY`
> 
> **Key Fields:** *Arrangement*, *Full Description*, *Narrative*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Customers require information about the deposit accounts maintained with the bank along with periodic information in the form of statements. This enables the customer to,

- View the current position of the deposit at a given point of time.
- Plan renewal or redemption of deposits.

The statement displays the Narrative field, which describes the transaction or activity triggered. The Retail Deposits (AD) module allows amending the Narrative field to include more details of the transaction or activity.

In the TBC, the account statement features are available only for the print carrier. The system generates a record in STMT.ENTRY for every transaction in the deposit only for the statement generation purposes. The system uses these entries in statement generation and hands off to a Print Carrier solution during the statement frequency. These statements can be printed using the PRINTER.ID and REPORT.CONTROL setup. When the printing solution is not configured, the statements are held in &HOLD& folder.

Other statement solutions like CAMT, XML, swift statements should be handled by an external system.


#### ⚙️ Configuration

Statement Product Condition in Retail Deposits allows the user to define the,

- Frequency cycle for the generation of deposit account statement.
- Periodic statements that has to be sent to customer in any specific frequency as deemed fit by the bank, such as daily, weekly, fortnightly, or any day of every month.

The statements display the entries since the last statement in that cycle. Read the Statement Property Class user guide to understand field level details.

For user-defined activities, the user can configure the Narrative field to identify the transaction and map to the accounting entries using the AA soft accounting.

In AA.ARRANGEMENT.ACTIVITY , the Narrative field allows the user to describe the activity transaction. Additionally, in AC.POSTING.DETAIL , the user has the flexibility to extract information from the Full Description fields in the AA.PROPERTY and AA.ACTIVITY tables, which can be appended to the accounting entries.

In AC.POSTING.DETAIL , three additional narratives appear in the Narrative field of the STMT.ENTRY record. They are:

- Multi value 1 is the Full Description field from the AA.PROPERTY record.
- Multi value 2 is the Full Description field from the AA.ACTIVITY record.
- Multi value 3 a user-defined Narrative field entered in the AA.ARRANGEMENT.ACTIVITY .


#### 🔧 Working With

The below screenshot displays an arrangement activity, which is a transaction for reversal of bonus charge paid on a deposit arrangement.

The STMT.ENTRY application displays the three fields of narrative as defined in AC.POSTING.DETAILS .

The user can check the enquiry to view detailed narrative for the particular transaction activity.

In the TBC, the account statement features are available only for the print carrier. The system generates a record in STMT.ENTRY for every transaction in the deposit only for the statement generation purposes. The system uses these entries in statement generation and hands off to a Print Carrier solution during the statement frequency. These statements can be printed using the PRINTER.ID and REPORT.CONTROL setup. When the printing solution is not configured, the statements are held in &HOLD& folder.

Other statement solutions like CAMT, XML, swift statements should be handled by an external system.


#### 📋 Tasks

Related topics:

- Generate Deposit Advices

Customers require information about the deposit accounts maintained with the bank along with periodic information in the form of statements.


##### Workflow

This section allows the user to perform the below activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Find Deposit Arrangements | Enter an account arrangement ID in the Arrangement field and then click the FIND button. Click the Overview icon corresponding to a record. |
| Arrangement Overview (Deposit) | Click the Update icon corresponding to the Statement Details enquiry. |
| New Activities | Click the Do Activity Today icon corresponding to Update Tax Condition activity. |
| Arrangement Activity | Click the Validate icon. Enter values in the following fields: Statement Frequency Combined Statement Product Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

When a deposit has been created for the customer, the user can view the deposit details from the deposit report.


##### Enquiries and Reports

This section allows the user to view the below enquiries and reports:

Deposit Report

This enquiry displays the details of Arrangement Status, Current Principal, Tax, Charges, Interest, Maturity Date and so on, corresponding to a particular deposit Arrangement held by a customer.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA


> **Related Applications:** `AA.ACTIVITY`, `AA.ARRANGEMENT.ACTIVITY`, `AA.PROPERTY`, `AC.POSTING.DETAIL`, `AC.POSTING.DETAILS`, `PRINTER.ID`, `REPORT.CONTROL`, `STMT.ENTRY`

---


### 1.34  Swift Messages for Deposit


> **📇 Quick Reference Card**
> 
> **Purpose:** *From the creation of a deposit arrangement to its maturity and renewal, the system triggers advices and messages to the customers. For instance, when the customer funds the arrangement through a cheque clearing settlement, the bank triggers notifications to the customer on clearing of cheques and cr...*
> 
> **Applications:** `DE.MAPPING`, `DE.MESSAGE.SETUP`, `EB.ADVICES`
> 
> **Key Fields:** *Arrangement*, *Customer*, *Mapping Key*, *Role*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

From the creation of a deposit arrangement to its maturity and renewal, the system triggers advices and messages to the customers. For instance, when the customer funds the arrangement through a cheque clearing settlement, the bank triggers notifications to the customer on clearing of cheques and creation of deposits. Similarly, prior to the maturity of the deposit arrangement, the bank can alert the customer maybe a week in advance so that the customer can plan to either renew or redeem the deposit contract on the due date.

The Retail Deposits (AD) module allows the user to configure the below SWIFT type messages for corporate customers who are eligible to receive them.

- MT320 - For fixed loan confirmation
- MT350 - For deposit interest payment
- MT935 - For rate change advice


##### Risk Free Rates

The following are the SWIFT messages related to RFR:

- MT320 - For RFR contracts, the interest rate is populated with 0000 in case of CONF and ROLL events. The MATU event has the final interest rate populated.
- MT350 - For RFR-linked contracts, the interest rate is populated with 0000 in case of CONF events and the settlement advice has the interest rate populated.
- MT935 - For RFR contracts, the rate change advice is not generated as the rate resets daily.

The features related to activity messaging are not applicable for deposits in TBC and are handled by external systems. In TBC, notifications for deposits are provided in the form of events which should be consumed by the appropriate external delivery system for further processing.

Alerts can be configured in the TBC and the alert messaging content is handed off as an event to the delivery system associated to the TBC in a pre-configured format.

Read here to know more about TBC for deposits.


#### ⚙️ Configuration

The Retail Deposits (AD) module enables the user to configure alerts and messages for various types of activities using the conditions of Activity Messaging Property Class and the EB.ADVICES application.

The EB.ADVICES application manages the,

- Output of delivery message
- Type of format for messages
- Deal slips for activity

The AA-320 record of the EB.ADVICES displays the acknowledgement message for the creation of a new deposit arrangement. The Mapping Key fields provides the details of mapping in the DE.MAPPING record.

The EB.ADVICES record displays the setup for AA-320 message format definition.

The DE.MESSAGE.SETUP displays the setup for MT320 message format defintion.

The DE.MAPPING record displays details of field level mapping for the message to be delivered.

The EB.ADVICES record is mapped to a specific Activity or Activity Class ID in the condition of Activity Messaging Property Class.

Whenever the system triggers DEPOSITS-NEW-ARRANGEMENT Activity , the system triggers the relevant message AA-320.

If the user specifies the Role field as Owner, Joint Owner, etc., then it checks whether the customer related to the arrangement is having the roles assigned to them. Only when the roles are present the system processes the message for those particular customers.

If no Role field is left blank, then the bank sends message to all the related customers. When there are no matching roles in the deposit arrangement, then the system does not process the message.


#### 🔧 Working With

Read the AA (Advices and Alerts section) user guide for more information about customer preferences for delivery messages.


#### 📋 Tasks

Related topics:

- Open Deposit (AA)

Prior to the maturity of the deposit arrangement, the bank alerts the customer in a week advance so that the customer can plan to either renew or redeem the deposit contract on the due date.


##### Workflow

This section allows the user to perform the below activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Find Deposit Arrangements | Enter an account arrangement ID in the Arrangement field and then click the FIND button. Click the Overview icon corresponding to a record. |
| Arrangement Overview (Deposit) | Click the New Activity option. |
| New Activities | Click the Do Activity Today icon corresponding to Change Deposit Interest (User) activity. |
| Arrangement Activity | Click the Correspondence option in the Additional Details enquiry. Click the Alerts option in the Messages enquiry. Click the Subscribe for New Alert icon. Click the Subscribe icon corresponding to Arrangement Matured option. Enter a value in the Customer field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

When a deposit has been created for the customer, the user can view the deposit details from the deposit report.


##### Enquiries and Reports

This section allows the user to view the below enquiries and reports:

Correspondence

This enquiry displays the details of deposit Arrangement held by a customer.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA


> **Related Applications:** `DE.MAPPING`, `DE.MESSAGE.SETUP`, `EB.ADVICES`

---


### 1.35  Tax


> **📇 Quick Reference Card**
> 
> **Purpose:** *Tax is applied either on financial properties of an arrangement or on specific transactions. Financial properties include interest, charge, periodic charge, and account.*
> 
> **Applications:** `AA.ARRANGEMENT.ACTIVITY`, `AA.BILL.DETAILS`, `CUSTOMER.CHARGE`, `TAX`, `TAX.TYPE`, `TAX.TYPE.CONDITION`
> 
> **Key Fields:** *Actual Group*, *Arrangement*, *Context Tax Code*, *Context Tax Condition*, *Currency*, *Customer*, *Effective Date*, *GB Narrative* ... +12 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Tax is applied either on financial properties of an arrangement or on specific transactions. Financial properties include interest, charge, periodic charge, and account.

Different types of tax such as Withholding tax, Income tax and VAT can be calculated. Tax amounts can be displayed in the customer statements either separately or after netting off with interest or charge.

The system supports proportionate tax if there is a change in the tax structure during the interest payment period.

There are no specific limitations with regards to calculating and processing of taxes for deposits in TBC.

The tax related assessments are generally performed based on the customer attributes and these attributes are part of an external Party system like the Party TBC. Hence, the tax group that the customer belongs to can be updated using an API in the Actual Group attribute of the CUSTOMER.CHARGE application in TBC.


#### ⚙️ Configuration

The system enables tax calculation during issue bills, make due and capitalise for the respective interests, charges, periodic charges, account property and activities when configured in the tax condition. The calculated tax is updated against the TAX Property in the bill.

The system calculates tax with the support of the following core tables.

- The TAX table provides for each code, the percentage rate of tax, category and tax operand details.
- The TAX.TYPE table provides the ID for tax.
- The TAX.TYPE.CONDITION table includes the TAX.TYPE record and relate the TAX code.

The Tax Property Class relates the Interest or Charge Property Class with either TAX code or value from TAX.TYPE.CONDITION .

If the values at the product level for Tax Property Class are marked negotiable, then the TAX or TAX.TYPE.CONDITION can be populated.

It is possible to net interest amounts at the time of interest capitalisation of any set of interest property amounts.

Read the Tax Property Class user guide for more information.

Based on the setting in the Accounting Property Class, it is possible to book the tax entries as itemised along with interest and charges and not as single entry. This can either be a Property or Property Class specific choice.

The Property Class field indicates if the entries for that Property Class has to be Net or Itemised in the Method field. At the Property level, the user can choose the Property and mark it as Net or Property in the Method field.

To complete the tax related balance updates or accounting, the TBC generates an event which can be captured by the connected external GL (General Ledger) system.


##### Tax on Activities

Tax can be calculated on the transaction amount, bill amount or any balance when specific activities with activity class Type Process.tax are triggered. The user can configure the Trans Activity , Trans Bill Type , Trans Source Type , Trans Payment Type , and Trans Source Balance fields in the AA Tax property to define the activity on which the tax is to be calculated.

For Deposits product line, tax can be calculated for the following activities:

- Withdrawal from a deposit
- Deposit funding and other transactions triggered from a payment system (that is, DEPOSITS-APPLYPAYMENT-PAYMENT.RULES and DEPOSITS-APPLYPAYMENT-PAYOUT.RULES)
- Issue Bill for Charge, Periodic charges, and Payment schedule.


##### Tax on Account Property Made-Due or Paid

The user can define the tax condition to calculate tax on ACCOUNT property that is made-due or paid. For example, during deposit funding, tax can be collected on the expected amount by setting the Property field to the Account property defined in the deposit product. The Prop Tax Code or Prop Tax Cond field should be defined to specify the details (rate) for tax calculation.

For Deposits product line, tax is calculated on ACCOUNT property during

- Funding a deposit
- Deposit redemption
- Deposit Maturity (Tax on the payout amount that is created during maturity of the deposit)
- Deposit rollover with Maintain schedule (Tax on the amount that is paid out)
- Scheduled Make-Due of ACCOUNT properties (that is, Tax on PAY balance created during scheduled make-due based on the payment schedule definition).


##### Overriding Default Tax Conditions using Context Types

For tax on activities, it is possible that the user can pass overriding tax rate/amount at the AA.ARRANGEMENT.ACTIVITY level by using the context fields. This can be done by defining the Prop Tax Context , Tax Context , Context Tax Code , and Context Tax Condition fields in the Tax condition.

Read Overriding Default Tax Conditions using Context Types for more information.


#### 🔧 Working With

The system calculates tax on the interest part of the deposit arrangement.

The system assigns the Withholding Tax (WHT), as the tax type in the Tax Code Tax Condition field and applies 15% as withholding tax on the customer group.

The AA.BILL.DETAILS application for the deposit arrangement, for the interest amount, as displayed in the below screenshot holds the tax value with the property on which the tax has been calculated.

On a total bill amount of 145.82 USD, the system calculates tax of 15%, which is 21.87 USD. The Property field in AA.BILL.DETAILS displays the tax as DEPOSITINT-TAX with the amount.

The tax related assessments are generally performed based on the customer attributes and these attributes are part of an external Party system like the Party TBC. Hence, the tax group that the customer belongs to can be updated via an API in the Actual Group attribute of the CUSTOMER.CHARGE application in TBC.


##### Tax on Activities

Tax can be calculated on the transaction amount, bill amount or any balance for specific activities. The AA Tax property can be defined to mention the activity for which tax is to be calculated, the source balance and other details for calculating the tax amount. Consider,

- Transaction amount – USD 10,000
- Federal tax rate – 10%
- State tax rate – 15%

| Net | Gross |
|---|---|
| Federal tax amount = 10%*10,000=1000 State tax rate = 15%*10,000=1500 Total tax amount = 1000+1500=2500 | Federal tax amount =(10,000/(100-15)*10)=1333.33 State tax rate = (10,000/(100-15)*15)=2000 Total tax amount = 1333.33+2000=3333.33 |

The user can define the Tax condition and tax property to calculate tax on the following activities in deposits:

| Trans Activity | Trans Bill Type | Trans Source Type | Activity Class Type | Tax Calculation Method | Accounting |  |
|---|---|---|---|---|---|---|
| Tax Method/ Payment Method | Capitalise | Due |  |  |  |  |
| DEPOSITS-WITHDRAW-PAYOUT.RULES | - | TXN.AMOUNT | Process Tax, Gross Net Tax | Net | Dr CURACCOUNT -7500 Cr Customer account 7500 Dr CURACCOUNT -2500 Cr Internal account(tax) +2500 | Dr DUETAX -2500 Cr Internal account (tax) +2500 Dr CURACCOUNT -10000 Cr Customer account 10000 |
| Gross | Dr CURACCOUNT -10000 Cr Customer account 10000 Dr CURACCOUNT -3333.33 Cr Internal account(tax) +3333.33 | Restricted |  |  |  |  |
| DEPOSITS-REDEEM-ARRANGEMENT | PAYMENT | BILL.AMOUNT | Process Tax | Net | Dr CURACCOUNT -10000 Cr PAYACCOUNT +10000 Dr PAYACCOUNT -2500 Cr Internal account(tax) +2500 |  |
| Gross | Restricted |  |  |  |  |  |
| DEPOSITS-APPLYPAYMENT-PAYMENT.RULES | - | TXN.AMOUNT | Process Tax | Net | Dr Customer account -10000 Cr Properties in payment rules condition +10000 Dr CURACCOUNT -2500 Cr Internal account(tax) +2500 | Dr. Customer Account -10000 Cr. Properties in payment rules condition +10000 Dr. DUETAX -2500 Cr. Tax Internal Account +2500 |
| Gross | Restricted |  |  |  |  |  |
| DEPOSITS-APPLYPAYMENT-PAYOUT.RULES | - | TXN.AMOUNT | Process Tax, Gross Tax | Net | Dr Properties in Payout rules condition -10000 Cr Customer account 10000 Dr CURACCOUNT -2500 Cr Internal account(tax) +2500 | Dr DUETAX -2500 Cr Internal account (tax) +2500 Dr Properties in Payout rules condition -10000 Cr Customer account 10000 |
| Gross | Dr Properties in Payout rules condition -10000 Cr Customer account 10000 Dr CURACCOUNT -3333.33 Cr Internal account(tax) +3333.33 | Restricted |  |  |  |  |
| DEPOSITS-ISSUEBILL-CHARGE (Debit type of charges) | ACT.CHARGE | BILL.AMOUNT | Process Tax | Net | Dr CURACCOUNT -10000 Cr Charge PL +10000 Dr CURACCOUNT -2500 Cr Internal account(tax) +2500 | Dr DUETAX -2500 Cr Internal account (tax) +2500 Dr DUECHARGE -10000 Cr Charge PL +10000 |
| DEPOSITS-ISSUEBILL-PERIODIC.CHARGES (Debit type of charges) | PAYMENT | BILL.AMOUNT | Gross | Tax calculation using Gross method is not applicable for this activity. The bill is generated and tax is calculated by Net method (as it is the default tax calculation method). |  |  |
| DEPOSITS-ISSUEBILL-CHARGE (Credit type of charges) | ACT.CHARGE | BILL.AMOUNT | Process Tax | Net | Cr CURACCOUNT +10000 Dr Charge PL -10000 Dr CURACCOUNT -2500 Cr Internal account(tax) +2500 | Dr Charge PL -10000 Cr PAYCHARGE +10000 Dr PAYCHARGE -2500 Cr Internal account (tax) +2500 |
| DEPOSITS-ISSUEBILL-PERIODIC.CHARGES (Credit type of charges) | PAYMENT | BILL.AMOUNT | Gross | Tax calculation using Gross method is not applicable for this activity. The bill is generated and tax is calculated by Net method (as it is the default tax calculation method). |  |  |
| DEPOSITS-ISSUEBILL-PAYMENT.SCHEDULE (Interest property) | PAYMENT | BILL.AMOUNT | Process Tax, Gross Tax | Net | Cr CURACCOUNT +10000 Dr ACCINTEREST -10000 Dr CURACCOUNT -2500 Cr Internal account(tax) +2500 | Dr ACCINTEREST -10000 Cr PAYINTEREST +10000 Dr PAYINTEREST -2500 Cr Internal account (tax) +2500 |
| Gross | Tax calculation using Gross method is not applicable for this activity. The bill is generated and tax is calculated by Net method (as it is the default tax calculation method). |  |  |  |  |  |
| DEPOSITS-ISSUEBILL-PAYMENT.SCHEDULE (Account property) | PAYMENT | BILL.AMOUNT | Process Tax, Gross Tax | Net | Account when capitalised comes back to Deposit account balance. | Dr CURACCOUNT -10000 Cr PAYACCOUNT +10000 Dr PAYACCOUNT -2500 Cr Internal account (tax) +2500 Total Outstanding Bill Amount is 7500 CREDIT |
| Gross Applicable only for Pay type of bill for ACCOUNT property | Account when capitalised comes back to Deposit account balance | Dr CURACCOUNT -13333.33 Cr PAYACCOUNT +13333.33 Dr PAYACCOUNT -3333.33 Cr Internal account(tax) +3333.33 Total Original Bill Amount is 13333.33 and Outstanding Bill Amount is 10000 CREDIT. |  |  |  |  |

> **⚠️ Note:** In the case of Issue Bill activities for Deposits, tax can be calculated using Gross method only for DEPOSITS-ISSUEBILL-PAYMENT.SCHEDULE activity with a credit type of Account property. In all other cases, the Issue Bill activity is processed, and the corresponding tax is calculated using Net method as this is the default calculation method. An override is raised to indicate the same and can be viewed in the corresponding AA.ARRANGEMENT.ACTIVITY record. When transaction tax is set for DEPOSITS-ISSUEBILL-PAYMENT.SCHEDULE activity for Account property, Gross tax calculation method is restricted for the last payment schedule as it can result in a debit balance in the deposit. The system raises an error in this scenario and hence, it is recommended to not define Gross tax calculation method for the last payment schedule in deposits.


##### Tax on Account Property Made-Due or Paid

The user can define the tax condition to calculate tax on ACCOUNT property that is made-due or paid by setting the Property field to the Account property defined in the deposit product. Consider,

- Account Property Made-Due or Paid – USD 10,000
- Federal tax rate – 10%
- State tax rate – 15%

| Net | Gross |
|---|---|
| Federal tax amount = 10%*10,000=1000 State tax rate = 15%*10,000=1500 Total tax amount = 1000+1500=2500 | Federal tax amount =(10,000/(100-15)*10)=1333.33 State tax rate = (10,000/(100-15)*15)=2000 Total tax amount = 1333.33+2000=3333.33 |

The user can define the tax condition to calculate tax for the following activities which makes the Deposit Balance as Due or Pay:

| Use case | Tax Calculation Method | Accounting |
|---|---|---|
| Deposit Funding During deposit funding, the tax calculated on the Account property is made due by default and this cannot be modified. | Net | Cr CURACCOUNT 10000 Dr EXPACCOUNT -10000 Dr DUETAX -2500 Cr Internal account(tax) +2500 Total Outstanding Bill amount is 12500 DEBIT |
| Gross | Restricted |  |
| Deposit Redemption | Net | Dr CURACCOUNT -10000 Cr PAYACCOUNT +10000 Dr PAYACCOUNT -2500 Cr Internal account(tax) +2500 Total Outstanding Bill Amount is 7500 CREDIT |
| Gross | Restricted |  |
| Deposit Rollover with Maintain Schedule (where the deposit is rolled over with 60% of the proceeds and 40% is paid out to the customer). In this example, 10,000 is the 40% amount that is paid out. | Net | Dr CURACCOUNT -10000 Cr PAYACCOUNT +10000 Dr PAYACCOUNT -2500 Cr Internal account(tax) +2500 Total Outstanding Bill Amount is 7500 CREDIT |
| Gross | Restricted |  |
| Deposit Maturity | Net | Dr CURACCOUNT -10000 Cr PAYACCOUNT +10000 Dr PAYACCOUNT -2500 Cr Internal account(tax) +2500 Total Outstanding Bill Amount is 7500 CREDIT |
| Gross | Restricted |  |
| Deposit Scheduled Make-Due The Gross tax calculation method is not applicable for the last payment schedule in Deposits as it can result in a debit balance in the deposit. | Net | Dr CURACCOUNT -10000 Cr PAYACCOUNT +10000 Dr PAYACCOUNT -2500 Cr Internal account(tax) +2500 Total Outstanding Bill Amount is 7500 CREDIT |
| Gross Applicable only for Pay type of bill for ACCOUNT property | Dr CURACCOUNT -13333.33 Cr PAYACCOUNT +13333.33 Dr PAYACCOUNT -3333.33 Cr Internal account(tax) +3333.33 Total Original Bill Amount is 13333.33 and Outstanding Bill Amount is 10000 CREDIT |  |


##### Overriding Default Tax Conditions using Context Types

The tax rate that is configured at the tax condition level can be overridden at the arrangement activity level for tax on activities. The user can pass overriding tax rate/amount at the AA.ARRANGEMENT.ACTIVITY level using the context fields.

Read Overriding Default Tax Conditions using Context Types for more information.


#### 📋 Tasks

Related topics:

- Open Deposit (AA)

Banks can apply tax for interest, charge, periodic charge, account property, and activities of a deposit arrangement. Tax can be calculated and overwritten at the arrangement activity level when specific activities are triggered.


##### Workflow

This section allows the user to perform the below activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Find Deposit Arrangements | Enter an account arrangement ID in the Arrangement field and then click the FIND button. Click the Overview icon corresponding to a record. |
| Arrangement Overview (Deposit) | Click the New Activity option. |
| New Activities | Click the Do Activity Today icon corresponding to Update Tax Condition activity. |
| Arrangement Activity | Enter a value in the GB Narrative field. Click the Validate icon. Click the Tax tab and then enter values in the following fields: Property Tax Code Tax Condition Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Tax . |
| Define tax condition | Define the Prop Tax Context , Tax Context , Context Tax Code , and Context Tax Condition fields in the tax product condition for the Transaction Tax property. |
| Product Proof and Publish | Proof and Publish the product using the Product Manager application |
|  | Product Catalog . |
| Product Catalogue | Click the New Arrangement icon corresponding to Retirement Plan Deposits. |
| New Arrangement | Enter values in the following fields. Customer Currency Effective Date Enter the commitment amount and term of the deposit. Click the Validate a deal icon to check for errors and overrides. Click the Commit the deal icon. |
| Find Deposit Arrangements | Authorised . Enter the deposit arrangement ID in the Arrangement field and then click the FIND button. Click the Overview icon corresponding to a record. |
| Arrangement Overview (Deposit) | Click the Withdraw Deposit option. |
| Arrangement Activity | Enter Withdrawal Amount . Enter the overriding tax details using the context fields for the TAX.CALC.METHOD context types and other user defined context types for passing the tax rate or amount. Click the Validate a deal icon to check for errors and overrides. Click the Commit the deal icon. |


#### 📊 Outputs

There are no Outputs available for Tax feature.


> **Related Applications:** `AA.ARRANGEMENT.ACTIVITY`, `AA.BILL.DETAILS`, `CUSTOMER.CHARGE`, `TAX`, `TAX.TYPE`, `TAX.TYPE.CONDITION`

---


### 1.36  Valuations and Interface to Securities Module


> **📇 Quick Reference Card**
> 
> **Purpose:** *An arrangement can be active in a portfolio only when the customer funds the deposit arrangement.*
> 
> **Applications:** `ASSET.TYPE`, `SC.POS.ASSET`, `SUB.ASSET.TYPE`
> 
> **Key Fields:** *Margin Rate*, *Portfolio ID*, *Portfolio Id*, *Portfolio No.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

An arrangement can be active in a portfolio only when the customer funds the deposit arrangement.

Read the Funding of Deposits user guide for more information.

The features related to linking of deposits to the customer portfolio for the purpose of combined portfolio valuation and management are not applicable in TBC. These functionalities can be enabled through external solutions. Read here to know more about TBC for deposits.


#### ⚙️ Configuration

The Portfolio ID attribute in the Account Property Class indicates the portfolio, which links the customer’s arrangements, such as loans, deposits, or even savings under the same ID. This is done only while creating a new arrangement or during the arrangement period. No additional configuration is required.

Read the Reporting Property Class user guide for more details on Position Management linked to AA Deposits.


#### 🔧 Working With

The Portfolio ID field in the Account Property Condition allows the user to input the ID, which links the customer’s arrangements, such as loans, deposits, or even savings under the same ID.

An arrangement is active in a portfolio only after a disbursal (in case of loans) or a settlement is done (in case of deposits).

The customer can hold the arrangement in any foreign currency and the portfolio in the local currency (USD), which is cross-currency valuation. In this case, the system picks rates from the currency table automatically. Any kind of changes made to the disbursed loan or settled deposit reflects in the portfolio indicating a movement of funds. Changes such as, change interest, redemption of funds, payoff or closure, partial funding within cancel period, partial withdrawal from deposit, increase of term amount, term etc. are possible.

The AA valuation can be configured into the Securities module depending on the parameter setting required. The following screenshot displays a simple configuration with the creation of ASSET.TYPE and SUB.ASSET.TYPE .

Read the Securities user guide for more details on the possible configuration for valuation.

The below screenshot displays the SUB.ASSET.TYPE that links the ASSET.TYPE to the new SUB.ASSET.TYPE

> **⚠️ Note:** The user can link only one sub asset type to an asset type at a time.

The user can specify different margin rates for different asset types.

> **⚠️ Note:** The margin rates specified in the Margin Rate field becomes effective only for deposit type arrangements, that is, the margin value amount in the SC.POS.ASSET file updates only for a deposit account. The same is not applicable for loans.

The system displays the portfolio ID in the Portfolio No. field in the Account Conditions, at arrangement level, to enable AA to be included in the portfolio valuations.

The user can view the valuation using the Portfolio Valuation-Cost enquiry.

The system updates the SC.POS.ASSET file only after the above query is run.


#### 📋 Tasks

Related topics:

- Open Deposit (AA)

The Portfolio ID field in the Account Property Condition allows the user to enter the ID, which links the customer’s arrangements, such as, loans, deposits, or even savings under the same ID.


##### Workflow

This section allows the user to perform the below activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Product Catalog . |
| Product Catalogue | Click the New Arrangement icon corresponding to Fully Negotiable deposit. |
| New Arrangement | Enter values in the following fields: Customer Currency Effective Date Click the Validate icon. Select the Account option and then click the Additional tab. Enter a value in the Portfolio Id field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

There are no Outputs available for Valuations and Interface to Securities Module feature.


> **Related Applications:** `ASSET.TYPE`, `SC.POS.ASSET`, `SUB.ASSET.TYPE`

---


### 1.37  Withdrawal from a Deposit


> **📇 Quick Reference Card**
> 
> **Purpose:** *The interest payable to the customer and the excess funds paid can be withdrawn from the deposit. These withdrawals can be posted as per the customer settlement requests or can be withdrawn by the customer until which they form part of the arrangement balances.*
> 
> **Applications:** `AC.ALLOCATION.RULE`, `BENEFICIARY`, `PAYMENT ORDER`, `PAYMENT.ORDER`, `PAYMENT.ORDER.PARAMETER`, `PAYMENT.ORDER.PRODUCT`, `TRANSACTION`
> 
> **Key Fields:** *Adjust Balance Type*, *Adjust Description*, *Adjust Property*, *Adjustment Amount*, *Arrangement*, *Change To Product*, *Counterparty*, *Counterparty Type* ... +12 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The interest payable to the customer and the excess funds paid can be withdrawn from the deposit. These withdrawals can be posted as per the customer settlement requests or can be withdrawn by the customer until which they form part of the arrangement balances.

The Payout Rules Property Condition along with the Settlement Property Condition governs the payment of balances from the deposit arrangement at the time of settlement activities such as interest payout, excess funds payout, maturity proceeds payout, early mature or early redemption of deposits. The amount is paid to the specified savings account within the bank or to other bank accounts of the customer, using the PAYMENT.ORDER application.

The outgoing payments in a deposit can be restricted to pre-defined counter accounts only which are added during deposit opening and maintenance processes.

In TBC, when the user withdraws funds from the deposit, the system proceeds to settle the balances to an account within the TBC. If the account or beneficiary is outside the TBC, the system forwards a settlement request to the account or beneficiary by publishing an event which should be consumed by an external payments system, for further processing.

Hence, the payment order related details are not applicable for deposits in TBC.

> **⚠️ Note:** It is not possible to define and process nominated counter party restrictions in deposits using TBC.


#### ⚙️ Configuration

The Payout Rules allow the banks to define the rules of payment of funds, out of the arrangement, such as interest, pay charges and excess funds received.

The Payout Rules Property Class lists the properties and sequences to be settled during the Interest Payout Activity (DEPOSITS-APPLYPAYMENT-PO.WITHDRAWAL) or Redemption Activity (DEPOSITS-APPLYPAYMENT-PO.EARLY.WITHDRAWAL).

The Reminder Activity (DEPOSITS-APPLYPAYMENT-PO.EARLY.WITHDRAWAL) will be the Apply Payment Activity for principal reduction, which facilitates partial pre-closure of deposits, upon customer request.

The Payout Rules definition can be used to pay the interest for the excess funds received.

The below screenshot displays the Payment Rule Type definition used to pay balances within the bill date.

The below screenshot displays the AC.ALLOCATION.RULE for DEPOSIT-ACCOUNT.

The Settlement Property Class has the below listed fields, which enable the payout settlement process.

- Payout Settlement - enables settlement. Yes for enabling settlement No for disabling the settlement
- Payout Ppty Class and Payout Property - Lists the Property Classes or Properties that are processed for Payout Settlement. This is a multi-value field and the user can input multiple properties that are to be paid out, such as principal, interest, pay charges, etc.
- Payout Account - Displays the account details in case the accounts are available within the bank. The user can input a valid account number, maintained in the system. The amount billed under the same payment date can be combined and settled as a single settlement when automatic settlement with the same account is defined.
- Payout Beneficiary - Links to the core BENEFICIARY table and defines the beneficiary of funds. This field is also used in concurrence with the Payout Po Product field. Read the Settlement using Payment Order user guide for more information.

In the TBC, when the user withdraws funds from the deposit, the system settles the balances to an account within the TBC. If the account or beneficiary is outside the TBC, the system forwards a settlement request to the account or beneficiary by publishing an event, which should be consumed by an external payments system for further processing. Hence, the payment order related details are not applicable for the deposits in the TBC.

The accounting related features and processing are handled by an external GL system, for deposits in the TBC. Therefore, when the withdrawal of a deposit is processed, the TBC generates an event, which can be consumed by the external GL (General Ledger) system, to complete the balance updates or accounting.

This application is responsible for

- Handling payment order requests from different sources (TCIB, AA),
- Passing the payments to the payment systems (FT, TPH, External System)
- Tracking the payment orders based on the responses received from the payment systems.

The PAYMENT.ORDER application is linked to AA, so that settlement actions, such as deposit funding, deposit payout and interest payment can be initiated using the Settlement Activity.

From Payment Order, payment instruction passes on to FT, TPH, or any External System for processing, based on the configuration in the PAYMENT.ORDER.PARAMETER .

PAYMENT.ORDER.PARAMETER - company level parameter table for the PAYMENT.ORDER application. In this application, the user can define the payment system through which instruction from payment order is processed in the Payment Connection Method field namely FT, TPS, External or a Conditional setup

- PAYMENT.ORDER.PRODUCT —The user can create a record for a product and define some specific configurations namely Allow FX (whether to allow for ex transaction or not) Allow BIC (for setting BIC as mandatory or non-mandatory) Check Account Restrictions
- The setup defined is automatically default to the Payment Order record.
- BENEFICIARY : In this application, the user can pre-define the beneficiary details and this defaults to the PAYMENT ORDER record. The user can define the following details, Beneficiary Account Number Beneficiary Name Beneficiary Bank Details
- Settlement Product Condition: The user can create a Settlement Product Condition, where the record name created in the PAYMENT.ORDER.PRODUCT table are listed in the Pref Product field.

All other existing setup, such as Settlement Activity, Payment Type, etc., should also be included in the Settlement Product Condition and attached to an AA Product.

Now, on creating an Arrangement using this product, all Settlement Product Conditions are defaulted to the record. The user can include the already created BENEFICIARY record ID in the settlement instruction.

On execution of the Activity defined in the Settlement Product Condition, the payment instruction from an Arrangement is mapped to the PAYMENT.ORDER application.

Based on the configuration in the PAYMENT.ORDER.PARAMETER record, the instruction will move to FT, TPH or an External System. In the Arrangement Overview screen, the user can click the Payment Order tab to view the PO record.

The user can offset pay bills generated with existing due bills and vice versa. The corresponding property is offset with the pay or due bill generated.

- Offset Property Class—indicates the Property Class balance to be offset.
- Offset Property—indicates the Property balance to be offset.
- Offset Required—defines whether offset of balances is required for the Property Class or Property.

The following are the available values:

- Active or Yes—denotes offset required
- No—denotes offset not required.

The following activities indicate the activities that define the list of due balances need to be offset using pay balance.

- Offset Pay in Activity specifies the Offset Payment Rule Activity that defines the list of due balances that need to be offset using the pay balance.
- Offset Pay out Activity specifies the Offset Payout Rule Activity that defines the list of pay balances that need to be debited to offset due balance created.

It is possible to offset outstanding due bill raised against a pay bill raised now. The Activity Class is used for the same. When a pay is raised, the due bill outstanding for the property indicated is settled immediately and the remaining is paid

It is possible to offset outstanding pay bill against due bill raised now. The Activity Class is used for the same. When a due is raised, the pay bill outstanding for the property indicated is settled immediately and the rest is made due.


##### Nominated Counter Accounts

The outgoing payments to a deposit can be restricted to pre-defined counter accounts only which are added during deposit opening and maintenance processes. This can be achieved using the associated multi-value set of fields - Counterparty Type and Counterparty in the account condition.

Read Notification for Nominated Counterparty Details and Notification for Change in Beneficiary Details of a Nominated Counterparty to know about configuring notifications for nominated counter accounts in deposits.

In TBC, it is not possible to define, and process nominated counter party restrictions in deposits.


#### 🔧 Working With

The user can define a suitable payout rule to withdraw funds available in PAYACCOUNT, UNCACCOUNT or CURACCOUNT. For example, when there is excess amount paid over a bill, the system automatically moves this amount to the UNC account, thereby making it available for the user to withdraw.

The user can,

- Control the withdrawals from a contract in a given period using the Activity Restriction and Periodic Rules Property Classes.
- Charge the customer for withdrawals more than the permissible limit.
- Charge the customer for every transaction performed on this contract or for selected transactions alone. The charges can also be deferred over a certain period, depending on the customer’s requirement.

The user can simulate the withdrawal transaction to the current , future or a back date. It can also allow the pre-closure of contracts by allowing the customer to withdraw all the available balances including the accrued interest.

The user can capture balances for takeover contracts and can withdraw the same.


##### Illustration for Settlement

The Settlement account is defined to determine the account to which the payout can be done. This is triggered based on the Payout Settlement Activity as defined in the Payout Condition. It is also possible to define the Property and the associated Property Class for which the Settlement must happen.

In TBC, when the user withdraws funds from the deposit, the system proceeds to settle the balances to an account within the TBC. If the account or beneficiary is outside the TBC, the system forwards a settlement request to the account or beneficiary by publishing an event which should be consumed by an external payments system for further processing.

Hence, the payment order related details are not applicable for deposits in TBC.

A payment order can be generated, deposit funding or payment of funds from deposits (Charges, interest or maturity proceeds). PAYIN.BENEFICIARY and PAYIN.PO.PRODUCT, PAYOUT.BENEFICIARY and PAYOUT.PO.PRODUCT indicates the Beneficiary information and the relevant payment order product for configuration. -ISSUE.ORDER-ARRANGEMENT Activity Class indicates payment order generation.

The payout order request update the new suspense balance ADVANCE and ADVSUSPENSE; no new balance types for payment.

The ISSUE PAYMENT ORDER action is to create the order request in both payment and payout using Beneficiary. The ACCOUNTING action is used only for Payout - ADVANCE balance type and the new suspense balance accounting entry.

The below screenshot displays the Arrangement Overview page.

The below screenshot displays the Product and the associated Property Class for the Settlement

The below screenshot displays the details in the Payment Order.

The below screenshots displays the Funds Transfer and Additional Details in the Settlement Process.

When bill offsetting is setup and when a pay bill is generated with an outstanding due bill, the pay bill settles the due balances and the remaining balances are released as pay balances.

Likewise, when bill offsetting is setup, when a due bill is generated and a pay bill is outstanding, the due bill is offset with pay balances outstanding and the remaining balances are outstanding as due balances.

In a live arrangement, any backdated activity which invokes a financial recalculation (reverse and replay) that is, a backdated rate change, the system updates the defined settlement account and makes correcting entries.

The system creates a contra entry to reverse the previous debit or credit and replaces it with a new debit or credit (a delta adjustment is not made). Tax that is previously calculated is also corrected in the same manner.

In TBC, when there is back value dated correction, the system proceeds to settle the bills to an account within the TBC. If the account or beneficiary is outside the TBC, the system forwards a settlement request to the account or beneficiary by publishing an event which should be consumed by an external payments system for further processing.

The accounting related features and processing are handled by an external GL system for deposits in TBC. The TBC emits an event which can be captured by the connected external GL (General Ledger) system to complete the balance updates or accounting related to back valued dated adjustments.

An existing deposit arrangement calculates some payable interest with tax deducted and settles this to the dedicated settlement account 2000003592. A back dated rate change is transacted increasing the rate from 6 to 7.99 percent.

- A revised bill is created.
- The settlement account is debited (original amount) and credited the new calculated amount. In the below case a bill has been produced for the amount of GBP 2.18 (Interest GBP 3.12 minus Tax GBP 0.94). The defined settlement account is credited with interest amount. A backdated rate change is triggered changing from 6 to 7.99 percent. From the Deposit a new bill is created with a new amount of GBP 2.91 (Interest GBP 4.16 minus Tax GBP 1.25). The settlement account 2000003592 is updated with correcting entries. Dr GBP 2.18 correcting the original credit entry Cr GBP 2.91 posting new interest calculation


##### Nominated Counter Accounts

The outgoing payments in a deposit can be limited to pre-defined counter accounts or nominated counter accounts only using the Counterparty Type and Counterparty fields in the account condition. When the Counterparty Type is set to Pay.out or Both, the system validates if the beneficiary used for outgoing payments is one of the beneficiaries defined in the associated Counterparty field.

Based on the scenario , the counter account can be set only for Payin or for Payout or Both.

- When the system is set to evaluate the Payout transactions using the option Payout in Counterparty Type , only the outgoing payments with Validate Counter Party as Yes in TRANSACTION are monitored, and incoming payments are not monitored. The system raises an override when the payment is not made to one of the beneficiaries mentioned in the associated Counterparty field.
- When both incoming and outgoing payments should be evaluated, it is recommended to setup the Counterparty Type as Both and set Validate Counter Party as Yes in TRANSACTION code used. The system raises an override when the incoming payments are not received from or outgoing payments are not made to one of the beneficiaries mentioned in the associated Counterparty field.
- When the user prefers to ensure that Payin transactions must have a specific Beneficiary and Payout transaction must have a different Beneficiary, the Counterparty Type must be multivalued to take the values Payin and Payout and their respective beneficiaries must be defined alongside them as Counterparty .

Read here to know more on the working of counter accounts in a deposit.

In TBC, it is not possible to define, and process nominated counter party restrictions in deposits.


#### 📋 Tasks

Related topics:

- Perform Repayment of Deposit (AA)
- Account and Deposit Processes (Retail)

The Deposit Arrangement administration can be done by triggering various activities in a deposit arrangement through which various conditions can be updated as per the requirement.


##### Workflow

In Withdrawal from a Deposit, the user can perform the below activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Find Lending Arrangements | Enter a value in the Arrangement field. Click the FIND button. Click the Overview icon. |
| Arrangement Overview (Lending) | Click the New Activity option. |
| New Activities | Click the Do Activity Today icon corresponding to the Capture Balance activity. |
| Arrangement Activity | Enter a value in the Narrative field. In the Balance Maintenance section, enter values in the following fields: Adjust Description Adjust Property Adjust Balance Type New Balance Amount Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Find Lending Arrangements | Enter a value in the Arrangement field. Click the FIND button. Click the Overview icon. |
| Arrangement Overview (Deposits) | Click the New Activity option. |
| New Activities | Click the Do Activity Today icon corresponding to the Update Activity for Renewal activity. |
| Arrangement Activity | Enter a value in the Narrative field. In the Renewal Condition section, enter a value in the Change To Product field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

This option allows the user to perform AA Partial Withdrawal.

1. AA Partial Withdrawal .
2. Enter values in the following fields Debit Account Number Credit Account Payment Amount
3. Click the Validate icon to check for errors
4. Click the Commit icon and accept the Override, if any.
5. Run the BNK/PAYMENT.STPFLOW.HEAVY service for successful transaction.

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Find Deposit Arrangements | Enter the required field values and click the FIND button. |
| AA Arrangement | Enter a value in the Arrangement field. Click the FIND button. Click the Overview icon. |
| Arrangement Overview (Deposits) | Click the New Activity option. |
| New Activities | Click the Do Activity Today icon corresponding to the Update Settlement Instructions activity. |
| Arrangement Activity | Enter a value in the Narrative field. Click the Settlement Instruction section to expand. In the Initial Funding, Charges Settlement screen, enter values in the following fields: Active Y/N Settlement A/c In the Interest & Redemption Settlement screen, enter values in the following fields: Active Y/N Settlement A/c Click the Validate icon to check for errors and overrides. Click the Commit icon. Accept the overrides, if any. |


#### 📊 Outputs

There are no Outputs available for Withdrawal from a Deposit feature.


> **Related Applications:** `AC.ALLOCATION.RULE`, `BENEFICIARY`, `PAYMENT ORDER`, `PAYMENT.ORDER`, `PAYMENT.ORDER.PARAMETER`, `PAYMENT.ORDER.PRODUCT`, `TRANSACTION`

---


### 1.38  Chargeoff


> **📇 Quick Reference Card**
> 
> **Applications:** `AA.ACCOUNT.DETAILS`, `AA.ACTIVITY.HISTORY`, `AA.BILL.DETAILS`, `AA.INTEREST.ACCRUALS`, `CATEG.ENTRY`, `RE.CONSOL.SPEC.ENTRY`
> 
> **Key Fields:** *Bill Type*, *Charge Off Amount*, *Charge Off Percentage*, *Charge off Amount*, *Charge off Percentage*, *Full Chargeoff*, *New Property Amount*, *Or Prop Amt* ... +8 more
> 
> **Sections:** 🔧 Working With


#### 🔧 Working With

Working with Loan Charge-off Key Features Charge-off is different from writing off the arrangement. The key features of charge-off are: A full or multiple partial charge-off transaction is possible. The interest on the charge-off balance should accrue, but is not passed to income. Reversal of charge-off transactions is possible Removal from charge-off or partial removal from charge-off (that is, a lessening of the charge-off amount) is possible as well. Dual accounting –that is, having two sets of books, the customer record vs. the bank record and applying payments independently to the two records. The charge-off feature is available for the Lending Product Line. The Charge-off Property has to be included in the product for charging off an account. Activity Class - Charge-off Full/Complete Charge-off The LENDING-CHARGEOFF-ARRANGEMENT Activity Class is used for charge-off of an arrangement. The complete outstanding in the loan is charged off. Partial Charge-off or Charge-off in Parts It is possible to charge off a loan, in parts. The LENDING-CHARGE-OFF-ACCOUNT Activity Class is used to charge-off the Account Property balance, based on the charge-off order. This is used to both charge-off an amount of principal (that is, increase charge-off amount) and to reduce the charge-off (that is, decrease the charge-off amount) if required. If a loan is being charged-off for the first time, this Activity is responsible for creating the charge-off balances as well as the customer’s shadow balances. Handling Charge-off under FASB Regulations For handling charge-off under certain specific regulations (FASB), the bank user uses the CHARGEOFF-REPORTING activity. Differences in TBC The features related to handling charge-off under FASB regulations are not applicable for loans in TBC. Dual Accounting For loan contracts, apart from the customer balances, it is possible to store two separate balances, the bank balances along with the charge-off balances. When a Lending Product with Charge-off Property is proofed and published, the system automatically creates the balance type records to maintain charge-off balances along with the customer and bank balances. For a loan that is charged off, for CUR , the balances prior to the Charge-off Activity is stored as a shadow CUR CUST. The charge-off amount is stored in CUR CO and the amount under banks book is stored as CUR . The CUR CO charge-off balance, is the contingent balance and CUR CUST is a balance used for internal purpose and CUR is only non-contingent in nature. When the LENDING-CREDIT-ARRANGEMENT activity is processed, the amount credited to UNC is also credited to UNC CUST. When the LENDING-DEBIT-ARRANGEMENT activity is processed, the amount debited from UNC is also be debited from UNC CUST. Differences in TBC To complete the accounting to update the balances in a charged-off loan, the TBC generates an event, which can be captured by the connected external GL (General Ledger) system. Shadow Balances When a loan is charged-off, the borrower is unaware of this action, and continues to receive regular billing notices. As a result, when a loan is fully or partially charged off there is a situation to maintain two sets of books: A customer record (that is, the customer’s view of the balances and bills) A bank record (that is, the bank’s view of the balances). Prior to the charge-off, the customer and the bank records are the same (and therefore there is only one set of books). However once a loan is partially or fully charged off, the views are different. Customer Record Banks generally don’t communicate charge-off decision to the customers. So, a customer is unaware of a charge-off. Copying the balances prior to the Charge-off Activity creates a shadow record. This now becomes the customer record and does not include any of the effects of the charge-off. The bills and payments continue to be processed normally against this customer record. The payments received have to be apportioned as per the Payment Rules according to the customer. The customer balances are apportioned in this repayment order. Bank Record Full/Complete Charge-off For a full or complete charge-off using the LENDING-CHARGEOFF-ARRANGEMENT activity, there are no bank balances. The BNK balances are zero in this case. Charge-off in Parts/Partial Charge-off A charge-off creates the shadow balances for the customer record that do not include the effects of the charge-off (that is, the customer is completely unaware). As a result, the existing balances (customer balance less charge-off amount) continue to be referred to as the bank record and includes the effects of the charge-off (for example, the charged-off balance). As the arrangement advances, it also contains the interest accrual on the bank balance and charged-off balance separately. Additionally payments to the loan are allocated in a different manner on the bank record than on the customer record. This is based upon the value of the book balances and the status of the loan (for example, partially charged-off, fully charged-off or non-accrual). Internal inquiry screens display both the customer and the bank record, once a loan is partially or fully charged off. Reports breakdown the information this way as well – including both the bank balances and the customer balances. Charge-Off Balances The CUR CO and each ACC CO balance corresponds to the charge-off balance for the principal and the interest respectively. The system creates these balances by appending a CO at the end of each balance type. Differences in TBC To complete the accounting to update the balances in a charged-off loan, the TBC generates an event, which can be captured by the connected external GL (General Ledger) system. Multiple Interest Accruals For a full charge-off, the system accrues interest for charge-off and the customer balances namely CO and CUST balances. There is no bank balance to accrue interest for the BNK balances. For a partial charge-off (charge-off in parts), the system accrues interest for bank balance (for example, CUR ), charge-off and the customer balances. The system also accrues interest for the chargeoff and customer balances namely CO and CUST balances. It is necessary to accrue both charge-off and customer interest on the corresponding balances separately. Differences in TBC When a loan contract in TBC is charged-off, the TBC generates an event, which can be captured by the connected external GL (General Ledger) system to complete the accounting and balance updates. Full/Complete Charge-off During a full charge-off, the arrangement balances are moved to the Chargeoff PL. As part of shadow accounting, CUR CUST and CUR CO balances are maintained during a full Chargeoff. This results in the accrual of balances per Interest Property for each of this principal balance. Each of them accrues interest at the same rate but based upon their balance. ACC CUST is accrued on CUR CUST and ACC CO is accrued on CUR CO. Though multiple interest accruals are done based on different balances, definition of source balance for each type of accrual is not required. Product configuration contains: Property Source INTEREST CURACCOUNT Corresponding Accruals in a full charge-off loan are: Balance Source ACCINTERESTCO CURACCOUNTCO ACCINTERESTCUST CURACCOUNTCUST Partial Charge-off or Charge-off in Parts In a partial charge-off, there are three balances: CUR , CUR CUST, CUR CO. Hence, there are three accrual balances per Interest Property and each accrues interest at the same rate but based upon their balance. ACC is accrued on CUR then ACC CUST is accrued on CUR CUST. Though multiple interest accruals are done based on different balances, definition of source balance for each type of accrual is not required. The interest is calculated on: Property Source INTEREST CURACCOUNT Corresponding accruals in a partial charge-off loan are: Balance Source ACCINTEREST CURACCOUNT ACCINTERESTCO CURACCOUNTCO ACCINTERESTCUST CURACCOUNTCUST Product Setup and Charge-off Balances When a Lending Product with Charge-off Property is proofed and published, the system automatically creates the below balance type records to maintain customer, bank and charge-off balances. Except bank balances, other balance type records which are created by system are contingent in nature. Bank Balances Charge-off Balances Customer Balances CUR CUR CO CUR CUST DUE DUE CUST CUST UNC UNC CUST ACC ACC CO ACC CUST DUE DUE CUST CUST CUR CO balance type holds the cumulative amount that’s been charged-off against an account. ACC CO balance type is used for posting the accrued interest on charged-off balances namely CUR CO. Dual Billing In the case where a loan is in Charge-Off status, AA.BILL.DETAILS is updated with both the customer and the bank due amounts. For a complete charge-off, the reflection of the charge-off billing is found in the billed balances. The bank amount is zero For a partial charge-off, two sets of figures (the customer and bank amounts) are calculated and stored on the bill. The customer and the bank amounts differ due to the effect of the charged-off principal as well as the alternate way of applying credits to the arrangement. Illustration of Partial Charge-off The changes that happen in an arrangement when a charge-off is performed is illustrated with the help of the below example. The arrangement is in delinquent status and is being charged off using the LENDING-CHARGEOFF-ACCOUNT Activity giving the transaction amount as 80,000 USD. This means 80,000 USD of principal is charged off. The Loan Arrangement Overview is displayed below. The Charge-off Activity is shown below. The Loan Arrangement Overview After Charge-off is shown below. Comparison of Arrangement Balances Before And After Charge-off The ECB balances before charge-off of 80,000 is shown below. The ECB balances after charge-off of 80,000 is shown below. Note that the arrangement balances have changed as a result of the charge-off. Bill Generated Before/After Charge-off On bill generation, AA.BILL.DETAILS is updated with both the customer and the bank due amounts for each of these accruals. AA.BILL.DETAILS stores the bank related fields that get updated on and after the charge-off of an arrangement. Once the charge-off is done, then the customer balances are stored in existing amount related fields and bank balances are stored in the BNK (bank) fields. Overdue processing is triggered based on the bills getting aged. The Os Prop Amt and Or Prop Amt fields of the bill are based on the customer balances(original amount) and regular overdue processing is triggered for the same. Balance type AA.BILL.DETAILS CUR Os Prop Amt Bnk Or Prop Amt Bnk CUR CUST Os Prop Amt Or Prop Amt Key Features of Full/Complete Charge-off A complete charge-off is done using the LENDING-CHARGEOFF-ARRANGEMENT activity. After a complete charge-off is made in the arrangement, the Full Chargeoff field in the AA.ACCOUNT.DETAILS application displays Yes. During charge-off, the loan principal is charged off to the PL Category assigned to the Account property class. The interest is charged off to the PL Category assigned to the Interest property class. Any tax is charged-off to the PL Category assigned to the Tax property class. Validations During a Complete Charge-off When this activity is executed, the system performs the below validations and results in error in below scenarios: The bank performs the charge off after clearing any outstanding credit balances of the loan (like UNC/INV/AVL). Hence if there are any credit balances available during a charge-off, the system raises the following error. When there is a charge with outstanding pay balance, the arrangement cannot be charged off. The pay balance must be cleared and then charge-off should be triggered in the system. Post charge-off, the banks do not prefer to disburse any further loans or increase the loan commitment further. Hence, the disbursement activity is not allowed after the charge off. During the cooling and cancel period, the loan charge-off is not allowed. Any income to the arrangement is booked to the Chargeoff PL of that Property An arrangement that has undergone partial charge-off can undergo full charge-off, but an arrangement that is completely charged off cannot be charged off further. Loans cannot go to negative rate when loan is in charge-off. Dormant loans cannot be charged off. When an arrangement has a charge set to amortise, the charge cannot be charged off. The system raises an error when the user tries to do a full charge-off when there is a charge amortisation in progress. During charge-off, the system calculates the penalty interest if this has been configured and this helps the bank to access the real charge-off amount for all the property. Illustration of Charge-off Consider a loan that has few bills outstanding and is delinquent. Perform a charge-off. The charged-off arrangement is shown below. The charge-off information in AA.ACCOUNT.DETAILS is as shown below. Arrangement Balances Movement The loan principal balances and billed interest balances are moved to Chargeoff PL and are stored in CO and CUST balances as off-balance sheet items. Here, the sum is: ACCPRINCIPALINTCO=ACCPRINCIPALINTCUST+DELPRINCIPALINTCUST CURACCOUNTCO=DELACCOUNTCUST+CURACCOUNTCUST Bills A bill that was already generated is also updated with the charge-off information. In a full charge-off, the BNK balances for the Property after charge-off is zero. The billed amount and outstanding balance here represents the CUST balance, as shown below Interest Accruals After a charge-off, the interest accruals are under CUST and CO balances. Charge Bills Charge-Off An arrangement with interest and charge bills is being fully charged off, including all interest and charges in the bills along with outstanding principal. Any Activity Charge, Periodic Charge and Rule break charge are also charged off. This is subject to certain evaluation: The system evaluates if there are any pay charges outstanding and raises an error to indicate that the same must be settled. The system evaluates if there is charge collected that is undergoing amortisation, then the system doesn’t allow to charge off that arrangement. Consider an arrangement that has been charged off. During a charge-off, charge bills are also charged off. A rule break that is being charged off is shown below. The balances after the charge-off, also reflects the charges being charged off. Accounting for Charges in Charge-off RE.CONSOL.SPEC.ENTRY is generated during the charge-off of the principal decrease fee, a rule break fee. For charge-off books it is as shown below. For customer books it is as shown below. Activity Charge for charge-off books is shown below. Activity Charge for customer books is shown below The charge-off entries for the charge debited in the banks PL are as follows: For the Rule break fee: For the Activity Charge: Charge-off of Upfront Profit Contracts It is possible to setup upfront profit in loan arrangements. For such a loan, the interest is collected upfront and is booked to the PL over a period as accruals. Read Islamic Finance-Upfront Sale for more information. The below arrangement has upfront bills with outstanding bills. This arrangement has a profit amount of 10,000 USD that is collected for a year’s tenure. The upfront profit is booked between RECDEFERREDPFT and ACCDEFERREDPFT at the time of booking the arrangement. DR RECDEFERREDPFT -10,000 CR ACCDEFERREDPFT 10,000 During accruals, the profit is booked between ACCDEFERREDPFT and PL DR ACCDEFERREDPFT -48.84 CR PL 48.84 The accruals for the month are -1513.79 and the balance in ACCDEFERREDPFT is 8486.21 at the end of month. On the due date of the profit, the accruals of the month are posted to the RECDEFERREDPFT from DUEDEFERREDPFT DR DUEDEFERREDPFT -1513.79 CR RECDEFERREDPFT 1513.79 As a result of this, RECDEFERREDPFT has a balance of -8486.21 Time Head Movement Balances Creation RECDEFERREDPFT -10,000 -10,000 Creation ACCDEFERREDPFT 10,000 10,000 Monthly Accrual ACCDEFERREDPFT -1513.79 8486.21 Due date RECDEFERREDPFT 1513.79 8486.21 Illustration of Charge-off Upfront Profit The arrangement is now charged off. The balances from CURACCOUNT have moved to CURACCOUNTCO. A part of the principal amount is billed already. So CURACCOUNTCUST+DELACCOUNTCUST amounts to the total principal. The bill is in delinquent status from the customer perspective and the balance is stored in DELDEFERREDPFTCUST as -1513.79. The RECDEFFEREDPFTCUST gives the outstanding amount as per customer, -8,486.21 that is pending receivable. There are four days accrual after the last bill date for 180.38 that has resulted in the ACCDEFERREDPFTCUST is 8305.83 (8,486.21-180.38). Time Head Movement Balances Creation RECDEFERREDPFT -10,000 -10,000 Creation ACCDEFERREDPFT 10,000 10,000 Monthly Accrual ACCDEFERREDPFT -1513.79 8486.21 Due date RECDEFERREDPFT 1513.79 8486.21 4 days accruals after due date ACCDEFERREDPFT -180.37 8305.83 Repayment in the Charge-Off Loan A repayment received in the upfront profit loan arrangement is allocated as per the payment rule given below. The balances of the same loan arrangement after a couple of days are; Time Head Movement Balances Creation RECDEFERREDPFT -10,000 -10,000 Creation ACCDEFERREDPFT 10,000 10,000 Monthly Accrual ACCDEFERREDPFT -1513.79 8486.21 Due date RECDEFERREDPFT 1513.79 8486.21 6 days accruals after due date ACCDEFERREDPFT -270.56 8215.64 The same update is in the AA.INTEREST.ACCRUALS as shown below. A payment of 5000 on the arrangement and this is apportioned against the CUST and CO balances as per the Payment Rules and Chargeoff Rules respectively. In customer perspective, the Payment Rules apportions the payment towards to DEFFEREDPFT first and then the ACCOUNT Property as seen below. The same is reflected in arrangement balances as shown below. In charge-off perspective, the repayment works as explained below. The Charge-off condition governs the repayment rule for charge off balances. The Charge-off condition for the upfront profit loan is given below. In this arrangement, the loan is fully charged off. So the Billed and Current Balance Type options do not have any impact and the system apportions the payment for the CHARGEOFF balance type. Thus, the full payment of 5000 is apportioned to the ACCOUNT balance. This can be seen in the screenshot below. In banks’ books repayment is as explained below. The repayment is received in the banks’ book against the CHARGEOFF PL as indicated in Accounting Condition. The repayment of 5000 is credited to the PL indicated in this accounting condition as seen below. Charge-off in Charge Component - Upfront Profit Contract In the contract below, a charge booked at the time of arrangement creation is shown. The impact on the charge bill during a charge-off is shown in the subsequent screenshots The arrangement balances before a charge-off are shown below. The arrangement balances after charge-off as shown below. A comparison of the bill details before and after the charge-off is shown below: The accounting entries in charge-off are as follows: The charge-off entry in the PL, is a debit to the banks PL as seen in CATEG.ENTRY . The charge-off entries to bank and customer books are as RE.CONSOL.SPEC.ENTRY . In the charge-off books, the CO entry is as shown below. In the customer books, the CUST entry is as shown below.

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

When a loan contract in TBC is charged-off, the TBC generates an event, which can be captured by the connected external GL (General Ledger) system to complete the accounting and balance updates.


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

The features related to handling charge-off under FASB regulations are not applicable for loans in TBC.


> **Related Applications:** `AA.ACCOUNT.DETAILS`, `AA.ACTIVITY.HISTORY`, `AA.BILL.DETAILS`, `AA.INTEREST.ACCRUALS`, `CATEG.ENTRY`, `RE.CONSOL.SPEC.ENTRY`

---


### 1.39  Charges


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

The accounting related features and processing are handled by an external GL system for loans in TBC. Therefore, to complete the accounting related to charges (such as for suspension, accrual and amortisation of charges and so on), the TBC generates an event, which can be captured by the connected external GL (General Ledger) system.


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

The accounting related features and processing are handled by an external GL system for loans in TBC. Therefore, to complete the accounting related to charges (such as for suspension, accrual and amortisation of charges and so on), the TBC generates an event, which can be captured by the connected external GL (General Ledger) system.


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

The accounting related features and processing are handled by an external GL system for loans in TBC. Therefore, to complete the accounting related to charges (such as for suspension, accrual and amortisation of charges and so on), the TBC generates an event, which can be captured by the connected external GL (General Ledger) system.


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

The accounting related features and processing are handled by an external GL system for loans in TBC. Therefore, to complete the accounting related to charges (such as for suspension, accrual and amortisation of charges and so on), the TBC generates an event, which can be captured by the connected external GL (General Ledger) system.


##### Preferential Pricing

The below screenshot displays the New Arrangement Fee waived off because the arrangement has been created as a Valued Customer.

It is possible to define pricing benefits (that is, preferential pricing) for certain loan contracts based on factors such as customer age, rating, channel and so on. The user can define preferential pricing for loans in TBC and teh system can evaluate at the enterprise layer, that is TEP (Temenos Enterprise Pricing).


##### Rebate Processing

The below screenshot displays the rebate processing.

For some loan products, the customers protect their loan commitment with the help of insurance covers against risks such as death and disability. The insurance policy can be for the entire loan term or particular period such as yearly and then it is renewed at the end of every period. Rebate processing provides a facility to rebate the outstanding amount of premium for loan insurance on pre-closure or on cancellation at a later stage or cancellation within a certain grace period.

The aim of the rebate processing feature is, to render the ability to use a local routine for certain types of amortisation calculation. However, in AA, the generic accrual processing mechanism allows the user to amortise or accrue fixed amounts supplied by applications through a direct API or accounting entries. The standard method of processing is to straight line the amount on a daily basis.

It is possible to post to an internal account category (instead of PL) in the Accounting version.

The user can define the start date of accrual calculation. From that day, the accrual and account postings begin. On the first day, the calculation is based on the beginning of the accrual period – Start Date in the EB.ACCRUAL record. The changes to the grace period is considered only if the record is reversed, and if the record is reversed, no accounting activity takes place.

This feature provides an option to rebate the outstanding amount of premium for loan insurance on pre-closure or on cancellation at a later stage or cancellation within a certain grace period.

Home loan insurance, or any mortgage redemption insurance plan, is part of a banker's sales pitch when extending sizable long-term credit, such as a home loan. These plans hedge the risk of loss in case the borrower dies or becomes disabled during the loan term, especially an unsecured loan. The banks fund the insurance portion as part of the loan amount, which is repaid by the customers as part of the loan. The insurance policy can be done for the entire loan term or particular period.

The solution deals with the option to define the grace period, rebate on cancellation of an insurance contract and insurance rebate on pre-closure of a loan.

The accounting related features and processing are handled by an external GL system for loans in TBC. Therefore, to complete the accounting related to charges (such as for suspension, accrual and amortisation of charges and so on), the TBC generates an event, which can be captured by the connected external GL (General Ledger) system.


##### Pre-Closure and Dues Settlement

The below arrangement has a start date of 18 Apr with cooling date set as 23 Apr. As the customer opted not to proceed with the loan, the user closes the arrangement before the cooling date and the system displays the error message that the dues are not settled. Unless the dues are either settled or waived, the system does not allow the user to close the arrangement.


##### Tax on Charges

It is possible to levy a tax on charge if necessary. The below screenshot displays the Tax on Charges.


##### Pre-Closure of a Loan and Rebate Processing

An arrangement is created with Insurance Property as shown in the below screenshot.

The charge percentage is negotiable at arrangement level to add or less value based on the customer’s credibility.


> **Related Applications:** `EB.ACCRUAL`

---


### 1.40  LendingRule78


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

In TBC, there are no specific limitations for defining loan contracts with the Rule of 78 method for interest calculation.

---


### 1.41  Limit Facility for Loan


> **📇 Quick Reference Card**
> 
> **Purpose:** *The sanctioned limit is the total exposure that the bank can take on a particular client for facilities offered by the bank. Such limits are recorded using the Limit Property Class in arrangements.*
> 
> **Key Fields:** *Limit Id*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

The sanctioned limit is the total exposure that the bank can take on a particular client for facilities offered by the bank. Such limits are recorded using the Limit Property Class in arrangements.

In Lending TBC, the limit sanctioned for a loan can be updated by providing the limit key (from the external limit solution) in the Limit Id attribute of the Limit Condition. Other features pertaining to Limits are not applicable for Lending TBC. Read Introduction to Loan Limit for more information on loan limits in TBC.

---


### 1.42  Loan Commitment


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

Whenever a pre-closure within the cooling period is processed for a loan, the system generates an event, which can be captured by an external accounting system for accounting and bookkeeping purposes.

The Loan Cancellation functionality allows a loan to be automatically cancelled if the commitment amount is not fully availed by the customer in the stipulated time period. The stipulated time is defined as the number of days under Term Amount Property Class.

The system schedules the LENDING-CANCEL-ARRANGEMENT Activity, which triggers the cancellation if the loan is not fully disbursed by that cancel period.

The banks can configure a pre-advice to be sent to the customer to indicate the cancellation that would come up due to the pending disbursement. The pre-advice configuration is achieved through the Activity Messaging Property which has associated multi-value attributes, such as Pre Notice Activity and Pre Notice Days . The Pre Notice Activity attribute has to be LENDING-CANCEL-ARRANGEMENT and Pre Notice Days attribute controls the time in advance when the notification has to be sent.

In the TBC, instead of sending the notification or advice, the system generates an event which should be consumed by an external system for further processing.

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


### 1.43  Migration of LendingArrangements


> **📇 Quick Reference Card**
> 
> **Applications:** `AA.ACTIVITY.CLASS`, `AA.ARRANGEMENT.ACTIVITY`, `AA.CONTEXT TYPE`, `ACCOUNT`, `CUSTOMER`, `EB.CASHFLOW`, `LIMIT`, `PERIODIC.RATE`
> 
> **Key Fields:** *AMC*, *Activity*, *Arrangement*, *Context Name*, *Context Value*, *Context name*, *Currency*, *Customer* ... +26 more
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

In TBC, during migration of a loan contract, the information related to owners and other parties can be input from an external system such as Party TBC. The system evaluates this customer information against the records found in the external system.

For each customer in a loan arrangement, a corresponding LIMIT record is created in our system before creating the arrangement.

In TBC, during the takeover of a loan, the user can update the sanctioned limit amount for the loan using the Limit Id field in the Limit condition.

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

In TBC, the loan contracts are migrated to products which are designed and defined using a product management system like the TPM (Temenos Product Manager).

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

- It is possible to configure the reporting condition to hand off the required information to an external system for calculating the annual percentage rate for loans in TBC. The TBC generates a business event to hand off the cashflows to an external system for further processing to take place. All other features related to Reporting condition are not applicable for TBC.
- The features pertaining to EIR as well as AMC are not applicable for loans in TBC and can be enabled using external solutions.

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


### 1.44  Payment Holiday


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

There are no specific limitations to define payment holidays for loans in TBC.


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

To complete the accounting related to balance updates for holiday interest, the TBC generates an event, which can be captured by the connected external GL (General Ledger) system.


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

The feature related to printing the results of payment holiday simulations is not applicable for loans in TBC.


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

In TBC, when the user defines payment holiday for a loan contract, the TBC generates a business event for updating the cashflows and no accounting takes place for the same in TBC.


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


### 1.45  Scheduling Payments


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

It is possible to configure the reporting condition to hand off the required information to an external system for calculating the annual percentage rate for loans in TBC. The TBC generates a business event to hand off the cashflows to an external system and no further processing takes place.


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

- In TBC, it is possible to notify the customer in advance about an upcoming payment in the loan. The system generates an event to notify the customer in advance about the scheduled instalment. Notifications to the customer based on events in the loan must be handled through external delivery subsystem.
- The billed amount for loan contracts in TBC can be settled as follows upon reaching the finalisation date: Capitalised to the same loan account or Forwarded as a settlement request by publishing an event to an account or beneficiary outside the TBC.


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

In the following example, payments are skipped on 6th, 7th, 9th and 11th month. However, the system projects the schedule for the arrangement by adjusting the skipped installment amounts for the rest of the payment period using its calculation logic. The below screen shot displays the AA.PRD.DES.PAYMENT.SCHEDULE record. The below screen shot displays the Enquiry schedule projection Disbursement Linked Payments When a loan product has to collect principal (down) payments along with disbursement, it can be set-up using the DISBURSEMENT relative date option and a TRANSACTION based Payment type. The consumer loan product in model bank illustrates this set-up where a downpayment of 25% is collected for each disbursement and the rest of the payments are collected on 30, 60 & 90th day. Case 1: Downpayment with Automatic Full Disbursement An arrangement is created for USD 1000 and is fully disbursed (automatically) The disbursement fee is calculated on each disbursement and is capitalised. 20% for loans upto 500 16% for loans above 500 but less than1000 8% for loans above 1000 25% of the disbursed amount plus the charge is collected as downpayment and is billed online. The net CUR account movement is 1160 25% of the movement ,that is, 290 is calculated as a payment bill and is raised along with this disbursement. Differences in TBC The features related to automatic disbursement are not applicable for loans in TBC. Case 2: Downpayment with Partial Disbursement An arrangement created for USD 5000 The disbursement fee is calculated on each disbursement and is capitalised. 20% for loans upto 500 16% for loans above 500 but less than1000 8% for loans above 1000 25% of the disbursed amount plus the charge is collected as downpayment and is billed online. The disbursements are done manually First Disbursement for 3000 Net movement in CUR balance is 3,240 25% of the movement, that is, 810 is calculated as a payment bill and is raised along with this disbursement. Second and final disbursement for 2000 New movement in CUR balance is 2160 25% of the movement, that is, 540 is calculated as a payment bill and is raised along with the second disbursement.


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

The accounting related features and processing are handled by an external GL system for loans in TBC. Therefore, to complete the accounting related to deferred payments, the TBC generates an event, which can be captured by the connected external GL (General Ledger) system.


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


### 1.46  Weighted Average Rate


> **📇 Quick Reference Card**
> 
> **Purpose:** *When loans are being disbursed in multiple tranches, each having its own interest rate a Weighted Average Rate (WAR) for the arrangement has to be calculated and applied to the contract after each disbursement .*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

When loans are being disbursed in multiple tranches, each having its own interest rate a Weighted Average Rate (WAR) for the arrangement has to be calculated and applied to the contract after each disbursement .

A weighted average interest rate is an average that is adjusted to reflect the contribution of each loan to the total debt. The weighted average multiplies each loan’s disbursement interest rate by the loan balance and divides the sum by the total loan balance. Each loan’s disbursement interest rate contributes to the weighted average in proportion to the loan’s percentage of the total debt.

The Weighted Average Rate Type of Interest condition enables the calculation of the weighted average rate, which determines the actual effective rate of the arrangement.

There are no specific limitations with regards to calculating and processing of weighted average rates for loans in TBC. It is not possible to automatically disburse the commitment amount for loans in TBC.

---


### 1.47  Misc


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


## Chapter 2: Deposits - FD


Deposits - FD module of Temenos Transact


### Features in Deposits - FD


| # | Feature | Sections |
|---|---------|----------|
| 2.1 | Fiduciaries Workflow | Intro, Confi, Worki, Tasks, Outpu |
| 2.2 | Misc | Intro |


### 2.1  Fiduciaries Workflow


> **📇 Quick Reference Card**
> 
> **Purpose:** *Fiduciary (FD) deposits are deposits placed by customers with other banks through their banker who acts as an agent bank. The customer can choose from a wide range of deposit offerings without opening an account with the bank where they wish to place the deposit. The customer can choose an external ...*
> 
> **Applications:** `CUSTOMER`, `FD.ACTIVITY`, `FD.ADVICES`, `FD.FIDUCIARY`, `FD.FIDUCIARY/FD.PARAMETER`, `FD.PARAMETER`, `PAYMENT.ORDER`, `PAYMENT.ORDER.PRODUCT` ... +1 more
> 
> **Key Fields:** *Accrual Fqu*, *Accrual Min Amt*, *Accrue Amort*, *Acct Trans PO*, *Acct With Bank Bic*, *Acct With Bank Customer*, *Acct With Bank Name*, *Amount* ... +100 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Fiduciary (FD) deposits are deposits placed by customers with other banks through their banker who acts as an agent bank. The customer can choose from a wide range of deposit offerings without opening an account with the bank where they wish to place the deposit. The customer can choose an external bank and deposit (whose terms and conditions are known) or can allow their bank to negotiate the best terms with any external bank.

The agent bank can pool multiple deposits together and negotiate better terms. The agent bank debits the amount from their customer’s account and places the same with the external bank. This feature describes the FD deposit workflow in Temenos Transact where the Temenos Transact bank is acting as the Agent bank.


#### ⚙️ Configuration

This is covered as part of the Fiduciaries Parameters feature.


#### 🔧 Working With

This topic details the workflow of the FD module in Temenos Transact .


##### FD.FID.ORDER

This is the first main application used when dealing with customers placing Fiduciary Deposits. Basically, this application records the request from the customers and places a deposit on their behalf until it is authorised and the corresponding FD.FIDUCIARY is made. No accounting or commissions are calculated or posted at the time of receiving the order.

The basic deposit types are:

1. Fixed
2. Call or Notice
3. One-off contracts
4. Automatically renewable Principal only Principal plus income Rounded amounts Principal plus income plus current account balance in value date The smallest between the 2nd and 3rd option The smallest between the 1st and 3rd option

A sub-type is defined optionally, distinguishing deposits placed with external institutions (OUT) from deposits done inside the group (IN), where the placement bank belongs to the same group as the customers bank. The notion of CD is also introduced, allowing the placement of funds inside the group without requiring the signature of the fiduciary mandate. It is also possible to accrue or amortise charges mentioned in the Charge Type field in FD.FID.ORDER application for the FIXED type of orders.

The list of FD.FID.ORDER is shown below.

To enable this functionality, the FT.COMMISSION.TYPE record updated in Charge Type field should have values in the following fields.

The Accrue Amort field can either be A for Accrual or M for Amortisation. If it is set to A, then charges are accrued till the charge date. If this field is set to M, then the charges are amortised. The accrual or amortisation frequency is decided by the value in the Accrual Fqu field.

On authorisation of FD.FIDUCIARY , a record is generated in the internal file EB.ACCRUAL with relevant details. Entries are passed for accruals during COB. If the amount of the charge to be accrued or amortised is less than the amount mentioned in the Accrual Min Amt field, then no accrual process takes place (there is no EB.ACCRUAL record). In this case, the charges are posted directly to Profit and Loss (P&L).

When a fixed fiduciary order is entered with a term, the system checks if there is a record in FD.GROUP.PAYMENT corresponding to the bank, currency, term and if so:

- The system automatically defaults the Interest Rate and Interest Day Basis from the FD.GROUP.PAYMENT application.
- The Val Date Offset is checked from the record in FD.GROUP.PAYMENT . If this field is blank, then the system uses the value defined in the Val Date Offset field in FD.PARAMETER . If the date is not set, then the system uses the Days Delivery field in CURRENCY application and defaults the value date.
- The Holiday Calendar is checked from the record in FD.GROUP.PAYMENT . If the Holiday Calendar field is blank, the system uses the value defined in the Holiday Calendar field in FD.PARAMETER to calculate the interest dates and maturity date for the fixed term deposits.

> **⚠️ Note:** For fixed fiduciary contracts, the interest rate applicable as on the value date of the order is fixed for the entire period. The interest rate does not change.

The withholding tax is calculated based on the tax code defined in the Withholding Tax Code field in FD.FID.ORDER . The tax code applicable for the respective group defined in TAX.TYPE.CONDITION is defaulted in FD.PARAMETER .

The value in Withholding Tax Amt field is calculated based on the tax code in the Withholding Tax Code field.


##### Pooling of Orders

Every FD.FID.ORDER is added to a group or pool. A group can have just one order or orders can continue to be pooled into the group until it is closed. This depends on the value in Pooling field in FD.FID.ORDER . When there is no value in the field, the order is placed in a separate group and placed as a single order. By default, the orders that have same currency, value date and maturity date are pooled together. If additional fields need to be checked for pooling, the same can be specified in the Pooling Fields field in FD.PARAMETER application. The FD.POOL.GROUP application holds the orders from FD.FID.ORDER with common attributes in separate Pools for investment. The records will initially be Open and will then be move to closed.

The fiduciary orders can be grouped automatically by setting the Pooling field in FD.FID.ORDER to Auto. Temenos Transact will place the order in a pool that matches its currency and maturity date and is open. If the pool with the fiduciary details cannot be found or they are closed, a new record is setup. Alternatively, if the Pooling field in FD.FID.ORDER is set to manual, then they can be manually added to a group. An open pool group becomes closed when all the deals stored in it become approved. After this, deals cannot be added to the group.

When the pool is closed, system creates a new record to the hold table of FD.FIDUCIARY corresponding to the closed group.


##### Approving Orders for Investment

Each order has to be approved for investment. When order is placed individually, that is, there are no values in the pooling related field and there is only one order in the group, then approving the order is easy. However, when multiple orders are pooled together and several pooled groups exists, the selection of the fiduciary orders that are to be approved and placed may be very tedious for the dealer as each order must be processed individually. To reduce the number of manipulations, a facility allows to process several transactions in one shot. The dealer can list the orders to be processed using an enquiry. As these orders have already been pooled into a group, the dealer has to approve the group. The drop-down allows a dealer to:

- Edit one of the orders in the group or
- Approve and close the whole group or
- Select the placement option for closing and initiating the placement.

Sometimes the dealer has to change the group allocated to one or several orders. The transfer of several orders from one group to another can be done by selecting the orders to be moved and globally allocating them a new group number. This can be achieved by using the FD.APPROVE.POOLING - Approve Pooled Orders (Fixed) and FD.APPROVE.POOLING.NOTICE - Approve Pooled Orders (Notice) enquiries. Both the enquiries are used with the L function. An illustration of how to approve all the orders of a group and close it is explained in the below screenshots. Select an order of a group and choose the Close group option in the drop-down menu.

Another way to close a group is described below.

- Select the orders and choose them using the drop-down menu.
- Select the Placement option in the drop-down menu.

The corresponding record in FD.FIDUCIARY is shown below screenshot.


##### FIDUCIARY PLACEMENTS

The FD.FIDUCIARY is the second main application which is used for the far end of the fiduciary agreement and in placing the fiduciaries with foreign institutions or external banks. The account officer uses FD.FID.ORDER and the dealers use FD.FIDUCIARY to invest the funds. When orders are approved and a pool is closed, the system automatically creates a record in FD.FIDUCIARY in IHLD status for the total amount of the pool. The reason for placing them in HOLD status is that at this stage the FD.FIDUCIARY records are not complete and cannot be validated.

The bank where the deposit is to be placed and the interest rate needs to be entered. For notice contracts, the interest rate is picked up from a record in FD.GROUP.PAYMENT .After the dealer enters the details of the bank or institution where funds are to be placed, the record is authorised. Accounting is done at this stage. Each customer’s account is debited for the deposit amount committed by them and the total amount is credited to the external bank nostro account.

| Field Name | Description |
|---|---|
| ID | Indicates the record ID of FD.FIDUCIARY |
| Fid Bank | Displays the value in the Fid Bank field in FD.FIDUCIARY application |
| Fid Bank Ref | Holds the reference as provided by the Fiduciary bank |
| Order ID | Holds the FD.FID.ORDER ID |
| Interest Rate | Defaults from FD.FIDUCIARY application |
| Interest Frequency | Defaults from FD.FIDUCIARY application |
| Sys Int Date | Automatically calculated by the system based on the frequency set up in FD.FIDUCIARY |
| Sys Interest Amt -XX | Indicates the system calculated interest amount for the same period |
| Sys Wht Tax –XX | Defaults the value from Sys Wht Tax Amt in FD.FID.ORDER |
| Fid Bank Int Date -XX | Allows to input the interest date as provided by the Fiduciary bank. It helps to reconcile between Temenos Transact date and Fiduciary bank date |
| Fid Bank Int Amt -XX | Defaults to the value in Interest Amt field |
| Fid Bank Wht Tax -XX | Defaults to system calculated tax amount and can be changed |
| XX | Defaults to Sys Interest Amt but can be changed. This is to input the interest amount as provided by the Fiduciary bank which helps to reconcile between Temenos Transact interest amount and Fiduciary bank interest amount. A change up to one round unit (example, USD 1) is allowed. This will be the interest amount updated in FD.FIDUCIARY . |
| Total Interest | Indicates the total of the Interest Amt fields |
| Maturity Date | Indicates the maturity date of the Fiduciary. If early maturity is accepted, then this field is updated with early maturity date. |
| Maturity Amt | Holds the principal amount on maturity. If early maturity is accepted, this field is updated with the early maturity amount. |
| Mat Amt Recd Date | Indicates when the maturity amount or early maturity amount was actually received from the Fiduciary bank. |

| Field Name | Description |
|---|---|
| Acct Trans PO | Flag that decides whether to process counterparty payment through the PAYMENT.ORDER application or not. The possible values are: Yes - Signifies that a PO is generated and MT202 is triggered from PO . NULL - MT202 is generated directly from Fiduciary. |
| Po Product | Holds a valid record of PAYMENT.ORDER.PRODUCT . |
| Po Susp Categ | Holds a valid category account. It is the wash category used while generating entries related to external payments. |


##### Renewal of Fixed Fiduciary Contracts

Fixed fiduciaries run between two predefined dates and once the dates are set, it cannot be modified. Due to the rigid nature, a fixed fiduciary can have renewal options to be set. This can be done with or without income and can have the frequency set to run automatically. The frequency is defined in FD.FID.ORDER by the Renewal Type , Renewal Amt and Round Renewal fields. The selection of the fiduciary contracts to be renewed may be very tedious, as each order must be processed individually. In order to reduce the number of manipulations, a facility allows the processing of several transactions in one attempt. With this facility, the renewals processing is divided into three steps:

1. Preparation of the renewal options The preparation phase allows the account officer to select the fiduciary orders to be renewed according to his own defined criteria. Further, eventually it allows the defining by grouping of orders and the characteristics of the renewals. These options are stored in the FD.PREPARE.RENEWALS application until their approval.
2. Approval of the renewal options The approval phase consists of the transfer of the prepared renewal options from the FD.PREPARE.RENEWALS application to the FD.FID.ORDER application. This transfer may be done either in one attempt or for (one or) several orders.
3. Generation of the renewed orders This phase consists of a background process (FD.PROCESS.RENEWALS) used to generate the renewed orders with a status depending on both the values of the Renewal Type field in FD.FID.ORDER and the presence of overrides or not.

On a certain number of days, as defined within the Renew Rpt Days field (renewal days) in FD.PARAMETER , prior to the maturity of fiduciary fixed orders the account officers have the ability to prepare their renewal options ( Renewal Type , Renewal Amt and Round Renewal fields ) using the FD.PREPARE.RENEWALS application. This information is stored in the FD.PREPARE.RENEWALS application with an authorised status. Once the account officer is satisfied with the renewal options defined, then they can be validated either in one attempt or in several steps by using the FD.PREPARE.RENEWALS APPROVE enquiry. Then, the renewal information is moved from the FD.PREPARE.RENEWALS application from where they are archived and deleted in the FD.FID.ORDER application.

The account officer can display the list of orders that may potentially be renewed by using the Prepare Renewals (FD.PREPARE.RENEWALS) enquiry with the L function.

If the account officer wants to apply the same criteria to the last five orders, the orders can be selected and picked with the button or by the context menu. The below screenshot illustrates selecting an order using the context menu.

The Prepare Renewals (FD.PREPARE.RENEWALS) enquiry showing selected records is illustrated below.

The FD.PREPARE.RENEWALS input screen appears.

Only the first order of the selection is displayed. The criteria are changed as follows and the selection is accepted:

- In the Renewal Type field, set the value to SEMI.

- In the Renewal Amt field, set the value to NET.

- In the Round Renewal field, set the value to Y.

An override message is displayed as shown in the below screenshot.

After confirmation, the enquiry is refreshed and the result is listed as shown in the below screenshot.

All data with a star are recorded in the FD.PREPARE.RENEWALS application and are waiting for approval. The approval step can be achieved using the FD.PREPARE.RENEWALS APPROVE enquiry with L function.

Selecting an order and validating it with the Approve Renewal Order option selected from the context menu can approve the renewal of an order.

Selecting orders, whose renewal is to be approved, and picking them using the context menu can achieve the same result.

Select the Pick Item option from the context menu.

The following screen is displayed.

Commit the selection and the following message is displayed for validation in one shot of all the selected orders.

Then, the orders are updated in the FD.FID.ORDER application and deleted from the FD.PREPARE.RENEWALS application.

A customer can request to close a fixed fiduciary deposit, before the maturity date. The anticipated reimbursement is processed as a normal reimbursement with an earlier maturity date with optional penalties to be paid by the customer. Anticipating a reimbursement is only possible for deposits whose pool group is made of a single order. The penalty commission is used to compensate the unit paying the interest. It is calculated in the form of either a reduction of the initial interest rate (deposit outside the group) or a commission charged to the customer (deposit within the group). This penalty commission may be automatically calculated by the system or input in the form of either a percentage to apply on the principal amount of the deposit or a flat amount. It is not subject to Value Added Tax (VAT) because it is considered as an interest reduction. It is deducted from the amount reimbursed to the customer and from the amount to reimburse by the unit paying the interest.

The penalty fees are used to compensate the customer unit. They may be automatically calculated by the system or input in the form of either a percentage to apply on the principal amount of the deposit or a flat amount. They are subject to VAT according to the current rules for fees and commissions. They are deducted from the amount reimbursed to the customer and credited to an internal account.

An anticipated reimbursement is activated using the Early Mat Dt field in FD.FID.ORDER . Once a date is entered in this field, a default value is applied from FD.GROUP.CONDITION to the Penal Commission Type (penalty commission code) and the Charge Type (penalty charge code) fields in FD.FID.ORDER . Furthermore, the Charge Date and Charge Event fields are populated with the maturity date and the value as Maturity, if a default penalty Charge Type exists (defined in FD.GROUP.CONDITION with a Charge Event set to EARLYMAT). The user can then change the default values and manually input the penalty commissions and charges. After commitment, the system:

- Calculates the penalty commission amounts ( Default Penal Commission Amount and Penal Commission Amount fields, if the values are not yet populated).
- Calculates the penalty charge amounts ( Def Chg Amt and Charge Amount if not yet populated), together with the associated tax on these charges.
- Refreshes the usual commissions taken in arrears according to the new duration of the contract (together with their associated taxes).

Then, the early maturity can either be cancelled by removing the date previously entered in the Early Mat Dt field or accepted by setting the Early Status field in FD.FIDUCIARY to ACCEPTED, hence reducing the interest rate by means of the Early Interest Rate field in FD.FIDUCIARY . Accounting entries are not raised while the early maturity is not accepted in FD.FIDUCIARY. Accepting the early maturity in FD.FIDUCIARY results in the following actions:

- Updating the maturity date from the new one
- Adjusting the interest amount
- Updating the schedules
- Updating FD.BALANCES
- Updating the FD.ORDER.MATURITY application used for renewals
- Deleting the old forward entries
- Creating new forward entries
- Updating limits and collaterals
- Updating the FD.ORDER.CUST application
- Updating the pooling group in the FD.POOL.GROUP application

A call or notice fiduciary has a start date (VALUE.DATE) but end date is not available. The deal is terminated using a notice period by which the customer must notify the account officer with whom they wish to terminate the deal.

Orders which have Pooling Status field set to None can be reimbursed by setting a Reimburse Date. Once the record is authorised, the Reimburse Status field is marked as REQUESTED. The request is manually communicated to the Fiduciary bank and once it is accepted, the dealer has to open the record in FD.FIDUCIARY and mark the Reimburse Status field to ACCEPTED. Once accepted, the system will mature the order and credits the funds to the customer.

Notice deposits in a pool can also be reimbursed at any time. For orders which have been pooled either manually or automatically, the Reimburse Date field is a no input field and the REIMBURSE REQ field must be used in conjunction with the principal change fields in order to reimburse the order. When this field is set to YES and the placement hits an interest settlement date, the order is reimbursed and removed from the placement. To reimburse the order prior to the next interest settlement date, a principal change should be entered which reduces the principal to zero with a value date of the required reimbursement. This field must be set to YES. This action repays the principal as of the value date set in the principal change fields, but the interest is paid only at the interest settlement date, at which point the order will be fully reimbursed.

If at this stage the placement contract ( FD.FIDUCIARY ) has a principal of zero (that is, any orders are not contributing to the placement), the placement is then reimbursed.

A call or notice fiduciary can also have some of its details changed midterm, such as the amount invested, the value date of the fiduciary and so on. Renewal options are not available for call or notice fiduciaries.


##### Confirmations

The FD module supports the confirmations on two levels. Firstly, it enables the sending out of confirmations and for confirmations to be accepted from external banks or brokers, if necessary. Once a deal is placed, a record is raised on either FD.UNCONF.BROKER or FD.UNCONF.CUSTOMER . These records are LIVE files with only a key in the record. Once the confirmation is received, the relevant deal is verified (using the Verify function) and the record on the relevant unconfirmed record is removed. A deal can skip the entire confirmation stage by not setting either Confirmation by Broker or Confirm by Counterparty depending on whether the deal goes through a broker or straight to a bank. The lists of deals unconfirmed from either fiduciary banks or brokers are available using enquiries or through the menu system.

The FD module supports the confirmations by the customer placing the order and by banks that have accepted the placement. There is no functional relevance on the system and a deal can live its entire life span without ever being confirmed.


##### Deal Slips

Deal slips can be generated for both the orders (when taken) and the placements (when effected) or at other stages required by the user. Refer the Version section in System Administration Guide for more information on the creation and setting of deal slips.


##### Services

The following are the services in the FD module.

This process completes the authorisation process of any partially authorised placements and orders. A fixed placement can be partially authorised when a system recovery has been run. Some of the linked orders may be authorised, whilst others remain unauthorised together with the placement.

If an error is made in entering the customer details on an order that forms part of a placement, this process adjusts the order details as follows. A new order is created with the same amount, currency, value date and maturity but with different customer details. The existing order is reversed together with all accounting and limit details. Then the correct accounting and limit updates are raised to the replacing order.

This routine runs before the schedule processing and is driven by the FD.GROUP.TODAY table that holds the IDs of the FD.GROUP.PAYMENT records that are to be changed during the day. All placements linked to the FD.GROUP.PAYMENT records are processed to regenerate the next set of schedules for those contracts. The placement contracts are obtained by selecting the FD.GROUP.PLACEMENT application.

This process moves the matured contracts to the HISTORY table. The FD.PARAMETER application defines the number of days post maturity at which this happens.

This process handles scheduled events such as maturity, principal or rate changes, interest payments and all associated delivery. Commission taken in arrears are processed at this point.

This process handles changes resulting from a change at customer or contract level to a component of the consolidation key. Refer the Reporting User Guide for more information on how these are constructed. Refer the Application Accounting User Guide for a more explanation of Temenos Transact consolidated accounts.

This process accrues interest and commissions at a frequency defined by the user on the FD.PARAMETER application. The accounting entries are not raised as a result. The figures are produced solely for the purpose of portfolio valuations.

This process runs monthly at the COB and updates the records in FD.CUST.VALUE.


##### Accounting

The accounting entries are generated at various stages throughout the life cycle of the contract. These are all contingent as the deposit and placement are off- balance sheet items for the bank.

| Column 1 | Column 2 | Column 3 |
|---|---|---|
| Dr | Drawdown A/C | (Principal) |
| Cr | Principal Liquidation A/C | (Principal) |
| Dr | Commission Liquidation A/C | (Commission) |
| Cr | Interest Liquidation A/C | (Interest) |

| Forward Valued Order |  |  |
|---|---|---|
| Cr | CRF type FWDCONTCR | (Principal) |
| Forward Valued Placement |  |  |
| Dr | CRF type FWDCONTDB | (Principal) |

| Drawdown Order |  |  |
|---|---|---|
| Dr | Drawdown A/C | (Principal) |
| Cr | CRF type CONTCR | (Principal) |
| Commission in Advance |  |  |
| Dr | Commission Liquidation A/C | (Commission) |
| Cr | P&L PL Accr Comm | (Commission) |
| Note: PL Accr Comm is a user-defined category on FD.PARAMETER . |  |  |
| Drawdown Placement |  |  |
| Dr | CRF type CONTDB | (Principal) |
| Cr | Drawdown A/C | (Principal) |

| Order |  |  |
|---|---|---|
| Dr | CRF type PL Accr Comm | (Accrued commission) |
| Cr | P&L PL Accr Comm | (Accrued commission) |

| Commission received in advance |  |  |
|---|---|---|
| Dr | Client Account |  |
| Cr | Deferred Fiduciary Commission Income |  |

| Daily accrual of commission receivable |  |  |
|---|---|---|
| Dr | Income Receivable - Fiduciary Commission |  |
| Cr | Fiduciary Commission Income |  |
| Reversal of previous period-to-date commission accrual |  |  |
| Dr | Fiduciary Commission Income |  |
| Cr | Income Receivable – Fiduciary Commission |  |
| Current period-to-date accrual of fiduciary commission receivable under In-out method |  |  |
| Dr | Income Receivable – Fiduciary Commission |  |
| Cr | Fiduciary Commission Income |  |
| Daily amortisation of fiduciary commission |  |  |
| Dr | Deferred Fiduciary Commission Income |  |
| Cr | Fiduciary Commission Income |  |
| Reversal of previous period-to-date commission amortised |  |  |
| Dr | Fiduciary Commission Income |  |
| Cr | Deferred Fiduciary Commission Income |  |
| Current period-to-date amortisation of fiduciary commission income under In-out method |  |  |
| Dr | Deferred Fiduciary Commission Income |  |
| Cr | Fiduciary Commission Income |  |

| Order |  |  |
|---|---|---|
| Cr | Interest Liquidation A/C | (Interest) |
| Commission in Arrears on Interest |  |  |
| Dr | Commission Liquidation A/C | (Commission) |
| Cr | CRF type PL Accr Comm | (Commission) |
| Placement |  |  |
| Dr | Interest Liquidation A/C | (Interest) |

| Order |  |  |
|---|---|---|
| Dr | CRF type CONTCR | (Principal) |
| Cr | Principal Liquidation A/C | (Principal) |
| Commission in Arrears |  |  |
| Dr | Commission Liquidation A/C | (Commission) |
| Cr | CRF type CONTDB | (Commission) |
| Placement |  |  |
| Dr | Principal Liquidation A/C | (Principal) |
| Cr | CRF type CONTDB | (Principal) |

There are certain scenarios where the banks may face a delay in receiving the funds from the Fiduciary bank and in such cases the banks do not want to credit the amount to the customer’s account before the actual receipt. Also, some banks does a cash matching before crediting funds to the customers.

In such cases, the system posts the amount to the Int Acc Categ field in FD.PARAMETER as on the interest payment date for all fiduciary orders that have a record in FD.SCHEDULE.DEFINE application. Then based on the date set in Fid Bank Int Date field in FD.SCHEDULE.DEFINE , the system reverses the entry from the Int Acc Categ field and credits to the actual customer’s account. The process of crediting customer account on actual receipt of amount holds for Maturity date processing.


#### 📋 Tasks

Related topics:

- Renew Fiduciary Orders
- Initiate Fiduciary Order
- Amend or Approve Pooled Orders
- Place Fiduciary
- Fiduciary Processes
- Amend/Approve Pooled Orders
- Place Fiduciary

Fiduciary Deposit or Contract is an investment by the bank in the form of deposit with another bank. Such investment is done under the name of the bank but for the benefit of the customer as the beneficial owner. With fiduciary deposits, the customer can enjoy higher returns and greater tax advantages in comparison with the normal bank deposits.

Fiduciary Deposits application is used to take deposit orders from clients and place them individually or in groups with foreign institutions that may be either external or a member of the same group as the deposit unit. A small handling commission is charged and as there is no liability for either the deposit or placement they are recorded as below the line on the bank’s general ledger.


##### Workflow

This section allows the user to perform the below tasks:

This screen allows the user to create a fixed fiduciary order.

1. Input a Fixed Fid Order .
2. In the FD Fixed Order screen, enter values in the following fields: Client Currency Amount Maturity Date
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon.

This screen allows the user to create a notice fiduciary order.

1. Input a Notice Fid Order .
2. In the FD Notice Orders screen, enter values in the following fields: Client Currency Amount Notice Days
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon.

| SCREENS | WORKFLOW |
|---|---|
|  | Amend Fixed Fid Order . |
| List of Fixed Orders that have been Placed | Click the Amend icon of a corresponding record. |
| Amend Fixed FDs | Enter values in the fields that needs to be updated. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Amend Notice Fid Order . |
| List of Notice Orders that have been Placed | Click the Amend icon of a corresponding record. |
| Amend Notice FD Orders | Enter values in the fields that needs to be updated. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Approve/Edit Pooled Orders (Fixed) . |
| Approve Pooling Individually/Edit Pooled Order (Fixed) | Click the Edit Order icon of a corresponding record. |
| FD Fixed Order | Enter values in the fields that require amendment. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Approve/Edit Pooled Orders (Notice) . |
| Approve Pooling Individually/Edit Pooled Order (Notice) | Click the Edit Order icon of a corresponding record. |
| FD Notice Orders | Enter values in the fields that require amendment. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Input Fiduciary Placement . |
| List of Deposits to be Placed | Select the Fixed Placement option corresponding to a record and then click the Launch icon. |
| Fixed Plmt | Enter values in the following fields: Fiduciary Bk Interest Rate In the Settlement Details tab, select a value in the Fid Bk Corres field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

This enquiry enables the user to modify the fiduciary placements available in the core banking system. The user can modify interest rate for Fixed contracts and interest payment date for Notice contracts along with settlement details, if any.

To amend a fixed placement record, follow the below steps:

1. Amend Fixed/Notice Placements .
2. Click the Amend Fixed icon.
3. Enter values in the fields that require amendment.
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon.

| SCREENS | WORKFLOW |
|---|---|
|  | Replaceable Orders . |
| List of FD Orders | Enter values in the required fields and then click the FIND button. |
| List of Fiduciary Orders | Click the Replace icon. |
| FD Orders | Enter values in the below fields: Replace Order No Fid Type Client Currency Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Replaced Orders . |
| List of FD Orders | Enter values in the required fields and then click the FIND button. |
| List of Replaced Fiduciary Orders | Click the View Old icon. The system displays the record in view mode. |
| FD Orders | Verify the record details. |

| SCREENS | WORKFLOW |
|---|---|
|  | Approve/Reject Amendments . |
| List of Amended FDs | Enter values in the required fields and then click the FIND button. |
| List of Amendments to Order | Click the Amend icon. |
| Approve Amendments to Notice FD / Approve Amendments to Fixed FDs | Enter values in the fields that require amendment. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Early Maturity FD Orders . |
| List of FD Orders | Enter values in the required fields and then click the FIND button. |
| List of Fiduciary Orders | Click the View Order icon. |
| FD Orders | Verify the record details. |

| SCREENS | WORKFLOW |
|---|---|
|  | Renew Individual Order . |
| Renew Individual Order | Click the Input Renewal icon of a corresponding record. |
| Renewal | Enter values in the fields that needs to be updated. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

This fast path enquiry enables the user to enter the renewal details for the list of fixed fiduciary orders available in the core banking system.

1. Prepare Bulk Renewals .
2. Select the required order and enter the necessary renewal details.
3. Amend the values in the below fields, if required. Renewal Type Renewal Amt Round renewal?
4. Click the Apply the chosen operation to the selected row(s) icon.

| SCREENS | WORKFLOW |
|---|---|
|  | Complete Renewed Orders . |
| Renewed Fiduciary Orders to complete | Click the Complete icon of a corresponding record. |
| FD Fixed Order | Enter values in the fields that require amendment. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

This enquiry displays the interest payment schedule of fixed Term Deposits till the maturity.

To view an Interest record, follow the below steps:

1. Interest Schedule for Fixed Fiduciary .
2. Click the View Schedule icon of a corresponding record.

To amend the interest details, follow the below steps:

1. Interest Schedule for Fixed Fiduciary .
2. Click the Modify icon of a corresponding record.
3. Enter values in the following fields: FID Bank Int Date FID Bank WHT Tax Interest Amt Maturity Amt Recd Date
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon.

To view the fiduciary record, perform the following steps:

1. Interest Schedule for Fixed Fiduciary .
2. Click the View Fiduciary icon of a corresponding record.

This enquiry displays the list of modified fixed term deposits schedule with respect to Interest or Maturity payment date and amount.

To view the modified interest record, follow the below steps:

1. Authorise Interest Schedule for Fixed Fiduciary .
2. Click the View Schedule icon of a corresponding record.

To authorise the modified interest record, follow the below steps:

1. Authorise Interest Schedule for Fixed Fiduciary .
2. Click the Authorise Schedule icon of a corresponding record.
3. Click the Authorise icon to authorise the record.

This screen holds details such as, upcoming interest settlement date and the interest rates applicable for all notice contracts of a given currency and notice period with a particular fiduciary bank.

1. Input Interest Defaults .
2. Enter values in the following fields: GB Description Current Int Rate
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon.

This screen enables the user to create a record for each customer dealing with fiduciaries.

The key to this file must be a valid record on the CUSTOMER application.

1. Input Customer Defaults .
2. Enter values in the following fields: Mandate Held Preferred Ccy.1 Pref Bank.1.1 Fiduciary Type.1
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon.

This screen enables the user to define the list of depositories by deposit type and currency.

This file is used by the FD.FIDUCIARY application to define whether the placement updated by the dealer requires additional checks from back office or not.

1. Input Placements Defaults .
2. Enter values in the following fields: Currency Stnd Bank.1.1 Auth Req.1.1
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon.


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to fiduciary contracts in the core banking system.


##### Enquiries and Reports

This section allows the user to view the below enquiries and reports:

List of Fid Orders

This enquiry displays the list of fiduciary orders available in the core banking system.

List of Fid Placements

This enquiry displays the list of fiduciary placements available in the core banking system.

Interest Details

This enquiry displays the interest details of the fiduciary orders and placements available in core banking system.

List of Renewed Orders

This enquiry displays the list of renewed fiduciary orders available in the core banking system.

Records due for Renewal

This enquiry displays the list of fiduciary orders pending for renewal in the core banking system.

Renewal Report

This is a close of business report, which displays the list of fiduciaries pending for renewal.


##### SWIFT Messages

The user can view the below swift messages, enquiries and reports while processing Fiduciaries Workflow.

Message MT320 is sent to confirm a fixed fiduciary placement contract.

It is generated while entering a new fixed placement contract. Upon amendment, cancellation and maturity of the fixed deal the same message is addressed to the fiduciary bank of the deal.

Message MT330 is sent to confirm a call or notice fiduciary placement contract.

It is generated while entering a new call or notice placement contract. Upon amendment, the same message is addressed to the fiduciary bank of the deal.


##### Advices

The below list of advices are generated by the core banking system pertaining to Fiduciaries Workflow.

When a fixed fiduciary order is entered, system generates a deal slip for the same.


##### Alerts

NA


> **Related Applications:** `CUSTOMER`, `FD.ACTIVITY`, `FD.ADVICES`, `FD.FIDUCIARY`, `FD.FIDUCIARY/FD.PARAMETER`, `FD.PARAMETER`, `PAYMENT.ORDER`, `PAYMENT.ORDER.PRODUCT`, `PP.COMPANY.PROPERTIES`

---


### 2.2  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *Fiduciary deposits take deposit orders from customers and place them individually or in groups with foreign institutions that may be either external or a member of the same group as the deposit unit. This feature discusses the various parameter setting necessary to place a fiduciary order.*
> 
> **Key Fields:** *Accr Cycle Comm*, *Accr Cycle Int*, *Acct Trans PO*, *Application*, *Auto Chg Rate*, *Broker Cat*, *Days Prior Conf*, *Ex Asset Type* ... +18 more
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- APIs
- Temenos Transact Services

Fiduciary deposits take deposit orders from customers and place them individually or in groups with foreign institutions that may be either external or a member of the same group as the deposit unit. This feature discusses the various parameter setting necessary to place a fiduciary order.


##### Product Configuration

The initial applications populated are listed below.

- FD.PARAMETER
- FD.ACTIVITY
- FD.ADVICES
- FD.CHARGE.PARAMETER
- FD.COMMISSION.TYPE
- FD.CUST.DETAILS
- FD.FID.CURRENCY
- FD.TXN.CODES
- FD.MATURITY.DATES
- FD.PLACEMENT.PROFILE
- FD.BANK.DETAILS
- FD.STANDARD.PERIODS
- FD.RATE.DEVIATION

Fiduciaries use the CUSTOMER.CHARGE application for amending charges by customer or by group. Therefore, the following application must be setup:

| Files | Records |
|---|---|
| CONDITION.PRIORITY | Record FIDUCIARY |
| FD.GEN.CONDITION | Default record 099 must be defined (user – defined record). |
| FD.GROUP.CONDITION | Default record 099 must be defined (for fiduciary type, fixed or notice) (user-defined record). |

Once these are defined, the user must run (from within Temenos Transact ) the INSTALL.FID.CUST.CHARGES program to update the CUSTOMER.CHARGE records. For automatic ID generation, the two main application to be setup in the COMPANY application are FD.FID.ORDER and FD.FIDUCIARY .

The user must add or create an AUTO.ID.START record to initialise the first ID by setting the Application field to FDOR and the Id Start field to display as FDOR9935600001 for FD.FID.ORDER . For FD.FIDUCIARY these must be FD and display as FD9935500001 respectively.

The above two applications must be added to the CONSOLIDATE.COND file to include in the general ledger.

This FD.ACTIVITY application is used to specify internal activities of the life cycle of fiduciaries and give a language description for system enrichment purposes. The records must be in place before instigating any deals.

This application creates an interface for a fiduciary activity either to the delivery system or to a deal slip. The key is made of two parts, two letters and a three-figure number. The first of the two letters specifies the fiduciary type (fixed or notice) and the second whether the deal is at the placement or order stage (P or O). The three-figure number is a ID on the FD.ACTIVITY application. This means that for each activity the user can issue one of four separate advices dependent on stage and type. Instead of giving a Message Type and Print Format , the user can give the key to another record on FD.ADVICES and it uses the Message Type and Print Format from that record.

For each deal category or for fixed or notice deals, the commission charge settings can be set in FD.CHARGE.PARAMETER . Commission can be taken in advance or arrears based on either the principal interest or income.

When entering an order from a customer, the commission basis can be specified in FD.COMMISSION.TYPE . Standard and specific types can be defined. The charging of tax and the basis for the commission are defined here. The following calculation types are defined as:

- Flat - implies the same commission rate irrespective of the amount.
- Level - flat rate depending on which level the amount falls.
- Band - implies a level, except that the charge is on a climbing scale (for example, 0.5% for first 100,000, then 0.3% for next 400,000 and 0.2% after that).

It also specifies whether commission type calculates against the amount deposited in the fiduciary or the customer's overall business with the bank.

A record for each customer dealing with Fiduciaries must be created on FD.CUST.DETAILS application The ID of this application must be a valid record on the CUSTOMER application. Each customer of the bank has specific needs with regard to deposits placed on their behalf.

Banks that they trust can be specified as those they do not wish to be used. Limits are set on how much can be placed with specific institutions. Specific rate category, margin on interest, interest calculation method and rounding type may be defined by fiduciary type or category.

It is likely that the treasury department does not make placements with other institutions for small or odd currency amounts. The FD.FID.CURRENCY application provides a means of restricting orders to minimum amounts (defined by fiduciary type or category and tenor for fixed orders or tenor event for notice orders) and for amounts above that minimum for which the multiples can be placed (defined by fiduciary type or category and ranges of amounts). An override is generated if a non -standard amount is inputted.

Rather than hard coding the transaction codes that are used for events within the Fiduciary Deposits (FD) module, the SYSTEM record on FD.TXN.CODES allows the user to specify which transaction codes are used for which event. This application has only one record called SYSTEM and cannot be modified once it is created .

The FD.CUST.VALUE is a LIVE file that holds the last calculated value of the total assets or liabilities for each fiduciary customer. It is updated monthly in the COB routine FD.EOD.UPDATE.CUST.VALUE.

In order to group a maximum of orders with the same maturity date and to generate bigger volume, standard maturity days can be defined by year or month and currency (individually for only a set of specific currencies, or for all currencies except some special ones for which specific dates are set).

When a frequency (like, 1M, 3M and 6M) is used to enter in the maturity of a contract, the system calculates the resulting date by taking into account the holidays in the country related to the deal currency.

It then compares this date with the dates stored in the corresponding record of FD.MATURITY.DATES (these dates may have to be converted to working dates) and chooses one according to the adjustment rules defined in the Matdates field of FD.PARAMETER application.

The back-office process around a fiduciary placement consists of checking and eventually changing the settlement instructions proposed by the system. As there are only small risks involved by a Fiduciary deposit and as most of the Fiduciary deals are always placed with the same depositories, they often need not be checked.

It is possible to list depositories, defined by deposit type and currency, for which no additional check is required by the back-office once the dealer has approved the placement.

The ID of this FD.BANK.DETAILS application must be a valid bank recorded on the CUSTOMER application. Each fiduciary bank may have specific practices such as interest calculation method with regard to deposits placed with them.

The FD.STANDARD.PERIODS application allows the user to record, by company and upper limit of tenor (in number of days), the tenor code (TERM) of a renewed deposit for the calculation of its maturity date.

The FD.RATE.DEVIATION application allows the user to record the rate fluctuations (up and down) over which an automatic interest rate change may be applied to notice contracts done inside the group.

When dealing in placements that are at call or have a defined notice period, there must be agreed dates when interest is to be settled. Banks usually have pre-defined arrangements for each type stating at what interval interest is settled. Temenos Transact also needs to be advised of changes to the rates that affect call or notice placements made with external banks. This is catered in the FD.GROUP.PAYMENT table where the rates and interest details of the banks can be stored and updated.

Banks may need to maintain a record of a range of fixed term deposits which are offered by different institutions. The FD.GROUP.PAYMENT application allows to enter the details of fixed term deposits. The ID of the record is in the BANK.CURRENCY.TERM format, where TERM is the term of a deposit. The term can be days, weeks or months.

100461.USD.12M

100461.USD.12D

100461.GBP.3W

If the ID has a term, then Days Prior Conf and Auto Chg Rate fields are no-input fields. The Int Day Basis field holds a valid interest day basis supported by the FD module. The Holiday Calendar field accepts any calendar including region value (example, US00) and Val Date Offset is used to arrive at the value date of a record in FD.FID.ORDER .

This is a live concat file in which each record only contains a key. It is used to associate groups and placement banks with the corresponding FD.FID.ORDER deals that are placed there. The ID is made up of four parts separated by dots. The first part is the placement bank, the second is the currency, the third is the number of days and the fourth is the FD.FID.ORDER number.

The data is held this way (opposed to a key and a list of multi-valued keys to FD.FID.ORDER ) as it is quicker and this application is generally used in time critical COB processing.

Similar to the FD.GROUP.PLACEMENT application, this is a live concat file with each record containing only a key. The ID is similar to FD.GROUP.PLACEMENT except that there is no fourth part where the Deal number is. This application is used to list all the banks whose FD.GROUP.PAYMENT records have changed. Once the details in the FD.FID.ORDER and FD.FIDUCIARY are updated, the record is deleted.


##### Illustrating Model Parameters

The model parameters for Fiduciary Deposits are explained below:

| Field | Description |
|---|---|
| Fiduciary Type | Indicated type of fiduciary contract that is allowed (Fixed or Notice). |
| Margin Rate | Indicates the default margin rate associated with the Fiduciary Type . |
| Accr Cycle Int | Defines the date and frequency for the next accrual of interest. Frequency can be either DAILY or MONTHLY. |
| Accr Cycle Comm | Defines the date and frequency for the next commission accrual. Frequency can be either DAILY or MONTHLY. |
| Pl Accr Comm | Indicates the profit and loss category used for posting commission accruals for fixed fiduciary orders. |
| Int Diff Cat | Indicates the category code of the internal account to be used for posting any difference entry between the placement interest and order interest. |
| Broker Cat | Indicates the profit and loss category to be debited when brokerage is payable. |
| Renewal Days | Defines the number of days prior to maturity of the existing order, when the renewed order is to be created. It can be defined as 1-99 “C/W”, calendar or working days before the maturity of the existing order. |
| Ex Asset Type | Indicates the asset types to be excluded for customer valuation. |
| Ex Sub Ass Type | Indicates the sub asset types to be excluded for customer valuation. |
| Placement Profile | Defines whether the FD.PLACEMENT.PROFILE must be used to allocate or check the bank of placement within fiduciary transaction. |
| Holiday Calendar | Calculates Interest and Maturity dates for Fixed Term Deposits. |
| Value Date Offset | Offset is used to arrive at the value date of the Fiduciary Order. |
| Interest Schedule | Defines whether the interest payment schedule is required to generate for Fixed Fiduciary contracts. |
| Int Acct Categ | Indicates the account used to post funds from fiduciary (Interest / Maturity Amount) until the actual fund is received from the fiduciary bank. |
| Acct Trans PO | Flag that decides whether to process counterparty payment through the PAYMENT.ORDER application or not. The possible values are: Yes - Signifies that a PO is generated and MT202 is triggered from PO . NULL - MT202 is generated directly from Fiduciary. |
| Po Product | Holds a valid record of PAYMENT.ORDER.PRODUCT . |
| Po Susp Categ | Holds a valid category account. It is the wash category used while generating entries related to external payments. |

This application is used to define the default charge details used for calculating the commission amount payable by the customer on a fiduciary order. The parameters can be defined at the level of the category, code of the order, or the order type (Fixed /Notice).

This application is used to define the depositories for which no back-office intervention is required by deposit type and currency. This file is used by the program FD.FIDUCIARY to define whether the placement updated by the dealer requires additional checks from the back-office or not. In other terms, depending on whether the depository used for the placement is defined in the FD.PLACEMENT.PROFILE application or not, the status of the record in FD.FIDUCIARY is either live or unauthorised.


##### Illustrating Model Products

Model products are not applicable for this module.

---


---


## Appendix A: Glossary of T24 Applications & Fields


This glossary lists all T24/Transact application names and field names referenced throughout this document, with descriptions where available.


### Applications


| Application | Description |
|------------|-------------|
| `AA.ACCOUNT.DETAILS` | T24 application: AA.ACCOUNT.DETAILS |
| `AA.ACCRUAL.FREQUENCY` | T24 application: AA.ACCRUAL.FREQUENCY |
| `AA.ACTION` | T24 application: AA.ACTION |
| `AA.ACTIVITY` | T24 application: AA.ACTIVITY |
| `AA.ACTIVITY.CLASS` | T24 application: AA.ACTIVITY.CLASS |
| `AA.ACTIVITY.HISTORY` | T24 application: AA.ACTIVITY.HISTORY |
| `AA.ACTIVITY.HISTORY.SIM` | T24 application: AA.ACTIVITY.HISTORY.SIM |
| `AA.ARR.` | T24 application: AA.ARR. |
| `AA.ARR.` | T24 application: AA.ARR. |
| `AA.ARR.` | T24 application: AA.ARR. |
| `AA.ARR.CUSTOMER` | T24 application: AA.ARR.CUSTOMER |
| `AA.ARR.INTEREST` | T24 application: AA.ARR.INTEREST |
| `AA.ARR.OFFICER` | T24 application: AA.ARR.OFFICER |
| `AA.ARR.PAYMENT.SCHEDULE` | T24 application: AA.ARR.PAYMENT.SCHEDULE |
| `AA.ARR.TERM.AMOUNT` | T24 application: AA.ARR.TERM.AMOUNT |
| `AA.ARRANGEMENT` | T24 application: AA.ARRANGEMENT |
| `AA.ARRANGEMENT.ACTIVITY` | T24 application: AA.ARRANGEMENT.ACTIVITY |
| `AA.ARRANGEMENT.SIM` | T24 application: AA.ARRANGEMENT.SIM |
| `AA.BILL.DETAILS` | T24 application: AA.BILL.DETAILS |
| `AA.BILL.TYPE` | T24 application: AA.BILL.TYPE |
| `AA.CHARGE.DETAILS` | T24 application: AA.CHARGE.DETAILS |
| `AA.CONTEXT TYPE` | T24 application: AA.CONTEXT TYPE |
| `AA.CUSTOMER.ARRANGEMENT` | T24 application: AA.CUSTOMER.ARRANGEMENT |
| `AA.CUSTOMER.ARRANGEMENT.HIST` | T24 application: AA.CUSTOMER.ARRANGEMENT.HIST |
| `AA.CUSTOMER.ARRANGMENT.HIST` | T24 application: AA.CUSTOMER.ARRANGMENT.HIST |
| `AA.DECISION.PARAMETER` | T24 application: AA.DECISION.PARAMETER |
| `AA.INTEREST.ACCRUAL` | T24 application: AA.INTEREST.ACCRUAL |
| `AA.INTEREST.ACCRUALS` | T24 application: AA.INTEREST.ACCRUALS |
| `AA.INTEREST.DETAILS` | T24 application: AA.INTEREST.DETAILS |
| `AA.NEXT.ACTIVITY` | T24 application: AA.NEXT.ACTIVITY |
| `AA.OVERDUE.STATS` | T24 application: AA.OVERDUE.STATS |
| `AA.PARAMETER` | T24 application: AA.PARAMETER |
| `AA.PAYMENT.RULE.TYPE` | T24 application: AA.PAYMENT.RULE.TYPE |
| `AA.PAYMENT.TYPE` | T24 application: AA.PAYMENT.TYPE |
| `AA.PERIODIC.ATTRIBUTE` | T24 application: AA.PERIODIC.ATTRIBUTE |
| `AA.PRD.DES.PAYMENT.SCHEDULE` | T24 application: AA.PRD.DES.PAYMENT.SCHEDULE |
| `AA.PRODUCT` | T24 application: AA.PRODUCT |
| `AA.PRODUCT.DESIGNER` | T24 application: AA.PRODUCT.DESIGNER |
| `AA.PRODUCT.GROUP` | T24 application: AA.PRODUCT.GROUP |
| `AA.PRODUCT.LINE` | T24 application: AA.PRODUCT.LINE |
| `AA.PROPERTY` | T24 application: AA.PROPERTY |
| `AA.PROPERTY.CLASS` | T24 application: AA.PROPERTY.CLASS |
| `AA.SCEHDULED.ACTIVITY` | T24 application: AA.SCEHDULED.ACTIVITY |
| `AA.SCHEDULED.ACTIVITY` | T24 application: AA.SCHEDULED.ACTIVITY |
| `AA.SIM.CUSTOMER` | T24 application: AA.SIM.CUSTOMER |
| `AA.SIM.INTEREST` | T24 application: AA.SIM.INTEREST |
| `AA.SIMMULATION.RUNNER` | T24 application: AA.SIMMULATION.RUNNER |
| `AA.SIMULATION.CAPTURE` | T24 application: AA.SIMULATION.CAPTURE |
| `AA.SIMULATION.RUNNER` | T24 application: AA.SIMULATION.RUNNER |
| `AA.SIMULATION.SERVICE` | T24 application: AA.SIMULATION.SERVICE |
| `AA.SIMULATION.SERVICE.LIST` | T24 application: AA.SIMULATION.SERVICE.LIST |
| `AC.ALLOCATION.RULE` | T24 application: AC.ALLOCATION.RULE |
| `AC.ALLOCATION.RULES` | T24 application: AC.ALLOCATION.RULES |
| `AC.ENTRY.PARAM` | T24 application: AC.ENTRY.PARAM |
| `AC.EVENT` | T24 application: AC.EVENT |
| `AC.EVENTS` | T24 application: AC.EVENTS |
| `AC.INWARD.ENTRY` | T24 application: AC.INWARD.ENTRY |
| `AC.LOCKED.EVENT` | T24 application: AC.LOCKED.EVENT |
| `AC.LOCKED.EVENTS` | T24 application: AC.LOCKED.EVENTS |
| `AC.POSTING.DETAIL` | T24 application: AC.POSTING.DETAIL |
| `AC.POSTING.DETAILS` | T24 application: AC.POSTING.DETAILS |
| `ACCOUNT` | T24 application: ACCOUNT |
| `ACCOUNT.ACCRUAL` | T24 application: ACCOUNT.ACCRUAL |
| `ACCOUNT.CLOSURE` | T24 application: ACCOUNT.CLOSURE |
| `ACCR.REV.PARAM` | T24 application: ACCR.REV.PARAM |
| `ASSET.TYPE` | T24 application: ASSET.TYPE |
| `BASIC.INTEREST` | T24 application: BASIC.INTEREST |
| `BENEFICIARY` | T24 application: BENEFICIARY |
| `BENEFICIARY.LINKS` | T24 application: BENEFICIARY.LINKS |
| `CATEG.ENTRY` | T24 application: CATEG.ENTRY |
| `CURRENCY` | T24 application: CURRENCY |
| `CUSTOMER` | T24 application: CUSTOMER |
| `CUSTOMER.CHARGE` | T24 application: CUSTOMER.CHARGE |
| `DE.MAPPING` | T24 application: DE.MAPPING |
| `DE.MESSAGE.SETUP` | T24 application: DE.MESSAGE.SETUP |
| `EB.ACCRUAL` | T24 application: EB.ACCRUAL |
| `EB.ADVICES` | T24 application: EB.ADVICES |
| `EB.CASHFLOW` | T24 application: EB.CASHFLOW |
| `EB.CONTRACT` | T24 application: EB.CONTRACT |
| `EB.CONTRACT.BALANCES` | T24 application: EB.CONTRACT.BALANCES |
| `EB.EVENTS` | T24 application: EB.EVENTS |
| `EB.LOOKUP` | T24 application: EB.LOOKUP |
| `EB.SYSTEM.ID` | T24 application: EB.SYSTEM.ID |
| `EXTERNAL.SEPA.DETAILS` | T24 application: EXTERNAL.SEPA.DETAILS |
| `F.SIMULATION.DETAILS` | T24 application: F.SIMULATION.DETAILS |
| `FD.ACTIVITY` | T24 application: FD.ACTIVITY |
| `FD.ADVICES` | T24 application: FD.ADVICES |
| `FD.FIDUCIARY` | T24 application: FD.FIDUCIARY |
| `FD.FIDUCIARY/FD.PARAMETER` | T24 application: FD.FIDUCIARY/FD.PARAMETER |
| `FD.PARAMETER` | T24 application: FD.PARAMETER |
| `FT.COMMISSION.TYPE` | T24 application: FT.COMMISSION.TYPE |
| `GENERIC.ACCOUNTING.REQUEST` | T24 application: GENERIC.ACCOUNTING.REQUEST |
| `LIMIT` | T24 application: LIMIT |
| `LIMIT.REFERENCE` | T24 application: LIMIT.REFERENCE |
| `MS.PARAMETER` | T24 application: MS.PARAMETER |
| `PAYMENT ORDER` | T24 application: PAYMENT ORDER |
| `PAYMENT.ORDER` | T24 application: PAYMENT.ORDER |
| `PAYMENT.ORDER.PARAMETER` | T24 application: PAYMENT.ORDER.PARAMETER |
| `PAYMENT.ORDER.PRODUCT` | T24 application: PAYMENT.ORDER.PRODUCT |
| `PERIODIC.INTEREST` | T24 application: PERIODIC.INTEREST |
| `PERIODIC.RATE` | T24 application: PERIODIC.RATE |
| `PP.COMPANY.PROPERTIES` | T24 application: PP.COMPANY.PROPERTIES |
| `PP.HEAVYWEIGHTPRODUCTCOND` | T24 application: PP.HEAVYWEIGHTPRODUCTCOND |
| `PRINTER.ID` | T24 application: PRINTER.ID |
| `RC.CONTRACT.PRIORITY` | T24 application: RC.CONTRACT.PRIORITY |
| `RE.CONSOL.SPEC.ENTRY` | T24 application: RE.CONSOL.SPEC.ENTRY |
| `REPORT.CONTROL` | T24 application: REPORT.CONTROL |
| `RFR.CONDIITON` | T24 application: RFR.CONDIITON |
| `RFR.CONDITION` | T24 application: RFR.CONDITION |
| `RFR.MIGRATION` | T24 application: RFR.MIGRATION |
| `RFR.MIGRATION.DETAILS` | T24 application: RFR.MIGRATION.DETAILS |
| `SC.POS.ASSET` | T24 application: SC.POS.ASSET |
| `STMT.ENTRY` | T24 application: STMT.ENTRY |
| `SUB.ASSET.TYPE` | T24 application: SUB.ASSET.TYPE |
| `TAX` | T24 application: TAX |
| `TAX.TYPE` | T24 application: TAX.TYPE |
| `TAX.TYPE.CONDITION` | T24 application: TAX.TYPE.CONDITION |
| `TEC.ITEMS` | T24 application: TEC.ITEMS |
| `TRANSACTION` | T24 application: TRANSACTION |
| `TSA.SERVICE` | T24 application: TSA.SERVICE |


### Fields Referenced


| Field | Field | Field |
|-------|-------|-------|
| `A` | `AA Bundle ID` | `AMC` |
| `Aa Product` | `Aa Product Group` | `Account Debit Rule` |
| `Accr Cycle Comm` | `Accr Cycle Int` | `Accrual Fqu` |
| `Accrual Min Amt` | `Accrue Amort` | `Acct Trans PO` |
| `Acct With Bank Bic` | `Acct With Bank Customer` | `Acct With Bank Name` |
| `Active Y/N` | `Activity` | `Activity Link` |
| `Activity Type` | `Actual Amount` | `Actual Amt` |
| `Actual Group` | `Actual Pay Date` | `Adj Int Prop` |
| `Adjust Balance Type` | `Adjust Description` | `Adjust Property` |
| `Adjust Rate` | `Adjustment Amount` | `Admin` |
| `Advance Payment Restriction` | `Advice` | `Aging Status` |
| `Align Dates` | `Allowed Product` | `Alt Acct Id` |
| `Alt Acct Type` | `Alt Id` | `Alt Id Type` |
| `Alt Payment Method` | `Alt Payment Routine` | `Alternate ID` |
| `Alternate Id` | `Alternate Id Type` | `Amortisation Term` |
| `Amount` | `Application` | `Application Field Name` |
| `Application Field Name, Field Operand, and Value From, Value To` | `Application Method` | `Application Name` |
| `Application Order` | `Application Type` | `Apr Type` |
| `Arrangement` | `Arrangement Id` | `Arrangement Status` |
| `Attribute` | `Attribute Type` | `Attribute Value` |
| `Auth Req.1.1` | `Auto Chg Rate` | `Auto Pay Acct` |
| `Auto Run` | `Auto Settle` | `Avail Expiry Date` |
| `Avail Start Date` | `Available Start Date` | `Available Expiry Date` |
| `Available Start Date` | `Back-to-Back FX` | `Back-to-back FX` |
| `Balance Type` | `Bank To Bank` | `Bank to Bank` |
| `Bank to Bank Info` | `Base Ccy Product` | `Base Date Type` |
| `Batch Stage` | `Beneficial Owner` | `Beneficiary` |
| `Beneficiary Customer` | `Beneficiary Name` | `Bill Produced` |
| `Bill ID` | `Bill Produced` | `Bill Status` |
| `Bill Type` | `Broker Cat` | `Bundle Arrangement` |
| `Bus Day Centre` | `Cal Routine` | `Calc Amount` |
| `Calc Type` | `Calculation Routine` | `Calculation Type` |
| `CalculationType` | `Cancel` | `Cancel Date` |
| `Cancel Period` | `Change Period` | `Change Activity` |
| `Change Amount` | `Change Date` | `Change Date Type` |
| `Change Period` | `Change To Product` | `Charge Account` |
| `Charge Amount` | `Charge Date` | `Charge Event` |
| `Charge Off Amount` | `Charge Off Percentage` | `Charge Routine` |
| `Charge Type` | `Charge off Amount` | `Charge off Percentage` |
| `Client` | `Closure Method` | `Closure Notes` |
| `Closure Period` | `Closure Reason` | `Closure Type` |
| `Combine Bill At Parent` | `Commitment Drawdown` | `Commitment Reversal` |
| `Comparison Type` | `Condition by Term` | `Confirm by Counterparty` |
| `Confirmation by Broker` | `Context Name` | `Context Name Value` |
| `Context Tax Code` | `Context Tax Condition` | `Context Value` |
| `Context name` | `Contra Acc` | `Contra Acct Categ` |
| `Contra Cr Txn Code` | `Contra Currency` | `Contra Dr Txn Code` |
| `Contra Entry` | `Cooling Convention` | `Cooling Date` |
| `Cooling Date Adj` | `Cooling Period` | `Cooling Waive Class` |
| `Cooling Waive Prop` | `Counterparty` | `Counterparty Type` |
| `Cr Txn Code` | `Create Retry Trigger` | `Credit Account` |
| `Credit Amount` | `Credit Nostro Account` | `Credit Value Date` |
| `Currency` | `Current Int Rate` | `Cus Bic Code` |
| `Cust Name No` | `Custom Priority Rank` | `Customer` |
| `Customer No` | `Customer ID` | `Customer Rate` |
| `Customer Spread` | `Cut Off Date` | `Cut Off Time` |
| `D` | `Data Item` | `Date Convention` |
| `Days Delivery` | `Days Prior Conf` | `Debit Amount` |
| `Debit Book Code` | `Debit Currency` | `Debit Value Date` |
| `Def Account` | `Def Chg Amt` | `Def Prev Settle` |
| `Default Attr Option` | `Default Ol Accrual` | `Default Penal Commission Amount` |
| `Default RFR PI Key` | `Default Spread` | `Defer Date` |
| `Defer Period` | `Delivery Days` | `Denomination Details` |
| `Dr Txn Code` | `Draw down acc` | `Due Frequency` |
| `Due Rule` | `Due Type` | `EIR` |
| `Early Interest Rate` | `Early Mat Dt` | `Early Status` |
| `Effective Date` | `Emit Business Event` | `End Date` |
| `Entry Delim` | `Event Type` | `Ex Asset Type` |
| `Ex Sub Ass Type` | `Exclude Application Field` | `Exclude Field Operand` |
| `Exclude Field Operation` | `Exclude Flag’` | `Exclude Value From` |
| `Exclude Value To` | `Exclusion Flag` | `Execute Simulation` |
| `Expiry Date` | `Expiry date` | `Extend Cycle` |
| `External Posting` | `F` | `FID Bank Int Date` |
| `FID Bank WHT Tax` | `Fid Bank` | `Fid Bank Corr` |
| `Fid Bank Int Amt` | `Fid Bank Int Date` | `Fid Bank Ref` |
| `Fid Bank Wht Tax` | `Fid Bk Corr Add` | `Fid Bk Corres` |
| `Fid Type` | `Fiduciary Bk` | `Fiduciary Type` |
| `Fiduciary Type.1` | `Field Delim` | `Field Name 1.1` |
| `Field Name 1.2` | `Field Name 1.3` | `Field Name 1.4` |
| `Field Name 1.5` | `Field Name 1.6` | `Field Name.1.1` |
| `Field Name.1.2` | `Field Name.1.3` | `Field Name.1.4` |
| `Field Name.1.5` | `Field Name.1.6` | `Field Operand` |
| `Field Operation` | `Field Value 1.1` | `Field Value 1.2` |
| `Field Value 1.3` | `Field Value 1.4` | `Field Value 1.5` |
| `Field Value 1.6` | `Field Value From` | `Field Value To` |
| `Field Value.1.1` | `Field Value.1.2` | `Field Value.1.3` |
| `Field Value.1.4` | `Field Value.1.5` | `Field Value.1.6` |
| `Finalise Bills` | `Finalise Bills` | `Financial Date` |
| `Fixed` | `Flat Charge` | `Frequency` |
| `Full Chargeoff` | `Full Commitment Activity` | `Full Description` |
| `Fwd Acct Mode` | `GB Closure Notes` | `GB Description` |
| `GB Narrative` | `Generate Iban` | `Group Bill Type` |
| `Group Min Amount` | `Group Min Property` | `Hol Restrict Item` |
| `Hol Restrict Type` | `Holiday Amt` | `Holiday Calendar` |
| `IBOR Cut Off Date` | `ID` | `Id Start` |
| `In Adv` | `Inadv` | `Include Future Disb` |
| `Int Acc Categ` | `Int Acct Categ` | `Int Comp Acct` |
| `Int Day Basis` | `Int Diff Cat` | `Int Liqu Acct` |
| `Int Period End Date` | `Int period end date.` | `Interest Amt` |
| `Interest Day Basis` | `Interest Frequency` | `Interest Liqu Acct` |
| `Interest Rate` | `Interest Schedule` | `Interface Type` |
| `Intermed Addr` | `Intermed Bank Customer` | `Internal Booking` |
| `Internal Limit` | `LCY Amount` | `Last Activity Date` |
| `Legacy War Rate` | `Limit Id` | `Link AC Number` |
| `Link Account` | `Linked Ac Number` | `Linked Account Number` |
| `Linked Appl` | `Linked Appl Id` | `Loc Cap Chk Rtn` |
| `Loc Processor` | `Loc post process` | `Loc pre process` |
| `Loc prioritise` | `Loc processor` | `Lookback Type` |
| `Mandate Held` | `Mandatory` | `Mapping Key` |
| `Margin Operand` | `Margin Rate` | `Master Arrangement` |
| `Master Live Date` | `Mat Amt Recd Date` | `Mat Date Convention` |
| `Matdates` | `Maturity Amt` | `Maturity Amt Recd Date` |
| `Maturity Date` | `Max Percentage` | `Maximum Amt.1` |
| `Maximum Term Cap` | `Message Type` | `Method` |
| `Migration Status` | `Min. Tfr Cr 1` | `Min. Tfr Dr 1’` |
| `Minimum Amt.1` | `Minimum Payment Type` | `Mode` |
| `Modify/Cancel Payment Holidays` | `Name` | `Narrative` |
| `New Balance Amount` | `New Payment Amount` | `New Property Amount` |
| `No Activity Indicator` | `Notice Account` | `Notice Amount` |
| `Notice Availability` | `Notice Convention` | `Notice Days` |
| `Notice Period` | `Notice Reason` | `Notice Reference` |
| `Notice Type` | `Nr Value` | `Nr Value Source` |
| `Number of Installments` | `Number of Instalments` | `Number of Payments` |
| `On Activity` | `On Activity, Recalculate` | `Online Retry Attempts` |
| `Optional` | `Or Prop Amt` | `Or Prop Amt Bnk` |
| `Order Date` | `Order Delivery` | `Order ID` |
| `Order Initiation Type` | `Order Initiation Type` | `Orig Contract Date` |
| `Orig Contract Date` | `Original Contract Date` | `Original Property Amount` |
| `Os Prop Amt` | `Os Prop Amt Bnk` | `Parent Account` |
| `Pay Freq` | `Payin Account` | `Payment` |
| `Payment Category` | `Payment Connection Method` | `Payment Date` |
| `Payment Execution Date` | `Payment Freq` | `Payment Method` |
| `Payment Mode` | `Payment Order Product` | `Payment Purpose` |
| `Payment Type` | `Payment amount` | `Payment type` |
| `Payout Account` | `Payout Beneficiary` | `Payout Po Product` |
| `Payout Ppty Class` | `Payout Property` | `Payout Settlement` |
| `Penal Commission Amount` | `Penal Commission Type` | `Percentage` |
| `Period End Date` | `Period Type` | `Period Type, Notice Amount` |
| `Periodic Index` | `Periodic Interest` | `Periodic Interest Key` |
| `Periodic Type` | `Periodic Value` | `Pl Accr Comm` |
| `Placement Profile` | `Po Product` | `Po Reference` |
| `Po Susp Categ` | `Pool Sweep` | `Pooling` |
| `Pooling Fields` | `Portfolio ID` | `Portfolio Id` |
| `Portfolio No.` | `Post process` | `Posting Restrict` |
| `Posting Restriction` | `Pr Value` | `Pre Cob Check` |
| `Pre Notice Activity` | `Pre Notice Days` | `Pre processor` |
| `Pref Bank.1.1` | `Pref Prod` | `Pref Product` |
| `Preferred Ccy.1` | `Prev Settle` | `Primary Officer` |
| `Prin Change/Order Amt` | `Principal` | `Principal Chg amount` |
| `Print Format` | `Prioritise` | `Priority Execution` |
| `Priority Rank Type` | `Processing Date` | `Processor` |
| `Prod Cat End` | `Prod Cat Start` | `Prod Prop Ol Accrual` |
| `Product` | `Product Only` | `Prog Pay Perc` |
| `Prop Ol Accrual` | `Prop Tax Code` | `Prop Tax Cond` |
| `Prop Tax Context` | `Property` | `Property 1` |
| `Property Class` | `Property Ol Accrual` | `Property.1` |
| `Proportional Calc` | `RFR` | `RFR Delta Spread` |
| `RFR Flooring` | `RFR Int Property` | `RFR PI Key` |
| `RFR PI key` | `RFR Spread` | `RFR Spread Treatment` |
| `Rank Based Priority` | `Rate` | `Rc Condition` |
| `Rc Type` | `Reason` | `Recalculate` |
| `Recalculate Method` | `Recalculation` | `Receiver Bic` |
| `Reconstruct Settlement` | `Record Id` | `Record Type` |
| `Redemption Date` | `Refer Settlement` | `Refer Settlement Type` |
| `Reimburse Date` | `Remainder Activity` | `Renew Rpt Days` |
| `Renewal Amt` | `Renewal Days` | `Renewal Type` |
| `Repay Period` | `Repay Type` | `Repay type` |
| `Replace Order No` | `Request Code` | `Request Payment Holiday` |
| `Request Payment Holidays` | `Request Type Sub Type` | `Reserve Funds` |
| `Residual Amount` | `Retry Attempts` | `Retry Fqu` |
| `Retry Options` | `Retry Period` | `Revolving` |
| `Rfr Calc Method` | `Rfr Convention` | `Rfr Spread Treatment` |
| `Role` | `Rollover` | `Round Renewal` |
| `Round Renewal fields` | `Round renewal?` | `Routine Name` |
| `Rule End` | `Rule Start` | `Rule Start Date` |
| `Rule.1` | `Run Activity` | `STMT` |
| `SWFMXEffectiveDate` | `Schedule Type` | `Settle Status` |
| `Settlement A/c` | `Settlement Type` | `Sim Currency` |
| `Sim Date` | `Sim End Date` | `Sim Reference` |
| `Sim Run Date` | `Start Date` | `Start date` |
| `StartDt Option` | `Status` | `Stmt` |
| `Stnd Bank.1.1` | `Susp Appln` | `Susp Class Cr` |
| `Susp Class Dr` | `Susp End Date` | `Susp Start Date` |
| `Sweep Cancel Date` | `Swift Ref` | `Sys Bill Type` |
| `Sys Int Date` | `Sys Interest Amt` | `Sys Wht Tax` |
| `System Id` | `Takeover Npv` | `Takeover method` |
| `Tax Code Tax Condition` | `Tax Context` | `Tax Inclusive` |
| `Term` | `Term Amount` | `Term Tol Days` |
| `Term Type` | `Term Variation` | `Tot Due Amt` |
| `Tot Neg Accr Amt` | `Total Due` | `Total Due Amnt` |
| `Total Interest` | `Trans Activity` | `Trans Payment Type` |
| `Trans Source Type` | `Transaction Code` | `Treasury Rate` |
| `Txn Code` | `Txn Type` | `Type` |
| `Up to Amount.1` | `Update Commit On Capitalisation` | `Update Commit on Capitalisation` |
| `Update Prod Condition` | `Update Utilised Commitment` | `Update Utilised Commitment` |
| `V` | `Val Date Offset` | `Validate Counter Party` |
| `Value` | `Value Date` | `Value Date Offset` |
| `Value Date/Change Date` | `Value Dtd Acctng Y/N` | `Value From` |
| `Value To` | `Version Name` | `Waive Bill Type` |
| `Waive Class` | `Waive Class, Waive Prop and Waive Bill Type` | `Waive Prop` |
| `Warehouse Reqd` | `Withdrawal Amount` | `Withdrawal Date` |
| `Withholding Tax Amt` | `Withholding Tax Code` | `alue` |
| `dd` | `etail` | `iter` |
| `t` | `xx` | `xx` |
| `Field.Value` |  |  |


---


## Appendix B: Consolidated Field Reference


This appendix consolidates all field description tables from across the documentation, grouped by sub-module. This provides a single reference for all field definitions.


### Deposits - AD (AD)


**Hybrid Pooling**

| Account Type | Company Name | System Date |
|---|---|---|
| CT account (100001) | Temenos core banking Norway company | 25/10/2017 |
| TR account (100002) | Temenos core banking Norway Sweden | 23/10/2017 |
| TR account (100003) | Temenos Core Banking Norway Finland | 24/10/2017 |

**Misc**

| Values in the Data Item field | Description |
|---|---|
| CONTROL TOTAL | Displays the total number of items in the request. If this is provided in the message, it is checked against the number of actual entries in the message. |
| SIGN | When the sign is not supplied in the request, the value in the header is used by default. |
| CURRENCY | When the currency is not supplied in the request, the value in the header is used by default. |
| LOCAL REF | Supplied at the header level and stored in the AC.INWARD.ENTRY record, which stores the header of the CSMBATCH message. |
| EXT.BATCH.REF | The batch reference provided in the batch message (if any) is not only populated in the batch entry in AC.INWARD.ENTRY , but also in the individual ones. For CSM and CSMBULK, this is populated in the accounting entries raised on the contra account and on the accounts specified in the request message; it will be stored in STMT.ENTRY / CATEG.ENTRY / RE.CONSOL.SPEC.ENTRY , in the ADD.DETAIL.VALUE field associated with the ADD.DETAIL.NAME field, which has the value “EXT.BATCH.REF”. |

**Misc**

| Values in the Contra Entry field | Description |
|---|---|
| ENTRY | The balancing entry is raised for each entry indicated in the request. |
| CURRENCY.NET | Balance by currency, netting debit and credit entries, irrespective of the value date. If the entries that are part of an online posting message are netting for each currency to zero, a balancing entry is not raised. |
| CURRENCY | Balance by currency and sign, irrespective of the value date. A consolidated entry is created for all debit/credit entries, per each currency. |
| CCY.VAL.NET | Balance by value date and currency, irrespective of sign netting debits and credits. If the entries that are part of an online posting message are netting to zero per currency and per value date, a balancing entry is not raised. |
| CURRENCY.VAL.NET | Balance by currency, sign and value date. A consolidated entry is created for all debit/ credit entries, per each currency, sign and value date. |
| LOCAL | To raise balancing entries in the local currency irrespective of request currency. Balancing happens by value date, processing date, accounting date, and netting the debit and credit entries irrespective of sign. |
| CCY.PROC.NET | To allow balancing using currency, processing date, and netting debit and credit entries irrespective of sign. |

**Misc**

| Business Event | Description |
|---|---|
| settlementService.checkFunds.fundAvailable | Event for a cover request when sufficient funds are available in the account |
| settlementService.checkFunds.fundNotAvailable | Event for a cover request when sufficient funds are not available in the account |
| settlementService.creditRequest.accountCredited | Event for a book request when the account is credited successfully |
| settlementService.creditRequest.creditFailed | Event for a book request when credit transaction to an account fails |
| settlementService.creditRequest.creditSubmittedForRetry | Event for a book request when credit transaction to an account submitted for a retry |
| settlementService.creditRequest.creditSuspended | Event for a book request when credit transaction to an account gets suspended |
| settlementService.debitRequest.accountDebited | Event for a book request when the account is debited successfully |
| settlementService.debitRequest.debitFailed | Event for a book request when debit transaction to an account fails |
| settlementService.debitRequest.debitSubmittedForRetry | Event for a book request when debit transaction to an account submitted for a retry |
| settlementService.debitRequest.debitSuspended | Event for a book request when debit transaction to an account gets suspended |
| settlementService.reserveRequest.fundReserved | Event for a reserve request when the funds are reserved successfully |
| settlementService.reserveRequest.reserveFundFailed | Event for a reserve request when the funds reserve fails |
| settlementService.transactionRetry.fundRecovered | Event for a transaction retry when the funds are recovered successfully |
| settlementService.transactionRetry.fundReserved | Event for a transaction retry when the funds are reserved successfully |

**Misc**

| S.No. | Parameters | Description |
|---|---|---|
| 1. | AC.ENTRY.PARAM | The processing rules related to Generic Accounting Interface (GAI) messages are described in the AC.ENTRY.PARAM application. Nonfinancial option in the Attribute field indicates the non-financial clearing messages and its respective responses updated in the AC.INWARD.ENTRY.NONFIN table. If this attribute is not set, all messages continue to update in existing way, that is, in the AC.INWARD.ENTRY table. |

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

**Accounting in Deposits**

| Enquiries | Description |
|---|---|
| AA.DETAILS.ACCOUNT | Displays the Product, Account Number, Arrangement Date, Customer Name and Arrangement Status of an Arrangement |
| AA.DETAILS.ACTIVITY.LOG.FIN | Displays the activity log of an Arrangement |
| AA.DETAILS.ACTIVITY.LOG.FIN ARRANGEMENT.ID | Displays the financial activity log of an Arrangement |
| AA.DETAILS.ACTIVITY.LOG.FIN.HISTORY | Displays the financial activities log maintained in the history table such as Date, Activity, Type, Transaction Amount and Status of an Arrangement |
| AA.DETAILS.ACTIVITY.LOG.FINANCIAL.FIN | Displays the Activity Type, Status and Transaction Amount of an Arrangement |
| AA.DETAILS.ACTIVITY.LOG.USER.FIN | Displays the User Activities, Status, and Transaction Amount of an Arrangement |
| AA.DETAILS.ACTIVITY.LOG.PENDING.FIN | Displays the pending financial activities of an Arrangement |
| AA.DETAILS.ACTIVITY.LOG.SYSTEM.FIN | Displays the financial activity initiated by the system of an Arrangement |
| AA.DETAILS.ACTIVITY.LOG.TOTAL | Displays the total activity log details of an Arrangement |
| AA.DETAILS.ACTIVITY.LOG.USER.FIN | Displays the financial activities initiated by the user of an Arrangement |

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


### Deposits - FD (FD)


**Fiduciaries Workflow**

| Field Name | Description |
|---|---|
| ID | Indicates the record ID of FD.FIDUCIARY |
| Fid Bank | Displays the value in the Fid Bank field in FD.FIDUCIARY application |
| Fid Bank Ref | Holds the reference as provided by the Fiduciary bank |
| Order ID | Holds the FD.FID.ORDER ID |
| Interest Rate | Defaults from FD.FIDUCIARY application |
| Interest Frequency | Defaults from FD.FIDUCIARY application |
| Sys Int Date | Automatically calculated by the system based on the frequency set up in FD.FIDUCIARY |
| Sys Interest Amt -XX | Indicates the system calculated interest amount for the same period |
| Sys Wht Tax –XX | Defaults the value from Sys Wht Tax Amt in FD.FID.ORDER |
| Fid Bank Int Date -XX | Allows to input the interest date as provided by the Fiduciary bank. It helps to reconcile between Temenos Transact date and Fiduciary bank date |
| Fid Bank Int Amt -XX | Defaults to the value in Interest Amt field |
| Fid Bank Wht Tax -XX | Defaults to system calculated tax amount and can be changed |
| XX | Defaults to Sys Interest Amt but can be changed. This is to input the interest amount as provided by the Fiduciary bank which helps to reconcile between Temenos Transact interest amount and Fiduciary bank interest amount. A change up to one round unit (example, USD 1) is allowed. This will be the interest amount updated in FD.FIDUCIARY . |
| Total Interest | Indicates the total of the Interest Amt fields |
| Maturity Date | Indicates the maturity date of the Fiduciary. If early maturity is accepted, then this field is updated with early maturity date. |
| Maturity Amt | Holds the principal amount on maturity. If early maturity is accepted, this field is updated with the early maturity amount. |
| Mat Amt Recd Date | Indicates when the maturity amount or early maturity amount was actually received from the Fiduciary bank. |

**Fiduciaries Workflow**

| Field Name | Description |
|---|---|
| Acct Trans PO | Flag that decides whether to process counterparty payment through the PAYMENT.ORDER application or not. The possible values are: Yes - Signifies that a PO is generated and MT202 is triggered from PO . NULL - MT202 is generated directly from Fiduciary. |
| Po Product | Holds a valid record of PAYMENT.ORDER.PRODUCT . |
| Po Susp Categ | Holds a valid category account. It is the wash category used while generating entries related to external payments. |

**Misc**

| Field | Description |
|---|---|
| Fiduciary Type | Indicated type of fiduciary contract that is allowed (Fixed or Notice). |
| Margin Rate | Indicates the default margin rate associated with the Fiduciary Type . |
| Accr Cycle Int | Defines the date and frequency for the next accrual of interest. Frequency can be either DAILY or MONTHLY. |
| Accr Cycle Comm | Defines the date and frequency for the next commission accrual. Frequency can be either DAILY or MONTHLY. |
| Pl Accr Comm | Indicates the profit and loss category used for posting commission accruals for fixed fiduciary orders. |
| Int Diff Cat | Indicates the category code of the internal account to be used for posting any difference entry between the placement interest and order interest. |
| Broker Cat | Indicates the profit and loss category to be debited when brokerage is payable. |
| Renewal Days | Defines the number of days prior to maturity of the existing order, when the renewed order is to be created. It can be defined as 1-99 “C/W”, calendar or working days before the maturity of the existing order. |
| Ex Asset Type | Indicates the asset types to be excluded for customer valuation. |
| Ex Sub Ass Type | Indicates the sub asset types to be excluded for customer valuation. |
| Placement Profile | Defines whether the FD.PLACEMENT.PROFILE must be used to allocate or check the bank of placement within fiduciary transaction. |
| Holiday Calendar | Calculates Interest and Maturity dates for Fixed Term Deposits. |
| Value Date Offset | Offset is used to arrive at the value date of the Fiduciary Order. |
| Interest Schedule | Defines whether the interest payment schedule is required to generate for Fixed Fiduciary contracts. |
| Int Acct Categ | Indicates the account used to post funds from fiduciary (Interest / Maturity Amount) until the actual fund is received from the fiduciary bank. |
| Acct Trans PO | Flag that decides whether to process counterparty payment through the PAYMENT.ORDER application or not. The possible values are: Yes - Signifies that a PO is generated and MT202 is triggered from PO . NULL - MT202 is generated directly from Fiduciary. |
| Po Product | Holds a valid record of PAYMENT.ORDER.PRODUCT . |
| Po Susp Categ | Holds a valid category account. It is the wash category used while generating entries related to external payments. |


---
