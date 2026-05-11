
# Temenos Transact — Cash_Management Module Documentation


> **Comprehensive User Guide**
> Generated: 13 April 2026
> Content: Configuration | Reference | Field Descriptions | Glossary


## Table of Contents

  - [Cash_Management Module Overview](#cash_management-module-overview)
    - [Sub-Module Summary](#sub-module-summary)
    - [How to Use This Guide](#how-to-use-this-guide)
  - [Chapter 1: Cash_Management - BN](#chapter-1-cash_management---bn)
    - [Features in Cash_Management - BN](#features-in-cash_management---bn)
    - [1.1  Account Statements](#11-account-statements)
    - [1.2  Charges and Commissions](#12-charges-and-commissions)
    - [1.3  Hybrid Pooling](#13-hybrid-pooling)
    - [1.4  Misc](#14-misc)
    - [1.5  Charges](#15-charges)
    - [1.6  SubAccounts](#16-subaccounts)
    - [1.7  Limit Balance](#17-limit-balance)
    - [1.8  Misc](#18-misc)
    - [1.9  Chargeoff](#19-chargeoff)
    - [1.10  Charges](#110-charges)
    - [1.11  LendingRule78](#111-lendingrule78)
    - [1.12  Loan Commitment](#112-loan-commitment)
    - [1.13  Migration of LendingArrangements](#113-migration-of-lendingarrangements)
    - [1.14  Payment Holiday](#114-payment-holiday)
    - [1.15  Scheduling Payments](#115-scheduling-payments)
    - [1.16  Weighted Average Rate](#116-weighted-average-rate)
    - [1.17  Misc](#117-misc)
  - [Chapter 2: Cash_Management - PO](#chapter-2-cash_management---po)
    - [Features in Cash_Management - PO](#features-in-cash_management---po)
    - [2.1  NSF ExceptionProcessing](#21-nsf-exceptionprocessing)
    - [2.2  External LoC](#22-external-loc)
    - [2.3  Investment Sweeps](#23-investment-sweeps)
    - [2.4  Misc](#24-misc)
    - [2.5  Notional Pooling](#25-notional-pooling)
    - [2.6  Overdraft Protection](#26-overdraft-protection)
    - [2.7  Physical Pooling](#27-physical-pooling)
  - [Appendix A: Glossary of T24 Applications & Fields](#appendix-a-glossary-of-t24-applications-fields)
    - [Applications](#applications)
    - [Fields Referenced](#fields-referenced)
  - [Appendix B: Consolidated Field Reference](#appendix-b-consolidated-field-reference)
    - [Cash_Management - BN (BN)](#cash_management---bn-bn)
    - [Cash_Management - PO (PO)](#cash_management---po-po)

---


## Cash_Management Module Overview


This document provides comprehensive documentation for the **Cash_Management** module of Temenos Transact. It covers **2 sub-modules** with a total of **24 feature areas**.


### Sub-Module Summary


| # | Sub-Module | Code | Features | Description |
|---|-----------|------|----------|-------------|
| 1 | **Cash_Management - BN** | `BN` | 17 | Cash_Management - BN module of Temenos Transact |
| 2 | **Cash_Management - PO** | `PO` | 7 | Cash_Management - PO module of Temenos Transact |


### How to Use This Guide


Each feature in this document is organized into the following sections:

- 📖 **Introduction** — Overview and purpose of the feature
- ⚙️ **Configuration** — How to set up and configure the feature
- 🔧 **Working With** — Operational usage and field descriptions
- 📋 **Tasks** — Step-by-step procedures
- 📊 **Outputs** — Reports, enquiries, and generated outputs

Each feature includes a **Quick Reference Card** at the top with application names, key fields, prerequisites, and a summary. Appendices provide a full glossary, consolidated field tables, and end-to-end use-case scenarios.

---


## Chapter 1: Cash_Management - BN


Cash_Management - BN module of Temenos Transact


### Features in Cash_Management - BN


| # | Feature | Sections |
|---|---------|----------|
| 1.1 | Account Statements | Intro |
| 1.2 | Charges and Commissions | Worki |
| 1.3 | Hybrid Pooling | Intro, Confi, Worki, Tasks, Outpu |
| 1.4 | Misc | Intro |
| 1.5 | Charges | Worki |
| 1.6 | SubAccounts | Confi |
| 1.7 | Limit Balance | Intro |
| 1.8 | Misc | Intro |
| 1.9 | Chargeoff | Worki |
| 1.10 | Charges | Worki |
| 1.11 | LendingRule78 | Intro |
| 1.12 | Loan Commitment | Confi |
| 1.13 | Migration of LendingArrangements | Worki |
| 1.14 | Payment Holiday | Intro, Confi, Worki |
| 1.15 | Scheduling Payments | Confi, Worki |
| 1.16 | Weighted Average Rate | Intro |
| 1.17 | Misc | Intro |


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


### 1.2  Charges and Commissions


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


### 1.3  Hybrid Pooling


> **📇 Quick Reference Card**
> 
> **Purpose:** *The following provides the user with an overview on Balance Netting (BN):*
> 
> **Key Fields:** *AA Bundle ID*, *Act Credit Check*, *Align Dates*, *Allow Netting*, *Alt Acct Id*, *Alt Acct Type*, *Alt Id Type*, *Alternate Id* ... +60 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The following provides the user with an overview on Balance Netting (BN):

- Balance Netting (BN) pool is a hybrid cash pool, which the advantages of cash concentration but maintains records of individual account transaction and balances.
- Every transaction for an account within a pool is transparently diverted to a concentration account per currency while transaction accounts have a memo record of every entry and maintains a memo-balance. Hierarchical arrangement of structures allows accounts to be sub-grouped under summary accounts within the pool.
- This is beneficial for the corporate group to manage cash-flow and bank account balances efficiently, with the ability to concentrate balances per currency at the pool level, net interest is optimised for the whole group.
- Cover control in real-time within the structure makes efficient use of available liquidity while maintaining overall control of credit utilisation within the pool.
- This helps the corporate have a full view and control of their liquidity to minimise their short-term credits and also to manage their working capital.
- Balance netting as a cash pooling alternative to zero balancing or notional pooling, minimises the risk for the financial institution and also helps the financial institution and the corporate regulatory compliance better.
- The BN cash pool consists of five different account types arranged in a hierarchical structure. The account types are Master Account (MA), Currency Top Account (CT), Multi-Currency Summary Account (SA), Single-Currency Summary Account (CS) and Transaction Account (TR). There are some TR accounts that are held in other systems, which is reflected in Temenos Transact as mirror TR accounts.
- Only TR’s carry transactions, the four other account types only carries account balances. Balances on all levels are updated real-time from transaction posted to TR’s. Although, the transactions are diverted to the CT, the query on them is always for balances and not for individual movements. Account statements are produced at the TR level.
- Bank balances (represented only by balances on CT’s) are kept separate, and the CT’s always show the net position of all transactions posted to TR’s in each currency. Only the CT’s balances are to be reported to the bank’s general ledger. All other accounts are memo accounts.


##### Features of Hybrid Pool

- Every transaction that hits a TR is automatically replicated by the system on the corresponding CT account (as a real posting) and on the corresponding summary accounts (as memo posting) so as to maintain balances and enable cover control at every level possible. Individual movements are recorded at the CT level Individual movements are suppressed at the summary account level (but balances are maintained real-time)

- Real time cover control (limit check) for the bank limit at CT or MA level. Types of external over control: Multi-Currency Credit Facility ( MCCF) Multi-Currency Facility (MCF) Single Currency Credit Facility (SCCF) Single Currency Facility
- Real time over control for the corporate’s own internal limits at TR, CS or SA level. Transactions can be classified as, Internal transactions happening between two TRs of the same pool (they don’t affect the pool balance) External credit or debit transactions happening on a TR against another account outside of the pool and this increases or decrease the pool balance.
- Internal cover control can be enabled or disabled based on transaction types internal and/or external.
- When switched on, the internal limits also play a part in determining if a payment can be made.
- Bank interest fees calculated at CT level and posted against that CT account and is reflected on the bank’s books.
- When calculated at MA level, it is posted against a nominated CT account.
- The corporate’s own internal interest fees are charged against their subsidiaries, represented by summary type account (CS or SA) or at the TR account level. These are off-balance sheet for the bank and need not reflect on their books.
- The BN cash pool improves liquidity handling and facilitates treasury processes. Efficient treasury management requires optimal usage of banks, solutions and processes, this includes: Continuous visibility to real-time cash balances Efficient support systems and fully compliant solutions A clear overview of liquidity to prevent overdrafts and costly transactions Visibility over currency exposures Minimised manual work, freeing up time for value added services

- This optimisation achieved when all accounts are available cross-border and cross-currency in an easy to use format.
- The BN cash pool helps the corporate treasury to: Get a grip on group liquidity Fund and administrate local accounts Avoid running large local credit facilities Use idle cash in one country to cover a deficit in another Maximise net interest on group liquidity Establish common accounting routines for inter company balances Create multi-level account hierarchy to reflect corporate structure Optimise credit and debit interest on overnight pool position Calculate interest on accounts within the pool based on internal rates

A hybrid cash pool, which provides all of the advantages of cash concentration but maintains records of individual account transaction and balances. Every transaction for an account within a pool is transparently diverted to a concentration account per currency while transaction accounts have a memo record of every entry and maintains a memo-balance. Hierarchical arrangement of structures allows accounts to be sub-grouped under summary accounts within the pool.

AA bundle arrangement governs the pool terms and conditions between bank and customer. The arrangement includes base currency, allowed currencies, country of domicile for the arrangement (transaction accounts can be domiciled at any branch), interest rates, fees and credit facilities. Multi-currency arrangements calculate interest on the entire structure using weighted interest rates. The arrangement allows pools to include accounts across all branches of the bank. The entire balance of the pool viewed in currency of the master account bundle (physical conversion does not takes place).

The Bundle product feature is enhanced to facilitate IBAN generation for the master account of the Bundle.

The user can input the Generate Iban and Alt Id Type fields during Bundle Draft activities, Preliminary Stages and New Bundle activity. For live Bundles, the user can update the fields through BUNDLE-UPDATE-PRODUCT.BUNDLE activity.

If Generate Iban is set to Yes, the IBAN is generated at the time of validating Switch to preliminary and Update activities. This enables the search for the master arrangement using the IBAN number.

For additional information refer to the Generating IBAN section in Product Bundle.

Currency positions are maintained in on-balance sheet currency top accounts (one per currency), every transaction for an account in the respective currency within a pool is transparently diverted to these accounts. Bank interest is calculated using the balances of these accounts.

Off-balance sheet memo-account types allow sub-grouping of the BN pool. types of summary account

- Summary account (memo account) – groups together accounts of the same currency
- Currency summary account – groups together accounts in different currencies

> **⚠️ Note:** Both types of summary account maintain a memo-balance calculated from the balances of all of its child accounts. In the case of the currency summary account the balance is calculated in the currency of the currency summary account (physical conversion takes place).

Transaction accounts are off-balance sheet and all have account numbers recognised by local clearings. Every transaction for a TR is transparently diverted to the respective currency top account very has a memo record of every transaction and maintains a memo-balance. Existing on-balance accounts can be added to a balance netting pool and are automatically converted to off-balance sheet TR when joining.

A special type of off-balance sheet in Temenos which records transactions and balance on accounts held with the bank that are maintained in another vendor’s core banking system.

When the bank provides credit facilities to the corporate this available at individual currency or multi-currency level. Within the structure it is possible to set (whether the facility is used throughout the structure) and in the case of a multi-currency facility, exclude currencies that need not participate in the facility. Credit cover control checks available balance at all levels within the structure and reports breaches even if cover is available within the pool.

Interest rates between the bank and the corporate can be set on all summary and transaction accounts within the cash pool. Alternatively interest rates can be set at summary and/or transaction account level.

The options distribute interest to transaction accounts within a balance netting pool are:

- Summary and transaction accounts have no interest calculated
- Summary and transaction counts have interest calculated but not posted
- Summary and transaction accounts have interest calculated and posted

Summary and transaction accounts can inherit interest rate, limits and fee conditions from an immediate parent or parent higher up within the BN pool structure. Different conditions can be inherited from different parents.

BN cash pool structures can be graphically built, maintained and viewed through a graphical hierarchy representing the links between accounts.

The transactions arriving or leaving accounts within the cash pool are transparently diverted to the respective currency top account transactions between accounts within the cash pool can be posted without needing to pass through the currency top account. Such intra cash-pool transactions include:

- Account to account transfers
- Standing orders
- Sweeps
- Internal interest and charges

Internal Foreign Exchange (FX) allows the corporate customer to perform cross-currency movements without affecting the bank’s currency positions. Such transactions entered manual one-off internal transfer or auto generated as sweeps. When posting internal transactions between TR within the same BN ash ool the balances of the respective currency top accounts are not changed.

The BN ash pool definition stores buy, sell, mid-rate and spread rates of currencies allowed for internal FX.


##### Functional Overview

BN pool structure accounts are implemented as follows:

| Account Types | Description |
|---|---|
| Master account | AA product bundle The Property Class bundle hierarchy specifies the allowed products of the hierarchy and the hierarchy structure itself. |
| Currency top account | On-balance sheet AR account and attached to the MA bundle as bundle participants. One of these CT accounts are nominated as the recipient of the bundle for interest at MA level and it is effectively deemed as the currency of the MA for advices or statements or MA balance enquiries purposes |
| Transaction or Mirror transaction or Currency summary or Multi currency summary accounts | Off-balance sheet AR accounts Currency summary, multi-currency summary and CT accounts – disabled for external posting Multi-currency summary account – enabled to maintain currency wise balances |

| Column 1 | Column 2 |
|---|---|
| MA level cover control | A limit shared by all the CT accounts of that MA, with Allow Netting field set as Yes, in Limit property class. |
| Multi Currency Credit Facility(MCCF) | Credit facility granted by the bank. Implemented as a limit shared by all the CT accounts, with Allow Netting field set as Yes, in Limit property class. |
| Multi Currency Facility (MCF) | Credit facility is not granted by the bank. Implemented as a limit (with limit amount as 0), shared by all the CT accounts, with Allow Netting switched on in limit. |
| Single Currency Credit Facility(SCCF) | Credit facility granted by the bank. Implemented as a single limit for each CT account. |
| Single Currency Facility(SCF) | Credit facility is not granted by the bank. Implemented as CT accounts without any limit attached to them. |
| Restrict utilisation of a limit for a specific currency | The Utilize Limit and Utilize Amount fields in Limit Property are used to completely restrict a CT account from utilising the available balance of a shared limit or specify a cap for utilising the available balance of the shared limit. |

- The Credit Check and Transaction Type fields in limit property to enable or disable internal cover control by transaction types
- The Utilize Amount field reused is treated as the Internal Limit Amount’

Automation of administrative tasks related to the Balance Netting (BN) pool administration is possible throughout the lifecycle such as, opening, maintenance and closure of the pool.

- Opening a pool structure takes the user through a purpose built workflow starting from creating a raft structure, moving it to preliminary and then taking it live.
- Maintenance of the pool structure includes pool level events such as, addition or removal (external restructuring) or changing parent (internal restructuring) of the accounts in the pool – This is allowed both in preliminary and live status.
- Closure events in the pool structure could be that of an individual account or substructure or the whole pool itself.

Several validations and orchestrations are in place to guide the user.


#### ⚙️ Configuration

The below configuration should be setup before setting up a hybrid pool:

When the system needs to apply different set of exchange rates during currency conversion for cover control or interest calculation purposes (at CT or multi-currency summary accounts level, it is done by specifying a different currency market in the individual account product definitions.

- Hence, a new CURRENCY.MARKET record needs to be created.
- ID – 2
- Description: ECB
- This currency market is configured in each CURRENCY record along with the rates or spreads.
- During processing, when the system cannot find the exchange rates for the currency market, for a given currency, it uses the default CURRENCY.MARKET 1.

The Transaction Type field in TRANSACTION table classifies the transaction codes as Internal or External. The credit and debit transaction codes used must be classified as Internal in the TRANSACTION table for,

- Configuring manual internal transfers (through FUNDS.TRANSFER )
- Automated internal transfers ( STANDING.ORDER ) or sweeps ( AC.CASH.POOL )

| Account Type | Account Number | Balance |
|---|---|---|
| Master | AA181081MPX8 (USD) | – |
| Currency top | 85577 (USD) | 8000 (USD) |
| Currency top | 85588 (EUR) | 0 (EUR) |
| Transaction | 85596 (USD) | 3000 (USD) |
| Transaction | 85607 (USD) | 5000 (USD) |
| Transaction | 85618 (EUR) | 0 (EUR) |

The below configuration should be setup after setting up hybrid pool:

The currency top accounts is setup as AR product. It can be a new product under the same product group as other standalone accounts.

The account property class defines the characteristics of an account.

- The following fields are setup to define a currency top account. External Posting – No Bal Conversion Mkt – 2 (the new currency market created for BN purposes)

- The following fields are defined as non-negotiable, so a user is not able to change them at the account arrangement level. Balance Treatment External Posting Multi Currency Link Acc Num Bal Conversion Mkt

The limit property class specifies the default options for bank limits, (for currency top accounts).

The following fields are setup at a specific currency condition level, it is known at the product design time, if a certain currency exposure needs to be limited.

- Utilize Limit – No This attribute is used when restricting a particular CT account from utilising limit and while enabling a (TR or CS or SA) for internal limits. The CT account in that currency cannot utilise the shared limit even when it continues to contribute its credit balances to other accounts sharing the same limit.

Interest can setup at the bundle (interest compensation on the master account) or individual account level (CT account level).

- In the case of the former, the relevant interest property of the recipient account of the bundle is configured to calculate interest based on a rate derived from currency weighted rate calculation.

The Interest property class is used to define that. In this case, this is done at the Recipient CT Account Arrangement level conditions (should this be a negotiation with the customer – if not, it is defined in the Interest Product condition).

The following fields are setup to define currency weighted rate calculation.

- Custom Rate (within the associated multi-value set of setting tier conditions) – Yes
- Custom Rate Calculation – MULTI.CURRENCY.WEIGHTED.METHOD (In the Default Values CCY tab)
- Run Time Rate Calc – Yes
- Custom Type – Expand this multi-value for each currency that is allowed in the Master Account Product
- Custom Name – Choose Fixed or Floating depending on the rate for the currency
- Custom Value – Either a fixed rate or link it to BASIC.INTEREST index (Key to Basic Rate Text )

| Property Class | Mandatory/Optional |
|---|---|
| Property Class | Mandatory/Optional |
| CUSTOMER | Mandatory |
| PRODUCT.BUNDLE | Mandatory |
| INTEREST.COMPENSATION | Mandatory |
| BUNDLE.HIERARCHY | Mandatory |
| ELIGIBILITY | Mandatory |
| ACTIVITY.MESSAGING | Optional |
| ACTIVITY.PRESENTATION | Optional |

| Column 1 | Column 2 | Column 3 | Column 4 | Column 5 |
|---|---|---|---|---|
| Product of settlement account must be allowed in the pool | Not needed | – | – | Implicitly covered by mandating bundle membership in #4 ( this validation can be removed) |
| Settlement account must allow external postings | AF, AV and AS – Paying settlement or payout settlement or default Settlement account as the case may be | AA-PAYIN.AC.ALLOW.EXT.POSTING AA-PAYOUT.AC.ALLOW.EXT.POSTING AA-DEFAULT.AC.ALLOW.EXT.POSTING | Paying account doesn't allow the following: External posting payout account External posting default settlement account External posting |  |
| Settlement account must be a memo account | Not needed | AA-PAYIN.ACCOUNT.MUST.BE.MEMO AA-PAYOUT.ACCOUNT.MUST.BE.MEMO AA-DEFAULT.ACCOUNT.MUST.BE.MEMO | Paying account and it is not, Memo Payout account Memo Default settlement account Must be off-balance | Currently closure is not allowed. If the account is a bundle member, then it is postponed to 1B. Currently, it is a two step process of unlinking and closing. |
| Settlement account must be a member of the same bundle (ps), only if this account is part of a Bundle Hierarchy. This validation only applies for CS, SA and CT but not to a normal AR arrangement. For a normal AR arrangement, the settlement account can be memo and have its own diversion account ( that is, a TR can be attached as a settlement account to a normal AR, AL or AD (ps)) | As override during update activity, Settle payoff and transform but error during make due-schedule | AA-ACT.NOT.MBR.OF.SAME.BUNDLE | Account & is not a member of same bundle | Currently we don't allow CLOSURE if the account is a bundle member - this was postponed to 1B. For now it is a two step process of unlinking and then closing |
| Account debit rule must always be FULL for paying accounts (ps), only if this account is part of a Bundle Hierarchy (ps). | Error always. AF, AV and AS - the appropriate AC.DB.RULE | AA-PAYIN.AC.DB.RULE.MUST.BE.FULL | Account debit rule must be set to FULL within a Bundle Hierarchy |  |
| For any property in payment schedule, activity charges, activity restriction with payment method as DUE, a paying account must be defined. |  | AA-PAYIN.AC.MAND.PMT.TYPE.OFF.BAL | For schedule : Paying account is mandatory for payment type &1 defined in &2. For activity charges and activity restrictions - Paying account is mandatory for payment type &1 for &2 | For Schedule : &1 - Payment Type; &2 - description of the property where this is defined (schedule) For , activity charge or arrangement rule : &1 - Payment Type and &2 - description of activity charges or activity restriction property |
| For any property in payment schedule, activity charges, activity restriction with payment method as PAY, a payout account must be defined. |  | AA-PAYOUT.AC.MAND.FOR.PPTY.OFF.BAL | Payout account is mandatory for property & defined in & | Same as above |
| If property or property class from #7 is defined in settlement, but payout switch is OFF If any Payment Type from #6 above is defined in Settlement, but Payin switch OFF |  | AA-PAYOUT.SET.SWITCH.NOT.ON AA-PAYIN.SET.SWITCH.NOT.ON | Settlement switch is not set to YES for &1 Settlement switch is not set to YES for &1 | &1 – Property or Property Class &1 – Payment Type |
| If no settlement instruction has been defined for the payout property or property class from #7 If no settlement instruction has been defined for the payment type from #6 |  | AA-PAYOUT.SET.INSTRUCTION.NOT.FOUND AA-PAYIN.SET.INSTRUCTION.NOT.FOUND | Settlement instruction is not found for property &1 Settlement instruction is not found for Payment Type &1 | &1 – Property or Property Class &1 – Payment Type |
| Counter booking account is mandatory if any payment method in payment schedule, activity charges, activity restriction has payment method as PAY, DUE or CAPITALISE, unless bill type is AUTO.WAIVE (for Payment Schedule) |  | AA-COUNTER.BOOKING.ACCOUNT.MAND | Counter booking account is mandatory |  |
| Counter booking account must be a member of the same bundle (hierarchy) |  | AA-ACT.NOT.MBR.OF.SAME.BUNDLE | Account and it is not a member of same bundle |  |
| Counter booking account must allow external postings |  | AA-CTR.BK.AC.NOT.ALLOW.EXT.POSTING | Counter booking account and must allow posting to be made |  |
| Counter booking account must a MEMO account | Not needed | AA-CTR.BK.AC.MUST.BE.MEMO | Counter booking account & is not off-balance account |  |
| Counter booking account product must be allowed in the pool | Not needed |  |  | Implicitly covered by mandating bundle membership in #12 We can remove this validation |
| Counter booking activities are mandatory (ps), only if counter booking account is specified (ps). | Always error. AF - Counter booking credit activity and counter booking debit activity | AA-MAND.FIELD | Input is mandatory | On the contrary, Counter Booking Activities can be specified without Counter Booking Account - say, defaulted from Product |
| Counter booking activities must be valid |  | AA.INVALID.ACTIVITY.TYPE | Invalid activity type in Activity.Class | This is checked in AA.ACTIVITY.CLASS USED.PROPCLASS must contain SETTLEMENT USED field must be DR.COUNTER.BOOKING.ACTIVITY or CR.COUNTER.BOOKING.ACTIVITY respectively |
| Settlement or counter booking account is in a different company |  | AA.SET.COM.DIFF.FROM.ARR.COM | (Settlement or counter booking) account (account number) does not belong to (company) | Is only raised as override during input, not as error during processing |
| Settlement or counter booking account is in a different company (current arrangement is a CT account) |  | AA.SET.ACT.COM.DIF.FROM.ARR.COMP.EP | [Settlement/Counter Booking] Account [account number] does not belong to [company] | Is only raised as override during input, not as error during processing |
| Settlement or counter booking account is in a different currency |  | AA.SET.CCY.DIFF.FROM.ARR.CCY | (Settlement or counter booking) account (account number's) currency (currency) is not the same as this account's (arrangement currency) | Is raised as override during input, not as error during processing |
| Settlement or counter booking account is in a different currency (current arrangement is a CT account) |  | AA.SET.CCY.DIFF.FROM.ARR.CCY.EP | (Settlement or counter booking) Account (account number's) currency (currency) is not the same as this account's (arrangement currency) | Is raised as override during input, not as error during processing |


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


#### 📋 Tasks

There are no Tasks available for Hybrid Pool feature.


#### 📊 Outputs

There are no Outputs available for Hybrid Pool feature.

---


### 1.4  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *Balance netting pool is a hybrid cash pool, which provides all of the advantages of cash concentration but maintains records of individual account transactions and balances. Every transaction for an account within a pool is transparently diverted to a concentration account per currency. Whilst trans...*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- Temenos Transact Services

Balance netting pool is a hybrid cash pool, which provides all of the advantages of cash concentration but maintains records of individual account transactions and balances. Every transaction for an account within a pool is transparently diverted to a concentration account per currency. Whilst transaction accounts have a memo record of every entry and maintains a memo-balance. Hierarchical arrangement of structures allows accounts to be sub-grouped under summary accounts within the pool.


##### Configuring Balance Netting

Balance Netting has no specific configuration to be set up at the parameter level.

---


### 1.5  Charges


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


### 1.6  SubAccounts


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


### 1.7  Limit Balance


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


### 1.8  Misc


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


### 1.9  Chargeoff


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


### 1.10  Charges


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


### 1.11  LendingRule78


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


### 1.12  Loan Commitment


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


### 1.13  Migration of LendingArrangements


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


### 1.14  Payment Holiday


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


### 1.15  Scheduling Payments


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


### 1.16  Weighted Average Rate


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


### 1.17  Misc


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


## Chapter 2: Cash_Management - PO


Cash_Management - PO module of Temenos Transact


### Features in Cash_Management - PO


| # | Feature | Sections |
|---|---------|----------|
| 2.1 | NSF ExceptionProcessing | Confi |
| 2.2 | External LoC | Intro, Confi, Worki, Tasks, Outpu |
| 2.3 | Investment Sweeps | Intro, Confi, Worki, Tasks, Outpu |
| 2.4 | Misc | Intro |
| 2.5 | Notional Pooling | Intro, Confi, Tasks, Outpu |
| 2.6 | Overdraft Protection | Intro, Confi, Tasks, Outpu |
| 2.7 | Physical Pooling | Intro, Confi, Worki, Tasks, Outpu |


### 2.1  NSF ExceptionProcessing


> **📇 Quick Reference Card**
> 
> **Applications:** `AC.ACCOUNTING.PARAM`, `AC.BALANCE.COMPONENT`, `AC.CREDIT.CHECK`, `NSF.PARAMETER`
> 
> **Key Fields:** *Charge Negotiable*, *Chrg Negotiable*, *Def Fund Decision*, *Expiry Days*, *Fund Deci Approve Act; Fund Deci Rej Act; Rev Approve Act; Rev Rej Act*, *Fund Decision Upd*, *Grace Balance Type*, *Grace Locked Reserve Condition* ... +10 more
> 
> **Sections:** ⚙️ Configuration


#### ⚙️ Configuration

This topic covers the system usage of NSF exception processing.


##### Balance Components –AC.BALANCE.COMPONENT

The AC.BALANCE.COMPONENT application defines the balance components that can be configured for the NSF credit check. These balance components are classified as BASE and OPTION.

This application can only be viewed and cannot be modified as they are released and maintained by Temenos. The balance components can be used to configure the available balance for credit check during the NSF processing. The below screenshot shows the list of balance components released by Temenos.


##### Configuring the Available Balance –AC.CREDIT.CHECK

This AC.CREDIT.CHECK application creates different combinations of balance components, which can be used in credit check processing when the transaction is initiated.

It gives the flexibility to define and use different balance components for credit checking based on the transaction or activity.

This is configured in two parts.

This type is a mandatory single value field and should be defined with one of the base type balance components released by Temenos (in AC.BALANCE.COMPONENT ).

This type is an optional multi-value field which allows the bank to configure any number of option type balance components released by Temenos (in AC.BALANCE.COMPONENT ).

The below screen shot shows an example of AC.CREDIT.CHECK , which is used to define the Base balance type as WORKING and Option balance types as SWEEP and LOCK.FUNDS.


##### NSF Exception Processing Parameter –NSF.PARAMETER

This parameter is a pre-requisite for NSF processing.

The information pertaining to the order of processing the debit and credit items to the account, settlement types, expiry date and default decisions for the respective settlement types is configured in this parameter application.

The NSF.PARAMETER can be defined at the system or company level. In the absence of company specific parameter, the system level configuration is used.

The order of processing debit and credit items to the checking account is configured in the Order field. It is defaulted to Creditdebit, which indicates that the credit items to be processed first and the debit items to be processed in the order of time. The other option is Time, which indicates that the credits and debits are to be processed in the order of time.

The fields from Settle Type to Chrg Negotiable is a set of associated fields which defines the default rules for funds decision for approval, rejection and reversal. The usage of these fields are described in the below table.

| Field Name | Description |
|---|---|
| Settle Type | The possible values in the field are: PTL (Payed Through Limits) – Account balance including transaction amount is within the limit available at the time of posting the entry. POL (Payed Outside Limit) – Either account balance including transaction amount is in excess of the limit available at the time of posting the entry or the limit is not applicable (Opt-Out) for the respective debit transaction or activity. SET (Automatic Settlement) – Force settled with NSF. This debit transaction or activity is forced to be settled at the activity class definition. |
| Expiry Days | Indicates the cut-off period for manual decision making. This is the number of days within which the bank user should either approve or reject the NSF item and negotiate the NSF fee or charge. If the decision is not actioned manually, the default decision (if defined in the NSF parameter) applies on the COB of the expiry date of the NSF exception item. |
| Def Fund Decision | Hold the value approved or rejected. |
| Fund Decision Upd | Hold the value system or manual, to indicate the fund decision update. |
| Fund Deci Approve Act; Fund Deci Rej Act; Rev Approve Act; Rev Rej Act | Arrangement activity to be triggered for the default decision processing for fund approval/rejection or reversal approval/rejection. |
| Charge Negotiable | Hold the value YES or NO, to indicate if the NSF fee or charge is negotiable. |
| NSF Decision Hook | Configure the user exit routine to overrule the rule-based NSF decisioning of account transactions. |
| NSF Start Balance | Indicates the starting balance that must be used when calculating the accounts available balance used for the NSF evaluation process. It belongs to a set of associated fields. The allowed values are: Open.booked Open.valued If there is no value defined, Open.valued is the default value. |
| NSF Balance Type | Defines the inclusion of active debit holds and active credit holds in the available balance calculation during the NSF Evaluation process. It belongs to a set of associated fields. The allowed values are: Lock.funds Credit.reserve If there is no value defined, the available balance is calculated by including all the balance components. |
| NSF Lock Reserve Condition | The allowed values are: Lock.funds.date - Includes active debit locked events Credit.reserve.date - Includes active credit locked events. If there is no value defined for the associated balance type, the system refers the definition in AC.ACCOUNTING.PARAM . |
| NSF Process Type | The allowed value is: Exclude.return - Excludes the debit transaction amount from calculating the running balance when the default decision of the entry is set as RETURN or REJECT. |


##### NSF Exception Processing Parameter –NSF.PARAMETER

To enable the Grace Period NSF Charge Waiver process, the user must configure the required fields in NSF.PARAMETER as shown below.

| Field Name | Description |
|---|---|
| Grace Period Type | Indicates the balance cure method applied when Grace Period functionality is enabled. The supported values are: Full – The account must have an available balance and tolerance greater or equal to 0 for the NSF charges to be waived. Partial – Each NSF exception is evaluated to determine if the positive movement of the available balance is sufficient to cover that item. |
| Grace Start Balance | Indicates the starting balance used for calculating the accounts available balance (used for grace period waiver). The allowed values are: Actual.booked - Indicates the account’s booked balance for today. A transaction is considered booked once it is completed and the balances are updated. Transactions with a forward processing date (for example, non-stop transactions entered at the close of business) are not included in this balance until the bank’s system date matches the processing date of the transaction. Actual.value - Indicates the account’s value-dated balance for today, which is used for interest calculation. Transactions with a forward value date are not included in today’s value-dated balance until the specified value date arrives. If the balance is not defined, then Actual.value is considered as the default value. |
| Grace Balance Type | Indicates the debit locked events and credit locked events are included when calculating the account available balances used for grace period waiver. The supported values are Lock.funds and Credit.reserve. The user can select one or both the options. |
| Grace Locked Reserve Condition | Indicates if current day’s active locked events should be used or if the maximum or minimum amounts should be used when debit locked events and credit locked events are included in the account available balance calculation. The supported values are Lock.funds.date and Credit.reserve.date. The user can select one or both the options. If the field is left blank for the associated Grace Balance Type , then the system uses the setting defined in Lock Reserve Condition in AC.ACCOUNTING.PARAM as default. |


> **Related Applications:** `AC.ACCOUNTING.PARAM`, `AC.BALANCE.COMPONENT`, `AC.CREDIT.CHECK`, `NSF.PARAMETER`

---


### 2.2  External LoC


> **📇 Quick Reference Card**
> 
> **Purpose:** *Line of Credit (LoC) or Credit Cards (CC) can be used as a source of funds when covering funds deficit on the sweeping accounts. In cases when the source of funds or concentration account is maintained outside of the Temenos Transact, an External Arrangement is opened in Temenos Transact. During swe...*
> 
> **Applications:** `AA.PRD.DES.ACTIVITY.MAPPING`, `AC.ACCOUNT.SWEEP.ERROR`, `AC.ACCOUNT.SWEEP.HIST`, `AC.BALANCE.TYPE`, `AC.CASH.POOL`, `AC.CP.GROUP.PARAM`, `AC.SWEEP.CONDITIONS`, `AC.SWEEP.TYPE` ... +2 more
> 
> **Key Fields:** *Cmt Bal Type*, *Commitment Balance Type*, *Draw Bal Type*, *Drawing Balance Type*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Line of Credit (LoC) or Credit Cards (CC) can be used as a source of funds when covering funds deficit on the sweeping accounts. In cases when the source of funds or concentration account is maintained outside of the Temenos Transact, an External Arrangement is opened in Temenos Transact. During sweep execution, any transaction posted against the sweeping account is balanced automatically against the special cross-system wash account defined in the underlying sweep type record. External systems holding LoC or CC accounts feeds the Temenos Transact with information about their balances.

In a real time, for the sweep execution, the system uses the latest known information about balances. The system emit business events when the funding or link account involved in the sweep being is external arrangement, that is, Line of Credit or Credit Card.


#### ⚙️ Configuration

The External Line of Credit or Credit Card is represented in the Temenos Transact environment as an external arrangement, where the total commitment amount and the total drawing amount of the loan is presented in the Temenos Transact as off-book balances. Sweep instruction accepts a reference to such external arrangement in the same way as if that arrangement maintains the on-book (real) balance in Transact books.

To define balances ( Drawing Balance Type and Commitment Balance Type ) that can be used by the Temenos Transact in the ODP sweeps processing, the following balance prefixes are defined using the EB.LOOKUP table:

The Commitment Balance Type is shown in the image below.

The Drawing Balance Type is shown in the image below.

Relevant balance types must be created as memo balances in AC.BALANCE.TYPE as shown below.

The commitment amount is shown in the image below.

The drawings amount is shown in the image below.

Update the activity mapping for external accounts on debit and credit arrangements in AA.PRD.DES.ACTIVITY.MAPPING as shown in the image below.


#### 🔧 Working With

Line of Credit (LoC)or Credit Cards (CC) used as a source of funds when covering funds deficit on the sweeping accounts and in corporate cash pools. An ODP (Over Draft Protection) sweep against the external arrangement allows the balance available on the external arrangement to be considered in calculation of Overdraft Funds available on the cash account.

- An external arrangement is created in Transact to represent the External Line of Credit, whereas the total commitment and total drawing amount of the loan are the memo balances.
- Balances reflecting the amount of drawings and total commitment amount is fed from the banks’ software to the Transact. In a real time or within the ODP sweep execution, the system uses the latest known information about balances.

Refer to the Configuring External LoC section for more details about the set up.

For the ODP (Overdraft Protection) Sweep from LoC’s external to Transact,

- Commitment balance must be fed with the LoC Amount and the drawing balance must be fed with the outstanding balance of the LoC. The Temenos Transact computes the available for sweeping balance.
- Alternatively, available for sweeping balance can directly be fed to the Temenos Transact as commitment balance.

For the ODP (Overdraft Protection) sweep from credit cards external to Transact,

- Commitment balance must be fed with the credit Line amount and drawing balance must be fed with the outstanding balance of the credit card. the Temenos Transact computes the available for sweeping balance.
- Alternatively, available for sweeping balance can directly be fed to Transact as commitment balance.

Determining the available balance for LoC or CC:

Draw Bal Type : This field holds the total drawings of the Line of Credit or Credit Card account. Drawing Balance must be fed with the Outstanding balance of the LoC.

Cmt Bal Type : This field holds the total commitment of the Line of Credit or Credit Card account. Commitment Balance must be fed with the LoC Amount.

The Draw Bal Type and Cmt Bal Type fields of the AC.SWEEP.TYPE refers to the AC.BALANCE.TYPE table. Sweeps use the balance types defined in these fields to derive from the Transact AA Lending or external arrangement that how much funds can be moved to or from the arrangement.

In case of maintenance sweeps, when the sweeping account is funded from the CC or LoC, to calculate the amount of funds available under the LoC, the cash pool system considers the difference between the total commitment and the current drawings.

When sweeping the surplus funds to the LoC or CC, the cash pool system considers the current drawing balance when calculating the amount that could be swept to the LoC.

Sweep suspense account to be configured with internal account category for a loan type of product.

In case of the corporate sweeps against the LoC, the excess of funds may be pushed back to the LoC to repay the borrowed amount.

In case of the Maintenance Sweeps, the sweep type is configured to define the balance available to draw from the LoC, which is usually the total commitment amount less total drawings.

In case of the Surplus sweeps, the sweep type is configured to define the maximum amount that could be repaid to the LoC, which is usually the total drawings from the LoC.

When the sweep is processed, if the funding or the link account is external arrangement, then system automatically balances the sweep transaction against the special cross-system wash account as configured on the respective sweep type.

For example,

In a maintenance sweep, if the funds required to be swept is USD 500 from an external arrangement to a Transact sweep account, the system raises the following three ledger entries.

- Dr. Sweep Suspense Account: -USD 500
- Cr. Sweeping Account: USD 500
- Dr. External Arrangement Account: -USD 500 (Memo/Off-Book Entry - XDRBALANCEINF)

In a surplus sweep, if the funds required to be paid is USD 500 to an external arrangement from a Transact sweep account, the system raises the following three ledger entries.

- Cr. Sweep Suspense Account: USD 500
- Dr. Sweeping Account: -USD 500
- Cr. External Arrangement Account: USD 500 (Memo/Off-Book Entry - XDRBALANCEINF)

While sweep execution, the system emits the following business events when the funding or the link account involved in the sweep is an external arrangement.

In a maintenance sweep, when funds are requested from an external funding accounts like LoC or CC,

- Event Name: accounts.sweepTransaction.fundsRequested
- Event Description: Request to be disburse or release funds from the loan or credit card accounts held in the systems external to Transact
- Event Data: Event Payload includes the following details.

| Event Attribute Name | Description |
|---|---|
| transactionReference | Indicates the unique reference for the sweep transaction which has initiated the funds request. |
| transactionDate | Indicates the business date on which the sweep transaction was initiated. |
| sweepingAccountId | Indicates the Account Reference/ID of the sweeping account in Transact. |
| sweepingAccountCurrency | Indicates the currency of the sweeping account. |
| contraCategoryOrAccount | Indicates the sweep suspense account. |
| accountId | Indicates the Account Reference/ID of the external arrangement in Transact that represents the LOC/CC on the external systems. |
| alternateReferences | Collection – Contains details of all alternate ids applicable for the external arrangement in Transact. |
| requestAmount | Indicates the amount that is required to be disbursed or released from the loan or credit card accounts held in the systems external to Transact. |
| requestCurrency | Indicates the Currency associated to the requestedAmount. |
| alternateAccountType | Identifies the alternate account id type applicable for the associated alternate Id of the external arrangement in Transact. |
| alternateAccountId | Identifies the alternate account id applicable for the associated alternate account id type of the external arrangement in the Temenos Transact. For example, Account Reference of the LOC / CC in the external system. |

In a surplus sweep, when funds are paid out to an external account like LoC or CC, the following event is emitted.

- Event Name: accounts.sweepTransaction.fundsPaidOut
- Event Description: Funds available on the sweeping account is paid out to an external account - LoC or CC
- Event Data: Event Payload includes the following details

| Event Attribute Name | Description |
|---|---|
| transactionReference | Indicates the unique reference for the sweep transaction which has initiated the funds request. |
| transactionDate | Indicates the business date on which the sweep transaction was initiated. |
| sweepingAccountId | Indicates the Account Reference/ID of the sweeping account in Transact. |
| sweepingAccountCurrency | Indicates the currency of the sweeping account. |
| contraCategoryOrAccount | Indicates the sweep suspense account. |
| accountId | Account Reference/ID of the external arrangement in Transact that represents the LOC/CC on the external systems. |
| alternateReferences | Collection – Contains details of all alternate ids applicable for the external arrangement in Transact. |
| paidOutAmount | Indicates the amount that is repaid to the LoC / CC in the external system. |
| currency | Indicates the Currency associated to the paidOutAmount. |
| alternateAccountType | Identifies the alternate account id type applicable for the associated alternate Id of the external arrangement in Transact. |
| alternateAccountId | Identifies the alternate account id applicable for the associated alternate account id type of the external arrangement in Transact. For example, Account Reference of the LOC / CC in the external system. |

In case of insufficient funds in the Loan available balance, below process takes place.

Failed loan disbursements are reported back to Transact using the Generic Accounting Interface (GAI) API, providing information about the reason of the failure. The API request sent to Transact must include following details:

- Sweeping account number
- Failed disbursement amount
- Unique sweep reference
- Funds requested date

When the message about failed loan disbursement is received in Transact,

- Relevant sweep transaction is marked as failed, a new GAI post routine is released from Temenos which updates the file AC.ACCOUNT.SWEEP.ERROR in Transact.
- The amount credited by the ODP sweep to checking account is reversed, posting credit to the sweep suspense account. No update of the external arrangement happens automatically as part of that reversal.

| Account Details | Account No |
|---|---|
| Sweeping Account | 123242 |
| Funding Account (LoC) | 123258 |


#### 📋 Tasks

There are no Tasks available for External LoC feature.


#### 📊 Outputs

There are no Outputs available for External LoC feature.


> **Related Applications:** `AA.PRD.DES.ACTIVITY.MAPPING`, `AC.ACCOUNT.SWEEP.ERROR`, `AC.ACCOUNT.SWEEP.HIST`, `AC.BALANCE.TYPE`, `AC.CASH.POOL`, `AC.CP.GROUP.PARAM`, `AC.SWEEP.CONDITIONS`, `AC.SWEEP.TYPE`, `EB.LOOKUP`, `STMT.ENTRY`

---


### 2.3  Investment Sweeps


> **📇 Quick Reference Card**
> 
> **Purpose:** *Temenos Transact enables the Corporate users to invest their excess funds in an investment instrument and re-deposit into the Checking Account in case of deficit.*
> 
> **Applications:** `AA.PROPERTY`, `AC.ACCOUNT.SWEEP.HIST`, `AC.BALANCE.TYPE`, `AC.CASH.POOL`, `AC.SWEEP.CONDITIONS`, `AC.SWEEP.TYPE`, `CURRENT.ACCOUNT`, `EXTERNAL.ACCOUNT` ... +2 more
> 
> **Key Fields:** *Link Suspension End Date*, *Link Suspension Start date*, *Link Sweep Cancel Date*, *Max Contribution Amount*, *Max Contribution Amt*, *Max Redemption Amt*, *Max Sweep Amt*, *Min Contribution Amt* ... +6 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Temenos Transact enables the Corporate users to invest their excess funds in an investment instrument and re-deposit into the Checking Account in case of deficit.

When the Checking Account (also known as DDA Account/Main Account/Master Account) has surplus funds, the surplus amount could be transferred to an investment instrument that yields a favourable interest rate. If funds in the Checking Account is in deficit, then the funds invested in the investment instrument are matured and transferred to the checking account. A combination of Line of Credit (LoC) Accounts and Investment Account can also be linked to the Checking Account and funds could be transferred to both the link accounts and vice-versa. Investment Sweep execution is an end of day process and hence the transfer of funds happen during close of business.

For Surplus sweeps, there is an option to sort the sweep amounts from 'High to Low' or 'Low to High' and then execute the sweep. Also there could be a restriction on the minimum and maximum amounts invested into an Investment Account.

For Maintenance sweeps, when the funds are redeemed from the Investment Account, we can optionally restrict the minimum and maximum redemption amount.


#### ⚙️ Configuration

When the Investment type of sweeps have to be processed,

- The Investment Account Configuration has to be as defined and an investment account has to be created under this product for each cash pool record.
- The suspense account for a given investment type has to be mentioned in the Sweep Susp Acct field of the AC.SWEEP.TYPE record.
- The conditions to be applied to the investment product to be defined in AC.SWEEP.CONDITIONS .
- It is suggested to have the Minimum and Maximum Amounts in AC.CASH.POOL record with the same value.


##### Investment Account Configuration

To configure the Investment Account,

1. Create the AA.PROPERTY record as shown in the image below.
2. Make reporting type as Internal in AC.BALANCE.TYPE .
3. Create a new product group named INVESTMENT.ACCOUNT .
4. Create a new product under the product group INVESTMENT.ACCOUNT .
5. Proof and publish the product.


#### 🔧 Working With

When the Checking Account has excess funds, the excess amount is transferred from the Checking Account to the Investment Account.

Below values can be defined for Surplus sweep:

- Sweep Amount Sorting : 'High to Low' or 'Low to High' before sweep execution and sweep to be executed based on the sweep amounts sorted. This option has to be defined in the appropriate AC.SWEEP.TYPE record.
- Min Sweep Amt / Max Sweep Amt : Sweeps from current account to investment account could be restricted based on the minimum and maximum sweep amount. These fields are available in AC.SWEEP.CONDITIONS .
- Min Contribution Amt / Max Contribution Amt : The funds invested by a bank to a specific Investment Instrument could be restricted based on the values in Min Contribution Amt and Max Contribution Amt . These fields are available in AC.SWEEP.CONDITIONS .

Sweep sorting from low to high:

(For this example 14313 is used) and sweep amt sorting as low to high.

AC.SWEEP.CONDITIONS record created for today’s date with the above sweep type, max contribution amt as 100,000 and Min Contribution Amt USD 1000.

Four accounts to be created with product as CURRENT.ACCOUNT . These are used as main master accounts in the 4 different cash pool records.

Four investment accounts with product as INVESTMENT.ACCOUNT to be created (One investment account for each cash pool record).

Four different cash pool records are input with Investment type of link accounts and the above created sweep type. The balances in the main master account are maintained with the amount exceeding the maximum amount. Also, the balances to be maintained in such a way that the overall sweep amount of the five cash pools doesn’t exceed Max Contribution Amt and is over Min Contribution Amt.

CASH POOL 1 - Sweep Amt USD 6700

CASH POOL 2 - Sweep Amt USD 1500

CASH POOL 3 - Sweep amt USD 9200

CASH POOL 4 - Sweep amt USD 1000

View of the STMT.ENTRY after COB is shown in the image below.

Sweep has been performed in low to high sorted order.

(For this example 14313 is used) and Sweep Amt Sorting as high to low.

AC.SWEEP.CONDITIONS record is created for today’s date with the above sweep type, Max Contribution Amt as USD100,000 and Min Contribution Amt as USD1,000.

Four accounts to be created with product as CURRENT.ACCOUNT . These are used as main master accounts in the four different cash pool records.

Four investment accounts with product as INVESTMENT.ACCOUNT to be created (One investment account for each cash pool record).

Four different cash pool records are input with Investment type of link accounts and the above created sweep type. The balances in the main master account are maintained with the amount exceeding the maximum amount. Also, the balances to be maintained in such a way that the overall sweep amount of the five cash pools doesn’t exceed Max Contribution Amt and is over Min Contribution Amt .

CASH POOL 1 - Sweep Amt USD 6700

CASH POOL 2 - Sweep Amt USD 1500

CASH POOL 3 - Sweep amt USD 9200

CASH POOL 4 - Sweep amt USD 1000

View of the STMT.ENTRY after COB is shown in the image below.

Sweep has been performed in high to low sorted order.

Minimum and Maximum Sweep Amount:

- If the sweep amount of a cash pool record is greater than the minimum sweep amount, then the cash pool record is considered for sweeping.
- If the sweep amount of a cash pool record is less than the minimum sweep amount, then the cash pool record is not considered for sweeping.
- If the sweep amount of a cash pool record is greater than the maximum sweep amount, then the maximum amount is considered as the sweep amount.
- If the sweep amount of a cash pool record is less than the maximum sweep amount but greater than the minimum sweep amount, then the cash pool record considered for sweeping.

> **⚠️ Note:** The sweep execution for Investment Accounts is determined by considering both Min/Max Sweep Amounts and Min/Max Contribution Amounts.

Minimum and Maximum Contribution Amount:

| Cash Pool ID | Sweep Amount (USD) |
|---|---|
| Sweep 1 | 500.00 |
| Sweep 2 | 1,000.00 |
| Sweep 3 | 2,000.00 |
| Sweep 4 | 3,000.00 |
| Sweep 5 | 2,200.00 |
| Total | 8,700.00 |

| Cash Pool ID | Sweep Amount (USD) |
|---|---|
| Sweep 1 | 500.00 |
| Sweep 2 | 1,500.00 |
| Sweep 3 | 2,000.00 |
| Sweep 4 | 5,000.00 |
| Sweep 5 | 2,500.00 |
| Total | 11,500.00 |

| Cash Pool ID | Sweep Amount (USD) | Investment Position Balance |
|---|---|---|
| Beginning of processing |  | 100,000.00 |
| Sweep 1 | 30,000.00 | 70,000.00 |
| Sweep 2 | 20,000.00 | 50,000.00 |
| Sweep 3 | 10,000.00 | 40,000.00 |
| Sweep 4 | 30,000.00 | 10,000.00 |
| Sweep 5 | 10,000.00 | 0 |

| Cash Pool ID | Sweep Amount (USD) | Investment Position Balance | Remaining in DDA |
|---|---|---|---|
| Beginning of processing |  | 1,00,000.00 |  |
| Sweep 1 | 30,000.00 | 70,000.00 | 0.00 |
| Sweep 2 | 20,000.00 | 50,000.00 | 0.00 |
| Sweep 3 | 10,000.00 | 40,000.00 | 0.00 |
| Sweep 4 | 30,000.00 | 10,000.00 | 0.00 |
| Sweep 5 | 11,000.00 | 0.00 | 1,000.00 |


##### Processing of Maintenance Sweeps

When the Main Master Account (also known as DDA Account/Main Account/Master Account/Checking Account) has deficit, the deficit amount is transferred from the Investment Account to Main Master Account.

The amounts swept in and out of the Investment Account can be restricted by defining the values in Min Redemption Amt and Max Redemption Amt fields in AC.SWEEP.CONDITIONS .

When taking into account the Min Redemption Amt , and the DDA account fulfills its specified criteria.

DDA Account Balance: USD - 3,000.00

Investment Account Balance: USD 4,000.00

Minimum Redemption Amt = USD 1,000.00

Minimum Balance = USD 1,000.00

The DDA account has a deficit of USD 4,000.00. As this exceeds the minimum redemption amount (USD 1,000.00), the sweep are executed and accounting entries are generated as below.

Dr Investment Account USD 4,000.00

Dr Sweep Susp Account USD 4,000.00

Cr DDA Account USD 4,000.00

When taking into account the Min Redemption Amt , and the DDA account does not fulfills its specified criteria.

DDA Account Balance : USD 200.00

Investment Account Balance: USD 4,000.00

Minimum Redemption Amt = USD 1,000.00

Minimum Balance = USD 1,000.00

The DDA account has a deficit of USD 800.00. Since this is less the minimum redemption amount (USD 1,000.00), the sweep is not be executed and accounting entries are not generated.

When taking into account the Max Redemption Amt , and the DDA account fulfills its specified criteria.

DDA Account Balance : USD -100,000.00

Investment Account Balance: USD 400,000.00

Minimum balance = USD 1,000.00

Max Redemption Amount = USD 100,000.00

Partial Transfer = Yes

The DDA account has a deficit of USD 101,000.00. As this exceeds the maximum redemption amount (USD 100,000.00), the sweep is executed and accounting entries are generated as below.

Dr Investment Account USD 100,000.00

Dr Sweep Susp Account USD 100,000.00

Cr DDA Account USD 100,000.00


##### Processing of Combo Sweeps

Combo sweeps is a combination of LoC and Investment Accounts. Currently, combo sweeps support multiple LoCs to be attached in a single cash pool, but only one investment account.

Here, apart from the main master account, the drawing balance of the loan account is also repaid when there is sufficient funds in the Main Master/Investment Account

|  | DDA BALANCE | INVESTMENT MIN/MAX AMOUNT | INVESTMENT BALANCE | INVESTMENT INCREMENT | LOC COMMITMENT BALANCE | LOC DRAWINGS BALANCE | LOC AVAILABLE | LOC MIN/MAX AMOUNT | LOC INCREMENT |
|---|---|---|---|---|---|---|---|---|---|
| TRANSACTIONS | 125,000.00 | 10,000.00 | 150,000.00 | 10,000.00 | 1,500,000.00 | -500,000.00 | 1,000,000.00 | 3,000.00 | 1,000.00 |
| -122,000.00 |  | -150,000.00 |  |  | 122,000.00 |  |  |  |  |
| 150,000.00 |  |  |  |  | 150,000.00 |  |  |  |  |
| -150,000.00 |  |  |  |  |  |  |  |  |  |
| ENDING BALANCE | 3,000.00 |  | 0.00 |  |  | -228,000.00 | 1,272,000.00 |  |  |

|  | BALANCE IN MAIN ACCOUNT | INVESTMENT MIN/MAX AMOUNT | INVESTMENT BALANCE | INVESTMENT INCREMENT | LOC COMMITMENT BALANCE | LOC DRAWING BALANCE | LOC AMT AVAILABLE | LOC MIN/MAX AMOUNT | LOC INCREMENT |
|---|---|---|---|---|---|---|---|---|---|
| TRANSACTIONS | -1,573,000.00 | 10,000.00 | 1,000,000.00 | 10,000.00 | 5,000,000.00 | 0.00 | 5,000,000.00 | 10,000.00 | 100.00 |
| 1,000,000.00 |  | -1,000,000.00 |  |  |  | -590,000.00 |  |  |  |
| 590,000.00 |  |  |  |  |  |  |  |  |  |
| ENDING BALANCE | 17,000.00 |  | 0.00 |  |  | -590,000.00 | 4,410,000.00 |  |  |


##### Processing of Sweep Suspension and Cancellation

Transact offers the capability to pause/revoke the sweep for single link account in a cash pool record. This is done by giving values in the fields Link Suspension Start date , Link Suspension End Date and Link Sweep Cancel Date of the cash pool record. The sweep would be inactive from the start date until the end date.

When the sweep for an investment account is suspended or cancelled, the balances in the money market account or working capital account is reverted to the main account. An entry would be recorded to debit the investment account and credit the main account. Any accrued interest is disbursed to the main account during the next interest payment frequency. If the cash pool contains additional link accounts, such as LoC, current or savings account, the sweep proceeds as anticipated for those accounts.


##### Multi-Pass

In a multi-tiered sweep structure, if the master account doesn't possess sufficient funds to address the overdrafts of its subordinate accounts, a decision might be reached to allocate funds to cover a segment of these overdrafts, known as the non-returnable amount. If there are still funds available in the master account after addressing the non-returnable amounts, they can be assigned to cover the returnable balances of the accounts, following the prescribed sequence.

To process a multi pass,

- If the overall debit is lesser than the overall credit (inclusive of the projected sweep into the master account), standard sweeping happens.
- Conversely, if the overall debit exceeds the overall credit (including the projected sweep into the master account), sweeps are performed with multipass functionality. Retrieve the details of the returnable balance for all accounts within the group and calculate the non-returnable balance. If the booked balance is either in credit or exceeds the returnable balance for the day, the non-returnable balance is considered zero. However, if the booked balance is in debit and is less than the Returnable Balance, the non-returnable balance is calculated as the difference between the booked balance and the returnable balance for the specified booking date. Total funding required and the available balance are then determined. Based on the available balance, funds are allocated according to the predefined sequence within the cash pool group. All the accounts should be zero balance accounts. Non-returnable balances are deducted first in accordance with the defined sequence. If there is still an available balance, returnable balances are then allocated. Next, identify parent sub-accounts and calculate the total sweep amount. Finally, execute the sweep based on the total sweep amount calculated.


#### 📋 Tasks

Related topics:

- Configuring Investment Sweeps

There are no Tasks available for Investment Sweeps feature.


#### 📊 Outputs

There are no Outputs available for Investment Sweeps feature.


> **Related Applications:** `AA.PROPERTY`, `AC.ACCOUNT.SWEEP.HIST`, `AC.BALANCE.TYPE`, `AC.CASH.POOL`, `AC.SWEEP.CONDITIONS`, `AC.SWEEP.TYPE`, `CURRENT.ACCOUNT`, `EXTERNAL.ACCOUNT`, `INVESTMENT.ACCOUNT`, `STMT.ENTRY`

---


### 2.4  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *Cash Management or Cash Pooling The companies employ a cash management technique to hold funds at financial institutions. Cash pooling allows companies to combine their credit and debit positions in various accounts into one account, and includes techniques, such as notional cash pooling and cash co...*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- APIs
- Temenos Transact Services
- System Maintained Files

Cash Management or Cash Pooling The companies employ a cash management technique to hold funds at financial institutions. Cash pooling allows companies to combine their credit and debit positions in various accounts into one account, and includes techniques, such as notional cash pooling and cash concentration. is a financial management strategy that allows companies to maximise both the current credit and debit positions, so that a corporation receives the most benefit from those positions.

The cash pooling module in Temenos Transact supports both physical and notional pooling.

- Physical pooling brings together the balances in nominated accounts to a target account. This allows companies to manage the surplus The amount of an asset or resource that exceeds the portion that is utilised. A surplus is used to describe many excess assets including income, profits, capital and goods. It often occurs in a budget (when expenses are less than the income taken in) or inventory (when fewer supplies are used than retained). cash more efficiently. It gives the customer the ability to internally finance any deficit thereby avoiding additional expenses.
- Notional Pooling Notional cash pooling lets the company combine the balances of several accounts in order to limit low balance or transaction fees. Cash concentration or zero balancing lets the company physically combine various accounts into one single account. allows banks to offer corporate customers the ability to pool funds from various accounts without any physical movement of funds between the accounts. The balances are brought together notionally into a single pool account to calculate the interest. The interest earned in this pool account is redistributed amongst the customers' accounts.


##### Configuring Cash Pooling

Cash Pooling has no specific configuration to be set up at the parameter level.


##### Illustrating Model Parameters

The following parameter tables are available in Model Bank:

| S.No. | Parameters | Description |
|---|---|---|
| 1. | AC.SWEEP.TYPE | This parameter table is used to create rules for various sweep types. Multiple AC.SWEEP.TYPE records can be created with many combinations of rules for each sweep type. |
| 2. | ACCOUNT.CLASS | To set up Notional Pooling, the ACCOUNT.CLASS records such as ICASUSPCR and ICASUSPDR must exist in the system. ICASUSPCR is used for credit interest postings ICASUSPDR is used for debit interest postings |
| 3. | ICA.HIERARCHY.PARAMETER | This must be setup before building any hierarchy in the system. Here, the record ID is the COMPANY code. This record contains the category and transaction codes for all possible types of Notional Pooling interest postings. |


##### Illustrating Model Products

Cash Management is a financial management strategy that allows companies to maximise both the current credit and debit positions so that a corporation receives the most benefit from those positions. PO Module supports the below products:

| S.No. | Product Name | Features |
|---|---|---|
| 1. | Balance Netting Pool | Enables Corporates to manage their funds in an efficient and effective manner. Helps creation of a pool with relevant accounts, such as: Currency Top Account (CT) Master Account (MA) Currency Summary Account (CS) Summary Account (SA) Transaction Account (TR) Mirror Transaction Account (MTR) Credit and debit transactions within the cash pool are transparently diverted to the respective Currency Top Account. Such intra cash-pool transactions include: account-to-account transfers standing orders sweeps |
| 2. | Notional Pooling | Allows banks to offer corporate customers the ability to pool funds from different accounts without physical movement of funds. The balances are brought together notionally into a single pool account to calculate the interest. The interest earned in this pool account is redistributed among the customers' accounts. |
| 3. | Transactional Pooling | Physical Pooling helps in bringing together the balances of nominated accounts into a target account. Cash flow supports the following types of poolings: Maintenance Surplus Two Way Cash flow Create cash pool record checking the actual rules to see whether transfer of funds needs to be made from one account to another. Transaction Pooling can be run online or during the COB using overdraft Limits. |

---


### 2.5  Notional Pooling


> **📇 Quick Reference Card**
> 
> **Purpose:** *Notional pooling allows banks to offer corporate customers the ability to pool funds from various accounts without any physical movement of funds between the accounts. The balances are brought together notionally into a single pool account to calculate the interest. The interest earned in this pool ...*
> 
> **Key Fields:** *Account Capitalisation*, *Account Distribution Type*, *Account No*, *Cr Adj Categ, Cr Adj Txn Pl and Cr Adj Txn Ac*, *Cr Category*, *Cr Txn Code Ac*, *Cr Txn Code Pl*, *Create Group Main Account* ... +17 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Notional pooling allows banks to offer corporate customers the ability to pool funds from various accounts without any physical movement of funds between the accounts. The balances are brought together notionally into a single pool account to calculate the interest. The interest earned in this pool account is redistributed amongst the customers' accounts.


#### ⚙️ Configuration

Simple notional pool has main and sub accounts.

The below screenshot has two sub accounts and one main account. Each account earns interest and it is calculated and processed under the normal interest and charges calculations. Additional interest is earned in a notional pool by pooling the balances of the accounts and calculating interest using the main account's interest rate.

The difference between the amount of interest earned by three accounts and the pool as a group is the group difference. This group difference is re-distributed amongst the pool.


##### Parameters and Files used in Notional Pooling

Notional pooling uses the following parameters or applications:

The below ACCOUNT.CLASS records should exist in the system for notional pooling to be setup and are used for:

- ICASUSPCR – Credit interest postings
- ICASUSPDR – Debit interest postings

> **⚠️ Note:** The setup can be similar to SUSPCR and SUSPDR records or can have their own category codes.

| Field Name | Description |
|---|---|
| Dr Category | Identifies the category code assigned to the profit and loss debit entries generated, as a result of notional pooling. |
| Dr Txn Code Pl | Specifies the transaction codes for debit entries to profit and loss. |
| Dr Txn Code Ac | Specifies the transaction codes for debit entries to the customer accounts. |
| Dr Adj Categ, Dr Adj Txn Pl and Dr Adj Txn Pl | Specifies the debit adjustment entries. |

This record is entered before a notional pool is created. This record describes the hierarchy and defines the main account of the top level group of the hierarchy.

| Field Name | Description |
|---|---|
| Ica Main Account | Defines the main account in a notional pool hierarchy (to which this account belongs). A hierarchy consists of linked groups of accounts. Each group contains a main account along with an unlimited number of sub accounts. System populated field. A sub account in one group can be a main account in a lower level group. There can be an unlimited number of groups in a hierarchy. |
| Ica Main Acct Ind | When this field is set to Yes, it indicates that this account is the main account of the group. |
| Ica New Main Acc | Used to enter the main account that this sub account is linked to. A main account must also be linked to itself. It is used in conjunction with the Ica Start Date field . The Ica Start Date is the date on which this account joins the notional pool. |
| Ica Add Remove | Adds or removes an account to a hierarchy. |
| Ica Main Acct and Ica Main Date | Contain a historical list of main accounts and the start dates for the links to the main account are listed in chronological order starting with the most recent System maintained fields |

The below examples enables the user to understand,

The below screenshot shows top account fields and their corresponding values:

On authorisation, the system populates the below fields:

- Ica New Main Acc – 85804
- Ica Start Date – 2018/04/18

The following screenshot shows sub account fields and their corresponding values:

On authorisation, the system populates the below fields:

- Ica New Main Acc – 85804
- Ica Start Date – 2018/04/18


#### 📋 Tasks

Related topics:

- Execute Intra-Day Sweep (Transactional Pooling)
- Create Sub Account (Notional Pooling)
- Accounts and Deposits Processes (Corporate)

Notional Pooling allows bank to offer corporate customers the ability to pool funds from various accounts without any physical movement of funds between the accounts.

The balances are brought together notionally into a single pool account to calculate the interest. The interest earned in the pool account is redistributed among the customer’s accounts.


##### Workflow

The user can process the notional pooling by using the below workflow:

This menu allows the user to create a group for which the account is going to be a top account.

To create a group hierarchy, follow the below steps:

1. Group Hierarchy .
2. In the Contract Screen, select the Name of the Hierarchy from the Group Hierarchy field and then click the Edit icon.
3. Select an account from the Top Account field.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.

This menu allows the user to create a group main account by setting the Account Distribution Type field as either Interest or Ratio.

To create a group main account, follow the below steps:

1. Main Account .
2. In the Account Details screen, select the Customer Number from the Customer field and enter a value in the Account No field and then click the FIND button.
3. In the Account Details screen, click the Create Group Main Account icon.
4. In the Create Group main Account screen, select the account from the New Main Account field and set the value for the Account Distribution Type field.
5. Click the Validate icon to check for the errors and overrides.
6. Click the Commit icon to submit the record.

This menu allows the user to create a sub account and link it to main accounts.

To create a sub account, follow the below steps:

1. Sub Account .
2. In the Account Details screen, select the Customer Number from the Customer field and enter a value in the Account No field and then click the FIND button.
3. In the Account Details screen, click the Create Notional Subaccount icon.
4. In the Create Sub Account screen, enter values in the following fields and other required fields. New Main Account Distribution Ratio
5. Click the Validate icon to check for the errors and overrides.
6. Click the Commit icon to submit the record.

This menu allows the user to remove the sub account link from the main account.

To remove the sub account link from the main account, follow the below steps:

1. Remove Sub Account .
2. In the Account Details screen, select the Customer Number from the Customer field and enter a value in the Account No field and then click the FIND button.
3. In the Account Details screen, click the Remove Sub Account icon to remove the sub account link from main account.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.

This menu allows the user to authorise or delete the unauthorised notional pool main accounts.

To authorise the unauthorised notional pool main accounts, follow the below steps:

1. Main Account .
2. In the Unauthorised Notional Pool Main Accounts screen, click the Authorise icon to authorise the unauthorised notional pool main accounts.
3. Verify the transaction details and then click the Authorise icon to commit the authorisation.

To delete the unauthorised notional pool main accounts, follow the below steps:

1. Main Account .
2. In the Unauthorised Notional Pool Main Accounts screen, click the Delete icon to delete the unauthorised notional pool main accounts.
3. Click the Delete icon to commit the authorisation.

This menu allows the user to authorise or delete the unauthorised notional pool sub accounts.

To authorise the unauthorised notional pool sub accounts, follow the below steps:

1. Sub Account .
2. In the Unauthorised Notional Pool Sub Account screen, click the Authorise icon to authorise the unauthorised sub accounts.
3. Verify the transaction details and then click the Authorise icon to commit the authorisation.

To delete the unauthorised notional pool sub accounts, follow the below steps:

1. Sub Account .
2. In the Unauthorised Notional Pool Sub Account screen, click the Delete icon to delete the unauthorised sub accounts.
3. Click the Delete icon to commit the deletion.

This menu allows the user to authorise or delete the unauthorised removal of sub account link.

To authorise the unauthorised removal of sub account link, follow the below steps:

1. Authorise/Delete remove sub account link .
2. In the Unauthorised Removal of Sub Account Link screen, click the Authorise icon to authorise the removal of sub account link records.
3. Verify the transaction details and then click the Authorise icon to commit the authorisation.

To delete the unauthorised removal of sub account link, follow the below steps:

1. Authorise/Delete remove sub account link .
2. In the Unauthorised Removal of Sub Account Link screen, click the Delete icon to delete the removal of sub account link records.
3. Click the Delete icon to commit the deletion.

This menu allows the user to set the capitalisation frequency for an account. The Interest Computation Account (ICA) group interest is calculated based on the interest conditions pertaining to the main account of the group and posted during capitalisation of the same.

To set the capitalisation frequency, follow the below steps:

1. Account Capitalisation .
2. In the Contract screen, select an Account ID from the Account Capitalisation field and then click the Edit icon.
3. In the Account Capitalisation screen, click the Click to Update frequency icon to set the frequency pattern and set the value for the Start of Day Capitalisation field.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.

This menu allows the user to set the interest conditions for an account.

To set the interest conditions for an account, follow the below steps:

1. Account Credit Interest .
2. In the Contract screen, select an Account ID from the Credit Interest for an Account field and then click the Edit icon.
3. In the Credit Interest for an Account screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.


#### 📊 Outputs

Notional Pooling allows bank to offer corporate customers the ability to pool funds from various accounts without any physical movement of funds between the accounts.

The balances are brought together notionally into a single pool account to calculate the interest. The interest earned in the pool account is redistributed among the customer’s accounts.


##### Enquiries and Reports

This section helps the user to view the notional pooling accounts hierarchy and beneficiary interest.

Notional Pool Accounts Hierarchy

This enquiry allows the user to view the list of accounts which are formed as a group for notional pooling along with their interest compensation account hierarchy details. The user can view the notional pool accounts details by clicking the ICA Group Details icon.

View beneficiary interest

This enquiry displays the list of sub accounts under a main account, their earning as a group, and their distribution among the sub accounts as per the methods chosen (Ratio or Interest) in the notional pooling hierarchy.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


### 2.6  Overdraft Protection


> **📇 Quick Reference Card**
> 
> **Purpose:** *Temenos Transact Overdraft Protection (ODP) is the functionality that enables banks to extend the option to their customers of authorising debit transactions even when there are insufficient funds in their checking account or corporate cash pool. This feature mitigates overdraft fees by automaticall...*
> 
> **Applications:** `AC.ACCOUNTING.PARAM`, `AC.CASH.POOL`, `AC.CP.GROUP.PARAM`, `AC.CREDIT.CHECK`
> 
> **Key Fields:** *Balance To Use*, *Drop Credit Reservations*, *Main Master*, *No Hierarchy Reqd*, *Reserve Sweep Projections*, *Shared Balances*, *Sweep Debit Reservations*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Temenos Transact Overdraft Protection (ODP) is the functionality that enables banks to extend the option to their customers of authorising debit transactions even when there are insufficient funds in their checking account or corporate cash pool. This feature mitigates overdraft fees by automatically transferring funds from linked funding accounts such as Current or Checking Accounts, Lines of Credit, Savings, or Deposit Accounts.

The ODP conducts real-time balance checks and reserves the available funds on the funding accounts, that is, when a customer initiates a transaction that overdraws the checking account or the cash pool, the system assesses the available funds across connected funding accounts, places a lien on the available funds to extent of funds required to cover the overdraft on the transaction account as a part of the online transaction processing, ensuring customers are informed about their current balance status and potential overdraft situations.

However, the actual movement of funds from the funding account to the cash pool or the checking accounts is managed by the standard Temenos sweeping functionality provided by the Cash Pooling module. The ODP sweeps are run during the Transact COB.

The table below explains the types of funding accounts that supports ODP.

| Funding Accounts | Accounts Belong to | Pre-requisites in Accounts |
|---|---|---|
| Savings Accounts | Arrangement Accounts (AR) Product Line | Follow Component-based credit check processing |
| External Line of Credits | External Accounts (XP) Product Line | Configure Commitment Balance and Drawings Balance types |
| Investment Accounts | Arrangement Accounts (AR) Product Line | Configure Memo or Internal balance types Follow Component-based credit check processing |
| Line of Credits | Arrangement Loans (AL) Product Line | Configure Commitment Balance and Drawings Balance types |

> **⚠️ Note:** The primary role of ODP sweep projections is to prevent the overuse of balances on Funding Accounts, especially when the same funding source is linked across multiple ODP sweeps covering multiple checking accounts or cash pools. The availability of funds for direct withdrawal from funding accounts depends on the balance rules defined within the funding arrangement. These rules determine how funds are allocated and utilized across different accounts or cash pools, thus impacting the potential for direct fund withdrawal in various scenarios.

The following are the highlights of the ODP.


##### ODP from Multiple Sources

ODP facilitates funding from multiple sources. For example, checking an account that receives funding from both a savings account and a line of credit account for ODP in Retail. Similarly, an investment account and a line of credit account for ODP in Corporate funds a cash pool. Moreover, the same funding account can provide funds for multiple cash pools, or the same savings account can fund more than one checking or current account.


##### Sweep Groups

A sweep group identifies a set of linked accounts, belonging to the same customer in retail contexts or representing a cash pool in corporate scenarios. It establishes a structured sequence by determining the priority for allocating funds among checking accounts or cash pools. The grouping of checking and funding accounts into a single group under the Many-to-Many funding block is shown in the diagram above.


##### Real-time Sweep Projections

When the checking account or cash pool groups lack sufficient balance to cover a debit transaction, the system automatically considers the funds available in linked accounts. It reserves these funds as sweep projections before allowing the system to post the transaction thereby reducing the risk of funds being withdrawn from the linked accounts.


##### Real-time Adjustment of Sweep Projections

This ensures a dynamic response to changes in the checking account or cash pool groups. When the account receives funds, the system automatically drops or adjusts any sweep projections against the linked accounts. This allows the customer to access the funds in the linked accounts promptly, offering flexibility and efficient fund utilisation.


#### ⚙️ Configuration

This topic covers the system-level and product-level configurations required for enabling Overdraft Protection (ODP) feature.


##### Enabling ODP for Retail Accounts

As a prerequisite, to enable ODP for Retail accounts like checking or current accounts, set-up a sweep group by defining Shared Balances as Accounts and No Hierarchy Reqd as Yes in AC.CP.GROUP.PARAM .

- It is not mandatory to define Main Master .
- When Balance To Use is not defined, by default the configurations defined at the level of Sweep Type take precedence.
- The sweep group is a one-time definition, that is, when a customer links another checking or current account to funding accounts for ODP, the sweeps can be defined under the same sweep group.

The checking or current accounts must be included in a maintenance style sweep using AC.CASH.POOL in order to link one or more funding accounts, such as a savings account or a line of credit.


##### Enabling ODP for Cash Pools

As a prerequisite, to enable ODP for Corporate cash pools, set-up a sweep group by defining Shared Balances as Pool Balance in AC.CASH.POOL .

- It is mandatory to define Main Master .
- When Balance To Use is not defined, by default the configurations defined at the level of Sweep Type take precedence.
- Each cash pool requires a separate sweep group.

The Main Master account of the cash pool must be included in a maintenance or a surplus or two-way style sweep using AC.CASH.POOL in order to link one or more funding accounts, such as an investment account or a line of credit.

Read the Physical Pooling section for more information on the creation and maintenance of sweeps.


##### Enabling Real-time Sweep Projections

By default, the system allocates the funds on the linked accounts against the overdraft allowed on the transaction accounts as a part of ODP. To disable the allocation of funds on the linked accounts, the user must set Reserve Sweep Projections as Disable in AC.ACCOUNTING.PARAM .


##### Enabling Overdraft Protection for Debit Holds or Reservations

To enable the Overdraft Protection feature for Debit Holds or Reservations, the user must set Sweep Debit Reservations to any of the values in AC.ACCOUNTING.PARAM as given below.

- Active – Funds are reserved on the funding account for the Active Debit Reservations, that is, the reservations with a start date as the current day or less than the current day.
- All – Funds are reserved on the funding account for all Debit Reservations including future-dated debit reservations.
- None (default) – No funds are reserved on the funding account as sweep projections.

If the user modifies the configuration, the same is applied for subsequent debit holds/reservations.

> **⚠️ Note:** Sweep Debit Reservations can be set as Active or All only if Reserve Sweep Projections is not set as Disable.


##### Drop or Adjust Sweep Projections Against the Credit Holds or Reservations

To enable the system to automatically drop or adjust sweep projections against the credit holds or reservations posted to the checking account, the user must set Drop Credit Reservations in AC.ACCOUNTING.PARAM as any of the below values.

- Active – Sweep projections on the funding account are dropped or adjusted only against the active credit reservations posted to the sweeping account. Active refers to the reservation with the start date as the current date.
- All – Sweep projections on the funding account are dropped or adjusted against the credit reservations posted to the sweeping account including future-dated credit reservations.
- None (default) – Sweep projections on the funding account are not dropped or adjusted based on the credit reservations posted to the sweeping account.

If the user modifies the configuration, the same is applicable only for subsequent credit holds/reservations.

> **⚠️ Note:** Drop Credit Reservations can be set as Active or All only if Reserve Sweep Projections is not set as Disable.


##### Credit Check Configuration for Enabling Overdraft Protection

Temenos Transact allows the bank to define a group of balance components using AC.CREDIT.CHECK to determine the funds available on the account, that are used in the funds check process. To consider funds available in the linked accounts during the funds check process on the checking accounts, the SWEEP component must be included in the credit check balance components group. Read Balance Components – AC.BALANCE.COMPONENT and Configuring the Available Balance – AC.CREDIT.CHECK to learn more about including the SWEEP component.

The user must link the credit check group created using AC.CREDIT.CHECK to respective transaction activities by configuring the accounts product conditions as shown below.


#### 📋 Tasks

There are no Tasks available for Overdraft Protection feature.


#### 📊 Outputs

There are no Outputs available for Overdraft Protection feature.


> **Related Applications:** `AC.ACCOUNTING.PARAM`, `AC.CASH.POOL`, `AC.CP.GROUP.PARAM`, `AC.CREDIT.CHECK`

---


### 2.7  Physical Pooling


> **📇 Quick Reference Card**
> 
> **Purpose:** *Physical pooling brings together the balances in the nominated accounts into a target account. This allows companies to manage the surplus The amount of an asset or resource that exceeds the portion that is utilised. A surplus is used to describe many excess assets including income, profits, capital...*
> 
> **Applications:** `AC.ACCOUNT.SWEEP.HIST`, `AC.CASH.POOL`, `AC.CASH.POOL.LINK`, `AC.CP.GROUP.PARAM`, `AC.CREDIT.CHECK`, `AC.SWEEP.CONDITIONS`, `AC.SWEEP.TYPE`, `EB.CONTRACT.BALANCES` ... +1 more
> 
> **Key Fields:** *Acct Mode*, *Adjustment*, *Aggregate Bal*, *Allocate Sweep Amount*, *Amount Routine*, *Amt Sweep Routine*, *Back Value Adjustment*, *Back Value Capitalisation* ... +123 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Physical pooling brings together the balances in the nominated accounts into a target account. This allows companies to manage the surplus The amount of an asset or resource that exceeds the portion that is utilised. A surplus is used to describe many excess assets including income, profits, capital and goods. It often occurs in a budget (when expenses are less than the income taken in) or inventory (when fewer supplies are used than retained). cash efficiently. It gives the customer the ability to internally finance any deficit thereby avoiding additional expenses.

A pool is setup to move funds automatically from one specified account to another when certain conditions on the account are met. This supports four types of pooling:

- Maintenance pool – Maintains a balance at a given level. When the balance in an account falls below a minimum amount, funds are pooled from feeder accounts to the designated account to maintain the minimum balance.
- Surplus pool – Moves excess funds from an account where the account balance goes above the maximum amount that is specified.
- Two-way pool – It is a combination of a maintenance and surplus. Money moves from one account to another account that has fallen below the minimum balance. Or money can be paid from the account if it has surplus funds over the maximum balance.
- Cash-flow pool – It is same as the two-way pool however, the amount of funds that can be returned to an account is restricted.

> **⚠️ Note:** Physical pooling is run online or during the Close of Business (COB) and it makes use of overdraft limits.


##### Back-value Dated Sweeping

Backdated sweeping allows the system to post sweep transactions based on value date. The user can setup sweep transactions between accounts, which can be run multiple times based on value dated balance. When the sweeping account receives multiple value-dated (back or future dated) transactions, the system splits the transactions based on the value date and sweeps the amount to the master account. Once the back-value dated transactions are posted through sweeping process, the interest recalculation is applied automatically.

Account upload order functionality allows users to set target balances for maintenance sweeps. When the account balance falls below the target amount, the account is funded (by debiting the Master account) to maintain the target balance. This allows top-up of sweeping account for a specific limit.


##### Sweeping Suspension Based on Account Blocking (Debits/Credits)

The user can restrict the sweep by updating the suspension sign in cash pool record. When the account is blocked for debit or credit, the sweep transactions are also blocked. Sweep block sign is done manually in cashpool records or automatically using Local routine. When the account is unblocked, the sweeping record is manually removed to process the sweeps.


##### Locked Amount with Sweep per Value Date

Cashpool application considers the locked amount and the remaining amount is swept to the master account with split per value date. When the account has back-value dated transactions, the system considers the locked amount to process the sweep with split per value date. The system maintains the locked amount in the respective account sweep history, regardless of the sweep processing. Temenos Transact considers the current date locked amount for the current value dated transactions.


##### Understanding External Corporate Sweeps

The external corporate sweeps allow the user to define corporate sweep transactions between Transact accounts and external accounts. This functionality helps corporates automatically sweep the funds from Transact to other financial institutions without manual intervention. When the system executes the sweep, it generates the payment order for the sweep amount.


#### ⚙️ Configuration

Physical pooling uses the following parameters and tables:

The AC.SWEEP.TYPE , AC.SWEEP.CONDITIONS AC.CP.GROUP.PARAM , AC.CASH.POOL and INTRA.DAY.SWEEP applications are used to setup the physical pooling. The system updates AC.CASH.POOL.LINK , AC.ACCOUNT.SWEEP.HIST and EB.CONTRACT.BALANCES files with pooling information.

The Use Limits field in AC.SWEEP.TYPE checks the overdraft limit set on an account. Allowed values are Yes or No. When set to:

- Yes – Limit attached to the overdraft account is checked.
- No – Disregards any limit in the overdraft account.

The system supports two methods of calculating the pool amount locally. In both cases, a local routine is attached to the AC.SWEEP.TYPE record, using the Amt Sweep Routine field.

- When the Rtn With Sw Amt field is set to Yes, Temenos Transact calculates the pool amount and then the local routine applies a local calculation to the Temenos Transact calculated pool amount, and then returns the local pool amount.
- When the Rtn With Sw Amt field is set to No, the local routine calculates the pool amount.

The routine has five parameters:

- Account balance of the TO account before the sweep amount is calculated, along with the TO account ID
- Account balance of the FROM account before the sweep amount is calculated, along with the FROM account ID
- Sweep amount with the appropriate sign
- Cash pool link record
- Value date of the sweep transaction

> **⚠️ Note:** The third parameter, sweep amount is used by the called routine for further validation as per the client's local requirements, and is passed back to the system for raising the sweep transaction.

- When the Return At Sod field is set to Yes, the amount transferred during the COB activity using cash pooling is returned to the same account during the next start of day (SOD) operation with the SOD value date.
- This functionality is not available when the Back Value Adjustment field is set to Yes, in the AC.CP.GROUP.PARAM record.

The two balance types in the Balance to Use field in the AC.SWEEP.TYPE application are:

- Booked Less Locked – Deducts the locked amount from the online actual balance.
- Booked With Fwd Less Locked – Deducts the locked amount from the online actual balance and in addition considers all forward entries.

> **⚠️ Note:** The system uses these balance types when calculating the amount to be swept.

This field in the AC.SWEEP.TYPE application allows the user to set whether the system should makes a partial transfer (and not the whole amount) when there are insufficient funds in the funding account, instead of not executing the sweep transaction.

Maximum concentration cap or insufficient available funds.

The user allows overdrafts on the account using the Acct Mode field, which are not memo type. This field can be set to Sao or Snp. When set to:

- SAO –The system accepts overdrafts and the necessary amount is moved even when the account gets overdrawn.
- SNP – The system rejects the overrides encountered while executing a sweep and does not process the sweep. The rejected sweep is stored in AC.ACCOUNT.SWEEP.ERROR .

> **⚠️ Note:** This is applied for both maintenance and surplus sweep irrespective of the options selected in the Partial Transfer field.

The AC.SWEEP.TYPE application defines the sweep types used in a sweep record. The balance of the entire cash pool or the currency position is considered when the system triggers the sweeping transaction.

The Pool Sweep field accepts Cash Pool, Currency or Null as values. When set to:

- Null – The system considers the balance of the sweeping account (the account in the AC.CASH.POOL record ID) as sweeping criteria, when the sweeping transaction is triggered.
- Cash Pool – The system considers the balance of the entire cash pool, when the sweeping transaction is triggered. In the case of balance netting pool, the system considers relevant balances of all currency top accounts of the cash pool re-calculated. The currency of the sweeping TR account uses bank exchange rates existing in the system at the time of the transaction execution.
- Currency – The system uses this option when the purpose of the sweep is to move a specific currency position of the cash pool. This option is only applicable to balance netting pool. When this option is chosen in the balance netting pool, the system only considers the balance of the currency top account opened in the currency of the sweeping transaction account in sweeping criteria.

A maintenance sweep record type is created in the system, where the Pool Sweep field is set to Currency.

This functionality helps in configuring the system to perform zero-balancing sweeps in two ways:

- Sweeping the booked balance in one single tranche
- Sweeping the booked balance in multiple tranches (split per value date)

These options can be setup at the paratmeter level of the AC.SWEEP.TYPE application. The Zero Balancing field has the following options:

- Per Value Date
- Per Booking Date
- None

On selecting,

- Per Value Date – The total of all transactions booked since the previous run is swept in multiple tranches per each value date.
- Per Booking Date or None – The total of all transactions booked since the previous sweep run is transferred in a single tranche.

To setup a zero balancing sweep,

Set the Zero Balancing field in AC.SWEEP.TYPE application to Per Value Date and set the Balance to Use field as Online Actual.

Zero Balancing Sweep – Cover Control

In zero balancing, when the system performs cover control on the concentration account, all sweeping transactions that are split per value date are netted together.When cover control is switched on as a result of the entire transaction execution, the concentration account is in breach of the cover control conditions and the entire transaction is suppressed.

This field specifies the configuration to calculate the debit holds and credit holds when the Balance to use field is configured as ‘Booked Including Reservations’.

Sweep Reserve Condition can be set as 'Lock Funds Date' and 'Credit Reserve Date'.

Lock Funds Date - Indicates that only Active (Today) debit reservations or debit-locked events are considered for calculating the available or usable balance of the sweeping account.

Credit Reserve Date - Indicates that only Active (Today) credit reservations or credit-locked events are considered for calculating the available or usable balance of the sweeping account.

When Sweep Reserve Condition is not configured, then the system considers the minimum of credit reservations and the maximum of debit reservations of the sweeping account.

This field specifies the configuration on the level of AC.SWEEP.TYPE named ‘Funding Account Balance’ with two options:

- ‘Credit Check’ – The available funds in the funding account are calculated according to the criteria specified in the Credit Check.
- ‘None / Null’ – The Working Balance of the funding account is treated as available funds.

This configuration is applicable only for maintenance style of sweeps.

AC.CREDIT.CHECK should be configured with following components and attach the same to the Balance Availability property conditions of the funding account product against the activity for sweep debits.

- Working – Base (Online Cleared/Collected)
- Float – Optional
- Debit Reserve Active – Optional
- Credit Reserve Active – Optional

This field defines the sorting criteria which is applied prior to the execution of the surplus sweeps. This applies only for sweeps involving the investment accounts for a particular investment type. If sorting is required during surplus sweep processing, the sweep amounts are first determined, and subsequently, the sorting occurs based on the specified value in this field. Following the sorting, the sweeps are executed accordingly.

For example, consider a scenario with five cash pool records having surplus sweep amounts of USD 1000, USD 2000, USD 3000, USD 4000, and USD 5000 respectively. If 'Low to High' is chosen, the system executes the sweeps in ascending order of the sweep amount. If 'High to Low' is selected, the system processes the sweeps in descending order of the sweep amount.

This field refers to the Suspense Category to be used:

- For the Loan Products (For example, Line of Credit/Credit Card), where the actual account is maintained outside Transact, any transaction posted against the sweep account is automatically balanced against this Suspense Account
- For Investment Sweeps - Any transaction posted against the customer’s investment account is balanced against the Suspense Account created using the category specified in this field.

A unique category to be used to differentiate between the different loan and investment products.

| Sweeping account | Account C 1 |
|---|---|
| Account A balance | 1000.00 USD |
| Maximum amount | 700.00 USD |
| Rule | Surplus |

The AC.SWEEP.CONDITIONS application captures the boundary conditions and limitations to be applied before executing the sweeps from sweeping account to funding account. The record ID is a Free Text-CCY-Date. Currently, the records are supported in local currency only.

The sweep type for which the conditions are to be applied are mentioned in this field. Sweep Types are multi-valued, so several sweep types could be given to follow the same set of conditions.

Indicates the maximum amount that can be invested in the Investment account on a given day across all the customers participating in the investment. Sum of all the investment amount across all the customers in an investment account on a given day should be less than or equal to the maximum contribution amount.

Indicates the minimum amount that can be invested in the Investment account on a given day across all the customers participating in the investment. Sum of all the investment amount across all the customers in an investment account on a given day should be greater than or equal to the minimum contribution amount.

Indicates the maximum amount that a customer can withdraw from an investment account on a given day.

Indicates the minimum amount that a customer can withdraw from an investment account on a given day.

Indicates the maximum amount that can be swept at a time from the current account to the investment account.

Indicates the minimum amount that can be swept at a time from the current account to the investment account.

Holds the unit amount in terms of which the sweep has to happen.

Indicates the Currency of the Maximum and Minimum Sweep Amount.

This field controls the maximum amount that can be in place on the account. Only allowed with TWO WAY or SURPLUS type sweep rules. The amount mentioned in this field is defaulted in the Minimum Amt field in the cash pool record.

This field controls the maximum amount that can be in place on the account. Only allowed with TWO WAY or MAINTENANCE type sweep rules. The amount mentioned in this field is defaulted in the Minimum Amt field in the cash pool record.

The view of AC.SWEEP.CONDITIONS is shown in the image below.


##### Sweeping Suspension Based on Account Blocking (Debits/Credits)

To suspend the sweep in AC.CASH.POOL , the Susp Sign field should be set as Cr or Dr. When set to,

- Cr – The sweep is suspended by posting credit to sweeping account.
- Dr – The sweep is suspended by debiting the sweeping account.

> **⚠️ Note:** The Susp Start Date and Susp End Date (optional) fields are also set.


##### Locked Amount with Sweep per Value Date

The Balance to Use field is set to ‘Booked Less Locked’ or ‘Working Less Locked Amt’ in AC.CP.GROUP.PARAM to sweep the funds per value date. When the Back Value Adjustment field is set as Adjustment, the validation is removed for ‘Booked Less Locked’ and ‘Working Less Locked’ and the transaction is split per value date and the sweep is executed.


##### Defining Internal Wash Accounts for External Corporate Sweeps

To process the external sweep transactions, the user has to define Po Wash Categ for external sweeps with the internal account category in AC.SWEEP.TYPE . When the user defines this field, Transact allows them to define Beneficiary Id in AC.CASH.POOL to process the external sweeps. If this Po Wash Categ is left blank, Transact prompts an error message if the user provided a Beneficiary Id in AC.CASH.POOL .


#### 🔧 Working With

The below applications are used for sweep transactions:

| Field Name | Amount |
|---|---|
| Cashflow Amount | 100,000.00 |
| Aggregate Bal | 50,000.00 |

| Column 1 | Column 2 |
|---|---|
| Sweeping group ID | The AC.CP.GROUP.PARAM record ID of a specific group, in which the account belongs |
| Master account number | Account set as main master in AC.CP.GROUP.PARAM record |
| Master company time | The server or company time of the account is mentioned in the Main Master field |
| Sweep run time | The run time set in INTRA.DAY.SWEEP record |
| Sweep account number | @ID of AC.CASH.POOL of the sweeping record is set as the sweeping account |
| Sweep account company ID | Temenos Transact company where the sweep account resides |
| Sweep account cut-off time | The cut-off time defined for the sweep account of Temenos Transact companies |
| Link account number | Concentration account of the sweeping record that is set as link account |
| Link account company ID | Temenos Transact company where the link account resides |
| Link account cut-off time | The cut-off time defined for the link account of Temenos Transact companies |

| Date | Account A | Account B | ACCOUNT C |
|---|---|---|---|
| Opening Bal | -1000.00 | 0.00 | 1000.00 |
| 03/03/02 | -2000.00 | 1000.00 | 3000.00 |
| 04/03/02 | -2000.00 | -2000.00 | -2000.00 |
| 05/03/02 | 1000.00 | -3000.00 | -2000.00 |
| 06/03/02 | 1500.00 | -3000.00 | 1000.00 |
| 07/03/02 | 1500.00 | -3000.00 | -4000.00 |
| 08/03/02 | 1000.00 | -3000.00 | -3000.00 |
| 09/03/02 | -3000.00 | -3000.00 | -3000.00 |
| 10/03/02 | -3000.00 | 5000.00 | -3000.00 |
| 11/03/02 | -3000.00 | 5000.00 | -1000.00 |
| 12/03/02 | -3000.00 | 7000.00 | 0.00 |

All pools processed over an account is recorded in this live table. The ID of the table is

When sweeps are triggered online or during COB, the sweeps are executed first and then the charges are collected separately. When the debit account has sufficient balance to cover only the sweep amount and not the charge amount, the account is overdrawn for the charge amount irrespective of the account mode (Sao or Snp).

When a sweep is executed and the account has sufficient balance to cover only the sweep amount and not the charge amount,

- The PO module is enabled for Transaction Recycler and when the account is, Linked – The account is not overdrawn and the charge details are updated in RC.DETAIL live file Not linked – The accounting is called in SSS mode and the account is not overdrawn, but an internal suspense account is debited

- Transaction Recycler is not enabled for PO module. When the accounting mode in AC.SWEEP.TYPE is: Sao – The account is overdrawn Snp – The sweep is rejected

The AC.CP.SWEEP.CHARGE service must be running when INTRA.DAY.SWEEP is triggered to collect the sweep charges online. Otherwise, the charge details are written to a work file (AC.CP.CHARGE.LIST) and processed during that day’s COB.

Enabling Transaction Recycler for PO module

1. Attach the application name linked to the system ID for PO module in AC.APPLICATION.LINK .

1. Attach the application name in the override record for which the transaction recycler is to be enabled and set the Fwd Acct Mode as SSS.

1. Define a record to PO module in RC.CONDITION table.

1. Attach the system ID of PO module using ACCP in the record AC of RC.CAPTURE with Rc Type field set as IC.CHARGE and RCCondition field as the record ID created earlier, that is, PO.

When a sweep is executed and if the balance in the debit account has sufficient balance to cover only the sweep amount and not the charge amount, then the account is not overdrawn and the charge amount details are updated in a live file, RC.DETAIL . The internal suspense account (formed using the category code defined in RC.CAPTURE ) is debited for the charge amount and PL is credited.

This application defines the accounting mode to be called at the time of execution of sweeps. To cater to this requirement, Acct Mode field in AC.SWEEP.TYPE application is used and this field accepts Sao or Snp as values. When set to:

- Sao – All overrides encountered on execution of sweep is system accepted and the sweep is executed. All the successful sweeps are recorded in AC.ACCOUNT.SWEEP.HIST .
- Snp – When there is any override, the system rejects the sweep. The overrides can be on account of insufficient balance or due to various account level restrictions like post no entries, locked amount.

The details of rejected sweeps are updated in the AC.ACCOUNT.SWEEP.ERROR table.

This file records details of all back value processing.

- It is updated on the account number to be back valued, (the value date of the back value transaction and a sequence number).
- An account can receive more than one back value transaction.
- Each record holds the details of all accounts re-pooled as a result of the original account's new balance.
- The key to CORR.GROUP.CP is held in the account sweep history record of every account included in the back value process, (as many accounts are effected).

The below screenshot shows a CORR.GROUP.CP record for account 18554.

This is a system maintained file and is created when the AC.CASH.POOL record is authorised

- This file records individual rule and specifies the amounts and frequencies
- Changes in the AC.CASH.POOL is updated in this application

Balances within a pool are grouped together for the purpose of balance checking in the case of maintenance pools. The Shared Balances field in the AC.CP.GROUP.PARAM application is used to determine the type of setup. The field accepts any one of the following values:

- Yes – all accounts that are part of the same cash pool group share their available balances to be considered in case of any overdraft during the maintenance sweep. This option can only be used when the Balance To Use field is set as ’Working’.
- Partial – all accounts that are part of the same cash pool group share their available balances to be considered in case of any overdraft during the maintenance sweep. This option can only be used when the Balance To Use field is any balance type, not only 'Working'.
- No or None – balances of the account part of the same cash pool group are not shared.
- Account – the balances are shared only by a child account and the main master account within the group. This option can be used with any balance type, with the exception of Ac Balance Type.

When the balances need to be grouped, a record is created in the AC.SHARED.ACCOUNT application. The ID of this record is the GROUP.ID and all the accounts in the group are recorded here.

If the Account option is selected in the Shared Balances field, the system performs a set of validations:

- In AC.CP.GROUP.PARAM The Balance To Use field should be other than Ac Balance Type The Main Master account entered in the record should not have a 'Limit' attached, which can be shared.
- In AC.CASH.POOL The system does not allow any other sweeping style than Maintenance. Maintenance sweeps should be covered in full. The Partial Transfer field from the AC.SWEEP.TYPE record used in the sweeping record, needs to be set to No, otherwise, the system raises an error message when the sweeping record is created. One Level Cash Pool Sweeping Group in which the funding account (Concentration or Link Account) is the same account as the one set as the Main Master account in the AC.CP.GROUP.PARAM record. The system does not allow the input of multiple funding accounts (link accounts) and input of a funding account which is different from the Main Master account. Maintenance sweeps should be set with an ’every business day’ frequency. If the frequency is set differently, the system raises an error message.

Using this option, when a debit transaction is posted against a sweeping account, the system considers the balance of the Main Master account in the credit check. If the Main Master account has sufficient balance, then the amount which is necessary to cover the deficit of the sweeping account is reserved at the master account level and swept when the sweeping transaction is triggered.

A cash pool group has been set up in the system having a Main Master account 85391 with a balance of 1000 USD.

Two maintenance sweep records have been created to maintain 0 balance in the account 85405 and account 85413. The system covers any deficit of funds of the accounts taking money from the Main Master account. In the AC.CP.GROUP.PARAM application, if the Shared Balances field is set as Yes, it means that the accounts involved in the cash pool group shares their balances.

Two maintenance sweeping records were created in the AC.CASH.POOL application having the Main Master account as Link Account (Concentration Account).

If the Shared Balances field is set as either Yes or Partial

The system updates the Eb Group Id field for each account. This field contains the shared balances group id which is used by the cash pooling functionality during the online overdraft checking to determine if an account (with it set) has additional overdraft checking on other accounts in its group.

After the above setup, the following transactions are posted in the system:

- A funds transfer transaction for Debit 500 USD is posted against the account 85405, making its balance 500 USD in Debit.
- A funds transfer transaction for Debit 1000 USD is posted against the Main Master account 85391.

When the Main Master account is debited, the system considers that a deficit of 500 USD needs to be covered for account 85405 by a maintenance sweep and, in this case, an override message is raised. The override indicates that if the account is debited with 1000 USD, there is an insufficient balance in the cash pool sweeping group for covering the balance deficit in the child account. If the funds transfer record was not authorized, then the Main Master account’s balance remains as 1000 USD.

- A funds transfer transaction for Debit 5000 USD is posted against the account 85413, making its balance 5000 USD in debit.
- A funds transfer transaction for Debit 1 USD is posted against the Main Master Account 85391.

When the Main Master account is debited, the system considers that a deficit of 500 USD needs to be covered for the account 85405 and deficit of 5000 USD for the account 85413 by the maintenance sweeps and, in this case, an override message is raised. The override indicates that if the account is debited with 1 USD, there is an insufficient balance in the cash pool sweeping group for covering the balance deficit in the child accounts.

If the funds transfer record is not authorised, the Main Master account’s balance remains 1000 USD.

- The system runs the sweeps. The Main Master account is debited with 5.500 USD, account 85405 credited with 500 USD and account 85413 credited with 5000 USD.

Consider a cash pool group having a Main Master account 10017233202 with a balance of 1000 USD.

Two maintenance sweep records are created to maintain zero balance in the 10017233203 and 10017233204 accounts. In the AC.CP.GROUP.PARAM application, if the Shared Balances field is set as Account, then the master account shares its balance with the sweeping accounts.

A debit transaction of 500 USD is posted on child account 10017233203. The system checks if there are enough funds taking into consideration its own balance, plus the balance of the master account. As there are enough funds on the Master account, the transaction is posted.

A debit transaction of 400 USD is posted on account 10017233204. The system checks if there are sufficient funds taking into consideration as its own balance and the balance of the master account. The master account has a balance of 1000 USD but 500 USD are reserved by the account 10017233203. So, the available amount is 500 USD. As this is sufficient, the transaction is posted.

The system reserved these amounts at the Master account level as there is sufficient balance to cover the deficit.

When the system triggered the sweeps, the reservations are cleared from the Main Master account and the funds are transferred to the child accounts.

The Master account’s balance becomes 100 USD.

The balance of child account 10017233203 becomes zero as the deficit of 500 USD was covered by the Master account during the sweep.

The balance of child account 10017233204 becomes zero as the deficit of 500 USD was covered by the Master account during the sweep.

When the Account option is selected at the level of the cash pool sweeping group, the system performs a credit check considering the aggregated balances on two levels:

- For the Child accounts within the structure: When performing debit transactions against the child accounts (sweeping accounts) in a maintenance sweep record, if they are part of the same Cash Pool Sweeping Group, the system performs the credit check considering the balances of child and funding accounts.
- For the Main Master account within the structure: When a debit transaction is posted against the Main Master account (concentration account), the system performs the credit check considering its balance, the amount reserved due to debits posted against the child accounts and a Single Overdraft Limit (if available).

When calculating the reservation amount, the system considers the type of balance selected in AC.CP.GROUP.PARAM and the minimum amount to be maintained in the account.

For a cash pool group with the Shared Balances field set to Account, in case any of the child accounts receive a credit transaction after an amount was reserved at the master account level by the same account, the reservation is reduced.

The credit check for the accounts is set to be performed on following balance types:

- Main Master: Booked Balance – Sweep amount
- Account 56789: Booked Balance
- Account 34567: Booked Balance

Two maintenance sweeping records are created between account 56789 and the Main Master account 12345 and between account 34567 and Main Master account 123456.

The maintenance sweeping records are set to maintain the balances of the 56789 and 34567 accounts as zero.

The current balances of accounts are shown in the below screenshot.

A debit transaction of 1000 USD is posted against the account 56789. The system considers as funds available in the account’s 56789 balance and the Main Master account’s balance as,

500 USD + 1000 USD= 1500 USD

The funds are sufficient and the transaction is posted.

The booked balance of account 56789 becomes 500 USD. The system calculates the amount necessary to be swept to cover the deficit in the account 56789 and considers the booked balance, which is equal to debit 500 USD. The system needs to maintain zero balance in the account and 500 USD is reserved on the Main Master account.

A credit transaction of 300 USD is posted against the account 56789. The booked balance of account 56789 becomes 200 USD and funds reserved on the Main Master account are reduced and becomes 200 USD.

A credit transaction of 500 USD is posted against the account 34567. The booked balance of account 34567 becomes 500 USD. Funds reserved are not reduced at the Main Master account’s level as they were not reserved by the account 34567.

| Date | Participant Account (100001) | Master Account (200002) |
|---|---|---|
| 16 April 2019 | 0 | 3000.00 |
| 17 April 2019 | 0 | 2000.00 |

Account upload order option is available in AC.CASH.POOL application to set the target balances. Whenever the account balance falls below the minimum amount defined, Temenos Transact transfers the sweeping account by debiting the master account. This is enabled only for maintenance sweeps. The user can define target balance in the Target Balance field and the sweeping account is funded to reach the target balance.

Define the Maintenance sweep and set the Balance To Use as Booked Less Locked in AC.SWEEP.TYPE .

- Sweep account (100001): 50.00 USD
- Master account (200002): 250.00 USD
- Frequency: Daily, every business day
- Schedule: COB
- Minimum amount: 30.00
- Transfer Amount : 50.00

A card transaction for debit in participant account for USD 40 (booking takes place after 2 days).

Sweeping transactions

- The sweep is executed for USD 40.00.
- Participant account actual balance USD 90.00.

Sweeping suspension is applicable for all sweep types. When the Susp Sign field is set as Dr or Cr, the sweep is suspended. When a sweep is to be blocked with debit, the Susp Sign should be set as Dr and vice-versa for Cr.

When the link account is blocked for,

- Debit – The Susp Sign field is updated as Cr .
- Credit – The Susp Sign field is updated as Dr.

The below examples enables the user to understand the sweeping suspension:

A Cash pool is setup as follows:

- Master account: 100001
- Member account: 100002

Zero balancing sweeps are setup against 100002, using 100001 as a link account.

Debit blocking: 100002

Opening balance: 10000

Minimum amount: 0.00

Maximum amount: 0.00

Frequency: BSNSS

When a debit block is set on account 100002, the Susp Start Date field is updated in AC.CASH.POOL record and Susp Sign field is updated Dr. When sweep processing is intraday or EOD, Temenos Transact checks the cashpool record and the sweep is not processed.

A Cashpool is setup as follows:

- Master account: 100001
- Member account: 100002

Zero Balancing sweeps are setup against 100002 using 100001 as a link account.

Credit blocking: 100001

Opening balance: 10000

Minimum amount: 0.00

Maximum amount: 0.00

Frequency: BSNSS

When a credit block is set on account 100001, the Susp Start Date field is updated in AC.CASH.POOL record and Susp Sign is updated as Cr. When sweep processing is intraday or EOD, Temenos Transact checks the cashpool record, Suspense Start Date , posting sign and sweep is not processed.

| Column 1 | Column 2 | Column 3 |
|---|---|---|
| Booked Date | Value Date | Transaction |
| 18-April-2020 | 18-April-2020 | Incoming funds CR 5000 |
| 18-April-2020 | 18-April-2020 | Incoming funds CR 2000 |
|  |  |  |
| Booked balance | 7000 |  |
| End of day sweep | 18-April-2020 | 7000 |
|  |  |  |
| Opening booked balance | 1000 |  |
| 19-April-2020 | 19-April-2020 | Incoming funds CR 3000 |
| 19-April-2020 | 19-April-2020 | Outgoing funds DR 1000 |
| Booked balance | 3000 |  |
| End of day sweep | 19-April-2020 | 2000 |

The external corporate sweeps allow the user to set sweep transactions to/from accounts held in another system within the bank or another financial institution. AC.CASH.POOL executes the external sweeps and generates payment orders to/from other banks. When the user defines the beneficiary record id in AC.CASH.POOL , Transact checks the beneficiary account details in BENEFICIARY and generates payment orders.

While processing the sweep transactions, the user can optionally define Link Acct when defining Beneficiary Id and Payment Product in AC.CASH.POOL . It is mandatory to define Payment Product when defining Beneficiary Id . Transact automatically defaults the internal wash account in Link Acct based on the category defined in Po Wash Categ of AC.SWEEP.TYPE .

Processing external sweeps are applicable for all types of sweeps (Maintenance, Surplus, Cashpool and Two-Way). The Beneficiary Id field in AC.CASH.POOL allows the user to select valid records from BENEFICIARY .

The below screenshot displays a cash pool record created with,

- the sweeping account as 104833 with Beneficiary record
- the sweep type as Maintenance sweep

Transact updates the sweeping transaction details in AC.ACCOUNT.SWEEP.HIST after the completion of sweep processing.

Transact generates the payment order for debiting the link account and crediting it to the sweep account (@ID).

| Transaction Type | Transaction Amount (USD) | Booked / Posted Balance (USD) | Cleared / Collected Balance (USD) | Cumulative Debit Holds (USD) | Cumulative Credit Holds (USD) | Available Balance (USD) |
|---|---|---|---|---|---|---|
| Starting Balance |  | 100 | 100 |  |  | 100 |
| Debit Hold Today | -555 | 100 | 100 | -555 |  | -455 |
| Check Debit | -600 | -500 | -500 | -555 |  | -1055 |
| Credit Hold Today | 1000 | -500 | -500 | -555 | 1000 | -55 |
| Customer – Debit | -500 | -1000 | -1000 | -555 | 1000 | -555 |
| Future Dated Credit Hold (T+1) | 100 | -1000 | -1000 | -555 | 1100 | -555 |
| Future Dated Debit Hold (T+1) | -55 | -1000 | -1000 | -610 | 1100 | -555 |


#### 📋 Tasks

Related topics:

- Create Sub Account (Notional Pooling)
- Execute Intra-Day Sweep (Transactional Pooling)
- Accounts and Deposits Processes (Corporate)
- Set Up, Amend Pool and Groups

Physical Pooling is bringing together of balances in nominated accounts into a target account. This allows companies to manage the surplus cash more efficiently. Physical Pooling gives the customer the ability to internally finance any deficit, thereby avoiding additional expenses.

Multicurrency Sweep

Multicurrency Sweep is the execution of the sweep between accounts of different currencies.

At the time of execution of multicurrency sweep, system uses the appropriate exchange rate from the CURRENCY table based on the value defined in the EXCH.RATE.TYPE field of AC.CP.GROUP.PARAM , which can be either Mid or Buy/Sell rate.

Spread that needs to be applied on the exchange rate can be defined in the EXCH.RATE.SPR field of AC.CP.GROUP.PARAM application, which gets defaulted in the EXCH.RATE.SPR field of AC.CASH.POOL application record. The defaulted value can be amended by the user.

Market exchange profit for the spread amount is calculated and accounted into the PL category defined in the POMKKEXCHPFT of ACCOUNT.CLASS application. The details of exchange rate, spread, market exchange profit, and so on are updated in AC.CASH.POOL.HIST record.

When a sweep is reversed, the exchange rate used at the time of execution of sweep is used at the time of reversal.


##### Workflow

The user can process the physical pooling using the below workflow:

This menu allows the user to create different cash pool types, such as, shared without sweep, shared with sweep and sweep without sharing balances.

To create a shared without sweep cash pool process, perform the following steps:

1. Create Cash Pool (Process) .
2. In the User Prompt screen, select the Setup CP-Shared without Sweep option in the Choose Cash Pool Type field and then click the Launch icon.
3. Select a required Group ID from the Shared W/O Sweep field.
4. Click the Edit icon.
5. Enter values in the mandatory and other required fields.
6. Click the Validate icon to check for the errors and overrides.
7. Click the Commit icon to submit the record.

To create a shared with sweep cash pool process, perform the following steps:

1. Create Cash Pool (Process) .
2. In the User Prompt screen, select the Setup CP–Shared with Sweep option from the Choose Cash Pool Type field and then click the Launch icon.
3. Select a Group ID from the Simple group field.
4. Click the Edit icon.
5. Enter values in the mandatory and other required fields.
6. Click the Validate icon to check for the errors and overrides.
7. Click the Commit icon to submit the record.

To create a cash pool sweep without sharing balances, perform the following steps:

1. Create Cash Pool (Process) .
2. In the User Prompt screen, select the Setup CP-Sweep w/o Sharing Bal option from the Choose Cash Pool Type field and then click the Launch icon.
3. Select a Group ID from the Sweep W/O Sharing Bal field.
4. Click the Edit icon.
5. Enter values in the mandatory and other required fields.
6. Click the Validate icon to check for the errors and overrides.
7. Click the Commit icon to submit the record.

This menu allows the user to create a simple group by which the user is creating an AC.CP.GROUP.PARAM application record for creation of float transfer.

To create a simple group, perform the below steps:

1. Simple Group .
2. Select a Group ID from the Simple group field.
3. Click the Edit icon
4. Enter values in the mandatory and other required fields
5. Click the Validate icon to check for the errors and overrides.
6. Click the Commit icon to submit the record.

This menu allows the user to create a sub group and link to main group.

To create a sub group and link to main group, perform the below steps:

1. Create sub group and link to main group .
2. In the Contract Screen, select the Group ID from the Shared with Sweep field.
3. Enter the mandatory and other field values as required.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.

This menu allows the user to create a shared balances group.

To create a shared balances group, perform the below steps:

1. Shared Balances Group .
2. In the Contract Screen, select the Group ID from the Shared W/O Sweep field.
3. Enter the mandatory and other field values as required.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.

This menu allows the user to create a shared balances sub group.

To create a shared balances sub group, perform the below steps:

1. Create shared balances sub group .
2. In the Contract Screen, select the Group ID from the Shared W/O Sweep field.
3. Enter the mandatory and other field values as required.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.

This menu allows the user to authorise or delete the unauthorised groups.

To authorise the unauthorised group, perform the below steps:

1. Authorise/delete group .
2. In the Unauthorised Group screen, click the Authorise icon corresponding to a record.
3. Verify the transaction details and click the Authorise icon to commit the authorisation.

To delete the unauthorised group, perform the below steps:

1. Authorise/delete group .
2. In the Unauthorised Group screen, click the Delete icon corresponding to a record.
3. Click the Delete icon to commit the deletion.
4. Click the OK button in the message box that appears.

This menu allows the user to authorise or delete the unauthorised sub groups.

To authorise the unauthorised sub group, perform the below steps:

1. Authorise/delete sub group .
2. In the Unauthorised Sub Group screen, click the Authorise icon corresponding to a sub group record.
3. Verify the transaction details and click the Authorise icon to commit the authorisation.

To delete the unauthorised sub group, perform the below steps:

1. Authorise/delete sub group .
2. In the Unauthorised Group screen, click the Delete icon corresponding to a sub group record.
3. Click the Delete icon to commit the deletion.
4. Click the OK button in the message box that appears.

This menu allows the user to create a cash pool sweep rule, which can be set to sweep intraday at COB with or without sharing the group balance.

To set a cash pool sweep rule, perform the below steps:

1. Create Cash Pool .
2. In the Contract Screen, select the Transaction Ref from the Cash Pool-Sweep field and then click the Edit icon.
3. In the Cash Pool – Sweep screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.

This menu allows the user to amend the created cash pool sweep records.

To amend the created cash pool records, perform the below steps:

1. Amend Cash Pool .
2. In the Amend Cash Pool screen, click the Amend icon corresponding to a cash pool record.
3. In the Cash Pool – Sweep screen, enter values in the fields which needs to be amended.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.

This menu allows the user to authorise or delete the unauthorised cash pool records.

To authorise the unauthorised cash pool records, perform the below steps:

1. Authorise/delete Cash pool .
2. In the Unauthorised Cash Pool screen, click the Authorise icon corresponding to a cash pool record.
3. Verify the transaction details and click the Authorise icon to commit the authorisation.

To delete the unauthorised cash pool records, perform the below steps:

1. Authorise/delete Cash pool .
2. In the Unauthorised Cash Pool screen, click the Delete icon corresponding to a cash pool record.
3. Click the Delete icon to commit the deletion.
4. Click the OK button in the message box that appears.

This menu allows the user to run the sweeps during the day.

To run the sweeps during the day, perform the below steps:

1. Run Sweeps .
2. In the Contract Screen, select the Group ID from the Intra Day Sweep field.
3. Click the Edit icon.
4. In the Intra Day Sweep screen, enter values in the necessary fields as required.
5. Click the Validate icon to check for the errors and overrides.
6. Click the Commit icon to submit the record.

This menu allows the user to authorise or delete the unauthorised group records.

To authorise the unauthorised group records, perform the below steps:

1. Group .
2. In the Unauthorised Group screen, click the Authorise icon corresponding to a group record.
3. Verify the transaction details and click the Authorise icon to commit the authorisation.

To delete the unauthorised group records, perform the below steps:

1. Group .
2. In the Unauthorised Group screen, click the Delete icon corresponding to a group record.
3. Click the Delete icon to commit the deletion.
4. Click the OK button in the message box that appears.

This menu allows the user to authorise or delete the unauthorised cash pool records.

To authorise the unauthorised cash pool records:

1. Cash Pool .
2. In the Unauthorised Cash Pool screen, click the Authorise icon corresponding to a cash pool record.
3. Verify the transaction details and click the Authorise icon to commit the authorisation.

To delete the unauthorised cash pool records:

1. Cash Pool .
2. In the Unauthorised Cash Pool screen, click the Delete icon to delete the unauthorised cash pool records.
3. Verify the transaction details and click the Delete icon to commit the deletion.
4. Click OK in the message box that appears.

| SCREENS | WORKFLOW |
|---|---|
|  | Financing Cash Pool . |
| Contract Screen | Select a group id in the Financing Cash Pool field drop-down. Click the Edit icon. |
| Financing Cash Pool | In the Financing Cash Pool tab, enter values in the required fields. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

This menu allows the user to reverse the Close of Business (COB) cash pool sweep. The COB cash pool sweep can be reversed by entering the Group name with the Verify function and in the case of the Intra-day sweeps, reversal can be made by entering the Group ID.

To reverse a last run sweep, follow the below steps:

1. Reverse last run sweeps .
2. In the Contract screen, enter the Group name or Group ID or select a value from the Reverse Last Run Sweep field drop-down and then click the Edit icon.
3. Enter a value in the Description field.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.


#### 📊 Outputs

Physical Pooling is bringing together the balances of nominated accounts into a target account. This allows companies to manage the surplus cash more efficiently. Physical Pooling gives customers the ability to internally finance any deficit, thereby avoiding additional expenses.


##### Enquiries and Reports

This section helps the user to view the physical pooling sweep movements, cash pool account list, sweep history, etc.

Cash Pool Groups .

This enquiry displays information on the list of cash pool groups. The user can view the list of cash pool groups by either running the enquiry without any details or by entering the group id. The user can view the individual cash pool groups by clicking the View icon.

Cash Pool Links .

This enquiry displays information on links for the cash pool groups. The user can view the list of cash pool link by either running the enquiry without any details or by entering the group id. The user can view the individual cash pool records by clicking the View icon.

Shared Account .

This enquiry displays information on the list of accounts that have shared their balances. The user can view the shared account details by either running the enquiry without any details or by entering the group id.

Sweep History .

This enquiry displays information on history of all the sweeps that had occurred with the date and amount.

Group Position .

This enquiry displays the group position along with the individual account balances when the user enters the group id in the selection criteria.

Sweep Movements .

This enquiry displays the list of sweep movements in a group along with the transaction reference, amount and date.

Projected sweep movements .

This enquiry displays the list of projected sweep movements along with the next sweep date.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA


> **Related Applications:** `AC.ACCOUNT.SWEEP.HIST`, `AC.CASH.POOL`, `AC.CASH.POOL.LINK`, `AC.CP.GROUP.PARAM`, `AC.CREDIT.CHECK`, `AC.SWEEP.CONDITIONS`, `AC.SWEEP.TYPE`, `EB.CONTRACT.BALANCES`, `INTRA.DAY.SWEEP`

---


---


## Appendix A: Glossary of T24 Applications & Fields


This glossary lists all T24/Transact application names and field names referenced throughout this document, with descriptions where available.


### Applications


| Application | Description |
|------------|-------------|
| `AA.ACCOUNT.DETAILS` | T24 application: AA.ACCOUNT.DETAILS |
| `AA.ACTIVITY.CLASS` | T24 application: AA.ACTIVITY.CLASS |
| `AA.ACTIVITY.HISTORY` | T24 application: AA.ACTIVITY.HISTORY |
| `AA.ARR.PAYMENT.SCHEDULE` | T24 application: AA.ARR.PAYMENT.SCHEDULE |
| `AA.ARRANGEMENT.ACTIVITY` | T24 application: AA.ARRANGEMENT.ACTIVITY |
| `AA.BILL.DETAILS` | T24 application: AA.BILL.DETAILS |
| `AA.CONTEXT TYPE` | T24 application: AA.CONTEXT TYPE |
| `AA.INTEREST.ACCRUALS` | T24 application: AA.INTEREST.ACCRUALS |
| `AA.PARAMETER` | T24 application: AA.PARAMETER |
| `AA.PAYMENT.TYPE` | T24 application: AA.PAYMENT.TYPE |
| `AA.PERIODIC.ATTRIBUTE` | T24 application: AA.PERIODIC.ATTRIBUTE |
| `AA.PRD.DES.ACTIVITY.MAPPING` | T24 application: AA.PRD.DES.ACTIVITY.MAPPING |
| `AA.PRD.DES.PAYMENT.SCHEDULE` | T24 application: AA.PRD.DES.PAYMENT.SCHEDULE |
| `AA.PRODUCT.DESIGNER` | T24 application: AA.PRODUCT.DESIGNER |
| `AA.PRODUCT.GROUP` | T24 application: AA.PRODUCT.GROUP |
| `AA.PRODUCT.LINE` | T24 application: AA.PRODUCT.LINE |
| `AA.PROPERTY` | T24 application: AA.PROPERTY |
| `AA.PROPERTY.CLASS` | T24 application: AA.PROPERTY.CLASS |
| `AA.SIMULATION.CAPTURE` | T24 application: AA.SIMULATION.CAPTURE |
| `AC.ACCOUNT.SWEEP.ERROR` | T24 application: AC.ACCOUNT.SWEEP.ERROR |
| `AC.ACCOUNT.SWEEP.HIST` | T24 application: AC.ACCOUNT.SWEEP.HIST |
| `AC.ACCOUNTING.PARAM` | T24 application: AC.ACCOUNTING.PARAM |
| `AC.ALLOCATION.RULE` | T24 application: AC.ALLOCATION.RULE |
| `AC.ALLOCATION.RULES` | T24 application: AC.ALLOCATION.RULES |
| `AC.BALANCE.COMPONENT` | T24 application: AC.BALANCE.COMPONENT |
| `AC.BALANCE.TYPE` | T24 application: AC.BALANCE.TYPE |
| `AC.CASH.POOL` | T24 application: AC.CASH.POOL |
| `AC.CASH.POOL.LINK` | T24 application: AC.CASH.POOL.LINK |
| `AC.CP.GROUP.PARAM` | T24 application: AC.CP.GROUP.PARAM |
| `AC.CREDIT.CHECK` | T24 application: AC.CREDIT.CHECK |
| `AC.EVENT` | T24 application: AC.EVENT |
| `AC.SWEEP.CONDITIONS` | T24 application: AC.SWEEP.CONDITIONS |
| `AC.SWEEP.TYPE` | T24 application: AC.SWEEP.TYPE |
| `ACCOUNT` | T24 application: ACCOUNT |
| `CATEG.ENTRY` | T24 application: CATEG.ENTRY |
| `CURRENT.ACCOUNT` | T24 application: CURRENT.ACCOUNT |
| `CUSTOMER` | T24 application: CUSTOMER |
| `EB.ACCRUAL` | T24 application: EB.ACCRUAL |
| `EB.CASHFLOW` | T24 application: EB.CASHFLOW |
| `EB.CONTRACT` | T24 application: EB.CONTRACT |
| `EB.CONTRACT.BALANCES` | T24 application: EB.CONTRACT.BALANCES |
| `EB.EVENTS` | T24 application: EB.EVENTS |
| `EB.LOOKUP` | T24 application: EB.LOOKUP |
| `EXTERNAL.ACCOUNT` | T24 application: EXTERNAL.ACCOUNT |
| `INTRA.DAY.SWEEP` | T24 application: INTRA.DAY.SWEEP |
| `INVESTMENT.ACCOUNT` | T24 application: INVESTMENT.ACCOUNT |
| `LIMIT` | T24 application: LIMIT |
| `LIMIT.REFERENCE` | T24 application: LIMIT.REFERENCE |
| `MS.PARAMETER` | T24 application: MS.PARAMETER |
| `NSF.PARAMETER` | T24 application: NSF.PARAMETER |
| `PERIODIC.RATE` | T24 application: PERIODIC.RATE |
| `RC.CONTRACT.PRIORITY` | T24 application: RC.CONTRACT.PRIORITY |
| `RE.CONSOL.SPEC.ENTRY` | T24 application: RE.CONSOL.SPEC.ENTRY |
| `STMT.ENTRY` | T24 application: STMT.ENTRY |


### Fields Referenced


| Field | Field | Field |
|-------|-------|-------|
| `AA Bundle ID` | `AMC` | `Aa Product` |
| `Aa Product Group` | `Account Capitalisation` | `Account Distribution Type` |
| `Account No` | `Acct Mode` | `Act Credit Check` |
| `Activity` | `Activity Link` | `Actual Amount` |
| `Actual Amt` | `Actual Pay Date` | `Adjustment` |
| `Advance Payment Restriction` | `Aggregate Bal` | `Aging Status` |
| `Align Dates` | `Allocate Sweep Amount` | `Allow Netting` |
| `Allowed Product` | `Alt Acct Id` | `Alt Acct Type` |
| `Alt Id Type` | `Alt Payment Method` | `Alt Payment Routine` |
| `Alternate Id` | `Alternate Id Type` | `Amortisation Term` |
| `Amount` | `Amount Routine` | `Amt Sweep Routine` |
| `Application Method` | `Arrangement` | `Attribute Type` |
| `Attribute Value` | `Available Company` | `Back Value Adjustment` |
| `Back Value Capitalisation` | `Back-to-Back FX` | `Back-to-back FX` |
| `Bal Conversion Mkt` | `Balance Routine` | `Balance To Use` |
| `Balance To Use` | `Balance Treatment` | `Balance to Use` |
| `Base Ccy Product` | `Basic Rate Text` | `Beneficiary Id` |
| `Bill Produced` | `Bill Produced` | `Bill Status` |
| `Bill Type` | `Bundle Arrangement` | `Business Day Definition` |
| `Cal Routine` | `Calc Amount` | `Calc Type` |
| `Calculation Routine` | `Calculation Type` | `CalculationType` |
| `Cash Pool-Sweep` | `Cashflow Amount` | `Ccy` |
| `Change Amount` | `Charge Amount` | `Charge Code` |
| `Charge Debit Account` | `Charge Negotiable` | `Charge Off Amount` |
| `Charge Off Percentage` | `Charge off Amount` | `Charge off Percentage` |
| `Choose Cash Pool Type` | `Chrg Negotiable` | `Cmt Bal Type` |
| `Combine Bill At Parent` | `Commitment Balance Type` | `Commitment Drawdown` |
| `Commitment Reversal` | `Company` | `Comparison Type` |
| `Concentration Account` | `Context Name` | `Context Value` |
| `Context name` | `Cooling Date Adj` | `Cooling Period` |
| `Cr Adj Categ, Cr Adj Txn Pl and Cr Adj Txn Ac` | `Cr Category` | `Cr Txn Code Ac` |
| `Cr Txn Code Pl` | `Create Group Main Account` | `Create Retry Trigger` |
| `Credit Check` | `Credit Interest for an Account` | `Currency` |
| `Currency Maximum` | `Current Balance` | `Custom Name` |
| `Custom Priority Rank` | `Custom Rate` | `Custom Rate Calculation` |
| `Custom Type` | `Custom Value` | `Customer` |
| `Date Convention` | `Def Account` | `Def Fund Decision` |
| `Def Prev Settle` | `Default Variation` | `Defer Date` |
| `Defer Period` | `Description` | `Dr Adj Categ, Dr Adj Txn Pl and Dr Adj Txn Pl` |
| `Dr Category` | `Dr Txn Code Ac` | `Dr Txn Code Pl` |
| `Draw Bal Type` | `Drawing Balance Type` | `Drop Credit Reservations` |
| `Due Frequency` | `Due Rule` | `Due Type` |
| `EIR` | `EXCH.RATE.SPR` | `EXCH.RATE.TYPE` |
| `Eb Group Id` | `Effective Date` | `Emit Business Event` |
| `End Date` | `Event Type` | `Exch Rate Spr` |
| `Exch Rate Type` | `Expiry Days` | `Expiry date` |
| `Exposure Date` | `Extend Cycle` | `External Posting` |
| `Field Name.1.1` | `Field Name.1.2` | `Field Name.1.3` |
| `Field Name.1.4` | `Field Name.1.5` | `Field Name.1.6` |
| `Field Value.1.1` | `Field Value.1.2` | `Field Value.1.3` |
| `Field Value.1.4` | `Field Value.1.5` | `Field Value.1.6` |
| `Finalise Bills` | `Finalise Bills` | `Financial Date` |
| `Financing Cash Pool` | `Float Transfer` | `Frequency` |
| `Full Chargeoff` | `Full Commitment Activity` | `Fund Deci Approve Act; Fund Deci Rej Act; Rev Approve Act; Rev Rej Act` |
| `Fund Decision Upd` | `Fwd Acct Mode` | `Generate Iban` |
| `Grace Balance Type` | `Grace Locked Reserve Condition` | `Grace Period Type` |
| `Grace Start Balance` | `Group Bill Type` | `Group Hierarchy` |
| `Group Id` | `Group Min Amount` | `Group Min Property` |
| `Group.Id` | `Hol Restrict Item` | `Hol Restrict Type` |
| `Ica Add Remove` | `Ica Main Account` | `Ica Main Acct` |
| `Ica Main Acct Ind` | `Ica Main Date` | `Ica New Main Acc` |
| `Ica Start Date` | `In Adv` | `Inadv` |
| `Include Future Disb` | `Interest Adjustment` | `Internal Limit` |
| `Intra Day` | `Intra Day Sweep` | `Intra-day` |
| `Last Maint Date` | `Legacy War Rate` | `Link AC Number` |
| `Link Ac Number` | `Link Acc Num` | `Link Account` |
| `Link Account 1` | `Link Account 2` | `Link Account Number` |
| `Link Acct` | `Link Suspension End Date` | `Link Suspension Start date` |
| `Link Sweep Cancel Date` | `Linked Ac Number` | `Linked Account Number` |
| `Loc Cap Chk Rtn` | `Loc Processor` | `Loc post process` |
| `Loc pre process` | `Loc prioritise` | `Loc processor` |
| `Lock Reserve Condition` | `Main Group Id` | `Main Master` |
| `Mandatory` | `Master Arrangement` | `Master Company Time` |
| `Master Live Date` | `Master Type` | `Max Concentration Amt` |
| `Max Contribution Amount` | `Max Contribution Amt` | `Max Percentage` |
| `Max Redemption Amt` | `Max Sweep Amt` | `Maximum Amount` |
| `Maximum Amt` | `Maximum Amt.1` | `Maximum Balance` |
| `Maximum Concentration Amount` | `Maximum Concentration Amt` | `Maximum Term Cap` |
| `Method` | `Min Amount Transfer` | `Min Amt Transfer` |
| `Min Contribution Amt` | `Min Contribution Amt.` | `Min Redemption Amt` |
| `Min Sweep Amt` | `Min TFR Cr` | `Min TFR Dr` |
| `Min TRF Cr` | `Min TRF Dr` | `Min. Tfr Cr 1` |
| `Min. Tfr Dr 1’` | `Minimum Amount` | `Minimum Amt` |
| `Minimum Amt.1` | `Minimum Payment Type` | `Modify/Cancel Payment Holidays` |
| `Movement Supress` | `Multi Currency` | `NSF Balance Type` |
| `NSF Decision Hook` | `NSF Lock Reserve Condition` | `NSF Process Type` |
| `NSF Start Balance` | `New Main Account` | `New Payment Amount` |
| `New Property Amount` | `No Activity Indicator` | `No Hierarchy Reqd` |
| `Nr Value` | `Nr Value Source` | `Number of Installments` |
| `Number of Instalments` | `Number of Payments` | `On Activity` |
| `On Activity, Recalculate` | `Online Retry Attempts` | `Optional` |
| `Or Prop Amt` | `Or Prop Amt Bnk` | `Order` |
| `Orig Contract Date` | `Original Property Amount` | `Os Prop Amt` |
| `Os Prop Amt Bnk` | `Override Amount` | `Override Percent` |
| `Owing Customer` | `POMKKEXCHPFT` | `Parent Account` |
| `Partial Amount` | `Partial Transfer` | `Participant Currency` |
| `Participant Owner` | `Pay Freq` | `Payment` |
| `Payment Date` | `Payment Freq` | `Payment Method` |
| `Payment Mode` | `Payment Order Product` | `Payment Product` |
| `Payment Type` | `Payment amount` | `Payment type` |
| `Penalty Interest` | `Percentage` | `Periodic Attribute` |
| `Periodic Type` | `Po Wash Categ` | `Pool Sweep` |
| `Post process` | `Pr Value` | `Pre Notice Activity` |
| `Pre Notice Days` | `Pre processor` | `Pref Pymt Product` |
| `Prev Settle` | `Principal` | `Prioritise` |
| `Priority Execution` | `Priority Rank Type` | `Processing Date` |
| `Processor` | `Prod Cat End` | `Prod Cat Start` |
| `Product` | `Product Only` | `Prog Pay Perc` |
| `Property` | `Property 1` | `Property.1` |
| `RCCondition` | `Rank Based Priority` | `Rc Condition` |
| `Rc Type` | `Recalculate` | `Recalculate Method` |
| `Recalculation` | `Refer Settlement` | `Refer Settlement Type` |
| `Repay Period` | `Repay Type` | `Repay type` |
| `Reporting Type` | `Request Payment Holiday` | `Request Payment Holidays` |
| `Reserve Sweep Projections` | `Residual Amount` | `Retry Attempts` |
| `Retry Fqu` | `Retry Options` | `Retry Period` |
| `Return At Sod` | `Return Rule Priority` | `Reverse Last Run Sweep` |
| `Revolving` | `Rtn With Sw Amt` | `Rule` |
| `Rule Priority` | `Rule Start` | `Rule Start Date` |
| `Rule.1` | `Run Time Rate Calc` | `Sb Group Id` |
| `Schedule` | `Schedule Type` | `Secondary Limit Amount` |
| `Sequence` | `Sequencing` | `Settle Status` |
| `Settle Type` | `Settlement Type` | `Shared Balances` |
| `Shared Balances` | `Shared W/O Sweep` | `Shared with Sweep` |
| `Simple group` | `Start Date` | `Start date` |
| `Start of Day Capitalisation` | `StartDt Option` | `Stmt` |
| `Sub Group` | `Susp Appln` | `Susp End Date` |
| `Susp Sign` | `Susp Start Date` | `Suspend End Date` |
| `Suspend Indefinite` | `Suspend Start Date` | `Suspense End Date` |
| `Suspense Indefinite` | `Suspense Start Date` | `Suspense indefinite` |
| `Sweep Amount Sorting` | `Sweep Amt Sorting` | `Sweep Cancel Date` |
| `Sweep Chg Amount` | `Sweep Chg Code` | `Sweep Cut-Off Time` |
| `Sweep Debit Reservations` | `Sweep Reserve Condition` | `Sweep Susp Acct` |
| `Sweep Time` | `Sweep Times` | `Sweep Unit Amount` |
| `Sweep W/O Sharing Bal` | `System Id` | `Takeover Npv` |
| `Takeover method` | `Target Balance` | `Tax Amount` |
| `Tax Inclusive` | `Term` | `Top Account` |
| `Tot Due Amt` | `Total Due` | `Transaction Type` |
| `Transfer Amount` | `Transfer Unit Amount` | `Trigger Max Bal` |
| `Trigger Min Bal` | `Txn Code` | `Txn Type` |
| `Type` | `Up To Percent` | `Up to Amount` |
| `Up to Amount.1` | `Up to Percent` | `Update Commit On Capitalisation` |
| `Update Commit on Capitalisation` | `Update Utilised Commitment` | `Update Utilised Commitment` |
| `Upto Amount` | `Use Limits` | `Use Secondary Limit` |
| `Utilise Limit` | `Utilize Amount` | `Utilize Limit` |
| `Value` | `Value Dtd Acctng Y/N` | `Waive Bill Type` |
| `Waive Charges` | `Waive Class, Waive Prop and Waive Bill Type` | `Zero Balancing` |
| `xx` | `xx` | `Field.Value` |


---


## Appendix B: Consolidated Field Reference


This appendix consolidates all field description tables from across the documentation, grouped by sub-module. This provides a single reference for all field definitions.


### Cash_Management - BN (BN)


**Hybrid Pooling**

| Account Types | Description |
|---|---|
| Master account | AA product bundle The Property Class bundle hierarchy specifies the allowed products of the hierarchy and the hierarchy structure itself. |
| Currency top account | On-balance sheet AR account and attached to the MA bundle as bundle participants. One of these CT accounts are nominated as the recipient of the bundle for interest at MA level and it is effectively deemed as the currency of the MA for advices or statements or MA balance enquiries purposes |
| Transaction or Mirror transaction or Currency summary or Multi currency summary accounts | Off-balance sheet AR accounts Currency summary, multi-currency summary and CT accounts – disabled for external posting Multi-currency summary account – enabled to maintain currency wise balances |

**Hybrid Pooling**

| Account Type | Company Name | System Date |
|---|---|---|
| CT account (100001) | Temenos core banking Norway company | 25/10/2017 |
| TR account (100002) | Temenos core banking Norway Sweden | 23/10/2017 |
| TR account (100003) | Temenos Core Banking Norway Finland | 24/10/2017 |

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


### Cash_Management - PO (PO)


**NSF ExceptionProcessing**

| Field Name | Description |
|---|---|
| Settle Type | The possible values in the field are: PTL (Payed Through Limits) – Account balance including transaction amount is within the limit available at the time of posting the entry. POL (Payed Outside Limit) – Either account balance including transaction amount is in excess of the limit available at the time of posting the entry or the limit is not applicable (Opt-Out) for the respective debit transaction or activity. SET (Automatic Settlement) – Force settled with NSF. This debit transaction or activity is forced to be settled at the activity class definition. |
| Expiry Days | Indicates the cut-off period for manual decision making. This is the number of days within which the bank user should either approve or reject the NSF item and negotiate the NSF fee or charge. If the decision is not actioned manually, the default decision (if defined in the NSF parameter) applies on the COB of the expiry date of the NSF exception item. |
| Def Fund Decision | Hold the value approved or rejected. |
| Fund Decision Upd | Hold the value system or manual, to indicate the fund decision update. |
| Fund Deci Approve Act; Fund Deci Rej Act; Rev Approve Act; Rev Rej Act | Arrangement activity to be triggered for the default decision processing for fund approval/rejection or reversal approval/rejection. |
| Charge Negotiable | Hold the value YES or NO, to indicate if the NSF fee or charge is negotiable. |
| NSF Decision Hook | Configure the user exit routine to overrule the rule-based NSF decisioning of account transactions. |
| NSF Start Balance | Indicates the starting balance that must be used when calculating the accounts available balance used for the NSF evaluation process. It belongs to a set of associated fields. The allowed values are: Open.booked Open.valued If there is no value defined, Open.valued is the default value. |
| NSF Balance Type | Defines the inclusion of active debit holds and active credit holds in the available balance calculation during the NSF Evaluation process. It belongs to a set of associated fields. The allowed values are: Lock.funds Credit.reserve If there is no value defined, the available balance is calculated by including all the balance components. |
| NSF Lock Reserve Condition | The allowed values are: Lock.funds.date - Includes active debit locked events Credit.reserve.date - Includes active credit locked events. If there is no value defined for the associated balance type, the system refers the definition in AC.ACCOUNTING.PARAM . |
| NSF Process Type | The allowed value is: Exclude.return - Excludes the debit transaction amount from calculating the running balance when the default decision of the entry is set as RETURN or REJECT. |

**NSF ExceptionProcessing**

| Field Name | Description |
|---|---|
| Grace Period Type | Indicates the balance cure method applied when Grace Period functionality is enabled. The supported values are: Full – The account must have an available balance and tolerance greater or equal to 0 for the NSF charges to be waived. Partial – Each NSF exception is evaluated to determine if the positive movement of the available balance is sufficient to cover that item. |
| Grace Start Balance | Indicates the starting balance used for calculating the accounts available balance (used for grace period waiver). The allowed values are: Actual.booked - Indicates the account’s booked balance for today. A transaction is considered booked once it is completed and the balances are updated. Transactions with a forward processing date (for example, non-stop transactions entered at the close of business) are not included in this balance until the bank’s system date matches the processing date of the transaction. Actual.value - Indicates the account’s value-dated balance for today, which is used for interest calculation. Transactions with a forward value date are not included in today’s value-dated balance until the specified value date arrives. If the balance is not defined, then Actual.value is considered as the default value. |
| Grace Balance Type | Indicates the debit locked events and credit locked events are included when calculating the account available balances used for grace period waiver. The supported values are Lock.funds and Credit.reserve. The user can select one or both the options. |
| Grace Locked Reserve Condition | Indicates if current day’s active locked events should be used or if the maximum or minimum amounts should be used when debit locked events and credit locked events are included in the account available balance calculation. The supported values are Lock.funds.date and Credit.reserve.date. The user can select one or both the options. If the field is left blank for the associated Grace Balance Type , then the system uses the setting defined in Lock Reserve Condition in AC.ACCOUNTING.PARAM as default. |

**External LoC**

| Event Attribute Name | Description |
|---|---|
| transactionReference | Indicates the unique reference for the sweep transaction which has initiated the funds request. |
| transactionDate | Indicates the business date on which the sweep transaction was initiated. |
| sweepingAccountId | Indicates the Account Reference/ID of the sweeping account in Transact. |
| sweepingAccountCurrency | Indicates the currency of the sweeping account. |
| contraCategoryOrAccount | Indicates the sweep suspense account. |
| accountId | Indicates the Account Reference/ID of the external arrangement in Transact that represents the LOC/CC on the external systems. |
| alternateReferences | Collection – Contains details of all alternate ids applicable for the external arrangement in Transact. |
| requestAmount | Indicates the amount that is required to be disbursed or released from the loan or credit card accounts held in the systems external to Transact. |
| requestCurrency | Indicates the Currency associated to the requestedAmount. |
| alternateAccountType | Identifies the alternate account id type applicable for the associated alternate Id of the external arrangement in Transact. |
| alternateAccountId | Identifies the alternate account id applicable for the associated alternate account id type of the external arrangement in the Temenos Transact. For example, Account Reference of the LOC / CC in the external system. |

**External LoC**

| Event Attribute Name | Description |
|---|---|
| transactionReference | Indicates the unique reference for the sweep transaction which has initiated the funds request. |
| transactionDate | Indicates the business date on which the sweep transaction was initiated. |
| sweepingAccountId | Indicates the Account Reference/ID of the sweeping account in Transact. |
| sweepingAccountCurrency | Indicates the currency of the sweeping account. |
| contraCategoryOrAccount | Indicates the sweep suspense account. |
| accountId | Account Reference/ID of the external arrangement in Transact that represents the LOC/CC on the external systems. |
| alternateReferences | Collection – Contains details of all alternate ids applicable for the external arrangement in Transact. |
| paidOutAmount | Indicates the amount that is repaid to the LoC / CC in the external system. |
| currency | Indicates the Currency associated to the paidOutAmount. |
| alternateAccountType | Identifies the alternate account id type applicable for the associated alternate Id of the external arrangement in Transact. |
| alternateAccountId | Identifies the alternate account id applicable for the associated alternate account id type of the external arrangement in Transact. For example, Account Reference of the LOC / CC in the external system. |

**Misc**

| S.No. | Parameters | Description |
|---|---|---|
| 1. | AC.SWEEP.TYPE | This parameter table is used to create rules for various sweep types. Multiple AC.SWEEP.TYPE records can be created with many combinations of rules for each sweep type. |
| 2. | ACCOUNT.CLASS | To set up Notional Pooling, the ACCOUNT.CLASS records such as ICASUSPCR and ICASUSPDR must exist in the system. ICASUSPCR is used for credit interest postings ICASUSPDR is used for debit interest postings |
| 3. | ICA.HIERARCHY.PARAMETER | This must be setup before building any hierarchy in the system. Here, the record ID is the COMPANY code. This record contains the category and transaction codes for all possible types of Notional Pooling interest postings. |

**Misc**

| S.No. | Product Name | Features |
|---|---|---|
| 1. | Balance Netting Pool | Enables Corporates to manage their funds in an efficient and effective manner. Helps creation of a pool with relevant accounts, such as: Currency Top Account (CT) Master Account (MA) Currency Summary Account (CS) Summary Account (SA) Transaction Account (TR) Mirror Transaction Account (MTR) Credit and debit transactions within the cash pool are transparently diverted to the respective Currency Top Account. Such intra cash-pool transactions include: account-to-account transfers standing orders sweeps |
| 2. | Notional Pooling | Allows banks to offer corporate customers the ability to pool funds from different accounts without physical movement of funds. The balances are brought together notionally into a single pool account to calculate the interest. The interest earned in this pool account is redistributed among the customers' accounts. |
| 3. | Transactional Pooling | Physical Pooling helps in bringing together the balances of nominated accounts into a target account. Cash flow supports the following types of poolings: Maintenance Surplus Two Way Cash flow Create cash pool record checking the actual rules to see whether transfer of funds needs to be made from one account to another. Transaction Pooling can be run online or during the COB using overdraft Limits. |

**Notional Pooling**

| Field Name | Description |
|---|---|
| Dr Category | Identifies the category code assigned to the profit and loss debit entries generated, as a result of notional pooling. |
| Dr Txn Code Pl | Specifies the transaction codes for debit entries to profit and loss. |
| Dr Txn Code Ac | Specifies the transaction codes for debit entries to the customer accounts. |
| Dr Adj Categ, Dr Adj Txn Pl and Dr Adj Txn Pl | Specifies the debit adjustment entries. |

**Notional Pooling**

| Field Name | Description |
|---|---|
| Ica Main Account | Defines the main account in a notional pool hierarchy (to which this account belongs). A hierarchy consists of linked groups of accounts. Each group contains a main account along with an unlimited number of sub accounts. System populated field. A sub account in one group can be a main account in a lower level group. There can be an unlimited number of groups in a hierarchy. |
| Ica Main Acct Ind | When this field is set to Yes, it indicates that this account is the main account of the group. |
| Ica New Main Acc | Used to enter the main account that this sub account is linked to. A main account must also be linked to itself. It is used in conjunction with the Ica Start Date field . The Ica Start Date is the date on which this account joins the notional pool. |
| Ica Add Remove | Adds or removes an account to a hierarchy. |
| Ica Main Acct and Ica Main Date | Contain a historical list of main accounts and the start dates for the links to the main account are listed in chronological order starting with the most recent System maintained fields |

**Physical Pooling**

| Field Name | Amount |
|---|---|
| Cashflow Amount | 100,000.00 |
| Aggregate Bal | 50,000.00 |


---
