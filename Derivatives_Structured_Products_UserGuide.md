
# Temenos Transact — Derivatives_Structured_Products Module Documentation


> **Comprehensive User Guide**
> Generated: 13 April 2026
> Content: Configuration | Reference | Field Descriptions | Glossary


## Table of Contents

  - [Derivatives_Structured_Products Module Overview](#derivatives_structured_products-module-overview)
    - [Sub-Module Summary](#sub-module-summary)
    - [How to Use This Guide](#how-to-use-this-guide)
  - [Chapter 1: Derivatives_Structured_Products - DI](#chapter-1-derivatives_structured_products---di)
    - [Features in Derivatives_Structured_Products - DI](#features-in-derivatives_structured_products---di)
    - [1.1  DigitalInvestments](#11-digitalinvestments)
    - [1.2  Dual and Triple Currency Investments](#12-dual-and-triple-currency-investments)
    - [1.3  Misc](#13-misc)
  - [Chapter 2: Derivatives_Structured_Products - DP](#chapter-2-derivatives_structured_products---dp)
    - [Features in Derivatives_Structured_Products - DP](#features-in-derivatives_structured_products---dp)
    - [2.1  AccumulatorsAndDecumulators](#21-accumulatorsanddecumulators)
    - [2.2  Misc](#22-misc)
  - [Chapter 3: Derivatives](#chapter-3-derivatives)
    - [Features in Derivatives](#features-in-derivatives)
    - [3.1  Accounting](#31-accounting)
    - [3.2  Aggregation SEC.TRADE SSI](#32-aggregation-sectrade-ssi)
    - [3.3  Asian and Performance Options](#33-asian-and-performance-options)
    - [3.4  BasketOptions](#34-basketoptions)
    - [3.5  CDS](#35-cds)
    - [3.6  Close Out](#36-close-out)
    - [3.7  Commissions](#37-commissions)
    - [3.8  Constraints](#38-constraints)
    - [3.9  Corporate Actions](#39-corporate-actions)
    - [3.10  Derivatives Contract Master](#310-derivatives-contract-master)
    - [3.11  Derivatives Price Update](#311-derivatives-price-update)
    - [3.12  DX Package Option](#312-dx-package-option)
    - [3.13  Exotic Options](#313-exotic-options)
    - [3.14  FX OTC Options](#314-fx-otc-options)
    - [3.15  Limits](#315-limits)
    - [3.16  MarginCalculation](#316-margincalculation)
    - [3.17  Market Ex Profit](#317-market-ex-profit)
    - [3.18  MiFID Transaction Reporting](#318-mifid-transaction-reporting)
    - [3.19  Misc](#319-misc)
    - [3.20  Non Stop Processing](#320-non-stop-processing)
    - [3.21  Order Grouping](#321-order-grouping)
    - [3.22  Order Processing](#322-order-processing)
    - [3.23  Reporting](#323-reporting)
    - [3.24  Revaluation](#324-revaluation)
    - [3.25  Static setup](#325-static-setup)
    - [3.26  Swaptions](#326-swaptions)
    - [3.27  SWIFT MT306 for Exotic Options](#327-swift-mt306-for-exotic-options)
    - [3.28  Trade](#328-trade)
    - [3.29  Transaction Fees and Charges](#329-transaction-fees-and-charges)
    - [3.30  Transfers](#330-transfers)
    - [3.31  Misc](#331-misc)
    - [3.32  Misc](#332-misc)
  - [Chapter 4: Derivatives_Structured_Products - PT](#chapter-4-derivatives_structured_products---pt)
    - [4.1  PT](#41-pt)
  - [Chapter 5: Derivatives_Structured_Products - SY](#chapter-5-derivatives_structured_products---sy)
    - [Features in Derivatives_Structured_Products - SY](#features-in-derivatives_structured_products---sy)
    - [5.1  DigitalInvestments](#51-digitalinvestments)
    - [5.2  Dual and Triple Currency Investments](#52-dual-and-triple-currency-investments)
    - [5.3  Misc](#53-misc)
    - [5.4  Misc](#54-misc)
    - [5.5  XF](#55-xf)
    - [5.6  PT](#56-pt)
    - [5.7  AccountingValuation](#57-accountingvaluation)
    - [5.8  CommonFlow](#58-commonflow)
    - [5.9  CommonSetup](#59-commonsetup)
    - [5.10  CorporateActions](#510-corporateactions)
    - [5.11  Delivery](#511-delivery)
    - [5.12  Misc](#512-misc)
  - [Chapter 6: Derivatives_Structured_Products - XF](#chapter-6-derivatives_structured_products---xf)
    - [6.1  XF](#61-xf)
  - [Appendix A: Glossary of T24 Applications & Fields](#appendix-a-glossary-of-t24-applications-fields)
    - [Applications](#applications)
    - [Fields Referenced](#fields-referenced)
  - [Appendix B: Consolidated Field Reference](#appendix-b-consolidated-field-reference)
    - [Derivatives_Structured_Products - DI (DI)](#derivatives_structured_products---di-di)
    - [Derivatives_Structured_Products - DP (DP)](#derivatives_structured_products---dp-dp)
    - [Derivatives (DX)](#derivatives-dx)
    - [Derivatives_Structured_Products - PT (PT)](#derivatives_structured_products---pt-pt)
    - [Derivatives_Structured_Products - SY (SY)](#derivatives_structured_products---sy-sy)
    - [Derivatives_Structured_Products - XF (XF)](#derivatives_structured_products---xf-xf)

---


## Derivatives_Structured_Products Module Overview


This document provides comprehensive documentation for the **Derivatives_Structured_Products** module of Temenos Transact. It covers **6 sub-modules** with a total of **51 feature areas**.


### Sub-Module Summary


| # | Sub-Module | Code | Features | Description |
|---|-----------|------|----------|-------------|
| 1 | **Derivatives_Structured_Products - DI** | `DI` | 3 | Derivatives_Structured_Products - DI module of Temenos Transact |
| 2 | **Derivatives_Structured_Products - DP** | `DP` | 2 | Derivatives_Structured_Products - DP module of Temenos Transact |
| 3 | **Derivatives** | `DX` | 32 | Derivatives module of Temenos Transact |
| 4 | **Derivatives_Structured_Products - PT** | `PT` | 1 | Derivatives_Structured_Products - PT module of Temenos Transact |
| 5 | **Derivatives_Structured_Products - SY** | `SY` | 12 | Derivatives_Structured_Products - SY module of Temenos Transact |
| 6 | **Derivatives_Structured_Products - XF** | `XF` | 1 | Derivatives_Structured_Products - XF module of Temenos Transact |


### How to Use This Guide


Each feature in this document is organized into the following sections:

- 📖 **Introduction** — Overview and purpose of the feature
- ⚙️ **Configuration** — How to set up and configure the feature
- 🔧 **Working With** — Operational usage and field descriptions
- 📋 **Tasks** — Step-by-step procedures
- 📊 **Outputs** — Reports, enquiries, and generated outputs

Each feature includes a **Quick Reference Card** at the top with application names, key fields, prerequisites, and a summary. Appendices provide a full glossary, consolidated field tables, and end-to-end use-case scenarios.

---


## Chapter 1: Derivatives_Structured_Products - DI


Derivatives_Structured_Products - DI module of Temenos Transact


### Features in Derivatives_Structured_Products - DI


| # | Feature | Sections |
|---|---------|----------|
| 1.1 | DigitalInvestments | Intro, Confi, Worki, Tasks, Outpu |
| 1.2 | Dual and Triple Currency Investments | Intro, Confi, Worki, Tasks, Outpu |
| 1.3 | Misc | Intro |


### 1.1  DigitalInvestments


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Digital Investment is an OTC Structured Product, which links a traditional money market investment with the purchase of a digital option. The digital investment provides the investor the possibility to profit from an exchange rate and:*
> 
> **Key Fields:** *B2B Reference*, *Create Deposit*, *Create Option*, *Exercise Expire*, *New Maturity Date*, *Pay Out From Mm*, *Suppress Underlying*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The Digital Investment is an OTC Structured Product, which links a traditional money market investment with the purchase of a digital option. The digital investment provides the investor the possibility to profit from an exchange rate and:

- If the investor’s view is correct, a higher return is received than a conventional time deposit.
- If the investor’s view is incorrect, the return is less or zero, that is, the cash payout from the digital option is sent as an additional interest on the deposit.

The tower investment is a variant of digital investment. The major difference is that the digital investment has American barriers, that is, the monitoring of the spot exchange rate against the barriers happens continually. The digital and/or tower investment is principal protected, that is, the investor is assured of the investment amount redemption. The SY.DIGITAL.INVEST application records the transaction, which creates the underlying deposit and option based on the configuration. Temenos Transact can be parameterised either to handle the entire life cycle of the contract (standard flow) or to work as a back office system (interface flow).

- Full or Standard Flow - The core banking product does end to end processing of a digital investment, including the creation of the underlying option and deposit.
- Interfaced Flow - The bank uses an external software for the life cycle management of a digital investment contract and use the core banking product only as a back office system. The core banking product does not do the full processing. Instead, the system is designed to get the information from external systems and hold them together to form a single structured product contract.

The events in the life cycle of a digital invest contract are as follows.

| Event | Description |
|---|---|
| Inception | The contract is recorded in the system and the underlying option deal and deposit are created |
| Fixing | The fixing decision is made and the investor receives minimum or maximum rate, depending on the spot exchange rate, in comparison with the upper and lower barriers |
| Maturity | The contract expires on the maturity date and the deposit is redeemed |


#### ⚙️ Configuration

The SY.PRODUCT.DEFINITION application controls the functional and behavioural competencies of a digital investment contract. The events in the digital investment contract life cycle is defined in this application, which cannot be amended by the user. However, the user can amend the other parameters available in this application, and also set the category codes and transaction codes required to process a digital investment contract.

The bank can also extend the basic definition and create their own variants by setting up the records in SY.PRODUCT.VARIANT . The ID of this application contains two parts separated by ‘_’. The prefix is the product definition that is extended, while the suffix refers to the variants. All the parameters defined in the product definition are inherited by the product variant and can be amended. The configuration defined in the product variant takes precedence over the parameters defined in the product definition.

> **⚠️ Note:** The tower investment contracts would typically be a variant.


#### 🔧 Working With

For the digital investment feature to work in Temenos Transact , the SY.DIGITAL.INVEST application is used. The booking model and event processing methods are also mandatory for this feature.


##### Digital Investment for Structured Products

The SY.DIGITAL.INVEST application records a digital investment contract and its variants. A digital investment contract has an embedded deposit and an option contract. The terms of a digital investment contract are given in the below table.

| Term Sheet Element | Description |
|---|---|
| Value Date | Indicates the effective date of the contract |
| Deposit Currency | Indicates the currency of the deposit |
| Deposit Amount | Indicates the amount of the deposit in deposit currency |
| Tracking Currency | Indicates the tracking currency, which along with the deposit currency forms the currency pair. The spot exchange rate for this currency pair is tracked against the barrier rates. |
| Maximum Interest Rate | Indicates the maximum interest rate on the deposit if the option is in-the -money |
| Minimum Interest Rate | Indicates the minimum interest rate on the deposit. The investor receives the interest amount based on this rate, if the option expires worthless. |
| Upper Barrier | Indicates the upper barrier exchange rate for the digital option |
| Lower Barrier | Indicates the lower barrier exchange rate for the digital option |
| Maturity Date | Indicates the maturity date of the contract |

The Pay Out From Mm field indicates whether the bank wants to create the option on their books or they prefer to adjust the interest rate in the MM contract to effect the cash pay-out. If this field is set to Yes, option trade is not created. The payout is effected by adjusting the interest rate in the deposit. If this field is set to No, the option trade is created. On exercise of the option, the cash pay-out happens from the option and the deposit is redeemed with the minimum interest rate. This field must be set to No, when the profit and loss for this structured product needs to be segregated between the option and deposit.

Though the payout remains the same in the both the above approaches, the Profit and Loss for the option and deposit are posted to different P&L accounts in the second approach, while the Money Market (MM) P&L account is used for both the option and deposit components of the pay-out in the first approach. The user sets this field accordingly based on how the P&L must be treated.

Depending on the parameter setup, the following underlying transactions are created automatically by the system.

| Scenario | Parameter Setup | Underlying Transaction |
|---|---|---|
| 1 | Create Deposit = Yes, Create Option = Yes | Option created, deposit created |
| 2 | Create Deposit = No, Create Option = Yes | Option created |
| 3 | Create Deposit = Yes, Create Option = No | Deposit created |

In the standard or full mode of processing, the core banking product creates and manages the underlying transactions. This mode is selected by setting the Suppress Underlying field in SY.PRODUCT.DEFINITION to No. Thus, the Create Deposit and Create Option fields default to Yes.

In the interface mode of processing, the core -banking product creates the structure, while the underlying transactions are created by the upstream systems. A common reference and identifier bind the underlying transactions and structure together. The transactions created by the interface are also managed by the interface. For example, if the option is created by the interface, the exercise or expiry of the option must be triggered by the interface.

Further flexibility is available, where the core banking product creates one of the underlying transactions, while the other is updated from the interface. This can be achieved by setting either the Create Option or Create Deposit fields to Yes.


##### Booking Model

The bank is one of the parties to a digital or tower investment contract. The customer contract is hedged (covered) by entering into an opposing contract with a counterparty. A typical scenario is as below:

- Customer vs Dealer book (customer leg of the deal)
- Dealer book vs Counterparty (counterparty leg of the deal)

When dealing with a customer, the bank accepts a deposit. In the back-to-back deal with the counterparty, the bank places funds with the counterparty. The hedging can be either at individual deal or cumulative level.

- Individual level - Each customer deal is covered by a counterparty deal
- Cumulative level - Many customer deals are covered by a cumulative counterparty deal

The B2B Reference field in SY.DIGITAL.INVEST links the customer deal with the counterparty deal for reporting purposes.


##### Event Processing

The event processing involves the fixing and unwinding of contracts.

The decision as to whether the investor receives the minimum or maximum interest is communicated to the system by updating the Exercise Expire field in the contract. The investor receives maximum and minimum interest if this field is set to Exercise and Expire, respectively.

Once this is updated in the contract, the fixing event runs on the fixing date and updates the underlying transactions.

The unwinding is an early termination event. If the contract needs to be unwound, the New Maturity Date field can be updated to an earlier maturity date. It is also possible to charge a penalty for early termination.


#### 📋 Tasks

There are no Tasks available for Digital Investments feature.


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to Digital Investments in the core banking system.


##### Enquiries and Reports

The section helps the user to view the below enquiries and reports:

Trades List

This enquiry displays the list of all the digital investment contracts available in the core banking system.

Unwound Trades

This enquiry displays the list of all the digital investment unwound contracts.

Back to Back Trades

This enquiry displays the list of all the digital investment contracts with back-to-back reference.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


### 1.2  Dual and Triple Currency Investments


> **📇 Quick Reference Card**
> 
> **Purpose:** *Dual Currency Investments (DCI) are structured products that link a traditional Money Market (MM) investment to the sale of a Foreign Exchange (FX) call option on the invested currency or precious metal. The customer receives enhanced interest on the MM deposit. On maturity date, the customer receiv...*
> 
> **Key Fields:** *Agency Booking Model*, *Alternate Ccy1*, *B2B Reference*, *Convert Interest*, *Create Deposit*, *Create Option*, *Interest Currency*, *Local Or Source* ... +9 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Dual Currency Investments (DCI) are structured products that link a traditional Money Market (MM) investment to the sale of a Foreign Exchange (FX) call option on the invested currency or precious metal. The customer receives enhanced interest on the MM deposit. On maturity date, the customer receives the redemption amount either in the deposit currency or in the alternate currency. The redemption is in the alternate currency if the currency option is in-the-money from the bank’s perspective.

Triple Currency Investment (TCI) is similar to DCI, the difference is that the presence of a third currency attribute. The redemption might be in deposit currency or in any one of the alternate currencies.

DCI and TCI contracts are not principal protected. When the redemption is in the alternate currency, the investor incurs a loss depending on exchange rate movement and it is possible for such a loss to reduce the principal. Temenos Transact is parameterised to handle the entire life cycle of the contract (standard flow) or to work as a back office system (Interface flow).

- Full or standard flow – Temenos Transact does end-to-end processing of a DCI and TCI contract, including the creation of the underlying deposit and the currency option. On the maturity date, the system either exercises or expires the currency option. The decision to exercise or expire is determined by the user and is communicated to the system by setting the relevant fields. If the option is exercised, the redemption amount from the deposit is converted to the alternate currency by booking an FX spot deal. If the option is expired, then the redemption is in the deposit currency.
- Interfaced Flow - If the banks uses the external software for life cycle management of a DCI and TCI contract and uses Temenos Transact only as a back-office system, then full processing is not done by Temenos Transact . Instead, the system gets the information from external systems and holds them together to form a single SY contract.

> **⚠️ Note:** The full or standard flow and interfaced flow do not apply for the agency booking model.

The terms of a DCI and TCI contract are explained in the following table.

| Term Sheet Element | Description |
|---|---|
| Value Date | Effective date of the deposit |
| Deposit Currency | Currency of the deposit |
| Deposit amount | The principal investment amount |
| Alternate Currency | Alternate currency |
| Strike Exchange Rate | Agreed forward exchange rate between the deposit currency and the alternate currency |
| Interest Rate | Enhanced interest rate for the deposit |
| Fixing date | The date on which the spot exchange rate is compared against the strike price and exercise or expire decision is made |
| Maturity date | Maturity date of the deposit or contract |
| Alternate currency 2 | Applicable for TCI contracts only. This is the other alternate currency |
| Strike exchange rate 2 | Applicable for TCI contracts only. Agreed forward exchange rate between the deposit currency and alternate currency 2 |

The events in the life cycle of a DCI and TCI contracts are explained in the following table.

| Event | Description |
|---|---|
| Inception | The contract is recorded in the system. The underlying deposit and option transaction are created |
| Fixing | Decision event. The spot exchange rate is compared against the strike exchange rate; the user decides whether to exercise or expire the currency option. |
| Maturity | The deposit matures and depending on the fixing decision, the redemption amount is either converted to the alternate currency (through a FX spot deal) or redeemed in the deposit currency. This event would be scheduled to run on the maturity. |
| Unwinding | Unwinding is an early termination event whereby the maturity date can be advanced to an earlier date. |

There are variants of DCI that is traded in the market. Few of these variants are explained in the following table.

| Variant | Description |
|---|---|
| Precious Metal Investments | In this variant, either the deposit currency or the alternate currency is a precious metal defined as a currency in the system |
| DCI with barriers | In this variant, the currency option is a barrier option. Option can have knock-in or knock-out features. In Temenos Transact terms, this is defined as an exotic option |
| Principal only conversion | In this variant, if the option is exercised, then only the principal is converted to the alternate currency. The interest amount is repaid in the deposit currency |
| Tripe Currency Investment | In this variant, there are two alternate currencies. The redemption can be in the deposit currency or in any of the alternate currencies |


#### ⚙️ Configuration

The SY.PRODUCT.DEFINITION parameter application controls the functionality and behaviour of a DCI and TCI contract. The events in the life cycle of a DCI and TCI contract are defined in this application. These events cannot be amended by the user. However, the user can amend the other parameters available in this application and also set the category codes and transaction codes required to process the DCI and TCI contracts.

Banks can also extend the basic definition and create their own variants. This is achieved by setting up records in SY.PRODUCT.VARIANT record. The ID of this application contains two parts separated by an underscore (_). The prefix is the product definition that is being extended, while the suffix refers to the variants. All the parameters defined in the product definition are inherited by the product variant and can be amended. The configuration defined in the product variant takes precedence over the one defined in the product definition.


#### 🔧 Working With

The SY.DCI application is used to transact in DCI and TCI contract and its variants.


##### Transaction Booking Model

Temenos Transact supports two types of transaction booking models. The booking model is identified by the Agency Booking Model field in SY.PRODUCT.DEFINITION and SY.PRODUCT.VARIANT applications. When this field is set to Yes, the Agency booking model is enabled and when set to No, the principal booking model is enabled.

| Scenario | Parameter Setup | Underlying Transaction |
|---|---|---|
| 1 | Create Deposit = Yes, Create Option = Yes | Option created, Deposit created |
| 2 | Create Deposit = No, Create Option = Yes | Option created |
| 3 | Create Deposit = Yes, Create Option = No | Deposit created |

| Credit or Debit Indicator | Account | Date | Amount (In alternate currency) |
|---|---|---|---|
| Dr | Counterparty’s alternate currency account | Maturity date | Principal plus interest |
| Cr | Customer’s alternate currency account | Maturity date | Principal plus interest |


##### Interest Processing for Precious Metal Contracts

Where the deposit is in a precious metal currency, it is possible to specify an interest currency. The interest pay-out is made in this currency. The interest would be calculated in the deposit currency and converted to the interest currency (at the time of fixing) using the spot exchange rate.

This is applicable only when the deposit is redeemed (option is expired) in the deposit currency or when the Convert Interest field is set to No. When the deposit is redeemed in the alternate currency (option is exercised), the interest currency is not relevant. In such cases, the interest is converted to the alternate currency using the strike price (exchange rate). This scenario is explained in the below table:

| Convert Interest = No | Convert Interest = Yes |  |  |
|---|---|---|---|
| Exercise | Expiry | Exercise | Expiry |
| FX for principal amount | Principal in dep CCY | FX for Principal + Interest | Principal in dep CCY |
| Interest in Interest Currency @ Spot | Interest in Interest Currency @ Spot | Interest in Interest Currency @ Spot |  |


#### 📋 Tasks

Related topics:

- Manage Processing of DCI or TCI (SY)
- Trading Processes

Dual Currency Investments (DCI) are structured products that link a traditional money market investment to the sale of a Forex (FX) Call Option on the invested currency or precious metal. The customers receive enhanced interest on the Money Market Deposit. On Maturity date, the customer receives the redemption amount either in the Deposit Currency or in the alternate Currency. Redemption might be in the alternate Currency, if the Currency Option is in the money from the bank’s perspective.

Triple Currency Investment (TCI) is similar to DCI, the difference being the presence of a third Currency attribute. Redemption might be in Deposit Currency or in any one of the alternate Currency.


##### Workflow

The user can process the Dual Currency and Triple Currency Investments by using the below workflows:

This enquiry displays the list of all unauthorized dual currency investment and triple currency investment contracts for own book.

To view the trades, follow the below steps:

1. Authorise Dual/Triple Ccy Investments .
2. In Unauthorised DCI/TCI Trades screen, click the View icon.

To authorise the trades, follow the below steps:

1. Authorise Dual/Triple Ccy Investments .
2. In Unauthorised DCI/TCI Trades screen, click the Authorise icon.
3. In DCI Agency Booking/ Triple Currency Investments screen, click the Authorise icon.

To delete the trades, perform the following steps

1. Authorise Dual/Triple Ccy Investments .
2. In Unauthorised DCI/TCI Trades screen, click the Delete icon.
3. In DCI Agency Booking/ Triple Currency Investments screen, click the Delete icon.


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to Dual and Triple Currency Investments in the core banking system.


##### Enquiries and Reports

The section helps the user to view the below list of enquiries and reports:C

Trades List

This enquiry displays the list of dual currency contracts with the corresponding underlying trades.

Exotic Trades

This enquiry displays the list of exotic dual currency contracts.

Exotic Trades Triggered

This enquiry displays the list of exotic dual currency contracts for which exotics are triggered.

Back to Back Trades

This enquiry displays the list of all dual currency contracts and their corresponding back to back trades.

Prematured Trades

This enquiry displays the list of pre-maturing dual currency investment contracts.

In and Out of Money

This enquiry displays the status of all the dual currency investment contracts. Based on the status, the user can redeem the deposit either in alternate currency or contract currency.

Trades List

This enquiry displays the list of triple currency investment contracts with the corresponding underlying trades.

Exotic Trades

This enquiry displays the list of exotic triple currency investment contracts available in the core banking system.

Exotic Trades Triggered

This enquiry displays the list of triple currency investment contracts for which exotic is triggered.

Prematured Trades

This enquiry displays the details of all the pre-maturing triple currency investment contracts.

In and Out of Money

This enquiry status of all the triple currency investment contracts. Based on the status, the user can redeem the deposit either in alternate currency or in contract currency.

Back to Back Trades

This enquiry displays the list of all the triple currency back-to-back trades.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


### 1.3  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *Introduction to Retail Sweeping ⓘ Content migrated: Old structure mapped (To be planned)*
> 
> **Key Fields:** *Alternate Ccy 1*, *Alternate Ccy 2*, *Alternate.Ccy.2*, *Exercise Ccy*, *Exercise Ccy,*, *Exercise Expire*, *First Date*, *Last Date* ... +6 more
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Introduction to Retail Sweeping ⓘ Content migrated: Old structure mapped (To be planned)

Related topics:

- Temenos Transact Services

This module handles two business products namely:

- Dual and Triple Currency Investments
- Digital Investments


##### Product Configuration

Read the below configuration sections for setting up the functionality of Dual/Triple Currency and Digital Investments (DI) module.

- Dual and Triple Currency Investments
- Digital Investments


##### Illustrating Model Parameters

The model parameters for Digital Investments (DI) are explained below:

Dual Currency Investments (DCI) are Structured Products (SY) that link a traditional Money Market (MM) investment to the sale of an FX call option on the invested currency or precious metal. The customer receives enhanced interest on the MM deposit. On maturity date, the customer receives the redemption amount either in the deposit currency or in the alternate currency. The redemption is in the alternate currency, if the currency option is in-the-money from the bank’s perspective.

Triple Currency Investment (TCI) is similar to DCI, the difference is that the presence of a third currency attribute. The redemption might be in deposit currency or in any one of the alternate currencies.

DCI and TCI contracts are not principal protected. When the redemption is in the alternate currency, the investor incurs a loss depending on exchange rate movement. It is possible for such a loss to reduce the principal.

| Field | Description |
|---|---|
| Variant | Variant for the contract to use the said categories based on the SY.PRODUCT.VARIANT selected. |
| Trade Date | Holds the trade date of the contract. Trade date cannot be forward dated and should fall between the First Date and Last Date of the corresponding product definition record. |
| Maturity Date | Maturity date is the termination date of the contract. Maturity date will be defaulted based on Term and Value Date . |
| Trade Ccy | This is the deposit currency in which the customer deposit or takes loan in MM.MONEY.MARKET . Is the Trade Ccy of DX.TRADE . |
| Alternate Ccy 1 | The alternate currency in which the deposit amount is paid back, that is, the delivery currency in DX.TRADE and the other currency in FOREX |
| Alternate.Ccy.2 | The second alternate currency in which the deposit amount is paid back, that is, this field enables the triple currency investment. On exercise of option FOREX gets created between Trade Ccy and Alternate Ccy 2 . The option trade between Trade Ccy and Alternate Ccy 1 is expired. |
| Exercise Expire | When the field is set to EXERCISE the option contract is exercised and when set to EXPIRE the option contract is expired. The value to the field can be manually determined. When not the fixing event determines the value to this field. The fixing routine to have 2 parameter which are outcoming. The 1st to hold the EXERCISE or EXPIRE as value saying the decision and the second to hold the Exercise Ccy, if suppose the decision is to exercise the option contract. |
| Exercise Ccy | The currency in which the forex is created when it is Alternate Ccy 1 then the DX.TRADE is exercised. When it is Alternate Ccy 2 then it means the DX.TRADE between trade and first alternate currency is expired and a new FX gets created between Trade Ccy and Alternate Ccy 2 . |

| Element | Description |
|---|---|
| Value date | Effective date of the deposit |
| Deposit currency | Currency of the deposit |
| Deposit amount | The principal investment amount |
| Alternate currency | Alternate currency used |
| Strike exchange rate | Agreed forward exchange rate between the deposit currency and the alternate currency |
| Interest rate | Enhanced interest rate for the deposit |
| Fixing date | The date on which, the spot exchange rate is compared against the strike price and exercise or expire decision is made. |
| Maturity date | Maturity date of the deposit or contract |
| Alternate currency 2 | Applicable for TCI contracts only. This is the other alternate currency. |
| Strike exchange rate 2 | Applicable for TCI contracts only. Agreed forward exchange rate between the deposit currency and alternate currency. |

| Event | Description |
|---|---|
| Inception | The contract is recorded in the system. The underlying deposit and option transaction are created. |
| Fixing | Decision event. The spot exchange rate is compared against the strike exchange rate. The user decides whether to exercise or expire the currency option. |
| Maturity | The Deposit matures and depending on the fixing decision, the redemption amount, is either converted to the alternate currency (through a FX Spot Deal) or redeemed in the deposit currency. This event is scheduled to run on the maturity. |
| Unwinding | Unwinding is an early termination event, where the maturity date can be advanced to an earlier date. |

| Variant | Description |
|---|---|
| Precious metal investments | In this variant, either the deposit currency or the alternate currency, is a precious metal defined as a currency in the system. DCI with barriers - In this variant, the currency option is a barrier option. Option can have knock-in or knock-out features. In Temenos Transact terms, this is defined as an exotic option. |
| Principal only conversion | In this variant, if the option is exercised, then only the principal is converted to the alternate currency. The interest amount is repaid in the deposit currency. |
| Tripe currency investment | In this variant, there are two alternate currencies. The redemption can be in the deposit currency or in any of the alternate currencies. |


##### Illustrating Model Products

Model products are not applicable for this module.

---


---


## Chapter 2: Derivatives_Structured_Products - DP


Derivatives_Structured_Products - DP module of Temenos Transact


### Features in Derivatives_Structured_Products - DP


| # | Feature | Sections |
|---|---------|----------|
| 2.1 | AccumulatorsAndDecumulators | Confi, Worki, Tasks, Outpu |
| 2.2 | Misc | Intro |


### 2.1  AccumulatorsAndDecumulators


> **📇 Quick Reference Card**
> 
> **Key Fields:** *Accrual Basis*, *Accrued Units1*, *Agency Booking Model*, *Alternate Ccy1*, *Apply Leverage*, *B2B Reference*, *Block Amount*, *Block Nominal* ... +45 more
> 
> **Sections:** ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### ⚙️ Configuration

The SY.PRODUCT.DEFINITION application is used to control the functionality and behaviour of an accumulator or decumulator transaction. The events in the life cycle of an accumulator or decumulator contract is defined in this application. These events cannot be amended by the user. However, the user can amend other parameters available in this application and also set the category codes and transaction codes required to process an accumulator contract.

The bank can also extend the basic definition and create their own variants. The user can setup records in the SY.PRODUCT.VARIANT application to create the variants. The ID of this application contains two parts separated by '_'. The prefix is the product definition that is being extended, while the suffix refers to the variants. All the parameters defined in the product definition are inherited by the product variant and can be amended. The configuration defined in the product variant takes precedence over the one defined in the product definition.


#### 🔧 Working With

The SY.ACCU.DECU application is used to transact in accumulator and decumulator contracts. The Product Type field indicates whether the contract entered is an accumulator or decumulator.


##### Illustrating Transaction Booking Model

Temenos Transact supports two types of transaction booking models. The Agency Booking Model field in the SY.PRODUCT.DEFINITION and SY.PRODUCT.VARIANT applications, identifies the booking model. When this field is set to Yes, the agency booking model is enabled and when set as No, the principal booking model is enabled.

The user must input the details and terms in SY.ACCU.DECU record and populate all the required fields. When this record is committed, the system creates the underlying option using the DX.TRADE application for the full lots (including gearing). The underlying option is SELL PUT in the customer side for an accumulator and SELL CALL in the customer side for a decumulator.

The fields from the SY.ACCU.DECU record are mapped to the underlying DX.TRADE application and any overrides or errors in the accumulator and decumulator contracts are raised against the SY.ACCU.DECU contract, so that the user can validate. Upon authorising the SY.ACCU.DECU record, the underlying option is automatically authorised (if Suppress Underlying is set to No). The lots of underling option is determined by the below formula:

The SY.TRANSACTION record is built and other SY log tables are updated. The bank is one of the parties to any accumulator or decumulator contract. The customer contract is often hedged or covered by entering into an opposing contract with a counterparty. Thus, a typical scenario is as explained below:

- Customer vs dealer book (customer leg of the deal).
- Dealer book vs counterparty (counterparty leg of the deal).

Hedging can be at,

- Individual deal level - A counterparty deal covers each customer deal
- Cumulative level - A cumulative counterparty deal covers many customer deals

The B2B Reference field is used to link the customer deal with the counterparty deal. This linkage is used for reporting purposes.

> **⚠️ Note:** The Sy Master field is not mandatory, as the user could define the currency pair through the Trade Ccy and Alternate Ccy1 fields. If a Sy Master is attached, Risk Level is defaulted from the Sy Master field, which facilitates the input of Risk Level directly in the transaction.

| S.No | SY.ACCU.DECU | SEC.TRADE |
|---|---|---|
| 1. | Security Code | Security Code |
| 2. | Fixing Date (From the current fixing period multi value set) | Trade Date |
| 3. | Settlement Date (From the current fixing period multi-value set) | Value Date |
| 4. | Customer | Customer No |
| 5. | Counterparty | Broker No |
| 6. | Accrued Units1 (From the current fixing period multi-value set) | Cust No Nom |
| 7. | Strike Price1 | Cust Price |
| 8. | Product Type | If Product Type = Accumulator, Cust Trans Code = BUY. Else, Cust Trans Code = SEL |
| 9. | Sy Dx Reference | Sy Dx Reference |
| 10. | Trans Reference | Sy Trans Id |


##### Event Processing

Various events such as fixing event and knock-out event are possible in the life cycle of an accumulator or decumulator contract. These events can be scheduled to run during the COB batch processing or hoc by the user.

This event is scheduled to run on every working day. The accrual is performed based on the current market price. If the current market price is less than the strike price of the contract, the gearing factor is applied. Depending on the value in the Accrual Basis field in the SY.PRODUCT.DEFINITION application, either the first or last day or both the days are included for accrual. The accrued units are updated in the Accrued Units1 field, which can be amended by the user.

The contracts for which the knock-in price is updated, the accrual is commenced only when Knock In field is set to Yes, that is, only when the contract is knocked in. If the Geared Accrual field in the SY.PRODUCT.DEFINITION or SY.PRODUCT.VARIANT applications is set to YES, the accrual applies gearing factor without comparing the spot price to the strike price. This applies to the scenario, where the accrual reflects the worst case scenario.

The Accrual Basis field accepts an additional drop-down value No Accrual. When this option is selected, the system does not process accrual during COB. In this case, the value in the Accrued Units1 field is updated by the user or from an upstream interface.

The Suspend Accrual field is used to suspend the accrual process. The requirement to suspend accrual arises due to the following:

- The underlying security may not be traded in the market due to a Corporate Action (CA) event.
- The STOCK.EXCHANGE might have an unscheduled emergency holiday.

The suspension can be reset by updating the reset date in the Susp Reset Date field.

Fixing event is the periodical settlement event. This is a scheduled event which takes place based on the fixing frequency or schedule. The user can make amendments to the system calculated values, while this event runs in COB.

- The Accrued Units1 field is amended to change the system calculated accrual values.
- The Market Price1 and Settlement Amount1 fields are updated for cash settled contracts.
- The Sett Instr Units and Sett Instr Price is updated for contracts pay out through participatory notes.

When the fixing event runs, the option exercised for the accrued units and the residual units (maximum possible accrual less the accrued units) is expired. Thus fixing results in both a partial exercise and partial expire of the option.

Each fixing period is represented as a multi-value set. Once a particular fixing is processed, the field Fixed Status is updated as FIXED and the corresponding multi value set cannot be amended.

> **⚠️ Note:** For principal booking transaction model, the option is exercised for creation of the SEC.TRADE record. In the case of agency transaction booking model, the SEC.TRADE is created directly from the accumulator or decumulator contract.

The accumulator or decumulator contract can be knocked out, when the knock-out price is breached. This is indicated to the system by setting the Knock Out field to Yes. The knock-out event runs when the contract is flagged as knocked out. The option is exercised for the accrued units of the current fixing period. This is a termination event, where the off balance sheet entries are dropped, the security and fund block is released and the contract is marked as knocked out.

> **⚠️ Note:** For principal booking transaction model, the option is exercised for creation of the SEC.TRADE record. In the case of agency transaction booking model, the SEC.TRADE is created directly from the accumulator or decumulator contract.

Contract can be unwound, at any point of time. It can be a full or partial unwind.

- Full unwind - Contract is closed.
- Partial unwind - Obligation is reduced.

Unwind related multi-value set of fields are used to flag the contract as unwound and also define penalty charges. The unwind effective date needs to be within the current fixing period. In case of a full unwind, the unwind set of fields cannot be multi valued. For partial unwind, it is possible to multi-value these fields to capture further partial unwinds.

For partial unwind, the New Daily Units field must be populated and all subsequent accrual are based on this value. In case of back-dated unwind (that is, unwind effective date is earlier than today), the accrued units must be corrected manually. The event Unwinding Adhoc should be run as ad hoc event to process the partial knock-out.

Full unwind is event termination. If the unwind effective date is later than the last fixing date, the option is exercised for the accrued units of the current fixing. The unwind event is scheduled to run on the date of amendment (setting of the unwind flag) or the unwind effective date (whichever is later).

> **⚠️ Note:** For principal booking transaction model, the option is exercised for creation of the SEC.TRADE record. In the case of agency transaction booking model, the SEC.TRADE is created directly from the accumulator or decumulator contract.

Contract can be novated to an external party or it could be an internal novation. The value in the Novation field in the SY.ACCU.DECU application determines the type of novation. The Novated To and Novated From fields are used to capture additional novation information.

An optional novation fee can also be charged. Novation is also a termination event, where the blocks are released and notional entries are reversed.


##### Defining Calendar

The Calendar field in the SY.ACCU.DECU application accepts a valid region, as defined in the REGION application. The calendar defined for this region is referred for building the fixing schedule and working out the total number of working days. The same calendar is used for the accrual process.

The transaction is synchronised with the Calendar on each fixing date (as part of the fixing event). The remaining number of working days are recalculated at each fixing.

> **⚠️ Note:** Any changes to calendar for the current fixing period are not recognized by the system. The Suspend Accrual functionality is used in scenarios, where there is an emergency holiday declaration (for example, Typhoon).


##### Defining Limit Update

If limit is setup for SY.ACCU.DECU contracts, the limit reference is defaulted to the Limit Ref field. The SY.ACCU.DECU application passes on the amount that is updated as the total outstanding amount in the LIMIT application. The limit is updated at the following stages:

- Inception - Contract is booked. At the time of inception, the limit is updated to the extent of Notional Amt field.
- Fixing - Periodical settlement. At each fixing, the obligation reduces. The outstanding obligation is available in the Run Notional Amt field. The limit is updated such that the outstanding amount is equal to the Run Notional Amt field.
- Termination or maturity - During termination or maturity, the outstanding amount for this contract is zero


##### Blocking

The user can block funds for an accumulator contract or can block shares for a decumulator contract. The Block Amount and Block Nominal fields are updated to block the funds or shares, respectively. The end date of block can be specified in the Block Until field. Unblock happens automatically on the end date of the block. If the contract is terminated before the end date, (due to a knock-out event, an unwind event or any event leading to termination of the contract), all the blocks are released.

For the security block, blocking set of fields are multi-valued to create multiple blocks. This is required, when the underlying is held in different depositories and sub-accounts and where there is more than one security position for the same underlying security. The multi-value can also be used to setup a staggered blocking and unblocking schedule. The Covered Contract field in the SY.ACCU.DECU application determines the type of security block as explained below:

- Uncovered - For uncovered contracts, blocking is not required.
- Partially Covered - For the partially covered contracts, the user manually enters the quantity and duration of the block in the Block Nominal and Block Until fields.
- Fully Covered - The blocking functionality for the fully covered contracts are explained in the following sections.

- Inception - When the decumulator contract is first captured, the obligation nominal is stored in the Total Units field (which includes geared nominal) and the security position is blocked using the SC.BLOCK.SEC.POS blocking application. The nominals to be blocked are equal to Total Units . The blocking is done automatically by the system for fully covered contracts.
- Fixing - Obligation is reduced at each fixing and the same is tracked through the Remaining Units fields. As a part of the fixing event, the block is adjusted such that the blocked position is only to the extent of Remaining Units (gearing is applied).
- Termination - At termination, all the blocks is released.


#### 📋 Tasks

Related topics:

- Manage Processing of DCI or TCI (SY)
- Administration and Static Data and Corporate Actions

Accumulators allow an investor to accumulate a fixed quantity of an underlying share at the strike price, on each trading day of the investment period and are usually structured with a knock-out feature. This means that the accumulators are terminated, when the price of the underlying share closes at or above a pre-determined barrier price (also known as knock-out price), which is set above the initial spot price. Shares are purchased and accrued on a daily basis. Settlement of aggregate accumulation occurs regularly on pre-determined settlement dates.

Decumulators on the other hand, allow investors to sell a fixed quantity of an underlying share at a pre-determined strike price, on each trading day of the investment period. This forward price is set at a premium to the initial spot price of the underlying share.

In the core banking system, there are applications to enter accumulator and decumulator contracts. The Product Type field in the SY.ACCU.DECU application indicates whether the contract entered is an accumulator or a decumulator.

The user has to enter values in all the required fields. When the record is authorised, the system creates the underlying option (which might be a sell or put on the customer side for an accumulator and sell or call on the customer side for a decumulator) automatically.


##### Workflow

In Accumulators and Decumulators, the user can perform the following activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Trades List . |
| Accu Decu Trades | Enter values in the required fields. Click the FIND button. |
| List of Accumulator/Decumulator trades | Click the View Underlying Trade icon corresponding to a record. |
| Trade Details | Verify the record details. |

This enquiry displays the list of fixing (periodical settlement) details of FX accumulator or decumulator contracts, which enables the user to exercise or expire the contracts with an option to apply for leverage.

To enable the exercise or expire option and apply leverages, perform the following steps:

1. Fixing Schedules .
2. Enter the EXPIRE or EXERCISE option in the column Exercise/Expire field and the YES or NO option in the Apply Leverage field.
3. Click the Apply the chosen operation to the selected row(s) button.


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to accumulators and decumulators in the core banking system.


##### Enquiries and Reports

The user can view the following enquiries and reports:

Back to Back Trades

This enquiry displays the list of all the back to back trades along with the open positions.

Fixing Schedule

This enquiry displays the fixing schedule of all the accumulator and decumulator trades along with the accrued units after each fixing.

Blocked Position

This enquiry displays the list of all the accumulator and decumulator trades for which the positions are blocked.

Suspended Trades

This enquiry displays the list of all the suspended accumulator and decumulator trades along with the details of suspension.

Knocked in Trades

This enquiry displays the list of all the accumulator and decumulator trades which are knocked in.

Knocked out Trades

This enquiry displays the list of all the accumulator and decumulator trades which are knocked out.

Funds Blocked

This enquiry displays the list of all the accumulator and decumulator trades for which the funds are blocked.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


### 2.2  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *Introduction to Retail Sweeping ⓘ Content migrated: Old structure mapped (To be planned)*
> 
> **Key Fields:** *Contract Status*, *Daily Units*, *First Date*, *Fixing Frequency*, *Last Date*, *Maturity Date*, *Option Type*, *Product Type* ... +4 more
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Introduction to Retail Sweeping ⓘ Content migrated: Old structure mapped (To be planned)

Related topics:

- Temenos Transact Services

Accumulators allow an investor to accumulate, a fixed quantity of an underlying share at the strike price, on each trading day of the investment period. Accumulators are usually structured with a knock-out feature. This means that the accumulators are terminated, when the price of the underlying share closes at or above a pre-determined barrier price (also known as knock-out price), which is set above the initial spot price. Shares are purchased and accrued on a daily basis. Settlement of aggregate accumulation occurs regularly on pre-determined settlement dates.

On the other hand, decumulators allows the investors to sell a fixed quantity of an underlying share at a pre-determined strike price, on each trading day of the investment period. This forward price is set at a premium to the initial spot price of the underlying share. Decumulators are also structured with a knock-out feature and are terminated early when the price of the underlying share closes at or below a pre-determined barrier. When the price of the underlying share closes at or below the pre-determined barrier price, a knock-out event occurs.


##### Product Configuration

Temenos Transact is parameterised either to handle the entire life cycle of the contract (standard flow) or to work as a back-office system (interface flow).

- Full or standard flow - Temenos Transact does an end-to-end processing of SY.ACCU.DECU including the creation of the underlying option. On each settlement date, the system creates a SEC.TRADE for the accrued units by exercising the option and reduces the outstanding nominal in the option trade. On knock-out or on maturity, the system creates a SEC.TRADE for accrued units and expires the option.
- Interfaced flow - If the banks use other external software for life cycle management of SY.ACCU.DECU and use Temenos Transact only as a back-office system, Temenos Transact does not perform the full processing. Instead, the system is designed to get the information from external systems and hold them together to form a single SY contract. The full or standard flow and interfaced flow do not apply for the agency booking model.

The key terms in accumulator or decumulator contract are explained in the following table.

| Term sheet element | Description |
|---|---|
| Value Date | Commences the contractual obligation from this date |
| Underlying security | Denotes the underlying security which is accumulated or decumulated over the tenor of the contract |
| Strike Price | Denotes the forward price at which the underlying security is purchased or sold |
| Knock out price | Denotes the barrier price. When the spot price of the underlying security breaches this barrier, the contract gets knocked out (terminated). |
| Daily units | Denotes the number of shares that must be accrued on a daily basis |
| Gearing Factor | Applies on the days, when the spot price of the underlying is unfavorable to the investor comparing the strike price |
| Fixing Frequency | Denotes the periodicity at which the settlement of accumulated or decumulated shares occur |
| Maturity Date | Denotes the date on which the contractual obligation ends |

The events in the life cycle of an accumulator or decumulator contract are explained in the following table.

| Event | Description |
|---|---|
| Inception | Commences contractual obligation for the investor. The contract is recorded in the system and the underlying option trade is created. |
| Accrual | Units (of the underlying security) are accrued on a daily basis. For contracts with gearing factor, the gearing factors are applied on the days when the spot price of the underlying is unfavourable to the investor comparing the strike price of the contract. |
| Fixing | Effects the settlement of the accumulated or decumulated shares. The underlying option is exercised and this creates the SEC.TRADE transaction for the underlying security. This is a scheduled periodic event. |
| Knockout | Occurs when the price barrier is breached, that is, when the spot price of the underlying touches the knock-out price. When this event occurs, the contract is terminated. |
| Unwinding | Terminates the contract either fully or partially. In a full unwind, the contract is terminated earlier. In a partial unwind, the contract continues to be active, but the obligation (that is, daily accrual units) is reduced for the rest of the contract period. |
| Novation | Transfers the contract between customers and banks. Internal novation - Contract is transferred from one customer account to another External novation - Contract is transferred from customer account in one bank to another |
| Maturity | Indicates the end date of the contract. The contractual obligation ceases on this date. |

The variants of accumulator or decumulator contracts, prevalent in the market are explained in the following table.

| Variant | Description |
|---|---|
| Non-leveraged accumulator or decumulator | Denotes the plain vanilla accumulator without a gearing factor |
| Leveraged accumulator | Holds an additional attribute that is, gearing factor. Gearing factor is applied to the accrual on the days when the spot price is unfavourable to the customer, comparing the strike price. The potential loss to the investor is higher in this variant, compared to the plain vanilla variant. |
| Guaranteed accumulator or decumulator | Assures the investor of guaranteed accumulation. That is, a certain number of underlying shares might be accumulated or decumulated and settled, even if the knock-out price barrier is breached early in the life of the accumulator contract. |

The following features are available in this product:

For certain emerging markets, off market transfers are prohibited by regulations or policies (for example, Taiwanese shares). Accumulators with such shares as underlying are either cash settled or settled through a participatory note.

The accumulators or decumulators can be cash settled, that is, at the time of fixing, instead of delivering the shares, the cash difference between the strike price and market price can be settled. Strike price is one of the terms of the contract, whereas the market price varies at the time of fixing. Market price can be updated at the time of fixing, based on which Temenos Transact calculates the settlement amount.

Markets can be disrupted due to natural calamities such as typhoon. On such occurrences, the accrual needs to be suspended on that day and resumed once the market is open for trading. The suspension of accrual is updated in the STOCK.EXCHANGE application.

For direct equity transactions, stamp tax is calculated on the trade cost, for equity transactions arising out of accumulators or decumulators, the stamp tax is calculated based on the quantity of units purchased multiplied by the stamp duty price. The stamp duty price is determined as:

Unwind happens anytime during the life cycle of an accumulator or decumulator contract. If unwinding happens in the middle of a fixing period, the customer can settle the shares accumulated in the current fixing period. However, the share settlement takes place only on the subsequent fixing date. Also, the customer can choose not to settle the shares for current fixing period (in such cases, the penalty is higher). It is also possible to do a partial unwinding, that is, reduce the obligation nominals.

There are two types of novation as explained below:

- External novation occurs when the position is transferred outside the bank.
- Internal novation occurs when the position is transferred from one customer account to another customer account (for example, from an individual account of a customer to a joint account).

> **⚠️ Note:** An optional novation fee is also charged.

If the bank acts the principal for the accumulator contract, it can act either as principal or agent for the share settlement, which depends on the type of legal agreement signed with the client and counterparty. Therefore, the Settlement Role field in the SY.ACCU.DECU application accepts the PRINCIPAL or AGENT values. The value in this field is mapped to the share settlement transaction and it is subsequently used for stamp tax calculation.


##### Illustrating Model Parameters

The model parameters for Equity Accumulator (DP) are explained below:

Accumulators allow an investor to accumulate, a fixed quantity of an underlying share at the strike price, on each trading day of the investment period. Accumulators are usually structured with a knock-out feature. This means the accumulators are terminated, when the price of the underlying share closes at or above a pre-determined barrier price (also known as knock-out price), which is set above the initial spot price. Shares are purchased and accrued on a daily basis. Settlement of aggregate accumulation occurs regularly on pre-determined settlement dates.

Decumulators allow an investor to sell a fixed quantity of an underlying share at a pre-determined strike price, on each trading day of the investment period. This forward price is set at a premium to the initial spot price of the underlying share. They are also structured with a knock-out feature and are terminated early, when the price of the underlying share closes at or below a pre-determined barrier. When the price of the underlying share closes at or below the pre-determined barrier price, a knock-out event occurs.

Product definition provides parameterization of the product and connections between units and events. It defines the SY.EVENT (s) that take place throughout a product’s life cycle and the related operations on SY.UNIT (s) that are performed when that event takes place, thus creating a full product life cycle.

The SY.PRODUCT.DEFINITION record ID is the same as the related SY.PRODUCT.DESCRIPTION record. SY.PRODUCT.DEFINITION acts as a template for the SY.PRODUCT record instances that are automatically created per transaction during processing.

The bank can extend the basic product definition and create their own variants. This is achieved by setting up records in SY.PRODUCT.VARIANT application. The ID of this table contains two parts separated by ‘_’. The prefix is the product definition that is being extended, while the suffix refers to the variants. All the parameters defined in the product definition are inherited by the product variant and can be amended at the variant level. Different P and L categories and flags can be set at the variant level. The configuration defined in the product variant takes precedence over the one defined in the product definition.

The product variant can have its own SUB.ASSET.TYPE and PRODUCT.CATEGORY , and these applications are key differentiators useful for reporting purposes.

| Field | Description |
|---|---|
| Product Type | This field indicates this is an accumulator or decumulator contract. |
| Contract Status | The status of the contract is updated in this field. When the contract is created, the status is ACTIVE, subsequently as the contract undergoes various life cycle events, the status is updated as below. |
| Option Type | This field holds the option type of the underlying option. This is auto populated based on the Product Type field. For accumulator contract, the underlying is a PUT option, for decumulator contract, the underlying is a CALL option. |
| Trade Date | This field holds the trade date of the contract. Trade date cannot be forward dated and should fall between the First Date and Last Date of the corresponding product definition record. |
| Maturity Date | Maturity date is the termination date of the contract. Maturity date is defaulted based on Term and Value Date . |
| Daily Units | This field holds the number of units (nominal) to be accrued per day. The value should be a multiple of contract size of the underlying DX.CONTRACT.MASTER . |
| Fixing Frequency | The Accumulator and Decumulator contracts accrue the underlying security on a daily basis. The accrued units are settled periodically (This periodic settlement is known as fixing). |

| Element | Description |
|---|---|
| Value Date | Contractual obligation commences from this date. |
| Underlying security | The underlying security which is accumulated or decumulated over the tenor of the contract. |
| Strike Price | The forward price at which the underlying security is purchased or sold. |
| Knock out price | This is the barrier price, when the spot price of the underlying security breaches this barrier, the contract gets knocked out (terminated). |
| Daily units | The number of shares that must be accrued on a daily basis. |
| Gearing factor | The gearing factor is applied on the days when the spot price of the underlying is unfavourable to the investor when compared to the strike price. |
| Fixing drequency | Settlement of accumulated or decumulated shares occur at this periodicity. |
| Maturity Date | The contractual obligation ends at this date. |

| Event | Description |
|---|---|
| Inception | Contractual obligation commences for the investor. The contract is recorded in the system and the underlying option trade is created. |
| Accrual | Units (of the underlying security) is accrued on a daily basis. For contracts with gearing factor, the gearing factors are applied on those days when the spot price of the underlying is unfavourable to the investor when compared against the strike price of the contract. |
| Fixing | Settlement of the accumulated or decumulated shares are effected through this event. The underlying option is exercised and this creates the SEC.TRADE transaction for the underlying security. This is a scheduled periodic event. |
| Knockout | This event can occur when the price barrier is breached, that is, when the spot price of the underlying touches the knock-out price. When this event occurs, the contract is terminated. |
| Unwinding | The contract can be unwound either fully or partially. In a full unwind, the contract is terminated early. In a partial unwind, the contract continues to be active, but the obligation (that is, daily accrual units) are reduced for the rest of the contract period. |
| Novation | The contract can also be novated, which is transferred from one customer account to another customer account (Internal novation) or transferred to a different bank (external novation). |
| Maturity | It is the end date of the contract. The contractual obligation ceases on this date. |

| Variant | Description |
|---|---|
| Non leveraged accumulator or decumulator | This is the plain vanilla accumulator without a gearing factor. |
| Leveraged Accumulator | This variant has an additional attribute, which is, gearing factor. Gearing factor is applied to the accrual on those days where the Spot Price is unfavorable to the customer, when compared to the strike price. The potential loss to the investor is higher in this variant as compared to the plain vanilla variant. |
| Guaranteed accumulator or decumulator | This variant assures the investor of guaranteed accumulation. That is, a certain number of underlying shares might be accumulated or decumulated and settled, even if the knock-out price barrier is breached early in the life of the accumulator contract. |


##### Illustrating Model Products

Model products are not applicable for this module.

---


---


## Chapter 3: Derivatives


Derivatives module of Temenos Transact


### Features in Derivatives


| # | Feature | Sections |
|---|---------|----------|
| 3.1 | Accounting | Intro, Confi, Worki |
| 3.2 | Aggregation SEC.TRADE SSI | Intro, Confi, Worki, Tasks, Outpu |
| 3.3 | Asian and Performance Options | Intro, Confi, Worki, Tasks, Outpu |
| 3.4 | BasketOptions | Intro, Confi, Worki, Tasks, Outpu |
| 3.5 | CDS | Intro, Confi, Worki, Tasks, Outpu |
| 3.6 | Close Out | Intro, Confi, Worki, Tasks, Outpu |
| 3.7 | Commissions | Intro, Confi, Worki, Tasks, Outpu |
| 3.8 | Constraints | Intro, Confi, Tasks, Outpu |
| 3.9 | Corporate Actions | Intro, Confi, Tasks, Outpu |
| 3.10 | Derivatives Contract Master | Intro, Confi, Tasks, Outpu |
| 3.11 | Derivatives Price Update | Intro, Confi, Worki, Tasks, Outpu |
| 3.12 | DX Package Option | Intro, Confi, Worki, Tasks, Outpu |
| 3.13 | Exotic Options | Intro, Confi, Worki, Tasks, Outpu |
| 3.14 | FX OTC Options | Intro, Confi, Tasks, Outpu |
| 3.15 | Limits | Intro, Confi, Worki, Tasks, Outpu |
| 3.16 | MarginCalculation | Intro, Confi, Worki, Tasks, Outpu |
| 3.17 | Market Ex Profit | Intro, Confi, Tasks, Outpu |
| 3.18 | MiFID Transaction Reporting | Intro, Confi, Worki, Tasks, Outpu |
| 3.19 | Misc | Intro |
| 3.20 | Non Stop Processing | Intro, Confi |
| 3.21 | Order Grouping | Intro, Confi, Worki, Tasks, Outpu |
| 3.22 | Order Processing | Intro, Confi, Worki, Tasks, Outpu |
| 3.23 | Reporting | Intro, Confi, Tasks, Outpu |
| 3.24 | Revaluation | Intro, Confi, Worki, Tasks, Outpu |
| 3.25 | Static setup | Intro, Confi, Worki, Tasks, Outpu |
| 3.26 | Swaptions | Intro, Confi, Worki, Tasks, Outpu |
| 3.27 | SWIFT MT306 for Exotic Options | Intro, Confi, Worki, Tasks, Outpu |
| 3.28 | Trade | Intro, Confi, Tasks, Outpu |
| 3.29 | Transaction Fees and Charges | Intro, Confi, Worki, Tasks, Outpu |
| 3.30 | Transfers | Intro, Confi, Tasks, Outpu |
| 3.31 | Misc | Intro |
| 3.32 | Misc | Intro |


### 3.1  Accounting


> **📇 Quick Reference Card**
> 
> **Purpose:** *Financial Accounting in Derivatives is flexible and allows user to define different Profit & Loss categories and internal account and suspense account categories, to post entries.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With


#### 📖 Introduction

Financial Accounting in Derivatives is flexible and allows user to define different Profit & Loss categories and internal account and suspense account categories, to post entries.

DX.TRADE is a double-sided application where both sides can be customers or one side can be a customer while the other is a broker or counterparty or dealer. In order to handle accounting flow in all of these cases, all trade related postings on either side of the contract are washed through the suspense accounts or P&L categories

This feature explains where the various categories need to be defined and how accounting works in DX module.


#### ⚙️ Configuration

This section details the configuration of accounting related DX applications.


##### ConfiguringACCOUNT.CLASS

The definition of the suspense accounts or P&L categories through which postings are washed are specified in the ACCOUNT.CLASS application. The below table describes the various types of record held in the ACCOUNT.CLASS hold application.

| ACCOUNT.CLASS ID | Type | Description |
|---|---|---|
| SUSPDXIMCR | Account | Suspense account for credit initial margin |
| SUSPDXIMDR | Account | Suspense account for debit initial margin |
| SUSPDXVMCR | Account | Suspense account for credit futures variation margin |
| SUSPDXVMDR | Account | Suspense account for debit futures variation margin |
| SUSPDXOMCR | Account | Suspense account for credit option variation margin |
| SUSPDXOMDR | Account | Suspense account for debit option variation margin |
| SUSPDXCGCR | Account | Suspense account for credit DX charges |
| SUSPDXCGDR | Account | Suspense account for debit DX charges |
| SUSPDXPRCR | Account | Suspense account for credit option premium payments |
| SUSPDXPRDR | Account | Suspense account for debit option premium payments |
| SUSPDXRPCR | Account | Suspense account for credit realised P&L |
| SUSPDXRPDR | Account | Suspense account for debit realised P&L |
| DXCSNDUE | P&L | Suspense P&L category for DX commission due not paid (not utilised until phase 2) |
| DXCSNEARN | P&L | Suspense P&L category for DX commission earned, but not received (not utilised until phase 2) |
| DXCSNPAID | P&L | Suspense P&L category for DX commission paid |
| DXCSNRCVD | P&L | Suspense P&L category for DX commission received |

The category consideration is important while setting up the ACCOUNT.CLASS records. If different categories are used for the debit and credit ACCOUNT.CLASS , the two internal suspense accounts (one for debit and one for credit) net to zero. However, the individual account balance increases or decreases. It is preferred to use the same CATEGORY for the debit and the credit ACCOUNT.CLASS , so that the funds wash in and out of the same suspense account.


##### ConfiguringDX.EVENT.TYPE

Category codes for various fees, charges etc., are defined in DX.EVENT.TYPE application.

The CATEGORY codes to be set up are of three types as explained below.

This category should be set up for all non-P&L ACCOUNT.CLASS records (Read the Configuring ACCOUNT.CLASS section for more information). This is required for tax posting (TT), option premium posting (PP) and initial margin posting (IM) DX.EVENT.TYPE records.

A dummy internal account CATEGORY code should be set up for entry into DX.EVENT.TYPE records where the category code is not used (CA, CC, CI, CR, UO) and also for commission or fee postings if the Use Ft TX Code field is set in DX.EVENT.TYPE .

The system opens internal accounts in all other currencies automatically if at least one internal account is set up manually for each internal account category code entered.

The wash account currency to be used for posting the option premiums to an internal account is set in the Wash Acc T ype field in DX.EVENT.TYPE . The following are the valid values in this field:

- Blank (postings occur in the reference currency)
- Local (postings occur in the system local currency)
- Trade (postings occur in the currency of the contract)

This field can be used only for a premium posting event (PP).

A product category in the appropriate range should be set up for each DX.CONTRACT.CLASS defined by the bank.

| Transaction types in RE.TXN.CODE | Description |
|---|---|
| CLO | Derivatives contract closeout |
| UOV | Derivatives unrealised option value |


#### 🔧 Working With

This section deals with the working mechanism of accounting in Temenos Transact .


##### Illustrating Contingent Asset or Liability

On contract initiation ( DX.EVENT.TYPE CI), a CRF posting (as shown in the below table) is created to show an off-balance sheet asset or liability active during the contract’s life.

| Type of Contract | CRF Type |
|---|---|
| Own book portfolio buys contract | Debit CRF type DXFUTBUY |
| Own book portfolio sells contract | Credit CRF type DXFUTSELL |

On reversal, complete closeout or maturity of the trade, the postings are backed out. For partial closeouts, a pro rata amount based on the ratio of lots closed to total lots on the trade is backed out.

Contingent asset or liability is applicable only for own book portfolios.


##### Illustrating Trade and Value Dated Accounting

If the posting offsets are set in DX.CONTRACT.MASTER , the trade or value date accounting setup only affects the posting of option premiums, commissions or fees, or settlement P&L. . The forward-dated real accounting entries are made to customer or internal accounts only in such instances.

The Value Dated Acctng field in ACCOUNT.PARAMETER controls the handling of the forward-dated account entries as the DX module utilises Temenos Transact standard core accounting.

A bank customer buys an option versus a broker; the option in question has premium and fees posted at the trade time. If the Prem Post Offset field in DX.CONTRACT.MASTER for the instrument is set to two (that is a two-day offset between premium date and posting), Temenos Transact responds as follows:

DR the Customer account option premium with Value date as ‘today’

That is the premium hits the customer’s account immediately and is shown on the customer’s statement

DR the Customer account option premium with Value date as ‘today’ + two working days

That is, the premium is booked as a forward dated entry and does not appear on the customer’s statement until ‘today + two working days’.

> **⚠️ Note:** The Trade Date or Value Date field in DX.TRADE does not affect whether the premiums or commissions are posted at trade or closeout time for a contract.

If a DX instrument is set to have premiums and commissions charged on settlement (or close-out), the sum is not posted until a trade on that instrument is closed out even in a trade-dated accounting environment.


##### Illustrating Trade Dated GL Accounting

Trade dated GL (TDGL) is an accounting treatment in which the customer's balance is updated on the value date. However, the balance sheet general ledger is updated on the trade date but it is updated under the payable or receivable heads. In TDGL accounting, future value dated entries are treated as follows:

- Account actual balances are not updated until the value date.
- Movements do not appear on account statements until the value date.
- Movements reflect in the balance sheet under payable and receivable.

TDGL for DX is set in ACCOUNT.PARAMETER application with the relevant categories. DX posts the premium or commission entries to the payable or receivable accounts (respectively) on trade date and on value date and the customer account is debited and settled against the payable or receivable accounts.

Sell option (to customer)

- Premium booking on trade date: Dr premium receivable (in native currency) Cr unrealised profit
- Premium settlement on value date: Dr customer account Cr premium receivable (in native currency)


##### Understanding Taxes in Derivatives

There are tax related fields in DX.ORDER , DX.TRADE and DX . CLOSEOUT applications for the tax requirements. The tax fields accept manual input or usage of API (in case of DX . CLOSEOUT ) and the core raises appropriate accounting entries for the tax amount depending on the nature of the trade.

The multi-valued tax related fields in the applications mentioned above are:

| Application | Fields |
|---|---|
| DX.ORDER | Pri Tax Code , Pri Tax Type , Tax Amt Acy , Tax Amt Tcy , Sec Tax Code , Sec Tax Type , Sec Tax Amt Acy , and Sec Tax Amt Tcy |
| DX.TRADE | Pri Tax Code , Pri Tax Type , Tax Amt Acy , Tax Amt Tcy , Sec Tax Code , Sec Tax Type , Sec Tax Amt Acy , and Sec Tax Amt Tcy |
| DX. CLOSEOUT | Tax Code , Tax Type , Tax Amt Acy , and Tax Amt Tcy |

Also, the tax details are recorded in the DX.TRANSACTION application for reporting purposes.

The Tax Amt Tcy and Sec Tax Amt Tcy are display-only fields, which display the equivalent amount in trade currency.

When the record relates to customer deals, four entries are generated.

The customer account is debited and credited to a wash through suspense account. Then the wash through suspense account is debited and credit is posted to the Tax internal account.

The tax collected in the tax internal account will have to be manually credited to the Tax authorities on due dates. This will be a manual process and not done automatically.

As part of the setup, a TT type DX.EVENT.TYPE record is required with a PL category code linked to it. A CATEG.ENTRY is raised to debit the PL category defined in DX.EVENT.TYPE (TT) for the tax payable and a corresponding entry is raised to credit the internal account.

This process also raises two wash through entries. The following screenshots display the corresponding STMT.ENTRY and CATEG.ENTRY , respectively.

The same set of fields are available in the DX.ORDER application, to capture the tax at the time of order execution. It is also possible to compute taxes at the time of closeout in the DX.CLOSEOUT application with an API is specified in the Closeout Api field of DX.PARAMETER .

In this case, the tax accounting entry or entries are raised from the DX.CLOSEOUT record once it is authorised.

---


### 3.2  Aggregation SEC.TRADE SSI


> **📇 Quick Reference Card**
> 
> **Purpose:** *Trade Aggregation is a process of aggregating the trades and generating a bulk settlement instruction instead of sending a settlement instruction per trade. This reduces the number of SWIFT settlement instructions and facilitates a smoother settlement process.*
> 
> **Applications:** `DX.CLOSEOUT`, `DX.CO.ASSIGN.AUTO`, `DX.CO.ASSIGN.MANUAL`, `DX.CO.EXERCISE.AUTO`, `DX.CO.EXERCISE.MANUAL`, `DX.CONTRACT.MASTER`, `DX.CUSTOMER`, `DX.EXCHANGE.MASTER` ... +8 more
> 
> **Key Fields:** *Aggr Cut Off Time*, *Aggr Id*, *Aggr Req*, *Aggr Utc Time*, *Aggregation Ref*, *Broker*, *Call Put*, *Close Out Id* ... +23 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Trade Aggregation is a process of aggregating the trades and generating a bulk settlement instruction instead of sending a settlement instruction per trade. This reduces the number of SWIFT settlement instructions and facilitates a smoother settlement process.

In a Derivatives option contract,

- The option holder exercises the contract and buys/sells the underlying shares at the specified strike price.
- The option seller is assigned and buys/sells the underlying share when the buyer exercises the contract.

In both scenarios, the system creates underlying security transactions during the closeout of the contract. The system sends a Standard Settlement Instruction (SSI) to the depository from these security trades whenever the trades are authorised. Further, the depository sends the settlement instruction status and updates in the transaction accordingly.


#### ⚙️ Configuration

This topic explains the basic configuration to be set to aggregate the trades and generate a bulk settlement instruction.


##### Trade Aggregation

To enable the aggregation of settlement instruction at the system level for the underlying security trades generated from the derivative option contracts, the user must set Trd Aggr to Yes in DX.PARAMETER .


##### Broker Aggregation

To enable the aggregation of Settlement Instruction for the underlying security trades generated from the derivative option contract, for a particular broker or counterparty, the user must set Sec Trd Aggr to Yes in DX.CUSTOMER . This field can be set only when Trd Aggr is set to Yes in DX.PARAMETER . Also, this field is enabled only when Customer Type is Broker or Counterparty.


##### Automatic Generation of SSI for Aggregated Securities

To enable the automatic generation of Settlement Instruction for the aggregated security trades, the user must define UTC time or local server time in DX.EXCHANGE.MASTER .

If the user defines UTC time in Aggr Utc Time , on validating the record the system automatically calculates the local server time and the updates the time in Aggr Cut Off Time .

Consider a Security where the exchange is located in Singapore and local server and transactions are executed in New York (US). In this scenario, the system performs the auto aggregation of the underlying security in Singapore time at 14:30 hrs. The UTC of Singapore is UTC+08:00 and the UTC of New York is UTC-04:00. In this scenario, the user must update Aggr Utc Time as 06:30am (this corresponds to Singapore time of 14:30 hrs). The system automatically converts the UTC to the local server time of New York as 02:30am.

Also, the local server time can be defined directly in Aggr Cut Off Time , in this case Aggr Utc Time is left blank.

The auto generation of settlement instruction is performed based on the time set in Aggr Cut Off Time .


##### SP.STP.PARAM

The user must set Sp Aggr Launch Version to a valid version of SP.AGGR.LAUNCH to generate aggregated trade record in SP.RECONCILIATION. The SP AGGREGATION.SERVICE service performs the auto-process during the time defined in Aggr Cut Off Time .


#### 🔧 Working With

When the derivative options are exercised or assigned in DX.CLOSEOUT , the system creates appropriate corresponding security transactions. When the transactions are performed, the system identifies the aggregation for the broker, based on the setup in DX.CUSTOMER by assigning a unique ID based on certain combination. This topic explains about the generation of unique IDs.


##### Aggregating SSI

The workflow for this functionality is depicted below.

- Configuration setup must be done as a prerequisite as discussed in the Configuration section.
- The closeout suite of applications include DX.CO.EXERCISE.MANUAL, DX.CO.ASSIGN.MANUAL, DX.CO.EXERCISE.AUTO, and DX.CO.ASSIGN.AUTO.


##### Creating Aggregation ID

To aggregate the security trades created from the closeout, the system creates a unique ID in the closeout applications for each unique combination of the fields ( Contract Code , Maturity , Strike , Call Put , and System Date ). The system updates the ID automatically in Aggr Id of the respective closeout suite of applications. For system exercised closeouts performed during COB process, it creates ID and updates in Aggregation Ref of security trades directly.

| S No. | Contract Code | Maturity | Strike | Option Date | Transaction ID | DX.CO.EXERCISE.MANUAL | Aggr Id |
|---|---|---|---|---|---|---|---|
| 1 | 240000 | 20230418 | 50 | Call | DXTRA2310912345 | DXCOEXR2310912345 | AGGR2310982789 |
| 2 | 240000 | 20230418 | 50 | Call | DXTRA2310998989 | DXCOEXR2310954321 | AGGR2310982789 |

| Customer | Portfolio | Contract | Maturity Date | Strike | Transaction ID | Option Style |
|---|---|---|---|---|---|---|
| 100285 | 100285-1 | 210050 | 202304 | 40 | DXTRA2310912345 | Call |
| 100273 | 100273-1 | 210050 | 202304 | 40 | DXTRA2310954321 | Call |
| 100286 | 100286-1 | 210050 | 202304 | 40 | DXTRA2310998989 | Call |
| 100400 | 100400-1 | 210050 | 202304 | 40 | DXTRA2310545454 | Call |

| Operand | Description |
|---|---|
| EQ | Selects all the contracts where the strike price is equal to the value provided in Strike. |
| GE | Select all the contracts where the strike price is greater than or equal to the value provided in Strike. |
| LE | Select all the contracts where the strike price is less than or equal to the value provided in Strike. |

| Customer | Portfolio | Contract | Maturity Date | Strike | Transaction ID | Option Style |
|---|---|---|---|---|---|---|
| 100285 | 100285-1 | 240000 | 20230418 | 50 | DXTRA2310912345 | Call |
| 100286 | 100286-1 | 240000 | 20230418 | 50 | DXTRA2310998989 | Call |
| 100291 | 100291-1 | 240000 | 20230418 | 50 | DXTRA2310545454 | Call |

In DX.CONTRACT.MASTER , if the user sets System Exercise to Yes, the system performs automatic exercise of contract during end of day process with the certain condition, that is, the contract should be in the money. During closeout, the system creates a record in SEC.TRADE in IHLD status. If the user defines Sec Trd Aggr as Yes of DX.CUSTOMER application, the system generates Aggr Id and updates the ID in Aggregation Ref of respective SEC.TRADE .


##### CreatingSP.AGGREGATION

The system creates all the underlying records in SEC.TRADE with IHLD status. Once the SEC.TRADE records are authorised, the records are created in SP.AGGREGATION against each SEC.TRADE (the ID of the Sp Aggregation is the same as that of the SEC.TRADE ). On running the OFS.MESSAGE.SERVICE service, the system extracts below list of field values from SEC.TRADE and updates in Sp Aggregation . If the records in SEC.TRADE are not authorised, the trades are not considered for aggregation.

> **⚠️ Note:** If user manually removes the ID from Aggregation Ref and commits the record, then the removed record is not considered for the aggregation.


##### Aggregation of Security Trades

| Customer | Portfolio | Contract | Broker | Strike | Aggr Id | SEC.TRADE |
|---|---|---|---|---|---|---|
| 100285 | 100285-1 | 240000 | 100112 | 50 | AGGR2310871484 | SCTRSC2310912345 |
| 100286 | 100286-1 | 240000 | 100112 | 50 | AGGR2310871484 | SCTRSC2310954321 |
| 100291 | 100291-1 | 240000 | 100112 | 50 | AGGR2310871484 | SCTRSC2310945454 |

| Customer | Portfolio | Contract | Broker | Strike | Aggr Id | SEC.TRADE | Record Status |
|---|---|---|---|---|---|---|---|
| 100285 | 100285-1 | 240000 | 100112 | 50 | AGGR2310871484 | SCTRSC2310912345 | LIV |
| 100286 | 100286-1 | 240000 | 100472 | 50 | AGGR2310871484 | SCTRSC2310954321 | LIV |
| 100291 | 100291-1 | 240000 | 100492 | 50 | AGGR2310871484 | SCTRSC2310945454 | IHLD |

| Customer | Contract | Broker | Strike | Aggr Id | SEC.TRADE | Aggregation Ref |
|---|---|---|---|---|---|---|
| 100285 | 240000 | 100112 | 50 | AGGR2310871484 | SCTRSC2310912345 | AGGR2310871484*50 |
| 100286 | 240000 | 100472 | 50 | AGGR2310871484 | SCTRSC2310954321 | AGGR2310871484*49 |
| 100291 | 240000 | 100492 | 50 | AGGR2310871484 | SCTRSC2310945454 | AGGR2310871484*48 |

The system performs an auto process by creating a record with Aggr Id in SP.AGGR.LAUNCH based on the time defined in Aggr Cut Off Time of DX.EXCHANGE.MASTER . The system performs this process only once a day as per the time defined. The system considers all the Aggr Id s that are yet to be processed and aggregates the security trades for all authorized security trades. Once the record is committed successfully, the system creates and triggers the record SP.RECONCILATION . Multiple records are created in SP.RECONCILIATION when any of the combinations of field values differ in the SP.AGGREGATION records. Once the system creates records of SP.RECONCILIATION , the system updates the record ID in Recon Id of SP.AGGR.LAUNCH . This process is performed by running the SP AGGREGATION.SERVICE service.

The system-created records are updated with Generated By set as System in SP.AGGR.LAUNCH .

During the creation of SP.RECONCILIATION record, the system also creates a record in SC.MT548.MATCH.QUEUE in IHLD status.


##### Generation of Aggregated Standard Settlement Instruction Message

SP.RECONCILIATION holds the aggregated details of the security trades that are created from the derivative closeout applications with reference to Aggr Id . When the system creates the record, a standard settlement instruction message (540-543) is generated for the aggregated trades.


#### 📋 Tasks

There are no Tasks available for Aggregation of Security Trade SSI feature.


#### 📊 Outputs

There are no Outputs available for Aggregation of Security Trade SSI feature.


> **Related Applications:** `DX.CLOSEOUT`, `DX.CO.ASSIGN.AUTO`, `DX.CO.ASSIGN.MANUAL`, `DX.CO.EXERCISE.AUTO`, `DX.CO.EXERCISE.MANUAL`, `DX.CONTRACT.MASTER`, `DX.CUSTOMER`, `DX.EXCHANGE.MASTER`, `DX.PARAMETER`, `SC.MT548.MATCH.QUEUE`, `SEC.TRADE`, `SP.AGGR.LAUNCH`, `SP.AGGREGATION`, `SP.RECONCILATION`, `SP.RECONCILIATION`, `SP.STP.PARAM`

---


### 3.3  Asian and Performance Options


> **📇 Quick Reference Card**
> 
> **Purpose:** *An Asian option is an option type where the payout depends on the average price of the underlying asset over a certain period of time as opposed to standard options (American and European) where the payout depends on the price of the underlying asset at a specific point in time (maturity). Asian opt...*
> 
> **Key Fields:** *Asian Type*, *Average Spot*, *Average Strike*, *Call/ Put*, *Fixed Strike*, *Market Price*, *Observation Date*, *Observation Dates* ... +10 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

An Asian option is an option type where the payout depends on the average price of the underlying asset over a certain period of time as opposed to standard options (American and European) where the payout depends on the price of the underlying asset at a specific point in time (maturity). Asian options are classified as:

- Fixed Strike – The strike is fixed, while average of spot price is used to determine the pay off.
- Fixed Spot –the spot price is fixed and the strike price is the average of spot prices on the observation dates.

Performance options track the performance of the underlying asset from the date of commencement of the option upto maturity. The appreciation (or depreciation) of the underlying is used to determine the payout.


#### ⚙️ Configuration

Configure the DX.CONTRACT.MASTER application as shown below to enable the Asian and Performance options in DX module.

| Field | Description |
|---|---|
| Option Value Type | Contains a drop-down value called Asian. If this field is populated, either Asian Type or Performance field is populated. |
| Asian Type | The allowed values are Fixed Strike Floating Strike This field is mandatory if Option Value Type is Asian and Performance field is not set to Yes. A validation ensures if Fixed Strike is selected, and Settlement Method is set to CASH. This is a no input field, if Option Value Type is not set to Asian. |
| Performance | This is a Yes or No field. If it is set to Yes, the performance of the underlying asset is used to determine the payout Where, Where, Underlying final - Spot price on fixing date Underling initial - Spot price on start date of the contract When this field is set to Yes, the strike price and the call or put indicator in the trade is irrelevant. The default values to be used are: Strike set to 1 Call/ Put set to Call When this field is set, the Settlement Method is in cash always. |

The following contract shows an Asian option with floating strike option.

This following contract shows an Asian option with performance option.


#### 🔧 Working With

The following section explains about the Asian and Performance option transaction processing. The following fields in DX.TRADE can be used for Asian and Performance option transactions.

| Field | Description |
|---|---|
| Participation Rate | A percentage field that is used to calculate the final payout of the option. This is a mandatory field, if Performance field is set to Yes in DX.CONTRACT.MASTER |
| Observation Date -XX | A multi value field where the observation schedule can be defined. This is a mandatory field when Option Value Type is set to Asian. The number of multi values is equal to the number of dates in the fixing schedule |
| Observed Spot Rate -XX | An associated multi value field that indicates the spot price of the underlying asset on the Observation Date |
| Spot Price Initial | Indicates the spot price of the underlying asset on commencement of the contract. This price is used to calculate the performance of contracts with Performance field set to Yes |

> **⚠️ Note:** When Performance field is set to Yes in DX.CONTRACT.MASTER , the Strike Price defaults to 1 and Option Type to CALL.

The trade displays the Observation Date multi value set as shown in the below screenshot.

This trade is for Performance option and the Participation Rate and Spot Price Initial fields are updated as shown in the below screenshot.


##### Closeout Applications

The closeout applications are listed below.

- DX.CO.EXERCISE.MANUAL
- DX.CO.ASSIGN.MANUAL
- DX.CO.EXERCISE.AUTO
- DX.CO.ASSIGN.AUTO

Read the Closeout feature for more information. The fields listed below are available in the closeout applications:

| Field | Description |
|---|---|
| Observation Date -XX | Defaults the values from DX.TRADE and it is a no input field |
| Observed Spot Rate -XX | Defaults the values from DX.TRADE . The values are amendable (that is, if values are available in DX.TRADE , then rate is populated by default in this field. The user can also input and override the default value.) |
| Participation Rate | Defaults the values from trade and it is a no input field |
| Performance | Indicates the calculated value, If the Performance field is set to Yes and the Option Value Type is set to Asian, Where, n = number of observation dates, Underlying final (i) = Underlying spot price on corresponding observation date (that is, Observed Spot Rate ), Underlying initial = Spot Price Initial If the Performance field is set and the Option Value Type is not set to Asian, then Where, Underlying final = Market Price , Underlying initial = Spot Price Initial |
| Average Spot | This is a calculated value. Updated only when Asian Type field is set to Fixed Strike in DX.CONTRACT.MASTER . where, n = number of multi values (that is, the value in the Observation Date field) This field can be modified by the user. |
| Average Strike | Indicates the calculated value which is updated only when Asian Type field is set to Floating Strike in DX.CONTRACT.MASTER . where n = number of multi values (that is, the value in the Observation Dates field) This field can be modified by the user. |

The calculation of settlement amount is calculated as per the table below.

| Performance | Asian Type | Call/ Put | Settlement Amount |
|---|---|---|---|
| Yes | - | - | Notional * Participation Rate * Performance |
| No | Fixed Strike | Call | Average Spot - Strike |
| No | Fixed Strike | Put | Strike - Average Spot |
| No | Floating Strike | Call | Market Price - Average Strike |
| No | Floating Strike | Put | Average Strike - Market Price |

> **⚠️ Note:** In case of Floating Strike Contracts with Physical Settlements, the underlying transactions are generated with Average Strike. The Participation Rate and Observation Date fields are part of the selection criteria in DX.CO.ASSIGN.AUTO and DX.CO.EXERCISE.AUTO applications. The settlement amount calculated as per the above calculation can be amended by the user.

The calculation of an average strike for a floating strike contract is shown in the below screenshot.


#### 📋 Tasks

Related topics:

- Create Derivatives Master

This application holds the contract definitions of all of the contract types which are tradable in the Derivatives module. It defines the characteristics of future, stock or option contracts. Basic contract details, pricing data, trading size, maturity date validation and so on are all captured here.


##### Workflow

This feature allows the user to perform the following tasks:

This screen enables the user to create a derivatives contract master for Asian option style.

1. DX Contract Master Asian Options .
2. In DX Instrument – Asian Option tab, enter values in the following fields: Mnemonic GB Descript.1 GB Short Name Exchange Contract Class Contract Type Sub Asset Type Asian Type Performance Delivery Method (Should be set as “CASH”) Units of Measure Contract Size In Price Details tab, enter values in the following fields: Tick Size.1 Tick Value.1 Min Price Mvmt.1 In Contract Dates tab, enter values in the following fields: Maturity Type
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon.


#### 📊 Outputs

There are no Outputs available for Asian and Performance Options feature.

---


### 3.4  BasketOptions


> **📇 Quick Reference Card**
> 
> **Purpose:** *Basket option is a type of financial derivative in which the underlying asset is a group, or a basket of commodities, securities or currencies. This feature has all the characteristics of a standard option, difference being the strike price which is based on the weighted value of its component.*
> 
> **Key Fields:** *Basket Type*, *Call Amount*, *Call Ccy*, *Call Ccy/Put Ccy*, *Cash Amount*, *Cash Ccy*, *Cash Exercise*, *Contract Code* ... +28 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Basket option is a type of financial derivative in which the underlying asset is a group, or a basket of commodities, securities or currencies. This feature has all the characteristics of a standard option, difference being the strike price which is based on the weighted value of its component.

The basket option as similar to the other options, gives the holder the right (but not the obligation) to buy or sell an underlying asset at a specific price, on or before a certain date. The basket options are traded through the Derivatives (DX) module where equity and currency baskets are supported.

A trade can be booked with:

- Single notional in reference or base currency
- Multiple currency pairs or securities
- Multiple strike prices

Temenos Transact also supports the processing of life cycle events such as:

- Exercise
- Expiry


#### ⚙️ Configuration

The basket option can be configuration in Temenos Transact by setting the following applications.


##### DX.CONTRACT.CLASS

The Contract Type field in DX.CONTRACT.CLASS application must be set to Basket which indicates that the record is a basket option class.


##### DX.CONTRACT.MASTER

A new record is created in the DX.CONTRACT.MASTER application with the specific to the DX.CONTRACT.CLASS record created for basket option.

Once the basket contract class is selected, the below fields in DX.TRADE are updated automatically.

| Field | Default Value |
|---|---|
| Underlying | Basket |
| Price Source | Interface |
| Tick Value | 1 |
| Tick Size | 1 |
| Contract Size | 1 |
| Currency | No input |
| Delivery Currency | No input |
| Settlement Method | No input |
| Contract Size | No input |
| Exchange | Non-mandatory |
| Option Style | Non-mandatory |


##### DX.CONTRACT.TERMS

The DX.CONTRACT.TERMS application allow creation of frequently traded baskets. The basket is linked to the trade and the values from the basket defaults to the trade. If a record is not created in this application, then the user can enter the relevant values in the trade directly.

| Field | Description |
|---|---|
| Mnemonic | Indicates the alternate identifier for the basket |
| Unique Identifier | Indicates the unique identifier such as ad valorem number |
| Ulying Asset Class | Indicates whether the underlying is an equity or currency basket. This is a mandatory field. The values are : Equity Currency |
| Basket Type | Indicates the type of basket. The values are: Null (default value) Best of the Market Custom Weighted Equal Weighted Worst of the Market The value Null indicates that it is not a basket option. Though there are four types of baskets available at present, this list is scalable. This list can be configured based on the BASKET.TYPE user defined value in the EB.LOOKUP table. |
| Price Source | Indicates the identifier of a price interface. This value overrides the value in the Price Source field in DX.CONTRACT.MASTER . |
| Call Put | Indicates if the holder has the right, but not obligation, to buy or sell stock at a fixed price at a future date. The values are: None Call Put |
| Trade Ccy | Indicates the trade currency |
| Maturity Date | Indicates the delivery period or prompt date of the contract transacted |
| Settlement Method | Indicates the settlement mode of the option contract. The values are: Cash Physical |
| Static Leg | Indicates if the buy or sell currency should be same in all multi-value pairs. This field is mandatory for currency basket. The values are: None Call Put |
| Ulying Security | Indicates if the underlying is a security or currency basket. This field is mandatory if Ulying Asset Class field is set to Equity. Either underlying (equity basket) or Call Ccy/Put Ccy (currency basket) is mandatory. The fields from Ulying Security to Ulying Strike Price is part of an associate multi-value set. |
| Call Ccy | Indicates the currency in which the customer buys the FX spot deal. This field is mandatory if Ulying Asset Class field is set to Currency. |
| Put Ccy | Indicates the currency in which the customer sells the FX spot deal. This field is mandatory if Ulying Asset Class field is set to Currency. |
| Weight | Indicates the weight of the currency pair or the underlying in this basket |
| Strike Percentage | Indicates the strike expressed as a percentage of spot rate. Either strike percentage or strike is mandatory for this field. |
| Ulying Strike Ccy | Indicates the currency in which the exchange rate is quoted. This field is applicable for currency basket. |
| Ulying Strike Price | Indicates the strike price of the currency pair or underlying |


#### 🔧 Working With

When the contract being traded is a Basket, the DX.TRADE allows the definition of multiple underlying events.

| Field | Description |
|---|---|
| Contract Terms | Indicates the value defaulted from DX.CONTRACT.TERMS if the contract terms are defined. The details defaulted from DX.CONTRACT.TERMS cannot be modified. If the value is not defined in DX.CONTRACT.TERMS , the basket details can be input directly in the trade. |
| Settlement Method | Indicates the value defaulted from DX.CONTRACT.TERMS |
| Basket Type | Indicates the value defaulted from DX.CONTRACT.TERMS |
| Ulying Asset Class | Indicates whether the underlying is an equity or currency basket. The values are: Equity Currency |
| Static Leg | Indicates if the buy or sell currency should be same in all multi-value pairs. This field is mandatory for currency basket. The values are: None Call Put |
| Ulying Security | Indicates the value defaulted from DX.CONTRACT.TERMS . This is a display-only field. |
| Call Ccy | Indicates the currency in which the customer buys the FX spot deal defaulted from DX.CONTRACT.TERMS |
| Put Ccy | Indicates the currency in which the customer sells the FX spot deal defaulted from DX.CONTRACT.TERMS |
| Weight | Indicates the weight of the currency pair or equity in the basket defaulted from DX.CONTRACT.TERMS |
| Spot Price | Indicates the spot price of the underlying equity or exchange rate of the associated currency pair |
| Strike Percentage | Indicates the strike expressed as a percentage of spot rate |
| Ulying Strike Ccy | Indicates the currency in which the exchange rate is quoted. This field is applicable for currency basket. |
| Ulying Strike Price | Indicates the strike price of the currency pair or underlying |
| Exercise | Indicates the settlement of a physically settled basket. If this field is set to Yes: A SEC.TRADE record is created for the associated underlying of the basket for an equity basket . The price and nominal in SEC.TRADE is the associated strike price and quantity, respectively. A FX deal is created for the associated currency pair for a currency basket. |
| Quantity | Indicates the number of shares to be delivered of this underlying. This multi-value field is applicable only for physical delivery method and mandatory for equity basket when the Exercise field is set to Yes. |
| Call Amount | Indicates the amount received by the customer in the Call Ccy . This multi-value field is applicable only for physical delivery method and mandatory for currency basket when the Exercise field is set to Yes. |
| Put Amount | Indicates the amount received by the customer in the Put Ccy . This multi-value field is applicable only for physical delivery method and mandatory for currency basket when the Exercise field is set to Yes. |
| Cash Exercise | Indicates if a cash pay-out is triggered for the amount and currency specified in the Cash Amount and Cash Ccy fields, respectively. This field is applicable only for cash settled baskets. |
| Cash Amount | Indicates the cash amount to be paid out for a cash settled option. |
| Cash Ccy | Indicates the currency corresponding to the Cash Amount field. |

> **⚠️ Note:** If the Contract Terms field is updated, the values from the corresponding DX.CONTRACT.TERMS record are populated and cannot be amended. Alternatively, the terms can be directly input in the DX.TRADE application. The exotic fields are disabled for basket options.


##### Price and Valuation

The system does not calculate the price of basket options. The valuation or market price is calculated per contract and entered in the SYDX.MARKET.VAL application.


##### Maturity

At the time of maturity, the Exercise field must be set for each underlying for physical delivery and the Cash Exercise field must be set for cash pay-out. If the Exercise field is set, the SEC.TRADE record is created for the associated underlying. For example, if a basket has five underlying securities and the Exercise field is set for three underlying securities, three SEC.TRADE records are created. If the Cash Exercise field is set, a cash pay-out is generated.

A combination of cash pay-out and physical settlement is also possible For example, for a physically settled basket, cash pay-out can be used for fractional shares. It is equivalent to an option expiry if neither the Exercise nor Cash Exercise fields are set at the time of maturity processing.


##### Position Updates

The DX.REP.POSITION record is updated for basket options. The ID contains the Trade ID as all baskets use the same generic contract master. Additionally, the field in DX.REP.POSITION holds the DX.CONTRACT.TERMS relevant to this position (if available). Each position is unique and represents one basket.


##### Corporate Actions

The DX.DIARY application handles the Corporate Action (CA) on any of the underlying securities in an equity basket, which requires change in the strike price of that underlying.

The existing Contract Code field also accepts DX.CONTRACT.TERMS record. If this field is set, the system identifies all DX.TRADES based on these contract terms and corrects the strike price and/or lots of the equity undergoing the CA.

If the underlying security changes due to a conversion event, this can be updated in the DX.DIARY record and the system identifies the relevant trades and corrects the Ulying Security field in the DX.TRADE application.


##### Accounting

The contingent entries for notional amount are raised for own book trades. The entries for premium and charges are raised as in the DX.TRADE application.


##### Limit Updates

The limit can be updated for basket options. For an option buyer, the outstanding limit is adjusted to the extent of the premium amount. For an option seller, the outstanding limit is adjusted to the extent of the notional amount.


#### 📋 Tasks

Related topics:

- Initiate Basket Option
- Trading Processes

A basket option is a type of financial derivative, where the underlying asset is a group or basket of commodities, securities or currencies. Similar to other options, a basket option also gives the holder the right, but not the obligation, to buy or sell the basket at a specific price, on or before a certain date.


##### Workflow

This section allows the user to perform the below tasks:

This screen enables the user to enter a derivatives trade directly for basket option contracts.

1. Basket Options Input .
2. Enter values in the following fields: Contract Trade Date Maturity Date Call or Put Strike Price Buy or Sell Price/Premium Sec Cust(Broker) Sec Account Sec Price Customer No.1 Pri Lots.1 Sec Cpty No
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon.


#### 📊 Outputs

There are no Outputs available for Basket Options feature.

---


### 3.5  CDS


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Credit Default Swap (CDS) is a financial swap agreement, where the seller of the CDS compensates the buyer, in the event of a loan default or other credit event. The buyer of the CDS makes a series of payments (CDS fee, spread or premium) to the seller and in exchange receives a payoff, if the l...*
> 
> **Key Fields:** *As*, *As Currency*, *Bond Ccy*, *Bond Value*, *Buy or Sell*, *Contract Class*, *Contract Code*, *Contract Type* ... +23 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The Credit Default Swap (CDS) is a financial swap agreement, where the seller of the CDS compensates the buyer, in the event of a loan default or other credit event. The buyer of the CDS makes a series of payments (CDS fee, spread or premium) to the seller and in exchange receives a payoff, if the loan defaults.

In the event of a default:

- The buyer of the CDS receives compensation (usually the face value of the loan).
- The seller of the CDS takes possession of the defaulted loan.

In Temenos Transact , a CDS is captured using the Derivatives (DX) module.


#### ⚙️ Configuration

The section details the configuration required for Credit Default Swap (CDS).


##### Contract Class Definition -DX.CONTRACT.CLASS

The DX.CONTRACT.CLASS application defines a contract class for CDS by setting the Contract Type field to CDS.


##### Contract Definition -DX.CONTRACT.MASTER

The DX.CONTRACT.MASTER application holds the contract definitions of various contract types that are tradable in the DX module.

The specific configurations done for each field is explained below.

| Field | Description |
|---|---|
| Contract Class | Indicates the type of instruments traded on the relative exchange. This is a mandatory field and must be set to CDS. |
| Delivery Method | Defines the delivery method for specified contract at maturity. This is a mandatory field and must be set as Physical for CDS. The physical delivery of the underlying bond or instrument is done manually, if required. |

> **⚠️ Note:** The system automatically raises entries to debit or credit the bank’s P&L and pay or receive the amount of the contract on exercise of a CDS contract.

| Column 1 | Column 2 |
|---|---|
| Tick Size | Indicates the unit of quotation allowed. To avoid potentially infinitely small price fluctuations, the relative exchange, limits the minimum amount by which prices may change. This is a mandatory field and the value must be set to 1.0000. |
| Tick Value | Indicates the value derived from the Tick Size . This is a mandatory field and the value must be set to 1.0000. |
| Min Price Mvmt | Indicates the minimum price movement. This does not necessarily move by the tick size. This is a mandatory field and the value must be set to 0.0001. |

| Column 1 | Column 2 |
|---|---|
| Maturity Type | Defines the type of maturity. This is a mandatory field and is set as Daily or Monthly. |

| Column 1 | Column 2 |
|---|---|
| Prem Post Time | Indicates when the premium is posted to an account. This field must be set to TRADE for the premium to be paid or received in full on the trade date. |

| Column 1 | Column 2 |
|---|---|
| Underlying | Indicates the financial instrument, equity or commodity upon which a futures or options contract is based. This field must be set to Other. |
| Option Type | Indicates the type of option traded. This field must have a valid DX.OPTION.TYPE record for CDS contracts. |

> **⚠️ Note:** The separate price and valuation can be captured by setting the contract master as an exotic contract.

The DX.OPTION.TYPE record distinguishes each type of Contract. It is mandatory to distinguish each type of contract and capture separate price and valuation, as there is a generic DX.CONTRACT.MASTER for all CDS transactions. Each CDS is identified in the DX.TRADE application based on the underlying and other relevant details. If the Option Type field is not set as EXOTIC, a single DX.MARKET.PRICE record is created for all CDS contracts and it is not possible to distinguish price and valuation. The below screenshot displays a sample of option type that uses Trade ID to create a separate DX.MARKET.PRICE record for each transaction.


#### 🔧 Working With

The section helps the user to work with the CDS feature in Temenos Transact .


##### DX.TRADE

This application supports multiple premium payments, trade capture and delivery confirmations.

The fields used for using CDS are mentioned below.

| Field | Description |
|---|---|
| Contract Code | Indicates the DX.CONTRACT.MASTER ID |
| Buy or Sell | Indicates whether the customer is buying or selling the transaction as determined by the bank |
| Sec Buy Sell | Indicates whether the broker is buying or selling the transaction as determined by the bank |
| Prem Percent | Indicates the initial premium denoted as a percentage of notional amount |
| Underlying Bond | Indicates the instrument to which the CDS contract is created. This field is mandatory. |
| Bond Ccy | Indicates the defaulted trade currency. This is a display-only field. |
| Bond Value | Indicates the principal amount of the bond in asset currency |

For CDS, a P&L entry is raised for the bond value. Read DX.CO.MANUAL.EXERCISE or DX.CO.EXERCISE.AUTO for more information on Exercise.

The below screenshot displays the commission details of the contract.

This application also holds the details of the future premium payments of the contract as indicated in the below fields.

| Field | Description |
|---|---|
| Prem Pay Percentage | Determines whether the premium amount is entered in trade currency or system defaults it by calculating from the percentage defined in the Prem Percent field. The values are: YES - Prem Pymt Amt is a display-only field and the system calculates and generates the amount NO - Prem Pymt Amt is updated manually |
| Prem Pymt Amt | Indicates the amount in the contract currency. When the fields Prem Pay Percentage and Prem Pymt Freq are input, this field is updated with the respective amount. |
| Prem Pymt Freq | Indicates the premium payment frequency. The values are 1–5. |
| Prem Pymt Date | Defines the premium payment date for this period. When the fields Prem Pay Percentage and Prem Pymt Freq are input, this field is updated with the respective duration which is between trade date and maturity date |

> **⚠️ Note:** When the first premium is paid, then the Prem Pymt Freq , Prem Pymt Date and Prem Pymt Amt fields are frozen for user input.

| Column 1 | Column 2 |
|---|---|
| Prem Pay Future | Determines if Prem Pay Future is enabled or not. The values are: YES - Premium amount in the Prem Pymt Amt field is is updated in DX.PREMIUM.DETS and paid in SOD process on the premium date (date in the Prem Pymt Date field) NO - Premium amount is posted immediately with Prem Pymt Date as Value Date |

> **⚠️ Note:** Reversal of trade is not possible after the payment of the first premium.

The Exotic Fld Val holds the unique reference that is defaulted in DX.MARKET.PRICE to differentiate CDS contracts for separate pricing and valuation.

The below screenshot displays the audit fields.


##### DX.PREMIUM.DETS

If the Prem Pay Future field in DX.TRADE is set as Yes, the DX.PREMIUM.DETS live file is created with premium payment details (premium pay date and amount). The DX.PREMIUM.DETS ID defaults the trade ID. The Trade Status field gets updated as Closed, on trade closure.


##### DX.PREMIUM.DETS.HIST

The DX.PREMIUM.DETS.HIST LIVE table is a HISTORY table for DX.PREMIUM.DETS .

On reversal of trade, the records in DX.PREMIUM.DETS and DX.PREMIUM.DETS.HIST are deleted and updated, respectively. The reversal date must be before the first installment of premium payment in COB.

On archival of trade and transactions, the premium details from DX.PREMIUM.DETS are archived and updated in DX.PREMIUM.DETS.HIST .


##### DX.PREM.DETS.PAID

When the premium amount is paid at Start of Day (SOD), the DX.PREM.DETS.PAID LIVE table is created with paid premium details. The DX.PREMIUM.DETS.PAID ID defaults the trade ID. This table tracks the past premium payments. When a premium is posted, the paid premium details are deleted from DX.PREMIUM.DETS and updated in DX.PREM.DETS.PAID .


##### DX.PREM.DETS.PAID.HIST

The DX.PREM.DETS.PAID.HIST LIVE table is a HISTORY table for DX.PREM.DETS.PAID .

On archival of trade and transactions, the premium details from DX.PREM.DETS.PAID are archived and updated in DX.PREMIUM.DETS.PAID.HIST .


##### DX.TRANSACTION

The DX.TRANSACTION LIVE table is a log for trade, order and closeout. Whenever a premium payment is processed during the CDS life cycle, a new transaction is created.

The As Currency and As Principal are display-only fields. These fields default the values from DX.TRADE application.


##### Delivery

In a CDS contract, a SWIFT confirmation message (MT202) is generated on each premium payment.


#### 📋 Tasks

Related topics:

- Expire Credit Default Swaps
- Trading Processes

A Credit Default Swap (CDS) is a financial derivative or contract that allows an investor to swap or offset his or her credit risk with another investor.

To swap the risk of default, the lender buys a CDS from another investor who agrees to reimburse the lender in the case the borrower defaults. Most CDS requires an ongoing premium payment to maintain the contract, which is like an insurance policy.


##### Workflow

This feature allows the user to perform the following tasks:

| SCREENS | WORKFLOW |
|---|---|
|  | CDS Net Position . |
| CDS Position | Click the FIND button. |
| Aggregate net position - Credit Default Swaps | Select the View Trade option from the drop-down and then click the Launch icon. The system opens the record in view mode. |
| Credit Default Swap | Verify the record details. |


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to Credit Default Swap (CDS) in the core banking system.


##### Enquiries and Reports

This section helps the user to view the below enquiries and reports:

Active CDS List

This enquiry displays the active CDS Trades. The user has options to view trade, bond details and delivery messages related to the trade.

Outstanding Premium

This enquiry displays the outstanding premium with date, initial premium collected with initial premium percentage with the total premium value. The user has an option to view the trade details.

Premium Received

This enquiry displays the premium received with trade status, initial premium collected and the total premium value. The user has an option to view the trade details.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


### 3.6  Close Out


> **📇 Quick Reference Card**
> 
> **Purpose:** *An option contract expires and ceases to exist on maturity, if not acted upon before maturity. The buyer of the option can exercise the option if the option contract is in the money( or expire the option when the option contract is out of the money. On the other hand, a future contract cannot be exe...*
> 
> **Key Fields:** *Au Ct Class*, *Au Sett Delay*, *Au Sett Type*, *Call / Put*, *Call or Put*, *Cash Settle Ccy*, *Closeout Trade*, *Closeout Version* ... +56 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

An option contract expires and ceases to exist on maturity, if not acted upon before maturity. The buyer of the option can exercise the option if the option contract is in the money( or expire the option when the option contract is out of the money. On the other hand, a future contract cannot be exercised or assigned before the maturity date. The position can only be closed during maturity.

The brokerage firms automatically exercise these option contracts and do not allow the contracts to expire. When the buyer exercises an option, the option seller is assigned and the seller’s obligation has to be fulfilled. The users can also buy or sell the contracts to close their open positions before expiry.


#### ⚙️ Configuration

Generic configuration is not applicable for the various types of closeouts. Specific configuration is explained against each closeout type.


#### 🔧 Working With

Closeouts are performed against each leg of the contract separately. Temenos Transact is configured to closeout both sides of the deal automatically. The below table refers to the various closeout types and the applications or enquiries used to trigger the closeout.

| Closeout Type | Application | Enquiry | Description |
|---|---|---|---|
| Manual Closeout | DX.CO.MANUAL.INPUT | DX.CO.MANUAL.OPTION.BRWS | For options |
| DX.CO.MANUAL.FUTURE.BRWS | For futures |  |  |
| Maturity Closeout | DX.CO.MATURITY.INPUT | DX.CO.MATURITY.FUTURE.BRWS | For futures |
| Manual Exercise | DX.CO.EXERCISE.MANUAL | DX.CO.MANUAL.EXERCISE.BRWS | For options |
| Manual Expire | DX.CO.EXPIRE.MANUAL | DX.CO.MANUAL.EXPIRE.BRWS | For options |
| Manual Assign | DX.CO.ASSIGN.MANUAL | DX.CO.MANUAL.ASSIGN.BRWS | For options |
| Automatic Closeout | DX.CO.EXERCISE.AUTO |  | For options |
| DX.CO.EXPIRE.AUTO |  | For options |  |
| DX.CO.ASSIGN.AUTO |  | For options |  |
| COB Processing | DX.CO.AUTO.INPUT |  | For setting automatic closeout in DX.CUSTOMER , the Au Ct Class field is set to FUTURES, OPTIONS, BOTH or NONE. The Au Sett Type field is set to FIFO (first in first out), LIFO (last in first out) or FIFO DAY (today’s trades take precedence). The Au Sett Delay field is set to the number of days after trade when settlement or closeout occurs. |
|  |  | Setting the System Exercise in DX.CONTRACT.MASTER enables the system exercise of options during close of business (COB) |  |
|  |  | Setting the System Expiry in DX.CONTRACT.MASTER enables the system expiry of options during COB |  |

> **⚠️ Note:** Closeouts can be triggered by using the enquiries and by launching from the respective applications. Each closeout triggers a record in DX.CLOSEOUT application to perform the closeout.

The cash payouts are posted using the category and transaction codes specified in the respective records in DX.EVENT.TYPE, for example, CM - for contract maturity, AS - contract assignment, EX- contract exercise. In a multi-book environment, when the revaluation service ( DX.RV.SERVICE) and automatic COB closeout are processed, the customer’s SEC.ACC.MASTER (SAM) company context is loaded for the customer transaction and the lead company context is loaded for the broker transaction. As a result, during COB, the closeout record for the customer and broker sides (B2B) are generated in the customer’s SAM company. For online processing, the closeout record is generated in the company where the closeout is manually executed. The inter-company accounting entries are posted as explained below:

| Customer (SAM, Account) | Broker (Account) | Comments |
|---|---|---|
| Lead company | Branch company | Interco entries for broker |
| Branch company | Lead company | No Interco entries |
| Branch company | Branch company | Interco entries for broker |


##### DX.CLOSEOUT

This is the central application for processing the closeouts within the Temenos Transact Derivatives (DX) module. Once a closeout is passed to the closeout engine, a record in DX.CLOSEOUT is created. This record holds all the details of the closeout. Users cannot directly input closeouts into the DX.CLOSEOUT application (this must be done from an external source). Once a closeout is created in the DX.CLOSEOUT application, it can be authorised, deleted or reversed. So the users cannot re-run an existing closeout record, instead the user must run a new closeout. From the DX.CLOSEOUT application, the users can access the information regarding any specific closeout. The Status field denotes the various statuses of closeout as explained in the below table.

| Status | Description |
|---|---|
| RUNNING | Denotes that the closeout is created and processed. The status is updated when the record in DX.CLOSEOUT is in INAU |
| ACTIVE | Denotes that the trades are matched. The status is updated when the record in DX.CLOSEOUT is authorised |
| DELETED | Denotes that the closeout is reversed |

The Type field denotes the style of closeout as explained in the below table.

| Type | Description |
|---|---|
| SETTLEMENT | Identifies basic manual closeouts performed by the system. The field is set to Settlement when the closeout record is created from DX.CO.MANUAL.INPUT |
| MATURITY | Identifies the cash maturity settlements. The field is set to Maturity when the closeout record is created from DX.CO.MATURITY.INPUT |
| SYSTEM | Indicates the closeouts generated by the system under a specific set of circumstances. This is updated when the system is setup for automatic closeout ( System Exercise and System Expiry are set to Y) |
| EXERCISE | Indicates that the closeout records are generated from DX.CO.EXERCISE.MANUAL |
| EXPIRY | Indicates that the closeout records are generated from DX.CO.EXPIRE.MANUAL |
| ASSIGNMENT | Indicates that the closeout records are generated from DX.CO.ASSIGN.MANUAL |

The below screenshot shows a record in DX.CLOSEOUT of an option contract where the contract is exercised by the customer.

The below section explains the various methods in Temenos Transact to closeout options and futures.


##### Buy or Sell to Close

Closeouts (or settlements) are used to match the opposing buy or sell positions within the same contract to effectively close the open positions and realise the due profit or loss, if any. After the settlement, the position is closed out and the respective profit or loss is realised. The due commission or other charges to be paid during the settlement are also posted. Normally, exchange traded derivative contracts are not held until maturity. A derivative order input is used to offset an existing trade(s) by means of cash settlement of the profit or loss and the underlying product is not delivered during closeout. The details of the trade(s) to be offset by the order are captured during order input. When filling the order in the market, the system creates a trade and closes out this against the existing trade, thus offsetting the position.

In this method of closeout, the opposing buy and sell positions can be matched within the same contract to effectively close the open positions and realise the profit or loss dues, if any. The below screen shot shows closing out an options contract using DX.ORDER record.

The following fields of DX.ORDER are explained below.

| Field | Description |
|---|---|
| Order Closeout | Accepts the following values: Blank - If this field is left blank, changes are not made to the current processing. This option is selected by default Close - If this field is set to Close, a DX.TRADE of the trade which is to be off-set (closed out) is filled in the Closeout Trade field |
| Closeout Trade | Contains a valid DX.TRADE ID. This is the ID of the trade that has to be offset. The system throws a validation if the order ID being input does not match the trade (that is, the instrument, strike price, maturity date, call or put indicator does not match with the trade being offset). This is to ensure that the user enters the correct ID. A context enquiry is also provided against this field to list the trades that can be offset by this order. The version to be used for creating an automatic closeout record needs to be specified in the Closeout Version field in the DX.PARAMETER application. |


##### Futures Closeout

A futures contract can either be matured or offset by taking the opposite position. The two types of future closeout are explained below.

Manual closing out of futures by taking opposite position can be triggered through

- enquiry - (DX.CO.MANUAL.FUTURE.BRWS) or
- DX.CO.MANUAL.INPUT

The contract (future) is closed out by specifying the number of lots to be closed. On specifying the lots to be closed from the enquiry, the system creates a record in DX.CO.MANUAL.INPUT , which in turn creates a record in DX.CLOSEOUT. The enquiry selection criteria for futures closeout (maturity) involves the specification of a contract code, a delivery period and portfolio. The user may now select the trades and the number lots from each trade that has to be settled. The closeout is confirmed, as long as the total number of buy lots are same as the total number of sell lots.

The result of the enquiry search is shown below from which the number of lots to be closed out can be specified in Closeout Lots column.

The user must confirm whether the selected trade is the one for which the closeout has to be processed and select the number of lots from each trade to be settled. The record can be committed as long as the total numbers of buy and sell lots are same. A Manual Future/ Stock Closeout screen is displayed with the total profit or loss realised on the trades that are closed out and list of options to create an authorised or unauthorised record in DX.CLOSEOUT . When an unauthorised record in DX.CLOSEOUT is created, the user has to subsequently authorise the record so that the system can generate the realised profit and loss entries. However, when the record in DX.CLOSEOUT is created in authorised status, these entries are generated immediately.

The bank users must run the relevant enquiry to process a new manual closeout. Once the settlement is confirmed, the closeout engine reports the following:

- The current closeout ID
- Profit or loss realised in the closeout
- Any commission charged as part of the closeout

The closeout ID generated is an ID to the primary side closeout record held in the DX.CLOSEOUT application. The lots chosen for closing are processed through the Tra Pnd Sett and Tra Pnd Lots fields in the DX.TRANSACTION application. These fields hold the closeout ID and the number of lots pending for closeout. In DX.CO.MANUAL.INPUT , when the DX.CLOSEOUT (unauthorised) is set created, the below fields in DX.TRADE are updated to display the number of lots pending for settlement:

- Pri Pnd Sett
- Sec Pnd Sett
- Pri Pnd Lots
- Sec Pnd Lots

> **⚠️ Note:** The user cannot directly input into the DX.CLOSEOUT application using INPUT function. The users can only authorise, delete, or reverse a closeout. After authorising the closeout, the number of open lots in the DX.TRADE and DX.TRANSACTION are decremented, and the closeout details are moved to Trasettnos field in DX.TRANSACTION and to Pri Settnos or Sec Settnos fields in DX.TRADE .

Any commissions, profit or loss for the closeout are posted after authorisation.

The DX.CO.MATURITY.INPUT application is used for maturing a futures contract. The application can also be launched through a front-end enquiry Cash Maturity Future/Stock Closeout (DX.CO.MATURITY.FUTURE.BRWS). The following is an example of a futures stock maturity closeout in Temenos Transact that identifies what constitutes a pseudo transaction or trade.

- If the user wishes to closeout a transaction of a sell of a quantity of 25 lots of the instrument Dec00 Chicago Mercantile Exchange (CME) GBP currency futures at 1.4245, the Exchange Delivery Settlement Price (EDSP) at the time of the maturity closeout is 1.4400.
- Then the original transaction is cash settled against a buy of quantity of 25 lots of the instrument Dec00 (CME) GBP currency futures on December 12, 2000 at 1.4400. This transaction is automatically created as a pseudo transaction and it does not physically exist as a position within Temenos Transact.
- The short position of 25 lots is cash settled against a long position of 25 lots.
- The overall position is now zero.
- The profit and loss is the difference between the sums of sell and buy values: 25 lots *internal price = USD 2,225,781.25 25 lots * internal price = USD 2,250,000.00 A loss of USD 24,218.75 is realised

The below explains the process of closing out a future contract through maturity.

1. Input values for the Cash Maturity Future/Stock Closeout (DX.CO.MATURITY.FUTURE.BRWS) enquiry shown below.
2. Then, the user selects the trades and the number of lots from each trade to be settled before committing the record. The system creates a new record in DX.CO.MATURITY.INPUT (similar to DX.CO.MANUAL.INPUT )
3. Once a maturity price is entered, the settlement is confirmed to produce either an authorised or unauthorised closeout record.
4. Once the settlement is authorised, the closeout engine reports the current closeout ID, profit or loss of the closeout and any commission charged as part of the closeout.

Futures contracts which need to be settled physically must be configured in the system. The Delivery Method field in the respective DX.CONTRACT.MASTER record of the Futures contract needs to be set to Physical.

On maturity of contract, a record in DX.CO.MATURITY.INPUT is created automatically by the system. A record can also be manually created by the user to mature the futures contract.

The DX.CLOSEOUT records are created on both the customer and counterparty sides in INAU or LIVE status based on the Unauth Auth field value in DX.CO.MATURITY.INPUT to mark the termination of the contract on both the sides.

Once the records in DX.CLOSEOUT are authorised, a corresponding SEC.TRADE record is created with Record Status set to IHLD status for the underlying security for physical settlement of the trade.


##### Options Closeout

The buyer of an option can exercise or expire the option while the seller can be assigned. Option exercise, expiry and assignment can be manual processes, where a user can select the trades and lots to be processed. It can also be an automatic process where the system does the selection. The processing methodologies are identical regardless the method used to select the transactions. For the options being exercised or assigned, the appropriate corresponding transactions ( SEC.TRADE or FOREX ) are also created.

Hence, depending on the position taken and based on whether the option is ’In the money’ or ’Out of the money’ an option contract can be:

- Assigned
- Exercised
- Expired

Apart from the above methods, an option can also be manually closed out (by taking the opposite position). All of the above can be triggered manually or automatically.

| Fields | Description |
|---|---|
| Settlement Ccy | Holds the currency of the cash payout |
| Settlement Amount | For cash settled options, the cash payout is calculated by the system (by comparing the spot price of the underlying against the strike price). This can be amended by the user. Cash entry is generated for this amount when the closeout is processed |
| Market Price | Holds the market price of the underlying security at the time of assignment |
| Cash Settle Ccy | Holds the delivery currency for the options with underlying as SECURITY.MASTER when the Settlement Method field is set to CASH. The exchange rate between this currency and contract currency is defined in the Delivery Ccy Rate field |
| Delivery Ccy Rate | Holds the exchange rate between contract and delivery currency |
| Settlement Instrument | The alternate settlement instrument which is settled on exercise |
| Sett Instrument Contract Size | Holds the contract size of the alternate settlement instrument which is mandatory, when settled using alternate underlying |
| Sett Instrument Price | Holds the price of the alternate settlement instrument which is mandatory, when settled using alternate underlying |
| Quote Ccy | Holds the currency in which the value in the Spot Exchange Rate field is quoted |
| Spot Exchange Rate | Holds the current exchange rate between the currency pairs of an FX option quoted in the Quote Ccy field |
| Fx Payout Currency | Holds the currency in which the payout is to be made |
| Spot Payout Rate | Holds the exchange rate between Quote Ccy and Fx Payout Currency fields |

| Fields | Description |
|---|---|
| Settlement Ccy | Holds the currency of the cash payout |
| Settlement Amount | For cash settled options, the cash payout is calculated by the system (by comparing the spot price of the underlying security against the strike price). This can be amended by the user. Cash entry is generated for this amount when the closeout is processed. |
| Market Price | Holds the market price of the underlying security at the time of exercise |
| Cash Settle Ccy | Holds the delivery currency for the options with underlying as SECURITY.MASTER when the Settlement Method field is set to CASH. The exchange rate between this currency and contract currency is defined in the Delivery Ccy Rate field. |
| Delivery Ccy Rate | Holds the exchange rate between contract and delivery currency |
| Settlement Instrument | Indicates the alternate settlement instrument that is settled on exercise |
| Sett Instrument Contract Size | Holds the contract size of the alternate settlement instrument, which is mandatory when settled using alternate underlying |
| Sett Instrument Price | Holds the price of the alternate settlement instrument, which is mandatory when settled using alternate underlying |
| Quote Ccy | Holds the currency in which the Spot Exchange Rate is quoted |
| Spot Exchange Rate | Holds the current exchange rate between the currency pairs of FX option quoted in the Quote Ccy field |
| Fx Payout Currency | Holds the currency in which the payout is to be made |
| Spot Payout Rate | Holds the exchange rate between the Quote Ccy and Fx Payout Currency fields |

If the option is out of the money, the option buyer can choose to expire the option. The process is similar to the exercise of option.

Using the Manual Option Expiry (DX.CO.MANUAL.EXPIRE.BRWS) enquiry, the user can manually choose the options to expire. According to the selection criteria, the trades are displayed.

The user can select the transactions and the number of lots to be expired, and then commit the selection.

On authorising the manual expiry, the closeout (expiry) is done through the DX.CO.EXP.MANUAL.SERVICE, which removes these options from the open position and makes the necessary postings.

> **⚠️ Note:** The postings include premiums for contracts with posting at the time of settlement.

The DX.CO.EXPIRE.AUTO application is used to configure the system to automatically choose the options to expire.

If the Cust Or Port mandatory field is set to ALL, the close out (expiry) is done through the DX.CO.EXP.AUTO.SERVICE.


##### Manual Closeout of Option

Manual closing out of options is similar to that explained for futures. This is done by taking opposite position to the original position and can be triggered through

- Enquiry - (DX.CO.MANUAL.OPTION.BRWS) or
- DX.CO.MANUAL.INPUT

The contract (option) is closed out by specifying the number of lots to be closed. On specifying the lots to be closed from the enquiry, the system creates a record in DX.CO.MANUAL.INPUT , which in turn creates a record in DX.CLOSEOUT . The enquiry selection criteria for options involve the selection of a contract code, a delivery period, a strike price and the option type (call or put). In addition, values are entered in other fields to further restrict the selection of trades. All the open trades matching these criteria are displayed. The user may now select the trades and the number lots from each trade that have to be settled. The close out is confirmed as long as the total number of buy lots are same as the total number of sell lots.


##### Automatic or System Closeout

The below explains how an automatic or system closeout of options is performed in the system.

| Application | Description |
|---|---|
| DX.EXCHANGE.MASTER | The Sett Allowed field is set to: Yes - Allows settlement or closeout on the exchange No - Disables the settlement or closeout Leaving this field blank defaults to Yes. |
| DX.CUSTOMER | The Au Ct Class field is set to FUTURES, OPTIONS, BOTH or NONE. The Au Sett Type field is set to FIFO (first in first out), LIFO (last in first out) or FIFO DAY (current day’s trades take precedence). The Au Sett Delay field is set to the number of days after trade when settlement or closeout can occur. |
| DX.CONTRACT.MASTER | The Sett Allowed field is set to: Yes - Allows the settlement or closeout No – Does not allow the settlement or closeout Blank - Defaults to DX.EXCHANGE.MASTER setting |
| DX.TRADE | The Xxx Allow Sett ( Pri Allow Sett or Sec Allow Sett ) field is set to: Yes - Allows settlement or closeout No - Prohibits auto or system settlement for the closeout |


##### System Closeout

This method is identical to the automatic option exercise and expiry processes except that the user initiates the end of exchange process. To trigger automatic expire and exercise, the System Exercise or System Expire needs to be set in DX.CONTRACT.MASTER of the respective contract. The system selects the options that require processing by checking the last trade or declaration dates in the open trades (that is, Dec Date as Today). It also checks that the customer or trade is not set up to hold the options open for a certain number of days. The system determines if each option trade must be exercised, expired or left alone based on the following:

- Strike price
- Underlying price
- Price differences defined in the DX.CONTRACT.MASTER application

> **⚠️ Note:** For options, the system assignment is not supported as it cannot automatically determine the accurate number of lots that the bank has been assigned. If the Settlement Method is Physical and the option is ‘in the money’ during COB of the declaration date, a record in SEC.TRADE (in case of Equity option) or Forex contract (in case of a forex option) is created in IHLD status.

If the Settlement Method is Cash and the option is ‘in the money’ during the COB of the declaration date, the closeout occurs in two ways:

- If the Review Cash Posting field is set as Yes in DX.PARAMETER , a record is created in the DX.CO.EXERCISE.MANUAL application in IHLD status. The value in the Settlement Amount field is updated based on the difference between the strike price of the contract and the spot price on the declaration date. When the record in the DX.CO.EXERCISE.MANUAL application is authorised, a record in DX.CLOSEOUT is created with Live status and the position is removed (the holdings in the contract are liquidated). An accounting entry is generated for the settlement amount when the record in DX.CLOSEOUT is authorised. The settlement amount can be modified by launching the Update Settlement Amount (DX.CO.EXERCISE.MANU.AUTH) fast path enquiry and by directly entering the settlement amount for the close-out.
- If the Review Cash Posting field is set as No in DX.PARAMETER , a record is created in DX.CO.EXERCISE.MANUAL with Live status and a record in DX.CLOSEOUT is created. The value in the Settlement Amount field is updated with the difference between the strike price of the contract and the spot price on the declaration date. An accounting entry is generated for the settlement amount, which cannot be reviewed by the user once posted.

If the Settlement Method field is Cash and the option is ‘out of the money’ during the COB of the declaration date, a record is created in DX.CO.EXPIRE.MANUAL . There is no accounting entry generated in this case and the position in the contract is closed.


##### Closing Out FX OTC Options

The FX OTC options are exercised and expired through the DX.CO.EXERCISE.AUTO and DX.CO.EXPIRE.AUTO applications. The following table explains the applications and the respective field settings.

| Application | Field | Description |
|---|---|---|
| DX.CO.EXERCISE.AUTO | Contract Ccy | Indicates the contract currency of option to be exercised. The currency must be a valid currency in the CURRENCY application, and it is a mandatory field for FX OTC options. |
| Delivery Ccy | Indicates the delivery currency of option to be exercised. The currency must be a valid currency in CURRENCY , and it is a mandatory field for FX OTC options. |  |
| DX.CO.EXPIRE.AUTO | Contract Ccy | Indicates the contract currency of option to be expired. The currency must be a valid currency in CURRENCY , and it is a mandatory field for FX OTC options. |
| Delivery Ccy | Indicates the delivery currency of option to be expired. The currency must be a valid currency in CURRENCY , and it is a mandatory field for FX OTC options. |  |


##### Option Settlement - Cash Payout

Temenos Transact supports multiple settlement methods for options. The option can be settled either physically or with cash. For options with underlying security, it is also possible to settle the option through an alternate instrument.

In certain markets, for options, the underlying Taiwanese share is non-deliverable (as a result of a regulatory constraint). Therefore, the option is settled through a participatory note issued by the option writer.

The user can input the value to determine the payout (spot price of the underlying for cash settlement or the quantity and price for settlement through an alternate instrument) in the closeout suite of applications. The same is used when the closeout is processed.

The cash payout on equity options is calculated as:

For a buyer of a CALL option, the cash payout is

For a buyer of a PUT option, the cash payout is

The following field settings are required for FX options during cash payout:

| Field | Description |
|---|---|
| Quote Ccy | Delivery and strike quote currencies for normal FX and generic FX OTC options, respectively |
| Spot Exchange Rate | The exchange rate between contract and the value in the Quote Ccy field |
| Fx Payout Ccy and Spot Payout Rate | The exchange rate between Fx Payout Currency and Quote Ccy fields |

Cash payout for an FX option is as described below:

For buyer of an FX CALL with delivery currency as weaker currency and trade currency as stronger currency with quote currency as stronger currency.

For buyer of an FX CALL with delivery currency as stronger currency and trade currency as weaker currency with quote currency as weaker currency.

For buyer of an FX PUT with delivery currency as weaker currency and trade currency as stronger currency with quote currency as weaker currency.

For buyer of an FX Put with delivery currency as stronger currency and trade currency as weaker currency with quote currency as stronger currency.

For buyer of FX CALL with delivery currency as weaker currency and trade currency as stronger currency with quote currency as weaker currency.

For buyer of FX CALL with delivery currency as stronger currency and trade currency as weaker currency with quote currency as stronger currency.

For buyer of FX PUT with delivery currency as weaker currency and trade currency as stronger currency with quote currency as stronger currency.

For buyer of FX PUT with delivery currency as stronger currency and trade currency as weaker currency with quote currency as weaker currency.


#### 📋 Tasks

Related topics:

- Exercise Option or Assignment
- Execute Settlement (Securities)
- Trading Processes
- Perform Auto Exercise or Expiry of Options

Closeouts or settlements are used to match opposing buy or sell positions within the same contract to effectively close the open positions and realise any profit or loss due. Once the settlement has occurred, the position is closed-out and profit or loss is realised. Commission and charges due to be paid at the settlement time are also posted.

The system supports the Auto Exercise and Auto Expiry of cash settled options during the end of the day processing. All In The Money (ITM) options which are not exercised until the last date must be auto exercised. The difference between the strike price and market price should be settled between the party and counterparty during the end of exchange processing. All Out of The Money (OTM) options which are not expired until the last date must be expired and the trade should be closed.


##### Workflow

In Close Out, the user can perform the following activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Manual Exercise Option . |
| List of Buy Option Trades | Enter values in the following mandatory fields: Contract Code Maturity Strike Call / Put Click the FIND button. Click the Exercise Lots icon. |
| Sys | Enter a value in the Expire Lots field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Manual Expiry Option . |
| List of Active Option Trades | Enter values in the following mandatory fields: Contract Code Maturity Strike Call / Put Click the FIND button. Click the Expire Lots icon. |
| Manual Option-Expire | Enter values in the required fields. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Manual Assign Option . |
| List of Sell Option Trades | Enter values in the following mandatory fields: Contract Code Maturity Strike Call / Put Click the FIND button. Click the Assign Lots icon. |
| Sys | Enter a value in the Expire Lots field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

The user can perform the automatic assignment of options.

To assign the lots automatically, perform the following steps:

1. Auto Assign Option .
2. In the Automatic Assignments tab, enter values in the following fields:
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon.

The user can perform the automatic exercise of options.

To exercise the lots automatically, perform the following steps:

1. Auto Exercise Option .
2. In the Auto tab, enter values in the following fields:
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon.

The user can perform the automatic expiry of trades.

To expire the lots automatically, perform the following steps:

1. Auto Expiry Option .
2. In the Auto Expiry tab, enter values in the following fields:
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon.

| SCREENS | WORKFLOW |
|---|---|
|  | Manual Mature Future . |
| List of Active Future Trades | Enter values in the following mandatory fields: Contract Code Maturity Click the FIND button. Click the Closeout buy vs sell icon. |
| Manual Closeout Input Feed | Enter a value in the Expired Lots field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

This enquiry enables the user to perform a manual closeout of the matching buy and sell positions of a customer for option contracts.

1. Manual Closeout Option .
2. Enter values in the below mandatory fields and in other required fields: Contract Code Maturity Strike Call / Put
3. Click the FIND button.
4. Enter the trade ID and then select the number of lots to be closed out.
5. Click the Commit icon.

This enquiry enables the user to perform a manual closeout of the matching buy and sell positions of a customer for future contracts.

1. Manual Closeout Future .
2. Enter values in the below mandatory fields and then click the FIND button. Contract Code Maturity
3. Enter the trade ID and then select the number of lots to be closed out.
4. Click the Commit icon.

This enquiry displays the list of exercise manual records created in IHLD. It allows the user to update the market price.

To update the market price, follow the steps below:

1. Update Market Price .
2. Click the FIND button.
3. Click the Update Market Price icon corresponding to a record.
4. In Manual Exercise screen, enter value in the Market Price field.
5. Click the Validate icon to check for errors and overrides.
6. Click the Commit icon.

This enquiry displays the list of exercise manual records created in IHLD. It allows the user to update the settlement amount.

To update the settlement amount, follow the steps below:

1. Update Settlement Amount ,
2. Click the FIND button.
3. Select the record and enter value in Settlement Amount field.
4. Click the Auth icon to commit the record.

This enquiry displays the list of auto assign options pending for authorisation.

To view a record, follow the below steps:

1. Authorise Assign Options .
2. Click the View icon.

To edit a record, follow the below steps:

1. Authorise Assign Options .
2. Click the Edit icon.
3. Amend values in the required fields.
4. Click the Validate icon.
5. Click the Commit icon.

To authorise a record, follow the below steps:

1. Authorise Assign Options .
2. Click the Authorise icon.

To delete a record, follow the below steps:

1. Authorise Assign Options .
2. Click the Delete icon.
3. Click the Delete icon to delete the record.

This enquiry displays the list of transactions with manually assigned options pending for authorisation.

To view a record, follow the below steps:

1. Authorise Assign Options .
2. Click the View icon.

To edit a record, follow the below steps:

1. Authorise Assign Options .
2. Click the Edit icon.
3. Amend values in the required fields.
4. Click the Validate icon.
5. Click the Commit icon.

To authorise a record, follow the below steps:

1. Authorise Assign Options .
2. Click the Authorise icon.

To delete a record, follow the below steps:

1. Authorise Assign Options .
2. Click the Delete icon.
3. Click the Delete icon to delete the record.

This enquiry displays the list of auto exercise options pending for authorisation.

To view a record, follow the below steps:

1. Authorise Exercise Options .
2. Click the View icon.

To edit the record, follow the below steps:

1. Authorise Exercise Options .
2. Click the Edit icon.
3. Amend values in the required fields.
4. Click the Validate icon.
5. Click the Commit icon.

To authorise a record, follow the below steps:

1. Authorise Exercise Options .
2. Click the Authorise icon.

To delete a record, follow the below steps:

1. Authorise Exercise Options .
2. Click the Delete icon.
3. Click the Delete icon to delete the record.

This enquiry displays the list of transactions with manually exercised options pending for authorization.

To view a record, follow the below steps:

1. Authorise Exercise Options .
2. Click the View icon.

To edit a record, follow the below steps:

1. Authorise Exercise Options .
2. Click the Edit icon.
3. Amend values in the required fields.
4. Click the Validate icon.
5. Click the Commit icon.

To authorise the record, follow the below steps:

1. Authorise Exercise Options .
2. Click the Authorise icon.

To delete the record, follow the below steps:

1. Authorise Exercise Options .
2. Click the Delete icon.
3. Click the Delete icon to delete the record.

This enquiry displays the list of auto expiry options pending for authorisation.

To view a record, follow the below steps:

1. Authorise Expire Options .
2. Click the View icon.

To edit a record, follow the below steps:

1. Authorise Expire Options .
2. Click the Edit icon.
3. Amend values in the required fields.
4. Click the Validate icon.
5. Click the Commit icon.

To authorise a record, follow the below steps:

1. Authorise Expire Options .
2. Click the Authorise icon.

To delete a record, follow the below steps:

1. Authorise Expiry Options .
2. Click the Delete icon.
3. Click the Delete icon to delete the record.

This enquiry displays the list of transactions with manually expired options pending for authorisation.

To view a record, follow the below steps:

1. Authorise Expire Options .
2. Click the View icon.

To edit a record, follow the below steps:

1. Authorise Expire Options .
2. Click the Edit icon.
3. Amend values in the required fields
4. Click the Validate icon.
5. Click the Commit icon.

To authorise a record, follow the below steps:

1. Authorise Expire Options .
2. Click the Authorise icon.

To delete a record, follow the below steps:

1. Authorise Expiry Options .
2. Click the Delete icon.
3. Click the Delete icon to delete the record.

This enquiry displays the list of transactions with manual closeout options pending for authorisation.

To view a record, follow the below steps:

1. Authorise Manual Closeouts .
2. Click the View icon.

To edit a record, follow the below steps:

1. Authorise Manual Closeouts .
2. Click the Edit icon.
3. Amend values in the required fields.
4. Click the Validate icon.
5. Click the Commit icon.

To authorise the record, follow the below steps:

1. Authorise Manual Closeouts .
2. Click the Authorise icon.

To delete a record, follow the below steps:

1. Authorise Manual Closeouts .
2. Click the Delete icon.
3. Click the Delete icon to delete the record.

This enquiry displays the list of transactions with manual maturity options pending for authorisation.

To view the record, follow the below steps:

1. Authorise Manual Maturities .
2. Click the View icon.

To edit a record, follow the below steps:

1. Authorise Manual Maturities .
2. Click the Edit icon.
3. Amend values in the required fields.
4. Click the Validate icon.
5. Click the Commit icon.

To authorise a record, follow the below steps:

1. Authorise Manual Maturities .
2. Click the Authorise icon.

To delete a record, follow the below steps:

1. Authorise Manual Maturities .
2. Click the Delete icon.
3. Click the Delete icon to delete the record.


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to order processing in the core banking system.


##### Enquiries and Reports

This section allows the user to view the below enquiries and reports.

Auto Exercise Closeout Details .

This enquiry displays the list of exercise manual records created by the system and allows the user to view the closeout records generated.

Auto Expire Closeout Details .

This enquiry displays the list of expire manual records created by the system and allows the user to view the closeout records generated.


##### SWIFT Messages

NA


##### Advices

The user can view the following advices:

An advice is generated on completion of activities like exercise, expiry, assignment, maturity and settlement. These are configured in DX.EVENT.TYPE application for the respective events.


##### Alerts

NA

---


### 3.7  Commissions


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Derivatives (DX) module enables automatic calculation of the trading commission based on the criteria setup in DX.COMMISSION . This facility allows commission and charges based on a number of decision levels as explained in the below table.*
> 
> **Key Fields:** *Channel*, *Charge Percent*, *Clfee Charge*, *Comm Charge*, *Exchange Type*, *Executing Broker*, *Exfee Charge*, *Field From* ... +20 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The Derivatives (DX) module enables automatic calculation of the trading commission based on the criteria setup in DX.COMMISSION . This facility allows commission and charges based on a number of decision levels as explained in the below table.

| Level | Defaults For |
|---|---|
| System | All conditions |
| Group | Customer groups setup within DX.GROUPING Contract groups setup within DX.CONTRACT.CLASS |
| Individual | Specific customer setup within DX.CUSTOMER Specific contract setup with DX.CONTRACT.MASTER |

The commission can be setup for the following combinations of customer or group or contract. These elements are separated by ‘-‘ and can be combined together to create the commission code. The codes, which denote a narrower scope of grouping are selected in precedence to those with greater generalisation. In each search to calculate commission, the order of priority and the list of valid combinations are given below:

- Customer and contract
- Customer and contract class
- Customer
- Customer group and contract
- Customer group and contract class
- Customer group
- Contract
- Contract class
- System default


#### ⚙️ Configuration

The procedure to determine the appropriate commission table can be controlled by the Search All Commsn field in DX.PARAMETER . If this field is set to No, records are not searched further after a record is matched with the key. If this field is set to Yes, each record found is searched to find all matching criteria.

The commission codes may be entered in the following formats.

| ID | Description | Abbreviation |
|---|---|---|
| CU100018 | Customer 100018 | (CU = Customer Code) |
| CGINT2 | Customer Group INT2 | (CG = Customer Group) |
| CT100 | Contract Code 100 | (CT = Contract Code) |
| CCGILTS | Contract Class GILTS | (CC = Contract Class) |
| CU100018-CT100 | Customer 100018, Contract 100 | (CU = Customer Code), (CT = Contract Code) |
| CU100018-CCGILTS | Customer 100018, Contract Class GILTS | (CU = Customer Code), (CC = Contract Class) |
| CGINT2-CT100 | Customer Group INT2, Contract 100 | (CG = Customer Group), (CT = Contract Code) |
| CGINT2-CCGILTS | Customer Group INT2, Contract Class GILTS | (CG = Customer Group), (CC = Contract Class) |
| SYSTEM | Catch All | System level defaults |

For the system to interpret the input, a two-character prefix is used to identify each element. Also, the application recognises mnemonics used by the source applications.

The extra criteria for determining the calculation of commission and charges are defined in DX.COMMISSION . The Field Name field contains a drop down list of fields from DX.TRADE . When a field is selected, the contents from the trade are compared, using the entry in the Operator field, against the values in the Field From and Field To fields. These fields are sub-valued for the tests to be combined for better refinement. The secondary leg fields on the trade are not listed in the Field Name field. If a primary leg field is selected, the corresponding secondary trade field name is displayed in the Sec Field Name field. This is used in tests for customers, which appear on the secondary leg of the trade.

The below screenshot shows an example which requires the following two conditions to be satisfied:

- The trade currency is equal to USD
- The number of lots is between 10 and 20

If either of the condition proves to be false for the trade, the commissions specified in this test set is not used.

Once the trade details are matched, up to five different types of commission and charges can be calculated. Each type can contain a commission or charge code linked to either FT.COMMISSION.TYPE or FT.CHARGE.TYPE . The types of commission or charges and fields in which they are entered are given in the below table.

| Commission Type | Field Name |
|---|---|
| Commissions | Comm Charge |
| Execution fees | Exfee Charge |
| Clearing fees | Clfee Charge |
| Regulatory fees | Rgfee Charge |
| Miscellaneous fees | Misc Charge |

More than one commission code can be entered for each commission type, but there is only one commission currency per type. If a commission currency is specified, this value overrides the currency defined in FT.COMMISSION.TYPE or FT.CHARGE.TYPE .

The Charge Percent field indicates a percentage multiplier to be applied for the charge amounts calculated. However, this is performed on types commission, execution and clearing fees only.

A bank has setup a customer group GROUPEXT for all relevant internal (own-book) customers, and a similar group GROUPINT for all non-own-book customers. On behalf of their internal accounts and external customers, they trade European options on EUREX and LIFFE. They are not trading members of any exchange, but use an external broker with the customer number 100324. This broker charges different rates for each exchange. These charges are created in FT.COMMISSION.TYPE as CISERXEXC and CISLIFFEEX, respectively. The bank charges the internal accounts the same rates, but charges the private customers a standard commission amount (STDCUST).

- The following standard exchange rules, commission are only actually charged when a position is closed out. In the GROUPEXT customer commission setup, the Pay Receive field is set to Pay, indicating that the customer is paying the commission to the bank.

- For the EXTERN1 customer group, the Field From is left blank so that the test with Field Name is set to EXCHANGE.CODE and Operator set to NE picks up all exchanges (LIFFE and EUREX in this example).

- The commission set-up for Broker A - 100115 has the Pay Receive field set to Receive, indicating that the bank is paying the commission to the broker.

- Another bank trades only foreign exchange options. It is assumed that there are no overriding commissions for brokers or exchanges and a general system default can be used.
- The bank has two commonly traded currencies (USD and GBP), for which it charges a percentage commission (STDPCNT). If other currencies are traded, extra charges (inputted as NONSTD) are levied.
- The sequence in which these tests are entered in DX.COMMISSION is important. In this scenario, the test for non-standard currencies is placed after the other two tests on the Trade Ccy .


#### 🔧 Working With

The commission fields in DX.TRADE display a summarised form of the commission data. After a trade is committed, detailed analysis of the trading commission can be viewed in DX.COMMISSION.DIAGS .

The following are the two main methods of entering the trading commission for a customer:

- Automatically from criteria set in DX.COMMISSION
- Manually overriding the commission fields

The method selected in the Pri Auto Manual or Sec Auto Manual fields in DX.TRADE controls the commission collection method.


##### Calculating the Commission Automatically

The commission fields are updated automatically in this method. All the defaulting values are driven by the details set in DX.COMMISSION .

In the below example, the commission system has matched a DX.COMMISSION record to this transaction and applied both the execution and clearing commissions. The commission amounts are held in Pri Comm Amt and are calculated at USD 250 and USD 375. The account to post the commissions are updated in the Pri Comm Acc field. If the account currency is different from the commission currency, the exchange rate to calculate the value in the Pri Cacc Amt field is displayed in Pri Comm Exc field. The Pri Comm Tax field indicates that the tax duty is levied on this commission.

If the customer (for whom commission and charges are calculated) is a broker and another broker is indicated in Executing Broker , the account or category for posting the execution fee only is changed to the executing broker’s account for any execution fees to be paid. Because the values of the trade can affect the automatic commission calculations, the commission fields are cleared for any change to a field on the trade. If a customer’s details fail the selection criteria, commission is not calculated and an override message is displayed.


##### Calculating the Commission Manually

For manual input of customer commission, one of the four different commission types are selected. Each commission type can be input only once per customer. The Pri Comm Cde or Sec Comm Cde field allows either of the following:

- A commission code from FT.COMMISSION.TYPE or FT.CHARGE.TYPE (or)
- The text override

If override is entered instead of a commission code, the commission currency, amount and posting account can be entered.

It is also possible to specify commission as a percentage of contract value or trade cost. In such cases, the commission is calculated based on the percentage entered in and the amount is updated in the trade. The commission amount can be amended as per the user requirement. The following example displays the calculating method used for customer number 100163, who is on the secondary side of the trade.

The DX.TRADE application allows the banks to collect commission from customers for exchange traded futures and options, who have entered into the trade by the exchange type (floor or electronic) or mode of transaction (electronic or telephone). The Exchange Type and Channel multi-value fields in DX.TRADE and DX.ORDER are used for this purpose as shown in the below table.

| Field | DX.TRADE | DX.ORDER |
|---|---|---|
| Exchange Type | Indicates the types of exchange used to enter the trade | Indicates the types of exchange used to enter the order |
| Channel | Indicates the modes of transaction used to enter the trade | Indicates the modes of transaction used to enter the order |


##### Trading in Centralised Company

The user can setup where all Securities (SC) and Derivatives (DX) trades take place in a centralised hub, for portfolios belonging to different companies (locations). The Port Comp Id field in SEC.ACC.MASTER holds the HUB Company. The DX trades and transactions take place only in this HUB Company. The portfolio's own company is updated in the Own Company field in SEC.ACC.MASTER .

Based on settings in INTERCO.PARAMETER , the P&L on account of commissions and charges is directly booked to the portfolio's own company. Also, the P&L for broker side charges is re-invoiced to the portfolio's own company through INTERCO accounting entries.


#### 📋 Tasks

There are no Tasks available for Commission and Charges feature.


#### 📊 Outputs

There are no Outputs available for Commission and Charges feature.

---


### 3.8  Constraints


> **📇 Quick Reference Card**
> 
> **Purpose:** *Constraints are set of conditions placed on portfolios or transactions to prohibit (and/or) report certain type of activity based on defined rules at global and institutional levels. The Derivatives (DX) module includes a method of applying constraints to which contracts (and/or) exchanges, customer...*
> 
> **Key Fields:** *Constraint Type*, *Contract Type*, *Exchange Code*, *Logic*, *Message Type*, *Narrative*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Constraints are set of conditions placed on portfolios or transactions to prohibit (and/or) report certain type of activity based on defined rules at global and institutional levels. The Derivatives (DX) module includes a method of applying constraints to which contracts (and/or) exchanges, customers or individual portfolios trade in the module. In DX module, constraints are defined using the DX.TRADING.CONSTRAINT application and the constraints are applied at a transaction level ( DX.ORDER and DX.TRADE ).


#### ⚙️ Configuration

The DX.TRADING.CONSTRAINT application allows setting up of trading constraints for a particular customer or portfolio. Based on the constraints defined here, the system test the data fields in DX.TRADE and DX.ORDER applications to determine whether the customer or portfolio is allowed to trade based on the details entered.

More than one constraint can be defined for a particular portfolio. The ID of DX.TRADING.CONSTRAINT contains either customer or portfolio ID followed by a suffix which can be used to define multiple constraints for the same portfolio.

- 100271.01
- 100271.02
- 100271-1.01

Based on the Constraint Type field, the system decides whether to permit or restrict trading for that particular customer or portfolio. If the Constraint Type is set to Permission, then the transaction is allowed only if the conditions specified are met. If the Constraint Type is set to Restriction, then the transaction is allowed only if the conditions specified are not met. Depending on the settings in the Message Type field, either an error or an override message is generated when the transaction is disallowed.

The Logic field can be used to link multiple conditions. It is possible to specify whether these conditions are logical AND or logical OR conditions. In the screenshot provided below, the system raises an error message in order or trade, if either of the condition is met. The Logic field is set to Or, so that the constraint is triggered if either of the condition is met.

The following error messages are displayed when the customer 100271 either trades in Futures or in Chicago Board of Trade (CBOT) options. When the order or trade is placed for the customer or portfolio with Contract Type field in DX.CONTRACT.MASTER set to Future, then the system generates an error ‘Only Allowed to Trade Options’ message. Similarly, when the order or trade is placed for the customer or portfolio with Exchange Code field in DX.CONTRACT.MASTER equal to 1 (Chicago Board of Trade - CBOT), the system generates an error ‘Not Allowed to Trade CBOT Options’ message.

Using the And operation, a single constraint can be linked together to produce a complex constraint. There is no limit to the number of constraints that can be held within a record. When the user attempts to enter restricted values in any transaction, the constraint displays the appropriate error message (shown in the Narrative field) in DX.TRADE and DX.ORDER .


#### 📋 Tasks

There are no Tasks available for Constraints feature.


#### 📊 Outputs

There are no Outputs available for Constraints feature.

---


### 3.9  Corporate Actions


> **📇 Quick Reference Card**
> 
> **Purpose:** *A corporate actions (CA) is an event initiated by a public company that brings an actual change to the securities, equity or debt issued by the company. For example, Stock split, spin-offs and demergers.*
> 
> **Key Fields:** *Ca Tra Version*, *Contract Code*, *Derivatives*, *Dx Diary Id*, *Event Type*, *Ex Date*, *New Ratio*, *New Str Pri* ... +1 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

A corporate actions (CA) is an event initiated by a public company that brings an actual change to the securities, equity or debt issued by the company. For example, Stock split, spin-offs and demergers.

Such corporate action events affect any derivative contract which has the security as an underlying. This section explains how to setup and process corporate actions such that all derivatives contracts are automatically adjusted.


#### ⚙️ Configuration

Corporate actions (CA) are defined using the DIARY.TYPE application in the Securities (SC) module. When a type of corporate action affects the nature of derivatives contracts in the security, the Derivatives field should be set to YES in DIARY.TYPE .


##### DX.PARAMETER

The Ca Tra Version field in DX.PARAMETER accepts a valid DX.TRADE version. The system uses this version to update the DX.TRADE records when entitlements are authorised.


#### 📋 Tasks

Related topics:

- Enter Diary Events
- Manage Subscription Based Corporate Action
- Administration and Static Data and Corporate Actions

Any activity that brings material change to an organisation and impacts its stakeholders, common and preferred shareholders, as well as bondholders are termed as Corporate Actions.

These events are generally approved by the company's board of directors. Shareholders may be permitted to vote on some events as well. Some corporate actions require shareholders to submit a response.


##### Workflow

This feature allows the user to perform the following tasks:

| SCREENS | WORKFLOW |
|---|---|
|  | Entitlement Actions . |
| List of Unauthorised Entitlements | Click the Authorise icon. |
| Authorise Entitlements | Enter a value in the Dx Diary Id field. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

This screen allows the user to enter a DX Corporate Action event, such as, a Stock split.

1. Generic Diary Capture .
2. In the Contract Screen , click the New icon.
3. Enter values in the following fields: Contract Code Event Type Ex Date Old Ratio New Ratio
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon to submit the record.


#### 📊 Outputs

There are no Outputs available for Corporate Actions feature.

---


### 3.10  Derivatives Contract Master


> **📇 Quick Reference Card**
> 
> **Purpose:** *The contract master for derivatives holds only the static information such as name, mnemonic, exchange on which the contract is traded, type of contract and so on. Dynamic information such as price, strike, maturity date, call or put (in the case of options) and so on are directly entered in the con...*
> 
> **Key Fields:** *Maturity Type*, *Min Price Mvmt.1*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The contract master for derivatives holds only the static information such as name, mnemonic, exchange on which the contract is traded, type of contract and so on. Dynamic information such as price, strike, maturity date, call or put (in the case of options) and so on are directly entered in the contract.


#### ⚙️ Configuration

The DX.CONTRACT.MASTER application holds the contract definitions of all the contracts tradable in the Derivatives (DX) module. This document deals with the configuration of static values in DX.CONTRACT.MASTER . Read the Working with Derivatives Contract Master for more information on the setup and requirements.


#### 📋 Tasks

DX.CONTRACT.MASTER is the main application that defines the characteristics of future , stock or option contracts that can be traded in the derivatives product. Basic contract details, pricing data, trading size, maturity date validation and so on are all captured here. Pay-out can be in terms of the alternate instrument or cash and the same is supported only for Equity options. If the delivery method is Cash, the pay-out currency can be specified.


##### Workflow

In Derivatives Contract Master, the user can perform the following activities:

To create a derivatives contract master for Options, follow the below steps:

1. DX Contract Master Options .
2. In the DX Contract Master tab, enter applicable values in the following fields: Mnemonic GB Descript.1 GB Short Name Exchange Contract Class Contract Type Sub Asset Type Delivery Method Units of Measure Contract Size
3. In the Price Details tab, enter a value in the Min Price Mvmt.1 field.
4. In the Contract Dates tab, enter a value in the Maturity Type field.
5. Click the Validate icon to check for errors and overrides.
6. Click the Commit icon.

To create a derivatives contract master for Futures, follow the below steps:

1. DX Contract Master Futures .
2. In the DX Contract Master tab, enter applicable values in the following fields: Mnemonic GB Descript.1 GB Short Name Exchange Contract Class Contract Type Sub Asset Type Delivery Method Units of Measure Contract Size
3. In the Price Details tab, enter applicable values in the following fields: Tick Size.1 Tick Value.1 Min Price Mvmt.1
4. In the Contract Dates tab, enter a value in the Maturity Type field.
5. Click the Validate icon to check for errors and overrides.
6. Click the Commit icon.

The DX.CREATE.PRICE application enables the user to input the pricing information for the derivatives master. Once the price details are created, system automatically creates a corresponding record in DX.MARKET.PRICE .

To enable pricing information for the derivatives master, follow the below steps:

1. Dx Create Price .
2. Enter applicable values in the following fields: Price Set Contract Code Maturity Date Trade Ccy
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon.


#### 📊 Outputs

There are no Outputs available forDerivatives Contract Master feature.

---


### 3.11  Derivatives Price Update


> **📇 Quick Reference Card**
> 
> **Purpose:** *Pricing of Derivatives (DX) contracts is very critical for many reasons. It determines whether the contract is in-the-money or at-the-money or out-of-the-money. It also determines the amount of variation margin to be paid or received and the value of the contract on any given day.*
> 
> **Key Fields:** *Alternative Price Set*, *B2B Reference*, *Build Pgm*, *Call/Put*, *Cons Data Item*, *Cons Data Name*, *Contract*, *Currnt/Closng/Whatif* ... +38 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Pricing of Derivatives (DX) contracts is very critical for many reasons. It determines whether the contract is in-the-money or at-the-money or out-of-the-money. It also determines the amount of variation margin to be paid or received and the value of the contract on any given day.


#### ⚙️ Configuration

This section explains the initial setup needed for updating prices of DX contracts.


##### DX.PRICE.SOURCE

The price in a derivative contract can be updated using various methods or sources. Price source describes what sort of pricing model is to be used. The sources can be manually input or using internal calculation routines such as Black and Scholes or through external data feed. The DX.PRICE.SOURCE application stores the various possible price sources, and if the price is to be determined by a calculation routine then the Program field is also updated in this application. .

When record Id in DX.PRICE.SOURCE is set to INTERFACE, then the DX.MARKET.PRICE application is not used to update prices. The value INTERFACE is set for OTC contracts, and in such instances, the SYDX.MARKET.VAL application is used to update the valuation amount.

> **⚠️ Note:** For OTC products, instead of prices, a valuation amount is updated per contract.

The following fields should be set up in DX.PRICE.SOURCE .

The Update Avail field should be set to Yes.

If an external price feed is deactivated, the

switch stops the DX system from requesting information from the price feed, and requires a manual update to take place in

.

The following section shows how to use and implement the Garman Kohlhagen (GK) method of price calculation.

| Field Name | Value |
|---|---|
| Interest Rate | Contract Currency |
| Sec Int Rate | Delivery Currency |
| Interest Basis | Interest Basis of the Contract Currency |
| Strike | Strike |
| Call/Put | Call Price/Put Price |
| Volatility | Call/Put Volatility |
| Underlying Price | Underlying Price or Exchange price of the two currencies |
| Und Int Price | Underlying Internal Price |


##### DX.PRICE.SET

The DX.PRICE.SET application allows the storage of different prices.

One price set is called CLOSING and could be used to store the official market closing price for exchange traded futures and options. Another price set is called CURRENT and could be used to store the real-time prices of the derivatives contract. The WHATIF price set can be used for speculative prices. This is just for simulation and does not result in accounting entries. Valuations for a position can then be performed using any of the price sets.

The following screenshot illustrates a DX.PRICE.SET that allows prices to be requested from a DX.PRICE.SOURCE, if it is not updated in the last 30 minutes. It is possible to leave these fields blank, which ensures that for the price set, the prices are always updated only on request and not be updated automatically after certain number of minutes.

Only one price set, usually Closing, is used for end-of-day processing which does valuation and margin Mark To Market accounting. The price set to be used for EOD processing is mentioned in DX.PARAMETER as shown in the following screenshot.


##### DX.CONTRACT.MASTER

For contracts that the user wants to have priced by a particular price source, the bank has to configure this field in the records in DX.CONTRACT.MASTER . The Price Set field is set to CLOSING, and the Price Source field is set to GK, which is used to generate a price. This means that closing prices are updated using GK price source.


#### 🔧 Working With

This topic discusses about how price update is performed for contracts.


##### DX.MARKET.PRICE

This application holds all the pricing information for contracts tradable in the Derivatives (DX) module. This application uniquely identifies the instrument, as for the same record in DX.CONTRACT.MASTER , there can be different strikes prices and maturities. The strike price and the maturity, along with the CALL/PUT indicator, is fed in at the trade level. All these factors (call/put option, strikes, maturity) form part of the DX.MARKET.PRICE ID and therefore uniquely identifies the instrument.

It allows the correct valuation of open positions (trades). The actual method used to value a position can vary; however, most methods rely on a market or fair value price. The system values all the portfolios during the revaluation process using a closing or fair value price. For exchange-based contracts, all the exchanges provide an official settlement price also called exchange delivery settlement price (EDSP). For over-the-counter (OTC) options, the prices are often manually input, calculated, or received from an external source. Throughout the day, when the contracts are being traded, current (or last) prices might be received which, if stored, allows online real valuations to take place.

In addition, users may want to change prices based on what they think might occur in the market and then revalue a portfolio based on these speculative prices. The application is therefore required to accept and store prices in the following situations:

- Manual price input
- Automatic price feeds (for example, Reuters, Telerate and Telekurs)
- Batch-based price downloads (for example, SPAN Risk Parameter tables)
- Ability to call a price model routine and store the returned price (for example, Black and Scholes)
- User-created speculative or What If prices

To understand the pricing in DX, it is important to understand the DX.MARKET.PRICE application. Prices within the DX module are identified by a combination of factors, for example, their price set, contract, the maturity date, or strike price of the contract.

- The CLOSING price for a JUN04 LIFFE Short Sterling Future (FSS) is identified as:

CLOSING:/110000/GBP/202006////:

where, CLOSING is the price set, 110000 is the contract, GBP is the contract currency and 202006 is the maturity year and month.

- Similarly, the CLOSING price for a JUN04 LIFFE Short Sterling Option (FSO) is identified as:

CLOSING:/ 210003/GBP/202006/CALL/97.5//:

CLOSING:/ 210003/GBP/202006/CALL/97.5/USD/E:

where USD is the delivery currency and E is the option style and CLOSING is the price set, 210003 is the contract, GBP is the contract currency, 202006 is the maturity year and month and 97.50 is the strike price.

Thus, it can be seen that the DX.MARKET.PRICE transaction ID string can be seen as a dynamic ID that is built to reflect the complexity of the underlying transaction.

In case of exotic options such as Double Barrier and KIKO, the market price ID is not sufficient to hold all the conditions. In such cases, a short key such as777777#1, 7777777#2 is used. #1 and #2 represent different barrier levels. This is shown in the following screenshot:

The details of exotic fields are stored in DX.POS.PRICE.XREF.LINK which gets updated only when multiple exotic events are found at trade level.


##### DX.CREATE.PRICE

When a trade is placed, the system automatically creates a record in DX.MARKET.PRICE . The record’s ID is a combination of security no, call/put, option type, strike, maturity date, and so on. If another trade takes place for the same combination, then system does not create a new record in DX.MARKET.PRICE as a record exists for the combination.

However, if a record in DX.MARKET.PRICE needs to be created without a transaction, the DX.CREATE.PRICE application can be used for this. While it is possible to create a record in DX.MARKET.PRICE manually, given the complex ID of the DX.MARKET.PRICE record, the DX.CREATE.PRICE provides an easier alternative to create a record in DX.MARKET.PRICE .

The user selects the Currnt/Closng/Whatif , Contract , Maturity Date and other details and sets the values for the Quote Ccy and Price fields.

On authorising the above record, the system automatically creates a record in DX.MARKET.PRICE in LIVE status. In this case, the Source Key field in DX.MARKET.PRICE holds the ID of DX.CREATE.PRICE .

> **⚠️ Note:** If a record already exists, then the price is updated in the existing record.


##### Price Setup for Different Contract Types

The following sections detail the specific instances of manual pricing as well as automatic pricing:

- Futures and Stock Prices
- Option Prices
- Automated Price Capture – Black Scholes and GK Methods
- FX OTC Options Price
- Mark to Market

The user enters the price into the contract record, with the optional update of the Interest Rate and Volatility of the contract to record the current market price for a future contract . Therefore, the closing price of 126.00 for June 2020, CBOT 5Y T-Note (110000) is shown in the following screenshot.

To record the current price for an option contract, the user must update the the strike price and call and put price for that option. So, a September 2020 Euro Bond (210003) CALL option with a strike price of 141.00 and premium of 17.25 is shown in the following screenshot.

There is also the opportunity for that strike price to enter the Delta , Gamma and Vega for the contract. There is the optional update of the Interest Rate and Volatility of the contract.

Option Prices with Underlying as Futures

Options on future is a type of derivative contract where the underlying is a derivative, Future. The underlying futures may be the same but have different maturities. The value in the Undlying Mat Date field in DX.CREATE.PRICE and DX.MARKET.PRICE holds the maturity date of the underlying futures contract.

The system validates the value in the Undlying Mat Date against the Maturity Type field in DX.CONTRACT.MASTER of the underlying future contract. The system raises an error in case of any discrepancy.

When the user creates a record with the value given in the Undlying Mat Date field, the system checks whether a record exists in DX.MARKET.PRICE for the underlying future with the given maturity date.

If the Undlying Mat Date field is left blank, then the system assumes that the option and the underlying future expiry are the same and checks for the record in DX.MARKET.PRICE record of the underlying future based on the option expiry date. In both the cases, if the record does not exist, the system raises a soft override as Underlying Market Price record does not exist.

Market Price with underlying maturity date

DX.CONTRACT.MASTER ID – 100100 (underlying futures DX.CONTRACT.MASTER ID -100101)

Maturity date of crude oil option contract – 20210720

Maturity date of crude oil futures contract – 20210920

Strike Price – USD 45

Option Type – Put

Option Style – American

The system checks for the futures (100101) DX.MARKET.PRICE record with maturity date 20210920. If the record does not exist, the system generates a soft override as Underlying market price record does not exist.

Market Price without underlying maturity date

DX.CONTRACT.MASTER ID – 100100 (underlying futures DX.CONTRACT.MASTER ID -100101)

Maturity date of crude oil option contract – 20210720

Strike Price – USD 45

Option Type – Put

Option Style – American

The system assumes that the option and future expiry are the same, and checks for the futures (100101) DX.MARKET.PRICE record with maturity date as 20210720. If the record does not exist, the system generates a soft override as Underlying Market Price record does not exist.

| Field | Obtained from |
|---|---|
| Fixed Rate | CURRENCY table |
| Time to Expiry | Automatically calculated from Maturity Date |
| Strike | DX.TRADE |

The Delivery Ccy and Option Style fields are defined in the DX.MARKET.PRICE application. The Delivery Ccy field defaults the delivery currency updated by DX.TRADE . It is a user-defined alpha currency code. The Option Style field holds the first character of option style value in DX.TRADE . The values are A for American, E for European or C for Caribbean options.

Prices are updated during the end-of-exchange (EOE) processing using the DX.CHECK.PRICES routine. This process should be run as an EOE preprocess to ensure that all prices are up-to-date as per the system requirement.

Prices can be updated online using the DX.RV.CHECK.PRICES application for verification. This basic application checks the current position across the DX system and requests a price for every open position that requires one. The normal validation rules apply.

After the application has opened, a price set field Currnt/Closng/Whatif ) should be selected. The three options are Online, End Of Exchange or Other. These are not linked to the DX.PRICE.SET application. Instead, it relates to the price setup in the DX.PARAMETER (SYSTEM record), which defines the price set to be used when the end-of-exchange process or online process is selected. If the user wants to define which price set they want to use, they should select Other and then enter an Alternative Price Set that links to the DX.PRICE.SET application.

After the request is completed, the system reports the status of the update. If all prices are updated, then the system updates the Error Text field as ‘All Prices have been updated’. If not, a warning message is displayed as ‘Errors have been encountered whilst checking prices’ and then all the prices or strike prices that have not been updated are listed. The record is committed to commit these updated prices to the database .

| Field | Description |
|---|---|
| Deal Reference | Holds the SY deal number or DX.TRADE ID |
| Valuation Ccy | Specifies the currency associated with the valuation amount |
| Valuation Amount | Specifies the valuation amount in the associated valuation currency |
| Valoren Number | For equity underlying structures, Valoren number is a unique number assigned to the structure (for example, by Telekurs), which is used subsequently for pricing data |
| Price | For equity underlying structures and options, if price per unit is available, then the valuation is derived from the price and quantity or lot size. |
| Trade Date | Date of the trade |
| B2B Reference | Back-to-back deal number |
| MTM Amount | Holds the MTM amount for DX component |


#### 📋 Tasks

Price Update provides knowledge about the market valuations for products, such as, derivatives and structured products.


##### Workflow

In Derivative Price Update, the user can perform the following activities:

| SCREENS | WORKFLOW |
|---|---|
|  | SY DX Valuation . |
| Valuation Details | Click the FIND button. Click the Update icon corresponding to a record. |
| Market Valuation Input | Enter values in the fields which needs to be updated. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

The DX.CREATE.PRICE application enables the user to input the pricing information for the derivatives master. Once the price details are created, system automatically creates a corresponding record in DX.MARKET.PRICE .

1. Dx Create Price .
2. Enter applicable values in the following fields: Price Set Contract Code Maturity Date Trade Ccy
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon.


#### 📊 Outputs

There are no Outputs available for Price Update feature.

---


### 3.12  DX Package Option


> **📇 Quick Reference Card**
> 
> **Purpose:** *Package options or options structures are structures which have more than one option component. They can be a combination of any of the following:*
> 
> **Key Fields:** *Acct With Bank Bic*, *Acct With Bank Customer*, *Acct With Bank Swift Addr*, *Bank to Bank Info*, *Ben Acct*, *Beneficiary Account No*, *Beneficiary Bank*, *Beneficiary Bic* ... +49 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Package options or options structures are structures which have more than one option component. They can be a combination of any of the following:

- Buy call
- Sell call
- Buy put
- Sell put

A typical example of a package option is a synthetic forward, which has two component options: A buy call and a sell put with the same underlying

- Strike price
- Maturity


#### ⚙️ Configuration

Though packaged options are part of the DX module, the core Structured Products (SY) tables have been used to manage the life cycle events.

The OPTSTRUCT record in SY.PRODUCT.DEFINITION application is setup for enabling the life cycle events of package options. Life cycle events run as SY events (like, trade capture, fixing of option structure and unwinding).

The Suppress Underlying field in the SY.PRODUCT.DEFINITION application decides how Temenos Transact processes the packaged option. If this field is set to Yes, then the system does not create the underlying component options. In this case, the underlying trades have to be interfaced from an upstream system and linked to the SY deal through the Sy Dx Reference field.

The Sy Dx Reference field in the derivative trades is the same as the Sy Dx Reference field of the structured trades. Temenos Transact does not validate these trades and the maturity processing of these trades has to be managed by the upstream system.

If the Suppress Underlying field is set to No, then the underlying trades can be either created manually or automatically (explained in the Working With Package Option section).


#### 🔧 Working With

Package options are also called as option structures and the terms are used interchangeably. Equity and Forex (FX) structures are supported in Temenos Transact . It is possible to book a trade with a single notional in reference or base currency. Also, the system can create all underlying option trades automatically or the user can link several existing option trades to form the structure.

The following are the various lifecycle events supported by the system:

- Trade capture
- Fixing of individual options within the structure
- Fixing of the structure as a whole
- Unwinding of the structure
- Reversal of the structure
- Valuation and mark to market (MTM)
- Final maturity

An option structure deal can be input by the user (or interfaced from an upstream system) in the DX.OPTSTRUCT application as shown below.

When the Suppress Underlying field in SY.PRODUCT.DEFINITION is set to NO, there are two ways to build an option structure.

The Build Structure field in the DX.OPTSTRUCT records can be set to Auto or Manual.

1. Auto – The user has to enter all the details of various options that are a part of the structure. This can be done by multi-valuing the Dx Trade Id fields and filling the details. Once the record is authorised, Temenos Transact automatically creates the options in DX.TRADE . All the trades have the same values in then Sy Dx Reference and Sy Transaction Id fields. The DX.TRADE ID is written back into the DX.OPTSTRUCT record in the Dx Trade Id field.
2. Manual –The option trades are created first either manually or through the interface. Subsequently, a DX.OPTSTRUCT record is opened and the user can enter various DX.TRADE IDs to be linked together as a structure. In this case, Temenos Transact does not create the underlying option trades. However, it updates the Sy Dx Reference and Sy Transaction Id in all the underlying trades. Once linked to a structure, amendments are not allowed on the underlying trades and are not shown separately in valuation enquiries.

If the Suppress Underlying field is set to Yes, the Build Structure field cannot be entered by the user. However, all the other fields from Dx Trade Id field to Deal Status field can be entered manually. Temenos Transact does not create the underlying trades.

For some option structures, the underlying options can be individually fixed at different times during the life of the structure. In some, it can be fixed as a whole once.

When a structure is built where individual component deals can be fixed on different dates, the Opt Exercise field in DX.OPTSTRUCT against that option multi-value has to be set to EXERCISE or EXPIRE. When the option fixing event runs, it exercises or expires the individual component deal. However, the structure remains active.

Cash settlement of individual options is not allowed.

Notional amount is not automatically adjusted. The user has to manually enter the new notional amount after an individual option is fixed. When a new notional amount is entered, the system reverses and re-books the notional entries (where dealer book is involved). Then, the customer limit is adjusted as per the new notional.

To fix the structure as a whole, the Fix Structure field is set to Yes. If cash settlement is required:

- Set the Cash Exercise field is set to Yes
- Enter the Cash Ccy and Cash Amount fields.

If individual deals need to be exercised, then set those deals as EXERCISE. The values in the Structure Fix Date and Opt Exercise Date fields should be the same in this case. If Opt Exercise field of an individual trade is left blank and Fix Structure field is set to Yes, then that individual trade expires.

When the structure fixing event runs, it raises the entries for the cash settlement if the Cash Exercise field is set to Yes Else, it exercises the individual components which are set as EXERCISE and the other components expires. The overall Deal Status field is marked as matured indicating that the DX.OPTSTRUCT application is closed.

If Suppress Underlying field is set to Yes, then Temenos Transact will not do any fixing.

It is possible to unwind the structure as a whole by setting the Unwind field to Yes in DX.OPTSTRUCT . Once this field is set, the unwind event is processed and the structure status is updated as Unwound. An unwind fee or penalty may be charged for early closure. All open underlying options expires.

Partial unwinding of the structure is not supported. If a single component needs to be removed from the structure, the user has to expire that individual option by setting the Opt Exercise field to Expire and then create a new deal outside the structure.

When Suppress Underlying field is set to Yes, the structure can be unwound but the child trades have to be expired manually.

Option structure deals can be reversed. Once DX.OPTSTRUCT deal is reversed, the underlying DX.TRADE records are reversed.

If the Suppress Underlying field is set to YES in SY.PRODUCT.DEFINITION , then the underlying options have to be either reversed manually or through the interface.

Once reversal is authorised, the DX.OPTSTRUCT deal cannot be re-instated.

If the Suppress Underlying field is set to No in SY.PRODUCT.DEFINITION , amendments are not permitted apart from the changes to Opt Exercise field. In such cases, amendments are effected through a reverse and re-book approach.

The entire structure is valued as a single deal. The valuation amount for the deal can be entered (or interfaced) into the SYDX.MARKET.VAL application. The record ID for this application is Sy Dx Reference _ . The Sy Dx Reference field uniquely identifies the deal. A valuation routine can also be attached to the SY.PRODUCT.DEFINITION record, which is triggered if the valuation is not interfaced or entered.

The Mtm Required field is set to Yes in SY.PRODUCT.DEFINITION , if a deal requires the MTM functionality. If this field is set to Yes, then an ability is provided in SY.PRODUCT.DEFINITION to attach a user defined routine to calculate the MTM value and populate the same in SYDX.MARKET.VAL . If the value is populated, the system raises the accounting entries for the same.

The underlying child DX.TRADE records does not update the positions. However, if dealer book is involved in the underlying trade, then DX.REP.POSITION record is created with the SY.TRANSACTION ID as part of the position key. This can be used for reporting (if required).

On the maturity date, the system marks the DX.OPTSTRUCT record as matured and the position ceases to exist. For those component option deals marked for exercise, the system exercises those derivative trades and rest of the options expires (provided Suppress Underlying field in SY.PRODUCT.DEFINTION is set to No). In case of cash settled structure, all the underlying options are expired and a cash payout entry is generated for the structure.

The system does not automatically create any back to back deals, either for the DX.OPTSTRUCT as a whole or for the underlying options.


##### Generating Payment Order fromDX.OPTSTRUCT

Banks can opt for the settlement of payments through PAYMENT.ORDER (PO) application. Under such cases the system:

- generates a record in PAYMENT.ORDER application by passing the necessary details.
- suppresses the generation of payment messages by the underlying application through old mechanism.

When the Po Application field in PWM.PO.PARAMETER is set to either DX.OPTSTRUCT or ALL, all payments made to the counterparty from DX.OPTSTRUCT application is made through PO, if:

- the counterparty’s account ( Cparty Cash Sett Acc or Cpa Prem Acc or Cpa Unwind Chg Acc ) is not a broker’s own cash or Nostro account.
- Pymt Msg Reqd field in DX.OPTSTRUCT is set to Yes
- credit has to be made to counterparty's account

If the counterparty has an own or Nostro account with the bank, then the same account is defaulted. If the counterparty does not have a Nostro account with the bank, and:

- If Temenos Payments is licensed, the system defaults the internal account based on the value in the Po Susp Categ field defined in PWM.PO.PARAMETER .

- If Temenos Payments is not licensed, the system determines the Nostro from NOSTRO.ACCOUNT and defaults the same in the counterparty account. If Nostro account is not found, then the system generates an error. The customer inputs an account manually and once the Nostro is determined, the system raises a payment order for crediting this Nostro account.

| Fields from DX.OPTSTRUCT or PWM.PO.PARAMETER | Fields in PAYMENT.ORDER | Conditional Mapping |
|---|---|---|
| T24 Bank BIC | Ordering Customer Bic | NA |
| Po Susp Categ in PWM.PO.PARAMETER | Debit Account | NA |
| Premium Currency or Unwind Chg Ccy or Cash Ccy | Debit Ccy | Depends on the event type. For example, for unwinding event system maps the Unwind Chg Ccy field |
| Value Date | Debit Value Date | NA |
| @ID ( DX.OPTSTRUCT Reference) | Ordering Reference | NA |
| Ben Acct | Beneficiary Account No | NA |
| BIC of Beneficiary Bank | Beneficiary Bic | NA |
| Beneficiary Bank | Beneficiary Customer | NA |
| Name of Beneficiary Bank | Beneficiary Name | System maps the Name from CUSTOMER application |
| BIC of Cpty No | Acct With Bank Bic | NA |
| Cpty No | Acct With Bank Customer | NA |
| Cpty Add | Acct With Bank Swift Addr | NA |
| Bic of Intr Bank | Intermed Bic | NA |
| Intr Bank | Intermed Bank Customer | NA |
| Intr Add | Intermed Swift Addr | NA |
| Premium Currency or Unwind Chg Ccy or Cash Ccy | Payment Currency | Depends on the event type. For example, for unwinding event system maps the Unwind Chg Ccy field |
| Cpa Prem Amt , Cash Amount , Cpa Unwind Chg Amt | Payment Amount | DX.OPTSTRUCT generates MT202 from various Structured Products (SY) events. Depending on whether the amount is premium, cash settlement or unwinding charges amount, the respective fields are mapped |
| Value Date | Required Credit Value Date | NA |
| NA | Bank to Bank Info | NA |
| NA | Internal Order Details | NA |
| Bank | Order Type | NA |
| Mapped from PWM.PO.PARAMETER if set | Order Initiation Type Payment Category Payment Method Payment Purpose | NA |
| Cpa Unwind Chg Acc or Cpa Prem Acc or Cparty Cash Sett Acc or Temenos Payments to determine | Credit Nostro Account | If the value Cpa Unwind Chg Acc or Cpa Prem Acc or Cparty Cash Sett Acc field is a Nostro account and does not belong to the counterparty, then the system defaults the value in the respective field. If the account is an internal category account formed using the value in the Po Susp Categ field, then the system does not populate any value in this field. Temenos Payments determine the Nostro account |
| Bic of Cpa Unwind Chg Acc or Cpa Prem Acc or Cparty Cash Sett Acc or Temenos Payments to determine | Receiver Bic | If it is a Nostro account does not belong to the counterparty, then system defaults the Bic of the Nostro account holder. If the account is an internal category account formed using the value in the Po Susp Categ field, then the system does not populate any value in this field. Temenos Payments determine the receiver of the message |

When the banks opt for the settlement of payments through PAYMENT.ORDER application, the system generates a record in PAYMENT.ORDER application by passing the necessary details. The system also records the PAYMENT.ORDER ID in the Po Reference field in SY.TRANSACTION application. Once the payments system processes the payment, the system generates an appropriate SWIFT (MT202) payment message.


#### 📋 Tasks

Related topics:

- Manage Packaged Option
- Trading Processes

Packaged options are option structures which has more than one option component. A typical example would be a synthetic forward, which has two component options - a Buy Call and a Sell Put with the same underlying, strike price and Maturity. The option components can be any combination of the following:

- Buy Call
- Sell Call
- Buy Put
- Sell Put


##### Workflow

This feature allows the user to perform the following tasks:

| SCREENS | WORKFLOW |
|---|---|
|  | Trades List . |
| List of Packaged Option Contracts | Click the View Underlying Option icon. The system opens the underlying trade in view mode. |
| Trade Details | Verify the trade details. |


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to order processing in the core banking system.


##### Enquiries and Reports

NA


##### SWIFT Messages

NA


##### Advices

The user can view the following advices:

A print advice is generated from a Packaged Option Trade which provides brief details of the trade.


##### Alerts

NA

---


### 3.13  Exotic Options


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Derivatives (DX) module supports the handling of exotic options, in addition to processing the plain vanilla options. Exotic options include more complex features than plain vanilla options and have additional rules governing their existence, valuation and processing.*
> 
> **Key Fields:** *Barrier Or Trigger*, *Co Pgm*, *Event Triggered*, *Exercise Expire*, *Exotic Event*, *Exotic Events Allowed*, *Exotic Fld Val*, *Exotic Type* ... +3 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The Derivatives (DX) module supports the handling of exotic options, in addition to processing the plain vanilla options. Exotic options include more complex features than plain vanilla options and have additional rules governing their existence, valuation and processing.

The following are the examples of exotic options handled by Temenos Transact :

- Kick-In or Knock-In A latent option contract that begins to function as a normal option (knocks in) only if a certain price level is reached before expiration.
- Knock-Out An option with a built-in mechanism, to expire worthless if a specified price level is exceeded.
- Knock-Out with Rebate A barrier option that offers a predetermined rebate, if the option is knocked out.
- Double Knock Out A double knock out option is a combination of two dependent knock out options. If one of the barriers is reached in a double knock out option, the other option is cancelled.
- No Touch An option which gives an investor an agreed payout, if the price of the underlying asset does not reach or surpass a predetermined price level.
- Double No Touch A type of exotic option that gives an investor an agreed payout, if the price of the underlying asset does not reach or surpass one of two pre-determined barrier levels. An investor using this type of option pays a premium to the broker and in return receives the right to select: Position of the barriers Time for expiration Payout to be received if the price fails to breach either of the barriers. With this type of option, the maximum possible loss is the cost of setting up the option.
- One Touch A type of exotic option that gives an investor a payout, once the price of the underlying asset reaches or surpasses a predetermined barrier. This option allows the investor to set the position of the barrier, the time for expiration and the payout to be received once the barrier is broken. The possible outcomes are: The barrier is breached and the trader collects the full payout, as agreed at the outset of the contract. The barrier is not breached and the trader loses the full premium paid to the broker.
- Instant One Touch An option that gives an investor a payout, once the price of the underlying asset reaches or surpasses a predetermined price level. Immediate payout is made.
- Double One Touch A type of exotic option that gives an investor an agreed payout, if the price of the underlying asset reaches or surpasses one of the two predetermined barrier levels. An investor using this type of option can determine the position of both barriers, the time for expiration and the payout to be received, if the price rises above one of the barriers. If either of the barrier levels is breached prior to expiration, the option is profitable and the buyer receives the payout. If any of the barrier levels is not breached prior to expiration, the option expires worthless and the trader loses all the premium paid to the broker for setting up the trade.
- European Digital This option can be exercised only at maturity date. Pays out fixed amount of asset or cash if the option is in the money at maturity date (regardless of the range in the money, the option is), otherwise worthless.
- European Double No Touch An option that gives an investor an agreed upon payout, if the price of the underlying asset does not reach or surpass one of the (two) predetermined price levels. This option can be exercised only at maturity date.
- European Double One Touch An option that gives the investor an agreed upon payout, if the price of the underlying asset reaches or surpasses one of the (two) predetermined price levels. This option can be exercised only at maturity date. Exotic events are not automatically triggered by the system and any actions that have been set up against an exotic option type are triggered when the Exotic Event field in DX.TRADE or DX.ORDER is set. Any further automation that is required has to be locally implemented. Therefore it is recommended to construct enquiries that display the exotic option deals that are eligible for exotic event trigger.


#### ⚙️ Configuration

The following applications are associated with the processing of exotic options:

- DX.OPTION.TYPE
- DX.EVENT.TYPE
- DX.USR.FLD.OPT
- DX.CONTRACT.MASTER


##### Exotic Deal Definition

The DX.OPTION.TYPE application defines the fields that appear on orders and trades associated with this option type and the routine that is executed during closeout when the Exotic Event field is set in DX.TRADE . For exotic options with multiple barriers or triggers, a separate record has to be set up for each barrier or option and all the required barriers or triggers can be linked at the transaction level.

The Barrier Or Trigger field defines whether the option is Barrier or Trigger type. A Barrier option kicks in or knocks out when a barrier is breached. For example, ‘Double Knock Out‘ is a barrier option. A Trigger option triggers a payment or non-payment when the price level is breached. For example, ‘Double No Touch’ is a Trigger option.

The Exercise Expire field defines the nature of the barrier or trigger. If this field is set to Exercise, the option knocks in (in case of the barrier option) or qualifies for payment (in case of the Trigger option). If this field is set to Expire, the option is knocked out (in case of the Barrier option) when the price level is breached, and a non-payment is signaled (in case of the Trigger option).


##### Event Definition

The DX.EVENT.TYPE application holds the details of all the processing or accounting events that can occur in the DX module. To define the event as an exotic option, the user has to create a record in this application by prefixing XO-, to the ID of the corresponding DX.OPTION.TYPE application. This application allows the user to define profit and loss (PL) categories, transactions and so on for each exotic event.


##### Exotic Deal Field Definition

The DX.USR.FLD.OPT application holds the re-usable user-defined fields for the DX.OPTION.TYPE application. An upper limit is used in many types of exotic options. The DX.USR.FLD.OPT application specifies the text, validation and field name for storing this upper limit. The DX.OPTION.TYPE application setup for each type of exotic option has to refer the DX.USR.FLD.OPT application. The user-defined fields appear in the DX.TRADE or DX.ORDER application.

If the Usr Fld Price field is set, the user-defined field(s) against which the field is set forms part of the positional and pricing record ID, for this type of options in Temenos Transact .

The fields in DX.OPTION.TYPE are updated based on the setup in DX.USR.FLD.OPT .

The setup for Single Barrier record is updated in the

record, as shown in the below screenshot.


##### DX.CONTRACT.MASTER

The user can set the allowed exotic events for the contract master by setting the Exotic Events Allowed field, while creating a DX.CONTRACT.MASTER record.


##### Routines for Processing Exotic Options

The black box routines downstream the processing of exotic options. These routines must be attached to the Co Pgm field in DX.OPTION.TYPE application. The routines are listed in the following table:

| Routines | Description |
|---|---|
| DX.XO.CREATE.FX | To create the underlying FX deal, user fields are not required |
| DX.XO.CREATE.SEC | To create the underlying SEC.TRADE , user fields are not required |
| DX.XO.CREATE.FX.KNOCKOUT | To create the underlying FX deal in case of knockout options, user fields are not required |
| DX.XO.CREATE.SEC.KNOCKOUT | To create the underlying SEC.TRADE in case of knockout options, user fields are not required |
| DX.XO.FWDCASHPAYOUT | To post accounting entry for settlement on closeout, the value or maturity date of option is adjusted for number of offset days, amount and currency user fields are required |
| DX.XO.INSTANT.CASHPAYOUT | To post accounting entry for settlement on closeout, the value closeout date is adjusted for number of offset days, amount and currency user fields are required |
| DX.XO.CREATE.FX.REBATE | To post accounting entry for the rebate amount in case of Knock-out options with rebate, amount and currency user fields are required |
| DX.XO.KNOCKOUT | To create underlying contracts regardless of the exotic types. If the Exotic Event flag is set and when the knock-out level is reached, the option is expired. |
| DX.XO.KNOCKIN | To create underlying contracts regardless of the exotic types. If the Exotic Event flag is set and when the knock-in level is reached, the option is valid. |


##### Exotic Options – Setup Examples

This section explains the setup of DX.OPTION.TYPE and DX.EVENT.TYPE applications for sample exotic option types. These applications utilise the user fields as explained in routines for processing the exotic options (as explained above).


##### Knock Out Option

The setup for DX.OPTION.TYPE and DX.EVENT.TYPE for the knock-out option is shown in the below screenshots.


##### Double Knock Out Option

In Double Knock Out option, Lower Knockout and Upper Knockout option type have to be setup. These two options should be attached in DX.TRADE .

The setup for

and

for the double knock out option is shown in the below screenshots.

The DX.EVENT.TYPE record for Lower and Upper Knockout can be created as explained in Knock Out example.


##### Double No Touch Option

In Double No Touch option, the user has to setup the following options:

- Lower No Touch
- Upper No Touch
- Cash Payout

The setup for

and

for the Double No Touch option is shown in the below screenshots.

The DX.EVENT.TYPE record for Upper and Lower No Touch options can be created as explained in the Knock Out example.


#### 🔧 Working With

This section explains the workflow of exotic options.


##### Knock Out

This section details the processing of Knock Out option.

A trade is created against the exotic option contract, specifying the strike and the knock out price in the Strike Price and Exotic Fld Val respectively. At this stage exotic event is not triggered, and hence the Event Triggered field is not set.

After the DX Trade is authorised, the below accounting entries are generated where the customer account is debited for the premium amount.

When the knock out level is reached, the field Event Triggered is set to Yes in DX.TRADE and the transaction is expired manually.

After the option is expired, the user has to run the BNK/DX.CO.EXP.MANUAL.SERVICE which creates the closeout records. One record each is created for the buyer and the seller.


##### Double Knock Out

This section details the processing of Double Knock Out option.

Before creating trade for the Double Knock out option, the Exotic Events Allowed field in DX.CONTRACT.MASTER should have the DX.OPTION.TYPE setup for Lower and Upper Knockout.

A trade is created against the exotic option contract, specifying the strike Price. The user has to multivalue the Exotic Type field to input the Lower and Upper Knockout price. At this stage exotic event is not triggered, and hence the Event Triggered field is not set.

After the trade is authorised, the below accounting entries are generated.

When any one of the knock out level (lower/higher) is reached, the Event Triggered field in the Exotic Type multivalue field is set to Yes in DX.TRADE and the transaction is expired manually. If the knockout level is not reached till the expiry of the contract, the contract can be exercised.

After the option is expired, the user has to run the BNK/DX.CO.EXP.MANUAL.SERVICE which creates the closeout records. One record each is created for the buyer and the seller.


##### Double No Touch

This section details the processing of Double No Touch option.

Before creating trade for the Double No Touch option, the Exotic Events Allowed field in DX.CONTRACT.MASTER should have the DX.OPTION.TYPE setup for Lower and Upper No Touch along with Cash Payout.

A trade is created against the exotic option contract, specifying the strike price. The user has to multivalue the Exotic Type field to input Lower No Touch price, Upper No Touch price, Cash Payout and Currency.

At this stage exotic event is not triggered, and hence the Event Triggered field is not set.

After the trade is authorised, the below accounting entries are generated.

When any one of the No Touch level (lower orhigher) is reached, the Event Triggered field in the Exotic Type multivalue is set to Yes in DX.TRADE and the transaction is expired manually. If the No Touch trigger is not reached, the contract can be exercised. The user has to set the Event Triggered field to Yes for the Cash Payout option.

After the option is exercised manually, two closeout records are created. One record is created for the buyer and the other record is created for the seller. For the Payout amount, the statement entry that is raised is shown in the below screenshot.


##### Replacement of Knock-In Option with a Vanilla Option

A bank might choose to replace a Knock In option with a plain vanilla option when the Knock In event occurs. This can be achieved by setting the Kickin Expire field to Yes. When the exotic event is triggered ( Exotic Event field is set to Yes) and DX.TRADE application is authorised, the trade is marked as closed. The user can then enter the vanilla option manually. The Kickin Expire field is available in the DX.PARAMETER , DX.CONTRACT.MASTER , and DX.TRADE applications. The trade defaults from the DX.CONTRACT.MASTER which is in turn defaulted from DX.PARAMETER . However, it is possible to amend the value at contract and trade level.


#### 📋 Tasks

Related topics:

- Trigger Exotic Options
- Trading Processes

Exotic options are a category of option contracts that differ from traditional options in their payment structures, expiration dates and strike prices.

The underlying asset or security can vary with exotic options allowing for more investment alternatives. Exotic options are hybrid securities that are often customisable to the needs of the investor.


##### Workflow

User can perform the following task, from this enquiry.

This enquiry displays the list of Exotic Options that are waiting to be triggered.

To trigger an Exotic Option, perform the following steps:

1. Trigger Exotic Option .
2. In the Exotic Events not yet Triggered screen, enter values in the search criteria and click the FIND button.
3. In the Exotic Events not yet Triggered screen, select the trades to be triggered by selecting the check box in the column before the Trans Reference column.
4. Enter the YES option in the box present in the Event Triggered? column corresponding to the selected Options.
5. Click the Apply the chosen operation to the selected row(s) icon.
6. Click the OK button in the message box that appears.


#### 📊 Outputs

There are no Outputs available for Exotic Options feature.

---


### 3.14  FX OTC Options


> **📇 Quick Reference Card**
> 
> **Purpose:** *Forex (FX) options are derivative options on underlying currency pairs, where the buyer can exchange one currency for another on a particular date, at a predetermined exchange rate. Generally, FX options are over-the-counter (OTC). These are hedging tools used by corporates as protection against adv...*
> 
> **Key Fields:** *Contract Class*, *Contract Type*, *Exchange*, *Tick Size*, *Tick Value*, *Type*, *Underlying*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Forex (FX) options are derivative options on underlying currency pairs, where the buyer can exchange one currency for another on a particular date, at a predetermined exchange rate. Generally, FX options are over-the-counter (OTC). These are hedging tools used by corporates as protection against adverse exchange rate movement.


#### ⚙️ Configuration

The FX OTC options are configured by creating a record in DX.CONTRACT.MASTER for all FX OTC options and specifying the currency pair at the trade level.

1. Creating a record in DX.CONTRACT.CLASS A separate record in DX.CONTRACT.CLASS is created. The Contract Type field is set to Fx-option.
2. Creating a record in DX.EXCHANGE.MASTER The Type field is set to Otc in the DX.EXCHANGE.MASTER application.
3. Creating a record in DX.CONTRACT.MASTER A generic contract master for FX OTC option is created as follows:


##### Setting up Delivery

A specific setup is not required to support delivery of MT305 and MT306 for FX OTC options. The standard delivery setup for derivatives must be followed. The following message types are supported.

- SWIFT MT305
- SWIFT MT306
- SWIFT MT601

MT305 is generated for confirmation of plain vanilla FX option contracts. MT306 is generated for confirmation of exotic FX options. MT601 is generated for confirmation of commodity option contract. Read the Outward Delivery section in Trade for more information.


#### 📋 Tasks

There are no Tasks available for FX OTC Options feature.

Currency options (also known as a forex option) give investors the right, but not the obligation, to buy or sell a particular currency at a pre-specific exchange rate before the option expires.

Currency options allow traders to hedge currency risk or to speculate on currency moves. Currency options consists of two main types, so-called vanilla options and over-the-counter SPOT options.


##### Workflow

This feature allows the user to perform the following tasks:

To capture a FX OTC options trade, perform the following steps:

1. Capture Derivatives Trade-Own Book .
2. Select the FX OTC Options from Choose DX Trade for Own Book.
3. Enter values in the following fields: Contract Trade Date Maturity Date Price/Premium Buy/Sell Customer Amount
4. Click the Validate icon to check for errors and overrides
5. Upon Successful validation, Click the Commit icon to submit the deal for authorisation


#### 📊 Outputs

There are no Outputs available for FX OTC Options feature.

---


### 3.15  Limits


> **📇 Quick Reference Card**
> 
> **Purpose:** *The inclusion of Derivatives (DX) within the Temenos Transact Limits module adds an extra element of risk control for customers trading in derivative instruments. Limits is applied within the derivatives operation to all products handled by the module.*
> 
> **Key Fields:** *Application*, *Contingent Value*, *Contract Class*, *Lim Amt Val Cont*, *Pri Limit Ref*, *Sec Limit Ref*, *Trade Type*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The inclusion of Derivatives (DX) within the Temenos Transact Limits module adds an extra element of risk control for customers trading in derivative instruments. Limits is applied within the derivatives operation to all products handled by the module.


#### ⚙️ Configuration

Limits allows fine-tuning of products into sub-products. Therefore, limits can be setup for different classes of contracts, for example, bonds, shares, currencies or commodities.

The limit reference conditions for DX.TRADE are defined using LIMIT.PARAMETER, for example, currency futures can set a different limit reference to currency options. Whenever a trade occurs for a relevant derivative product or portfolio, a limit check is done and generates an override if a limit is exceeded.

The amount used to update limit utilisation is set by choosing an option from Lim Amt Val Cont field in DX.PARAMETER . This field accepts the following values:

- Contingent Calculates a value based on the amount specified in Contingent Value field in DX.CONTRACT.MASTER Number of lots * Contingent value
- Value Calculates a value based on the following principles: Future - Number of lots * Internal price. Option buyer- Number of lots * Internal price. Option seller - Number of lots * Internal strike price.


#### 🔧 Working With

This topic helps the user to understand the functionality of limits.


##### Limits

The Limit module provides a control mechanism for the DX.TRADE and when entered, checks the availability of an authorised credit line for the customers involved with the trade. In real-time, the limit system is configured to monitor the availability and utilisation of customer limits.

Back end reports allow the monitoring of limits for commodities, countries, country group and currencies.

> **⚠️ Note:** LIMIT is a facility or credit line available to customer or group of customers, while LIMIT.REFERENCE is a type of limit, for example, futures and options limit.

DX.TRADE links a limit reference to each customer on both primary and secondary sides of the trade ( Pri Limit Ref and Sec Limit Ref fields respectively). Before any derivative trades are entered, all the proposed types of limit (global, product and sub-product) must be defined in LIMIT.REFERENCE .

The basic limit structure for bond futures linked under a more general product definition of futures are shown in the below screenshots.

The below screenshot shows a product LIMIT.REFERENCE :

The choice of limit reference selected for a customer is controlled from the criteria established in LIMIT.PARAMETER .

The below screenshot explains how different limits can be set for currency futures, bond futures and currency futures by testing values from Trade Type in DX.TRADE and Contract Class in DX.CONTRACT.MASTER .

There are two sides to a DX.TRADE , they are primary side and secondary side. Using one set of tests for both primary and secondary side customers can lead to problems where differences between sides need to be taken into account. This applies when processing tests on any fields prefixed with Pri or Sec in DX.TRADE .

The solution is to create another set of criteria in LIMIT.PARAMETER with DX.TRADE-SEC defined in the Application field. The application suffix –SEC, relates the tests solely to customers on the secondary side of the trade.

In the

application, if LIMIT is defined as 4554 and if

field is set to FUTURE. Then, in the DX.TRADE-SEC, the LIMIT is defined as 4555, if

field is set to FUTURE. In this case, for futures

, the limit is defaulted to 4554 for the customer on the primary side and to 4555 for a customer on the secondary side.

Once the limit is established for a particular customer, the system can use this information to ensure that the limit does not exceed. When the transaction limit exceeds, the user decides whether the excess can be allowed. When credit line is not setup, an override is raised (to create a system generated limit).

| Limit ID | Description | Limit | Utilisation | Remaining |
|---|---|---|---|---|
| 050027.0004552.01 | HP bond futures limit | 3M | - | - |

When more than one limit of the same type exists, the DX module defaults to the first limit (that is, the limit with serial number 01), unless the user specifically indicates it in the Pri Limit Ref and Sec Limit Ref fields provided in the DX.TRADE application.

When the required limit does not exist or is already fully utilised, the user can decide if a default limit must be generated. At the maturity of a DX transaction, the system provides an event notification to the LIMIT system, which resets the utilisation values.


#### 📋 Tasks

There are no Tasks available for Limits feature.


#### 📊 Outputs

There are no Outputs available for Limits feature.

---


### 3.16  MarginCalculation


> **📇 Quick Reference Card**
> 
> **Purpose:** *Margin is a critical concept for people trading in futures and derivatives in all asset classes. Futures margin is a deposit or an amount of capital one needs to post or deposit to control a Derivatives (DX) contract. The exchange determines and sets the futures margin rates. The margin is set based...*
> 
> **Key Fields:** *Gen Data Code*, *Init Margin Calc*, *Linked Trade*, *Suppress Vm Post*, *Vm Post Style*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Margin is a critical concept for people trading in futures and derivatives in all asset classes. Futures margin is a deposit or an amount of capital one needs to post or deposit to control a Derivatives (DX) contract. The exchange determines and sets the futures margin rates. The margin is set based on the risk of market volatility. When market volatility or price variance moves higher in a futures market, the margin rates rise. It is usually a small percentage of the contract value (for example, 3% or 5%). The margin is collected from the party with obligation to manage the risk incurred in the transaction.

There are two margins. The initial margin is collected at the time of entering into a futures contract. Variation or maintenance margin is collected whenever the value of a futures position falls. It is the amount required to bring the margin back to the initial margin percentage. Default risk is the risk that a lender takes on in the chance that a borrower will be unable to make the required payments on their debt obligation. The initial margin is used to cover the default risk incurred. Market risk is the possibility of an investor experiencing losses due to factors that affect the overall performance of the financial markets in which he or she is involved. The variation margin is used to cover the market risk incurred.

The DX contracts are revalued daily on a mark-to-market basis. The party, whose position has lost value, has to maintain the margin by paying cash. The variation margin is thus determined every day.


#### ⚙️ Configuration

For the initial margin setup and calculation, revaluation of Derivative (DX) contracts and variation margin setup and calculation and the configuration of multiple applications are mandatory as explained in this section.


##### DX.MARGIN.CALC

The margin requirements vary by exchange and it can change at the exchange’s discretion. Therefore, a black box approach is adopted and the API to calculate the margin can be defined by the user or can be specific to a particular region. By using the setup here, it is possible to set up margin APIs as required as part of Implementation. The DX.MARGIN.CALC application allows an entry or amendment of margin calculation routines into the DX module in Temenos Transact. The DX module is designed to use black boxes to return the information obtained in several different ways. The main applications call a shell routine and select the correct algorithm, routine or interface to return the required data for that margin calculation.

Margin calculations in DX also rely on this technique. The DX module calls a single grey box routine that determines the correct margin calculation by examining the exchange and the contract traded, if necessary. The DX.MARGIN.CALC application holds the descriptions of the calculations that may be used and points to PGM.FILE defining the actual routine to be called as part of the revaluation process.

The two default margining routines are STAND.IM and STAND.VM, which are the standard basic initial margin calculation and basic variation margin calculation routines. The Euronext-Amsterdam Exchange (AEX) and Options Clearing Corporation - Theoretical Inter-Market Margin System (OCC - TIMS) initial margin calculations are currently available, the number of margin calculation methods might increase in future.


##### DX.PARAMETER

The DX.PARAMETER application needs to be set up for variation margin postings. The revaluation P&L postings may be completely suppressed by setting the Suppress Vm Post field in DX.PARAMETER to Yes. The DX revaluation still calculates the figures for reporting purposes but they are not posted to the accounts. If P&L is calculated and posted, the Vm Post Style field allows the bank to select the mode of posting for the bank’s own book. The selections behave as follows:

| VM Posting Style | VM Posting Behaviour |
|---|---|
| Pl (default) | P&L calculated in contract currency Posted to P&L category in DX.EVENT.TYPE VM |
| Pllccy | P&L calculated in contract currency and converted to local currency Posted to P&L category in DX.EVENT.TYPE VM |
| Plrp | P&L calculated in contract currency Posted to P&L category in DX.EVENT.TYPE VM Sign reversed, posted to premium payment account (maintains replacement value) |
| Pllccyrp | P&L calculated in contract currency and converted to local currency Posted to P&L category in DX.EVENT.TYPE VM Sign reversed, posted to premium payment account in premium currency (maintains replacement value) |


##### DX.MARGIN.RATES

The DX module is used to calculate initial margin figures. The amount is calculated by black box initial margin routines controlled by the DX.MARGIN.CALC application. However, some of these routines require rates to be entered depending on the calculation performed. The DX.MARGIN.RATES application allows the entry of initial margin rates for various types of trades. These rates are used (as required) by various initial margin calculation routines. Further applications can be developed as required for specific initial margin calculation routines like Span.

The margin rates are entered on a contract and customer basis.

| Element | Sourced From |
|---|---|
| Contract class | A contract class from the DX.CONTRACT.CLASS application |
| Contract | A contract code from the DX.CONTRACT.MASTER application |
| Customer grouping | A group from the DX.GROUPING application |
| Customer | A customer from the DX.CUSTOMER application |


#### 🔧 Working With

This section explains the work flow of DX margin calculation-related applications in Temenos Transact .


##### Initial Margin Methods

The revaluation suite has a black box design, which enables easier development of new initial margin calculations, with a published standard and adds it to the DX module with minimum effort.

> **⚠️ Note:** To simplify the development of future margining algorithms, this method allows flexible local and customer-driven development of new routines without core development involvement.

For all margining algorithms used, the diagnostic information are created and stored for easy justification of the figures produced.

| Strategy | Description |
|---|---|
| SPREAD | Entered by buying and selling equal number of options of the same class on the same underlying security but with different strike prices or expiration dates. |
| STRADDLE | Neutral options strategy that involves simultaneously buying both a put option and a call option for the underlying security with the same strike price and the same expiration date |
| STRANGLE | Options strategy in which the investor holds a position in both a call and a put option with different strike prices, but with the same expiration date and underlying asset |
| TIME SPREAD | Options or futures spread established by simultaneously entering a long and short position on the same underlying asset at the same strike price but with different delivery months |

| Exchange | Abbreviation |
|---|---|
| AMEX | American Stock Exchange |
| CBOE | Chicago Board Options Exchange |
| NYSE | New York Stock Exchange |
| PHLX | Philadelphia Exchange |
| PSE | Pacific Exchange |


#### 📋 Tasks

There are no Tasks available for Margin Calculation feature.


#### 📊 Outputs

There are no Outputs available for Margin Calculation feature.

---


### 3.17  Market Ex Profit


> **📇 Quick Reference Card**
> 
> **Purpose:** *When a derivatives transaction involving FX conversion (trade currency being different from the customer’s account currency) is booked, the system applies an FX margin on the treasury rate for the currency conversion and generates market exchange PL entries accordingly. Market exchange profit is the...*
> 
> **Applications:** `ACCOUNT.CLASS`, `CURRENCY`, `DX.CONTRACT.MASTER`, `DX.PARAMETER`, `DX.PARMATER`, `FX.COMM.GROUP`, `FX.GEN.CONDITION`, `FX.GROUP.CONDITION`
> 
> **Key Fields:** *Closeout Sett Ccy*, *Co Comm Posting*, *Cus Fxmargin Txn*, *Delivery Currency*, *Mkt Exch Prt*, *Special Rate*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

When a derivatives transaction involving FX conversion (trade currency being different from the customer’s account currency) is booked, the system applies an FX margin on the treasury rate for the currency conversion and generates market exchange PL entries accordingly. Market exchange profit is the profit the bank makes in this implicit FX conversion. It is the difference between the bank-level treasury rate and customer rate (inclusive of the FX margin) applied to the transaction amount. Market exchange profit calculation and posting the exchange profit in local currency is based on the configuration of Mkt Exch Prt and Special Rate in DX.PARAMETER . Read the Configuring Market Exchange Profit section to understand more about these fields.

The bank offers different FX margins for different groups of customers. So, it is necessary to configure the margin based on customer groups. The system supports the configuration of margins based on customer groups. Customer group specific FX margin is applicable only for certain transactions that can be configured in DX.PARAMETER .


#### ⚙️ Configuration

The user must configure the following to calculate the market exchange profit of the derivatives transactions involving FX conversion. The user can also configure different FX margins for different customer groups.


##### Configuring Exchange Profit for Transactions with FX Conversion

This section explains the configurations required to calculate market exchange profit for the transactions involving FX conversion.

To calculate the market exchange profit for the transactions involving FX conversion (trade currency and customer’s account currency are different), the user must select Mkt Exch Prt (YES) and set Special Rate to Customer in DX.PARAMETER .

When the above configuration is set, the exchange rate in derivatives transactions is the treasury rate of the FX conversion along with applicable spread.

The below configuration must exist to define the PL category and to post the market exchange profit out of derivatives transaction. The event type MP (Market Exchange PL) entry is available to facilitate the posting of market exchange profit entries.

The below configuration must exist to post the FX suspense entries for the transactions involving FX conversion (trade currency different from the customer’s account currency).

- ACCOUNT.CLASS records SUSPDXFXCR and SUSPDXFXDR are available to post the FX suspense entries for debit and credit transactions when the user sets Mkt Exch Prt to Yes in DX.PARAMETER .
- The event type FS (FX Suspense entries) is available to post the FX suspense entries for the transactions involving FX conversion and when Mkt Exch Prt is set to Yes in DX.PARAMETER .


##### Configuring Market Exchange Profit with Customer Group Specific Margin

When the Mkt Exch Prt is set to Yes and Special Rate set to Customer in DX.PARAMETER , the system populates the treasury rate (Buy or Sell) with any spread defined in CURRENCY . This spread is common for all the customers.

The bank can offer different FX margin for different groups of customers. The following configuration helps the bank to setup different margin according to the customer or customer group.

The bank can apply distinct margins for customers or groups of customers to calculate the market exchange profit of the derivatives transaction.

- Group the customers using FX.GEN.CONDITION .
- Define FX margin percentage for a group of customers using FX.GROUP.CONDITION .
- To define a specific margin for derivatives transactions, the margin or FX.COMM.GROUP must be configured for the Derivatives (DX) deal type.

Read Configuring Automatic Defaulting of FX Margin for more information on the configuration of customer or customer group-based margin for DX.

If this configuration is not in place, the system calculates market exchange profit based on the customer spread defined in CURRENCY .

To define the transactions where customer group-based FX margin is applicable, the bank can parameterize the list of transactions in Cus Fxmargin Txn of DX.PARAMETER .

Cus Fxmargin Txn holds the below values.

- Buy - Transactions where the customer is the buyer of the option
- Sell - Transactions where the customer is the seller of the option
- Exercise - Exercise of long options
- Assign - Assignment of short options
- Expire - Option Expiry


##### Configuring Delivery Currency of Instrument as Closeout Settlement Currency

There are cash-settled options where the settlement can happen in the delivery currency as specified in the contract, which can be different from trade currency. The user must set Closeout Sett Ccy to Delivery.ccy in DX.PARMATER . If the user does not specify Delivery Currency in the contract definition ( DX.CONTRACT.MASTER ), the system considers the trade currency as the delivery currency and calculates the closeout cash settlement in the trade currency .


##### Configuring Posting of Commission in Closeout for Cash Settled Options

For cash-settled options, the system posts the commissions in closeout operation during the closeout authorisation online and the settlement amount posting is done during the execution of the XXX/DX.POST.CASH.PAYOUT service.

The user can configure the posting of commissions in closeout along with the settlement amount by setting Co Comm Posting as Service in DX.PARAMETER .

> **⚠️ Note:** This setup is mandatory when Mkt Exch Prt is set to Yes in DX.PARAMETER .


#### 📋 Tasks

There are no Tasks available for Market Exchange Profit feature.


#### 📊 Outputs

There are no Outputs available for Market Exchange Profit feature.


> **Related Applications:** `ACCOUNT.CLASS`, `CURRENCY`, `DX.CONTRACT.MASTER`, `DX.PARAMETER`, `DX.PARMATER`, `FX.COMM.GROUP`, `FX.GEN.CONDITION`, `FX.GROUP.CONDITION`

---


### 3.18  MiFID Transaction Reporting


> **📇 Quick Reference Card**
> 
> **Purpose:** *As part of the MIFID II regulation, the investment firms are obliged to report all the transactions which they execute for their customers not later than end of the next working day that is, T+1 day to the competent authorities.*
> 
> **Key Fields:** *Mifid Report Status*, *Post Update Rtn*, *Transaction Reporting*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

As part of the MIFID II regulation, the investment firms are obliged to report all the transactions which they execute for their customers not later than end of the next working day that is, T+1 day to the competent authorities.

All the transaction details which has to be reported must be captured at the trade level. Once the transaction is authorised, the details pertaining to Approved Reporting Mechanism (ARM) reporting is populated into a live database. Once the database is populated, the files can be extracted in any defined format using the Data Formatting Engine (DFE).


#### ⚙️ Configuration

The configuration for transaction reporting involves the parameter and database setup as explained below.


##### Setting up Parameter

The Transaction Reporting field in DX.PARAMETER is set to Yes, so that the transaction base is built and details to be reported are stored.


##### Holding Reportable Details in Database

The SCDX.ARM.MIFID.DATA record (transaction base) in the TX.TXN.BASE.PARMS application with all the reportable details of a transaction is shown below. If more fields must be included in the report, then additional fields can be added to this transaction base by amending the SCDX.ARM.MIFID.DATA record in TX.TXN.BASE.PARMS .

For each field added in the transaction base in the TX.TXN.BASE.PARMS application, the mapping must be provided to fetch the value related to the transaction. Mapping the fields in the transaction base from DX.TRADE record is shown below.


##### Data Formatting Engine

The Data Formatting Engine (DFE) must exist in order to generate the file from the database. Using DFE, the data can be extracted in any file formats such as csv, text file and so on. The records in DFE.PARAMETER and DFE.MAPPING must exist in order to extract the data from the database. The mapping and the field position in the report must be configured in DFE.MAPPING application.

The SCDX.ARM.UPD.DATE.TIME routine is available in core. The routine is attached in the Post Update Rtn field in DFE.MAPPING to ensure that the files created only in the database after the last extraction are selected and extracted.


#### 🔧 Working With

This section deals with the workflow of MiFID transaction reporting in DX module.


##### Transaction Reporting

The trades entered in the system are reported, if the configurations are already set.

The Mifid Report Status field is defaulted as Newt whenever a new transaction input in the system. This NEWT status shows that the transaction is a new transaction the MiFID transaction report.

The database updated with transaction details can be viewed using the MIFID II – Reporting Transactions (SCDX.ARM.MIFID.DATA) enquiry.


##### Generating the File Extract

Whenever the file (extracted excel sheet) must be generated, the user must trigger the BNK/OC.ONLINE.REPORTS service (or similar service). Once the service is triggered, the file extract is generated a shown below. Read SCDX.ARM.REPORT for more information on the data extracted from the SCDX.ARM.MIFID.DATA database into the csv sheet.


##### Modifying Reportable Transaction

Whenever a MiFID II reportable transaction is modified, a report with Mifid Report Status set to Canc is submitted. The new record with modified data is submitted as new report. Whenever the user wants to make any modifications, the user needs to change the Mifid Report Status field to Canc and submit the trade ( DX.TRADE ). The live database is updated with new record without any change in values except for the Mifid Report Status field changed as Canc and change in time stamp. This cancels the first report submitted prior to this with the same transaction reference.

> **⚠️ Note:** This section provides the instructions to modify the required details, if a bank user wants to change any values. This is an optional step.

The bank user needs to open the trade again and do the required modifications and should change the status in the Mifid Report Status field to Newt and submit again.

A new record is populated again in the live database with modified data and report status set as NEWT for the same transaction reference.

> **⚠️ Note:** For cancellations and deletions or reversals of transactions, the same procedure is followed. A cancellation report with Mifid Report Status set to Canc is submitted.


#### 📋 Tasks

There are no Tasks available for MiFID Transaction Reporting feature.


#### 📊 Outputs

The user can view the below list of enquiries related to MiFID Transaction Reporting in the core banking system.


##### Enquiries and Reports

This section allows the user to view the below enquiries and reports:

MIFID II Reporting

As part of the MIFID II regulation, the investment firms are obliged to report all the transactions which they execute for their clients not later than close of the next working day, that is, T+1 days to the competent authorities. This enquiry report captures all the relevant details like transaction reference, submission ID, trade booking date and report status pertaining to ARM reporting.

---


### 3.19  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Derivatives (DX) module allows trading in derivative contracts such as futures, options, and so on. The product supports trading, position keeping, valuation and closing out of both exchange-traded and Over the Counter (OTC) contracts, including exotics. The Derivatives product may be used by ba...*
> 
> **Key Fields:** *Average DPS*, *Average I Price*, *Average Price*, *B2b Active*, *B2b Co Ok*, *Barrier Trigger*, *Check Cust Funds*, *Class Category* ... +41 more
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- APIs
- Temenos Transact Services

The Derivatives (DX) module allows trading in derivative contracts such as futures, options, and so on. The product supports trading, position keeping, valuation and closing out of both exchange-traded and Over the Counter (OTC) contracts, including exotics. The Derivatives product may be used by banks trading on their own behalf, trading on behalf of their customers or offering their customers brokerage services.

Read Local Routine Insertion Points Guide for more information about insertion points and API for Derivatives.


##### Product Configuration

The parameters tables are the building blocks for designing the business process flow. It defaults common values to improve accuracy and efficiency.


##### Defining the Parameter

DX.PARAMETER is the main parameter control application for the DX module. It contains the single record named SYSTEM, which is read by other applications in DX and their behavior are controlled by the contents of this record.

The facilities that can be setup in DX.PARAMETER and other DX applications are detailed in the following sections.

| Cont Ulying Val | Description | Forex Derivatives | Other Derivatives |
|---|---|---|---|
| No | Only for futures and options with premium un-posted | Credit (CR) or Debit (DB) Central Reporting Facility (CRF) asset type Amount – cost of position or contingent value Currency – contract currency | CR or DB CRF asset type Amount – cost of position or contingent value Currency – contract currency |
| Yes | All trades | CR CRF asset type Amount – underlying receivable ccy amount Currency – receivable currency DB CRF asset type Amount – underlying payable ccy amount Currency – payable currency | CR and DB CRF asset type Amount – cost of position Currency – contract currency |

This functionality is activated at the DX.CONTRACT.MASTER level. The System Exercise and System Expiry fields are set to Yes, and a tolerance level is defined using the Exer Pri Mem , Exer Pri Non and Expiry Pri fields.

Whenever the manual settlement functionality is used, the system writes a record to the appropriate underlying application as mentioned below:

- DX.CO.MATURITY.INPUT
- DX.CO.ASSIGN.MANUAL
- DX.CO.EXERCISE.MANUAL
- DX.CO.EXPIRE.MANUAL
- DX.CO.MANUAL.INPUT

These applications may become huge and the user may not require it in the future. When the user does not want to retain these records, it can be set to clear automatically these applications during the COB process. The multi-value field Feed To Clear in the DX.PARAMETER application allows feed files to be selected and cleared along with their related unauthorised and history files when the COB runs. The DX.COB.CLEAR.FEEDS job in the DX.END.OF.DAY record in BATCH application runs the process daily to maintain these records.

The DX module has five methods of average price calculations:

- Normal
- Opening
- Purchase
- Unweighted
- None

These methods are defined at the contract level in the Average Price field in DX.CONTRACT.MASTER along with the number of decimal places required for average price. The Average Price and Average DPS fields in the DX.CONTRACT.MASTER application controls the average prices at the contract level. These fields are used for calculating the average price and to update Trade Price and Average I Price fields in DX.REP.POSITION . The five methods of average price calculations are explained as follows:

When the method is set to Normal, the average price is calculated using a standard average.

When the method is set to Opening, the average price is the average of buy prices of opening trades weighted by the number of lots traded.

Only the lots with the Tx Open Close field in DX.REP.POSITION set to Open and the Tx Buy Sell field in DX.REP.POSITION set to buy are considered.

When the method is set to Purchase, the average price is the average price trades weighted by the number of lots traded.

Only the lots where the Tx Buy Sell field in DX.REP.POSITION is buy are considered.

When the method is set to Unweighted, the average price is the average of buy prices of opening trades weighted by the number of lots traded.

Average price is not calculated.

> **⚠️ Note:** Positional updates to SC.POS.ASSET is set using the Sc Asset Upd field to Buy Sell Pos in DX.PARAMETER . This allows the description of the long and short positions separately. The Sc Asset Upd field can be set to Positional that enables to create the position cumulatively. If the field is set as Buy Sell Pos, the system segregates the long and short positions (all buys and sells are consolidated separately). This setup applies only for Exchange Traded Derivatives (ETD) contracts. OTC contracts are always be transactional. The module creates multiple records in DX.TRADE on each partial filling of DX.ORDER , at the average price of different levels at which the order is filled. The Create Trades field is set to No in the DX.ORDER until the final fill, then it is set to Yes. This creates one deal with the price set as the average of all the fills for the order. The Filled Lots , Filled Price , Filled Iprice and Create Trades fields are available in the DX.ORDER application. The Create Trade field in DX.ORDER defaults its value from DX.PARAMETER , which must be set to Yes for authorising the record in DX.ORDER . Every fill of a record in DX.ORDER creates a new multi-value set of the above-mentioned fields. The multi-value set averages to create the resultant DX.TRADE , while authorising the DX.ORDER .

Whenever a primary customer’s position is closed out, the corresponding opposite position of the secondary customer is also closed out automatically. The closeout does not require any separate authorisation by the user. Whenever an automatic secondary closeout cannot be performed for various reasons, there is a warning message to that effect. However, a secondary closeout does not result in a back-to-back closeout for the corresponding primary customer. For this purpose, the B2b Active field in DX.PARAMETER is used. The B2b Co Ok field in DX.CONTRACT.MASTER is used to activate the back-to-back closeout process.

| Applications | Description |
|---|---|
| DX.PARAMETER | The Special Rate field in DX.PARAMETER defines the class of customer for whom special rates are to be applied. When this field is left blank, it defaults the mid rates for calculations |
| DX.CUSTOMER | The best rate method is applied based on the customer type defined in the Special Rate field in DX.PARAMETER . For example, if the Special Rate in DX.PARAMETER field is set as dealer, then best rate is applied for transaction where the customer with Customer Type field in DX.CUSTOMER is set to Dealer |
| DX.TRADE | The rate at which conversion takes place is populated in Pri Prem Exc and Pri Comm Exc fields based on the definition in DX.PARAMETER . These fields can be overwritten for user-defined rates if the primary side of the DX.TRADE involves manual commission. |

This is an automated mechanism for equity options. When the underlying asset (shares or possible bonds) is used to cover one or more option contracts, that asset cannot be sold through the Securities (SC) module while the option contract is still active.

Margin requirements for written (sold) option trades can be reduced, if the counter party selling the option is in possession of the underlying asset. The blocking of securities position is done using Open Financial Source (OFS) to drive the SC.BLOCK.SEC.POS application. A valid value is entered in the Ofs Source field in DX.PARAMETER to activate this facility. The Pri Hedge Trade field is set to Covered in DX.TRADE to block a securities position on short covered call position and for protective put. If the requirement cannot be met, the deal is set as Uncovered in the Hedge Trade field. The user is informed about this in the transaction screen through an override on committing the transaction.

> **⚠️ Note:** At present, a deal position cannot be covered partially.

| Table Name | Description |
|---|---|
| DX.PARAMETER | The Cr Exp Calc Api field contains the API black box routine (DX.BB.CREDIT.EXPOSURE) created for calculating credit exposure |
| DX.CONTRACT.MASTER | The Int Rate Contract field is used to identify an interest rate derivative. When set to Yes, it is mandatory to enter a value in Life Underlying field |
| REVAL.ADDON.PERCEN | Based on the sub-asset type, add on percentage applicable for regulatory and credit reporting needs to be defined in the record in REVAL.ADDON . |

When the Check Cust Funds field is set Yes in DX.PARAMETER , the module calculates a best estimate initial margin figure for each transaction entered (order or trade). The value generated is used to block the customer funds until the next initial margin calculation is run (when the funds are physically removed from the customer’s account, in any case).

It also makes an unblocking posting forward dated to the notional maturity date of the deal. Defining a routine in Cost Calc Api field in DX.PARAMETER blocks the customer funds with respect to the premium cost of a transaction.

For all external customers, Revaluation P&L (variation margin) is posted to the account entered for that customer on DX.TRADE . For own book portfolios, unrealised - P&L calculated by the DX revaluation process are posted using the P&L category and transaction codes specified on the VM (Variation Margin) record in DX.EVENT.TYPE . Posting of revaluation, P&L for own book portfolios is controlled by the Margin Difference field in DX.PARAMETER .

- If this field is set to Yes, then when a new margin figure is calculated the difference between the previous margin amount and the new amount is posted.
- If this field is set to No, then the previous margin amount is reversed and the new margin amount is posted.

When the Vm Reversal Style field is set to New and the Margin Difference set to Yes, the reversal of variation margin for foreign currency contracts during closeouts are posted at the exchange rate at which it was booked. When Vm Reversal Style field is set to Old, it reverses the variation margin amount with prevailing exchange rate.

The variation margin are reversed on reversal of the DX.TRADE . Read Variation Margin Reversal for more information on how the reversal are handled.

The records in DX.TRADE are automatically generated to update the deal with respect to the order fill by filling orders through DX.ORDER . However, these trades can be created with their status set to INAU. This functionality is activated using the Stp Enabled Apps field in DX.PARAMETER .

The user designates the DX.ORDER application as a value in the field to activate the straight through processing of filled DX.ORDER records such that the corresponding DX.TRADE records are created with their status set to INAU. This activates the use of OFS, hence the TSA.SERVICE manager (TSM) should be running and the corresponding OFS.MESSAGE.SERVICE and OFS.RESPONSE.QUEUE is set to AUTO.

The DX.MONITOR.STP.PROCESS enquiry monitors the state of DX.ORDER and DX.CLOSEOUT generated OFS transaction messages, in case of any problem. It reports any transactions that require operator intervention, if a timeout period is specified, and it also reports on any transactions that were not handled within that time. The enquiry reports the following:

- DX.TRADE ID
- Error message
- Date and time of the generated transaction
- Length of time since the transaction is generated
- Timeout related issue

The Stp Timeout field in DX.PARAMETER represents the number of seconds that a transaction can await processing before being deemed to have timed out in the enquiry. This field is non-mandatory and when left blank, timeout checking is not done in the DX.MONITOR.STP.PROCESS enquiry.

The two possible options while posting Variation Margin entries are:

- Either the system is configured to post only the difference between current and previous date or
- Otherwise, the system reverses the full amount collected on the previous date and re-posts the current VM in full (Read Revaluation Profit and Loss (P&L) for more information).

When a DX.TRADE is reversed, only the last VM posting is reversed. This leaves the balance in the customer's account as correct on the date of reversal. However, the previous day’s balances since the start of the trade is not adjusted and this affects the interest charged on the account balances. When Vm Rev Type field is set to INDIVIDUAL in DX.PARAMETER , all VM entries are reversed with effective date. When this field is set to Yes, the system updates the DX.VARIATION.MARGIN.DETS table (a live table).

> **⚠️ Note:** The variation margin needs to be decided upfront by the bank. Hence it cannot be changed at the transaction level.

The ID of this table is . The system updates all the details (including the exchange rate, amount and the account to which VM was posted) every time a variation margin entry is posted for a trade. The system uses the values in this table and reverses each entry individually with the correct value date, when a trade is reversed. This ensures that the balance in the account is adjusted for each day.


##### Illustrating Model Parameters

The model parameters for the DX module are explained below:

| Field | Description |
|---|---|
| Margin Difference | Controls the posting of margin amount. |
| Price Order | Defines the order in which the price sets related fields should be searched to find the missing prices. |
| Price To Store and Price Days | Defines the period of storing the price sets related fields. Different period can be setup for each different price sets (CURRENT, CLOSING and WHATIF). |
| Suppress Underlying | Controls the creation of underlying during closeout process. |
| Fwd Post Eod | Posts the forward postings held in DX.FW.POSTINGS either in the start or end of business day by setting the Fwd Post Eod field accordingly. |
| Cost Calc Api and Cr Exp Calc Api | Facilitates configuring routines to calculate the net cost and credit exposure of the DX transaction. |
| B2b Active | Activates the back-to-back closeout processing when this field is set to Yes. |
| Closeout Version | Defines the version used for auto closeout by square-off order. |
| Cont Ulying Val | Allows the off-balance sheet postings made on entry of an own-book deal, to be based solely on the underlying value of the trade. |
| Sc Asset Upd | Defines the way of updating Asset Position details for Derivative trades. By Positional, the system updates the cumulative position of trades and update the price accordingly. By transactional, it updates the position for each trade separately. |
| Special Rate | Defines the class of customer, for whom special rates are to be applied. When this field is left blank, it defaults the mid rates for calculations. |
| Check Cust Funds | When set to Yes, system calculates the best estimated initial margin figure for each order or trade entered. |
| Vm Reversal Style | Controls the reversal of variation margin for foreign currency contracts. |
| Vm Rev Type | Manages whether all variation margin entries are reversed with effective date. |

The DX.CONTRACT.CLASS application allows to define a group of contracts such as equity options, equity futures and bond futures. Each contract class can be identified with a distinguished category code set in the Class Category field.

The DX.CONTRACT.TERMS application is more specific to basket options. The setup is done for each specific asset class like equity or currency.

| Field | Description |
|---|---|
| Barrier Trigger | Denotes whether the defined option is a barrier or trigger field type. |
| Exercise Expire | Depicts whether the exotic option is meant as a kick-in or kick-out event, with respect of being set to Exercise or Expire. |


##### Illustrating Model Products

Model products are not applicable for this module.

---


### 3.20  Non Stop Processing


> **📇 Quick Reference Card**
> 
> **Purpose:** *While financial transactions can happen any time round the clock, Non-Stop processing (NS) module helps in recording the transactions even during Close of Business (COB). This functionality allows Temenos Transact users to enter Derivatives (DX) transactions during the standard COB processing. This ...*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration


#### 📖 Introduction

While financial transactions can happen any time round the clock, Non-Stop processing (NS) module helps in recording the transactions even during Close of Business (COB). This functionality allows Temenos Transact users to enter Derivatives (DX) transactions during the standard COB processing. This feature explains the transactions that can take place Non-stop in DX module.


#### ⚙️ Configuration

The NS module should be licensed and available in the COMPANY record.

---


### 3.21  Order Grouping


> **📇 Quick Reference Card**
> 
> **Purpose:** *Orders of multiple customers with the same contract, maturity date, underlying maturity date, strike price, call or put option, and buy or sell combinations can be grouped and placed as a single order in the market in the parent-child structure.*
> 
> **Applications:** `CURRENCY`, `DX.CO.ASSIGN.AUTO`, `DX.CO.ASSIGN.MANUAL`, `DX.CO.EXERCISE.MANUAL`, `DX.CO.EXPIRE.MANUAL`, `DX.CUSTOMER`, `DX.ORDER`, `DX.PARAMETER` ... +4 more
> 
> **Key Fields:** *Ac Exc Trd*, *Authorise Child*, *Buy or Sell*, *Cancel Pend Order*, *Cancel Pend Orders*, *Co Lots*, *Contract*, *Contract Code* ... +28 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Orders of multiple customers with the same contract, maturity date, underlying maturity date, strike price, call or put option, and buy or sell combinations can be grouped and placed as a single order in the market in the parent-child structure.

Bulk orders with multiple customers can be categorised into customer and market sides to avoid any amendment or cancellation of one side impacting the other. The parent order is sent to the market, whereas the child order holds each customer’s order details.

- Parent Order – Represents the market side
- Child Order – Contains the customer order details

Banks can now group a number of DX client orders and place them as a single order in the market, thus segregating the market and customer side.


#### ⚙️ Configuration

To process parent-child bulk orders, set up the parameters by performing the following steps:

1. Create a synthetic counterparty and synthetic portfolio in the system and attach these to the Synthetic Cpty and Synthetic Port fields in the SC.STD.SEC.TRADE application. The synthetic customer defaults as the primary customer in the parent order, and the synthetic counterparty defaults as the secondary customer in the child order.
2. Set up records in DX.CUSTOMER for synthetic customer and synthetic counterparty to create and process parent-child orders in DX.
3. Attach the DX.ORDER,OFS version record in the Ord Ofs Version field in DX.PARAMETER to update the child orders during order execution, cancellation, or rejection of the parent order.


##### Calculating Secondary Fees at Cumulative Level

The Proc Sec Fees field in DX.PARAMETER is set to prorate the cumulative fees on the secondary customer side. The allowed values are:

- Yes – Indicates the fees on the secondary customer side are calculated at the cumulative level and then prorated among the trades. The consolidated and prorated fees are captured and stored in the DX.PARENT.CONSOLIDATE table.
- No – Indicates the secondary side fees are calculated at the individual trade level.


##### Defaulting Exchange Rates

The exchange rate will be the same for all the trades if the Fx Consolidate field is set and the currency pairs (account currency and trade currency) are the same. The exchange rate from the CURRENCY table will default for the first trade, and for the other trades, the exchange rate will default from the first trade if the currency pairs are the same.

If Fx Consolidate is set to:

- Acc Ccy - the same exchange rate is set for all trades if the currency pairs (account currency and trade currency) are the same.
- Ref Ccy - the same exchange rate is set for all trades if the currency pairs (reference currency and trade currency) are the same.
- Both - the same exchange rate is set for all trades if the currency pairs (account currency or trade currency and reference currency or trade currency) are the same.


#### 🔧 Working With

The below section explains the order grouping, trade, and post-trade life cycle for parent-child derivative orders.


##### Placing an Order

Following are the steps to place an order:

1. Create a parent order with the synthetic portfolio on the customer side and the actual broker on the market-side.
2. Set the Parent field in DX.ORDER to Yes, to denote the parent order.
3. Update the Parent Child Ref field in DX.ORDER with a unique reference, which links the parent and child orders. The secondary side of the parent order (actual broker) can also be given at the time of execution, like the existing process for single DX orders.
4. Create any number of child orders with the actual customer on the customer side and synthetic counterparty on the market side with Parent Child Ref as same as the one given in the parent order.
5. Ensure that the sum of the lots of the child orders should match the lots in the parent order. The below screenshots show an example of parent order with synthetic customer and child orders with synthetic broker.

Creating and grouping an order is either done in the front office or back office. When an order is entered, the system automatically creates a record in the DX.PARENT.LOG application. The ID of the application is a unique reference given in the Parent Child Ref field in DX.ORDER . When a subsequent order is entered with the same Parent Child Ref , the system checks the following details:

- Contract Code
- Maturity Date
- Option Type
- Option Style
- Strike Price
- Trade Direction (Buy/ Sell)
- Underlying maturity date

> **⚠️ Note:** If there is a mismatch, the system raises an error. For limit orders, if there is a mismatch in the Limit Type , Limit Price and Limit Date , the system raises a soft override.

The below screenshot is an example of the DX.PARENT.LOG application created for the parent-child reference Group1.

To authorise a bulk order, set the Authorise Child field to Yes in the parent order to allow bulk authorisation of the parent and child orders. After this field is set, the system automatically authorises the parent and child orders by running the XXX/DX.PARENT.CHILD.PROCESSING service.

> **⚠️ Note:** When the parent order is authorised without setting the Authorise Child as Yes, the user needs to manually authorise the child orders.


##### Executing an Order and Creating a Trade

Only the parent order is sent to the market for execution. When the parent order is transmitted to the market, the system updates the order status (Transmitted) in child orders using the XXX/DX.PARENT.CHILD.PROCESSING service. When the parent order is executed, the XXX/DX.PARENT.EXECUTION service prorates the fills to the child orders. The trades are generated directly between the customer and the broker, that is, the customer from the child order and the broker from the parent order are combined to form a single trade (parent and child trades are not created separately).

> **⚠️ Note:** When the parent order is filled, the system checks whether the sum of the child order lots is equal to the parent order lots. If there is a mismatch, the system displays a ‘Mismatch in Parent and Child Nominals’ error.

On execution, the system will be able to create individual trades for each execution. However, some markets mandate a single trade creation for all executions during the day. Both these scenarios are supported for grouped orders.

When the Day Trade field is set to Yes, the system consolidates multiple partial executions (within the exchange cut-off time) into a single trade.

> **⚠️ Note:** Refer the Consolidation of Partial Fills section to know more about the Day Trade functionality.

The following examples illustrate the execution of an order and creation of a trade:

| Orders | Order No | Order Lots | Filled Lots |
|---|---|---|---|
| Parent Order | DXORD2210900047 | 800 | 300 |
| Child Order 1 | DXORD2210900044 | 500 | = (300*500/800) =187.5 =187 (rounded down) |
| Child Order 2 | DXORD2210900045 | 100 | 37 |
| Child Order 3 | DXORD2210900046 | 200 | 76 |

Consider the following placed order:

- Child Order 1 – 100 lots
- Child Order 2 – 200 lots
- Child Order 3 – 500 lots
- Parent Order – 800 lots

The DX.ORDER.PARENT.REF enquiry in Parent Child Orders lists the orders grouped through the parent-child structure.

Following are the steps involved in grouping and transmitting the orders:

1. Transmit the parent order to the market.
2. Run the XXX/DX.PARENT.CHILD.PROCESSING service to automatically transmit the child orders.
3. The Day Trade field in DX.ORDER is set to Yes and the parent orders are filled for 200 lots at USD 10. The cut-off time is 14:00.
4. After the first fill of the parent order, run the XXX/DX.PARENT.EXECUTION service to prorate and fill the child orders. The system updates DX.PARENT.LOG as shown below.
5. The parent order is filled for 450 lots at USD 12.
6. After the second fill of the parent order, run the XXX/DX.PARENT.EXECUTION service to prorate and fill the child orders. The system updates DX.PARENT.LOG as shown below. When the set cut off time is reached, the XXX/DX.ORD.AGR.TRADE service creates a single trade.

The Proc Sec Fees field in DX.PARAMETER is set to Yes to allow the XXX/DX.ORD.AGR.TRADE service to calculate the cumulative fees on the secondary customer side and then prorate it (on the secondary side) among the trades created. For each execution, the fees is calculated at the parent level and prorated at the trade level.

Refer Calculating Secondary (Broker) Fees under Partial Execution with Day Trade set to No for more information on secondary fees.

> **⚠️ Note:** The process for calculating the primary (Customer) fees and defaulting exchange rates are the same as explained in the Calculating Primary (Customer) Fees and Defaulting Exchange Rates sections under Partial Execution with Day Trade set to No.

The parent order can be manually filled if there is no FIX market interface. Even in such cases, the system fills the child orders, that is, the parent order can be filled either by the FIX interface or manually by the user. The system treats both processes the same and fills the child orders automatically.

> **⚠️ Note:** In either case, child orders cannot be filled manually.

Child nominals will be rounded down if the prorate process results in fractional units and excess units are allocated to the first child, provided the open lots are greater or equal to the remaining lots.

When a parent order is about to expire, the system automatically expires the child orders, irrespective of the limit dates of the child orders. Child orders are excluded from the automatic expiry process as only the parent’s limit date is communicated to the market.

Following are the examples for limiting the expiry process:

Group 1

- Parent order – Sep 21, 2022
- Child 1 order – Sep 22, 2022
- Child 2 order – Sep 23, 2022

Group 2

- Parent order – Sep 21, 2022
- Child 1 order – Sep 20, 2022
- Child 2 order – Sep 21, 2022

> **⚠️ Note:** In both cases, on Sep 21, 2022, when the parent order expired, Child 1 and 2 automatically expired irrespective of the limit date in the child orders.

> **⚠️ Note:** DX.PARENT.LOG and DX.PARENT.CONSOLIDATE will be archived when the last trade in the parent-child group is archived.


##### Cancelling Parent and Child Orders

Orders can be cancelled by setting either:

- The Order Status field to Cancelled
- The Cancel Pend Orders field to Yes

When the Enterprise Wealth (EW) module is installed, the system allows cancellation of the parent order alone. When the Order Status of the parent order is set as ’Cancelled’, the system automatically updates the child order status as Cancelled. If there are any partially executed orders, then the system cancels the pending lots and a record in DX.TRADE is created for the filled lots.

When Cancel Pend Order of the parent order is set to Yes, the system cancels the pending lots and automatically updates the child order and parent order status to ‘Filled’.

> **⚠️ Note:** When the EW module is installed, the system does not allow direct cancellation of child orders.

If the EW module is not installed, the system allows the child orders to be cancelled. The user should amend the respective parent order manually.


##### Amending Parent and Child Orders

Orders can be amended by setting the Order Amend field to Yes and in the below scenarios:

The system does not allow the amendment of both parent and child orders except for the Limit Date , Limit Price , and Limit Type .

The system allows the amendment of both parent and child orders. The respective parent order must be amended manually to ensure that the order quantity matches.


##### Adding a new Trade Manually

Once the orders are filled and trades are created, you can create a new trade for the same parent-child reference by manually entering the trade details and Parent Child Ref . The system ensures that the trade created has the same details such as:

- Contract Code
- Maturity Date
- Option Type
- Option Style
- Strike Price
- Trade Direction (Buy/ Sell)
- Underlying maturity date

If there is a mismatch in any of the above details, the system raises an error. For such trades, the system calculates the fees at the individual trade level and updates the fees in the DX.PARENT.CONSOLIDATE table, provided the Proc Sec Fees field is set in DX.PARAMETER and update the Status field in the DX.PARENT.CONSOLIDATE table as MANU.

If the given Parent Child Ref value is unavailable in the system, an override such as ‘Parent reference does not exist’ is raised. When the override is accepted, trades are created, and for subsequent trades, the system does not raise an override and ensures the above criteria match.

If the given Parent Child Ref value is available in the system, but the respective execution sequence is unavailable, then the system raises the following error ‘Invalid Parent Reference’.


##### Reversing a Trade

After a trade is created, it can be reversed. When the trade is reversed, the system automatically updates the Status field of the respective trade in the DX.PARENT.CONSOLIDATE table as REVE.

When a manually created trade is reversed, the system automatically updates the Status field of the respective trade in the DX.PARENT.CONSOLIDATE table as MANU-REVE.

> **⚠️ Note:** In both the cases, a soft override ‘Reversal from parent child group’ is raised.


##### Post Trade Lifecycle Events

The Parent Child Ref field in DX.CO.EXERCISE.MANUAL , DX.CO.EXPIRE.MANUAL , DX.CO.ASSIGN.AUTO and DX.CO.ASSIGN.MANUAL holds a unique reference that links the group of trades created using the parent-child structure.

When the user selects Parent Child Ref , the system fetches all the DX transactions and populates the transaction ID in the Trans Id multi-value set, and populates the available open lots in the Co Lots field. The user can later modify the lots.

> **⚠️ Note:** The system defaults only those DX.TRANSACTION IDs with open lots not equal to zero.


#### 📋 Tasks

Orders of multiple customers having with the same contract, maturity date, underlying maturity date, strike price, call or put, and buy or sell combinations can be grouped and placed as one a single order in the market in the parent child structure.


##### Workflow

This section helps the user to perform the following tasks:

This screen allows the user to create DX Parent and Child order.

To create a parent-child order,

1. Order Capture .
2. In the Dx Order tab, enter values in the following fields: Contract Maturity Buy or Sell Customer No of Options
3. In Parent Child tab, enter values in the following field. Parent (only for Parent Order) Parent Child Ref (Should be same for both Parent and child order)
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon to submit the record.

| SCREENS | WORKFLOW |
|---|---|
|  | Parent Child Orders . |
| Parent Child Orders | Click View Open/Partial Orders to view the details of the Parent and Child orders for the respective Parent Child Ref . Click New Order to create new child order in the parent child group. Click the Amend/Cancel Parent Order icon to amend or cancel the parent order. Click the Fill Parent Order icon to execute the Parent Order of a group. |
| Derivatives Order | Enter a value in the respective field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | List of Parent Child Sell Options . |
| List of Parent Child Sell Options | Click List of Trades to view the list of Trade available for Parent Child Ref . Click the Assign Lots icon. |
| Derivatives Closeout | Enter a value in the Expire Lots field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | List of Parent Child Buy Options . |
| List of Parent Child Buy Options | Click List of Trades to view the list of Trade available for Parent Child Ref . Click the Exercise Lots icon. |
| Derivatives Order | Enter a value in the Expire Lots field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | List of Parent Child Buy/Sell Options . |
| List of Parent Child Buy/Sell Options | Click List of Trades to view the list of Trade available for Parent Child Ref . Click the Exercise Lots icon. |
| Derivatives Closeout | Enter a value in the Expire Lots field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

The user can view the below list of enquiries related to Order Grouping.


##### Enquiries and Reports

This section allows the user to view the below enquiries and reports:

Parent Child Orders .

This enquiry will display the following details.

- Contract
- Contract Types
- Maturity Date
- Buy/Sell
- Call/Put
- Strike Price
- Bulk Order Ref
- Bulk Order Status

The user to view the unmatched Parent and child orders, Cancellation, and Filled orders and Trades created for the grouped order using the drilldown.

View Canc/Filled Orders .

This enquiry will display the details of the Cancelled and Filled orders for the Parent Ref. Details displayed are as below.

- Parent Order ID
- Child Order ID
- Customer No
- Contract
- Maturity Date
- Call or Put
- Strike
- Buy or Sell
- Parent Child Ref
- Parent Order Status

The user to view Parent Order, Child Order, and Trade Details using the drilldown.

View Trade Details .

This enquiry will display the Consolidated trade details with following details

- Execution Reference
- Trade Reference
- Portfolio
- Portfolio Name
- Order Reference
- Traded Lots
- Status

The user to view the breakup of the secondary side fees for the respective trade using the drilldown.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA


> **Related Applications:** `CURRENCY`, `DX.CO.ASSIGN.AUTO`, `DX.CO.ASSIGN.MANUAL`, `DX.CO.EXERCISE.MANUAL`, `DX.CO.EXPIRE.MANUAL`, `DX.CUSTOMER`, `DX.ORDER`, `DX.PARAMETER`, `DX.PARENT.CONSOLIDATE`, `DX.PARENT.LOG`, `DX.TRADE`, `SC.STD.SEC.TRADE`

---


### 3.22  Order Processing


> **📇 Quick Reference Card**
> 
> **Purpose:** *Temenos Transact supports order capture for Exchange-Traded Derivatives (ETD). These orders can originate from either internal traders or external customers. The orders are entered either manually or by an interface from a front office system. Like any other market order, the order may be executed i...*
> 
> **Key Fields:** *Auto Authorise*, *Contract Class*, *Day Trade*, *Order Amend*, *Pri Original Lots*, *RM Status*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Temenos Transact supports order capture for Exchange-Traded Derivatives (ETD). These orders can originate from either internal traders or external customers. The orders are entered either manually or by an interface from a front office system. Like any other market order, the order may be executed in the market at which point it becomes a trade.


#### ⚙️ Configuration

The order processing feature has no specific configuration to be setup. The parameter applications are setup at the implementation stage.


#### 🔧 Working With

The below section explains order processing and its workflow.


##### Order Capture

The Derivatives (DX) module order entry allows the trader to check the validity of the order immediately and record the date or time when the order is given, entered and executed. The system checks the user's availability of funds or limits, therefore enabling a trader or credit officer to determine whether the order can be allowed. If as a result of the order being executed, any limits are breached, the system alerts the user. Similarly, if there are any constraints that are set for the particular customer or portfolio, the system warns the user.

An order can be amended, deleted or executed (manually or automatically) after it is entered. When it is executed fully or partially, the order becomes a trade. Therefore, one order can create multiple trades. In some cases, the order may not be executed or maybe only partially filled. At the end of exchange, all orders remaining unfilled are checked for their validity. All orders are reported and the expired orders are deleted.

The following screenshot displays a DX.ORDER entry for two customers party for a same deal, which is to be filled by a broker. An order is placed for a customer for 100 lots.

The order is filled by the user when the order is executed. The user enters the execution price only at the time of filling the order.

On filling the order, trade is created for the order.

The user can enter orders for multiple customers and fill an order partially in tranches.

The initial order has suffix as 0 in the record ID. When there are fills (that is, when the order is executed the order is filled), the suffix increases. The suffix is increased to 1 on filling the order as shown in the following screenshot. Then, the deal is partially filled (indicating partial execution) using DX.ORDER , with only 20 lots allotted to the second primary customer.

> **⚠️ Note:** Commissions can be in the 0 version and it gets defaulted in the subsequent versions. The execution price is updated on the secondary side of the order while filling the orders.

The following screenshots show a partially filled order.

In case of partially filled orders, the Lots field displays the number of lots open (yet to be filled) and the Pri Original Lots field displays the number of lots for which the order was placed.

When there are multiple customers and if there is a partial fill, then the partial fill is divided among the customers on a pro rata basis. In the above example, Customer 100291 had applied for 12 lots and customer 100271 has applied for 15 lots. On filling the order with 20 lots, Customer 100291 is filled with 9 lots and Customer 100271 is filled with 11 lots on a pro rata basis

As a result of partially filling the above order, a new instance of DX.TRADE is generated by the system in IHLD. When the Auto Authorise field in DX.ORDER is set to Yes, the trade is created in LIVE status. This is useful when orders are executed outside Temenos Transact and then fed into the system. Here, trades can be created in LIVE without user intervention, to maintain the sanctity of the record.

> **⚠️ Note:** The remaining lots can be filled later, either partially or fully.

In the above example, it is presumed that all filled orders are parameterised to create DX.TRADE records(s) with their status set to IHLD. However, it is possible to create these trades with a status of INAU.

| Day | Lots | Time | Price |
|---|---|---|---|
| Day 1 | 20 | 11:30 a.m. | 10 |
| Day 1 | 10 | 11:45 a.m. | 11 |
| Day 1 | 30 | 12:30 p.m. | 12.5 |
| Day 2 | 40 | 11:30 a.m. | 14 |


##### Order Workflow

The status of an order undergoes numerous changes during the life cycle of the order. These statuses are explained in the below table. Some of the statuses are user updated, while some are system updated. The Order Amend field in DX.ORDER needs to be set to Yes only then the user can amend the order status. The statuses Transmitted, Cancellation Request, Cancelled and Modification Request can be updated by the user. Other statuses are updated only by the system.

| Status | Description |
|---|---|
| Open | Initial capture of the order in the system |
| Transmitted | Order is placed with the exchange and acknowledged by the exchange |
| Partial | Order is partially filled, that is, partial execution |
| Filled | Order is fully executed |
| Cancellation Request | Request to cancel the pending lots placed with the market |
| Cancelled | Cancellation request accepted by the exchange |
| Modification Request | Modification of pending lots placed with the exchange |
| Expired | Order is expired |

The possible order workflows are shown below.

The difference between Modification Acknowledged and Modification Rejected is whether the change in order is reflected.

The initial order is for 10 lots and the user has modified it to 12 lots. If the modification is accepted, then the lots become 12, and if the modification is rejected, then the lots remain as 10. The status in both cases reverts to the previous status before the modification.

> **⚠️ Note:** The order status can be amended manually. The status is updated automatically for a fill order. The Order Amend field should be set to Yes, when there is a change in the order status. The order lots are updated manually for cancellation and modification. When the cancellation or modification request is rejected by the exchange, the status and order lots must be set to the earlier value. This is a manual update.


##### FX OTC Option Order

OTC derivatives do not require an order booking. In some cases, an order needs to be booked for some pre-trade checks. Only in those cases, an order is booked for OTC derivatives. When the Contract Class field in DX.CONTRACT.MASTER is set to FX OTC, a generic contract master is created to handle any currency pair. The Contract Class field is set as FX OTC in the DX.CONTRACT.CLASS application. When a generic FX OTC contract is created, the values in the Currency and Delivery Currency related fields in DX.CONTRACT.MASTER need not be mandatorily input.

> **⚠️ Note:** These fields can be blank.

The trade and delivery currencies can be given at the time of creating a DX.ORDER or DX.TRADE for such contracts. Further, the strike can also be quoted either in terms of trade or delivery currency.


#### 📋 Tasks

Related topics:

- Execute or Confirm Derivatives Order
- Execute Settlement (Derivatives)
- Process Upfront Payment Transactions
- Trading Processes

A derivative is a financial security with a value that is reliant upon or derived from an underlying asset or group of assets. The derivative itself is a contract between two or more parties and the derivative derives its price from the price fluctuations in the underlying asset.

Derivatives can either trade Over-the-Counter (OTC) or on an exchange. OTC traded derivatives, generally have a greater possibility of counterparty risk. Conversely, derivatives that are exchange traded are standardised and more heavily regulated.

Hedge funds are alternative investments using pooled funds that employ different strategies to earn active return or alpha, for their investors. Hedge funds are generally only accessible to accredited investors as they require less SEC regulations than other funds. Hedge funds face lesser regulations than mutual funds and other investment vehicles.


##### Workflow

This section allows the user to perform the following tasks:

This screen allows the user to enter an Exchange Traded Derivative (ETD) Future order.

1. Order Capture .
2. In the Dx Order tab, enter values in the following fields: Contract Maturity Buy or Sell Customer No of Options
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon to submit the record.

| SCREENS | WORKFLOW |
|---|---|
|  | Order Capture- OTC Order . |
| DX Order | Enter values in the following fields: Currency Pair Trade Date Maturity Date Customer Amount Buy/Sell Strike Price Premium Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record and accept the overrides, if any. |
|  | Work List . |
| Work List | Click the Action icon corresponding to a record. Click the Execute Activity icon corresponding to the running activity. |
| Treasury Transaction | Enter values in the following fields: Treasury Price Treasury Status Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record and accept the overrides, if any. |
|  | Dashboard . |
| Dashboard | Click the Action icon corresponding to a record. Click the Execute Activity icon against the running activity. Enter a value in the RM Status field. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record and accept the overrides, if any. |
|  | Worklist . |
| DX Order | In the Worklist tab, click the Action icon. Click the Execute Activity icon against the running activity. Enter values in the following fields: Treasury Price Treasury Status Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record and accept the overrides, if any. |
|  | Worklist . |
| DX Order | In the Worklist tab, click the Action icon . Click the Execute Activity icon against the running activity. Enter values in the fields that requires amendment. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record and accept the overrides, if any. Go back to Worklist tab and then click the Action icon. Click the Execute Activity icon against the running activity. Enter values in the fields that requires amendment. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record and accept the overrides, if any. |


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to order processing in the core banking system.


##### Enquiries and Reports

NA


##### SWIFT Messages

The user can view the below SWIFT messages:

MT305 is exchanged between the financial institutions which have agreed to a foreign currency option contract. This message confirms the details of a new contract between the parties and also any amendments to the previously agreed contracts.


##### Advices

NA


##### Alerts

NA

---


### 3.23  Reporting


> **📇 Quick Reference Card**
> 
> **Purpose:** *Reports provide important information for control and decision-making. This topic details the key applications for deriving reports and the various reports available in Derivatives (DX) module in Temenos Transact .*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Reports provide important information for control and decision-making. This topic details the key applications for deriving reports and the various reports available in Derivatives (DX) module in Temenos Transact .


#### ⚙️ Configuration

There is no configuration content for this feature.


#### 📋 Tasks

There are no Tasks available for Reporting feature.


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to report processing in the core banking system.


##### Enquiries and Reports

The section helps the user to view the below enquiries and reports:

Customer Derivatives Position

This enquiry displays the list of customer’s current derivatives position.

Option In/At the Money

This enquiry displays the list of all the option trades, which are in or out of money.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


### 3.24  Revaluation


> **📇 Quick Reference Card**
> 
> **Purpose:** *Revaluation is the process of evaluating the value of a contract based on the current market price. The Market price or premium of derivative contracts change daily based on market factors, volatility and so on. This, then results in an increase or decrease in the value of each contract.*
> 
> **Key Fields:** *All Customers*, *Base Currency*, *Contract*, *Contract Class*, *Countdown*, *Currency*, *Customer*, *Exchange* ... +14 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction


##### Introduction to Revaluation of Derivative Contracts

Revaluation is the process of evaluating the value of a contract based on the current market price. The Market price or premium of derivative contracts change daily based on market factors, volatility and so on. This, then results in an increase or decrease in the value of each contract.

Revaluation or Mark to market valuation of derivatives (DX) contracts is very critical to determine if the contract is

- In-the-money or out of the money, and
- to collect or pay variation margins to protect parties to the contract.

This feature explains how the revaluation of DX contracts is done in Temenos Transact . A part functionality of the DX module is to re-calculate the value of customer portfolios after the exchanges are closed. This can either be done as part of the overnight batch utility or as an on-line process. Revaluation is invoked in different modes and produces different events. The base of this module forms part of the end of exchange process and therefore is the part of the end of day processing for the module.

The revaluation module allows valuation, accounting and reporting of futures or stock and options held in the Temenos Transact DX system. Revaluation can be:

- End of day batch revaluation or processing
- Online ad hoc revaluations

In both cases, the revaluation calculation process is same. The differences are the products to be valued, the prices they are valued against and the resultant accounting treatment of the figures produced. So, along with the core revaluation process additional modules are written around it, which are called when required.


#### ⚙️ Configuration


##### Configuring Revaluation of Derivative Contracts

Revaluation is an everyday process. As a pre-requisite to revaluation:

1. Margin needs to be configured. Read Margin Calculation for more information on setup.
2. Market price needs to be updated. Read DX.MARKET.PRICE setup for more information.


#### 🔧 Working With


##### Working with Revaluation of Derivative Contracts

The core revaluation process consists of two major functions:

- Initial margin
- Variation margin allocation

Additional processes include retrieval or calculation of prices, retrieval of trades, posting of accounting entries and reporting of results. These additional processes are added into COB ( DX.COB.WORKFILE ) as required.

Read Margin Calculation for more information on configuring Initial Margin calculation and Variation Margin calculation.

The DX revaluation process is done at the customer or exchange level, whether it is online or COB. For each of these combinations, a record in the DX.COB.WORKFILE exists and any changes to this record can be traced in the DX.COB.WORKFILE.HISTORY table. If a combination no longer holds a position, it stays on the table until the Countdown (set as per the Hld Reval Days field in the DX.PARAMETER record) in the work file is negative. Later, it moves to HISTORY table.

> **⚠️ Note:** If position is not held during COB processing, the Countdown field is reduced by a value of 1.

The revaluation can be done in the following methods:

- Online by running the service
- During COB
- Ad-hoc

An online revaluation for one or more such combinations is requestedand done using a service. During COB, revaluation is done automatically as part of EOD processing. In order to process the revaluation, the TSA.SERVICE manager must be running. For Ad-hoc revaluation, no service is not needed. A what-if style revaluation is done by creating a record in the application DX.REVALUE application which is explained in detail below. An exchange is no longer blocked whilst the valuation processes online. Instead, the processing is only blocked if one of the users on a transaction is doing something that may impact the valuation for them on the exchange being processed.

Similarly, if a user chooses to enter a trade, close a position or run a corporate action when the COB is running, the system reports that service is running, and/or the following error displays. An ‘&’ valuation is being run by ‘&’ for customer ‘&’ on exchange ‘&’, please try again later.

The DX.REVALUE application allows the user to initiate an ad hoc what-if revaluation. The DX.REVALUE application allows the entry of the selection criteria defining the trades or positions to be revalued. Once the entries are input and authorised, the revaluation process passes the control to the Grey Box processes.

The selection criteria has four sections, ‘for whom’, ‘which trades’ and ‘parameters’.

- The ‘who’ consists of All Customers , Group , Customer and Portfolio . If all customers are to be revalued, the further ‘who’ selection fields are not available. For selection of individual customers, groups or portfolios, set All Customers fields to NO. Then, the user can identify a Group , Customer (s) or Portfolio (s) field. The user can choose only one field to populate.

- The ‘which trades’ allows the user to choose which kinds of trades from the customers are selected to revalue. Either all or a particular Currency , Exchange , Contract Class or Contract .

- The following fields allow the user to define which Price Set is to be used during revaluation. Re Calculate I M field specifies whether to calculate initial margin and is used to speed up the processing, if only variation margin figures are needed. It is impossible to calculate only initial margin without running the variation margin routines, as initial margin often requires variation margin figures to be present. Re Value Level field specifies at which level the top-level summary information in DX.REVALUE.SUMMARY and DX.REVALUE.EXCHANGE is to be stored. This allows the system to calculate the total margins for either a portfolio, a customer, or a customer group.

The user must start a revaluation by creating a new DX.REVALUE record and then define which customers or trades must be revalued. Revaluation records cannot be re-used. The processing begins after the record is authorised.

The DX.REVALUE.SUMMARY table details the total margin amounts for a customer, portfolio or group. This depends on the event, which triggered the revaluation:

- For a standard ad hoc revaluation, this ID can be the revaluation followed by a customer or portfolio or group depending on the revaluation level value set in the Re Value Level field in DX.REVALUE application.
- For an end of exchange, the ID is structured using a customer ID.

The below screenshot defines the margins for all contracts held by the customer 110018. This record details the figures held in the currencies in which they were calculated and the Base Currency for that customer held in Currency field in DX.CUSTOMER . It also holds the exchange rates used to convert these amounts. The details in the record is also a link down to the next level of reporting. The Exchange Keys holds all the keys of the DX.REVALUE.EXCHANGE records that combines to make the DX.REVALUE.SUMMARY table. Accounting entries are not posted for Adhoc Revaluation.

The DX.REVALUE.EXCHANGE record details the total margin amounts for a customer, portfolio or group in a currency on an exchange. This ID is dependent on the event that triggers the revaluation:

- For a standard ad hoc revaluation, this ID can be the revaluation followed by a customer, portfolio or group depending on the revaluation value set in the Re Value Level field in DX.REVALUE .

An example of key could be,

DXRVL9510900006*1*USD*10018

- DXRVL9510900006 - This is the key to the revaluation that created the record.
- 1 - This is the exchange code for which this record belongs.
- USD - This is the currency of the margins held at the exchange.
- 10018 - This is the customer/group or portfolio to which the margins relate.
- For an end of exchange, the ID is structured using a customer ID. For example,

DXEOE19088C100295E700*700*EUR*100295

The margins on USD contracts held on Exchange 2 for customer 110018 are detailed below. The exchange record details a number of group information:

- A link to the revaluation detail files, the IDs of the application names relating to those keys.
- The total margin figures for this currency and exchange.
- The combined commodities used and their constituent DX.CONTRACT.MASTER contracts.
- The margin totals on a contract-by-contract basis and a list of the transactions of that contract.

Revaluation Details

The lowest level files within the revaluation DX module’s revaluation suite are the revaluation detail files. For each record on the DX.MARGIN.CALC application, an application beginning with DX.REVAL.DET should exist. These files detail the data and calculations used to create the totals in the DX.EXCHANGE.MASTER application.

For a record in DX.MARGIN.CALC , there must be a live table called DX.REVAL.DET.SPAN existing in the system. Without this, revaluation cannot complete.

There are two standard margin routines provided with the DX module:

- STAND.VM
- STAND.IM

Their detailed application names are DX.REVAL.DET.STAND.VM and DX.REVAL.DET.STAND.IM .

- DX.REVAL.DET.CHREG.VM
- DX.REVAL.DET.STAND.IM
- DX.REVAL.DET.STAND.VM
- Exchange defined Initial margin requirements

A variation margin (revalue P&L) calculation black box CHREG.VM is released. This behaves in a similar way to the original STAND.VM calculation except that P&L is now calculated on options where the premium has already been paid, rather than the Unrealized Option Value calculated by STAND.VM .

CHREG.VM is available for selection in the Var Margin Calc field in DX.CONTRACT.MASTER .

This application holds the data required to calculate the standard initial margin on a group of transactions in the DX system. These transactions are grouped by exchange, by strategy, by contract and by customer or group or portfolio.

The information held is predominately held on a contract-by-contract basis, apart from the total initial and maintenance margins, and whether this exchange NETT’s its transaction against each other or is a gross(ing) exchange. The contract based information record shows the Initial Margin and Maintenance Margin values. For each contract, the rates used by the DX module to apply to this position, the type of rate, and data extracted from the DX.MARGIN.RATES record such as the Full , Spread , Straddle are all stored and can be seen in the record. The number of lots to be charged at a specific rate is also detailed. For example, 25 lots at 3000 per lot gives an initial margin figure of 75000.

This application holds the data required to calculate the standard variation margin on a transaction in the DX system. The constituent transactions are grouped in batches by exchange, by strategy, by contract and by customer or group or portfolio.

The information is held on a contract-by-contract basis with a total variation margin and unrealised option profit and loss. The figure for each transaction is displayed along with its transaction reference and a pointer to the version of transaction copied to the DX.REVAL.TRANSACTION application as a historical record. For each transaction, the record details the number of lots and the traded price and the current market price for that contract.

This is the controlling mechanism for the COB routines. This application provides an access point for starting online valuations as well as a work file for the COB to process the end of day valuations. This end of exchange processing is multi-threaded to the level of customer or exchange valuation.

Most of the processing work is passed to an online revaluation engine designed to process both online and during the COB. This means that both the COB and online valuations are multi-threaded by using services.

For example, a system with two exchanges and three customers results in six discrete threads being processed, one for each customer or exchange combination.

The possibility of one customer’s valuation failing and requiring a re-run of an entire exchange is removed, as only part of the customers position would have to be re-visited online. This increase in the number of threads is most noticeable on systems with large numbers of customers, thus has the effect of shortening the time taken for any COB processing.

A customer or exchange revaluation can be requested by changing the Status field of its corresponding record in the DX.COB.WORKFILE table either to ready or re-run. The user must first create the record and then ‘Verify’ to trigger the request for the TSA.SERVICE to launch the revaluation process. This updates the status to ‘Completed’ when successful. Accounting entries will be are generated, whenever an online revaluation is triggered.

Any errors or messages generated during the processing are updated on the Dialog section of the work file record, for example, ‘No Market Price Found for 100324*/15/EUR/200309/CALL/130.0*’. After rectifying error, the user can re-run the revaluation by requesting again.

Whenever, a revaluation is triggered for an own book portfolio through online or COB, accounting entries are generated.

If own book have a position in option contracts, revaluation triggers an accounting entry for the unrealised option value.

is posted for the change in option premium and the corresponding entry is posted in

.

This process does not require any request.

> **⚠️ Note:** If a new price change has occurred after an online revaluation, any customer or exchange affected needs to be manually requested again.

The COB verifies the status of the DX.COB.WORKFILE to decide which combination to revalue. In day-to-day processing, the status must only be ‘Completed’ or ‘Running’. Any combination of customer or exchange with the following status is revalued in the COB.

- New
- Ready
- Re-run
- Completed (with next run date less or equal to current bank day)

The Dialog section of the work file contains all messages, errors or warnings generated during the process.

This section is a technical guide which deals with new margining algorithms for use in the Temenos Transact DX product. It is not intended for non-technical staff. When creating new margining routines, it is important to note that the user cannot create a new record until the user has created a revaluation detail file. Read the Revaluation Details section (DX.REVAL.DET) for more information. The user should use the standard Temenos Transact LIVE table template (TEMPLATE.L).

In order to enter a record called SPAN.IM , an application called DX.REVAL.DET.SPAN.IM and a history table of the same application layout called DX.RV.DET.SPAN.IM.HIST is required. The existence of these files is vital for the correct function of the derivatives revaluation process, and without them the process cannot complete.

The revaluation suite has a black-box design, which allows new variation and initial margin calculations to be developed easily to a published standard and added to the DX module with the minimum of effort. This allows flexible local and client-driven development of new routines without core development involvement. The suite is designed to be triggered by user events.

- Ad hoc online 'What If…' revaluations triggered by DX.REVALUE .
- End of day, for exchanges traded today using the multi-threaded Temenos Transact end of day.

Once the trigger applications are authorised or verified, one of the grey box control process is called. These grey box processes act as the main controlling mechanism for the revaluation. The grey boxes ensure the integrity of data within the process and ensures that each black box receives the information it requires to complete the process successfully. The grey boxes also deal with errors generated by the black boxes and act accordingly.

DX.COB.REVALUE is the main control process for the revaluation. It processes the data required for the margin routine black boxes. Using the information, it has collected details about the Client, Trade, and so on. Then it chooses the relevant black box routine to process the information and return either an initial margin figure of variation margin figures for all the constituent transactions. After this has completed, it also produces diagnostic data for the revaluation. Read Revaluation Summary and Revaluation for Exchange for more information.


#### 📋 Tasks

Related topics:

- Initiate Direct Trade (Derivatives)
- Execute Settlement (Derivatives)
- Trading Processes

Revaluation is a calculated upward adjustment to a country's official exchange rate relative to a chosen baseline, such as, wage rates, price of gold or a foreign currency. In a fixed exchange rate regime, only a country's government, such as, its central bank can change the official value of the currency.

Currency revaluation can be triggered by a variety of events including changes in the interest rates between various countries and large-scale events that impact an economy.


##### Workflow

In Revaluation of Derivative Contracts, user can perform the following activities:

Using this option, the user can revalue either all portfolios of a customer or a specific portfolio or specific contracts and so on.

To perform Revaluation Criteria, follow the below steps:

1. Revaluation Criteria .
2. In the Revaluation Criteria tab, enter values in the following fields:
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon.

This enquiry displays the summarised results of revaluations that were run online.

To view the Initial Margin Report, perform the following steps:

1. Revaluation Summary .
2. In the Revaluation Summary screen, click the Initial Margin Details icon corresponding to a record.

To view the Futures Variation Margin Report, perform the following steps:

1. Revaluation Summary .
2. In the Revaluation Summary screen, click the Variation Margin Dets icon corresponding to a record.
3. In the Futures Variation Margins Report screen, click the Edit Trade icon.
4. In the Exchange Traded Instruments screen, enter values in the required fields.
5. Click the Validate icon to check for errors and overrides.
6. Click the Commit icon.
7. Accept the overrides, if any.


#### 📊 Outputs

There are no outputs available for Revaluation of Derivative Contracts.

---


### 3.25  Static setup


> **📇 Quick Reference Card**
> 
> **Purpose:** *This section describes the static setup of the Derivatives (DX) module.*
> 
> **Key Fields:** *Au Ct Class*, *Au Sett Type*, *Category*, *Chg Post Offset*, *Chg Post Time*, *Customer Type*, *Exch Member*, *Exch Session* ... +26 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

This section describes the static setup of the Derivatives (DX) module.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 🔧 Working With

The section helps the user to work with the static setup functionality.


##### Customers

The DX.CUSTOMER application supplements the main CUSTOMER application to record necessary information of individual customers for trading derivatives.

The Customer Type field indicates the type of customer such as Customer, Counterparty, Dealer, Broker and Exchange. All the customer types are similar and used for reporting purpose. However, the types Counterparty, Broker and Exchange have significant differences in the margining purpose.

The DX module is double sided for every position held by a customer or dealer, an equal and opposite position is held by broker, counterparty or exchange. Therefore, the system reverses all the positions held by brokers, counterparties and exchanges to ensure the accurate calculation and reconciliation of the margin results. The Brokers and Exchange customer types need not have portfolios for trading. The Customer and Dealer types represent the majority of the bank's customer and own-book trading, and must have SEC.ACC.MASTER portfolios set up before trading. The Exchange type can be selected only when the customer has a DX.EXCHANGE.MASTER record and holds the exchange’s positions during direct trading with the exchange.

The frequency of Batch and End of Exchange derivatives report generation can be set for the Customer.

The multi-value set of fields from Exchange to Marg Weighting allow the customer interaction with single or multiple exchanges defined in DX. This allows the bank to determine whether the customer is a member of an exchange and the trading type (speculative or hedge) of the customer in each exchange. The Exch Member field can be set to Trading, Clearing, Both or None. The Marg Weighting field enables the bank to apply a higher percentage weighting to any initial margin calculated on the relevant exchange(s) for customers considered to be at a greater trading risk.

The multi-value set of fields Au Ct Class defines the contract class closed by the settlement method defined in the Au Sett Type field.

The reporting and calculation of commission and margin for a customer depends on the DX.GROUPING record ID defined in the Group field.

> **⚠️ Note:** The fields from Margin Acc Ccy to Trading Status are display-only fields and are to be used in the future stages of the product development.

The value defined by the bank in the Reporting Ccy field is the customer’s default currency for DX revaluation. The currency defined in the first active SEC.ACC.MASTER portfolio (if one exists) is the default currency. If the default currency of the customer is not available, the system uses the company’s local currency.

The Renewal Frequency field defines the renewal frequency of a document. The value entered in this field must be a standard code defined in Temenos Transact . This DX.CUSTOMER record uses this value for information and reporting purposes.


##### Groups

The DX.GROUPING application allows grouping of DX customers for reporting and calculation of margin and commission. The group ID added to the DX.CUSTOMER record must be a valid ID defined in DX.GROUPING .

> **⚠️ Note:** The future developments of the Derivative product include the feature to perform revaluation at a hierarchical level. For example, if the system re-evaluates the customer group AA, then the groups such as AA.BB and AA.CC are also re-evaluated. The Margin Level field is reserved for future use, which is for defining an official margining level in a group hierarchy.


##### Exchanges

The DX.EXCHANGE.MASTER application defines the characteristics of the trading exchanges in which the customers are defined in the Temenos Transact DX module.

This application contains the types of information given below:

- Details of the exchange or market (such as, description and address).
- Default rules and methods for trading on the specific exchange (such as, margin calculations and premium posting times).
- Links to customers, portfolios, or accounts that represent the exchange in Temenos Transact for posting fees and other account entries.
- Basic details about the relationship between the exchange and other entities such as regulators (if any).

Each exchange is associated with a region, in this module for defining trading calendars in the HOLIDAY application.

The Exchange Type field defines if the exchange is Normal (real) or an OTC (pseudo-exchange) as defined by the bank for establishing OTC contracts in DX.CONTRACT.MASTER record.

The Prem Post Time and Chg Post Time fields indicate the time of trade or settlement (closeout) for option premiums and commission charges of all the contracts in the exchange, respectively. The Prem Post Offset and Chg Post Offset fields indicate the number of days the premium and commission charges posting are to be delayed, respectively.

The default margining parameters can be set for all contracts on the exchange. The Var Margin Calc and Init Margin Calc fields define the default variation and initial margin calculation records in DX.MARGIN.CALC . The margining algorithms on certain exchanges uses the values defined in the Nett Gross field.

The Trading Days field matches the trading days available in the HOLIDAY record associated with the region of the exchange. However, for some exchanges, there may be unusual trading day rules (for example, Monday to Thursday), which can be defined in this field. . The exchange’s specific trading opening and closing time are defined in the Trading Open and Trading Close fields. These are multi-value fields. The titles (if any) of the sessions available for trading certain products on the exchange day are defined in the Exch Session field.

The Max Months Fwd field constrains the setup of contracts on the exchange and sets the maximum number of months forward that any contract may be traded

The multi-value fields from Mutual Offset to Gen Data Limit define the exchange’s trading arrangements with other exchanges, electronic trading tools and any regulatory reporting schemes (if required).

> **⚠️ Note:** These fields are display-only and reserved for future use.

The Sett Allowed field defaults the behaviour of all contracts on the exchange with regard to automated settlements. If this field is set to No, the open positions in contracts in the exchange are not eligible for automatic settlement during the End of Exchange processing.

For a bank to record trades directly between the customers and exchange, both the bank and respective customers must be the members of the corresponding exchange. Such customers must exist in DX.CUSTOMER and the fields from Exchange Customer to House Customer must have inputs based on the local regulatory requirements.


##### Events

The DX.EVENT.TYPE application is critical for accounting in DX. Events that occur during the validity of a derivatives contract are selected from a predefined list and are related to the information used in accounting for the bank’s own-book portfolios. The module assigns one or more events to each activity performed on the system and recorded in the DX.TRANSACTION table.

For example, when a simple futures trade between a broker and bank’s own-book portfolio available in DX, for which the execution and clearing commission are due at the trade input time, two DX.TRANSACTION records are generated, one for each of the participants.

Each transaction is tested and has the following events assigned.

- Contract Initiation (CI) - Triggers contingent liability posting for own-book portfolio.
- Clearing Fee (FC) - Posts clearing fee calculated to broker account versus P&L category for own book portfolio.
- Execution Fee (FE) - Posts execution fee calculated to broker account versus P&L category for own book portfolio.

The following are the event types in DX.EVENT.TYPE record.

| Event code | Name | Description |
|---|---|---|
| CI | Contract inception | Initial entry of trade |
| CC | Contract cancellation | Cancellation of an authorised contract (contract reversal not part of an amendment and the contract completely cancelled) |
| CD | Contract deletion | Deletion of an unauthorised contract |
| CU | Contract unauth amendment | Amendment of an unauthorised contract |
| CR | Contract amendment reversal | Reversal of authorised trade details before amended details are entered |
| CA | Contract amendment | Amendment of authorised trade (new details) |
| CM | Contract maturity | Trade maturity |
| CS | Contract settlement | Settlement of trade (closeout) |
| PS | Partial Settlement | Partial settlement of lots |
| SR | Settlement reversal | Reversal of settlement (closeout) |
| PP | Premium posting | Posting of option premium |
| FC | Commission posting | Posting of Normal trading commission |
| FE | Execution fee posting | Posting of execution fees |
| FR | Regulatory fee posting | Posting of regulatory fees, if any |
| FL | Clearing fee posting | Posting of clearing fees |
| FM | Miscellaneous fee posting | Posting of any other miscellaneous charges entered manually |
| PO | Open position | Trade input forming opening position leg |
| PC | Close position | Trade input forming closing position leg |
| RP | Realised P&L | Realised P&L from the following: Maturity settlement Revaluation using nightly settlement conventions (for example, LIFFE settlement and reopen process) |
| UO | Unrealised option value | Unrealised option value generated by revaluation (not the variation margin as the product is not from mark-to-market or similar) |
| OA | Order amendment | Amendment of authorised order - new details |
| OC | Order cancellation | Cancellation of an authorised order |
| OD | Order deletion | Deletion of an unauthorised order |
| OF | Order fill | Fill or part-fill of an order, when the trade is created |
| OI | Order input | Input of an order and authorisation |
| OM | Option margin (Market Value) | Margin at market value |
| OX | Order abandon | Lots cancelled after a minimum of one partial fill |
| TT | Tax Posting | Posting of tax |
| IM | Initial Margin | Initial margin generated from revaluation |
| VM | Variation Margin | Variation margin (unrealised P&L) generated and posted by revaluation for futures |

For events referring to the posting of commissions and charges, the Use Ft Txn Code field is set to Category or Account. The transaction codes set on the FT.COMMISSION.TYPE or FT.CHARGE.TYPE records (if any) are used in the commission set up.

The category and transaction codes on the events are used for postings relating to own-book transactions only. The category code is mandatory for certain types of event.

The categories for the records PP (premium posting) and UO (unrealised option value) in DX.EVENT.TYPE can be assigned as:

- PP is the PL category (50000 - 59999) or an internal account category (10000 - 19999).
- UO is the PL category (50000 - 59999) or a product category (24000 - 24999).

If an internal account category is defined in the DX.EVENT.TYPE for PP, the system raises a STMT.ENTRY for the premium amount to the internal account category defined.

If a product category is mentioned in DX.EVENT.TYPE for UO, the system raises a RE.CONSOL.SPEC.ENTRY

If a PL category is defined in the DX.EVENT.TYPE for PP and UO, the system raises a code in the Category field.

If a PL category is assigned, the system books the premium amount in PL by raising appropriate

on entering a

for option contract. It raises debit or credit entry in

for long and short positions, respectively and corresponding entry is raised in

for broker’s account.

Similarly, the UO amount generated on account of revaluation (for own-book trades) are posted to PL by raising debit or credit entry (depending upon the position - long or short) in CATEG.ENTRY and corresponding entry is raised for internal account in STMT.ENTRY .

For example, if an own-book trade is entered for buying a call option by paying a premium of 15 for 10 lots (lot size is 1000), the system raises a debit entry in CATEG.ENTRY for the premium paid after authorising the trade.

The corresponding entry is generated in STMT.ENTRY to credit the broker account, along with the two wash through entries.

On revaluation of the position with a new price, for example 21 (in this case), the system calculates the UO amount and posts it to CATEG.ENTRY.

The corresponding debit entry is generated in STMT.ENTRY for an internal account.

Similarly, the UO amount generated on account of revaluation (for own-book trades) is posted to PL by raising debit or credit entry (depending upon the position - long or short) in CATEG.ENTRY and corresponding entry is raised for internal account in STMT.ENTRY .

The customer and broker transactions results are posted to the relevant accounts that are entered in DX.TRADE .

Based on the values in DX.EVENT.TYPE , the DX.REP.POS.ACTIVITY and DX.TXN.ACTIVITY reporting tables are generated to record the event activity.

The DX.REP.POS.ACTIVITY and DX.TXN.ACTIVITY tables track the events against positions and transactions, respectively. The Rep Updates field enables the event based reporting in the DX.PARAMETER application. The Tx Act Upd field determines if a DX.EVENT.TYPE reports to either of the DX.REP.POS.ACTIVITY and DX.TXN.ACTIVITY tables in the DX.EVENT.TYPE record.

| ID | Event Description | Requires CATEG.CODE | Generated By. |
|---|---|---|---|
| BV | Back valuation | NO | Back Valuation |
| BP | Broker profit | YES | Trade |
| FL | Clearing fee/CSN posting | YES | Trade |
| PC | Closed position | YES | Trade |
| FC | Commission posting | YES | Trade |
| CA | Contract amendment | YES | Trade |
| CR | Contract amendment (reversal) | YES | Trade |
| AS | Contract assignment | NO | Closeout |
| AR | Contract assignment (reversal) | NO | Closeout |
| CC | Contract cancellation | YES | Trade |
| EX | Contract exercise | NO | Closeout |
| ER | Contract exercise (reversal) | NO | Closeout |
| XP | Contract expiry | NO | Closeout |
| XR | Contract expiry (reversal) | NO | Closeout |
| CI | Contract inception | YES | Trade |
| CM | Contract maturity | YES | Trade |
| CS | Contract settlement | YES | Closeout |
| CP | Corporate action | NO | Corporate Actions |
| CX | Corporate action (reversal) | NO | Corporate Actions |
| FE | Execution fee/CSN posting | YES | Trade |
| CO | External transfer | NO | Tr/Pos Transfer |
| CT | Incoming transfer | NO | Tr/Pos Transfer |
| IM | Initial margin | YES | Re Valuation |
| II | Internal incoming transfer | NO | Tr/Pos Transfer |
| CN | Internal transfer | NO | Tr/Pos Transfer |
| FM | Misc fee posting | YES | Trade |
| PO | Open position | YES | Trade |
| OM | Option variation margin | YES | Re Valuation |
| OX | Order abandon | YES | Order |
| OA | Order amendment | YES | Order |
| OB | Order blocking | YES | Order |
| OC | Order cancellation (reversal) | YES | Order |
| OD | Order deletion | YES | Order |
| OF | Order fill | NO | Order |
| OI | Order input | YES | Order |
| OR | Order stage superseded | NO | Order |
| PP | Premium posting | YES | Trade |
| RP | Realised P and L | YES | Closeout |
| FR | Regulatory fee posting | YES | Trade |
| SR | Settlement reversal | YES | Closeout |
| TT | Tax posting | YES | Trade |
| CU | Unauth contract amendment | YES | Trade |
| CD | Unauth contract deletion | NO | Trade |
| UO | Unrealised option P and L | YES | Re Valuation |
| VM | Variation margin | YES | Re Valuation |


##### Local Currency Conversion of DX Contracts

This functionality enables the conversion of local currency commitments into Euro for cash settlements. Cash settlements warrant the effective realisation of any profit or loss for future contracts and payment of any outstanding option premium for option contracts. Read EURO User Guide for more information.


#### 📋 Tasks

An exchange rate is the value of one nation's currency versus the currency value of another nation or economic zone.

Most exchange rates are free-floating and will rise or fall based on supply and demand in the market.


##### Workflow

This section allows the user to perform the following tasks:

| SCREENS | WORKFLOW |
|---|---|
|  | Exchange Rates . |
| Latest Exchange Rates | Click the Update Rates icon corresponding to a record. |
| Buy/Sell Rates | Enter the values in the fields which are to be amended. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |


#### 📊 Outputs

There are no Outputs available for Static Setup feature.

---


### 3.26  Swaptions


> **📇 Quick Reference Card**
> 
> **Purpose:** *Swaption (an option in the underlying Swap), is one of the most traded Derivative (DX) contracts. Though options can be traded on a variety of swaps, the term Swaption typically refers to options on interest rate swaps. In a counterparty trading, swaption can either be a buyer or seller.*
> 
> **Key Fields:** *As Currency*, *As Fixed Rate*, *As Float Key*, *As Floating*, *As Int Frequency*, *As Principal*, *As Rr Frequency*, *Asset Ccy* ... +32 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Swaption (an option in the underlying Swap), is one of the most traded Derivative (DX) contracts. Though options can be traded on a variety of swaps, the term Swaption typically refers to options on interest rate swaps. In a counterparty trading, swaption can either be a buyer or seller.

The two types of Swaption contracts are:

The owner of swaption can enter a swap, in which the fixed leg is paid and floating leg is received.

The owner of swaption can enter a swap, in which the floating leg is paid and fixed leg is received.

The buyer and seller of swaption agree on the following points:

- Premium (price) of swaption
- Length of the option period
- Terms of the underlying swap including the notional amount
- The fixed rate (which equals the strike of the swaption)
- Frequency of observation for the floating leg of swap

In Temenos Transact , a swaption contract is captured through the Derivatives (DX) module. The DX module supports the following for swaptions:

- Trade capture
- Multiple premium processing on the specific value date
- Delivery confirmations

> **⚠️ Note:** Premium can be paid in multiple installments, initial premium is paid at the time of the trade and subsequent premiums are paid periodically.


#### ⚙️ Configuration

The DX.CONTRACT.CLASS and DX.CONTRACT.MASTER should be configured to use swaption in Temenos Transact DX module. The DX.CONTRACT.MASTER application holds the static instrument information while DX.CONTRACT.CLASS application is used to group similar contracts for reporting purposes.


##### DX.CONTRACT.CLASS

The swaption contract class is identified by setting the contract class Contract Type field to Swaption in the DX.CONTRACT.CLASS application.


##### DX.CONTRACT.MASTER

The DX.CONTRACT.MASTER application creates a contract for swaption transactions using the version DX.CONTRACT.MASTER , SWAPTION

The DX.CONTRACT.MASTER application holds the contract definitions of the contract types eligible for trading in the DX module. In the DX.CONTRACT.MASTER , SWAPTION version, the field Underlying is set to the value OTHER and Contract Class field has the value SWAPTION.

In the Swaption tab, the Delivery Method field defines the type of delivery made to the customer. This field is mandatory and must be set only as PHYSICAL. However, this field has no particular functionality but is used for querying purpose.

The system does not create a Swap automatically in a swaption contract. The physical Swap is created manually and the ID is updated in the DX.TRADE for future tracking.


#### 🔧 Working With

This section helps the user to work with the swaptions feature.


##### DX.TRADE

This application is used to capture swaption transactions. It supports multiple premium payments, trade capture and delivery confirmations. The relevant fields in this application are explained in the following table.

| Field | Description |
|---|---|
| Contract Code | Links the DX.CONTRACT.MASTER ID value, which in turn links the transaction level data with the relevant instrument static data |
| Call or Put | Confers upon the holder the right, but not obligation, to buy or sell the stock at a fixed price at a future date. Select CALL option for swaptions |
| Buy or Sell | Indicates whether the customer is buying or selling the transaction as determined by the bank |
| Sec Buy Sell | Indicates whether the broker is buying or selling the transaction as determined by the bank |
| Strike Price | Indicates the fixed rate at which the swaption contract is entered |
| Prem Percent | Indicates the initial premium denoted as a percentage of notional amount |
| Prem Pymt Amt | Indicates the premium amount value derived based on the values in Prem Percent and Asset Principal |
| Swap Delivery | Indicates whether the delivery method is CASH or PHYSICAL for swaption contracts |
| Swap Mat Date | Indicates the maturity date of swaption contract |
| Payment Type | Indicates whether the payment type is fixed. The values are: FIXED - The field As Fixed Rate should have values and cannot be left blank FLOATING - The field As Floating should have values and cannot be left blank This field is applicable only when the primary customer makes the pay amount an asset. |
| Receive Type | Indicates whether the receive type is fixed. The values are: FIXED - The field Lb Fixed Rate should have values and cannot be left blank FLOATING - The field Lb Floating should have values and cannot be left blank This field is applicable only when the primary customer makes the pay amount a liability. |

> **⚠️ Note:** The Payment Type and Receive Type fields for both asset and liability are also available in the Swap transaction application and hold the details of the underlying Swap.

| Column 1 | Column 2 |
|---|---|
| Asset Ccy | Indicates the asset currency which is defaulted from trade currency value for Swaption and Credit Default Swap contracts |
| As Fixed Rate | Indicates the fixed rate interest on asset side and must be same as Strike Price |
| Asset Principal | Indicates the asset principal in the asset currency which also denotes the notional amount for Swaption and Credit Default Swap contracts |
| As Float Key | Indicates the asset floating rate key. This field can have values only when Payment Type field is set as FLOATING. |
| As Int Frequency | Indicates the interest rate frequency |
| As Rr Frequency | Indicates the rate reset frequency. This field can have values only when Payment Type field is set as FLOATING. |
| Liab Ccy | Indicates the liability currency. This must be a valid currency from the currency table. |
| Liab Principal | Indicates the liability principal in liability currency |
| Lb Fixed Rate | Indicates the fixed rate interest on liability side and must be same as Strike Price |
| Lb Float Key | Indicates the liability floating rate key. This field can have values only when Receive Type field is set as FLOATING. |

| Column 1 | Column 2 |
|---|---|
| Prem Pay Percentage | Determines whether the premium amount is entered in trade currency or system defaults it by calculating from the percentage defined in the Prem Percent field. The values are: YES - Prem Pymt Amt is a display-only field and the system calculates and generates the amount NO - Prem Pymt Amt is updated manually |
| Prem Pymt Amt | Indicates the amount in the contract currency. When the fields Prem Pay Percentage and Prem Pymt Freq are input, this field is updated with the respective amount. |
| Prem Pymt Freq | Indicates the premium payment frequency. The values are 1- 5. |
| Prem Pymt Date | Defines the premium payment date for this period. When the fields Prem Pay Percentage and Prem Pymt Freq are input, this field is updated with the respective duration which is between trade date and maturity date. |

> **⚠️ Note:** When the first premium is paid, then the Prem Pymt Freq , Prem Pymt Date and Prem Pymt Amt fields are frozen for user input.

| Column 1 | Column 2 |
|---|---|
| Prem Pay Future | Determines if Prem Pay Future is enabled or not. The values are: YES - Premium amount in the Prem Pymt Amt field is updated in DX.PREMIUM.DETS and paid in SOD process on the premium date (date in the Prem Pymt Date field) NO - Premium amount is posted immediately with Prem Pymt Date as Value Date |

> **⚠️ Note:** Reversal of trade is not possible after the payment of the first premium.

The Exotics tab holds the transaction ID details of the contract. The Exotic Fld Val .1 field holds the unique transaction ID that is defaulted in DX.MARKET.PRICE .


##### DX.PREMIUM.DETS

When the Prem Pay Future field in DX.TRADE is set to YES, DX.PREMIUM.DETS LIVE table is created with premium payment details - premium pay date and amount. The DX.PREMIUM.DETS ID defaults the trade ID. This table tracks the future premium payments.

On trade closure, the Trade Status field is set as CLOSED.


##### DX.PREMIUM.DETS.HIST

The DX.PREMIUM.DETS.HIST LIVE table is a HISTORY table for DX.PREMIUM.DETS .

On reversal of trade, the records in DX.PREMIUM.DETS and DX.PREMIUM.DETS.HIST are deleted and updated, respectively. The reversal date must be before the first installment of premium payment in COB.

On archival of trade and transactions, the premium details from DX.PREMIUM.DETS are archived and updated in DX.PREMIUM.DETS.HIST .


##### DX.PREM.DETS.PAID

When premium amount is paid at Start of Day (SOD), the DX.PREM.DETS.PAID LIVE table is created with paid premium details. The DX.PREMIUM.DETS.PAID ID defaults the trade ID. This table tracks the past premium payments.

When a premium is posted, the paid premium details are deleted from DX.PREMIUM.DETS and updated in DX.PREM.DETS.PAID .

On trade closure the Trade Status field in DX.PREM.DETS.PAID table gets updated as CLOSED.


##### DX.PREM.DETS.PAID.HIST

The DX.PREM.DETS.PAID.HIST LIVE table is a HISTORY table for DX.PREM.DETS.PAID .

On archival of trade and transactions, the premium details from DX.PREM.DETS.PAID are archived and updated in DX.PREMIUM.DETS.PAID.HIST .


##### DX.TRANSACTION

The DX.TRANSACTION LIVE table is a log for trade, order and closeout. Whenever a premium payment is processed during the swaption life cycle, a new transaction is created.

The As Currency , As Principal , Lb Currency , and Lb Principal are display-only fields. These fields default the values from DX.TRADE application.


#### Accounting

Accounting entries are raised from DX.TRADE and periodical premium payments are posted at the Start of Day (SOD) process.


#### Limits

Not Applicable


#### 📋 Tasks

There are no Tasks available for Swaption feature.


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to swpations processing in the core banking system.


##### Enquiries and Reports

The section helps the user to view the below enquiries and reports:

Active Swaption Trades

This enquiry displays the list of active swaption trades available in the core banking system. The user have options to view the trades, floating rates and delivery messages related to the trade.

Net Swaption Position

This enquiry displays the net swaption positions of the swaption trades.

Swaptions In/Out of Money

This enquiry displays the list of swaption trades that are in and out of money.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


### 3.27  SWIFT MT306 for Exotic Options


> **📇 Quick Reference Card**
> 
> **Purpose:** *The SWIFT MT306 message is exchanged to confirm a foreign currency option contract. This message is used to confirm or notify the details of:*
> 
> **Applications:** `DX.OPTION.TYPE`, `DX.PARAMETER`, `DX.TRADE`, `DX.TRANSACTION`, `DX.USR.FLD.OPT`
> 
> **Key Fields:** *Barrier Evaluation*, *Barrier Level*, *Barrier Type*, *Barrier or Trigger*, *Cont Time Source*, *Description*, *Et Eq Modifier*, *Event Time Type* ... +13 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The SWIFT MT306 message is exchanged to confirm a foreign currency option contract. This message is used to confirm or notify the details of:

- A new contract between the parties.
- A barrier event, comprising of a knock-in or knock-out option, or hitting of a barrier level.


##### Contracts Supported by MT306

The MT306 message supports the following contracts:

- Vanilla options with Barrier conditions - An exotic option whose existence depends upon the underlying currencies exchange rate reaching pre-set barrier level. The option either springs into existence (known as knock-in) or, if the option already exists, it is extinguished (known as knock-out).
- Binary options - A class of options in which a fixed pay-out is made if a specified barrier condition is met or not met during the life of the option. They are also known as Digital options.
- Non-deliverable options – An option where the underlying currencies are not delivered, therefore they are cash-settled.


##### Option Styles

The MT306 message supports the following option styles:

- American: Exercised on any date prior to and including the expiration date as agreed by the parties to the trade.
- European: Exercised on the expiration date, at or before expiration time.


##### Barrier Events

The MT306 message supports the following types of barriers as per SWIFT Standards:

| Type of Barrier | Description |
|---|---|
| UIKI - Up and In Knock-in Event | An event that occurs when the spot rate is greater than or equal to the barrier level. If the event has occurred, the buyer of the option has the right to exercise it. If the event has not occurred, the option expires without any value. |
| DIKI - Down and In Knock-in | An event that occurs when the spot rate is less than or equal to the barrier level. If the event has occurred, the buyer of the option has the right to exercise it. If the event has not occurred, the option expires without any value. |
| UOKO - Up and Out Knock-out | An event that occurs when the spot rate is greater than or equal to the barrier level. If the event has occurred, the option expires without any value. If the event has not occurred, the buyer of the option shall have the right to exercise it. |
| DOKO - Down and Out Knock-out | An event that occurs when the spot rate is less than or equal to the barrier level. If the event has occurred, the option expires without any value. If the event has not occurred, the buyer of the option has the right to exercise it. |
| DKIN - Double Knock-in | An event that occurs when the spot rate is either, Greater than or equal to the upper barrier level, or Less than or equal to the lower barrier level If the event has occurred, the buyer of the option has the right to exercise it. If the event has not occurred, the option expires without any value. |
| DUKI - Dual Knock-in | An event that occurs when both the following events have happened: The spot rate is greater than or equal to the upper barrier level The spot rate is less than or equal to the lower barrier level If the event has occurred, the buyer of the option has the right to exercise it. If the event has not occurred, the option expires without any value. |
| DKOT - Double Knock-out | An event that occurs when the spot rate is either, Greater than or equal to the upper barrier level, or Less than or equal to the lower barrier level If the event has occurred, the option expires without any value. If the event has not occurred, the buyer of the option has the right to exercise it. |
| DUKO - Dual Knock-out | An event that occurs when both the following events have happened: The spot rate is greater than or equal to the upper barrier level The spot rate is less than or equal to the lower barrier level If the event has occurred, the option expires without any value. If the event has not occurred, the buyer of the option has the right to exercise it. |

> **⚠️ Note:** For the barrier events to occur, the barrier spot rate needs to breach (for example, be greater than or less than, as described in the relevant barrier event) the relevant barrier level(s) at any barrier event determination time, on any barrier event determination date. However, if the Barrier Event Equal Modifier is set as Y, then the words ‘or equal to’ can be removed from relevant barrier event definition.


##### System Processing

Barriers are defined in the DX.OPTION.TYPE application and can be linked to construct the required contract. For example, two barriers can be defined in DX.OPTION.TYPE , where one barrier represents the upper barrier and the other represents the lower barrier. Both barriers can be included in DX.TRADE to form a double or dual barrier contract.

Barriers are evaluated outside the system. When the barrier is breached, the corresponding Exotic Event field is set to ‘Yes’. Refer Exotic Options for more information on barriers.


#### ⚙️ Configuration

The following applications are associated with the configuration of SWIFT MT306 for exotic options:


##### Configuring SWIFT MT306 usingDX.OPTION.TYPE

The DX.OPTION.TYPE application defines the barriers and holds various attributes related to the barrier. Each barrier is defined as a separate record and can be linked in DX.TRADE . The DX.OPTION.TYPE application can be defined to use other exotic types and user-defined fields. The records in DX.OPTION.TYPE are not limited to barriers. To identify if a record pertains to a barrier, the Barrier or Trigger field should be set to ‘Barrier’. The DX.OPTION.TYPE application also holds various attributes related to the barrier. The barrier attributes are described below.

| Field | Description |
|---|---|
| Exercise Expire | Defines the nature of the barrier event. The allowed values are: Exercise - This option knocks in (in case of the vanilla option) or qualifies for cash payment (in case of the binary option) when the barrier is breached. Expire - This option is knocked out (in case of the vanilla option) or disqualifies for cash payment (in case of the binary option). |
| Upper or Lower | Defines whether the barrier is upper or lower. Based on the setup, the value from this field is mapped to the MT306 message. For the Upper Barrier Level TAG 37J is mapped and for the Lower Barrier Level TAG 37L is mapped. |
| Event Time Type | Specifies the period when a barrier is evaluated. This field accepts the following values: CONT – Indicates that barrier evaluation occurs on a continuous basis. DISC – Indicates that barrier evaluation occurs at a discrete point in time. The time must be mandatorily updated in DX.TRADE . This field is mapped to Tag 14M in Sequence F of the MT306 message. For Double or Dual Barrier contracts, the system must validate that either both barriers are ‘continuous’ or both are ‘discrete’. The system does not allow one barrier to be ‘continuous’ and the other to be ‘discrete’. Depending on the value defined in Event Time Type , additional information (tags) needs to be mapped in the MT306 message. CONT – Indicates either Tag 29O - Continuous Time Period or Tag 14N - Spot Market can be present, but not both. DISC – Indicates either 29J Barrier Event Determination Time or 14O Barrier Event Determination Time Source must be present, but not both. |

To capture the above information, a user-defined field (defined in the DX.USR.FLD.OPT application) should be attached to the barrier, and the Usr Fld Type field should be set as Time.Source. The field is defaulted in DX.TRADE and the field value is captured at transaction level. The below screenshot depicts a screenshot of a sample barrier.


###### List of Option Types

During event processing, SWIFT MT306 is generated and sent to the client. Messages are not generated for the cash payout event. The following list of option types are available in DX.OPTION.TYPE in the model bank.


###### CONT.KNOCKIN

A single barrier event with continuous barrier evaluation. This option knocks in or qualifies for payment when the barrier is breached.


###### DISC.KNOCKIN

A single barrier event with discrete barrier evaluation. This option knocks in or qualifies for payment when the barrier is breached.


###### CONT.KNOCKOUT

A single barrier event with continuous barrier evaluation. This option knocks out or disqualifies for payment when the barrier is breached.


###### DISC.KNOCKOUT

A single barrier event with discrete barrier evaluation. This option knocks out or disqualifies for payment when the barrier is breached.


###### CONT.UPPER.KNOCKIN

A double or dual barrier event with continuous barrier monitoring. This option includes both upper and lower barriers.

For the double barrier, either barrier can be breached for the option to knock in or qualify for payment. For the dual barrier, both barriers must be breached for the option to knock in or qualify for payment.


###### CONT.LOWER.KNOCKIN

A double or dual barrier event with continuous barrier monitoring. This option includes both upper and lower barriers.

For the double barrier, either barrier can be breached for the option to knock in or qualify for payment. For the dual barrier, both barriers must be breached for the option to knock in or qualify for payment.


###### DISC.UPPER.KNOCKIN

A double or dual barrier event with discrete barrier monitoring. This option includes both upper and lower barriers.

For the double barrier, either barrier can be breached for the option to knock in or qualify for payment. For the dual barrier, both barriers must be breached for the option to knock in or qualify for payment.


###### DISC.LOWER.KNOCKIN

A double or dual barrier event with discrete barrier monitoring. This option includes both upper and lower barriers.

For the double barrier, either barrier can be breached for the option to knock in or qualify for payment. For the dual barrier, both barriers must be breached for the option to knock in or qualify for payment.


###### CONT.UPPER.KNOCKOUT

A double or dual barrier event with continuous barrier monitoring. This option includes both upper and lower barriers.

For the double barrier, either barrier can be breached for the option to knock out or disqualify from payment. For the dual barrier, both barriers must be breached for the option to knock out or disqualify from payment.


###### CONT.LOWER.KNOCKOUT

A double or dual barrier event with continuous barrier monitoring. This option includes both upper and lower barriers.

For the double barrier, either barrier can be breached for the option to knock out or disqualify from payment. For the dual barrier, both barriers must be breached for the option to knock out or disqualify from payment.


###### DISC.UPPER.KNOCKOUT

A double or dual barrier event with discrete barrier monitoring. This option includes both upper and lower barriers.

For the double barrier, either barrier can be breached for the option to knock out or disqualify from payment. For the dual barrier, both barriers must be breached for the option to knock out or disqualify from payment.


###### DISC.LOWER.KNOCKOUT

A double or dual barrier event with discrete barrier monitoring. This option includes both upper and lower barriers.

For the double barrier, either barrier can be breached for the option to knock out or disqualify from payment. For the dual barrier, both barriers must be breached for the option to knock out or disqualify from payment.


###### CASH.PAYOUT

A cash payment event attached to the DX.TRADE application for binary options to process the cash payment. This is not a barrier, but captures the pay-out amount and pay-out currency for binary options.


##### Configuring SWIFT MT306 usingDX.CONTRACT.MASTER

The Option Type field is a multivalue set that holds the list of option types for the contract code. The user can either set the required option type or set the option type as ALL.


###### Generating Messages for Exotic Option Events

For the Exotic option contracts and events, the Fx Exot Dlv Msg field in DX.PARAMETER holds the value on which the message needs to be generated.

The allowed options are:

- All - Indicates the message is generated for contract confirmation and any barrier event occurrence.
- CONF - Indicates the message is generated for contract confirmation.
- BARRIER - Indicates the message is generated for any barrier event.


#### 🔧 Working With

SWIFT MT306 confirms or notifies the details of a foreign currency option contract whenever an exotic event is performed. The SWIFT MT306 is used for options that have exotic features. Temenos Transact generates the messages and sends it to the counterparty when it is a

- New contract
- During event processing – Knock In or Knock Out


##### Tag Mapping

The MT306 messages have many sequences. Click the below key sequences to view the related binary pay-out, barrier details, and non-deliverable options.

Sequence E - Binary Pay-out Amount


##### Linking Option Types inDX.TRADE

Based on the option types available, this section describes the linking of option types in DX.TRADE .

> **⚠️ Note:** All the option types are configured with the Et Eq Modifier field set as Y in DX.OPTION.TYPE .

The table below lists the knock in - vanilla option with a single knock in barrier, that is knocked in when the barrier is breached.

| Field | Value |
|---|---|
| Barrier Type | UIKI, DIKI |
| Option Variant | VANI |
| Barrier Evaluation | CONT, DISC |
| Exotic Type.1 | CONT.KNOCKIN, DISC.KNOCKIN |

The table below lists the vanilla option with a single knock out barrier, that is knocked out when the barrier is breached.

| Field | Value |
|---|---|
| Barrier Type | UOKO, DOKO |
| Option Variant | VANI |
| Barrier Evaluation | CONT, DISC |
| Exotic Type.1 | CONT.KNOCKOUT, DISC.KNOCKOUT |

The table below lists the binary option with a single barrier that qualifies for payment when the barrier is breached.

| Field | Value |
|---|---|
| Barrier Type | UIKI, DIKI |
| Option Variant | BINA |
| Barrier Evaluation | CONT, DISC |
| Exotic Type.1 | CONT.KNOCKIN, DISC.KNOCKIN |
| Exotic Type.2 | CASH.PAYOUT |

The table below lists the binary option with a single barrier that is disqualified from payment when the barrier is breached.

| Field | Value |
|---|---|
| Barrier Type | UOKO, DOKO |
| Option Variant | BINA |
| Barrier Evaluation | CONT, DISC |
| Exotic Type.1 | CONT.KNOCKOUT, DISC.KNOCKOUT |
| Exotic Type.2 | CASH.PAYOUT |

> **⚠️ Note:** In an MT306 message, for all double and dual barriers, the value in the upper barrier level is mapped to the TAG 37J barrier level and value in the lower barrier level is mapped to the TAG 37L lower barrier level.

The table below lists the vanilla option with a double knock in barrier that is knocked in when either barrier is breached.

| Field | Value |
|---|---|
| Barrier Type | DKIN |
| Option Variant | VANI |
| Barrier Evaluation | CONT, DISC |
| Exotic Type.1 | CONT.LOWER.KNOCKIN, DISC.LOWER.KNOCKIN |
| Exotic Type.2 | CONT.UPPER.KNOCKIN, DISC.UPPER.KNOCKIN |

The table below lists the vanilla option with a double knock out barrier that is knocked out if either barrier is breached.

| Field | Value |
|---|---|
| Barrier Type | DKOT |
| Option Variant | VANI |
| Barrier Evaluation | CONT, DISC |
| Exotic Type.1 | CONT.LOWER.KNOCKOUT, DISC.LOWER.KNOCKOUT |
| Exotic Type.2 | CONT.UPPER.KNOCKOUT, DISC.UPPER.KNOCKOUT |

The table below lists the vanilla option with a dual knock in barrier that is knocked in when both barriers are breached.

| Field | Value |
|---|---|
| Barrier Type | DUKI |
| Option Variant | VANI |
| Barrier Evaluation | CONT, DISC |
| Exotic Type.1 | CONT.LOWER.KNOCKIN, DISC.LOWER.KNOCKIN |
| Exotic Type.2 | CONT.UPPER.KNOCKIN, DISC.UPPER.KNOCKIN |

The table below lists the vanilla option with a dual barrier that is knocked out when both barrier is breached.

| Field | Value |
|---|---|
| Barrier Type | DUKO |
| Option Variant | VANI |
| Barrier Evaluation | CONT, DISC |
| Exotic Type.1 | CONT.LOWER.KNOCKOUT, DISC.LOWER.KNOCKOUT |
| Exotic Type.2 | CONT.UPPER.KNOCKOUT, DISC.UPPER.KNOCKOUT |

The table below lists the binary option with double barriers that qualifies for payment when either barrier is breached.

| Field | Value |
|---|---|
| Barrier Type | DKIN |
| Option Variant | BINA |
| Barrier Evaluation | CONT, DISC |
| Exotic Type.1 | CONT.LOWER.KNOCKIN, DISC.LOWER.KNOCKIN |
| Exotic Type.2 | CONT.UPPER.KNOCKIN, DISC.UPPER.KNOCKIN |
| Exotic Type.3 | CASH.PAYOUT |

The table below lists the binary option with double barriers that is disqualified from payment when either barrier is breached.

| Field | Value |
|---|---|
| Barrier Type | DKOT |
| Option Variant | BINA |
| Barrier Evaluation | CONT, DISC |
| Exotic Type.1 | CONT.LOWER.KNOCKIN, DISC.LOWER.KNOCKIN |
| Exotic Type.2 | CONT.UPPER.KNOCKOUT, DISC.UPPER.KNOCKOUT |
| Exotic Type.3 | CASH.PAYOUT |

The table below lists the binary option with dual barriers that is qualified for payment when both is breached.

| Field | Value |
|---|---|
| Barrier Type | DUKI |
| Option Variant | BINA |
| Barrier Evaluation | CONT, DISC |
| Exotic Type.1 | CONT.LOWER.KNOCKIN, DISC.LOWER.KNOCKIN |
| Exotic Type.2 | CONT.UPPER.KNOCKIN, DISC.UPPER.KNOCKIN |
| Exotic Type.3 | CASH.PAYOUT |

The table below lists the binary option with dual barriers that is disqualified from payment when both is breached.

| Field | Value |
|---|---|
| Barrier Type | DUKO |
| Option Variant | BINA |
| Barrier Evaluation | CONT, DISC |
| Exotic Type.1 | CONT.LOWER.KNOCKIN, DISC.LOWER.KNOCKIN |
| Exotic Type.2 | CONT.UPPER.KNOCKOUT, DISC.UPPER.KNOCKOUT |
| Exotic Type.3 | CASH.PAYOUT |

> **⚠️ Note:** In DX.TRADE , for double or dual barriers, the linked option types with barriers should have the same value in the Exercise Expire , Event Time Type and Et Eq Modifier fields in DX.OPTION.TYPE . For binary options, CASH.PAYOUT option type is mandatory if the Option Variant field is set as BINA.


##### Trade Processing

The records in DX.OPTION.TYPE are linked to DX.TRADE to specify the barriers of the contract. Attributes of the barriers are defined in DX.OPTION.TYPE . Some user-defined fields in the DX.OPTION.TYPE application are used to capture additional information related to barrier evaluation which must be mapped to the MT306 message.

The following are scenarios for trade processing:

Scenario 1 - Creating a record for a binary option with a single barrier

In this scenario, the user creates a record in

for a binary option with a single barrier, which qualifies for payment when the barrier is breached. The exotic option is created with the below details:

- Option Variant set as BINA
- Barrier Type set as UIKI

The following fields are set in DX.OPTION.TYPE and DX.TRADE .

- Exotic Type set as CONT.KNOCKIN
- Barrier Level set as 1.6565
- Cont Time Source set as NYSE09001500

And in the cash pay-out option

- Exotic Type set as CASH.PAYOUT
- Description set as CASH.PAYMENT
- Pay Put Ccy set as USD
- Pay Out Amount set as 8000

The screenshot below is an example of the DX.TRADE application.

The screenshot below shows the delivery reference ID updated in DX.TRANSACTION .

The screenshot below shows the SWIFT MT306 message with event details.

> **⚠️ Note:** Barrier evaluation is done outside the system. If the barrier is breached, it indicates to the system by setting the Exotic Event field as Yes in the CONT.KNOCKIN event type.

The screenshot below is an example of the DX.TRADE application.

The screenshot below shows the delivery reference ID updated in DX.TRANSACTION .

The screenshot below shows the SWIFT MT306 message with event details.

end of accordion body

Scenario 2 - Creating a record for a single barrier with vanilla option

In this scenario, the user creates a record in

for a single barrier with vanilla option. The exotic option is created with the below details:

- Option Variant set as VANI
- Barrier Type set as DOKO

The following fields are set in DX.OPTION.TYPE and DX.TRADE .

- Exotic Type set as DISC.KNOCKOUT
- Barrier Level set as 1.1212
- Cont Time Source set as NYSE0900

The screenshot below is an example of the DX.TRADE application.

The screenshot below shows the delivery reference ID updated in DX.TRANSACTION .

The screenshot below shows the SWIFT MT306 message with event details.

> **⚠️ Note:** Barrier evaluation is done outside the system, and once the barrier is breached, the system is indicated by setting the Exotic Event field as Yes in the DISC.KNOCKOUT event type. Since this is a knock out barrier, the option can only expire without any value.

The screenshot below is an example of the DX.TRADE application.

The screenshot below shows the delivery reference ID updated in DX.TRANSACTION .

The screenshot below shows the SWIFT MT306 message with event details.

end of accordion body

Scenario 3 - Creating a record for a vanilla option with double barrier

In this scenario, the user creates a record in

for a vanilla option with double barrier. The exotic option is created with the below details:

- Option Variant set as BINA
- Barrier Type set as DUKI

The following fields are set in DX.OPTION.TYPE and DX.TRADE .

Option Type 1

- Exotic Type set as CONT.UPPER.KNOCKIN
- Barrier Level set as 1.6565
- Cont Time Source set as NYSE09001500

Option Type 2

- Exotic Type set as CONT.LOWER.KNOCKIN
- Barrier Level set as 1.1212
- Cont Time Source set as *, indicating it is not required. Time source type is applicable only for the first multi value set

The screenshot below is an example of the DX.TRADE application.

The screenshot below shows the delivery reference ID updated in DX.TRANSACTION .

The screenshot below shows the SWIFT MT306 message with event details.

In this scenario, both barriers are breached, which is indicated to the system by setting the Exotic Event field to Yes in the respective multivalue set.

The screenshot below is an example of the DX.TRADE application.

The screenshot below shows the delivery reference ID updated in DX.TRANSACTION .

The screenshot below shows the SWIFT MT306 message with event details.

end of accordion body

Scenario 4 - Creating a record for non-deliverable and cash-settled options

In this scenario, the user creates a record in

for non-deliverable and cash-settled options.

The screenshot below shows the delivery reference ID updated in DX.TRANSACTION .

The screenshot below shows the SWIFT MT306 message with event details.

end of accordion body


#### 📋 Tasks

There are no Tasks available for the SWIFT MT306 for Exotic Options feature.


#### 📊 Outputs

There are no Outputs available for the SWIFT MT306 for Exotic Options feature.


> **Related Applications:** `DX.OPTION.TYPE`, `DX.PARAMETER`, `DX.TRADE`, `DX.TRANSACTION`, `DX.USR.FLD.OPT`

---


### 3.28  Trade


> **📇 Quick Reference Card**
> 
> **Purpose:** *This section describes the trade creation and the delivery features of Derivatives (DX).*
> 
> **Key Fields:** *Buy or Sell*, *Closeout Market Price*, *Contract*, *Customer No.*, *LINK.REFERENCE*, *Matured Lots*, *Maturity Date*, *Pri Lots* ... +5 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

This section describes the trade creation and the delivery features of Derivatives (DX).


#### ⚙️ Configuration

There is no specific configuration for trade. The parameter tables are setup at the implementation stage.


#### 📋 Tasks

Trade is a basic economic concept involving the buying and selling of goods and services, with compensation paid by a buyer to a seller, or the exchange of goods or services between parties.

The core banking system provides a holistic approach towards trading in Securities, Derivatives, Fiduciaries, REPO, RESO and Structured Products.


##### Workflow

This feature allows users to perform the following tasks:

| SCREENS | WORKFLOW |
|---|---|
|  | Modify/Delete F&O Trades . |
| F&O Trades to complete | Click the Complete icon corresponding to a record. |
| Trade | Enter values in the fields which needs to be amended. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
|  | Authorise ETD Trades . |
| F&O Trades awaiting authorisation | Click the Authorise icon. |
| Trade | Click the Authorise icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Fill Open Order . |
| List of Open / Partially filled Orders | Click the Fill icon. |
| DX Fill Details | Enter values in the fields which needs to be amended. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. Accept the overrides, if any. |

This screen allows the user to enter the European Union Financial Transactions Tax (EU FTT).

1. Direct trade Input - EU FTT .
2. In the Trade Details screen, enter values in the following fields: Contract Trade Date Maturity Date Buy or Sell Price/Premium Sec Cust(Broker) Sec Price
3. In the Primary Side tab, enter values in the following fields: Customer No. Pri Lots

1. In the Sec Side(Details) tab, enter values in the Sec Cpty No field.
2. Click the Validate icon to check for errors and overrides.
3. Accept the overrides, if any.
4. Click the Commit icon to submit the record.

| SCREENS | WORKFLOW |
|---|---|
|  | Futures By Maturity . |
| List of Futures by Maturity | Click the Manual Mature icon. |
| DX.CO.MATURITY.INPUT,SYSTEM | Enter values in the following fields: Closeout Market Price Matured Lots Click the Commit the deal icon. |
| Cash Settlement Input Feed | Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
|  | List of F&O Trades . |
| List of ETD Trades done Today | Click the View icon corresponding to a record. |
| Trade | The system displays the record in view mode. |

| SCREENS | WORKFLOW |
|---|---|
|  | Not Filled/Partly Filled Orders . |
| List of DX Orders not filled or partially filled | Click the Fill icon. |
| DX Fill Details | Enter values in the fields which needs to be amended. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. Accept the overrides, if any. |

| SCREENS | WORKFLOW |
|---|---|
|  | Execute Upfront Pymt Orders . |
| Upfront Fund Orders to be Executed | Select the Execute(Zero Auth) option. Click the Launch icon. |
| Order Execution | Enter values in the following fields: Broker No Broker Type Nominal Recd Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Complete Upfront Pymt Trades . |
| Upfront Fund Orders to be Executed | Select the View option. Click the Launch icon. |
| Trade Completion and Authorisation | The system opens the record in view mode. |

| SCREENS | WORKFLOW |
|---|---|
|  | Manage Upfront Pymt Trades . |
| Upfront Trades | Enter a value in any search criteria. Click the FIND button. |
| Upfront Security Trades | Click the View Position icon. |
| Client Sec Position by Security | The system opens the security positions record of the security. |

To capture a FX OTC cover trade, perform the following steps:

1. Capture Derivatives Trade-Own Book
2. Select the FX OTC Cover from Choose DX Trade for Own Book
3. Enter values in the following fields: Contract Contract Trade Date Maturity Date Price/Premium Buy/Sell Customer Amount
4. Click the Validate icon to check for errors and overrides
5. Upon Successful validation, Click the Commit icon to submit the deal for authorisation.

To capture an Exchange Traded Derivatives, perform the following steps:

1. Capture Derivatives Trade-Own Book
2. Select the Exchange Traded Derivatives from Choose DX Trade for Own Book
3. Enter values in the following fields: Contract Contract Trade Date Maturity Date Buy/Sell Own Book ID Price/Premium Call or Put (in case of option contract)
4. Click the Validate icon to check for errors and overrides
5. Upon Successful validation, Click the Commit icon to submit the deal for authorisation.

To capture a Generic Option trade, perform the following steps:

1. Capture Derivatives Trade-Own Book
2. Select the Generic Option from Choose DX Trade for Own Book.
3. Enter values in the following fields: Contract Trade Date Premium Counter Party Buy/Sell Counterparty Maturity Date
4. Click the Validate icon to check for errors and overrides
5. Upon Successful validation, Click the Commit icon to submit the deal for authorisation.


#### 📊 Outputs

Users can view the below list of enquiries and reports pertaining to Trade in the core banking system.


##### Enquiries and Reports

The navigation and uses of each enquiry is given in the drop-downs:

Filled Orders

This enquiry displays the list of all the orders filled so far and the Trades created for them.

Delivery Messages

This enquiry displays the delivery messages generated from a Derivatives trade. For FX Option trades, system generates a MT305 Swift message. A print advice is also generated on input, amendment, cancellation or closeout of a trade.

List of Open B2B Trades

This enquiry lists the Trades with similar Back-to-Back (B2B) reference. The user can check the contracts that have a Back-to-Back Trade reference and reconcile the differences if any.

List of Linked Trades

This enquiry lists the linked Trades with Common Unique Reference. If underlying trade is not traceable due to the missing Common Reference or a wrong reference, the users can manually map and update the same.

Options by Exercise Date

This enquiry displays all Option trades, where bank is a party, in descending order of exercise date. The exercise date is determined as set in the Contract Master record.

Own Book DX Position

This enquiry displays the Own Book derivatives positions. Users have options to view Other Position, Contract Definition, Calculated Price and Edit Market.

Warrants and Hegde Txn Details

Warrants issued by the Banks are hedged with Option Trades to offset losses in Investments. In Temenos Transact , issuance of warrants are handled through SEC.TRADE and hedging is done through DX.TRADE application. These two trades are linked using some common reference updated in the LINK.REFERENCE field.

This enquiry displays the list of both warrants and hedge transaction details with the same common reference to ensure that the correct transactions ( SEC.TRADE and DX.TRADE ) are linked. The user requires to provide a Common reference as mandatory key to retrieve the details. It also enables the user to identify incorrect linkages between transactions.

Warrants and Hegde Txn – Notional Reconciliation

Warrants issued by the Banks are hedged with Option Trades to offset losses in Investments. In Temenos Transact , issuance of warrants are handled through SEC.TRADE and hedging is done through DX.TRADE application. These two trades are linked using some common reference updated in the LINK.REFERENCE field.

This enquiry displays the list of the linked transactions to ensure the adequacy of the hedge trades by reconciling both the warrant and hedge transactions. The user requires to provide a Common reference as mandatory key to retrieve the details.


##### SWIFT Messages

The below list of SWIFT messages are generated by the core banking system pertaining to Trade.

MT305 is a message exchanged between the financial institution and corporate customers which have agreed to a foreign currency options contract. The details of the new contract between the counterparties or amendment to a previously agreed contract is confirmed in this message type.


##### Advices

The user can view the following advices:

A print advice is generated from a DX Trade which provides brief details of the trade.


##### Alerts

NA

---


### 3.29  Transaction Fees and Charges


> **📇 Quick Reference Card**
> 
> **Purpose:** *Two types of fee setup are available in the Derivatives (DX) module.*
> 
> **Key Fields:** *Base Amount*, *Channel*, *Charge Code*, *Charge Percent*, *Clfee Charge*, *Closeout Txn Amt*, *Comm Charge*, *Exchange Type* ... +29 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Two types of fee setup are available in the Derivatives (DX) module.

- DX.COMMISSION framework
- SCDX.CHARGE.PARAMETER framework

Any one of the frameworks can be used and this is controlled by a parameter setup. The DX module enables automatic calculation of the trading commission for derivatives transaction based on the criteria set up in the DX.COMMISSION application. This facility allows calculation of commission and charges based on a number of decision levels as explained in the below table.

| Level | Defaults For |
|---|---|
| System | All conditions |
| Group | Customer groups set up within the DX.GROUPING application Contract groups set up within the DX.CONTRACT.CLASS application |
| Individual | Specific customer set up within the DX.CUSTOMER application Specific contract set up within the DX.CONTRACT.MASTER application |


##### Setting up Fee inDX.COMMISSION

Commission can be set up for the following combinations of customer or group or contract. These elements are separated by ‘-‘ and can be combined to create the commission code. The codes, which denote a narrower scope of grouping, are selected in precedence to those with greater generalisation. In each search to calculate commission, the order of priority and the list of valid combinations are given below:

- Customer and contract
- Customer and contract class
- Customer
- Customer group and contract
- Customer group and contract class
- Customer group
- Contract
- Contract class
- System default


##### Setting up Multiple Charges Framework inSCDX.CHARGE.PARAMETER

The user can define any number of charges or taxes using the multiple charges framework for derivatives transaction. The various charges or taxes applicable for each event in the derivatives life cycle can be defined using this multiple charges framework. The charges or taxes that must be charged at the transaction level needs to be defined in the SCDX.CHARGE.PARAMETER application. Category codes related to the charge are defined in this application.

For each charge or tax defined in SCDX.CHARGE.PARAMETER , a record needs to be created in the SC.CHARGE.TAX.CALC application to define the calculations basis or rules of the charge or tax. Different calculation rules can be defined based on the various combinations of transaction characteristics:

- Stock exchange
- Security type
- Security domicile
- Transaction type
- Customer group

Based on the transaction characteristics, the defined charges or taxes are calculated.


#### ⚙️ Configuration

This topic details about the configuration of transaction fees, charges and commission in the Derivatives (DX) module.


##### DX.PARAMETER

The Scdx Charge Method field in the DX.PARAMETER application needs to be set to Yes, only then the charges or taxes specified in SCDX.CHARGE.PARAMETER is reflected in the transactions. If the field is set to No, then the charges are calculated based on the DX.COMMISSION setup.


#### 🔧 Working With

This topic details how transaction fees, charges and taxes are calculated and accounted in the Derivatives (DX) module.


##### DX.COMMISSION

The procedure to determine the appropriate commission table can be controlled by the Search All Commsn field in DX.PARAMETER . If this field is set to No, records are not searched further after a record is matched with the key. If this field is set to Yes, each record found is searched to find all matching criteria. The commission codes may be entered in the following formats.

| ID | Description | Abbreviation |
|---|---|---|
| CU100018 | Customer 100018 | (CU = Customer Code) |
| CGINT2 | Customer Group INT2 | (CG = Customer Group) |
| CT100 | Contract Code 100 | (CT = Contract Code) |
| CCGILTS | Contract Class GILTS | (CC = Contract Class) |
| CU100018-CT100 | Customer 100018, Contract 100 | (CU), (CT) |
| CU100018-CCGILTS | Customer 100018, Contract Class GILTS | (CU), (CC) |
| CGINT2-CT100 | Customer Group INT2, Contract 100 | (CG), (CT) |
| CGINT2-CCGILTS | Customer Group INT2, Contract Class GILTS | (CG), (CC) |
| SYSTEM | Catch All | System-level defaults |

For the system to interpret the input, a two-character prefix is used to identify each element. Also, the application recognises mnemonics used by the source applications.

The additional criteria for determining the calculation of commission and charges are defined in DX.COMMISSION . The Field Name field contains a drop-down list of fields from the DX.TRADE application. When a field is selected, the contents from the trade are compared using the entry in the Operand field against the values in the Field From and Field To fields. These fields are sub-valued for the tests to be combined for better refinement. The secondary leg fields on the trade are not listed in the Field Name field. If a primary leg field is selected, the corresponding secondary trade field name is displayed in the Sec Fld Nme field. This is used in tests for customers, which appear on the secondary leg of the trade.

The following screenshot shows an example, which requires the below two conditions to be satisfied:

- The trade currency is equal to USD
- The number of lots is between 10 and 20

If either of the condition proves to be false for the trade, the commissions specified in this example is not used.

Once the trade details are matched, a maximum of up to five different types of commission and charges can be calculated. Each type can contain a commission or charge code linked to either the FT.COMMISSION.TYPE or FT.CHARGE.TYPE application. The types of commission or charges and fields in which they are entered are given in the following table.

| Commission Type | Field Name |
|---|---|
| Commissions | Comm Charge |
| Execution fees | Exfee Charge |
| Clearing fees | Clfee Charge |
| Regulatory fees | Rgfee Charge |
| Miscellaneous fees | Misc Charge |

More than one commission code can be entered for each commission type, but there is only one commission currency per type. If a commission currency is specified, this value overrides the currency defined in FT.COMMISSION.TYPE or FT.CHARGE.TYPE . The Charge Percent field in DX.COMMISSION indicates a percentage multiplier to be applied for the charge amounts calculated. However, this is performed on certain types of commission, execution, and clearing fees only. The following are examples of simple commission.

A bank has set up a customer group GROUPEXT for all relevant internal (own-book) customers, and a similar group GROUPINT for all non-own-book customers. On behalf of their internal accounts and external customers, they trade European options on EUREX (European Derivatives Exchange) and LIFFE (London International Financial Futures and Options Exchange). They are not the trading members of any exchange, but use an external broker with the customer number 100324. This broker charges different rates for each exchange. These charges are created in FT.COMMISSION.TYPE as CISERXEXC and CISLIFFEEX, respectively. The bank charges the internal accounts the same rates, but charges the private customers a standard commission amount (STDCUST).

- According to standard exchange rules, commissions are only charged when a position is closed out. In the GROUPEXT customer commission setup, the Pay Receive Flag field is set to Pay indicating that the customer is paying the commission to the bank.
- For the EXTERN1 customer group, the Field From is left blank so that the example illustrated with Field Name set to Exchange Code and Operand set to Ne picks up all exchanges (LIFFE and EUREX in this example).
- The commission setup for Broker A - 100115 has the Pay Receive Flag field set to Receive, indicating that the bank is paying the commission to the broker.

- A bank trades only foreign exchange options. There are no overriding commissions for brokers or exchanges and a general system default can be used.
- The bank has two commonly traded currencies (USD and GBP), for which it charges a percentage commission (STDPONT). If other currencies are traded, extra charges (inputted as NONSTD) are levied.

The commission fields in DX.TRADE display a summarised form of the commission data. After a trade is committed, detailed analysis of the trading commission can be viewed in the DX.COMMISSION.DIAGS application. The following are the two main methods of entering the trading commission for a customer:

- Automatically from criteria set up in DX.COMMISSION
- Manually overriding the commission fields

The method selected in the Pri Auto Manual or Sec Auto Manual fields in DX.TRADE controls the commission collection method.

The commission fields are updated automatically in this method. All the defaulting values are driven by the details set up in DX.COMMISSION .

In the below example, the commission system has matched a record in DX.COMMISSION with this transaction and applied both the execution and clearing commissions. The commission amounts are held in Pri Commission Amt and are calculated as 250 USD and 375 USD. The account to post the commissions are updated in the Pri Commission Account field. If the account currency is different from the commission currency, the exchange rate to calculate the value in the Pri Cacc Amt field is displayed in the Pri Comm Exc field. The Pri Commission Tax field indicates that the tax duty is levied on this commission.

If the customer (for whom commission and charges are calculated) is a broker and another broker is indicated in the Executing Broker field in DX.TRADE , the account or category for posting the execution fee only is changed to the executing broker’s account for any execution fees to be paid. Because the values of the trade can affect the automatic commission calculations, the commission fields are cleared for any change to a field on the trade. If a customer’s details do not match the commission criteria, commission is not calculated and an override message is displayed.

| Field | DX.TRADE | DX.ORDER |
|---|---|---|
| Exchange Type | Indicates the types of exchange used to enter the trade | Indicates the types of exchange used to enter the order |
| Channel | Indicates the modes of transaction used to enter the trade | Indicates the modes of transaction used to enter the order |

| Field Name | Value |
|---|---|
| Charge Tax Type | Transaction Tax |
| Charge Tax Desc | Transaction Tax |
| Charge Tax Cat | 17200 |
| Chg Tax Cr Code | 80 |
| Chg Tax Dr Code | 30 |
| Chg Tax Cust Brok | Customer |
| Post Lcy | Yes |


#### 📋 Tasks

There are no Tasks available for Transaction Fees, Charges and Commission feature.


#### 📊 Outputs

There are no Outputs available for Transaction Fees, Charges and Commission feature.

---


### 3.30  Transfers


> **📇 Quick Reference Card**
> 
> **Purpose:** *Derivatives (DX) module allows transfer of trades between portfolios and customers (internally and externally).*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Derivatives (DX) module allows transfer of trades between portfolios and customers (internally and externally).


#### ⚙️ Configuration

Transfers are performed with or without account postings or confirmations being generated, if any. It is parameterised on a transfer-by-transfer basis.

Appropriate fields in the DX.TRADE , DX.TRANSACTION and DX.CLOSEOUT applications are used for Transfers functionality. When the DX.CO.XFER.MANUAL or DX.CO.EXT.XFER.MANUAL records are authorised, the DX.CLOSEOUT record is created to reflect the trade transfers.

The following transfer records are setup in DX.EVENT.TYPE :

- CN – Internal transfer (Transferor side)
- II – Internal transfer (Transferee side)
- CO – External transfer (Outgoing)
- CT – External transfer (Incoming)


#### 📋 Tasks

There are no Tasks available for Transfer feature.


#### 📊 Outputs

There are no Outputs available for Transfer feature.

---


### 3.31  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Single European Currency (Euro) was introduced on 1 January 1999. The Euro module was introduced in Temenos Transact to support countries converting from national currency units to Euros. The Euro module is a set of additional functionality across all applications and utilities designed to suppo...*
> 
> **Key Fields:** *Available Date*, *Base CCY Rank*, *Base Ccy Rank*, *Build Fwd Rate*, *Converted Lcy*, *Fixed Ccy*, *Fixed Rate*, *Fixed Start Date* ... +3 more
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- APIs
- Temenos Transact Services

The Single European Currency (Euro) was introduced on 1 January 1999. The Euro module was introduced in Temenos Transact to support countries converting from national currency units to Euros. The Euro module is a set of additional functionality across all applications and utilities designed to support the new requirements of the single currency and to provide a smooth conversion from the national currency. Although this module was designed to work with the introduction of the Single European Currency, this module supports additional functionality. For example, when there is a requirement to perform a conversion of the system base currency.

> **⚠️ Note:** Any reference to euro in this document can equally apply to any currency irrevocably fixed to another. If there is a requirement to change the base currency to a currency that is not used as the base for usual exchange quotation rates, then a slight change to the conversion will be required.

Following are the terminologies used in this document to explain the Euro conversion process:

| Term | Description |
|---|---|
| Article 235 | The council regulation (EC), which governs conversion and rounding rules for euro conversion. |
| EMU | European Monetary Union. |
| NCU | National Currency Unit – a general term for existing national currencies. |
| In-currency | A currency that is converting to EUR. |
| Out-currency | A currency that is not a member of EMU. |
| Triangulation | The process of converting one In-currency amount to another through the euro. |
| Re-denomination | Process of converting an In-currency transaction to the euro equivalent of something, which is at the fixed conversion rate. |
| Transition Phase | The phase where both NCU and EUR can be used. ERI (Euro Related Information) is added to SWIFT messages where the amount is converted from NCU to EUR. |


##### Product Configuration

The euro is a new currency that must be defined just as any other currency in Temenos Transact .

> **⚠️ Note:** Although the exchange rate between the existing ECU (code XEU) and the euro is defined as 1, the XEU must be treated as a separate currency.

The following tables should be configured to set euro as a new currency (code EUR).

Europe must be defined as a country in the COUNTRY application before the currency can be specified. There is probably already a code XE, used for the XEU. However, the euro will need its own country code (EU) to be defined.

The user can also define a Geographical Block to hold all In-countries.

The common characteristics of the euro should be defined in the CURRENCY.PARAM application. The user should set the Base Ccy Rank and a standard interest day basis should be agreed for the euro.

The CURRENCY record can now be defined for EUR. User must ensure that the correct Quotation Code is used. The Fixed Ccy , Fixed Start Date and Fixed Rate fields should not be used for the EUR currency.

The euro is defined as a currency before it is due to come into existence. However, financial movements can be generated with value date before this date (that is, 01/01/99). The Available Date field should be set to the start date of the currency. The system will generate an override message, if any entry is posted across an account with a value date prior to the Available Date.

Post this process, the euro is an existing currency and does not need an available date.

The value of Base Ccy Rank is defaulted to the value in CURRENCY.PARAM and cannot be amended directly. If a change is required, the underlying CURRENCY.PARAM record should be amended. The next amendment to the CURRENCY record will update this field.

EU should be defined in the HOLIDAY table. Settling process happens on all the day except Christmas and New Year holidays.

The PERIODIC.INTEREST table ‘01’ should be defined with the forward euro interest rates. The foreign exchange forward rates for this currency can be calculated automatically if required, by using the Build Fwd Rate field.

The user must check the BASIC.INTEREST application for existing base rates for the local currency and each of the In-currencies. A euro rate is required for each base rate used by existing contracts and accounts, which may be re-denominated in euro.

Account Conditions should be defined for each condition group that EUR accounts are expected to be opened in. Account group conditions are defined in the below applications:

- GROUP.DEBIT.INT
- GROUP.CREDIT.INT


##### Illustrating Model Parameters

This section covers the high-level parameterisation setup required to work with Single European Currency (Euro). This module helps the user to setup additional functionalities across all applications and utilities designed to support the requirements of single currency.

| S.No. | Parameters | Description |
|---|---|---|
| 1. | COUNTRY | This application allows the user to define the code EU as Euro need its own country code. In addition, Geographical Block field must be defined from the available dropdown geographies. |
| 2. | CURRENCY | This application allows the user to define the currency record for EUR. In addition, user must ensure that correct quotation code is defined. User must not define Fixed Ccy , Fixed Rate and Fixed Start Date for EUR Currency. |
| 3. | CURRENCY.PARAM | This application allows the user to define the common characteristics of Euro. In addition, Base CCY Rank must also be defined. |
| 4. | FORWARD.RATES | This application allows the user to define the premium or discount expected for the exchange rate of the Euro against the local currency when it is Out- Currency. However, if involved currency is In-Currency type, premium or discount must not be applied for the Euro. |
| 5. | HOLIDAY | This application allows the user to define the public holidays for EU, for the calendar years over which the bank's current business is spread. |
| 6. | PEIRODIC.INTEREST | This application allows the user to default the interest rate for any time period, which can be used by applications like foreign exchange on forward contracts using interest revaluation method or loans and deposits applications to perform automatic rollover. For Euro module, periodic interest must be defined with forward euro interest rates. |
| 7. | BASIC.INTEREST | This application allows the user to define floating rates – Base Rate, Prime Rate and Overnight Rate. Whenever there is a change in the rate, user must define the interest rates for the currency with the date on which it becomes active. A record must be defined for Euro with the applicable rates along with effective date. |
| 8. | EU.PARAMETER | This application allows the user to define the following: Company code – Code of the company where local currency is converted. Routine to calculate the new Euro account number. Default category for internal suspense accounts when converting contracts from one currency to fixed currency. Internal account category code to be used for posting adjustment entries in the new local currency after the conversion of the base currency has taken place. Transaction code used for all adjustment entries posted by the conversion process. The rate used to convert local currency amounts from Original Lcy to Converted Lcy . |
| 9. | PM.CALENDAR | This application allows the user to define a calendar in which possible settlements is allowed for Euro. |

---


### 3.32  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *The System Tables user guide explains the Customer and related reference tables and the Core Reference tables.*
> 
> **Applications:** `SYSTEM`
> 
> **Key Fields:** *Application Access Link*, *Application Access Type*, *Currency Name*, *Enable Customer Closure*, *FIELD.NAME*, *FIELD.VALUE*, *INT.BASIS*, *Interest Basis* ... +7 more
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- APIs
- Temenos Transact Services

The System Tables user guide explains the Customer and related reference tables and the Core Reference tables.

- Customer and related reference tables – This includes the following: The customer application and associated static tables. The customer centric functionalities.
- Core Reference tables – This includes core tables that act as reference for transaction processing as listed below: Country and related tables (like REGION , HOLIDAY and DATES ) Currency Category Interest related tables (like Accrual Parameter, Interest Basis, Basic Interest and Periodic Interest) Charge related tables Tax related tables Card Management tables Cheque Management tables Treasury and Settlements related tables Other Core Reference Tables


#### Product Configuration

The following system-wide applications help in grouping the customers and defining rules for the group based on the business purposes, like defining customer group specific charges and tax.

- CONDITION.PRIORITY
- XXX.GEN.CONDITION and XXX.GROUP.CONDITION, where XXX refers to the business application.
- APPL.GEN.CONDITION


##### Condition Priority

The purpose of the CONDITION.PRIORITY application is to specify, for certain applications, which data elements in other reference applications can be specified to determine condition groups. CONDITION.PRIORITY records can be created with the following IDs:

- ACCOUNT
- FIDUCIARY
- FUNDS.TRANSFER
- FX.MARGIN
- LETTER.OF.CREDIT
- SC.MANAGEMENT
- SC.SAFEKEEPING
- SC.TRADING
- STATEMENT
- TAX
- POR.TRANSACTION

CONDITION.PRIORITY is a CUS level application. Records of this application can be shared between companies, which share the same customer company, or there could be company-specific CONDITION.PRIORITY records by suffixing a hyphen and a Company Code in the ID.

For the

application, it is possible to have a specific record for the Company DE0010001 with the ID ACCOUNT-DE0010001.

The (parameters) records without a Company ID suffixed is applicable to the Master Customer Company (specified as Customer Company in the COMPANY application) as well as to Companies that do not have their own CONDITION.PRIORITY records.

An existing CONDITION.PRIORITY record cannot be modified. However, it is possible to specify parameters that are applicable in future (after the COB processing on a specified date, which can be either the processing date or any future date) by creating CONDITION.PRIORITY records by suffixing a hyphen and a date after the company code in the ID.

The record with ID ’ACCOUNT--20040702’ (with a null Company ID for the customer company) is applicable to the Master Customer Company and the record with ID ‘ACCOUNT-DE0010001-20040702’ is applicable to the Company DE0010001, both records to be effective after the COB processing on 2nd July 2004. The date specified can either be the processing date or it could be a future date.

It is possible to specify the priority items (fields) using the Priority Item field. This is a multi-valued field which defines the order in which fields are used, when matching conditions against values specified in the XXX.GEN.CONDITION records.

- Fields from CUSTOMER application can be specified in all CONDITION.PRIORITY records.
- Fields from ACCOUNT application can be specified only in the CONDITION.PRIORITY records related to ACCOUNT or STATEMENT.
- Fields from SEC.ACC.MASTER can be specified only in the three CONDITION.PRIORITY records related to Wealth application (with IDs SC.MANAGEMENT, SC.SAFEKEEPING and SC.TRADING).

The priority items specified in the CONDITION.PRIORITY records are defaulted as the field names in the corresponding XXX.GEN.CONDITION records.

While determining the condition groups of applications, the priority of the data items (specified as Priority Item ) is determined by their relative position in the CONDITION.PRIORITY record.

For each priority item specified in CONDITION.PRIORITY , users can also specify a validation, which ensures that a value entered for a priority item (in XXX.GEN.CONDITION applications) exists as a record ID in another table. This can also be used to display an enrichment when the value is entered.

In the

record for

, the

CATEGORY’ can have a validation specified in the

DESCRIPTION’. In this case, when a value for the CATEGORY is entered in

, the value entered should be a valid record ID in the

application, and the value of the

field in that

record will be displayed as an enrichment.


##### Parameters and Rules for Groups

The XXX.GEN.CONDITION applications provide the parameters to calculate the default groups for some applications. The priority data items, which are used in the XXX.GEN.CONDITION tables, are defaulted from the corresponding CONDITION.PRIORITY records.

The XXX.GEN.CONDITION applications and the corresponding CONDITION.PRIORITY records from which the priority data items are defaulted are listed below:

| XXX.GEN.CONDITION Applications | CONDITION.PRIORITY record ID from which priority data items are defaulted |
|---|---|
| ACCT.GEN.CONDITION | ACCOUNT |
| FD.GEN.CONDITION | FIDUCIARY |
| FT.GEN.CONDITION | FUNDS.TRANSFER |
| LC.GEN.CONDITION | LETTER.OF.CREDIT |
| SCPM.GEN.CONDITION | SC.MANAGEMENT |
| SCSK.GEN.CONDITION | SC.SAFEKEEPING |
| SCTR.GEN.CONDITION | SC.TRADING |
| STMT.GEN.CONDITION | STATEMENT |
| TAX.GEN.CONDITION | TAX |
| FX.GEN.CONDITION | FX.MARGIN |
| PP.GEN.CONDITION | POR.TRANSACTION |

The parameters specified in FD.GEN.CONDITION , FT.GEN.CONDITION , LC.GEN.CONDITION , SCPM.GEN.CONDITION , SCSK.GEN.CONDITION , SCTR.GEN.CONDITION , TAX.GEN.CONDITION , and PP.GEN.CONDITION are used to default the condition groups in the CUSTOMER.CHARGE application.

The parameters specified in ACCT.GEN.CONDITION are used to default the account group ( Condition Group ) in ACCOUNT , while those specified in STMT.GEN.CONDITION are used to default the frequency in ACCOUNT.STATEMENT .

For each XXX.GEN.CONDITION application, there is a corresponding XXX.GROUP.CONDITION application (except for STMT.GEN.CONDITION ) to define the various parameters for each group. The following XXX.GROUP.CONDITION applications exist:

- ACCT.GROUP.CONDITION
- FD.GROUP.CONDITION
- FT.GROUP.CONDITION
- LC.GROUP.CONDITION
- SCPM.GROUP.CONDITION
- SCSK.GROUP.CONDITION
- SCTR.GROUP.CONDITION
- TAX.TYPE.CONDITION
- FX.GROUP.CONDITION

All the XXX.GEN.CONDITION and XXX.GROUP.CONDITION applications referred here are of the FTD level, which may be company specific or shared between companies depending on the configuration of Default Finan Com or Spcl Fin File fields in the COMPANY record.

If the FTD type files for the Company DE0010001 are unique, then the

records for the Company DE0010001 can have the data items defaulted from the

record with ID as ‘ACCOUNT-DE0010001’ if that record exists, else from the default

record with ID as ‘ACCOUNT’.

While defining CONDITION.PRIORITY records to be applicable in future, it is possible to specify which XXX.GEN.CONDITION and XXX.GROUP.CONDITION records need to be retained, by specifying their IDs in the Gen Cond Keep and Group Cond Keep fields respectively. During COB processing on the specified date, these XXX.GEN.CONDITION records are automatically modified with priority data items applicable for the new structure, by retaining existing priority data items and their values. New priority data items are updated with null values.

Further, in conjunction with dated CONDITION.PRIORITY records, it is also possible to specify dated XXX.GEN.CONDITION records, which can become effective in future. Such XXX.GEN.CONDITION records are defined by suffixing a hyphen with a date (either processing date or a future date) in the ID. Priority data items in these records are defaulted from the corresponding dated CONDITION.PRIORITY records. These record IDs must not be defined as retention record IDs in the Gen Cond Keep field of CONDITION.PRIORITY .

After COB processing on the specified date, the dated XXX.GEN.CONDITION records replace the corresponding records without a date in the ID.

Those XXX.GEN.CONDITION records that are not included in the Gen Cond Keep field of the corresponding dated CONDITION.PRIORITY record or those records that do not have a corresponding dated XXX.GEN.CONDITION record are dropped after the COB processing on the specified date.

With the exceptions described below, future dated XXX.GROUP.CONDITION can be created with an ID of the format ‘xxx-Date’, provided the ID is not already specified in the Group Cond Keep field of the corresponding dated CONDITION.PRIORITY record. After COB processing on the specified date, the dated XXX.GROUP.CONDITION records replace the corresponding records without a date in the ID.

There is an exception to the above referred functionality (which existed before the CONDITION.PRIORITY application has been enhanced to accept dated records). The ID format of the SCPM.GROUP.CONDITION and SCSK.GROUP.CONDITION applications is ‘xxx.date’ (both parts mandatory and connected by a dot) to allow definition of parameters, which applies on various dates. The first part of the ID is validated against the first part of the corresponding XXX.GEN.CONDITION records. When the records in these applications are entered, there is no validation against the CONDITION.PRIORITY records.

The XXX.GROUP.CONDITION records whose IDs are not included in the Group Cond Keep field of the corresponding dated CONDITION.PRIORITY record, or which do not have a corresponding dated XXX.GROUP.CONDITION record (suffixed to the ID with a hyphen and date), will be dropped after the COB processing on the specified date. However, customer-specific XXX.GROUP.CONDITION records with ID format as ‘C-Customer ID’ is not dropped after COB processing.

For Payments, the parameters and conditions applicable for a group of customers is defined in PP.CLIENT.CONDITIONRECORD application. Please read Introduction to Client Conditions for more details.


##### Parameter to Default Groups UsingTemenos TransactRoutine

The APPL.GEN.CONDITION application is used to define group conditions for contracts based on a combination of decisions and calls to locally developed subroutines. For example, it allows specific tax codes to be applied to particular types of contract for particular types of customer.

There is one record per application for which many sets of group conditions can be defined. User must ensure that multiple set of groups are defined correctly, as the first set of conditions that pass the validation checks result in that contract group code being applied.

A Temenos Transact subroutine, APPL.GRP.CONDITION can be called to evaluate the current contract record using relevant APPL.GEN.CONDITON . It returns the first group code where all decision checks evaluate to true.

The MM.MONEY.MARKET and LD.LOANS.AND.DEPOSIT applications call the evaluation routine automatically. Other applications can call the evaluation routine from VERSION routines to update local reference fields with the relevant group code.

The subroutine processes these decisions and updates the Contract Group field in the application record whenever the contract is changed. If changes to the contract cause the conditions to break, then a new Contract Group code is generated, which results in a different tax code being applied. A default group code can be defined as the last group code without associated conditions, if required. TAX.TYPE.CONDITION allows the Contract Group code to be linked to the allocation of specific tax codes.


##### Illustrating Model Parameters

Specifications for System Tables are grouped into different functionalities.

Core Reference tables available in the model bank are given below:

| S.No. | Parameter | Description |
|---|---|---|
| 1. | COMPANY | Contains details such as company's name, mnemonic, classification details, applications that are to be run, company level defaults and parameters. |
| 2. | DATES | Each company has a Date record, which contains the run dates for the previous, current and the next working day. Batch (overnight) processing system updates the record automatically. |
| 3. | CONDITION.PRIORITY | Used to specify the data elements to determine the condition groups for each application. In addition, the order of general conditions to be applied when more than one general condition is involved can also be defined. |
| 4. | COUNTRY.GROUP | Used to group the countries based on residence or non-residence when applying charges. |
| 5. | COUNTRY | Contains the static details of each country such as country name, currency code and so on. The key for this application must be a standard I.S.O country code. The CURRENCY codes must be in the system before setting up the country parameter. |
| 6. | EB.TIME.ZONES | Defines the standard zones that have uniform mandated standard time. The ID must be a valid time zone name as specified in the Internet Assigned Numbers Authority (IANA) time zone database. |
| 7. | HOLIDAY | - Indicates the public holidays for each country, or region within a country for the calendar year. |
| 8. | LANGUAGE | Identifies the languages that are to be used in the system when defining multi-language fields. The Abbreviation code assigned to each Language is used as a screen prompt. |
| 9. | INTEREST.BASIS | Determines the component for interest calculation based on the inputs provided in the INT.BASIS field. |
| 10. | CURRENCY.PARAM | Contains the common details such as Numeric Currency Code , Currency Name , Number of Decimal Places and the Interest Basis for each currency. This table ensures that the same numeric code and no of decimals are used on all the different currency files. |
| 11. | CURRENCY.MARKET | Helps to identify the correct exchange and revaluation rates to be applied for each currency. |
| 12. | TRANSACTION | Contains information about all the Transaction Codes that can be used in Temenos Transact . |
| 13. | SECTOR | Sector codes are defined in this table and assigned to each Customer record to group them into broad classifications like Private Sector, Public Sector, and Corporate Banks and so on. |
| 14. | INDUSTRY | Helps to define and assign the Industry codes to each Customer record to identify the industry of the customer. |
| 15. | CATEGORY | Category codes are used to classify financial transactions in Temenos Transact according to the type of business operation or product. |
| 16. | AC.CONSOLIDATE.COND | Allows the user to define the rules for the consolidation of entries for either an Account or a Category record. |
| 17. | INTERCO.PARAMETER | Determines if automatic balancing entries are raised when processing transactions in a multi-company or a multi-department (in the same company) environment. |
| 18. | EB.DUPLICATE.TYPE | Defines duplicate check criteria for applications. |
| 19. | EB.LOOKUP | This is a generic template to hold all the lookups for data access service. The user can create an EB.LOOKUP record with the definition and use them as drop-down list in applications. |
| 20. | EB.SYSTEM.ID | Provides a description for the SYSTEM.ID field in the accounting entry files, which include STMT.ENTRY , CATEG.ENTRY , CONSOL.NET.TODAY and RE.CONSOL.SPEC.ENTRY . |
| 21. | CONSOLIDATE.COND | The consolidation records hold the consolidation key, series of balance, total debit and credit movement fields. The details are held in for: • Asset and Liability • Profit and Loss |
| 22. | GROUP.ACCRUAL.PARAM | This is a parameter file, which holds the options for the bulk accrual of accounts. It reduces the number of accrual accounting entries by consolidating at various levels. |
| 23. | EB.LOCAL.CONTENT.TABLE | Stores local context-data on customer records at BNK level. |
| 24. | ST.ORGANIZATION.STRUCTURE | Holds the organizational hierarchy of the bank. |
| 25. | ST.ORGANIZATION.CODE | Helps to create Organization Codes at each level defined in the ST.ORGANIZATION.STRUCTURE application. |
| 26. | ST.BRANCH | Holds the branch record, which is updated on authorising the ST.ORGANIZATION.CODE record defined for each branch. |
| 27. | ST.LINE.OF.BUSINESS | Line of Business is defined to create different Cost Centers for the bank and align them later to a particular branch depending on its requirement. |
| 28. | CUSTOMER.EXIT.STATUS | Allows the bank to define the exit statuses and the exit reasons for each customer type (Prospect and Customer). It holds the details such as, allowed customer types, allowed exit reasons. Further, it helps to reclassify a bank Rejected Prospect or Closed (Customer) back to its default or original status. |
| 29. | COMPANY.CREATE | Contains details, such as, Company's Name, Address, Mnemonic, Sub Division code, Creation Date and Default Company details. Allows user to create COMPANY record manually and from which data gets auto-populated in COMPANY application. |
| 30. | ST.CUSTOMER.CLOSURE.PARAM | Customer Exit Status . This parameter application is used to configure the following: Enable Customer Closure - This field can be entered only in the SYSTEM record. The user can select the provided check box to enable the customer closure process and perform the pre-closure checks. Define the pre-closure conditions - The Transact core and non-core applications that must be checked for the presence of the customer data before the customer is closed, can be defined as individual records in this table. The user can define the following attributes in these records where ID of the record will be populated with the application name. Application Access Type - This field is used to define the method through which the customer can be identified in the records of the application specified in the ID. This field will have two options: Field - Denotes that the system must access a particular field of the application to identify the customer ID - The system must use the ID of the record to identify the customer. Application Access Link - The user can provide a field name that will be referred to identify the presence of the customer data. |

Customer related tables available in the model bank are given below:

| S.No. | Parameter | Description |
|---|---|---|
| 1. | TARGET | Target codes defined in this table are assigned to Customer records in Temenos Transact to indicate how the customer fits in with the Bank's overall marketing strategy. |
| 2. | CUSTOMER.STATUS | Customer Status codes defined in this table are assigned to Customer records in Temenos Transact to classify the customers based on the criteria defined locally. |
| 3. | RELATION | Helps to specify the various types of relations that can exist between Customers and, or Person Entities. |
| 4. | CUST.GROUP.PURPOSE | Defines the rules for a Customer Group based on the purpose of the group. The rules include where the customer group can be used and how the customers and parties in the group can be stored. |
| 5. | PARTY.RELATIONSHIP | Used to define multiple relationships between customers. |
| 6. | DEPT.LEVEL | Contains the valid levels of departmental hierarchy that are permitted in the system. |
| 7. | DEPT.ACCT.OFFICER | Used to identify each Department and Account Officer in the bank by means of a code. Each Customer record has an Account Officer code assigned, which helps to generate the M.I.S reports at the Account Officer level. |
| 8. | ST.CDM.PARAMETER | Holds the parameter configurations for customer dormancy processing at the lead company level. |
| 9. | ST.CUSTOMER.ACTIVITY.PARAMETER | This is a Parameter setup table, which helps to maintain the data relation details for the applications and it is enhanced to configure Access Type and Link for Joint account holders as well. JH.ACCESS.TYPE - This field determines on how the application can be accessed to get the list of personal data for joint account holders. JH.ACCESS.LINK - This field provides the link of accessing the application for personal data for joint account holders. |
| 10. | COUNTRY.RULES | Helps to define the country specific rules. |
| 11. | ADDRESS.RULES | Helps to define the country specific address rules for each country. |
| 12. | COUNTRY.PARAMETER | Helps to check the address rule that has to be applied to get the address details of the customer in a particular company. |
| 13. | ADDRESS.OUTPUT.FORMAT | Helps to define the various address output formats from which the user can choose the output formats. |
| 14. | ADDRESS.OUTPUT.RULES | Helps to define the Address Output Rules used for a country. |
| 15. | CONTACT.TYPE.PARAMETER | Helps the user to define the characteristics of each contact type captured in the CUSTOMER application. |
| 16. | ST.REG.EXCLUDE.PARAM | Exclusion Parameter setup is used to skip the customer activity. PARTY.APPLICATION – This field specifies the Party application for which the exclude criteria is going to define. (For now, this field is defaulted with 'CUSTOMER'). FIELD.NAME –This field specifies the field name from the party application to define the exclude criteria. OPERAND – This field specifies the operand that connects the field name and value. FIELD.VALUE – This field specifies the value for the respective field name mentioned to define the exclude criteria. |

Interest related tables available in the model bank are given below:

| S.No. | Parameter | Description |
|---|---|---|
| 1. | BASIC.RATE.TEXT | Defines descriptions of the Basic Interest Rate table IDs to enable the user to identify each one of them easily. |
| 2. | BASIC.INTEREST | Defines and stores the frequently used floating rates accessed by Temenos Transact applications when required. |
| 3. | PERIODIC.INTEREST | Defines the interest rates based on the time period for each currency. |
| 4. | ST.PERIODIC.INTEREST | Acts as an index for PERIODIC.INTEREST . This application can be either manually created or through the ST.CREATE.PERIODIC.INDEX service. |


##### Illustrating Model Products

System table products available in the model bank are given below:

| S.No. | Products | Description |
|---|---|---|
| 1. | SECTOR | 141 – Common Sector 1001 – Individual 1002 – Staff 1002 – Director 2000 – Corporate 3000 - Banks |
| 2. | INDUSTRY | 1000 – Private Person 1050 – Textile and Garments 1200 – Staff 1600 – Non Profit Institutions |
| 3. | CATEGORY | 1000 – Demand Account 1001 – Current Account 1002 – CurrAcc with OD 1003 – Premium C/A |
| 4. | Exit Status | The below values can be held for exit status field: Rejected Deceased Closed Undesirable |


> **Related Applications:** `SYSTEM`

---


---


## Chapter 4: Derivatives_Structured_Products - PT


Derivatives_Structured_Products - PT module of Temenos Transact


### 4.1  PT


> **📇 Quick Reference Card**
> 
> **Purpose:** *Participating Forwards (PF) are Structured Products (SY) wherein a long Foreign Exchange (FX) option and a short FX option are combined to form a composite structure. At each periodical settlement date, either the long option is exercised or the short option is assigned depending on the spot exchang...*
> 
> **Key Fields:** *Agency Booking Model*, *Amount Bought*, *Amount Sold*, *B Apply Leverage*, *B Fixing*, *B Lev Sched Call Amt*, *B Lev Sched Put Amt*, *B Settlement Date* ... +41 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Participating Forwards (PF) are Structured Products (SY) wherein a long Foreign Exchange (FX) option and a short FX option are combined to form a composite structure. At each periodical settlement date, either the long option is exercised or the short option is assigned depending on the spot exchange rate in comparison with the strike price, and hence the investor ends up with a FX spot transaction. If the long option is exercised, the investor makes a profit and if the short option is assigned, the investor incurs a loss.

The underlying options are typically structured with a knock-out feature. When the spot exchange rate breaches this barrier, the option is knocked out. TARKO is an Over-the-Counter (OTC) contract which is similar to the PF. The only difference is that the knock-out barrier is not an exchange rate but rather the intrinsic value of the accumulated profits. In other words, the contract is knocked out, if the intrinsic value of the accumulated profits reaches a pre-determined amount.

Some variants of PF or TARKO can also contain an additional vanilla option which does not have any knock out feature. Temenos Transact is parameterised to handle the entire life cycle of the contract (standard flow) or to work as a back office system (interface flow).

- Full or Standard Flow - Temenos Transact does an end-to-end processing of a PF or TARKO contract, including the creation of underlying currency options. On the fixing date, the system would either Partially exercise the long option (or partially expire the short option) or Partially assign the short option (or partially expire the long option) based on user triggers.
- Interfaced Flow - Where the bank uses external software for life cycle management of a PF or TARKO contract and use Temenos Transact only as a back office system, Temenos Transact does not perform the full processing. Instead, the system fetches the information from external systems and holds them together to form a single Structured Product (SY) contract.

> **⚠️ Note:** The full or standard flow and interfaced flow do not apply for the agency booking model.


##### Product Configuration

The following product configuration is for PF and TARKO.

| S. No | Term Sheet Element | Description |
|---|---|---|
| 1. | Value Date | Effective date of the contract |
| 2. | Currency bought | The currency the investor buys |
| 3. | Currency sold | The currency sold by the investor |
| 4. | Call amount | The amount bought in each settlement period |
| 5. | Put amount | The amount sold in each settlement period |
| 6. | Fixing schedule | Periodical settlement frequency |
| 7. | Strike exchange rate | The strike exchange rate for the option |
| 8. | Knock out price | When this barrier price is breached, the option is knocked out. |
| 9. | Maturity date | Maturity date of the contract |

| S. No | Event | Description |
|---|---|---|
| 1. | Inception | The contract is recorded in the system. The underlying option deals are created. |
| 2. | Fixing | This is the periodical settlement event. The spot exchange rate is compared against the strike exchange rate, the decision is made to either exercise the long option or assign the short option. If the long option is partially exercised, then the short option needs to be partially expired. If the short option is partially assigned, then the long option needs to be partially expired. |
| 3. | Knock out | Both the long option and the short option can have knock-out features. When both the options are knocked out, the contract itself can be knocked out. |
| 4. | Unwinding | The contract can be terminated early. |
| 5. | Maturity | On maturity date, the contract ceases to exist. |

| S. No | Variant | Description |
|---|---|---|
| 1. | PF | In this variant, the PF or TARKO contract gets knocked out when the knock-out barrier is breached. |
| 2. | TARKO | In this variant, the PF or TARKO contract gets knocked out when the accumulated profit reaches a pre-defined level. |
| 3. | With Vanilla option | Some variants include a vanilla option which does not have a knock-out feature. |
| 4. | FX Accumulator or Decumulator | In this variant, the fixing schedule of the long and short option is the same. The notional amount of the short option would be the leveraged notional amount. |


##### Illustrating Model Parameters

The model parameters for Participating Forwards (PT) are explained below:

Participating forwards are SY wherein a long FX Option and a short FX Option are combined to form a composite structure. At each periodical settlement date, either the long option is exercised or the short option is assigned depending on the spot exchange rate in comparison with the strike price, the investor necessarily ends up with a FX spot transaction. If the long option is exercised, the investor makes a profit and if the short option is assigned, the investor incurs a loss.

The underlying options are typically structured with a knock-out feature, when the spot exchange rate breaches this barrier, the option is knocked out.

TARKO is an OTC contract which is similar to the participating forward. The only difference is that the knock-out barrier is not an exchange rate but rather the intrinsic value of the accumulated profits. In other words, the contract is knocked out if the intrinsic value of the accumulated profits reaches a pre-determined amount. Some variants of participating forwards or TARKO can also contain an additional vanilla option, which does not have any knock out feature.

| Field | Description |
|---|---|
| Variant | Refers to a particular variant, then the variant can be linked in this field. Once linked, the parameters and configurations defined for the variant would be used in processing the life cycle of the contract. |
| Currency Bought | Holds the currency that the customer buys |
| Currency Sold | Holds the currency that the customer sells |
| Trade Date | Holds the trade date of the contract. Trade date cannot be forward dated and should fall between the First Date and Last Date of the corresponding product definition record. |
| Maturity Date | Maturity date is the termination date of the contract. Maturity date will be defaulted based on Term and Value Date . |
| Premium Pay Receive | Indicates whether the customer have to pay or receive the premium amount |

| Element | Description |
|---|---|
| Value Date | Effective date of the contract |
| Currency bought | The currency the investor buys |
| Currency sold | The currency sold by the investor |
| Call amount | The amount bought in each settlement period |
| Put amount | The amount sold in each settlement period |
| Fixing schedule | Periodical settlement frequency |
| Strike exchange rate | The strike exchange rate for the option |
| Knock out price | When this barrier price is breached, the option is knocked out. |
| Maturity date | Maturity date of the contract |

| Event | Description |
|---|---|
| Inception | The contract is recorded in the system. The underlying option deals are created. |
| Fixing | This is the periodical settlement event. The spot exchange rate is compared against the strike exchange rate, the decision is made to either exercise the long option or assign the short option. If the long option is partially exercised the short option needs to be partially expired. If the short option is partially assigned the long option needs to be partially expired. |
| Knock out | Both the long option and the short option can have a knock out features, when both the options are knocked out, the contract itself can be knocked out. |
| Unwinding | The contract can be early terminated. |
| Maturity | On maturity date, the contract ceases to exist. |

| Variant | Description |
|---|---|
| PF | In this variant, the Participating Forwards and TARKO contract gets knocked out when the knock out barrier is breached. |
| TARKO | In this variant, the Participating Forwards and TARKO contract gets knocked out when the accumulated profit reaches a pre-defined level. |
| With vanilla option | Some variants include a vanilla option, which does not have a knock out feature. |
| FX Accumulator and Decumulator | In this variant, the fixing schedule of the long and short option is the same. The notional amount of the short option is the leveraged notional amount. |


##### Illustrating Model Products

Model products are not applicable for this module.


#### ⚙️ Configuration

The SY.PRODUCT.DEFINITION application is used to control the functioning and behaviour of a PF or TARKO contract. The events in the life cycle of a PF or TARKO contract is defined in this application. These events cannot be amended by the user. However, the user can amend the other parameters available in this application and also set the category codes and transaction codes required to process a PF or TARKO contract.

The bank can extend the basic definition and create their own variants by setting up the records in SY.PRODUCT.VARIANT application. The ID of this application contains two parts separated by ‘_’. The prefix is the product definition that is being extended, while the suffix refers to the variants. All the parameters defined in the product definition are inherited by the product variant and can be amended. The configuration defined in the product variant takes precedence over the one defined in the product definition.


#### 🔧 Working With

The SY.FX.FORWARDS application is used to transact in the PF or TARKO or FX Accumulator or FX Decumulator contracts.


##### Transaction Booking Model

Temenos Transact supports two types of transaction booking models. The booking model is identified by the Agency Booking Model field in the SY.PRODUCT.DEFINITION and SY.PRODUCT.VARIANT applications. When this field is set to Yes, the agency booking model is enabled and when set to No, the principal booking model is enabled.

| Scenario | Parameter Setup | Underlying Transaction |
|---|---|---|
| 1 | Suppress Underlying is set to No | Long option, short option |
| 2 | Suppress Underlying is set to Yes | Underlying transactions are not created. |

| FOREX fields | Mapped for Customer Leg FX (Transaction against Customer) | Mapped for Counterparty Leg FX(Transaction against Counterparty) |
|---|---|---|
| Buy Currency | Sell Currency | Buy Currency |
| Sell Currency | Buy Currency | Sell Currency |
| Amount Bought | B Lev Sched Put Amt | B Lev Sched Call Amt |
| Amount Sold | B Lev Sched Call Amt | B Lev Sched Put Amt |
| Deal Type | SP | SP |
| Counterparty | Customer | Counterparty |
| Dealer Desk | Dealer Desk | Dealer Desk |
| Value Date Buy | B Settlement Date | B Settlement Date |
| Value Date Sell | B Settlement Date | B Settlement Date |
| Base Ccy | Base Ccy | Base Ccy |

The event processing for a PF or TARKO contract is described in the below sections.

> **⚠️ Note:** For the agency booking model, though the event name refers to the option (Fixing Buy or Fixing Sell and so on), there is no underlying option. Buy refers to the events pertaining to ‘B’ set of fields and sell refers to events pertaining to the ‘S’ set of fields. When Single Schedule is set to Yes, the events pertaining to sell option is inactive, only the buy events are processed. However, the buy events have the logic to process both the buy and sell option.

Fixing is a scheduled event based on the fixing frequency. The long option, short option and the vanilla option could have a different fixing frequency, therefore there are three different fixing events, one per option. Each fixing period is represented by a multi-value set of fields. Before the event is run, the decision to exercise or expire the option needs to be updated in the contract for each option. The Buy Fixing , Sell Fixing , Vanilla Buy Fixing fields is used for this purpose.

If set to exercise, the option would be exercised for the scheduled amounts (the call and put amount for each fixing period) resulting in FX spot deal being generated. If set to expire, the option would be expired for the scheduled amounts.

When the fixing event is processed, the outstanding notional amount gets calculated and appropriate entries are posted. The outstanding notional amount is stored in the Run Notional in Sell Ccy and Run Notional in Buy Ccy fields.

> **⚠️ Note:** 1. Fixing event does not run unless the decision to expire or exercise the option is communicated to the system by updating the contract. There is no default selection, therefore contract needs to be updated with this decision for each option for each fixing period. 2. For contracts where the Single Schedule is set to Yes, the fixing decision is made through B Apply Leverage field. When B Apply Leverage field is set to Yes, the fixing would happen for the leveraged notional amount. When this field is not set, the fixing would be for the notional amount. Therefore, the default fixing would be for the unleveraged notional amount.

It is possible to undo the fixing if the fixing decision has been made erroneously. This can be achieved by using the Buy Undo Fixing, Sell Undo Fixing and Vanilla Buy Undo Fixing fields. Only the last fixing event can be undone, therefore this is not part of a multi-value set of fields.

> **⚠️ Note:** While exercise or expire action would be undone, the underlying FX deal needs to manually reversed.

Both the buy option and sell option can have a knock- out feature. It is possible for one option to be knocked out, while the other option is active. Therefore, there are two separate knock out events, one per option. Vanilla option does not have a knock-out feature.

The knock out field needs to be set to Yes for the corresponding option to trigger the knock out event. (Setting the field would schedule the knock out event to run on that day’s COB).

If the Run Current Fixing field is set to Yes, before knocking out, fixing for the current fixing period would be triggered. The scheduled amounts (only for the fixing period on which knockout occurs) can be amended, the amended amount need not be in terms of the strike price. This feature handles the variants with adjusted strike price. When the knock-out event is run, the outstanding notional amount would be appropriately adjusted.

It is possible to undo a knock-out, if the knock-out has been done erroneously. There are two events (one for the buy option, one for the sell option), which would be triggered when undo flag is set. That is, the event would be scheduled to run on the day the contract is flagged for the undo.

There is a separate event for the contract knock-out. This event runs when both the long option and short option are knocked out and the vanilla option has matured. The contract remains in the active status, even if one of the options is active. Thus, this event is scheduled to run on the day on which all options become inactive.

If this event is run as an ad-hoc event, there would be validation to verify that all options are inactive. This would be a termination event. The notional entries would be reversed.

The contract can be unwound that is, early terminated at any point of time. This is triggered by setting the Unwind field to Yes in the contract. The unwind event would be scheduled to run on the COB of amendment date (date on which the contract is flagged for unwind). This is also a termination event and the notional entries would be dropped.

The contract can be reversed at any point of time. If the reversal is done before the fixing event, the underlying options would also be reversed. If the reversal happens after the fixing (that is, Fixed Status field is updated for any of the options), then the underlying options needs to be reversed manually. FX spot deals generated out of option exercise also needs to be reversed manually.

Limit can be setup for SY.FX.FORWARDS contracts. If set, the limit reference defaults to the Limit Ref field. The SY.FX.FORWARDS application passes on the amount, which is updated in the total outstanding amount in the LIMIT application. The limit is updated at the following stages:

- Inception – contract is booked.
- Fixing – periodical settlement.
- Termination or maturity.

At the time of inception, the limit is updated to the extent of Total Notional in Sell Ccy field. That is, the worst case notional in the sell currency.

At each fixing, the obligation reduces. The outstanding obligation is available in the Run Notional in Sell Ccy field. The limit is updated to reflect the outstanding obligation.

During termination or maturity, the outstanding amount for this contract must be zero.


#### 📋 Tasks

Participating Forwards (PT) are Structured Products wherein a long FX option and a short FX option are combined to form a composite structure.


##### Workflow

This section allows the user to perform the below tasks:

| SCREENS | WORKFLOW |
|---|---|
|  | Trades List . |
| FX Forward/TARKO Trades | Enter values in the required fields and click the FIND button. |
| List of FX Forward/TARKO trades | Click the Edit Trade details icon. |
| FX Forward/ TARKO Input | Enter values in the required fields that require amendment. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Authorise FX Forwards/ TARKO . |
| Unauthorised Trades | Enter values in the required fields and click the FIND button. |
| List of Unauthorised FX Forward/TARKO trades | Select the Amend option from the drop-down and then click the Launch icon. In the FX Forwards/TARKO Input screen, enter values in the fields that require amendment. Click the Validate icon to check for errors and overrides.. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Unwound Trades . |
| List of Unwind Trades | Enter values in the required fields and click the FIND button. |
| List of Unwind FX Forward/TARKO trades | Select the Amend Trade Details option from the drop-down and then click the Launch icon. |
| FX Forwards/TARKO Input | Enter values in the fields that require amendment. Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to Participating Forwards and TARKO in the core banking system.


##### Enquiries and Reports

This section allows the user to view the below list of enquiries and reports:

Back to Back Trades

This enquiry displays the list of all FX forwards and TARKO contracts with back-to-back reference.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


---


## Chapter 5: Derivatives_Structured_Products - SY


Derivatives_Structured_Products - SY module of Temenos Transact


### Features in Derivatives_Structured_Products - SY


| # | Feature | Sections |
|---|---------|----------|
| 5.1 | DigitalInvestments | Intro, Confi |
| 5.2 | Dual and Triple Currency Investments | Intro, Confi |
| 5.3 | Misc | Intro |
| 5.4 | Misc | Intro |
| 5.5 | XF | Intro |
| 5.6 | PT | Intro |
| 5.7 | AccountingValuation | Intro, Confi, Worki, Tasks, Outpu |
| 5.8 | CommonFlow | Intro, Confi, Worki, Tasks, Outpu |
| 5.9 | CommonSetup | Intro, Confi, Worki, Tasks, Outpu |
| 5.10 | CorporateActions | Intro, Confi, Worki, Tasks, Outpu |
| 5.11 | Delivery | Intro |
| 5.12 | Misc | Intro |


### 5.1  DigitalInvestments


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Digital Investment is an OTC Structured Product, which links a traditional money market investment with the purchase of a digital option. The digital investment provides the investor the possibility to profit from an exchange rate and:*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration


#### 📖 Introduction

The Digital Investment is an OTC Structured Product, which links a traditional money market investment with the purchase of a digital option. The digital investment provides the investor the possibility to profit from an exchange rate and:

- If the investor’s view is correct, a higher return is received than a conventional time deposit.
- If the investor’s view is incorrect, the return is less or zero, that is, the cash payout from the digital option is sent as an additional interest on the deposit.

The tower investment is a variant of digital investment. The major difference is that the digital investment has American barriers, that is, the monitoring of the spot exchange rate against the barriers happens continually. The digital and/or tower investment is principal protected, that is, the investor is assured of the investment amount redemption. The SY.DIGITAL.INVEST application records the transaction, which creates the underlying deposit and option based on the configuration. Temenos Transact can be parameterised either to handle the entire life cycle of the contract (standard flow) or to work as a back office system (interface flow).

- Full or Standard Flow - The core banking product does end to end processing of a digital investment, including the creation of the underlying option and deposit.
- Interfaced Flow - The bank uses an external software for the life cycle management of a digital investment contract and use the core banking product only as a back office system. The core banking product does not do the full processing. Instead, the system is designed to get the information from external systems and hold them together to form a single structured product contract.

The events in the life cycle of a digital invest contract are as follows.

| Event | Description |
|---|---|
| Inception | The contract is recorded in the system and the underlying option deal and deposit are created |
| Fixing | The fixing decision is made and the investor receives minimum or maximum rate, depending on the spot exchange rate, in comparison with the upper and lower barriers |
| Maturity | The contract expires on the maturity date and the deposit is redeemed |


#### ⚙️ Configuration

The SY.PRODUCT.DEFINITION application controls the functional and behavioural competencies of a digital investment contract. The events in the digital investment contract life cycle is defined in this application, which cannot be amended by the user. However, the user can amend the other parameters available in this application, and also set the category codes and transaction codes required to process a digital investment contract.

The bank can also extend the basic definition and create their own variants by setting up the records in SY.PRODUCT.VARIANT . The ID of this application contains two parts separated by ‘_’. The prefix is the product definition that is extended, while the suffix refers to the variants. All the parameters defined in the product definition are inherited by the product variant and can be amended. The configuration defined in the product variant takes precedence over the parameters defined in the product definition.

> **⚠️ Note:** The tower investment contracts would typically be a variant.

---


### 5.2  Dual and Triple Currency Investments


> **📇 Quick Reference Card**
> 
> **Purpose:** *Dual Currency Investments (DCI) are structured products that link a traditional Money Market (MM) investment to the sale of a Foreign Exchange (FX) call option on the invested currency or precious metal. The customer receives enhanced interest on the MM deposit. On maturity date, the customer receiv...*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration


#### 📖 Introduction

Dual Currency Investments (DCI) are structured products that link a traditional Money Market (MM) investment to the sale of a Foreign Exchange (FX) call option on the invested currency or precious metal. The customer receives enhanced interest on the MM deposit. On maturity date, the customer receives the redemption amount either in the deposit currency or in the alternate currency. The redemption is in the alternate currency if the currency option is in-the-money from the bank’s perspective.

Triple Currency Investment (TCI) is similar to DCI, the difference is that the presence of a third currency attribute. The redemption might be in deposit currency or in any one of the alternate currencies.

DCI and TCI contracts are not principal protected. When the redemption is in the alternate currency, the investor incurs a loss depending on exchange rate movement and it is possible for such a loss to reduce the principal. Temenos Transact is parameterised to handle the entire life cycle of the contract (standard flow) or to work as a back office system (Interface flow).

- Full or standard flow – Temenos Transact does end-to-end processing of a DCI and TCI contract, including the creation of the underlying deposit and the currency option. On the maturity date, the system either exercises or expires the currency option. The decision to exercise or expire is determined by the user and is communicated to the system by setting the relevant fields. If the option is exercised, the redemption amount from the deposit is converted to the alternate currency by booking an FX spot deal. If the option is expired, then the redemption is in the deposit currency.
- Interfaced Flow - If the banks uses the external software for life cycle management of a DCI and TCI contract and uses Temenos Transact only as a back-office system, then full processing is not done by Temenos Transact . Instead, the system gets the information from external systems and holds them together to form a single SY contract.

> **⚠️ Note:** The full or standard flow and interfaced flow do not apply for the agency booking model.

The terms of a DCI and TCI contract are explained in the following table.

| Term Sheet Element | Description |
|---|---|
| Value Date | Effective date of the deposit |
| Deposit Currency | Currency of the deposit |
| Deposit amount | The principal investment amount |
| Alternate Currency | Alternate currency |
| Strike Exchange Rate | Agreed forward exchange rate between the deposit currency and the alternate currency |
| Interest Rate | Enhanced interest rate for the deposit |
| Fixing date | The date on which the spot exchange rate is compared against the strike price and exercise or expire decision is made |
| Maturity date | Maturity date of the deposit or contract |
| Alternate currency 2 | Applicable for TCI contracts only. This is the other alternate currency |
| Strike exchange rate 2 | Applicable for TCI contracts only. Agreed forward exchange rate between the deposit currency and alternate currency 2 |

The events in the life cycle of a DCI and TCI contracts are explained in the following table.

| Event | Description |
|---|---|
| Inception | The contract is recorded in the system. The underlying deposit and option transaction are created |
| Fixing | Decision event. The spot exchange rate is compared against the strike exchange rate; the user decides whether to exercise or expire the currency option. |
| Maturity | The deposit matures and depending on the fixing decision, the redemption amount is either converted to the alternate currency (through a FX spot deal) or redeemed in the deposit currency. This event would be scheduled to run on the maturity. |
| Unwinding | Unwinding is an early termination event whereby the maturity date can be advanced to an earlier date. |

There are variants of DCI that is traded in the market. Few of these variants are explained in the following table.

| Variant | Description |
|---|---|
| Precious Metal Investments | In this variant, either the deposit currency or the alternate currency is a precious metal defined as a currency in the system |
| DCI with barriers | In this variant, the currency option is a barrier option. Option can have knock-in or knock-out features. In Temenos Transact terms, this is defined as an exotic option |
| Principal only conversion | In this variant, if the option is exercised, then only the principal is converted to the alternate currency. The interest amount is repaid in the deposit currency |
| Tripe Currency Investment | In this variant, there are two alternate currencies. The redemption can be in the deposit currency or in any of the alternate currencies |


#### ⚙️ Configuration

The SY.PRODUCT.DEFINITION parameter application controls the functionality and behaviour of a DCI and TCI contract. The events in the life cycle of a DCI and TCI contract are defined in this application. These events cannot be amended by the user. However, the user can amend the other parameters available in this application and also set the category codes and transaction codes required to process the DCI and TCI contracts.

Banks can also extend the basic definition and create their own variants. This is achieved by setting up records in SY.PRODUCT.VARIANT record. The ID of this application contains two parts separated by an underscore (_). The prefix is the product definition that is being extended, while the suffix refers to the variants. All the parameters defined in the product definition are inherited by the product variant and can be amended. The configuration defined in the product variant takes precedence over the one defined in the product definition.

---


### 5.3  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *Introduction to Retail Sweeping ⓘ Content migrated: Old structure mapped (To be planned)*
> 
> **Key Fields:** *Alternate Ccy 1*, *Alternate Ccy 2*, *Alternate.Ccy.2*, *Exercise Ccy*, *Exercise Ccy,*, *Exercise Expire*, *First Date*, *Last Date* ... +6 more
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Introduction to Retail Sweeping ⓘ Content migrated: Old structure mapped (To be planned)

Related topics:

- Temenos Transact Services

This module handles two business products namely:

- Dual and Triple Currency Investments
- Digital Investments


##### Product Configuration

Read the below configuration sections for setting up the functionality of Dual/Triple Currency and Digital Investments (DI) module.

- Dual and Triple Currency Investments
- Digital Investments


##### Illustrating Model Parameters

The model parameters for Digital Investments (DI) are explained below:

Dual Currency Investments (DCI) are Structured Products (SY) that link a traditional Money Market (MM) investment to the sale of an FX call option on the invested currency or precious metal. The customer receives enhanced interest on the MM deposit. On maturity date, the customer receives the redemption amount either in the deposit currency or in the alternate currency. The redemption is in the alternate currency, if the currency option is in-the-money from the bank’s perspective.

Triple Currency Investment (TCI) is similar to DCI, the difference is that the presence of a third currency attribute. The redemption might be in deposit currency or in any one of the alternate currencies.

DCI and TCI contracts are not principal protected. When the redemption is in the alternate currency, the investor incurs a loss depending on exchange rate movement. It is possible for such a loss to reduce the principal.

| Field | Description |
|---|---|
| Variant | Variant for the contract to use the said categories based on the SY.PRODUCT.VARIANT selected. |
| Trade Date | Holds the trade date of the contract. Trade date cannot be forward dated and should fall between the First Date and Last Date of the corresponding product definition record. |
| Maturity Date | Maturity date is the termination date of the contract. Maturity date will be defaulted based on Term and Value Date . |
| Trade Ccy | This is the deposit currency in which the customer deposit or takes loan in MM.MONEY.MARKET . Is the Trade Ccy of DX.TRADE . |
| Alternate Ccy 1 | The alternate currency in which the deposit amount is paid back, that is, the delivery currency in DX.TRADE and the other currency in FOREX |
| Alternate.Ccy.2 | The second alternate currency in which the deposit amount is paid back, that is, this field enables the triple currency investment. On exercise of option FOREX gets created between Trade Ccy and Alternate Ccy 2 . The option trade between Trade Ccy and Alternate Ccy 1 is expired. |
| Exercise Expire | When the field is set to EXERCISE the option contract is exercised and when set to EXPIRE the option contract is expired. The value to the field can be manually determined. When not the fixing event determines the value to this field. The fixing routine to have 2 parameter which are outcoming. The 1st to hold the EXERCISE or EXPIRE as value saying the decision and the second to hold the Exercise Ccy, if suppose the decision is to exercise the option contract. |
| Exercise Ccy | The currency in which the forex is created when it is Alternate Ccy 1 then the DX.TRADE is exercised. When it is Alternate Ccy 2 then it means the DX.TRADE between trade and first alternate currency is expired and a new FX gets created between Trade Ccy and Alternate Ccy 2 . |

| Element | Description |
|---|---|
| Value date | Effective date of the deposit |
| Deposit currency | Currency of the deposit |
| Deposit amount | The principal investment amount |
| Alternate currency | Alternate currency used |
| Strike exchange rate | Agreed forward exchange rate between the deposit currency and the alternate currency |
| Interest rate | Enhanced interest rate for the deposit |
| Fixing date | The date on which, the spot exchange rate is compared against the strike price and exercise or expire decision is made. |
| Maturity date | Maturity date of the deposit or contract |
| Alternate currency 2 | Applicable for TCI contracts only. This is the other alternate currency. |
| Strike exchange rate 2 | Applicable for TCI contracts only. Agreed forward exchange rate between the deposit currency and alternate currency. |

| Event | Description |
|---|---|
| Inception | The contract is recorded in the system. The underlying deposit and option transaction are created. |
| Fixing | Decision event. The spot exchange rate is compared against the strike exchange rate. The user decides whether to exercise or expire the currency option. |
| Maturity | The Deposit matures and depending on the fixing decision, the redemption amount, is either converted to the alternate currency (through a FX Spot Deal) or redeemed in the deposit currency. This event is scheduled to run on the maturity. |
| Unwinding | Unwinding is an early termination event, where the maturity date can be advanced to an earlier date. |

| Variant | Description |
|---|---|
| Precious metal investments | In this variant, either the deposit currency or the alternate currency, is a precious metal defined as a currency in the system. DCI with barriers - In this variant, the currency option is a barrier option. Option can have knock-in or knock-out features. In Temenos Transact terms, this is defined as an exotic option. |
| Principal only conversion | In this variant, if the option is exercised, then only the principal is converted to the alternate currency. The interest amount is repaid in the deposit currency. |
| Tripe currency investment | In this variant, there are two alternate currencies. The redemption can be in the deposit currency or in any of the alternate currencies. |


##### Illustrating Model Products

Model products are not applicable for this module.

---


### 5.4  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *Introduction to Retail Sweeping ⓘ Content migrated: Old structure mapped (To be planned)*
> 
> **Key Fields:** *Contract Status*, *Daily Units*, *First Date*, *Fixing Frequency*, *Last Date*, *Maturity Date*, *Option Type*, *Product Type* ... +4 more
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Introduction to Retail Sweeping ⓘ Content migrated: Old structure mapped (To be planned)

Related topics:

- Temenos Transact Services

Accumulators allow an investor to accumulate, a fixed quantity of an underlying share at the strike price, on each trading day of the investment period. Accumulators are usually structured with a knock-out feature. This means that the accumulators are terminated, when the price of the underlying share closes at or above a pre-determined barrier price (also known as knock-out price), which is set above the initial spot price. Shares are purchased and accrued on a daily basis. Settlement of aggregate accumulation occurs regularly on pre-determined settlement dates.

On the other hand, decumulators allows the investors to sell a fixed quantity of an underlying share at a pre-determined strike price, on each trading day of the investment period. This forward price is set at a premium to the initial spot price of the underlying share. Decumulators are also structured with a knock-out feature and are terminated early when the price of the underlying share closes at or below a pre-determined barrier. When the price of the underlying share closes at or below the pre-determined barrier price, a knock-out event occurs.


##### Product Configuration

Temenos Transact is parameterised either to handle the entire life cycle of the contract (standard flow) or to work as a back-office system (interface flow).

- Full or standard flow - Temenos Transact does an end-to-end processing of SY.ACCU.DECU including the creation of the underlying option. On each settlement date, the system creates a SEC.TRADE for the accrued units by exercising the option and reduces the outstanding nominal in the option trade. On knock-out or on maturity, the system creates a SEC.TRADE for accrued units and expires the option.
- Interfaced flow - If the banks use other external software for life cycle management of SY.ACCU.DECU and use Temenos Transact only as a back-office system, Temenos Transact does not perform the full processing. Instead, the system is designed to get the information from external systems and hold them together to form a single SY contract. The full or standard flow and interfaced flow do not apply for the agency booking model.

The key terms in accumulator or decumulator contract are explained in the following table.

| Term sheet element | Description |
|---|---|
| Value Date | Commences the contractual obligation from this date |
| Underlying security | Denotes the underlying security which is accumulated or decumulated over the tenor of the contract |
| Strike Price | Denotes the forward price at which the underlying security is purchased or sold |
| Knock out price | Denotes the barrier price. When the spot price of the underlying security breaches this barrier, the contract gets knocked out (terminated). |
| Daily units | Denotes the number of shares that must be accrued on a daily basis |
| Gearing Factor | Applies on the days, when the spot price of the underlying is unfavorable to the investor comparing the strike price |
| Fixing Frequency | Denotes the periodicity at which the settlement of accumulated or decumulated shares occur |
| Maturity Date | Denotes the date on which the contractual obligation ends |

The events in the life cycle of an accumulator or decumulator contract are explained in the following table.

| Event | Description |
|---|---|
| Inception | Commences contractual obligation for the investor. The contract is recorded in the system and the underlying option trade is created. |
| Accrual | Units (of the underlying security) are accrued on a daily basis. For contracts with gearing factor, the gearing factors are applied on the days when the spot price of the underlying is unfavourable to the investor comparing the strike price of the contract. |
| Fixing | Effects the settlement of the accumulated or decumulated shares. The underlying option is exercised and this creates the SEC.TRADE transaction for the underlying security. This is a scheduled periodic event. |
| Knockout | Occurs when the price barrier is breached, that is, when the spot price of the underlying touches the knock-out price. When this event occurs, the contract is terminated. |
| Unwinding | Terminates the contract either fully or partially. In a full unwind, the contract is terminated earlier. In a partial unwind, the contract continues to be active, but the obligation (that is, daily accrual units) is reduced for the rest of the contract period. |
| Novation | Transfers the contract between customers and banks. Internal novation - Contract is transferred from one customer account to another External novation - Contract is transferred from customer account in one bank to another |
| Maturity | Indicates the end date of the contract. The contractual obligation ceases on this date. |

The variants of accumulator or decumulator contracts, prevalent in the market are explained in the following table.

| Variant | Description |
|---|---|
| Non-leveraged accumulator or decumulator | Denotes the plain vanilla accumulator without a gearing factor |
| Leveraged accumulator | Holds an additional attribute that is, gearing factor. Gearing factor is applied to the accrual on the days when the spot price is unfavourable to the customer, comparing the strike price. The potential loss to the investor is higher in this variant, compared to the plain vanilla variant. |
| Guaranteed accumulator or decumulator | Assures the investor of guaranteed accumulation. That is, a certain number of underlying shares might be accumulated or decumulated and settled, even if the knock-out price barrier is breached early in the life of the accumulator contract. |

The following features are available in this product:

For certain emerging markets, off market transfers are prohibited by regulations or policies (for example, Taiwanese shares). Accumulators with such shares as underlying are either cash settled or settled through a participatory note.

The accumulators or decumulators can be cash settled, that is, at the time of fixing, instead of delivering the shares, the cash difference between the strike price and market price can be settled. Strike price is one of the terms of the contract, whereas the market price varies at the time of fixing. Market price can be updated at the time of fixing, based on which Temenos Transact calculates the settlement amount.

Markets can be disrupted due to natural calamities such as typhoon. On such occurrences, the accrual needs to be suspended on that day and resumed once the market is open for trading. The suspension of accrual is updated in the STOCK.EXCHANGE application.

For direct equity transactions, stamp tax is calculated on the trade cost, for equity transactions arising out of accumulators or decumulators, the stamp tax is calculated based on the quantity of units purchased multiplied by the stamp duty price. The stamp duty price is determined as:

Unwind happens anytime during the life cycle of an accumulator or decumulator contract. If unwinding happens in the middle of a fixing period, the customer can settle the shares accumulated in the current fixing period. However, the share settlement takes place only on the subsequent fixing date. Also, the customer can choose not to settle the shares for current fixing period (in such cases, the penalty is higher). It is also possible to do a partial unwinding, that is, reduce the obligation nominals.

There are two types of novation as explained below:

- External novation occurs when the position is transferred outside the bank.
- Internal novation occurs when the position is transferred from one customer account to another customer account (for example, from an individual account of a customer to a joint account).

> **⚠️ Note:** An optional novation fee is also charged.

If the bank acts the principal for the accumulator contract, it can act either as principal or agent for the share settlement, which depends on the type of legal agreement signed with the client and counterparty. Therefore, the Settlement Role field in the SY.ACCU.DECU application accepts the PRINCIPAL or AGENT values. The value in this field is mapped to the share settlement transaction and it is subsequently used for stamp tax calculation.


##### Illustrating Model Parameters

The model parameters for Equity Accumulator (DP) are explained below:

Accumulators allow an investor to accumulate, a fixed quantity of an underlying share at the strike price, on each trading day of the investment period. Accumulators are usually structured with a knock-out feature. This means the accumulators are terminated, when the price of the underlying share closes at or above a pre-determined barrier price (also known as knock-out price), which is set above the initial spot price. Shares are purchased and accrued on a daily basis. Settlement of aggregate accumulation occurs regularly on pre-determined settlement dates.

Decumulators allow an investor to sell a fixed quantity of an underlying share at a pre-determined strike price, on each trading day of the investment period. This forward price is set at a premium to the initial spot price of the underlying share. They are also structured with a knock-out feature and are terminated early, when the price of the underlying share closes at or below a pre-determined barrier. When the price of the underlying share closes at or below the pre-determined barrier price, a knock-out event occurs.

Product definition provides parameterization of the product and connections between units and events. It defines the SY.EVENT (s) that take place throughout a product’s life cycle and the related operations on SY.UNIT (s) that are performed when that event takes place, thus creating a full product life cycle.

The SY.PRODUCT.DEFINITION record ID is the same as the related SY.PRODUCT.DESCRIPTION record. SY.PRODUCT.DEFINITION acts as a template for the SY.PRODUCT record instances that are automatically created per transaction during processing.

The bank can extend the basic product definition and create their own variants. This is achieved by setting up records in SY.PRODUCT.VARIANT application. The ID of this table contains two parts separated by ‘_’. The prefix is the product definition that is being extended, while the suffix refers to the variants. All the parameters defined in the product definition are inherited by the product variant and can be amended at the variant level. Different P and L categories and flags can be set at the variant level. The configuration defined in the product variant takes precedence over the one defined in the product definition.

The product variant can have its own SUB.ASSET.TYPE and PRODUCT.CATEGORY , and these applications are key differentiators useful for reporting purposes.

| Field | Description |
|---|---|
| Product Type | This field indicates this is an accumulator or decumulator contract. |
| Contract Status | The status of the contract is updated in this field. When the contract is created, the status is ACTIVE, subsequently as the contract undergoes various life cycle events, the status is updated as below. |
| Option Type | This field holds the option type of the underlying option. This is auto populated based on the Product Type field. For accumulator contract, the underlying is a PUT option, for decumulator contract, the underlying is a CALL option. |
| Trade Date | This field holds the trade date of the contract. Trade date cannot be forward dated and should fall between the First Date and Last Date of the corresponding product definition record. |
| Maturity Date | Maturity date is the termination date of the contract. Maturity date is defaulted based on Term and Value Date . |
| Daily Units | This field holds the number of units (nominal) to be accrued per day. The value should be a multiple of contract size of the underlying DX.CONTRACT.MASTER . |
| Fixing Frequency | The Accumulator and Decumulator contracts accrue the underlying security on a daily basis. The accrued units are settled periodically (This periodic settlement is known as fixing). |

| Element | Description |
|---|---|
| Value Date | Contractual obligation commences from this date. |
| Underlying security | The underlying security which is accumulated or decumulated over the tenor of the contract. |
| Strike Price | The forward price at which the underlying security is purchased or sold. |
| Knock out price | This is the barrier price, when the spot price of the underlying security breaches this barrier, the contract gets knocked out (terminated). |
| Daily units | The number of shares that must be accrued on a daily basis. |
| Gearing factor | The gearing factor is applied on the days when the spot price of the underlying is unfavourable to the investor when compared to the strike price. |
| Fixing drequency | Settlement of accumulated or decumulated shares occur at this periodicity. |
| Maturity Date | The contractual obligation ends at this date. |

| Event | Description |
|---|---|
| Inception | Contractual obligation commences for the investor. The contract is recorded in the system and the underlying option trade is created. |
| Accrual | Units (of the underlying security) is accrued on a daily basis. For contracts with gearing factor, the gearing factors are applied on those days when the spot price of the underlying is unfavourable to the investor when compared against the strike price of the contract. |
| Fixing | Settlement of the accumulated or decumulated shares are effected through this event. The underlying option is exercised and this creates the SEC.TRADE transaction for the underlying security. This is a scheduled periodic event. |
| Knockout | This event can occur when the price barrier is breached, that is, when the spot price of the underlying touches the knock-out price. When this event occurs, the contract is terminated. |
| Unwinding | The contract can be unwound either fully or partially. In a full unwind, the contract is terminated early. In a partial unwind, the contract continues to be active, but the obligation (that is, daily accrual units) are reduced for the rest of the contract period. |
| Novation | The contract can also be novated, which is transferred from one customer account to another customer account (Internal novation) or transferred to a different bank (external novation). |
| Maturity | It is the end date of the contract. The contractual obligation ceases on this date. |

| Variant | Description |
|---|---|
| Non leveraged accumulator or decumulator | This is the plain vanilla accumulator without a gearing factor. |
| Leveraged Accumulator | This variant has an additional attribute, which is, gearing factor. Gearing factor is applied to the accrual on those days where the Spot Price is unfavorable to the customer, when compared to the strike price. The potential loss to the investor is higher in this variant as compared to the plain vanilla variant. |
| Guaranteed accumulator or decumulator | This variant assures the investor of guaranteed accumulation. That is, a certain number of underlying shares might be accumulated or decumulated and settled, even if the knock-out price barrier is breached early in the life of the accumulator contract. |


##### Illustrating Model Products

Model products are not applicable for this module.

---


### 5.5  XF


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Interest Multiplier Facility (IMF) is a structured or composite product with a pair of term loan in one currency and term deposit in different currencies. The maturity dates of the loan and the deposit are always the same. In case of roll over, the loan and deposit are rolled over as one composi...*
> 
> **Key Fields:** *Ca Impact*, *Cob Phase*, *Early Maturity Date*, *Eb Activity*, *Event*, *First Date*, *Fixing Routine*, *Last Date* ... +8 more
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- Temenos Transact Services

The Interest Multiplier Facility (IMF) is a structured or composite product with a pair of term loan in one currency and term deposit in different currencies. The maturity dates of the loan and the deposit are always the same. In case of roll over, the loan and deposit are rolled over as one composite product. The loan funds the deposit and the redemption of the deposit repays the loan at maturity. The risk lies in the FX rate fluctuation between the loan and deposit currencies.


##### Product Configuration

Temenos Transact can be parameterised to handle the entire life cycle of the contract (standard flow) or to work as a back office system (interface flow).

- Full or Standard Flow - Temenos Transact does an end to end processing of an IMF, including creation of the underlying loan and deposit.
- Interfaced Flow - The bank uses an external software for the life cycle management of an IMF contract and use Temenos Transact only as a back office system. The Temenos Transact does not do the full processing. Instead, the system is designed to get the information from external systems and hold them together to form a single structured product contract.

The events in the IMF contract life cycle are shown in the below table.

| Event | Description |
|---|---|
| Inception | The contract is recorded in the system. The underlying option deals are created |
| Rollover | Roll over of the contract |
| Maturity | On maturity date, the contract ceases to exist |

The terms of an IMF contract are given in the below table.

| Term Sheet Element | Description |
|---|---|
| Value Date | Indicates the effective date of the contract |
| Deposit Currency | Indicates the currency of the deposit |
| Deposit Amount | Indicates the amount of the deposit in deposit currency |
| Loan Currency | Indicates the currency of the loan |
| Loan Amount | Indicates the loan amount in loan currency |
| Deposit Interest Rate | Indicates the interest rate for the deposit |
| Loan Interest Rate | Indicates the interest rate for the loan |
| Maturity Date | Indicates the maturity date of the contract |


##### Illustrating Model Parameters

The model parameters for Interest Multiplier Facility (IMF) are explained below:

IMF is a structured or composite product consisting of a pair of term loan in one currency and a term deposit in another currency. The maturity dates of the loan and the deposit are always the same. In case of roll over, the loan and deposit are rolled over as one composite product. The loan funds the deposit, at maturity and the redemption of the deposit repays the loan. The risk here lies in the FX rate fluctuation between the loan currency and deposit currency.

Rollover can be a manual rollover before a maturity or the contract can be set up to rollover automatically. At the rollover time, it is possible to increase or decrease the loan or deposit amount. It is also possible to change the interest rate on the loan or the deposit. Temenos Transact can be parameterised to handle the entire life cycle of the contract (standard flow) or to work as a back office system (interface flow).

Unwinding or early termination can be effected by updating the Early Maturity Date field. Early termination might attract an unwinding charge or penalty, which is updated in the field Unwind Chg Amt.

| Field | Description |
|---|---|
| Valuation Routine | Values the structured product based on the routine attached |
| Sweep Acct | System sweeps the transactions automatically from the customer segregated account to the customer source account, when this field is set to Yes |
| Sy Exclude Valuation | Reports the structured product deal only when this field is set to Yes. Otherwise, all transactions created by the structured product along with the structured product deal will be displayed. |
| Event | Displays the list of events that can occur in the product life cycle such as CREATE, INPUT, AUTHORISE, ROLLOVER etc and each event can be mapped with dependencies |
| Eb Activity | Invites the user to specify events that requires any delivery message(s) to be invoked |
| Cob Phase | Indicates the COB stage in which the associated event will be processed. For scheduled and/or rolling events the close of business processing will be invoked. |
| First Date and Last Date | Indicates the first and last date on which a deal for this product can be accepted into the system |
| Suppress Underlying | Denies the system from creating underlying transactions, when set to Yes and when set to No the underlying transactions are not suppressed and is created from the structured product contract. The life cycle events of the product is processed by Temenos Transact . |
| Sub Asset Type | Maps the valid record in Sub Asset Type with the application possibly |
| Fixing Routine | Holds a value only if Supress Underlying is set to No. Validation routines can be attached for fixing. |
| Mtm Routine | Facilitates attaching a routine for MTM (Mark to Market) or the user can manually define it by mentioning the categories |
| Ca Impact | Indicates whether Corporate Action is applicable or not for this definition |


##### Illustrating Model Products

Model products are not applicable for this module.

---


### 5.6  PT


> **📇 Quick Reference Card**
> 
> **Purpose:** *Participating Forwards (PF) are Structured Products (SY) wherein a long Foreign Exchange (FX) option and a short FX option are combined to form a composite structure. At each periodical settlement date, either the long option is exercised or the short option is assigned depending on the spot exchang...*
> 
> **Key Fields:** *Currency Bought*, *Currency Sold*, *First Date*, *Last Date*, *Maturity Date*, *Premium Pay Receive*, *Term*, *Trade Date* ... +2 more
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Participating Forwards (PF) are Structured Products (SY) wherein a long Foreign Exchange (FX) option and a short FX option are combined to form a composite structure. At each periodical settlement date, either the long option is exercised or the short option is assigned depending on the spot exchange rate in comparison with the strike price, and hence the investor ends up with a FX spot transaction. If the long option is exercised, the investor makes a profit and if the short option is assigned, the investor incurs a loss.

The underlying options are typically structured with a knock-out feature. When the spot exchange rate breaches this barrier, the option is knocked out. TARKO is an Over-the-Counter (OTC) contract which is similar to the PF. The only difference is that the knock-out barrier is not an exchange rate but rather the intrinsic value of the accumulated profits. In other words, the contract is knocked out, if the intrinsic value of the accumulated profits reaches a pre-determined amount.

Some variants of PF or TARKO can also contain an additional vanilla option which does not have any knock out feature. Temenos Transact is parameterised to handle the entire life cycle of the contract (standard flow) or to work as a back office system (interface flow).

- Full or Standard Flow - Temenos Transact does an end-to-end processing of a PF or TARKO contract, including the creation of underlying currency options. On the fixing date, the system would either Partially exercise the long option (or partially expire the short option) or Partially assign the short option (or partially expire the long option) based on user triggers.
- Interfaced Flow - Where the bank uses external software for life cycle management of a PF or TARKO contract and use Temenos Transact only as a back office system, Temenos Transact does not perform the full processing. Instead, the system fetches the information from external systems and holds them together to form a single Structured Product (SY) contract.

> **⚠️ Note:** The full or standard flow and interfaced flow do not apply for the agency booking model.


##### Product Configuration

The following product configuration is for PF and TARKO.

| S. No | Term Sheet Element | Description |
|---|---|---|
| 1. | Value Date | Effective date of the contract |
| 2. | Currency bought | The currency the investor buys |
| 3. | Currency sold | The currency sold by the investor |
| 4. | Call amount | The amount bought in each settlement period |
| 5. | Put amount | The amount sold in each settlement period |
| 6. | Fixing schedule | Periodical settlement frequency |
| 7. | Strike exchange rate | The strike exchange rate for the option |
| 8. | Knock out price | When this barrier price is breached, the option is knocked out. |
| 9. | Maturity date | Maturity date of the contract |

| S. No | Event | Description |
|---|---|---|
| 1. | Inception | The contract is recorded in the system. The underlying option deals are created. |
| 2. | Fixing | This is the periodical settlement event. The spot exchange rate is compared against the strike exchange rate, the decision is made to either exercise the long option or assign the short option. If the long option is partially exercised, then the short option needs to be partially expired. If the short option is partially assigned, then the long option needs to be partially expired. |
| 3. | Knock out | Both the long option and the short option can have knock-out features. When both the options are knocked out, the contract itself can be knocked out. |
| 4. | Unwinding | The contract can be terminated early. |
| 5. | Maturity | On maturity date, the contract ceases to exist. |

| S. No | Variant | Description |
|---|---|---|
| 1. | PF | In this variant, the PF or TARKO contract gets knocked out when the knock-out barrier is breached. |
| 2. | TARKO | In this variant, the PF or TARKO contract gets knocked out when the accumulated profit reaches a pre-defined level. |
| 3. | With Vanilla option | Some variants include a vanilla option which does not have a knock-out feature. |
| 4. | FX Accumulator or Decumulator | In this variant, the fixing schedule of the long and short option is the same. The notional amount of the short option would be the leveraged notional amount. |


##### Illustrating Model Parameters

The model parameters for Participating Forwards (PT) are explained below:

Participating forwards are SY wherein a long FX Option and a short FX Option are combined to form a composite structure. At each periodical settlement date, either the long option is exercised or the short option is assigned depending on the spot exchange rate in comparison with the strike price, the investor necessarily ends up with a FX spot transaction. If the long option is exercised, the investor makes a profit and if the short option is assigned, the investor incurs a loss.

The underlying options are typically structured with a knock-out feature, when the spot exchange rate breaches this barrier, the option is knocked out.

TARKO is an OTC contract which is similar to the participating forward. The only difference is that the knock-out barrier is not an exchange rate but rather the intrinsic value of the accumulated profits. In other words, the contract is knocked out if the intrinsic value of the accumulated profits reaches a pre-determined amount. Some variants of participating forwards or TARKO can also contain an additional vanilla option, which does not have any knock out feature.

| Field | Description |
|---|---|
| Variant | Refers to a particular variant, then the variant can be linked in this field. Once linked, the parameters and configurations defined for the variant would be used in processing the life cycle of the contract. |
| Currency Bought | Holds the currency that the customer buys |
| Currency Sold | Holds the currency that the customer sells |
| Trade Date | Holds the trade date of the contract. Trade date cannot be forward dated and should fall between the First Date and Last Date of the corresponding product definition record. |
| Maturity Date | Maturity date is the termination date of the contract. Maturity date will be defaulted based on Term and Value Date . |
| Premium Pay Receive | Indicates whether the customer have to pay or receive the premium amount |

| Element | Description |
|---|---|
| Value Date | Effective date of the contract |
| Currency bought | The currency the investor buys |
| Currency sold | The currency sold by the investor |
| Call amount | The amount bought in each settlement period |
| Put amount | The amount sold in each settlement period |
| Fixing schedule | Periodical settlement frequency |
| Strike exchange rate | The strike exchange rate for the option |
| Knock out price | When this barrier price is breached, the option is knocked out. |
| Maturity date | Maturity date of the contract |

| Event | Description |
|---|---|
| Inception | The contract is recorded in the system. The underlying option deals are created. |
| Fixing | This is the periodical settlement event. The spot exchange rate is compared against the strike exchange rate, the decision is made to either exercise the long option or assign the short option. If the long option is partially exercised the short option needs to be partially expired. If the short option is partially assigned the long option needs to be partially expired. |
| Knock out | Both the long option and the short option can have a knock out features, when both the options are knocked out, the contract itself can be knocked out. |
| Unwinding | The contract can be early terminated. |
| Maturity | On maturity date, the contract ceases to exist. |

| Variant | Description |
|---|---|
| PF | In this variant, the Participating Forwards and TARKO contract gets knocked out when the knock out barrier is breached. |
| TARKO | In this variant, the Participating Forwards and TARKO contract gets knocked out when the accumulated profit reaches a pre-defined level. |
| With vanilla option | Some variants include a vanilla option, which does not have a knock out feature. |
| FX Accumulator and Decumulator | In this variant, the fixing schedule of the long and short option is the same. The notional amount of the short option is the leveraged notional amount. |


##### Illustrating Model Products

Model products are not applicable for this module.

---


### 5.7  AccountingValuation


> **📇 Quick Reference Card**
> 
> **Purpose:** *Structured Products (SY) are pre-packaged investment products, wherein multiple components are combined to form a composite structure. This feature explains the various accounting entries and valuation models, which are possible in a SY deal.*
> 
> **Key Fields:** *Counterparty deal*, *Deal Reference*, *Eb Contract Balance*, *Estimation*, *MTM Amount*, *Mtm Amount*, *Mtm Required*, *Notional Diff* ... +10 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Structured Products (SY) are pre-packaged investment products, wherein multiple components are combined to form a composite structure. This feature explains the various accounting entries and valuation models, which are possible in a SY deal.


#### ⚙️ Configuration

Read the Common Setup feature document for more information.


#### 🔧 Working With

This section explains the various accounting, valuation strategies and stages in SY.


##### Initial Funding

The initial funding is debited from the customer's account and posted to an internal wash account, for the SYs that has an underlying deposit. Then the underlying MM is funded from this internal account. Thus, the accounting entry for the customer have only the structure reference and not reference from the underlying deposit. Similarly at the time of deposit maturity, the MM posts the funds to the internal account, and subsequently the same is posted to the customer's account with the structure reference. That is, the customer can view the structure deal as a single transaction rather than a collection of underlying component trades.

> **⚠️ Note:** The initial debit from the customer account happens immediately after the contract is authorised.

The typical accounting flow of SY is shown in the below screenshot.

From a general ledger perspective, the underlying contracts are reported as individual trades, which is essential from a regulatory reporting point as well as for risk monitoring purposes. This highlights that the customer is provided with a single instrument view, but the bank can view the SYs as the component deals and position.


##### Contingent Off-balance Sheet Entries

Structured Products are over-the-counter (OTC) in nature, with the bank acting as principal. In other words, the bank is one of the parties to the transaction. The bank can either take a position against the customer/counterparty, or hedge it through a separate street-side transaction. The off-balance sheet (contingent) entries for the notional amount must be posted for the bank’s own book position, for the SYs having a derivative component. The same is reversed at the time of contract maturity.

This is controlled by the Notional Entries field in the SY.PRODUCT.DEFINITION application. This field must be set to Yes for the system to post off-balance sheet entries. The notional amount varies from product to product, the user can input the notional amount overriding the system calculation.

The notional amount of a SY contract can undergo a change during the life cycle of the contract. In such cases, the notional entries must be re-posted. These entries can be reversed and rebooked, or an adjustment entry can be posted. This is controlled by the Notional Diff field in the SY.PRODUCT.DEFINITION application.


##### Mark to Market Entries

The SY contract is marked to market on a daily basis and Mark to Market (profit or loss) entry is posted for the bank’s own position. The balance sheet side of the Mark to Market (MTM) is posted to either an internal account or as a RE.CONSOL.SPEC.ENTRY based on the set-up in the SY.PRODUCT.DEFINITION application.


##### Illustrating Premium and Commission

Other transaction level accounting entries, such as premium fees would be posted with the structure reference. Profit and Loss categories for these accounting entries are defined at the individual product definition records.

| Cr/Dr | Account/Contract Balance | Amount | Reference | Note |
|---|---|---|---|---|
| Dr | 28142 | 100,000 | SY1520368897 | STMT.ENTRY |
| Cr | USD SY Category Wash Acct | 100,000 | SY1520368897 | STMT.ENTRY |
| Dr | USD SY Category Wash Acct | 100,000 | MM0033900019 | STMT.ENTRY |
| Cr | MM0033900019 | 100,000 | MM0033900019 | RE.CONSOL.SPEC.ENTRY |


##### Illustrating Valuation and MTM Accounting

The following are the various valuation and accounting types in SY.

SY valuations are performed by Temenos Transact based on the valuation routine defined in the corresponding SY.PRODUCT.DEFINITION record. If a valuation routine is not defined in SY.PRODUCT.DEFINITION , the generic routine is used. The syProductDefinition.genericValuation routine is a default routine, which performs an aggregation of the underlying trade valuations along with any balance remaining in the Eb Contract Balance field for the SY.TRANSACTION in question.

It is possible to restrict the underlying trades that are aggregated, by defining the components to include in the valuation in Value Units field. For example, the valuation of a SY.DCI can be configured based upon the underlying MM.MONEY.MARKET component, without including the underlying DX.TRADE component. If this field is left blank and the above generic valuation routine is being used, all underlying trades are aggregated for valuation purposes.

It is anticipated that, some SY products has their own method of valuation, wherein a specific valuation routine must be written and added to the relevant SY.PRODUCT.DEFINITION record. The key purpose of the routine is to enable SC.POS.ASSET , SC.VALUATION.EXTRACT and related enquiries to display valuations under the ASSET.TYPE or SUB.ASSET.TYPE SYs. Therefore, a SY contract displays as a single line in the customer’s portfolio valuation.

As a result, the underlying trades of the SY are not displayed individually in the SC.POS.ASSET and SC.VALUATION.EXTRACT records or on the portfolio valuation. For example, an underlying DX.TRADE is not displayed under the DX asset or sub-asset type valuation and it is controlled by setting the Sy Exclude Valuation field to Yes in SY.PARAMETER . If this field is not set in SY.PARAMETER , it can be set at individual product level on the SY.PRODUCT.DEFINITION record.

The exclusion of the underlying trades from the portfolio valuation is automatically flagged on the underlying contracts in the Sy Exclude Val field. The Portfolio Valuation - Cost (SC.VAL.COST) enquiry lists the valuation details and the user can amend the valuation details as shown in the below screenshot.

It is possible to feed the valuation from external sources, when it is provided by the counterparty. Temenos Transact also provides the facility to capture third party valuation. The SYDX.MARKET.VAL application is updated to achieve the third party valuation in Temenos Transact . This accepts the valuation amount for individual deals. Then, the valuation amount is used to update the Estimation field in the SC.POS.ASSET record, which is the key valuation application in the Securities (SC) module.

The SY deals are valued as a single structure. For example, SY.DCI creates an underlying MM contract for the deposit and a DX.TRADE for the option leg. The valuation of MM and DX.TRADE is suppressed and the SY deal alone is shown in the customer portfolio. The SYDX.MARKET.VAL application records the valuation for a SY deal or a DX contract. The fields in this application are explained below:

- Record ID - Indicates the unique or common reference and date. The unique reference can also be an external reference.
- Deal Reference - Holds the SY deal number or DX.TRADE ID.
- Valuation Currency - Specifies the currency associated with the valuation amount.
- Valuation - Specifies the valuation amount in the associated valuation currency.
- Valoren No - Indicates the unique number assigned to the equity underlying structures (for example, by Telekurs), which is subsequently used for pricing data.
- Price - Indicates the valuation derived from the price and quantity or lot size, when price per unit is available for equity underlying structures and options.
- Trade date - Indicates the date of the trade or deal.
- Counterparty deal - Indicates the back-to-back deal number. This field is blank for counterparty deal.
- MTM Amount - Holds the MTM amount for DX component.

As the date is the valuation date, for each SY deal or DX trade, there is a record for each day where valuation is received. This facilitates the maintenance of valuation and price history. Records are created in this application when the SY deal or the DX trade is committed with the ID and a unique reference trade date.

The valuation amount entered by the user is used to update the Estimation field in SC.POS.ASSET . When a record does not exist for a particular day, the valuation from the last available record is used to update the SC.POS.ASSET record.

It is also possible to enter the valuation only for the street-side of the deal and derive the customer side valuation from the street-side. This feature is useful when there is many to one hedge. That is, many customer legs are covered by a single street-side leg and valuation is received from the counterparty, only for the street-side leg.

The valuation for SY deals can be updated in three ways. They are prioritised as follows:

1. Valuation entered in or interfaced into the SYDX.MARKET.VAL application.
2. Valuation updated through a valuation routine attached in the SY.PRODUCT.DEFINITION record.
3. Summation of the valuation of underlying contracts.

> **⚠️ Note:** If the DX.TRADE is part of a SY structure, the SY deal reference is stored and not the DX.TRADE ID reference. In case of direct DX.TRADE s, the DX.TRADE ID is stored.

Price per unit can be a negative value for the some products. For example, in equity accumulators, when the position is unfavorable to the customer, the valuation and price can be a negative value. The SY contracts and DX.TRADE are bilateral. That is, the contract is between the two parties. The valuation amount updated in this application must be from the customer’s perspective for the SY contract and from the buyer’s perspective for a DX trade.

If the SY deal (equity accumulator) is entered between the customer and the dealer book, then the valuation amount entered (for example, -10 USD) in this application is from the customer perspective. That is, the customer is having an unrealised loss of 10 USD and the dealer book which is having an opposing position has an unrealised profit of 10 USD.

The bank’s own book is one of the parties of any SY contract for OTC contracts. The customer side transaction are hedged by the bank through a street-side transaction with an external counterparty. The booking model is as below:

- Customer vs dealer book.
- Dealer book vs counterparty.

The hedge can be a one-to-one transaction, that is, for each customer leg, there can be a street-side transaction. It is also possible to have a many-to-one hedge, that is, many customer leg transactions are hedged by a single street leg transaction.

Thus, the bank has a position against the customer and an opposite position with the counterparty. MTM accounting entries must be posted to record the unrealised P&L of the bank. While unrealised P&L are posted to the P&L category, the other side is posted to the balance sheet (either to a suspense account or a SPEC entry).

The MTM amount which is the unrealised P&L is derived from the valuation and stored in the Mtm Amount field in the SYDX.MARKET.VAL application (this Mtm Amount is from the bank’s perspective). The MTM related fields are available in SY.PRODUCT.DEFINITION and SY.PRODUCT.VARIANT applications.

MTM accounting can be switched on or off using the Mtm Required field. P&L category (for unrealised P&L) and the internal category (balance sheet side) can also be specified. If the internal account is not specified, then a SPEC entry is generated. For the SY products which include a deposit component, the unrealised P&L is derived from the valuation amount by subtracting the deposit portion (principal + accrued interest) from the valuation amount.


#### 📋 Tasks

There are no Tasks available for Accounting and Valuation feature.


#### 📊 Outputs

There are no Outputs available for Accounting and Valuation feature.

---


### 5.8  CommonFlow


> **📇 Quick Reference Card**
> 
> **Purpose:** *Every Structured Product (SY) has its own application for capturing the contract. These applications are described within each product. This feature describes the common properties shared by all SYs.*
> 
> **Key Fields:** *Acct With Bank Bic*, *Acct With Bank Customer*, *Acct With Bank Swift Addr*, *Alt Ccy Ben Acct*, *Alt Ccy Ben Bank*, *Alt Ccy Cpty Add*, *Alt Ccy Cpty No*, *Alt Ccy Intr Add* ... +88 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Every Structured Product (SY) has its own application for capturing the contract. These applications are described within each product. This feature describes the common properties shared by all SYs.


#### ⚙️ Configuration

This topic explains the configuration of SY as detailed in the Introduction of SY module.


#### 🔧 Working With

This section explains the following:

- Inputting a SY contract
- Processing trade
- Underlying trades
- Illustrating activity log
- Illustrating audit trail
- Defining constraints
- Defining customer position and
- Reporting error


##### Inputting a SY Contract

The trade entry screen for a product is designed to be straight forward and only contain information that pertains to the instrument being traded. This screen is the only screen that the user must address to enter a trade.

On entering a new deal the data is validated to ensure it is consistent with the requirements of the product as defined in the respective product definition. If there were any overrides or messages from the underlying components these are reported along with the overrides from the SY contract itself. The SY.ACCU.DECU application with an override being displayed is shown in the below screenshot.

On committing the SY.ACCU.DECU record successfully, a SY.TRANSACTION record is created. The core system recognises the contract by referring this SY.TRANSACTION record. All accounting entries carry this reference and the SY.TRANSACTION reference is stored in the contract as well.

The following sections cover the processing of the SY contracts in detail:


##### Processing Trade

When a product is traded, an instance of each of the product’s key definition is created for that transaction, along with a full log of the activity that has taken place as explained in the below screenshot.

Each SY.PRODUCT.DEFINITION provides the tracking functionality, which depends on the value in the Tracking field. This allows the underlying deal properties ( SY.PRODUCT , SY.EVENT and SY.UNIT ) to be edited, if required. The following are the options in the Tracking field in SY.PRODUCT.DEFINITION .

- If the Tracking field is set to Yes, the underlying deal properties cannot be amended and the related SY.PRODUCT.DEFINITION records are tracked.

- If the Tracking field is set to No, the deal properties are created as a copy of the related SY.PRODUCT.DEFINITION records and can be amended (if required). This provides the facility to make amendments for individual transactions, if they are required to deviate from the pre-configured product.

The following sections describe the records that are created when a SY contract is input and thus represents the life cycle of the trade.

Events are the key components of a product and defines the product life cycle. The Temenos Transact SY framework is a simple way of defining multiple events as required (based on Temenos Transact system events) and can be re-used or applied to a single product.

The SY.EVENT application provides a view to each event that has taken place or will take place during the SY trade life cycle, this also includes their current status. The ID format of SY.EVENT consists of the SY.EVENT.DEFINITION ID and the SY.TRANSACTION ID.

Creating and authorising a new ACCUDECU contract:

A new ACCUDECU contract is created and authorised. The below screenshots illustrates the life cycle events of this product. A SY.EVENT record is created for each event in the life cycle of this contract. The create and authorise events are already processed, while other events are due for process as per the schedule or on ad hoc basis. The events in an ACCUDECU contract are shown in the below screenshot.

The SY.EVENT application for the ACCUDECU contract is shown in the below screenshot.

Also, the events can run manually from Temenos Transact using the SY.EVENT application by setting the Process Id flag to Yes with only a note required to record the reason for the early or late processing of the event.

When a product is traded, in addition to the creation of the above SY.EVENT record, the related SY.UNIT records are also created for the transaction. The SY.UNIT record provides a view of each of the units of work that are processed or will be processed when the above events take place during the SY trade life cycle. The ID format of the SY.UNIT application consists of SY.UNIT.DEFINITION ID, SY.TRANSACTION ID and the instance of this record.

As all instruments in the SY module are composed of the existing component applications in Temenos Transact , it is possible to decompose or drill through to the trades, which constitute the SYs. These trades are tied to the SYs and cannot be manually amended by a non-SYs event. The product units in SY are shown in the below screenshot.

The user can further drill down to the underlying component to review the details from the above product unit screen. The underlying DX.TRADE related to the ACCUDECU contract is shown in the below screenshot.

The user can identify the deals generated by the SY module as they are stamped with the SY.TRANSACTION and SY.UNIT references.

> **⚠️ Note:** Any override which are approved during the entry of the SYs and the inputter details shown in the Inputter field are the inputter details of the SYs deal.

The SY.TRANSACTION and SY.UNIT references on underlying money market trade are shown in the below screenshot.

> **⚠️ Note:** The users of the vanilla DX.TRADE entry screens cannot make amendments to this deal. This is to avoid the SYs being invalidated.

The SY.PRODUCT provides the following:

- An overall view of the product that has been traded.
- The details of the events that take place throughout the trade life cycle.
- The corresponding operations on units when the event takes place.


##### Underlying Trades

The underlying trades linked to SYs are handled and processed through the standard processing of their respective modules. However, these trades are identified to be a part of a SY, as they have SY.TRANSACTION and SY.UNIT references recorded on them.

> **⚠️ Note:** It is not possible to update the underlying trades through the vanilla entry screens of the underlying applications. This is to avoid the SY being invalidated


##### Illustrating Activity Log

A series of activity logs are available, that can be used to investigate a SY transaction and provide a view of the following:

- Current status of a trade
- The events that took place during its life cycle

The SY.TRANSACTION is the key activity log and the starting point of a SY contract investigation. The SY.TRANSACTION provides a full audit trail of the events and the related units of work that took place during the SY trade life cycle, which is acquired during the audit. It records the values that are stored against the virtual fields during this time.

The log details stored in the SY.TRANSACTION application can be used to access another level of detail through the SY.EVENT.LOG and SY.UNIT.LOG table. These tables provide the details of the events and the details of the units at the time of processing. The SY.EVENT.LOG and SY.UNIT.LOG updated for a SY contract is shown in the below screenshots.


##### Illustrating Audit Trail

The SY.TXN.LINK and SY.CONTRACT.LINK tables maintain the links between the SY trade, the SY.TRANSACTION record and the underlying contract(s). The SY.TXN.LINK and SY.CONTRACT.LINK updated for a SY contract is shown in the below screenshots


##### Defining Constraints

Constraints may be defined for the input applications, which are used for capturing the SY contracts and for the SY.TRANSACTION records to apply constraints while inputting an event. These constraints can be defined using the standard Temenos Transact Generic Global Constraints functionality.


##### Defining Customer Position

While running the Client Details (CUSTOMER.POSITION) enquiry, the SY trades are displayed as a single line with the SY.TRANSACTION reference. As a result, the underlying trades of the SY are not displayed individually in the enquiry results. For example, an underlying DX.TRADE related to an ACCUDECU contract is not displayed.

This is controlled by setting the Sy Exclude Valuation field to Yes in SY.PARAMETER . If this field is set to No, the Sy Exclude Valuation field can be set at individual product level in the SY.PRODUCT.DEFINITION record.

A global Sy Product Category also needs to be defined in the SY.PARAMETER application. Alternatively, this can also be defined at product level in the SY.PRODUCT.DEFINITION application. The exclusion of the underlying trades from the CUSTOMER.POSITION application is automatically flagged on the underlying contracts using the Sy Exclude Val field. The following screenshot shows the SY positions being displayed in a single line unlike the ones of its component parts.


##### Reporting Error

Any error that occurs during the COB event processing are recorded in the SY.EVENT.ERRORS table. The records in this table refers to the corresponding OFS.REQUEST.DETAIL record, which provides a high-level detail of the errors that has occurred.

The OFS.REQUEST.DETAIL table related to SY errors are cleared during the SY.COB.CLEAR.OFSDET COB job, to avoid a build-up of records in the OFS.REQUEST.DETAIL table.

> **⚠️ Note:** The Maint Message Dets field must be set to Yes and the Det Prefix field must be set to SY in the record in OFS.SOURCE used for the SY processing in order to receive the records in OFS.REQUEST.DETAIL as described above, and subsequently clear them in COB.


##### Generating Payment Order fromSY.ACCU.DECU,SY.DCIandSY.FX.FORWARDS

The counterparty with whom banks enters a contract can be classified into two categories. One of the categories has an account relationship with Temenos Transact bank and the other category does not have an account relationship with Temenos Transact bank. If account relationship is not present, the settlement takes place through Nostro account of the counterparty. If settlement takes place through the Nostro account, the SY.ACCU.DECU , SY.DCI and SY.FX.FORWARDS applications have the in-built capability to automatically determine the Nostro and generate SWIFT Payment Message (MT202).

However, banks can opt for the settlement of payments through PAYMENT.ORDER application. Under such cases the system:

- Generates a record in PAYMENT.ORDER application by passing the necessary details.
- Suppresses the generation of payment messages by the underlying application through old mechanism.

When Po Application in PWM.PO.PARAMETER is set to either SY.ACCU.DECU , SY.DCI , SY.FX.FORWARDS or ALL, then all payments made to the counterparty from SY.ACCU.DECU application is made through payment order if:

- The counterparty’s account is not a broker’s own Nostro account or cash account or an internal category account other than the Po Susp Categ account
- Pymt Msg Req field is set to Yes and
- A credit has to be made to the counterparty's account

If the counterparty has own cash or Nostro account with the bank, then the account is defaulted. The payment order is raised and the system debits the customer and credits the counterparty account. If the counterparty does not have cash or Nostro account with the bank, and:

- If Temenos Payments is licensed, the system defaults the internal account based on the Po Susp Categ value defined in PWM.PO.PARAMETER .

- If Temenos Payments is not licensed then, the system determines the Nostro from NOSTRO.ACCOUNT and defaults the same in the counterparty account. If Nostro account is not found, then the system generates an error. The customer inputs an account manually and once the Nostro is determined, the system raises a payment order for crediting this Nostro account.

| Fields from SY.ACCU.DECU or PWM.PO.PARAMETER | Fields in PAYMENT.ORDER | Conditional Mapping |
|---|---|---|
| T24 Bank BIC | Ordering Customer Bic | NA |
| Po Susp Categ in PWM.PO.PARAMETER | Debit Account | NA |
| Premium Currency or Unwind Chg Ccy or Delivery Currency | Debit Ccy | Depends on the event type. For example, for unwinding event system maps the Unwind Chg Ccy field |
| Value date | Debit Value Date | NA |
| @ID ( SY.ACCU.DECU Reference) | Ordering Reference | NA |
| Ben Acct | Beneficiary Account No | NA |
| Bic of Beneficiary Bank | Beneficiary Bic | NA |
| Beneficiary Bank | Beneficiary Customer | NA |
| Name of Beneficiary Bank | Beneficiary Name | System maps the name from CUSTOMER application. |
| Bic of Cpty No | Acct With Bank Bic | NA |
| Cpty No | Acct With Bank Customer | NA |
| Cpty Add | Acct With Bank Swift Addr | NA |
| Bic of Intr Bank | Intermed Bic | NA |
| Intr Bank | Intermed Bank Customer | NA |
| Intr Add | Intermed Swift Addr | NA |
| Premium Currency or Unwind Chg Ccy or Delivery Currency | Payment Currency | Depends on the event type. For example, for unwinding event system maps the Unwind Chg Ccy field. |
| Cpty Prem Amt or Cpty Prem Amt + Cpty Fee Amt , Cpty Unwind Chg Amt Cpty Sett Amt | Payment Amount | When the contract is authorised: In case of Agency Model - Cpty Prem Amt + Cpty Fee Amt In case of non-agency model - Cpty Prem Amt In case of Unwinding: Cpty Unwind Chg Amt In case of Fixing roll - Cpty Sett Amt . When Cpty Sett Amt is null, then accumulator = last price - strike price and decumulator = strike price - last price |
| Value Date | Required Credit Value Date | NA |
| NA | Bank to Bank Info | NA |
| NA | Internal Order Details | NA |
| Bank | Order Type | NA |
| Mapped from PWM.PO.PARAMETER if set | Order Initiation Type Payment Category Payment Method Payment Purpose | NA |
| Counterparty Acc or Premium Acc or Unwind Chg Acc or Temenos Payments to determine | Credit Nostro Account | If Counterparty Acc or Premium Acc or Unwind Chg Acc is a Nostro account which does not belong to the counterparty, then system defaults the value in that field. If Counterparty Acc or Premium Acc or Unwind Chg Acc is an internal category account formed using the Po Susp Categ, then system does not populate any value in this field. Temenos Payments determine the nostro account. |
| Bic of Counterparty Acc or Premium Acc or Unwind Chg Acc or Temenos Payments to determine | Receiver Bic | If Counterparty Acc or Premium Acc or Unwind Chg Acc is a Nostro account which does not belong to the counterparty, then system defaults the Bic of these accounts. If Counterparty Acc or Premium Acc or Unwind Chg Acc is an internal category account formed using the Po Susp Categ, then system does not populate any value in this field. Temenos Payments determines the receiver of the message. |

| Fields from SY.DCI | Fields in PAYMENT.ORDER | Conditional Mapping |
|---|---|---|
| T24 Bank BIC | Ordering Customer Bic | NA |
| Po Susp Categ in PWM.PO.PARAMETER | Debit Account | NA |
| Premium Ccy or Unwind Chg Ccy | Debit Ccy | Depends on the event type |
| Value Date | Debit Value Date | NA |
| @ID ( SY.DCI Reference) | Ordering Reference | NA |
| Dep Ccy Ben Acct or Alt Ccy Ben Acct | Beneficiary Account No | NA |
| Bic of Dep Ccy Ben Bank or Alt Ccy Ben Bank | Beneficiary Bic | NA |
| Dep Ccy Ben Bank or Alt Ccy Ben Bank | Beneficiary Customer | NA |
| Name of Dep Ccy Ben Bank or Alt Ccy Ben Bank | Beneficiary Name | System maps the name from CUSTOMER application |
| Bic of Dep Ccy Cpty No or Alt Ccy Cpty No | Acct With Bank Bic | NA |
| Dep Ccy Cpty No or Alt Ccy Cpty No | Acct With Bank Customer | NA |
| Dep Ccy Cpty Add or Alt Ccy Cpty Add | Acct With Bank Swift Addr | NA |
| Bic of Dep Ccy Intr Bank or Alt Ccy Intr Bank | Intermed Bic | NA |
| Dep Ccy Intr Bank or Alt Ccy Intr Bank | Intermed Bank Customer | NA |
| Dep Ccy Intr Add or Alt Ccy Intr Add | Intermed Swift Addr | NA |
| Premium Currency or Unwind Chg Ccy | Payment Currency | NA |
| Premium Amt + Deposit Amt Cpty Prem Amt + Deposit Amt + Cpty Fee Amt Unwind Chg Amt | Payment Amount | When record is authorised Dealer book - Premium Amt + Deposit Amt Agency booking model - Cpty Prem Amt + Deposit Amt + Cpty Fee Amt Unwinding: Unwind Chg Amt |
| Value Date | Required Credit Value Date | NA |
| NA | Bank to Bank Info | NA |
| NA | Internal Order Details | NA |
| Bank | Order Type | NA |
| Mapped from PWM.PO.PARAMETER if set | Order Initiation Type Payment Category Payment Method Payment Purpose | NA |
| Cparty Deposit Acc , Cparty Alt Currency Account 1 , Counterparty Alt Currency Account 2 and Unwind Chg Acc or Temenos Payments to determine | Credit Nostro Account | If the account is a Nostro account which does not belong to the counterparty, then system defaults the value in the respective field. If it is an internal category account formed using the Po Susp Categ, then system does not populate any value in this field. Temenos Payments determines the Nostro account |
| Bic of Cparty Deposit Acc , Cparty Alt Currency Account 1 , Cparty Alt Currency Account 2 and Unwind Chg Acc or Temenos Payments to determine | Receiver Bic | If the account is a Nostro account which does not belong to the counterparty, then system defaults the BIC in the respective field. If it is an internal category account formed using the Po Susp Categ, then system does not populate any value in this field. Temenos Payments determines the receiver of the message |

| Fields from SY.FX.FORWARDS | Fields in PAYMENT.ORDER | Conditional Mapping |
|---|---|---|
| T24 Bank BIC | Ordering Customer Bic | NA |
| Po Susp Categ in PWM.PO.PARAMETER | Debit Account | NA |
| Premium Currency or Fx Payout Currency | Debit Ccy | Depends on the event |
| Value Date | Debit Value Date | NA |
| @ID ( SY.FX.FORWARDS Reference) | Ordering Reference | NA |
| NA | Beneficiary Account No | NA |
| Bic of Cp Bccy Ben Bank or Cp Sccy Ben Bank | Beneficiary Bic | NA |
| Cp Bccy Ben Bank or Cp Sccy Ben Bank | Beneficiary Customer | NA |
| Name of Cp Bccy Ben Bank or Cp Sccy Ben Bank | Beneficiary Name | System maps the name from CUSTOMER application. |
| Bic of Cp Bccy Cpty No or Cp Sccy Cpty No | Acct With Bank Bic | NA |
| Cp Bccy Cpty No or Cp Sccy Cpty No | Acct With Bank Customer | NA |
| Cp Bccy Cpty Add or Cp Sccy Cpty Add | Acct With Bank Swift Addr | NA |
| Bic of Cp Bccy Intr Bank or Cp Sccy Intr Bank | Intermed Bic | NA |
| Cp Bccy Intr Bank or Cp Sccy Intr Bank | Intermed Bank Customer | NA |
| Dep Ccy Intr Addr or Alt Ccy Intr Addr | Intermed Swift Addr | NA |
| Premium Currency or Fx Payout Currency | Payment Currency | Depends on the event. |
| Premium Amt Cpty Premium Amt + Cpty Fee Amt B Settlement Amt B Cpty Sett Amount S Settlement Amt S Cpty Sett Amount Vb Settlement Amt Vb Cpty Sett Amount Unwind Chg Amt Cpty Unwind Chg Amt | Payment Amount | When authorised Dealer book - Premium Amt Agency model - Cpty Premium Amt + Cpty Fee Amt ‘Fixing Buy' / 'Knockout Buy' Dealer book - B Settlement Amt Agency model - B Cpty Sett Amount Fixing Sell / Knockout Sell Dealer book - S Settlement Amt Agency model - S Cpty Sett Amount Fixing Vanila Buy Dealer book - Vb Settlement Amt Agency model - Vb Cpty Sett Amount Unwind Terminator Dealer book - Unwind Chg Amt Agency model - Cpty Unwind Chg Amt |
| Value Date | Required Credit Value Date | NA |
| NA | Bank to Bank Info | NA |
| NA | Internal Order Details | NA |
| Bank | Order Type | NA |
| Mapped from PWM.PO.PARAMETER if set | Order Initiation Type Payment Category Payment Method Payment Purpose | NA |
| Cparty Buy Ccy Acct or Cparty Sell Ccy Acct or Temenos Payments to determine | Credit Nostro Account | If it is a Nostro account which does not belong to the counterparty, then system defaults the value in the field. If it is an internal category account formed using the Po Susp Categ, then system does not populate any value in this field. Temenos Payments determines the Nostro account |
| Cparty Buy Ccy Acct or Cparty Sell Ccy Acct or Temenos Payments to determine | Receiver Bic | If it is a Nostro account which does not belong to the counterparty, then system defaults the BIC of the account holder. If it is an internal category account formed using the Po Susp Categ , then system does not populate any value in this field. Temenos Payments determines the receiver of the message. |

When the banks opt for the settlement of payments through PAYMENT.ORDER application, the system generates a record in PAYMENT.ORDER application by passing the necessary details. The system also records the PAYMENT.ORDER ID in Po Reference field in SY.TRANSACTION application. Once the payments system processes the payment, it generates an appropriate SWIFT (MT202) payment message.

The system raises an accounting entry by debiting the customer account and crediting the Po Susp Categ account from PWM.PO.PARAMETER . Temenos Payments

- Debits the Po Susp Categ account and credit the counterparty’s Nostro account, if the counterparty’s account is passed on from the application

- Determines the counterparty’s account, if it is not passed from the application and then credits the Nostro account by debiting the Po Susp Categ account.

> **⚠️ Note:** Use the payment system ID to view the accounting entries generated by PAYMENT.ORDER application.


#### 📋 Tasks

There are no Tasks available for Common Flow feature.


#### 📊 Outputs

There are no Outputs available for Common Flow feature.

---


### 5.9  CommonSetup


> **📇 Quick Reference Card**
> 
> **Purpose:** *The configuration of a product is the combination of events and units of work to synthesise the features of a Structured Products (SY), using the underlying Temenos Transact modules as the building blocks for that product.*
> 
> **Key Fields:** *Aa Product Group*, *Active*, *Asset Class*, *Asset Type*, *Cr Txn*, *Currency1*, *Currency2*, *Db Txn* ... +17 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The configuration of a product is the combination of events and units of work to synthesise the features of a Structured Products (SY), using the underlying Temenos Transact modules as the building blocks for that product.

SYs are pre-defined and consist of a series of functional elements which include the following:

- Product life cycle event definitions - Describes the possible Temenos Transact events which can happen to a product (for example, create, input, maturity, knock out).
- Product unit definitions - Acts as the mechanism for exposing other Temenos Transact modules to the SY module. It defines the actions or units of work to be performed when an event takes place (including any rules, decisions, calculations and so on).
- Product definitions - Records each SY definition, using elements drawn from the product life cycle event, product unit and product feature tables.

> **⚠️ Note:** The products themselves are pre-configured and the user is restricted to amend the configuration. For example, user cannot add or amend events or units. However, the user can update the category codes, attach API routines and set Yes or No flags.


#### ⚙️ Configuration

This section provides an overview of the SY framework and elaborates the configuration settings required for its functioning. The following are the sequence of steps to configure the SY framework from parameter set up to product configuration.

- Product life cycle overview
- Parameter settings
- Accounting setup
- Unit definition
- Event definition
- Product definition
- Product variant
- Product master

Before using the SY framework, the SY.PARAMETER record needs to be created along with an ACCOUNT.CLASS record with the ID as SYFUND.


##### SY.PARAMETER

The SY.PARAMETER application allows the high-level configuration of the SY module both system wide and company level. A SY.PARAMETER record must exist before company records are created. As per standard Temenos Transact processing, the system prioritises the lookup of configuration data in the following order:

1. Company level parameter
2. System level record

> **⚠️ Note:** For company records, input is not allowed to Sy Id Field , Sy Unit Field , Sy Excl Val Field , Table and Aa Product Group fields. In this instance, the values defined in the corresponding fields on the SYSTEM record are used.

The SY.PARAMETER application includes the definition of the OFS.SOURCE record to be used during processing. The default account settings, a default sub asset type, product category and the underlying Temenos Transact applications that are used as components of SY.

The OFS.SOURCE record attached to SY.PARAMETER must have the following settings:

- Source Type set to GLOBUS.
- Log Detail Level set to NONE.
- Maint Msg Dets set to Y.
- Det Prefix set to SY.

An OFS.SOURCE record is shown in the below screenshot.

The SUB.ASSET.TYPE applied to SY.PARAMETER is linked to an associated Asset Type as shown in the below screenshot.

An example of the CATEGORY defined in the Product Category is shown in the below screenshot.

A product specific category can also be defined at SY.PRODUCT.DEFINITION and SY.PRODUCT.VARIANT level.


##### Accounting Setup

The SY.TRANSACTION related statement entries require designated debit and credit transaction codes to be defined. The Stmt Narr Ref field is recommended to be set to TRANS for these two records. The TRANSACTION records (Debit/Credit transaction) that needs to be setup are illustrated in the below screenshot.

Once these records are created, it must be applied to the corresponding SY.PARAMETER fields Cr Txn and Db Txn as shown in the below screenshot.

In addition to the above settings, an SY.CATEGORY and ACCOUNT.CLASS record with the ID as SYFUND must be defined along with a related internal account (example, in local currency) per company. The ACCOUNT.CLASS record defines the CATEGORY to be used for the internal accounts required for the SY accounting process. A CATEGORY record is shown in the below screenshot.

The SYFUND definition in an ACCOUNT.CLASS record is shown in the below screenshot.

An internal record is shown in the below screenshot.

Additional internal accounts that does not already exist are automatically created during trade processing and are based on the pre-existing internal account.

The underlying component deals of a SY uses this account, whereas the customer are not exposed to underlying component deals. That is, this account acts as a wash through account between structure and the component deals.


##### Unit Definition

The SY.UNIT.DEFINITION application defines the units of work for specified SY.

A unit represents a component part of a SY and is usually a deal, through an existing Temenos Transact application or version. It can also be a unit of work or piece of processing to be carried out during the product life cycle (for example, an external API call, which passes information to another system). The unit also encapsulates a bi-directional mapping between the SY and the underlying Temenos Transact application or version, that is, it populates the required data on the underlying application.

An operation is triggered on a unit, when an event is processed during the SY life cycle. For example, the input of a new accumulator contract would trigger a unit that creates an underlying DX.TRADE .

These definitions act as a template for the SY.UNIT record instances that are automatically created per transaction during transaction processing.

Units also allows logical data manipulation and calculation through the use of product based variables (virtual fields), which allows the product to gather information from other parts of Temenos Transact without having them captured on the Temenos Transact user input application. This data can then be manipulated in various ways.

Using the product variables it is possible to introduce logic into the processing and filter out units of work, if they are not required under defined conditions.

> **⚠️ Note:** Unit definition is pre-configured, however the user can amend the version used to access the underlying application.


##### Event Definition

The SY.EVENT.DEFINITION application defines the events that take place during the life cycle of a SY (for example, create, input, maturity, knock out, kick in, fixing dates and so on). These definitions act as a template for the SY.EVENT record instances, which are automatically created per transaction during transaction processing.

> **⚠️ Note:** Event definition is pre-configured and cannot be amended. The user can make changes to the individual SY.EVENT instances. That is, the transaction level changes can be made to the event, which overrides the system wide setting defined in the event definition.

Events can map to Temenos Transact functions to other Temenos Transact events and can be defined to be triggered as an ad hoc by the user or an external process.The features that can be applied to events include the following:

- Allow event to run more than once during the life cycle of a single deal.
- Set an event to take place on scheduled dates, at regular frequencies, on an ad hoc basis or at specific stages of the product life cycle.
- Define the last event in a product’s life cycle, after which no events may take place.
- For scheduled and rolling events, define the phase in the COB in which the event takes place.

> **⚠️ Note:** The above example illustrates an adhoc event.

| Event | Description |
|---|---|
| sySystemAuthorise | Generic authorise plug in |
| sySystemAuthoriseReversal | Generic authorise reversal plug in |
| sySystemReverse | Generic reversal plug in |
| sySystemDelete | Generic delete plug in |
| sySystemDeleteAmendment | Generic delete amendment plug in |


##### Product Definition

The SY.PRODUCT.DEFINITION application provides parameterization of the product and connections between units and events. It defines the SY.EVENT (s) that take place throughout a product’s life cycle and the related operations on SY.UNIT (s) that are performed when that event takes place, thus creating a full product life cycle.

The SY.PRODUCT.DEFINITION record ID is the same as the related SY.PRODUCT.DESCRIPTION record. The SY.PRODUCT.DEFINITION record acts as a template for the SY.PRODUCT record instances that are automatically created per transaction during processing.

> **⚠️ Note:** The user has restricted access to the product definition. The user cannot amend the product life cycle (units and events cannot be changed), however the user can set the categories, attach EB.ACTIVITY for advices set as Yes or No and other boolean parameters.

The basic parameters that can be defined on the product include the following:

- Whether the creation of the underlying trades be suppressed.
- Whether the underlying trades be hidden from the portfolio valuation.
- A routine to calculate product valuation.
- A routine to be invoked during event fixing.
- A sub-asset type and product category (these can be defaulted from system wide default).
- Delivery messages.

Any dependencies between events are configured using the Dependency field. For example, a daily event to check whether a contract has kicked out depends on the trade being authorised.

The Active field is associated to the event and specifies whether the event and related dependencies are active. Any events that are inactive, raise an error. The SUB.ASSET.TYPE applied to the product can be defaulted from the system wide SY.PARAMETER setting or a product specific one can be defined. The SUB.ASSET.TYPE is linked to an associated ASSET.TYPE .

The SY.PRODUCT.INTERFACE application provides the link between the SY.PRODUCT.DEFINITION and the input application. Each SY has a unique input application. The link is provided by the Product Definition field in the SY.PRODUCT.INTERFACE .


##### Product Variants

The bank can extend the basic product definition and create their own variants. This is achieved by setting up records in the SY.PRODUCT.VARIANT application. The ID of this application contains two parts separated by '_'. The prefix is the product definition that is being extended, while the suffix refers to the variants. All the parameters defined in the product definition are inherited by the product variant and can be amended at the variant level. Different P&L categories and flags can be set at the variant level. The configuration defined in the product variant takes precedence over the one defined in the product definition.

The product variant can have its own SUB.ASSET.TYPE and Product Category , which are the key differentiators useful for reporting purposes.


##### Product Master

The SY.MASTER application holds the following static information for SY contracts.

| Field | Description |
|---|---|
| Asset Class | Holds the asset class of the underlying. For equity accumulator or decumulator contract, the value is Equity. For FX accumulator or decumulator contract, the value is FX. |
| Mnemonic | Holds the mnemonic, which is an alternative easy mean to reference the master |
| Underlying | Holds the underlying equity instrument. This field is not editable for FX related products, if the Asset Class is not set to Equity. |
| Currency1 | Holds the first currency in the currency pair. This field is not editable for equity products, if the Asset Class is set to Equity. |
| Currency2 | Holds the second currency in the currency pair. This field is not editable for equity products, if the Asset Class is set to Equity. |
| Use Master Sat | Indicates sub asset type associated with this master. This field is used for reporting purposes. |
| Risk Company | Accepts a valid company ID or ALL |
| Risk Level | Holds the product risk rating associated with the underlying of the associated company |

The SY.MASTER record can be linked at the transaction level. The value in the Risk Level field in the SY.MASTER record is defaulted in the respective transaction and can be amended at the transaction level.

The Use Master Sat field in the SY.PRODUCT.DEFINITION and SY.PRODUCT.VARIANT determines the reporting mechanism of SY contracts. When this field is set Yes, the Sub Asset Type (SAT) field defined in SY.MASTER is used for reporting SY contracts. If set to No, the SAT defined in the SY.PRODUCT.VARIANT is used for reporting.


#### 🔧 Working With

This topic is not applicable for this feature.


#### 📋 Tasks

There are no Tasks available for Common Setup feature.


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to Common Setup of structured products base in the core banking system.


##### Enquiries and Reports

This section allows the user to view the below enquiries and reports:

Transaction Overview

This enquiry provides a detailed overview of the structured products related transactions available in the core banking system.

Product Overview

This enquiry provides a detailed overview of the products related to the structured products module in the core banking system.


##### SWIFT Messages

NA


##### Advices

The below list of advices are generated by the core banking system pertaining to each event in the structured products.


##### Alerts

In Common Setup, the user can view the below list of alerts:

The below list of alerts are triggered by the core banking system for the structured products Accumulator and Decumulator.

This alert is triggered by the system after the initiation of a trade.

This alert is triggered by the system when Accu Decu trade is fixed.

This alert is triggered by the system when Accu Decu trade is suspended.

This alert is triggered by the system when Accu Decu trade is exercised.

This alert is triggered by the system when Accu Decu trade is unwound.

This alert is triggered by the system when Accu Decu trade is knocked-in.

This alert is triggered by the system when Accu Decu trade is knocked-out.

This alert is triggered by the system when Accu Decu trade is reversed.

This alert is triggered by the system when Accu Decu trade is accrued for the no of units.

This alert is triggered by the system when Accu Decu trade is blocked.

The below list of alerts are triggered by the core banking system for structured product dual currency investment.

This alert is triggered by the system after the dual currency investment trade is initiated.

This alert is triggered by the system after fixing is done for the dual currency investment trade.

This alert is triggered by the system after the dual currency investment trade is exercised.

This alert is triggered by the system after the dual currency investment trade is unwound.

This alert is triggered by the system after the dual currency investment trade is knocked-in.

This alert is triggered by the system after the dual currency investment trade is knocked-out.

This alert is triggered by the system after the exotics trade is performed for the dual currency investment product.

This alert is triggered by the system after the dual currency investment trade is reversed.

---


### 5.10  CorporateActions


> **📇 Quick Reference Card**
> 
> **Purpose:** *The economic factors of a Structured Product (SY) contract are impacted when the underlying security undergoes a Corporate Action (CA).*
> 
> **Key Fields:** *Applicable Element*, *Back To Back Deal*, *Ca Impact*, *Daily Units*, *Description*, *Diary Type*, *Element*, *Element New Ratio* ... +13 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The economic factors of a Structured Product (SY) contract are impacted when the underlying security undergoes a Corporate Action (CA).

Unlike the Securities CA suite, the processing of CA for SY does not result in a cash or securities movement. The trade economic factors alone undergo a (static) change. For example, the strike price of an Equity Accumulator (DP) needs to be updated to reflect the change in the spot price of the underlying equity, when the equity undergoes a CA event.

The following are the three types of term sheet information that undergoes changes as a result of a CA on the underlying equity:

- Price (like, strike price, knock out price, kick in price and so on)
- Quantity (like, total units, accrued units, lot size and so on)
- Security (underlying security)

The SY.DIARY application is used to process the CA on the underlying security. When a CA is processed through this application, it generates the SY.ENTITLEMENT records for the affected contracts. Once the user reviews the changes and authorises the same in the SY.ENTITLEMENT application, the SY contracts are updated with the modified or changed terms.


#### ⚙️ Configuration

The SYs that are linked to an underlying security are alone affected by the CA on the security. For example, currency linked SY are not impacted by CAs. The term sheet elements that are impacted by CA varies from product to product. The SY.PRODUCT.DEFINITION application indicates whether a particular SY is impacted by CA or not. If there is an impact, the term sheet elements impacted by CA is also defined in this application. The CA related fields in the SY.PRODUCT.DEFINITION application are described below:

- Ca Impact – This field can either be set to Yes or No. Yes - Indicates that this SY is impacted by CA on the underlying equity. For example, DP have value Yes for this field. No - Indicates that this SY is not linked to an equity and therefore not impacted by CA. For example, Dual Currency Investments (DCI) have the value No in this field.
- Applicable Element - Accepts the field name of the term sheet element in the transaction application. For example, in the SY.ACCU.DECU application, the fields might be Knockout Price , Strike Price1 , Strike Price2 , Total Units and so on. The Strike Price1 and Strike Price2 fields are part of an associated multi-value set. This can be multi-valued to capture more term sheet elements. Once this field is updated, it can be inferred that this particular term sheet element might be impacted by a CA on the underlying security.
- Element Type - Indicates whether the field specified in Applicable Element field is a value type or ratio type field. Value type fields are those, which need not be prorated when the value for the customer deal is derived from the back-to-back deal. For example, the Strike Price field need not be pro-rated, as the same strike price is recorded in the customer deal and back-to-back deal. If this field changes in the back-to-back deal, the same value can be updated in the customer deal. Ratio type fields are those, which needs to be prorated when derived from the back-to-back deal. For example, Daily Units is a prorated field. If there are 10 customer deals covered by one back-to-back deal, the Daily Units field in the back-to-back deal and the customer deal is different. When the value in the back-to-back deal changes, the change needs to be prorated on the customer deals.


#### 🔧 Working With

This section explains the workflow of SY Corporate Actions related applications in Temenos Transact .


##### SY.DIARY

This application is used to record the CA on the underlying equity. The important fields in this application are described below:

- Underlying Security - Holds the underlying security that has undergone a CA event. This should be a valid security master ID. All SY contracts that are linked to this security are selected for processing.
- Description - Holds the description of CA.
- Prod Definition - Holds the ID of the SY.PRODUCT.DEFINITION (example, SY.ACCU.DECU ).
- Diary Type - Holds a valid DIARY.TYPE record, indicating the type of CA event.
- Ex Date - All contracts with value date equal to or less than this date would be selected for processing.
- Back To Back Deal - Holds the deal reference of the back-to-back deal number. If this field is populated, then the Element Old Ratio and Element New Ratio fields have no input fields (instead of the ratio, the new changed value can be entered by the user). The user can input the new value of the term sheet element in the New Value field. This is updated on the back-to-back deal and also on the associated customer deals. For example, when the new strike price is input in the field the system updates the strike price on the back-to-back deal and the associated customer deals. For elements of value type such as strike price, knock-out price, the price is updated as it is. That is, the strike price in the back-to-back deal and the customer deals are the same. For elements of ratio type such as total units, accrued units, the new value would be prorated based on the notional amount of the customer deal against the notional amount of the back-to-back deal. This is not a mandatory field. This field is preferably used in situations where many customer deals are hedged or covered by a single back-to-back deal. In such instances, the new value for the affected element (such as, strike price) can be updated for back-to-back deal and the same can be federated for the customer deals. In instances where each customer deal is covered by a counterparty deal (that is, 1 to 1 cover), it is better to use Element Old Ratio and Element New Ratio fields.
- Element - The fields Element to Element New Ratio are part of a multi-value set. For each element defined in the Applicable Element field in SY.PRODUCT.DEFINITION application, there is a multi-value set. That is, the number of multi-value sets are equal to number of elements defined. This field accepts the field name of the element. For example, this could be Knockout Price or Strike Price1 .
- Element New Value - This is a no input field, if Back To Back Deal field is NULL.
- Element Old Ratio - Allows input only if the Back To Back Deal field is NULL. Holds the old ratio value of the element.
- Element New Ratio - Allows input only if the Back To Back Deal field is NULL. Holds the new ratio value of the element. For example, if the element is Strike Price and Element Old Ratio is two, and the Element New Ratio is one, this results in the reduction of strike price by 50%.
- New Security No - Populates only if there is a change in the underlying security. For example, in case of a CA event like stock conversion, the old security is replaced by the new security instrument.


##### SY.ENTITLEMENT

When the SY.DIARY record is processed and the CA service is running, the SY contracts (those contracts with this underlying security) are selected and the SY.ENTITLEMENT records are created. The ID of this application is SY.DIARY ID * Structured Product contract ID. Thus, for each contract selected by the CA service, there is a record in the SY.ENTITLEMENT application.

The ratio input in the SY.DIARY application is used to calculate the new value for each element. The calculated value is updated in SY.ENTITLEMENT for user review. If required, the user can amend the calculated value and authorise the SY.ENTITLEMENT record. Once authorised, the respective SY contract is updated with the new value for each element.


#### 📋 Tasks

A corporate action is an activity or event that brings material change to an organisation and affects its stakeholders. The company’s board of directors generally approve these events. In addition, shareholders are permitted to vote on some events as well.

Corporate Actions are considered as one of the most critical processing for the banks and asset managers. Each investor investing in securities needs to be informed of the Corporate actions occurrences so that investor can make his decisions accordingly. They are classified into three types:

- Mandatory – Affects all the shareholders of the company when the corporate actions is effective in market.
- Voluntary – Only a certain amount of shareholders who voluntarily decides to participate in the event.
- Mandatory with Choice – Affects all the shareholders, but are given with the choice to elect either in cash or stock or reinvested in the form of stock.


##### Workflow

In Accumulators and Decumulators, the user can perform the following activities:

This screen allows the user to record a structured product corporate action event.

Unlike the Securities Corporate Action suite, processing of Corporate Action for Structured Product and Derivatives does not result in a cash movement or securities movement, but only the trade economic factors undergo a (static) change. For example, including a change in strike price of a structure or an Option.

The following items can undergo a change as a result of a Corporate Action on the Underlying Equity.

- Price (Strike Price, Knock out price, Kick in price and so on.)
- Quantity (Total Units, Accrued Units, Lot Size and so on.)
- Security (Underlying Security)

To capture a SY Diary, follow the below steps:

1. Diary Input .
2. In the Input Event Details screen, enter values in the following fields:
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon.

| SCREENS | WORKFLOW |
|---|---|
|  | Unauthorised Entitlements . |
| Unauthorised Entitlements | Click the FIND button. Click the Edit icon corresponding to a record. |
| Entitlement Details | Enter values in the required fields. Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

There are no Outputs available for Corporate Actions feature.

---


### 5.11  Delivery


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Structured Products (SY) module uses standard Temenos Transact soft delivery messages, which can be attached at product level per event. By using the standard Temenos Transact delivery configuration, the records in EB.ACTIVITY can be attached at different stages of the configured product to prod...*
> 
> **Key Fields:** *Account*, *Eb Activity*, *Knock In*, *Knock Out*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

The Structured Products (SY) module uses standard Temenos Transact soft delivery messages, which can be attached at product level per event. By using the standard Temenos Transact delivery configuration, the records in EB.ACTIVITY can be attached at different stages of the configured product to produce specific delivery messages. The SY module exposes the following information to the delivery interface.

| Section | Position | Information |
|---|---|---|
| Input record | 1 | Record from the application used to enter the SY deal |
| Input record | 3 | SY.TRANSACTION record for the deal |
| Input record | 5 | SY.UNIT record (if processing a unit-level message) |
| Input record | 7.1 | Record key of the application used to enter the SY deal |
| Input record | 7.2 | SY.TRANSACTION record key for the deal |
| Input record | 7.3 | SY.UNIT record key (if processing a unit-level message) |
| Input record | 7.4 | SY.EVENT record key |
| Header | 8.1 | Company code |
| Header | 8.2 | Customer company code |
| Header | 8.5 | Currency for the deal, taken from the SY.TRANSACTION record |
| Header | 8.6 | User’s department code |
| Header | 8.7 | Customer (from SY.TRANSACTION ) |
| Header | 8.8 | SY.TRANSACTION record key |
| Header | 8.9 | Language of the customer (from 8.7) |
| Header | 8.10 | Account (from SY.TRANSACTION from the Account field) |
| Header | 8.11 | Value |

The required information can be mapped to the actual message output. The complete configuration of the actual message output format as detailed in the DE.FORMAT.PRINT application can be configured to suit individual requirements.


##### Email Alerts

Email and SMS alerts can be set for SY.ACCU.DECU (Accumulator or Decumulator) and SY.DCI (Dual Currency Investments) applications. Temenos Transact is configured to generate tec items, at the following stages of the product life cycle.

| Event Type | Description | Trigger Point |
|---|---|---|
| Trade initiation | Triggering an email alert on authorisation of SY contract | Authorise (event) - trade authorisation |
| Trade fixing | Fixing event of a SY is processed | Fixing (event) - fixing event is run |
| Trade exercise | Processing exercise event of a SY | Exercise (event) - exercise event |
| Trade expire | Expiration of SY | Mature (event) - expire event |
| Trade reversal | Reversal of SY deal | Reverse (event) - trade reversal |
| Trade amendment | Amendment of SY deal | Amend (event) - trade amendment |
| Knock in | Knocking in the product | Knock in (event) - Knock In set to Yes |
| Knock out | Knocking out the product | Knock out (event) - Knock Out set to Yes |
| Unwinding | Triggering unwinding | Unwinding (event) - unwinding product |
| Rollover | Triggering rollover | Rollover (event) - rollover product |
| Accrual | Accruing underlying units | Accrual (event) - accrue units |
| Corporate actions | Implementing the changes in terms of structure | Amend (event) - Corporate Action (CA) run |

If the relevant email or SMS message record is attached to the EB.ADVICES application and if the customer and DAO customer have subscribed to the same, an email or SMS is triggered.


##### Product Level Setup

The EB.ACTIVITY records can be specified for each event, depending on when the delivery must be produced. In the below example, a delivery message is produced at the time of contract initiation, a different delivery message is produced when the contract is reversed.

Once a SY contract is created, the corresponding SY.PRODUCT record stores the EB.ACTIVITY record IDs in the Eb Activity field, as shown in the below screenshot.

The delivery message references are stored in the SY.EVENT.LOG application, as shown in the below screenshot.

Once the delivery is created, the actual delivery message is viewed using the View Delivery Messages (DE.MSG.SUM) enquiry, as shown in the below screenshot.

The output of the delivery message is shown in the below screenshot.

> **⚠️ Note:** It is possible to attach EB.ACTIVITY to an event in the SY.PRODUCT.DEFINITION application. Also, it is possible to set an EB.ACTIVITY at the SY.PRODUCT.VARIANT level. The EB.ACTIVITY attached to the variant takes precedence over the one attached at the product definition level.

---


### 5.12  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *Introduction to Retail Sweeping ⓘ Content migrated: Old structure mapped (To be planned)*
> 
> **Key Fields:** *Active*, *Asset Class*, *Dependency*, *Min Period Kout*, *Risk Level*, *Sub Asset Type*, *Use Master Sat*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Introduction to Retail Sweeping ⓘ Content migrated: Old structure mapped (To be planned)

Related topics:

- Temenos Transact Services

Structured Products are pre-packaged investment products, wherein multiple components are combined to form a composite structure. These products have potential for high returns and are fraught with risk. They are linked to a market entity such as an equity or a currency pair.

The Structured Products (SY) framework is a part of the core product, while the individual products need to be licensed separately. It provides the support functions such as valuation and corporate action processing for structures. The SYs available in Temenos Transact are listed below:

- Dual or Triple Currency Investments (DI)
- Equity Accumulators And Decumulators (DP)
- Participating Forwards and TARKO (PT)
- Interest Multiplier Facility (XF)

> **⚠️ Note:** The SY module cannot be used, unless the individual products are installed.

The SY module provides the functionality to trade and process the pre-packaged SYs, constructed through the product builder. Although the SY module does not provide the facility to build new products on its own, it provides restricted access to the definition tables.

When a product is traded, an instance of each of the product’s key definition applications are created for that transaction, along with a complete log of the activity that has taken place. This three-tier architecture is employed for all of the key definition applications with the notable exception of the product, which does not have a log file. The log file of the product is denoted by the SY.TRANSACTION application, which is the deal that represents the traded instrument. This is shown in the below screenshot.


##### Product Configuration

The SY.PRODUCT.DEFINITION application provides parameterization of the product and connections between units and events. It defines the SY.EVENT (s) that take place throughout a product’s life cycle and the related operations on SY.UNIT (s) that are performed when that event takes place, thus creating a full product life cycle.

The SY.PRODUCT.DEFINITION record ID is the same as the related SY.PRODUCT.DESCRIPTION record. The SY.PRODUCT.DEFINITION record acts as a template for the SY.PRODUCT record instances that are automatically created per transaction during processing.

> **⚠️ Note:** The user has restricted access to the product definition. The user cannot amend the product life cycle (units and events cannot be changed), however the user can set the categories, attach EB.ACTIVITY for advices set as Yes or No and other boolean parameters.


##### Illustrating Model Parameters

The model parameters for SY are explained below:

The SY.PARAMETER application allows the high level configuration of the SY module, either system wide or at company level. The record "SYSTEM" must exist in this application before any company record is created. As per standard Temenos Transact processing, the system attempts to lookup configuration data from the company-level parameter record first, followed by the system level record.

- Valid Sub Asset Type can be mentioned at company level or at system level
- Categories for the wash transaction can be input at both levels
- Local reference tables can be given at system level not at company level
- Can be mapped to AA product group
- Default currency market can be input for the SY deals
- A product specific category can be defined at SY.PRODUCT.DEFINITION and SY.PRODUCT.VARIANT level.

The SY.MASTER holds the static information for SY contracts. The SY.MASTER record can be linked at the transaction level. The Risk Level from the SY.MASTER defaults in the respective transaction and can be amended at the transaction level.

The Use Master Sat field in the SY.PRODUCT.DEFINITION and SY.PRODUCT.VARIANT determines the reporting mechanism of SY products contracts. When this field is set Yes, the Sub Asset Type (SAT) defined in SY.MASTER is used for reporting SY contracts. If set to No, the SAT defined in the SY.PRODUCT.VARIANT is used for reporting.

- Asset Class to hold the underlying equity or FX.
- For FX currencies can be defined for currency pair.
- Valid Sub Asset Type can be given.
- Risk level can be maintained at company level.

The configuration of a product is the combination of events and units of work to synthesize the features of a SY, using the underlying Temenos Transact modules as the building blocks for that product. The SYs are pre-defined and consist of a series of functional elements which include the following:

Product life cycle event definitions - Describes the possible Temenos Transact events which can happen to a product (for example, create, input, maturity, knock out). Product unit definitions - Acts as the mechanism for exposing other Temenos Transact modules to the SY module. Defines the actions or units of work to perform when an event takes place (including any rules, decisions, calculations, and so on). Product definitions - Records each SY definition, using elements drawn from the product life cycle event, product unit and product feature tables.

The SY.UNIT.DEFINITION application defines the units of work for a specified Structured Product. A unit represents a component part of a Structured Product and is usually a deal through an existing core banking application or screen and can also be a unit of work or piece of processing to be carried out during the product life cycle (for example, an external API call, which passes information to another system). The unit also encapsulates a bi-directional mapping between the Structured Products and the underlying core banking application or screen, that is, it populates the required data on the underlying application.

- An operation on a unit is triggered when an event is processed during the Structured Products life cycle. For example, the input of a new accumulator contract triggers a unit that creates an underlying DX.TRADE .
- Default core banking application has to be mapped for the underlying event.
- EB activity can be mapped accordingly for the advices to be generated.
- Unit definition would be pre-configured. However, the user can amend the screen used to access the underlying application.

The SY.EVENT.DEFINITION application defines the events that take place during the life cycle of a Structured Product, such as, Create, Input, Maturity, Knock out, Kick in, Fixing dates and so on. These definitions act as a template for the SY.EVENT record instances that are automatically created per transaction during transaction processing.

- Allow event to run more than once during the life cycle of a single deal.
- Set an event to take place on scheduled dates at regular frequencies on an ad hoc basis or at specific stages of the product life cycle.
- Define the last event in a product’s life cycle, after which no further events may take place.
- For scheduled and rolling events - define the phase in the COB that the event takes place.

The SY.PRODUCT.DEFINITION provides parameterization of the product and connections between units and events. It defines the SY.EVENT (s) that take place throughout a product’s life cycle and the related operations on SY.UNIT (s) that are performed when that event takes place, thus creating a full product life cycle.

The SY.PRODUCT.DEFINITION record ID is the same as the related SY.PRODUCT.DESCRIPTION record. The SY.PRODUCT.DEFINITION acts as a template for the SY.PRODUCT record instances that are automatically created per transaction during processing. The basic parameters that can be defined on the product include:

- Any dependencies between events are configured using the Dependency field. For example, a daily event to check whether a contract has kicked out depends on the trade being authorised.
- Each attribute of this parameter are specific to the event.
- There are several events which can occur in a product life cycle (for example, CREATE, NEW, REVERSE, ACCURAL etc.). and each event can be mapped with dependencies.
- Each event can be specified if any delivery message(s) to be invoked.
- Can be mapped with the specific Unit definition based on the application SY.UNIT.DEFINITION .
- Valid SUB.ASSET.TYPE record can be mapped with the application.
- Validation routines can be attached.
- User can choose to include or exclude valuation for the event.
- Has the facility to attach a routine for MTM (Mark to Market) or the user can manually define it by mentioning the categories.
- Whether Corporate Action (CA) is applicable or not for this definition.

The Active field is associated to the event and specifies whether this event and related dependencies are active. Any events that are not active raises an error.

The SUB.ASSET.TYPE applied to the product can be defaulted from the system wide SY.PARAMETER setting or a product specific one can be defined. The SUB.ASSET.TYPE is linked to an associated ASSET.TYPE .

The bank can extend the basic product definition and create their own variants. This is achieved by setting up records in SY.PRODUCT.VARIANT application. The ID of this table contains two parts separated by ‘_’. The prefix is the product definition that is being extended, while the suffix refers to the variants. All the parameters defined in the product definition are inherited by the product variant and can be amended at the variant level. Different P and L categories and flags can be set at the variant level. The configuration defined in the product variant takes precedence over the one defined in the product definition.

The product variant can have its own SUB.ASSET.TYPE and PRODUCT.CATEGORY , and these applications are key differentiators useful for reporting purposes.

- Product variant can be defined per each event type.
- All the parameters defined in the product definition are inherited by the product variant and can be amended.
- The Min Period Kout field is relevant only for ACCU and DECU products. Allowed values are YES and NO. When set to YES, the contract is knocked out immediately when set to Knockout. When null or NO, the knockout action takes place only on the protected date.
- Each event can be specified if any delivery message(s) to be invoked.
- Can be mapped with the specific Unit definition based on the application SY.UNIT.DEFINITION .
- Valid SUB.ASSET.TYPE record can be mapped with the application.
- Validation routines can be attached.
- Has the facility to manually define it by mentioning the categories.
- Whether corporate action is applicable or not for this definition.


##### Illustrating Model Products

Model products are not applicable for this module.

---


---


## Chapter 6: Derivatives_Structured_Products - XF


Derivatives_Structured_Products - XF module of Temenos Transact


### 6.1  XF


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Interest Multiplier Facility (IMF) is a structured or composite product with a pair of term loan in one currency and term deposit in different currencies. The maturity dates of the loan and the deposit are always the same. In case of roll over, the loan and deposit are rolled over as one composi...*
> 
> **Key Fields:** *Auto Rollover Term*, *Ca Impact*, *Cob Phase*, *Dep Prin Adjust*, *Early Maturity Date*, *Eb Activity*, *Event*, *Final Maturity Date* ... +15 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Related topics:

- Temenos Transact Services

The Interest Multiplier Facility (IMF) is a structured or composite product with a pair of term loan in one currency and term deposit in different currencies. The maturity dates of the loan and the deposit are always the same. In case of roll over, the loan and deposit are rolled over as one composite product. The loan funds the deposit and the redemption of the deposit repays the loan at maturity. The risk lies in the FX rate fluctuation between the loan and deposit currencies.


##### Product Configuration

Temenos Transact can be parameterised to handle the entire life cycle of the contract (standard flow) or to work as a back office system (interface flow).

- Full or Standard Flow - Temenos Transact does an end to end processing of an IMF, including creation of the underlying loan and deposit.
- Interfaced Flow - The bank uses an external software for the life cycle management of an IMF contract and use Temenos Transact only as a back office system. The Temenos Transact does not do the full processing. Instead, the system is designed to get the information from external systems and hold them together to form a single structured product contract.

The events in the IMF contract life cycle are shown in the below table.

| Event | Description |
|---|---|
| Inception | The contract is recorded in the system. The underlying option deals are created |
| Rollover | Roll over of the contract |
| Maturity | On maturity date, the contract ceases to exist |

The terms of an IMF contract are given in the below table.

| Term Sheet Element | Description |
|---|---|
| Value Date | Indicates the effective date of the contract |
| Deposit Currency | Indicates the currency of the deposit |
| Deposit Amount | Indicates the amount of the deposit in deposit currency |
| Loan Currency | Indicates the currency of the loan |
| Loan Amount | Indicates the loan amount in loan currency |
| Deposit Interest Rate | Indicates the interest rate for the deposit |
| Loan Interest Rate | Indicates the interest rate for the loan |
| Maturity Date | Indicates the maturity date of the contract |


##### Illustrating Model Parameters

The model parameters for Interest Multiplier Facility (IMF) are explained below:

IMF is a structured or composite product consisting of a pair of term loan in one currency and a term deposit in another currency. The maturity dates of the loan and the deposit are always the same. In case of roll over, the loan and deposit are rolled over as one composite product. The loan funds the deposit, at maturity and the redemption of the deposit repays the loan. The risk here lies in the FX rate fluctuation between the loan currency and deposit currency.

Rollover can be a manual rollover before a maturity or the contract can be set up to rollover automatically. At the rollover time, it is possible to increase or decrease the loan or deposit amount. It is also possible to change the interest rate on the loan or the deposit. Temenos Transact can be parameterised to handle the entire life cycle of the contract (standard flow) or to work as a back office system (interface flow).

Unwinding or early termination can be effected by updating the Early Maturity Date field. Early termination might attract an unwinding charge or penalty, which is updated in the field Unwind Chg Amt.

| Field | Description |
|---|---|
| Valuation Routine | Values the structured product based on the routine attached |
| Sweep Acct | System sweeps the transactions automatically from the customer segregated account to the customer source account, when this field is set to Yes |
| Sy Exclude Valuation | Reports the structured product deal only when this field is set to Yes. Otherwise, all transactions created by the structured product along with the structured product deal will be displayed. |
| Event | Displays the list of events that can occur in the product life cycle such as CREATE, INPUT, AUTHORISE, ROLLOVER etc and each event can be mapped with dependencies |
| Eb Activity | Invites the user to specify events that requires any delivery message(s) to be invoked |
| Cob Phase | Indicates the COB stage in which the associated event will be processed. For scheduled and/or rolling events the close of business processing will be invoked. |
| First Date and Last Date | Indicates the first and last date on which a deal for this product can be accepted into the system |
| Suppress Underlying | Denies the system from creating underlying transactions, when set to Yes and when set to No the underlying transactions are not suppressed and is created from the structured product contract. The life cycle events of the product is processed by Temenos Transact . |
| Sub Asset Type | Maps the valid record in Sub Asset Type with the application possibly |
| Fixing Routine | Holds a value only if Supress Underlying is set to No. Validation routines can be attached for fixing. |
| Mtm Routine | Facilitates attaching a routine for MTM (Mark to Market) or the user can manually define it by mentioning the categories |
| Ca Impact | Indicates whether Corporate Action is applicable or not for this definition |


##### Illustrating Model Products

Model products are not applicable for this module.


#### ⚙️ Configuration

The SY.PRODUCT.DEFINITION application controls the functional and behavioural competencies of an IMF contract. The events in the IMF contract life cycle is defined in this application, which cannot be amended by the user. However, the user can amend the other parameters available in this application, and set the category codes and transaction codes required to process an IMF contract.

The bank can also extend the basic definition and create their own variants by setting up records in SY.PRODUCT.VARIANT . The ID of this application contains two parts separated by ‘_’. The prefix is the product definition that is extended, while the suffix refers to the variants. All the parameters defined in the product definition are inherited by the product variant and can be amended. The configuration defined in the product variant takes precedence over the parameters defined in the product definition.


#### 🔧 Working With

The SY.IMF application records the IMF contract and its variants. An IMF contract has an embedded loan and deposit. These deals are created in the system and linked to the IMF contract. Depending on the parameter setup, the following underlying transactions are created automatically by the system.

| Scenario | Parameter Setup | Underlying Transaction |
|---|---|---|
| 1 | Suppress Underlying = No | Loan and deposit created |
| 2 | Suppress Underlying = Yes | No underlying transactions created |

In the standard or full mode of processing, Temenos Transact creates and manages the underlying transactions. This mode can be selected by setting the Suppress Underlying field in SY.PRODUCT.DEFINITION to No. In the interface mode of processing, Temenos Transact creates the structure. The underlying transactions are created by the upstream systems. A common reference or identifier binds the underlying transactions and structure together.


##### Event Processing

The event processing involves the rollover and unwinding of contracts.

An IMF contract can be rolled over, that is, the maturity date can be extended. The rollover can either be principal only or a principal and interest rollover. The rollover can either be manual or automatic. At the time of rollover, it is possible to increase or decrease the loan or deposit amount. It is also possible to change the interest rate on the loan or deposit.

The auto rollover is enabled by updating the Auto Rollover Term field with the rollover frequency. If this field is updated, the contract rolls over until the value set in the Final Maturity Date field. If the Final Maturity Date field is not populated, the contract rolls over indefinitely. To stop the rollover process, the Auto Rollover Term field needs to be cleared, that is, set to null or blank value.

The contract can be rolled over manually by setting the Manual Rollover field to either EXTEND.MATURITY or ROLLOVER. The Maturity Date field is updated with the new maturity date, that is, the maturity date at the end of the rollover period. Both the loan and deposit principal can be adjusted through the Loan Prin Adjust and Dep Prin Adjust fields. The effective date of such an adjustment is the rollover date. The interest rates of the loan and deposit can also be adjusted and the adjustment becomes effective from the rollover date.

The unwinding or early termination is enabled by updating the Early Maturity Date field. The early termination might attract an unwinding charge or penalty, which is updated in the Unwind Chg Amt field.


#### 📋 Tasks

There are no Tasks available for Interest Multiplier Facility feature.


#### 📊 Outputs

There are no Outputs available for Interest Multiplier Facility feature.

---


---


## Appendix A: Glossary of T24 Applications & Fields


This glossary lists all T24/Transact application names and field names referenced throughout this document, with descriptions where available.


### Applications


| Application | Description |
|------------|-------------|
| `ACCOUNT.CLASS` | T24 application: ACCOUNT.CLASS |
| `CURRENCY` | T24 application: CURRENCY |
| `DX.CLOSEOUT` | T24 application: DX.CLOSEOUT |
| `DX.CO.ASSIGN.AUTO` | T24 application: DX.CO.ASSIGN.AUTO |
| `DX.CO.ASSIGN.MANUAL` | T24 application: DX.CO.ASSIGN.MANUAL |
| `DX.CO.EXERCISE.AUTO` | T24 application: DX.CO.EXERCISE.AUTO |
| `DX.CO.EXERCISE.MANUAL` | T24 application: DX.CO.EXERCISE.MANUAL |
| `DX.CO.EXPIRE.MANUAL` | T24 application: DX.CO.EXPIRE.MANUAL |
| `DX.CONTRACT.MASTER` | T24 application: DX.CONTRACT.MASTER |
| `DX.CUSTOMER` | T24 application: DX.CUSTOMER |
| `DX.EXCHANGE.MASTER` | T24 application: DX.EXCHANGE.MASTER |
| `DX.OPTION.TYPE` | T24 application: DX.OPTION.TYPE |
| `DX.ORDER` | T24 application: DX.ORDER |
| `DX.PARAMETER` | T24 application: DX.PARAMETER |
| `DX.PARENT.CONSOLIDATE` | T24 application: DX.PARENT.CONSOLIDATE |
| `DX.PARENT.LOG` | T24 application: DX.PARENT.LOG |
| `DX.PARMATER` | T24 application: DX.PARMATER |
| `DX.TRADE` | T24 application: DX.TRADE |
| `DX.TRANSACTION` | T24 application: DX.TRANSACTION |
| `DX.USR.FLD.OPT` | T24 application: DX.USR.FLD.OPT |
| `FX.COMM.GROUP` | T24 application: FX.COMM.GROUP |
| `FX.GEN.CONDITION` | T24 application: FX.GEN.CONDITION |
| `FX.GROUP.CONDITION` | T24 application: FX.GROUP.CONDITION |
| `SC.MT548.MATCH.QUEUE` | T24 application: SC.MT548.MATCH.QUEUE |
| `SC.STD.SEC.TRADE` | T24 application: SC.STD.SEC.TRADE |
| `SEC.TRADE` | T24 application: SEC.TRADE |
| `SP.AGGR.LAUNCH` | T24 application: SP.AGGR.LAUNCH |
| `SP.AGGREGATION` | T24 application: SP.AGGREGATION |
| `SP.RECONCILATION` | T24 application: SP.RECONCILATION |
| `SP.RECONCILIATION` | T24 application: SP.RECONCILIATION |
| `SP.STP.PARAM` | T24 application: SP.STP.PARAM |
| `SYSTEM` | T24 application: SYSTEM |


### Fields Referenced


| Field | Field | Field |
|-------|-------|-------|
| `Aa Product Group` | `Ac Exc Trd` | `Account` |
| `Accrual Basis` | `Accrued Units1` | `Acct With Bank Bic` |
| `Acct With Bank Customer` | `Acct With Bank Swift Addr` | `Active` |
| `Agency Booking Model` | `Aggr Cut Off Time` | `Aggr Id` |
| `Aggr Req` | `Aggr Utc Time` | `Aggregation Ref` |
| `All Customers` | `Alt Ccy Ben Acct` | `Alt Ccy Ben Bank` |
| `Alt Ccy Cpty Add` | `Alt Ccy Cpty No` | `Alt Ccy Intr Add` |
| `Alt Ccy Intr Addr` | `Alt Ccy Intr Bank` | `Alternate Ccy 1` |
| `Alternate Ccy 2` | `Alternate Ccy1` | `Alternate.Ccy.2` |
| `Alternative Price Set` | `Amount Bought` | `Amount Sold` |
| `Applicable Element` | `Application` | `Application Access Link` |
| `Application Access Type` | `Apply Leverage` | `As` |
| `As Currency` | `As Fixed Rate` | `As Float Key` |
| `As Floating` | `As Int Frequency` | `As Principal` |
| `As Rr Frequency` | `Asian Type` | `Asset Ccy` |
| `Asset Class` | `Asset Principal` | `Asset Type` |
| `Au Ct Class` | `Au Sett Delay` | `Au Sett Type` |
| `Authorise Child` | `Auto Authorise` | `Auto Rollover Term` |
| `Available Date` | `Average DPS` | `Average I Price` |
| `Average Price` | `Average Spot` | `Average Strike` |
| `B Apply Leverage` | `B Cpty Sett Amount` | `B Fixing` |
| `B Lev Sched Call Amt` | `B Lev Sched Put Amt` | `B Settlement Amt` |
| `B Settlement Date` | `B2B Reference` | `B2b Active` |
| `B2b Co Ok` | `Back To Back Deal` | `Bank to Bank Info` |
| `Barrier Evaluation` | `Barrier Level` | `Barrier Or Trigger` |
| `Barrier Trigger` | `Barrier Type` | `Barrier or Trigger` |
| `Base Amount` | `Base CCY Rank` | `Base Ccy` |
| `Base Ccy Rank` | `Base Currency` | `Basket Type` |
| `Ben Acct` | `Beneficiary Account No` | `Beneficiary Bank` |
| `Beneficiary Bic` | `Beneficiary Customer` | `Beneficiary Name` |
| `Block Amount` | `Block Nominal` | `Block Until` |
| `Bond Ccy` | `Bond Value` | `Broker` |
| `Broker No` | `Build Fwd Rate` | `Build Pgm` |
| `Build Structure` | `Buy Currency` | `Buy Fixing` |
| `Buy Schedule Call Amt` | `Buy Schedule Call Amt,` | `Buy Schedule Put Amt` |
| `Buy Schedule Put Amt,` | `Buy Undo Fixing, Sell Undo Fixing` | `Buy or Sell` |
| `Ca Impact` | `Ca Tra Version` | `Calendar` |
| `Call / Put` | `Call Amount` | `Call Ccy` |
| `Call Ccy/Put Ccy` | `Call Put` | `Call or Put` |
| `Call/ Put` | `Call/Put` | `Cancel Pend Order` |
| `Cancel Pend Orders` | `Cash Amount` | `Cash Ccy` |
| `Cash Exercise` | `Cash Settle Ccy` | `Category` |
| `Channel` | `Charge Code` | `Charge Percent` |
| `Check Cust Funds` | `Chg Post Offset` | `Chg Post Time` |
| `Class Category` | `Clfee Charge` | `Close Out Id` |
| `Closeout Market Price` | `Closeout Sett Ccy` | `Closeout Trade` |
| `Closeout Txn Amt` | `Closeout Version` | `Co Comm Posting` |
| `Co Lots` | `Co Pgm` | `Cob Phase` |
| `Comm Charge` | `Cons Data Item` | `Cons Data Name` |
| `Constraint Type` | `Cont Time Source` | `Cont Ulying Val` |
| `Contingent Value` | `Contract` | `Contract Ccy` |
| `Contract Class` | `Contract Code` | `Contract Size` |
| `Contract Status` | `Contract Terms` | `Contract Type` |
| `Convert Interest` | `Converted Lcy` | `Cost Calc Api` |
| `Countdown` | `Counterparty` | `Counterparty Acc` |
| `Counterparty Alt Currency Account 2` | `Counterparty deal` | `Covered Contract` |
| `Cp Bccy Ben Bank` | `Cp Bccy Cpty Add` | `Cp Bccy Cpty No` |
| `Cp Bccy Intr Bank` | `Cp Sccy Ben Bank` | `Cp Sccy Cpty Add` |
| `Cp Sccy Cpty No` | `Cp Sccy Intr Bank` | `Cpa Prem Acc` |
| `Cpa Prem Amt` | `Cpa Unwind Chg Acc` | `Cpa Unwind Chg Amt` |
| `Cparty Alt Currency Account 1` | `Cparty Alt Currency Account 2` | `Cparty Buy Ccy Acct` |
| `Cparty Cash Sett Acc` | `Cparty Deposit Acc` | `Cparty Sell Ccy Acct` |
| `Cpty Add` | `Cpty Fee Amt` | `Cpty No` |
| `Cpty Prem Amt` | `Cpty Premium Amt` | `Cpty Sett Amt` |
| `Cpty Unwind Chg Amt` | `Cr Exp Calc Api` | `Cr Txn` |
| `Create Deposit` | `Create Option` | `Create Trade` |
| `Create Trades` | `Credit Nostro Account` | `Currency` |
| `Currency Bought` | `Currency Name` | `Currency Sold` |
| `Currency1` | `Currency2` | `Currnt/Closng/Whatif` |
| `Cus Fxmargin Txn` | `Cust No Nom` | `Cust Or Port` |
| `Cust Price` | `Cust Trans Code` | `Customer` |
| `Customer No` | `Customer No.` | `Customer Type` |
| `Customer or Portfolio` | `DX.CONTRACT.MASTER` | `DX.TRADE ID` |
| `Daily Units` | `Date` | `Day Trade` |
| `Db Txn` | `Deal Reference` | `Deal Status` |
| `Deal Type` | `Dealer Desk` | `Debit Account` |
| `Debit Ccy` | `Debit Value Date` | `Dec Date` |
| `Delivery Ccy` | `Delivery Ccy Rate` | `Delivery Currency` |
| `Delivery Method` | `Delta` | `Dep Ccy Ben Acct` |
| `Dep Ccy Ben Bank` | `Dep Ccy Cpty Add` | `Dep Ccy Cpty No` |
| `Dep Ccy Intr Add` | `Dep Ccy Intr Addr` | `Dep Ccy Intr Bank` |
| `Dep Prin Adjust` | `Dependency` | `Deposit Amt` |
| `Derivatives` | `Description` | `Det Prefix` |
| `Diary Type` | `Dx Diary Id` | `Dx Trade Id` |
| `Early Maturity Date` | `Eb Activity` | `Eb Contract Balance` |
| `Element` | `Element New Ratio` | `Element New Value` |
| `Element Old Ratio` | `Element Type` | `Enable Customer Closure` |
| `Estimation` | `Et Eq Modifier` | `Event` |
| `Event Time Type` | `Event Triggered` | `Event Type` |
| `Ex Date` | `Exch Member` | `Exch Session` |
| `Exchange` | `Exchange Code` | `Exchange Customer` |
| `Exchange Keys` | `Exchange Type` | `Executing Broker` |
| `Exer Pri Mem` | `Exer Pri Non` | `Exercise` |
| `Exercise Ccy` | `Exercise Ccy,` | `Exercise Expire` |
| `Exercise/Expire` | `Exfee Charge` | `Exotic Event` |
| `Exotic Events Allowed` | `Exotic Fld Val` | `Exotic Fld Val .1` |
| `Exotic Type` | `Exotic Type.1` | `Exotic Type.2` |
| `Exotic Type.3` | `Expire Lots` | `Expired Lots` |
| `Expiry Pri` | `FIELD.NAME` | `FIELD.VALUE` |
| `Feed To Clear` | `Field From` | `Field Name` |
| `Field To` | `Filled Iprice` | `Filled Lots` |
| `Filled Price` | `Final Maturity Date` | `First Date` |
| `Fix Structure` | `Fixed Ccy` | `Fixed Rate` |
| `Fixed Start Date` | `Fixed Status` | `Fixed Strike` |
| `Fixing Date` | `Fixing Frequency` | `Fixing Routine` |
| `Freq` | `Full` | `Fwd Post Eod` |
| `Fx Consolidate` | `Fx Exot Dlv Msg` | `Fx Payout Ccy` |
| `Fx Payout Currency` | `Gamma` | `Geared Accrual` |
| `Gen Data Code` | `Gen Data Limit` | `Generated By` |
| `Geographical Block` | `Group` | `Hedge Trade` |
| `Hld Reval Days` | `House Customer` | `INT.BASIS` |
| `Init Margin Calc` | `Initial Margin` | `Inputter` |
| `Int Rate Contract` | `Interest Basis` | `Interest Currency` |
| `Interest Rate` | `Interest Rate` | `Intermed Bank Customer` |
| `Intermed Bic` | `Intermed Swift Addr` | `Internal Order Details` |
| `Intr Add` | `Intr Bank` | `JH.ACCESS.LINK` |
| `JH.ACCESS.TYPE` | `Kickin Expire` | `Knock In` |
| `Knock Out` | `Knockout Price` | `LINK.REFERENCE` |
| `Last Date` | `Lb Currency` | `Lb Fixed Rate` |
| `Lb Float Key` | `Lb Floating` | `Lb Principal` |
| `Liab Ccy` | `Liab Principal` | `Life Underlying` |
| `Lim Amt Val Cont` | `Limit Date` | `Limit Price` |
| `Limit Ref` | `Limit Type` | `Linked Trade` |
| `Loan Prin Adjust` | `Local Or Source` | `Log Detail Level` |
| `Logic` | `MTM Amount` | `Maint Message Dets` |
| `Maint Msg Dets` | `Maintenance Margin` | `Manual Rollover` |
| `Marg Weighting` | `Margin Acc Ccy` | `Margin Difference` |
| `Margin Level` | `Market Price` | `Market Price1` |
| `Matured Lots` | `Maturity` | `Maturity Date` |
| `Maturity Type` | `Max Months Fwd` | `Message Type` |
| `Mid Reval Rate` | `Mifid Report Status` | `Min Period Kout` |
| `Min Price Mvmt` | `Min Price Mvmt.1` | `Misc Charge` |
| `Mkt Exch Prt` | `Mnemonic` | `Mtm Amount` |
| `Mtm Required` | `Mtm Routine` | `Mutual Offset` |
| `Narrative` | `Nett Gross` | `New Daily Units` |
| `New Maturity Date` | `New Ratio` | `New Security No` |
| `New Str Pri` | `New Value` | `No of Options` |
| `No. of Lots` | `Notional Amt` | `Notional Diff` |
| `Notional Entries` | `Novated From` | `Novated To` |
| `Novation` | `Number of Decimal Places` | `Numeric Currency Code` |
| `OPERAND` | `Observation Date` | `Observation Dates` |
| `Observed Spot Rate` | `Ofs Source` | `Old Ratio` |
| `Operand` | `Operator` | `Opt Exercise` |
| `Opt Exercise Date` | `Option Date` | `Option Style` |
| `Option Type` | `Option Value Type` | `Option Variant` |
| `Ord Ofs Version` | `Order Amend` | `Order Closeout` |
| `Order Initiation Type` | `Order Status` | `Order Type` |
| `Ordering Customer Bic` | `Ordering Reference` | `Original Lcy` |
| `Own Company` | `Own Company Id` | `PARTY.APPLICATION` |
| `Parent` | `Parent Child Ref` | `Parent Child Ref` |
| `Participation Rate` | `Pay Out Amount` | `Pay Out From Mm` |
| `Pay Put Ccy` | `Pay Receive` | `Pay Receive Flag` |
| `Payment Amount` | `Payment Category` | `Payment Currency` |
| `Payment Method` | `Payment Purpose` | `Payment Type` |
| `Performance` | `Po Application` | `Po Reference` |
| `Po Susp Categ` | `Port Comp Id` | `Portfolio` |
| `Post Lcy` | `Post Update Rtn` | `Prem Pay Future` |
| `Prem Pay Percentage` | `Prem Percent` | `Prem Post Offset` |
| `Prem Post Time` | `Prem Pymt` | `Prem Pymt Amt` |
| `Prem Pymt Date` | `Prem Pymt Freq` | `Premium Acc` |
| `Premium Amt` | `Premium Ccy` | `Premium Currency` |
| `Premium Pay Receive` | `Pri Allow Sett` | `Pri Auto Manual` |
| `Pri Cacc Amt` | `Pri Comm Acc` | `Pri Comm Amt` |
| `Pri Comm Cde` | `Pri Comm Exc` | `Pri Comm Tax` |
| `Pri Commission Account` | `Pri Commission Amt` | `Pri Commission Ccy` |
| `Pri Commission Code` | `Pri Commission Tax` | `Pri Commission Type` |
| `Pri Hedge Trade` | `Pri Limit Ref` | `Pri Lots` |
| `Pri Original Lots` | `Pri Pnd Lots` | `Pri Pnd Sett` |
| `Pri Prem Exc` | `Pri Settnos` | `Price` |
| `Price Days` | `Price Order` | `Price Set` |
| `Price Source` | `Price To Store` | `Price/Premium` |
| `Principal` | `Proc Sec Fees` | `Process Id` |
| `Prod Definition` | `Product Category` | `Product Definition` |
| `Product Type` | `Put Amount` | `Put Ccy` |
| `Pymt Msg Req` | `Pymt Msg Reqd` | `Quantity` |
| `Quotation Code` | `Quote Ccy` | `Quote Currency` |
| `RM Status` | `Re Calculate I M` | `Re Value Level` |
| `Receive Type` | `Receiver Bic` | `Recon Id` |
| `Record ID` | `Record Status` | `Ref Exc Trd` |
| `Remaining Units` | `Renewal Frequency` | `Rep Updates` |
| `Reporting Ccy` | `Required Credit Value Date` | `Review Cash Posting` |
| `Rgfee Charge` | `Rho` | `Risk Company` |
| `Risk Level` | `Run Current Fixing` | `Run Notional Amt` |
| `Run Notional in Buy Ccy` | `Run Notional in Sell Ccy` | `S Cpty Sett Amount` |
| `S Fixing` | `S Settlement Amt` | `SYSTEM.ID` |
| `Sc Asset Upd` | `Scdx Charge Method` | `Search All Commsn` |
| `Sec Allow Sett` | `Sec Auto Manual` | `Sec Buy Sell` |
| `Sec Comm Cde` | `Sec Comm Code` | `Sec Cpty No` |
| `Sec Cust(Broker)` | `Sec Field Name` | `Sec Fld Nme` |
| `Sec Int Rate` | `Sec Limit Ref` | `Sec Pnd Lots` |
| `Sec Pnd Sett` | `Sec Price` | `Sec Settnos` |
| `Sec Trd Aggr` | `Security Code` | `Sell Currency` |
| `Sell Fixing` | `Sett Allowed` | `Sett Instr Price` |
| `Sett Instr Units` | `Sett Instrument Contract Size` | `Sett Instrument Price` |
| `Settle Ccy` | `Settlement Amount` | `Settlement Amount1` |
| `Settlement Ccy` | `Settlement Date` | `Settlement Instrument` |
| `Settlement Method` | `Settlement Role` | `Single Schedule` |
| `Source Key` | `Source Type` | `Sp Aggr ID` |
| `Sp Aggr Launch Version` | `Sp Aggregation` | `Special Rate` |
| `Spot Exchange Rate` | `Spot Payout Rate` | `Spot Price` |
| `Spot Price Initial` | `Spread` | `Static Leg` |
| `Status` | `Stirke Operand` | `Stmt Narr Ref` |
| `Stp Enabled Apps` | `Stp Timeout` | `Straddle` |
| `Strike` | `Strike Operand` | `Strike Percentage` |
| `Strike Price` | `Strike Price1` | `Strike Price2` |
| `Strike Quote` | `Strike,` | `Strike Price` |
| `Structure Fix Date` | `Sub Asset Type` | `Suppress Underlying` |
| `Suppress Vm Post` | `Supress Underlying` | `Susp Reset Date` |
| `Suspend Accrual` | `Swap Delivery` | `Swap Mat Date` |
| `Sweep Acct` | `Sy Dx Reference` | `Sy Excl Val Field` |
| `Sy Exclude Val` | `Sy Exclude Valuation` | `Sy Id Field` |
| `Sy Master` | `Sy Product Category` | `Sy Trans Id` |
| `Sy Transaction Id` | `Sy Unit Field` | `Synthetic Cpty` |
| `Synthetic Port` | `System Date` | `System Exercise` |
| `System Expire` | `System Expiry` | `System Expiry are set to` |
| `Table` | `Tax Interest Key` | `Tax Interest Type` |
| `Term` | `The Program field s` | `Theta` |
| `Tick Size` | `Tick Value` | `Time to Expiry` |
| `Tot Tax Int Lcy` | `Total Interest Tax` | `Total Notional in Sell Ccy` |
| `Total Units` | `Tra Pnd Lots` | `Tra Pnd Sett` |
| `Tracking` | `Trade` | `Trade Ccy` |
| `Trade Date` | `Trade Direction (Buy/ Sell)` | `Trade Price` |
| `Trade Status` | `Trade Type` | `Trade date` |
| `Trading Close` | `Trading Days` | `Trading Open` |
| `Trading Status` | `Trans ID` | `Trans Id` |
| `Trans Reference` | `Transaction Reporting` | `Trasettnos` |
| `Trd Aggr` | `Tx Act Upd` | `Tx Buy Sell` |
| `Tx Open Close` | `Type` | `Ulying Asset Class` |
| `Ulying Security` | `Ulying Strike Ccy` | `Ulying Strike Price` |
| `Unauth Auth` | `Und Int Price` | `Underlying` |
| `Underlying Bond` | `Underlying Price` | `Underlying Security` |
| `Underlying maturity date` | `Undlying Mat Date` | `Unique Identifier` |
| `Unwind` | `Unwind Chg Acc` | `Unwind Chg Amt` |
| `Unwind Chg Amt.` | `Unwind Chg Ccy` | `Update Avail` |
| `Upper or Lower` | `Use Ft Txn Code` | `Use Master Sat` |
| `Usr Fld Price` | `Usr Fld Type` | `Valoren No` |
| `Valoren Number` | `Valuation` | `Valuation Amount` |
| `Valuation Ccy` | `Valuation Currency` | `Valuation Routine` |
| `Value Date` | `Value Date Buy` | `Value Date Sell` |
| `Value Units` | `Vanilla Buy Fixing` | `Vanilla Buy Undo Fixing` |
| `Var Margin Calc` | `Variant` | `Vb Cpty Sett Amount` |
| `Vb Settlement Amt` | `Vega` | `Vm Post Style` |
| `Vm Rev Type` | `Vm Reversal Style` | `Volatility` |
| `Weight` | `Xxx Allow Sett` |  |


---


## Appendix B: Consolidated Field Reference


This appendix consolidates all field description tables from across the documentation, grouped by sub-module. This provides a single reference for all field definitions.


### Derivatives_Structured_Products - DI (DI)


**DigitalInvestments**

| Event | Description |
|---|---|
| Inception | The contract is recorded in the system and the underlying option deal and deposit are created |
| Fixing | The fixing decision is made and the investor receives minimum or maximum rate, depending on the spot exchange rate, in comparison with the upper and lower barriers |
| Maturity | The contract expires on the maturity date and the deposit is redeemed |

**DigitalInvestments**

| Term Sheet Element | Description |
|---|---|
| Value Date | Indicates the effective date of the contract |
| Deposit Currency | Indicates the currency of the deposit |
| Deposit Amount | Indicates the amount of the deposit in deposit currency |
| Tracking Currency | Indicates the tracking currency, which along with the deposit currency forms the currency pair. The spot exchange rate for this currency pair is tracked against the barrier rates. |
| Maximum Interest Rate | Indicates the maximum interest rate on the deposit if the option is in-the -money |
| Minimum Interest Rate | Indicates the minimum interest rate on the deposit. The investor receives the interest amount based on this rate, if the option expires worthless. |
| Upper Barrier | Indicates the upper barrier exchange rate for the digital option |
| Lower Barrier | Indicates the lower barrier exchange rate for the digital option |
| Maturity Date | Indicates the maturity date of the contract |

**Dual and Triple Currency Investments**

| Term Sheet Element | Description |
|---|---|
| Value Date | Effective date of the deposit |
| Deposit Currency | Currency of the deposit |
| Deposit amount | The principal investment amount |
| Alternate Currency | Alternate currency |
| Strike Exchange Rate | Agreed forward exchange rate between the deposit currency and the alternate currency |
| Interest Rate | Enhanced interest rate for the deposit |
| Fixing date | The date on which the spot exchange rate is compared against the strike price and exercise or expire decision is made |
| Maturity date | Maturity date of the deposit or contract |
| Alternate currency 2 | Applicable for TCI contracts only. This is the other alternate currency |
| Strike exchange rate 2 | Applicable for TCI contracts only. Agreed forward exchange rate between the deposit currency and alternate currency 2 |

**Dual and Triple Currency Investments**

| Event | Description |
|---|---|
| Inception | The contract is recorded in the system. The underlying deposit and option transaction are created |
| Fixing | Decision event. The spot exchange rate is compared against the strike exchange rate; the user decides whether to exercise or expire the currency option. |
| Maturity | The deposit matures and depending on the fixing decision, the redemption amount is either converted to the alternate currency (through a FX spot deal) or redeemed in the deposit currency. This event would be scheduled to run on the maturity. |
| Unwinding | Unwinding is an early termination event whereby the maturity date can be advanced to an earlier date. |

**Dual and Triple Currency Investments**

| Variant | Description |
|---|---|
| Precious Metal Investments | In this variant, either the deposit currency or the alternate currency is a precious metal defined as a currency in the system |
| DCI with barriers | In this variant, the currency option is a barrier option. Option can have knock-in or knock-out features. In Temenos Transact terms, this is defined as an exotic option |
| Principal only conversion | In this variant, if the option is exercised, then only the principal is converted to the alternate currency. The interest amount is repaid in the deposit currency |
| Tripe Currency Investment | In this variant, there are two alternate currencies. The redemption can be in the deposit currency or in any of the alternate currencies |

**Misc**

| Field | Description |
|---|---|
| Variant | Variant for the contract to use the said categories based on the SY.PRODUCT.VARIANT selected. |
| Trade Date | Holds the trade date of the contract. Trade date cannot be forward dated and should fall between the First Date and Last Date of the corresponding product definition record. |
| Maturity Date | Maturity date is the termination date of the contract. Maturity date will be defaulted based on Term and Value Date . |
| Trade Ccy | This is the deposit currency in which the customer deposit or takes loan in MM.MONEY.MARKET . Is the Trade Ccy of DX.TRADE . |
| Alternate Ccy 1 | The alternate currency in which the deposit amount is paid back, that is, the delivery currency in DX.TRADE and the other currency in FOREX |
| Alternate.Ccy.2 | The second alternate currency in which the deposit amount is paid back, that is, this field enables the triple currency investment. On exercise of option FOREX gets created between Trade Ccy and Alternate Ccy 2 . The option trade between Trade Ccy and Alternate Ccy 1 is expired. |
| Exercise Expire | When the field is set to EXERCISE the option contract is exercised and when set to EXPIRE the option contract is expired. The value to the field can be manually determined. When not the fixing event determines the value to this field. The fixing routine to have 2 parameter which are outcoming. The 1st to hold the EXERCISE or EXPIRE as value saying the decision and the second to hold the Exercise Ccy, if suppose the decision is to exercise the option contract. |
| Exercise Ccy | The currency in which the forex is created when it is Alternate Ccy 1 then the DX.TRADE is exercised. When it is Alternate Ccy 2 then it means the DX.TRADE between trade and first alternate currency is expired and a new FX gets created between Trade Ccy and Alternate Ccy 2 . |

**Misc**

| Element | Description |
|---|---|
| Value date | Effective date of the deposit |
| Deposit currency | Currency of the deposit |
| Deposit amount | The principal investment amount |
| Alternate currency | Alternate currency used |
| Strike exchange rate | Agreed forward exchange rate between the deposit currency and the alternate currency |
| Interest rate | Enhanced interest rate for the deposit |
| Fixing date | The date on which, the spot exchange rate is compared against the strike price and exercise or expire decision is made. |
| Maturity date | Maturity date of the deposit or contract |
| Alternate currency 2 | Applicable for TCI contracts only. This is the other alternate currency. |
| Strike exchange rate 2 | Applicable for TCI contracts only. Agreed forward exchange rate between the deposit currency and alternate currency. |

**Misc**

| Event | Description |
|---|---|
| Inception | The contract is recorded in the system. The underlying deposit and option transaction are created. |
| Fixing | Decision event. The spot exchange rate is compared against the strike exchange rate. The user decides whether to exercise or expire the currency option. |
| Maturity | The Deposit matures and depending on the fixing decision, the redemption amount, is either converted to the alternate currency (through a FX Spot Deal) or redeemed in the deposit currency. This event is scheduled to run on the maturity. |
| Unwinding | Unwinding is an early termination event, where the maturity date can be advanced to an earlier date. |

**Misc**

| Variant | Description |
|---|---|
| Precious metal investments | In this variant, either the deposit currency or the alternate currency, is a precious metal defined as a currency in the system. DCI with barriers - In this variant, the currency option is a barrier option. Option can have knock-in or knock-out features. In Temenos Transact terms, this is defined as an exotic option. |
| Principal only conversion | In this variant, if the option is exercised, then only the principal is converted to the alternate currency. The interest amount is repaid in the deposit currency. |
| Tripe currency investment | In this variant, there are two alternate currencies. The redemption can be in the deposit currency or in any of the alternate currencies. |


### Derivatives_Structured_Products - DP (DP)


**Misc**

| Term sheet element | Description |
|---|---|
| Value Date | Commences the contractual obligation from this date |
| Underlying security | Denotes the underlying security which is accumulated or decumulated over the tenor of the contract |
| Strike Price | Denotes the forward price at which the underlying security is purchased or sold |
| Knock out price | Denotes the barrier price. When the spot price of the underlying security breaches this barrier, the contract gets knocked out (terminated). |
| Daily units | Denotes the number of shares that must be accrued on a daily basis |
| Gearing Factor | Applies on the days, when the spot price of the underlying is unfavorable to the investor comparing the strike price |
| Fixing Frequency | Denotes the periodicity at which the settlement of accumulated or decumulated shares occur |
| Maturity Date | Denotes the date on which the contractual obligation ends |

**Misc**

| Event | Description |
|---|---|
| Inception | Commences contractual obligation for the investor. The contract is recorded in the system and the underlying option trade is created. |
| Accrual | Units (of the underlying security) are accrued on a daily basis. For contracts with gearing factor, the gearing factors are applied on the days when the spot price of the underlying is unfavourable to the investor comparing the strike price of the contract. |
| Fixing | Effects the settlement of the accumulated or decumulated shares. The underlying option is exercised and this creates the SEC.TRADE transaction for the underlying security. This is a scheduled periodic event. |
| Knockout | Occurs when the price barrier is breached, that is, when the spot price of the underlying touches the knock-out price. When this event occurs, the contract is terminated. |
| Unwinding | Terminates the contract either fully or partially. In a full unwind, the contract is terminated earlier. In a partial unwind, the contract continues to be active, but the obligation (that is, daily accrual units) is reduced for the rest of the contract period. |
| Novation | Transfers the contract between customers and banks. Internal novation - Contract is transferred from one customer account to another External novation - Contract is transferred from customer account in one bank to another |
| Maturity | Indicates the end date of the contract. The contractual obligation ceases on this date. |

**Misc**

| Variant | Description |
|---|---|
| Non-leveraged accumulator or decumulator | Denotes the plain vanilla accumulator without a gearing factor |
| Leveraged accumulator | Holds an additional attribute that is, gearing factor. Gearing factor is applied to the accrual on the days when the spot price is unfavourable to the customer, comparing the strike price. The potential loss to the investor is higher in this variant, compared to the plain vanilla variant. |
| Guaranteed accumulator or decumulator | Assures the investor of guaranteed accumulation. That is, a certain number of underlying shares might be accumulated or decumulated and settled, even if the knock-out price barrier is breached early in the life of the accumulator contract. |

**Misc**

| Field | Description |
|---|---|
| Product Type | This field indicates this is an accumulator or decumulator contract. |
| Contract Status | The status of the contract is updated in this field. When the contract is created, the status is ACTIVE, subsequently as the contract undergoes various life cycle events, the status is updated as below. |
| Option Type | This field holds the option type of the underlying option. This is auto populated based on the Product Type field. For accumulator contract, the underlying is a PUT option, for decumulator contract, the underlying is a CALL option. |
| Trade Date | This field holds the trade date of the contract. Trade date cannot be forward dated and should fall between the First Date and Last Date of the corresponding product definition record. |
| Maturity Date | Maturity date is the termination date of the contract. Maturity date is defaulted based on Term and Value Date . |
| Daily Units | This field holds the number of units (nominal) to be accrued per day. The value should be a multiple of contract size of the underlying DX.CONTRACT.MASTER . |
| Fixing Frequency | The Accumulator and Decumulator contracts accrue the underlying security on a daily basis. The accrued units are settled periodically (This periodic settlement is known as fixing). |

**Misc**

| Element | Description |
|---|---|
| Value Date | Contractual obligation commences from this date. |
| Underlying security | The underlying security which is accumulated or decumulated over the tenor of the contract. |
| Strike Price | The forward price at which the underlying security is purchased or sold. |
| Knock out price | This is the barrier price, when the spot price of the underlying security breaches this barrier, the contract gets knocked out (terminated). |
| Daily units | The number of shares that must be accrued on a daily basis. |
| Gearing factor | The gearing factor is applied on the days when the spot price of the underlying is unfavourable to the investor when compared to the strike price. |
| Fixing drequency | Settlement of accumulated or decumulated shares occur at this periodicity. |
| Maturity Date | The contractual obligation ends at this date. |

**Misc**

| Event | Description |
|---|---|
| Inception | Contractual obligation commences for the investor. The contract is recorded in the system and the underlying option trade is created. |
| Accrual | Units (of the underlying security) is accrued on a daily basis. For contracts with gearing factor, the gearing factors are applied on those days when the spot price of the underlying is unfavourable to the investor when compared against the strike price of the contract. |
| Fixing | Settlement of the accumulated or decumulated shares are effected through this event. The underlying option is exercised and this creates the SEC.TRADE transaction for the underlying security. This is a scheduled periodic event. |
| Knockout | This event can occur when the price barrier is breached, that is, when the spot price of the underlying touches the knock-out price. When this event occurs, the contract is terminated. |
| Unwinding | The contract can be unwound either fully or partially. In a full unwind, the contract is terminated early. In a partial unwind, the contract continues to be active, but the obligation (that is, daily accrual units) are reduced for the rest of the contract period. |
| Novation | The contract can also be novated, which is transferred from one customer account to another customer account (Internal novation) or transferred to a different bank (external novation). |
| Maturity | It is the end date of the contract. The contractual obligation ceases on this date. |

**Misc**

| Variant | Description |
|---|---|
| Non leveraged accumulator or decumulator | This is the plain vanilla accumulator without a gearing factor. |
| Leveraged Accumulator | This variant has an additional attribute, which is, gearing factor. Gearing factor is applied to the accrual on those days where the Spot Price is unfavorable to the customer, when compared to the strike price. The potential loss to the investor is higher in this variant as compared to the plain vanilla variant. |
| Guaranteed accumulator or decumulator | This variant assures the investor of guaranteed accumulation. That is, a certain number of underlying shares might be accumulated or decumulated and settled, even if the knock-out price barrier is breached early in the life of the accumulator contract. |


### Derivatives (DX)


**Accounting**

| ACCOUNT.CLASS ID | Type | Description |
|---|---|---|
| SUSPDXIMCR | Account | Suspense account for credit initial margin |
| SUSPDXIMDR | Account | Suspense account for debit initial margin |
| SUSPDXVMCR | Account | Suspense account for credit futures variation margin |
| SUSPDXVMDR | Account | Suspense account for debit futures variation margin |
| SUSPDXOMCR | Account | Suspense account for credit option variation margin |
| SUSPDXOMDR | Account | Suspense account for debit option variation margin |
| SUSPDXCGCR | Account | Suspense account for credit DX charges |
| SUSPDXCGDR | Account | Suspense account for debit DX charges |
| SUSPDXPRCR | Account | Suspense account for credit option premium payments |
| SUSPDXPRDR | Account | Suspense account for debit option premium payments |
| SUSPDXRPCR | Account | Suspense account for credit realised P&L |
| SUSPDXRPDR | Account | Suspense account for debit realised P&L |
| DXCSNDUE | P&L | Suspense P&L category for DX commission due not paid (not utilised until phase 2) |
| DXCSNEARN | P&L | Suspense P&L category for DX commission earned, but not received (not utilised until phase 2) |
| DXCSNPAID | P&L | Suspense P&L category for DX commission paid |
| DXCSNRCVD | P&L | Suspense P&L category for DX commission received |

**Accounting**

| Transaction types in RE.TXN.CODE | Description |
|---|---|
| CLO | Derivatives contract closeout |
| UOV | Derivatives unrealised option value |

**Accounting**

| Application | Fields |
|---|---|
| DX.ORDER | Pri Tax Code , Pri Tax Type , Tax Amt Acy , Tax Amt Tcy , Sec Tax Code , Sec Tax Type , Sec Tax Amt Acy , and Sec Tax Amt Tcy |
| DX.TRADE | Pri Tax Code , Pri Tax Type , Tax Amt Acy , Tax Amt Tcy , Sec Tax Code , Sec Tax Type , Sec Tax Amt Acy , and Sec Tax Amt Tcy |
| DX. CLOSEOUT | Tax Code , Tax Type , Tax Amt Acy , and Tax Amt Tcy |

**Aggregation SEC.TRADE SSI**

| Operand | Description |
|---|---|
| EQ | Selects all the contracts where the strike price is equal to the value provided in Strike. |
| GE | Select all the contracts where the strike price is greater than or equal to the value provided in Strike. |
| LE | Select all the contracts where the strike price is less than or equal to the value provided in Strike. |

**Asian and Performance Options**

| Field | Description |
|---|---|
| Option Value Type | Contains a drop-down value called Asian. If this field is populated, either Asian Type or Performance field is populated. |
| Asian Type | The allowed values are Fixed Strike Floating Strike This field is mandatory if Option Value Type is Asian and Performance field is not set to Yes. A validation ensures if Fixed Strike is selected, and Settlement Method is set to CASH. This is a no input field, if Option Value Type is not set to Asian. |
| Performance | This is a Yes or No field. If it is set to Yes, the performance of the underlying asset is used to determine the payout Where, Where, Underlying final - Spot price on fixing date Underling initial - Spot price on start date of the contract When this field is set to Yes, the strike price and the call or put indicator in the trade is irrelevant. The default values to be used are: Strike set to 1 Call/ Put set to Call When this field is set, the Settlement Method is in cash always. |

**Asian and Performance Options**

| Field | Description |
|---|---|
| Participation Rate | A percentage field that is used to calculate the final payout of the option. This is a mandatory field, if Performance field is set to Yes in DX.CONTRACT.MASTER |
| Observation Date -XX | A multi value field where the observation schedule can be defined. This is a mandatory field when Option Value Type is set to Asian. The number of multi values is equal to the number of dates in the fixing schedule |
| Observed Spot Rate -XX | An associated multi value field that indicates the spot price of the underlying asset on the Observation Date |
| Spot Price Initial | Indicates the spot price of the underlying asset on commencement of the contract. This price is used to calculate the performance of contracts with Performance field set to Yes |

**Asian and Performance Options**

| Field | Description |
|---|---|
| Observation Date -XX | Defaults the values from DX.TRADE and it is a no input field |
| Observed Spot Rate -XX | Defaults the values from DX.TRADE . The values are amendable (that is, if values are available in DX.TRADE , then rate is populated by default in this field. The user can also input and override the default value.) |
| Participation Rate | Defaults the values from trade and it is a no input field |
| Performance | Indicates the calculated value, If the Performance field is set to Yes and the Option Value Type is set to Asian, Where, n = number of observation dates, Underlying final (i) = Underlying spot price on corresponding observation date (that is, Observed Spot Rate ), Underlying initial = Spot Price Initial If the Performance field is set and the Option Value Type is not set to Asian, then Where, Underlying final = Market Price , Underlying initial = Spot Price Initial |
| Average Spot | This is a calculated value. Updated only when Asian Type field is set to Fixed Strike in DX.CONTRACT.MASTER . where, n = number of multi values (that is, the value in the Observation Date field) This field can be modified by the user. |
| Average Strike | Indicates the calculated value which is updated only when Asian Type field is set to Floating Strike in DX.CONTRACT.MASTER . where n = number of multi values (that is, the value in the Observation Dates field) This field can be modified by the user. |

**BasketOptions**

| Field | Default Value |
|---|---|
| Underlying | Basket |
| Price Source | Interface |
| Tick Value | 1 |
| Tick Size | 1 |
| Contract Size | 1 |
| Currency | No input |
| Delivery Currency | No input |
| Settlement Method | No input |
| Contract Size | No input |
| Exchange | Non-mandatory |
| Option Style | Non-mandatory |

**BasketOptions**

| Field | Description |
|---|---|
| Mnemonic | Indicates the alternate identifier for the basket |
| Unique Identifier | Indicates the unique identifier such as ad valorem number |
| Ulying Asset Class | Indicates whether the underlying is an equity or currency basket. This is a mandatory field. The values are : Equity Currency |
| Basket Type | Indicates the type of basket. The values are: Null (default value) Best of the Market Custom Weighted Equal Weighted Worst of the Market The value Null indicates that it is not a basket option. Though there are four types of baskets available at present, this list is scalable. This list can be configured based on the BASKET.TYPE user defined value in the EB.LOOKUP table. |
| Price Source | Indicates the identifier of a price interface. This value overrides the value in the Price Source field in DX.CONTRACT.MASTER . |
| Call Put | Indicates if the holder has the right, but not obligation, to buy or sell stock at a fixed price at a future date. The values are: None Call Put |
| Trade Ccy | Indicates the trade currency |
| Maturity Date | Indicates the delivery period or prompt date of the contract transacted |
| Settlement Method | Indicates the settlement mode of the option contract. The values are: Cash Physical |
| Static Leg | Indicates if the buy or sell currency should be same in all multi-value pairs. This field is mandatory for currency basket. The values are: None Call Put |
| Ulying Security | Indicates if the underlying is a security or currency basket. This field is mandatory if Ulying Asset Class field is set to Equity. Either underlying (equity basket) or Call Ccy/Put Ccy (currency basket) is mandatory. The fields from Ulying Security to Ulying Strike Price is part of an associate multi-value set. |
| Call Ccy | Indicates the currency in which the customer buys the FX spot deal. This field is mandatory if Ulying Asset Class field is set to Currency. |
| Put Ccy | Indicates the currency in which the customer sells the FX spot deal. This field is mandatory if Ulying Asset Class field is set to Currency. |
| Weight | Indicates the weight of the currency pair or the underlying in this basket |
| Strike Percentage | Indicates the strike expressed as a percentage of spot rate. Either strike percentage or strike is mandatory for this field. |
| Ulying Strike Ccy | Indicates the currency in which the exchange rate is quoted. This field is applicable for currency basket. |
| Ulying Strike Price | Indicates the strike price of the currency pair or underlying |

**BasketOptions**

| Field | Description |
|---|---|
| Contract Terms | Indicates the value defaulted from DX.CONTRACT.TERMS if the contract terms are defined. The details defaulted from DX.CONTRACT.TERMS cannot be modified. If the value is not defined in DX.CONTRACT.TERMS , the basket details can be input directly in the trade. |
| Settlement Method | Indicates the value defaulted from DX.CONTRACT.TERMS |
| Basket Type | Indicates the value defaulted from DX.CONTRACT.TERMS |
| Ulying Asset Class | Indicates whether the underlying is an equity or currency basket. The values are: Equity Currency |
| Static Leg | Indicates if the buy or sell currency should be same in all multi-value pairs. This field is mandatory for currency basket. The values are: None Call Put |
| Ulying Security | Indicates the value defaulted from DX.CONTRACT.TERMS . This is a display-only field. |
| Call Ccy | Indicates the currency in which the customer buys the FX spot deal defaulted from DX.CONTRACT.TERMS |
| Put Ccy | Indicates the currency in which the customer sells the FX spot deal defaulted from DX.CONTRACT.TERMS |
| Weight | Indicates the weight of the currency pair or equity in the basket defaulted from DX.CONTRACT.TERMS |
| Spot Price | Indicates the spot price of the underlying equity or exchange rate of the associated currency pair |
| Strike Percentage | Indicates the strike expressed as a percentage of spot rate |
| Ulying Strike Ccy | Indicates the currency in which the exchange rate is quoted. This field is applicable for currency basket. |
| Ulying Strike Price | Indicates the strike price of the currency pair or underlying |
| Exercise | Indicates the settlement of a physically settled basket. If this field is set to Yes: A SEC.TRADE record is created for the associated underlying of the basket for an equity basket . The price and nominal in SEC.TRADE is the associated strike price and quantity, respectively. A FX deal is created for the associated currency pair for a currency basket. |
| Quantity | Indicates the number of shares to be delivered of this underlying. This multi-value field is applicable only for physical delivery method and mandatory for equity basket when the Exercise field is set to Yes. |
| Call Amount | Indicates the amount received by the customer in the Call Ccy . This multi-value field is applicable only for physical delivery method and mandatory for currency basket when the Exercise field is set to Yes. |
| Put Amount | Indicates the amount received by the customer in the Put Ccy . This multi-value field is applicable only for physical delivery method and mandatory for currency basket when the Exercise field is set to Yes. |
| Cash Exercise | Indicates if a cash pay-out is triggered for the amount and currency specified in the Cash Amount and Cash Ccy fields, respectively. This field is applicable only for cash settled baskets. |
| Cash Amount | Indicates the cash amount to be paid out for a cash settled option. |
| Cash Ccy | Indicates the currency corresponding to the Cash Amount field. |

**CDS**

| Field | Description |
|---|---|
| Contract Class | Indicates the type of instruments traded on the relative exchange. This is a mandatory field and must be set to CDS. |
| Delivery Method | Defines the delivery method for specified contract at maturity. This is a mandatory field and must be set as Physical for CDS. The physical delivery of the underlying bond or instrument is done manually, if required. |

**CDS**

| Field | Description |
|---|---|
| Contract Code | Indicates the DX.CONTRACT.MASTER ID |
| Buy or Sell | Indicates whether the customer is buying or selling the transaction as determined by the bank |
| Sec Buy Sell | Indicates whether the broker is buying or selling the transaction as determined by the bank |
| Prem Percent | Indicates the initial premium denoted as a percentage of notional amount |
| Underlying Bond | Indicates the instrument to which the CDS contract is created. This field is mandatory. |
| Bond Ccy | Indicates the defaulted trade currency. This is a display-only field. |
| Bond Value | Indicates the principal amount of the bond in asset currency |

**CDS**

| Field | Description |
|---|---|
| Prem Pay Percentage | Determines whether the premium amount is entered in trade currency or system defaults it by calculating from the percentage defined in the Prem Percent field. The values are: YES - Prem Pymt Amt is a display-only field and the system calculates and generates the amount NO - Prem Pymt Amt is updated manually |
| Prem Pymt Amt | Indicates the amount in the contract currency. When the fields Prem Pay Percentage and Prem Pymt Freq are input, this field is updated with the respective amount. |
| Prem Pymt Freq | Indicates the premium payment frequency. The values are 1–5. |
| Prem Pymt Date | Defines the premium payment date for this period. When the fields Prem Pay Percentage and Prem Pymt Freq are input, this field is updated with the respective duration which is between trade date and maturity date |

**Close Out**

| Closeout Type | Application | Enquiry | Description |
|---|---|---|---|
| Manual Closeout | DX.CO.MANUAL.INPUT | DX.CO.MANUAL.OPTION.BRWS | For options |
| DX.CO.MANUAL.FUTURE.BRWS | For futures |  |  |
| Maturity Closeout | DX.CO.MATURITY.INPUT | DX.CO.MATURITY.FUTURE.BRWS | For futures |
| Manual Exercise | DX.CO.EXERCISE.MANUAL | DX.CO.MANUAL.EXERCISE.BRWS | For options |
| Manual Expire | DX.CO.EXPIRE.MANUAL | DX.CO.MANUAL.EXPIRE.BRWS | For options |
| Manual Assign | DX.CO.ASSIGN.MANUAL | DX.CO.MANUAL.ASSIGN.BRWS | For options |
| Automatic Closeout | DX.CO.EXERCISE.AUTO |  | For options |
| DX.CO.EXPIRE.AUTO |  | For options |  |
| DX.CO.ASSIGN.AUTO |  | For options |  |
| COB Processing | DX.CO.AUTO.INPUT |  | For setting automatic closeout in DX.CUSTOMER , the Au Ct Class field is set to FUTURES, OPTIONS, BOTH or NONE. The Au Sett Type field is set to FIFO (first in first out), LIFO (last in first out) or FIFO DAY (today’s trades take precedence). The Au Sett Delay field is set to the number of days after trade when settlement or closeout occurs. |
|  |  | Setting the System Exercise in DX.CONTRACT.MASTER enables the system exercise of options during close of business (COB) |  |
|  |  | Setting the System Expiry in DX.CONTRACT.MASTER enables the system expiry of options during COB |  |

**Close Out**

| Status | Description |
|---|---|
| RUNNING | Denotes that the closeout is created and processed. The status is updated when the record in DX.CLOSEOUT is in INAU |
| ACTIVE | Denotes that the trades are matched. The status is updated when the record in DX.CLOSEOUT is authorised |
| DELETED | Denotes that the closeout is reversed |

**Close Out**

| Type | Description |
|---|---|
| SETTLEMENT | Identifies basic manual closeouts performed by the system. The field is set to Settlement when the closeout record is created from DX.CO.MANUAL.INPUT |
| MATURITY | Identifies the cash maturity settlements. The field is set to Maturity when the closeout record is created from DX.CO.MATURITY.INPUT |
| SYSTEM | Indicates the closeouts generated by the system under a specific set of circumstances. This is updated when the system is setup for automatic closeout ( System Exercise and System Expiry are set to Y) |
| EXERCISE | Indicates that the closeout records are generated from DX.CO.EXERCISE.MANUAL |
| EXPIRY | Indicates that the closeout records are generated from DX.CO.EXPIRE.MANUAL |
| ASSIGNMENT | Indicates that the closeout records are generated from DX.CO.ASSIGN.MANUAL |

**Close Out**

| Field | Description |
|---|---|
| Order Closeout | Accepts the following values: Blank - If this field is left blank, changes are not made to the current processing. This option is selected by default Close - If this field is set to Close, a DX.TRADE of the trade which is to be off-set (closed out) is filled in the Closeout Trade field |
| Closeout Trade | Contains a valid DX.TRADE ID. This is the ID of the trade that has to be offset. The system throws a validation if the order ID being input does not match the trade (that is, the instrument, strike price, maturity date, call or put indicator does not match with the trade being offset). This is to ensure that the user enters the correct ID. A context enquiry is also provided against this field to list the trades that can be offset by this order. The version to be used for creating an automatic closeout record needs to be specified in the Closeout Version field in the DX.PARAMETER application. |

**Close Out**

| Fields | Description |
|---|---|
| Settlement Ccy | Holds the currency of the cash payout |
| Settlement Amount | For cash settled options, the cash payout is calculated by the system (by comparing the spot price of the underlying against the strike price). This can be amended by the user. Cash entry is generated for this amount when the closeout is processed |
| Market Price | Holds the market price of the underlying security at the time of assignment |
| Cash Settle Ccy | Holds the delivery currency for the options with underlying as SECURITY.MASTER when the Settlement Method field is set to CASH. The exchange rate between this currency and contract currency is defined in the Delivery Ccy Rate field |
| Delivery Ccy Rate | Holds the exchange rate between contract and delivery currency |
| Settlement Instrument | The alternate settlement instrument which is settled on exercise |
| Sett Instrument Contract Size | Holds the contract size of the alternate settlement instrument which is mandatory, when settled using alternate underlying |
| Sett Instrument Price | Holds the price of the alternate settlement instrument which is mandatory, when settled using alternate underlying |
| Quote Ccy | Holds the currency in which the value in the Spot Exchange Rate field is quoted |
| Spot Exchange Rate | Holds the current exchange rate between the currency pairs of an FX option quoted in the Quote Ccy field |
| Fx Payout Currency | Holds the currency in which the payout is to be made |
| Spot Payout Rate | Holds the exchange rate between Quote Ccy and Fx Payout Currency fields |

**Close Out**

| Fields | Description |
|---|---|
| Settlement Ccy | Holds the currency of the cash payout |
| Settlement Amount | For cash settled options, the cash payout is calculated by the system (by comparing the spot price of the underlying security against the strike price). This can be amended by the user. Cash entry is generated for this amount when the closeout is processed. |
| Market Price | Holds the market price of the underlying security at the time of exercise |
| Cash Settle Ccy | Holds the delivery currency for the options with underlying as SECURITY.MASTER when the Settlement Method field is set to CASH. The exchange rate between this currency and contract currency is defined in the Delivery Ccy Rate field. |
| Delivery Ccy Rate | Holds the exchange rate between contract and delivery currency |
| Settlement Instrument | Indicates the alternate settlement instrument that is settled on exercise |
| Sett Instrument Contract Size | Holds the contract size of the alternate settlement instrument, which is mandatory when settled using alternate underlying |
| Sett Instrument Price | Holds the price of the alternate settlement instrument, which is mandatory when settled using alternate underlying |
| Quote Ccy | Holds the currency in which the Spot Exchange Rate is quoted |
| Spot Exchange Rate | Holds the current exchange rate between the currency pairs of FX option quoted in the Quote Ccy field |
| Fx Payout Currency | Holds the currency in which the payout is to be made |
| Spot Payout Rate | Holds the exchange rate between the Quote Ccy and Fx Payout Currency fields |

**Close Out**

| Application | Description |
|---|---|
| DX.EXCHANGE.MASTER | The Sett Allowed field is set to: Yes - Allows settlement or closeout on the exchange No - Disables the settlement or closeout Leaving this field blank defaults to Yes. |
| DX.CUSTOMER | The Au Ct Class field is set to FUTURES, OPTIONS, BOTH or NONE. The Au Sett Type field is set to FIFO (first in first out), LIFO (last in first out) or FIFO DAY (current day’s trades take precedence). The Au Sett Delay field is set to the number of days after trade when settlement or closeout can occur. |
| DX.CONTRACT.MASTER | The Sett Allowed field is set to: Yes - Allows the settlement or closeout No – Does not allow the settlement or closeout Blank - Defaults to DX.EXCHANGE.MASTER setting |
| DX.TRADE | The Xxx Allow Sett ( Pri Allow Sett or Sec Allow Sett ) field is set to: Yes - Allows settlement or closeout No - Prohibits auto or system settlement for the closeout |

**Close Out**

| Application | Field | Description |
|---|---|---|
| DX.CO.EXERCISE.AUTO | Contract Ccy | Indicates the contract currency of option to be exercised. The currency must be a valid currency in the CURRENCY application, and it is a mandatory field for FX OTC options. |
| Delivery Ccy | Indicates the delivery currency of option to be exercised. The currency must be a valid currency in CURRENCY , and it is a mandatory field for FX OTC options. |  |
| DX.CO.EXPIRE.AUTO | Contract Ccy | Indicates the contract currency of option to be expired. The currency must be a valid currency in CURRENCY , and it is a mandatory field for FX OTC options. |
| Delivery Ccy | Indicates the delivery currency of option to be expired. The currency must be a valid currency in CURRENCY , and it is a mandatory field for FX OTC options. |  |

**Close Out**

| Field | Description |
|---|---|
| Quote Ccy | Delivery and strike quote currencies for normal FX and generic FX OTC options, respectively |
| Spot Exchange Rate | The exchange rate between contract and the value in the Quote Ccy field |
| Fx Payout Ccy and Spot Payout Rate | The exchange rate between Fx Payout Currency and Quote Ccy fields |

**Commissions**

| ID | Description | Abbreviation |
|---|---|---|
| CU100018 | Customer 100018 | (CU = Customer Code) |
| CGINT2 | Customer Group INT2 | (CG = Customer Group) |
| CT100 | Contract Code 100 | (CT = Contract Code) |
| CCGILTS | Contract Class GILTS | (CC = Contract Class) |
| CU100018-CT100 | Customer 100018, Contract 100 | (CU = Customer Code), (CT = Contract Code) |
| CU100018-CCGILTS | Customer 100018, Contract Class GILTS | (CU = Customer Code), (CC = Contract Class) |
| CGINT2-CT100 | Customer Group INT2, Contract 100 | (CG = Customer Group), (CT = Contract Code) |
| CGINT2-CCGILTS | Customer Group INT2, Contract Class GILTS | (CG = Customer Group), (CC = Contract Class) |
| SYSTEM | Catch All | System level defaults |

**Commissions**

| Commission Type | Field Name |
|---|---|
| Commissions | Comm Charge |
| Execution fees | Exfee Charge |
| Clearing fees | Clfee Charge |
| Regulatory fees | Rgfee Charge |
| Miscellaneous fees | Misc Charge |

**Commissions**

| Field | DX.TRADE | DX.ORDER |
|---|---|---|
| Exchange Type | Indicates the types of exchange used to enter the trade | Indicates the types of exchange used to enter the order |
| Channel | Indicates the modes of transaction used to enter the trade | Indicates the modes of transaction used to enter the order |

**Derivatives Price Update**

| Field Name | Value |
|---|---|
| Interest Rate | Contract Currency |
| Sec Int Rate | Delivery Currency |
| Interest Basis | Interest Basis of the Contract Currency |
| Strike | Strike |
| Call/Put | Call Price/Put Price |
| Volatility | Call/Put Volatility |
| Underlying Price | Underlying Price or Exchange price of the two currencies |
| Und Int Price | Underlying Internal Price |

**Derivatives Price Update**

| Field | Obtained from |
|---|---|
| Fixed Rate | CURRENCY table |
| Time to Expiry | Automatically calculated from Maturity Date |
| Strike | DX.TRADE |

**Derivatives Price Update**

| Field | Description |
|---|---|
| Deal Reference | Holds the SY deal number or DX.TRADE ID |
| Valuation Ccy | Specifies the currency associated with the valuation amount |
| Valuation Amount | Specifies the valuation amount in the associated valuation currency |
| Valoren Number | For equity underlying structures, Valoren number is a unique number assigned to the structure (for example, by Telekurs), which is used subsequently for pricing data |
| Price | For equity underlying structures and options, if price per unit is available, then the valuation is derived from the price and quantity or lot size. |
| Trade Date | Date of the trade |
| B2B Reference | Back-to-back deal number |
| MTM Amount | Holds the MTM amount for DX component |

**DX Package Option**

| Fields from DX.OPTSTRUCT or PWM.PO.PARAMETER | Fields in PAYMENT.ORDER | Conditional Mapping |
|---|---|---|
| T24 Bank BIC | Ordering Customer Bic | NA |
| Po Susp Categ in PWM.PO.PARAMETER | Debit Account | NA |
| Premium Currency or Unwind Chg Ccy or Cash Ccy | Debit Ccy | Depends on the event type. For example, for unwinding event system maps the Unwind Chg Ccy field |
| Value Date | Debit Value Date | NA |
| @ID ( DX.OPTSTRUCT Reference) | Ordering Reference | NA |
| Ben Acct | Beneficiary Account No | NA |
| BIC of Beneficiary Bank | Beneficiary Bic | NA |
| Beneficiary Bank | Beneficiary Customer | NA |
| Name of Beneficiary Bank | Beneficiary Name | System maps the Name from CUSTOMER application |
| BIC of Cpty No | Acct With Bank Bic | NA |
| Cpty No | Acct With Bank Customer | NA |
| Cpty Add | Acct With Bank Swift Addr | NA |
| Bic of Intr Bank | Intermed Bic | NA |
| Intr Bank | Intermed Bank Customer | NA |
| Intr Add | Intermed Swift Addr | NA |
| Premium Currency or Unwind Chg Ccy or Cash Ccy | Payment Currency | Depends on the event type. For example, for unwinding event system maps the Unwind Chg Ccy field |
| Cpa Prem Amt , Cash Amount , Cpa Unwind Chg Amt | Payment Amount | DX.OPTSTRUCT generates MT202 from various Structured Products (SY) events. Depending on whether the amount is premium, cash settlement or unwinding charges amount, the respective fields are mapped |
| Value Date | Required Credit Value Date | NA |
| NA | Bank to Bank Info | NA |
| NA | Internal Order Details | NA |
| Bank | Order Type | NA |
| Mapped from PWM.PO.PARAMETER if set | Order Initiation Type Payment Category Payment Method Payment Purpose | NA |
| Cpa Unwind Chg Acc or Cpa Prem Acc or Cparty Cash Sett Acc or Temenos Payments to determine | Credit Nostro Account | If the value Cpa Unwind Chg Acc or Cpa Prem Acc or Cparty Cash Sett Acc field is a Nostro account and does not belong to the counterparty, then the system defaults the value in the respective field. If the account is an internal category account formed using the value in the Po Susp Categ field, then the system does not populate any value in this field. Temenos Payments determine the Nostro account |
| Bic of Cpa Unwind Chg Acc or Cpa Prem Acc or Cparty Cash Sett Acc or Temenos Payments to determine | Receiver Bic | If it is a Nostro account does not belong to the counterparty, then system defaults the Bic of the Nostro account holder. If the account is an internal category account formed using the value in the Po Susp Categ field, then the system does not populate any value in this field. Temenos Payments determine the receiver of the message |

**Exotic Options**

| Routines | Description |
|---|---|
| DX.XO.CREATE.FX | To create the underlying FX deal, user fields are not required |
| DX.XO.CREATE.SEC | To create the underlying SEC.TRADE , user fields are not required |
| DX.XO.CREATE.FX.KNOCKOUT | To create the underlying FX deal in case of knockout options, user fields are not required |
| DX.XO.CREATE.SEC.KNOCKOUT | To create the underlying SEC.TRADE in case of knockout options, user fields are not required |
| DX.XO.FWDCASHPAYOUT | To post accounting entry for settlement on closeout, the value or maturity date of option is adjusted for number of offset days, amount and currency user fields are required |
| DX.XO.INSTANT.CASHPAYOUT | To post accounting entry for settlement on closeout, the value closeout date is adjusted for number of offset days, amount and currency user fields are required |
| DX.XO.CREATE.FX.REBATE | To post accounting entry for the rebate amount in case of Knock-out options with rebate, amount and currency user fields are required |
| DX.XO.KNOCKOUT | To create underlying contracts regardless of the exotic types. If the Exotic Event flag is set and when the knock-out level is reached, the option is expired. |
| DX.XO.KNOCKIN | To create underlying contracts regardless of the exotic types. If the Exotic Event flag is set and when the knock-in level is reached, the option is valid. |

**Limits**

| Limit ID | Description | Limit | Utilisation | Remaining |
|---|---|---|---|---|
| 050027.0004552.01 | HP bond futures limit | 3M | - | - |

**MarginCalculation**

| Strategy | Description |
|---|---|
| SPREAD | Entered by buying and selling equal number of options of the same class on the same underlying security but with different strike prices or expiration dates. |
| STRADDLE | Neutral options strategy that involves simultaneously buying both a put option and a call option for the underlying security with the same strike price and the same expiration date |
| STRANGLE | Options strategy in which the investor holds a position in both a call and a put option with different strike prices, but with the same expiration date and underlying asset |
| TIME SPREAD | Options or futures spread established by simultaneously entering a long and short position on the same underlying asset at the same strike price but with different delivery months |

**Misc**

| Cont Ulying Val | Description | Forex Derivatives | Other Derivatives |
|---|---|---|---|
| No | Only for futures and options with premium un-posted | Credit (CR) or Debit (DB) Central Reporting Facility (CRF) asset type Amount – cost of position or contingent value Currency – contract currency | CR or DB CRF asset type Amount – cost of position or contingent value Currency – contract currency |
| Yes | All trades | CR CRF asset type Amount – underlying receivable ccy amount Currency – receivable currency DB CRF asset type Amount – underlying payable ccy amount Currency – payable currency | CR and DB CRF asset type Amount – cost of position Currency – contract currency |

**Misc**

| Applications | Description |
|---|---|
| DX.PARAMETER | The Special Rate field in DX.PARAMETER defines the class of customer for whom special rates are to be applied. When this field is left blank, it defaults the mid rates for calculations |
| DX.CUSTOMER | The best rate method is applied based on the customer type defined in the Special Rate field in DX.PARAMETER . For example, if the Special Rate in DX.PARAMETER field is set as dealer, then best rate is applied for transaction where the customer with Customer Type field in DX.CUSTOMER is set to Dealer |
| DX.TRADE | The rate at which conversion takes place is populated in Pri Prem Exc and Pri Comm Exc fields based on the definition in DX.PARAMETER . These fields can be overwritten for user-defined rates if the primary side of the DX.TRADE involves manual commission. |

**Misc**

| Table Name | Description |
|---|---|
| DX.PARAMETER | The Cr Exp Calc Api field contains the API black box routine (DX.BB.CREDIT.EXPOSURE) created for calculating credit exposure |
| DX.CONTRACT.MASTER | The Int Rate Contract field is used to identify an interest rate derivative. When set to Yes, it is mandatory to enter a value in Life Underlying field |
| REVAL.ADDON.PERCEN | Based on the sub-asset type, add on percentage applicable for regulatory and credit reporting needs to be defined in the record in REVAL.ADDON . |

**Misc**

| Field | Description |
|---|---|
| Margin Difference | Controls the posting of margin amount. |
| Price Order | Defines the order in which the price sets related fields should be searched to find the missing prices. |
| Price To Store and Price Days | Defines the period of storing the price sets related fields. Different period can be setup for each different price sets (CURRENT, CLOSING and WHATIF). |
| Suppress Underlying | Controls the creation of underlying during closeout process. |
| Fwd Post Eod | Posts the forward postings held in DX.FW.POSTINGS either in the start or end of business day by setting the Fwd Post Eod field accordingly. |
| Cost Calc Api and Cr Exp Calc Api | Facilitates configuring routines to calculate the net cost and credit exposure of the DX transaction. |
| B2b Active | Activates the back-to-back closeout processing when this field is set to Yes. |
| Closeout Version | Defines the version used for auto closeout by square-off order. |
| Cont Ulying Val | Allows the off-balance sheet postings made on entry of an own-book deal, to be based solely on the underlying value of the trade. |
| Sc Asset Upd | Defines the way of updating Asset Position details for Derivative trades. By Positional, the system updates the cumulative position of trades and update the price accordingly. By transactional, it updates the position for each trade separately. |
| Special Rate | Defines the class of customer, for whom special rates are to be applied. When this field is left blank, it defaults the mid rates for calculations. |
| Check Cust Funds | When set to Yes, system calculates the best estimated initial margin figure for each order or trade entered. |
| Vm Reversal Style | Controls the reversal of variation margin for foreign currency contracts. |
| Vm Rev Type | Manages whether all variation margin entries are reversed with effective date. |

**Misc**

| Field | Description |
|---|---|
| Barrier Trigger | Denotes whether the defined option is a barrier or trigger field type. |
| Exercise Expire | Depicts whether the exotic option is meant as a kick-in or kick-out event, with respect of being set to Exercise or Expire. |

**Order Processing**

| Status | Description |
|---|---|
| Open | Initial capture of the order in the system |
| Transmitted | Order is placed with the exchange and acknowledged by the exchange |
| Partial | Order is partially filled, that is, partial execution |
| Filled | Order is fully executed |
| Cancellation Request | Request to cancel the pending lots placed with the market |
| Cancelled | Cancellation request accepted by the exchange |
| Modification Request | Modification of pending lots placed with the exchange |
| Expired | Order is expired |

**Static setup**

| Event code | Name | Description |
|---|---|---|
| CI | Contract inception | Initial entry of trade |
| CC | Contract cancellation | Cancellation of an authorised contract (contract reversal not part of an amendment and the contract completely cancelled) |
| CD | Contract deletion | Deletion of an unauthorised contract |
| CU | Contract unauth amendment | Amendment of an unauthorised contract |
| CR | Contract amendment reversal | Reversal of authorised trade details before amended details are entered |
| CA | Contract amendment | Amendment of authorised trade (new details) |
| CM | Contract maturity | Trade maturity |
| CS | Contract settlement | Settlement of trade (closeout) |
| PS | Partial Settlement | Partial settlement of lots |
| SR | Settlement reversal | Reversal of settlement (closeout) |
| PP | Premium posting | Posting of option premium |
| FC | Commission posting | Posting of Normal trading commission |
| FE | Execution fee posting | Posting of execution fees |
| FR | Regulatory fee posting | Posting of regulatory fees, if any |
| FL | Clearing fee posting | Posting of clearing fees |
| FM | Miscellaneous fee posting | Posting of any other miscellaneous charges entered manually |
| PO | Open position | Trade input forming opening position leg |
| PC | Close position | Trade input forming closing position leg |
| RP | Realised P&L | Realised P&L from the following: Maturity settlement Revaluation using nightly settlement conventions (for example, LIFFE settlement and reopen process) |
| UO | Unrealised option value | Unrealised option value generated by revaluation (not the variation margin as the product is not from mark-to-market or similar) |
| OA | Order amendment | Amendment of authorised order - new details |
| OC | Order cancellation | Cancellation of an authorised order |
| OD | Order deletion | Deletion of an unauthorised order |
| OF | Order fill | Fill or part-fill of an order, when the trade is created |
| OI | Order input | Input of an order and authorisation |
| OM | Option margin (Market Value) | Margin at market value |
| OX | Order abandon | Lots cancelled after a minimum of one partial fill |
| TT | Tax Posting | Posting of tax |
| IM | Initial Margin | Initial margin generated from revaluation |
| VM | Variation Margin | Variation margin (unrealised P&L) generated and posted by revaluation for futures |

**Static setup**

| ID | Event Description | Requires CATEG.CODE | Generated By. |
|---|---|---|---|
| BV | Back valuation | NO | Back Valuation |
| BP | Broker profit | YES | Trade |
| FL | Clearing fee/CSN posting | YES | Trade |
| PC | Closed position | YES | Trade |
| FC | Commission posting | YES | Trade |
| CA | Contract amendment | YES | Trade |
| CR | Contract amendment (reversal) | YES | Trade |
| AS | Contract assignment | NO | Closeout |
| AR | Contract assignment (reversal) | NO | Closeout |
| CC | Contract cancellation | YES | Trade |
| EX | Contract exercise | NO | Closeout |
| ER | Contract exercise (reversal) | NO | Closeout |
| XP | Contract expiry | NO | Closeout |
| XR | Contract expiry (reversal) | NO | Closeout |
| CI | Contract inception | YES | Trade |
| CM | Contract maturity | YES | Trade |
| CS | Contract settlement | YES | Closeout |
| CP | Corporate action | NO | Corporate Actions |
| CX | Corporate action (reversal) | NO | Corporate Actions |
| FE | Execution fee/CSN posting | YES | Trade |
| CO | External transfer | NO | Tr/Pos Transfer |
| CT | Incoming transfer | NO | Tr/Pos Transfer |
| IM | Initial margin | YES | Re Valuation |
| II | Internal incoming transfer | NO | Tr/Pos Transfer |
| CN | Internal transfer | NO | Tr/Pos Transfer |
| FM | Misc fee posting | YES | Trade |
| PO | Open position | YES | Trade |
| OM | Option variation margin | YES | Re Valuation |
| OX | Order abandon | YES | Order |
| OA | Order amendment | YES | Order |
| OB | Order blocking | YES | Order |
| OC | Order cancellation (reversal) | YES | Order |
| OD | Order deletion | YES | Order |
| OF | Order fill | NO | Order |
| OI | Order input | YES | Order |
| OR | Order stage superseded | NO | Order |
| PP | Premium posting | YES | Trade |
| RP | Realised P and L | YES | Closeout |
| FR | Regulatory fee posting | YES | Trade |
| SR | Settlement reversal | YES | Closeout |
| TT | Tax posting | YES | Trade |
| CU | Unauth contract amendment | YES | Trade |
| CD | Unauth contract deletion | NO | Trade |
| UO | Unrealised option P and L | YES | Re Valuation |
| VM | Variation margin | YES | Re Valuation |

**Swaptions**

| Field | Description |
|---|---|
| Contract Code | Links the DX.CONTRACT.MASTER ID value, which in turn links the transaction level data with the relevant instrument static data |
| Call or Put | Confers upon the holder the right, but not obligation, to buy or sell the stock at a fixed price at a future date. Select CALL option for swaptions |
| Buy or Sell | Indicates whether the customer is buying or selling the transaction as determined by the bank |
| Sec Buy Sell | Indicates whether the broker is buying or selling the transaction as determined by the bank |
| Strike Price | Indicates the fixed rate at which the swaption contract is entered |
| Prem Percent | Indicates the initial premium denoted as a percentage of notional amount |
| Prem Pymt Amt | Indicates the premium amount value derived based on the values in Prem Percent and Asset Principal |
| Swap Delivery | Indicates whether the delivery method is CASH or PHYSICAL for swaption contracts |
| Swap Mat Date | Indicates the maturity date of swaption contract |
| Payment Type | Indicates whether the payment type is fixed. The values are: FIXED - The field As Fixed Rate should have values and cannot be left blank FLOATING - The field As Floating should have values and cannot be left blank This field is applicable only when the primary customer makes the pay amount an asset. |
| Receive Type | Indicates whether the receive type is fixed. The values are: FIXED - The field Lb Fixed Rate should have values and cannot be left blank FLOATING - The field Lb Floating should have values and cannot be left blank This field is applicable only when the primary customer makes the pay amount a liability. |

**SWIFT MT306 for Exotic Options**

| Field | Description |
|---|---|
| Exercise Expire | Defines the nature of the barrier event. The allowed values are: Exercise - This option knocks in (in case of the vanilla option) or qualifies for cash payment (in case of the binary option) when the barrier is breached. Expire - This option is knocked out (in case of the vanilla option) or disqualifies for cash payment (in case of the binary option). |
| Upper or Lower | Defines whether the barrier is upper or lower. Based on the setup, the value from this field is mapped to the MT306 message. For the Upper Barrier Level TAG 37J is mapped and for the Lower Barrier Level TAG 37L is mapped. |
| Event Time Type | Specifies the period when a barrier is evaluated. This field accepts the following values: CONT – Indicates that barrier evaluation occurs on a continuous basis. DISC – Indicates that barrier evaluation occurs at a discrete point in time. The time must be mandatorily updated in DX.TRADE . This field is mapped to Tag 14M in Sequence F of the MT306 message. For Double or Dual Barrier contracts, the system must validate that either both barriers are ‘continuous’ or both are ‘discrete’. The system does not allow one barrier to be ‘continuous’ and the other to be ‘discrete’. Depending on the value defined in Event Time Type , additional information (tags) needs to be mapped in the MT306 message. CONT – Indicates either Tag 29O - Continuous Time Period or Tag 14N - Spot Market can be present, but not both. DISC – Indicates either 29J Barrier Event Determination Time or 14O Barrier Event Determination Time Source must be present, but not both. |

**SWIFT MT306 for Exotic Options**

| Type of Barrier | Description |
|---|---|
| UIKI - Up and In Knock-in Event | An event that occurs when the spot rate is greater than or equal to the barrier level. If the event has occurred, the buyer of the option has the right to exercise it. If the event has not occurred, the option expires without any value. |
| DIKI - Down and In Knock-in | An event that occurs when the spot rate is less than or equal to the barrier level. If the event has occurred, the buyer of the option has the right to exercise it. If the event has not occurred, the option expires without any value. |
| UOKO - Up and Out Knock-out | An event that occurs when the spot rate is greater than or equal to the barrier level. If the event has occurred, the option expires without any value. If the event has not occurred, the buyer of the option shall have the right to exercise it. |
| DOKO - Down and Out Knock-out | An event that occurs when the spot rate is less than or equal to the barrier level. If the event has occurred, the option expires without any value. If the event has not occurred, the buyer of the option has the right to exercise it. |
| DKIN - Double Knock-in | An event that occurs when the spot rate is either, Greater than or equal to the upper barrier level, or Less than or equal to the lower barrier level If the event has occurred, the buyer of the option has the right to exercise it. If the event has not occurred, the option expires without any value. |
| DUKI - Dual Knock-in | An event that occurs when both the following events have happened: The spot rate is greater than or equal to the upper barrier level The spot rate is less than or equal to the lower barrier level If the event has occurred, the buyer of the option has the right to exercise it. If the event has not occurred, the option expires without any value. |
| DKOT - Double Knock-out | An event that occurs when the spot rate is either, Greater than or equal to the upper barrier level, or Less than or equal to the lower barrier level If the event has occurred, the option expires without any value. If the event has not occurred, the buyer of the option has the right to exercise it. |
| DUKO - Dual Knock-out | An event that occurs when both the following events have happened: The spot rate is greater than or equal to the upper barrier level The spot rate is less than or equal to the lower barrier level If the event has occurred, the option expires without any value. If the event has not occurred, the buyer of the option has the right to exercise it. |

**SWIFT MT306 for Exotic Options**

| Field | Value |
|---|---|
| Barrier Type | UIKI, DIKI |
| Option Variant | VANI |
| Barrier Evaluation | CONT, DISC |
| Exotic Type.1 | CONT.KNOCKIN, DISC.KNOCKIN |

**SWIFT MT306 for Exotic Options**

| Field | Value |
|---|---|
| Barrier Type | UOKO, DOKO |
| Option Variant | VANI |
| Barrier Evaluation | CONT, DISC |
| Exotic Type.1 | CONT.KNOCKOUT, DISC.KNOCKOUT |

**SWIFT MT306 for Exotic Options**

| Field | Value |
|---|---|
| Barrier Type | UIKI, DIKI |
| Option Variant | BINA |
| Barrier Evaluation | CONT, DISC |
| Exotic Type.1 | CONT.KNOCKIN, DISC.KNOCKIN |
| Exotic Type.2 | CASH.PAYOUT |

**SWIFT MT306 for Exotic Options**

| Field | Value |
|---|---|
| Barrier Type | UOKO, DOKO |
| Option Variant | BINA |
| Barrier Evaluation | CONT, DISC |
| Exotic Type.1 | CONT.KNOCKOUT, DISC.KNOCKOUT |
| Exotic Type.2 | CASH.PAYOUT |

**SWIFT MT306 for Exotic Options**

| Field | Value |
|---|---|
| Barrier Type | DKIN |
| Option Variant | VANI |
| Barrier Evaluation | CONT, DISC |
| Exotic Type.1 | CONT.LOWER.KNOCKIN, DISC.LOWER.KNOCKIN |
| Exotic Type.2 | CONT.UPPER.KNOCKIN, DISC.UPPER.KNOCKIN |

**SWIFT MT306 for Exotic Options**

| Field | Value |
|---|---|
| Barrier Type | DKOT |
| Option Variant | VANI |
| Barrier Evaluation | CONT, DISC |
| Exotic Type.1 | CONT.LOWER.KNOCKOUT, DISC.LOWER.KNOCKOUT |
| Exotic Type.2 | CONT.UPPER.KNOCKOUT, DISC.UPPER.KNOCKOUT |

**SWIFT MT306 for Exotic Options**

| Field | Value |
|---|---|
| Barrier Type | DUKI |
| Option Variant | VANI |
| Barrier Evaluation | CONT, DISC |
| Exotic Type.1 | CONT.LOWER.KNOCKIN, DISC.LOWER.KNOCKIN |
| Exotic Type.2 | CONT.UPPER.KNOCKIN, DISC.UPPER.KNOCKIN |

**SWIFT MT306 for Exotic Options**

| Field | Value |
|---|---|
| Barrier Type | DUKO |
| Option Variant | VANI |
| Barrier Evaluation | CONT, DISC |
| Exotic Type.1 | CONT.LOWER.KNOCKOUT, DISC.LOWER.KNOCKOUT |
| Exotic Type.2 | CONT.UPPER.KNOCKOUT, DISC.UPPER.KNOCKOUT |

**SWIFT MT306 for Exotic Options**

| Field | Value |
|---|---|
| Barrier Type | DKIN |
| Option Variant | BINA |
| Barrier Evaluation | CONT, DISC |
| Exotic Type.1 | CONT.LOWER.KNOCKIN, DISC.LOWER.KNOCKIN |
| Exotic Type.2 | CONT.UPPER.KNOCKIN, DISC.UPPER.KNOCKIN |
| Exotic Type.3 | CASH.PAYOUT |

**SWIFT MT306 for Exotic Options**

| Field | Value |
|---|---|
| Barrier Type | DKOT |
| Option Variant | BINA |
| Barrier Evaluation | CONT, DISC |
| Exotic Type.1 | CONT.LOWER.KNOCKIN, DISC.LOWER.KNOCKIN |
| Exotic Type.2 | CONT.UPPER.KNOCKOUT, DISC.UPPER.KNOCKOUT |
| Exotic Type.3 | CASH.PAYOUT |

**SWIFT MT306 for Exotic Options**

| Field | Value |
|---|---|
| Barrier Type | DUKI |
| Option Variant | BINA |
| Barrier Evaluation | CONT, DISC |
| Exotic Type.1 | CONT.LOWER.KNOCKIN, DISC.LOWER.KNOCKIN |
| Exotic Type.2 | CONT.UPPER.KNOCKIN, DISC.UPPER.KNOCKIN |
| Exotic Type.3 | CASH.PAYOUT |

**SWIFT MT306 for Exotic Options**

| Field | Value |
|---|---|
| Barrier Type | DUKO |
| Option Variant | BINA |
| Barrier Evaluation | CONT, DISC |
| Exotic Type.1 | CONT.LOWER.KNOCKIN, DISC.LOWER.KNOCKIN |
| Exotic Type.2 | CONT.UPPER.KNOCKOUT, DISC.UPPER.KNOCKOUT |
| Exotic Type.3 | CASH.PAYOUT |

**Transaction Fees and Charges**

| ID | Description | Abbreviation |
|---|---|---|
| CU100018 | Customer 100018 | (CU = Customer Code) |
| CGINT2 | Customer Group INT2 | (CG = Customer Group) |
| CT100 | Contract Code 100 | (CT = Contract Code) |
| CCGILTS | Contract Class GILTS | (CC = Contract Class) |
| CU100018-CT100 | Customer 100018, Contract 100 | (CU), (CT) |
| CU100018-CCGILTS | Customer 100018, Contract Class GILTS | (CU), (CC) |
| CGINT2-CT100 | Customer Group INT2, Contract 100 | (CG), (CT) |
| CGINT2-CCGILTS | Customer Group INT2, Contract Class GILTS | (CG), (CC) |
| SYSTEM | Catch All | System-level defaults |

**Transaction Fees and Charges**

| Commission Type | Field Name |
|---|---|
| Commissions | Comm Charge |
| Execution fees | Exfee Charge |
| Clearing fees | Clfee Charge |
| Regulatory fees | Rgfee Charge |
| Miscellaneous fees | Misc Charge |

**Transaction Fees and Charges**

| Field | DX.TRADE | DX.ORDER |
|---|---|---|
| Exchange Type | Indicates the types of exchange used to enter the trade | Indicates the types of exchange used to enter the order |
| Channel | Indicates the modes of transaction used to enter the trade | Indicates the modes of transaction used to enter the order |

**Transaction Fees and Charges**

| Field Name | Value |
|---|---|
| Charge Tax Type | Transaction Tax |
| Charge Tax Desc | Transaction Tax |
| Charge Tax Cat | 17200 |
| Chg Tax Cr Code | 80 |
| Chg Tax Dr Code | 30 |
| Chg Tax Cust Brok | Customer |
| Post Lcy | Yes |

**Misc**

| Term | Description |
|---|---|
| Article 235 | The council regulation (EC), which governs conversion and rounding rules for euro conversion. |
| EMU | European Monetary Union. |
| NCU | National Currency Unit – a general term for existing national currencies. |
| In-currency | A currency that is converting to EUR. |
| Out-currency | A currency that is not a member of EMU. |
| Triangulation | The process of converting one In-currency amount to another through the euro. |
| Re-denomination | Process of converting an In-currency transaction to the euro equivalent of something, which is at the fixed conversion rate. |
| Transition Phase | The phase where both NCU and EUR can be used. ERI (Euro Related Information) is added to SWIFT messages where the amount is converted from NCU to EUR. |

**Misc**

| S.No. | Parameters | Description |
|---|---|---|
| 1. | COUNTRY | This application allows the user to define the code EU as Euro need its own country code. In addition, Geographical Block field must be defined from the available dropdown geographies. |
| 2. | CURRENCY | This application allows the user to define the currency record for EUR. In addition, user must ensure that correct quotation code is defined. User must not define Fixed Ccy , Fixed Rate and Fixed Start Date for EUR Currency. |
| 3. | CURRENCY.PARAM | This application allows the user to define the common characteristics of Euro. In addition, Base CCY Rank must also be defined. |
| 4. | FORWARD.RATES | This application allows the user to define the premium or discount expected for the exchange rate of the Euro against the local currency when it is Out- Currency. However, if involved currency is In-Currency type, premium or discount must not be applied for the Euro. |
| 5. | HOLIDAY | This application allows the user to define the public holidays for EU, for the calendar years over which the bank's current business is spread. |
| 6. | PEIRODIC.INTEREST | This application allows the user to default the interest rate for any time period, which can be used by applications like foreign exchange on forward contracts using interest revaluation method or loans and deposits applications to perform automatic rollover. For Euro module, periodic interest must be defined with forward euro interest rates. |
| 7. | BASIC.INTEREST | This application allows the user to define floating rates – Base Rate, Prime Rate and Overnight Rate. Whenever there is a change in the rate, user must define the interest rates for the currency with the date on which it becomes active. A record must be defined for Euro with the applicable rates along with effective date. |
| 8. | EU.PARAMETER | This application allows the user to define the following: Company code – Code of the company where local currency is converted. Routine to calculate the new Euro account number. Default category for internal suspense accounts when converting contracts from one currency to fixed currency. Internal account category code to be used for posting adjustment entries in the new local currency after the conversion of the base currency has taken place. Transaction code used for all adjustment entries posted by the conversion process. The rate used to convert local currency amounts from Original Lcy to Converted Lcy . |
| 9. | PM.CALENDAR | This application allows the user to define a calendar in which possible settlements is allowed for Euro. |

**Misc**

| S.No. | Parameter | Description |
|---|---|---|
| 1. | COMPANY | Contains details such as company's name, mnemonic, classification details, applications that are to be run, company level defaults and parameters. |
| 2. | DATES | Each company has a Date record, which contains the run dates for the previous, current and the next working day. Batch (overnight) processing system updates the record automatically. |
| 3. | CONDITION.PRIORITY | Used to specify the data elements to determine the condition groups for each application. In addition, the order of general conditions to be applied when more than one general condition is involved can also be defined. |
| 4. | COUNTRY.GROUP | Used to group the countries based on residence or non-residence when applying charges. |
| 5. | COUNTRY | Contains the static details of each country such as country name, currency code and so on. The key for this application must be a standard I.S.O country code. The CURRENCY codes must be in the system before setting up the country parameter. |
| 6. | EB.TIME.ZONES | Defines the standard zones that have uniform mandated standard time. The ID must be a valid time zone name as specified in the Internet Assigned Numbers Authority (IANA) time zone database. |
| 7. | HOLIDAY | - Indicates the public holidays for each country, or region within a country for the calendar year. |
| 8. | LANGUAGE | Identifies the languages that are to be used in the system when defining multi-language fields. The Abbreviation code assigned to each Language is used as a screen prompt. |
| 9. | INTEREST.BASIS | Determines the component for interest calculation based on the inputs provided in the INT.BASIS field. |
| 10. | CURRENCY.PARAM | Contains the common details such as Numeric Currency Code , Currency Name , Number of Decimal Places and the Interest Basis for each currency. This table ensures that the same numeric code and no of decimals are used on all the different currency files. |
| 11. | CURRENCY.MARKET | Helps to identify the correct exchange and revaluation rates to be applied for each currency. |
| 12. | TRANSACTION | Contains information about all the Transaction Codes that can be used in Temenos Transact . |
| 13. | SECTOR | Sector codes are defined in this table and assigned to each Customer record to group them into broad classifications like Private Sector, Public Sector, and Corporate Banks and so on. |
| 14. | INDUSTRY | Helps to define and assign the Industry codes to each Customer record to identify the industry of the customer. |
| 15. | CATEGORY | Category codes are used to classify financial transactions in Temenos Transact according to the type of business operation or product. |
| 16. | AC.CONSOLIDATE.COND | Allows the user to define the rules for the consolidation of entries for either an Account or a Category record. |
| 17. | INTERCO.PARAMETER | Determines if automatic balancing entries are raised when processing transactions in a multi-company or a multi-department (in the same company) environment. |
| 18. | EB.DUPLICATE.TYPE | Defines duplicate check criteria for applications. |
| 19. | EB.LOOKUP | This is a generic template to hold all the lookups for data access service. The user can create an EB.LOOKUP record with the definition and use them as drop-down list in applications. |
| 20. | EB.SYSTEM.ID | Provides a description for the SYSTEM.ID field in the accounting entry files, which include STMT.ENTRY , CATEG.ENTRY , CONSOL.NET.TODAY and RE.CONSOL.SPEC.ENTRY . |
| 21. | CONSOLIDATE.COND | The consolidation records hold the consolidation key, series of balance, total debit and credit movement fields. The details are held in for: • Asset and Liability • Profit and Loss |
| 22. | GROUP.ACCRUAL.PARAM | This is a parameter file, which holds the options for the bulk accrual of accounts. It reduces the number of accrual accounting entries by consolidating at various levels. |
| 23. | EB.LOCAL.CONTENT.TABLE | Stores local context-data on customer records at BNK level. |
| 24. | ST.ORGANIZATION.STRUCTURE | Holds the organizational hierarchy of the bank. |
| 25. | ST.ORGANIZATION.CODE | Helps to create Organization Codes at each level defined in the ST.ORGANIZATION.STRUCTURE application. |
| 26. | ST.BRANCH | Holds the branch record, which is updated on authorising the ST.ORGANIZATION.CODE record defined for each branch. |
| 27. | ST.LINE.OF.BUSINESS | Line of Business is defined to create different Cost Centers for the bank and align them later to a particular branch depending on its requirement. |
| 28. | CUSTOMER.EXIT.STATUS | Allows the bank to define the exit statuses and the exit reasons for each customer type (Prospect and Customer). It holds the details such as, allowed customer types, allowed exit reasons. Further, it helps to reclassify a bank Rejected Prospect or Closed (Customer) back to its default or original status. |
| 29. | COMPANY.CREATE | Contains details, such as, Company's Name, Address, Mnemonic, Sub Division code, Creation Date and Default Company details. Allows user to create COMPANY record manually and from which data gets auto-populated in COMPANY application. |
| 30. | ST.CUSTOMER.CLOSURE.PARAM | Customer Exit Status . This parameter application is used to configure the following: Enable Customer Closure - This field can be entered only in the SYSTEM record. The user can select the provided check box to enable the customer closure process and perform the pre-closure checks. Define the pre-closure conditions - The Transact core and non-core applications that must be checked for the presence of the customer data before the customer is closed, can be defined as individual records in this table. The user can define the following attributes in these records where ID of the record will be populated with the application name. Application Access Type - This field is used to define the method through which the customer can be identified in the records of the application specified in the ID. This field will have two options: Field - Denotes that the system must access a particular field of the application to identify the customer ID - The system must use the ID of the record to identify the customer. Application Access Link - The user can provide a field name that will be referred to identify the presence of the customer data. |

**Misc**

| S.No. | Parameter | Description |
|---|---|---|
| 1. | TARGET | Target codes defined in this table are assigned to Customer records in Temenos Transact to indicate how the customer fits in with the Bank's overall marketing strategy. |
| 2. | CUSTOMER.STATUS | Customer Status codes defined in this table are assigned to Customer records in Temenos Transact to classify the customers based on the criteria defined locally. |
| 3. | RELATION | Helps to specify the various types of relations that can exist between Customers and, or Person Entities. |
| 4. | CUST.GROUP.PURPOSE | Defines the rules for a Customer Group based on the purpose of the group. The rules include where the customer group can be used and how the customers and parties in the group can be stored. |
| 5. | PARTY.RELATIONSHIP | Used to define multiple relationships between customers. |
| 6. | DEPT.LEVEL | Contains the valid levels of departmental hierarchy that are permitted in the system. |
| 7. | DEPT.ACCT.OFFICER | Used to identify each Department and Account Officer in the bank by means of a code. Each Customer record has an Account Officer code assigned, which helps to generate the M.I.S reports at the Account Officer level. |
| 8. | ST.CDM.PARAMETER | Holds the parameter configurations for customer dormancy processing at the lead company level. |
| 9. | ST.CUSTOMER.ACTIVITY.PARAMETER | This is a Parameter setup table, which helps to maintain the data relation details for the applications and it is enhanced to configure Access Type and Link for Joint account holders as well. JH.ACCESS.TYPE - This field determines on how the application can be accessed to get the list of personal data for joint account holders. JH.ACCESS.LINK - This field provides the link of accessing the application for personal data for joint account holders. |
| 10. | COUNTRY.RULES | Helps to define the country specific rules. |
| 11. | ADDRESS.RULES | Helps to define the country specific address rules for each country. |
| 12. | COUNTRY.PARAMETER | Helps to check the address rule that has to be applied to get the address details of the customer in a particular company. |
| 13. | ADDRESS.OUTPUT.FORMAT | Helps to define the various address output formats from which the user can choose the output formats. |
| 14. | ADDRESS.OUTPUT.RULES | Helps to define the Address Output Rules used for a country. |
| 15. | CONTACT.TYPE.PARAMETER | Helps the user to define the characteristics of each contact type captured in the CUSTOMER application. |
| 16. | ST.REG.EXCLUDE.PARAM | Exclusion Parameter setup is used to skip the customer activity. PARTY.APPLICATION – This field specifies the Party application for which the exclude criteria is going to define. (For now, this field is defaulted with 'CUSTOMER'). FIELD.NAME –This field specifies the field name from the party application to define the exclude criteria. OPERAND – This field specifies the operand that connects the field name and value. FIELD.VALUE – This field specifies the value for the respective field name mentioned to define the exclude criteria. |

**Misc**

| S.No. | Parameter | Description |
|---|---|---|
| 1. | BASIC.RATE.TEXT | Defines descriptions of the Basic Interest Rate table IDs to enable the user to identify each one of them easily. |
| 2. | BASIC.INTEREST | Defines and stores the frequently used floating rates accessed by Temenos Transact applications when required. |
| 3. | PERIODIC.INTEREST | Defines the interest rates based on the time period for each currency. |
| 4. | ST.PERIODIC.INTEREST | Acts as an index for PERIODIC.INTEREST . This application can be either manually created or through the ST.CREATE.PERIODIC.INDEX service. |

**Misc**

| S.No. | Products | Description |
|---|---|---|
| 1. | SECTOR | 141 – Common Sector 1001 – Individual 1002 – Staff 1002 – Director 2000 – Corporate 3000 - Banks |
| 2. | INDUSTRY | 1000 – Private Person 1050 – Textile and Garments 1200 – Staff 1600 – Non Profit Institutions |
| 3. | CATEGORY | 1000 – Demand Account 1001 – Current Account 1002 – CurrAcc with OD 1003 – Premium C/A |
| 4. | Exit Status | The below values can be held for exit status field: Rejected Deceased Closed Undesirable |


### Derivatives_Structured_Products - PT (PT)


**PT**

| S. No | Term Sheet Element | Description |
|---|---|---|
| 1. | Value Date | Effective date of the contract |
| 2. | Currency bought | The currency the investor buys |
| 3. | Currency sold | The currency sold by the investor |
| 4. | Call amount | The amount bought in each settlement period |
| 5. | Put amount | The amount sold in each settlement period |
| 6. | Fixing schedule | Periodical settlement frequency |
| 7. | Strike exchange rate | The strike exchange rate for the option |
| 8. | Knock out price | When this barrier price is breached, the option is knocked out. |
| 9. | Maturity date | Maturity date of the contract |

**PT**

| S. No | Event | Description |
|---|---|---|
| 1. | Inception | The contract is recorded in the system. The underlying option deals are created. |
| 2. | Fixing | This is the periodical settlement event. The spot exchange rate is compared against the strike exchange rate, the decision is made to either exercise the long option or assign the short option. If the long option is partially exercised, then the short option needs to be partially expired. If the short option is partially assigned, then the long option needs to be partially expired. |
| 3. | Knock out | Both the long option and the short option can have knock-out features. When both the options are knocked out, the contract itself can be knocked out. |
| 4. | Unwinding | The contract can be terminated early. |
| 5. | Maturity | On maturity date, the contract ceases to exist. |

**PT**

| S. No | Variant | Description |
|---|---|---|
| 1. | PF | In this variant, the PF or TARKO contract gets knocked out when the knock-out barrier is breached. |
| 2. | TARKO | In this variant, the PF or TARKO contract gets knocked out when the accumulated profit reaches a pre-defined level. |
| 3. | With Vanilla option | Some variants include a vanilla option which does not have a knock-out feature. |
| 4. | FX Accumulator or Decumulator | In this variant, the fixing schedule of the long and short option is the same. The notional amount of the short option would be the leveraged notional amount. |

**PT**

| Field | Description |
|---|---|
| Variant | Refers to a particular variant, then the variant can be linked in this field. Once linked, the parameters and configurations defined for the variant would be used in processing the life cycle of the contract. |
| Currency Bought | Holds the currency that the customer buys |
| Currency Sold | Holds the currency that the customer sells |
| Trade Date | Holds the trade date of the contract. Trade date cannot be forward dated and should fall between the First Date and Last Date of the corresponding product definition record. |
| Maturity Date | Maturity date is the termination date of the contract. Maturity date will be defaulted based on Term and Value Date . |
| Premium Pay Receive | Indicates whether the customer have to pay or receive the premium amount |

**PT**

| Element | Description |
|---|---|
| Value Date | Effective date of the contract |
| Currency bought | The currency the investor buys |
| Currency sold | The currency sold by the investor |
| Call amount | The amount bought in each settlement period |
| Put amount | The amount sold in each settlement period |
| Fixing schedule | Periodical settlement frequency |
| Strike exchange rate | The strike exchange rate for the option |
| Knock out price | When this barrier price is breached, the option is knocked out. |
| Maturity date | Maturity date of the contract |

**PT**

| Event | Description |
|---|---|
| Inception | The contract is recorded in the system. The underlying option deals are created. |
| Fixing | This is the periodical settlement event. The spot exchange rate is compared against the strike exchange rate, the decision is made to either exercise the long option or assign the short option. If the long option is partially exercised the short option needs to be partially expired. If the short option is partially assigned the long option needs to be partially expired. |
| Knock out | Both the long option and the short option can have a knock out features, when both the options are knocked out, the contract itself can be knocked out. |
| Unwinding | The contract can be early terminated. |
| Maturity | On maturity date, the contract ceases to exist. |

**PT**

| Variant | Description |
|---|---|
| PF | In this variant, the Participating Forwards and TARKO contract gets knocked out when the knock out barrier is breached. |
| TARKO | In this variant, the Participating Forwards and TARKO contract gets knocked out when the accumulated profit reaches a pre-defined level. |
| With vanilla option | Some variants include a vanilla option, which does not have a knock out feature. |
| FX Accumulator and Decumulator | In this variant, the fixing schedule of the long and short option is the same. The notional amount of the short option is the leveraged notional amount. |

**PT**

| FOREX fields | Mapped for Customer Leg FX (Transaction against Customer) | Mapped for Counterparty Leg FX(Transaction against Counterparty) |
|---|---|---|
| Buy Currency | Sell Currency | Buy Currency |
| Sell Currency | Buy Currency | Sell Currency |
| Amount Bought | B Lev Sched Put Amt | B Lev Sched Call Amt |
| Amount Sold | B Lev Sched Call Amt | B Lev Sched Put Amt |
| Deal Type | SP | SP |
| Counterparty | Customer | Counterparty |
| Dealer Desk | Dealer Desk | Dealer Desk |
| Value Date Buy | B Settlement Date | B Settlement Date |
| Value Date Sell | B Settlement Date | B Settlement Date |
| Base Ccy | Base Ccy | Base Ccy |


### Derivatives_Structured_Products - SY (SY)


**DigitalInvestments**

| Event | Description |
|---|---|
| Inception | The contract is recorded in the system and the underlying option deal and deposit are created |
| Fixing | The fixing decision is made and the investor receives minimum or maximum rate, depending on the spot exchange rate, in comparison with the upper and lower barriers |
| Maturity | The contract expires on the maturity date and the deposit is redeemed |

**Dual and Triple Currency Investments**

| Term Sheet Element | Description |
|---|---|
| Value Date | Effective date of the deposit |
| Deposit Currency | Currency of the deposit |
| Deposit amount | The principal investment amount |
| Alternate Currency | Alternate currency |
| Strike Exchange Rate | Agreed forward exchange rate between the deposit currency and the alternate currency |
| Interest Rate | Enhanced interest rate for the deposit |
| Fixing date | The date on which the spot exchange rate is compared against the strike price and exercise or expire decision is made |
| Maturity date | Maturity date of the deposit or contract |
| Alternate currency 2 | Applicable for TCI contracts only. This is the other alternate currency |
| Strike exchange rate 2 | Applicable for TCI contracts only. Agreed forward exchange rate between the deposit currency and alternate currency 2 |

**Dual and Triple Currency Investments**

| Event | Description |
|---|---|
| Inception | The contract is recorded in the system. The underlying deposit and option transaction are created |
| Fixing | Decision event. The spot exchange rate is compared against the strike exchange rate; the user decides whether to exercise or expire the currency option. |
| Maturity | The deposit matures and depending on the fixing decision, the redemption amount is either converted to the alternate currency (through a FX spot deal) or redeemed in the deposit currency. This event would be scheduled to run on the maturity. |
| Unwinding | Unwinding is an early termination event whereby the maturity date can be advanced to an earlier date. |

**Dual and Triple Currency Investments**

| Variant | Description |
|---|---|
| Precious Metal Investments | In this variant, either the deposit currency or the alternate currency is a precious metal defined as a currency in the system |
| DCI with barriers | In this variant, the currency option is a barrier option. Option can have knock-in or knock-out features. In Temenos Transact terms, this is defined as an exotic option |
| Principal only conversion | In this variant, if the option is exercised, then only the principal is converted to the alternate currency. The interest amount is repaid in the deposit currency |
| Tripe Currency Investment | In this variant, there are two alternate currencies. The redemption can be in the deposit currency or in any of the alternate currencies |

**Misc**

| Field | Description |
|---|---|
| Variant | Variant for the contract to use the said categories based on the SY.PRODUCT.VARIANT selected. |
| Trade Date | Holds the trade date of the contract. Trade date cannot be forward dated and should fall between the First Date and Last Date of the corresponding product definition record. |
| Maturity Date | Maturity date is the termination date of the contract. Maturity date will be defaulted based on Term and Value Date . |
| Trade Ccy | This is the deposit currency in which the customer deposit or takes loan in MM.MONEY.MARKET . Is the Trade Ccy of DX.TRADE . |
| Alternate Ccy 1 | The alternate currency in which the deposit amount is paid back, that is, the delivery currency in DX.TRADE and the other currency in FOREX |
| Alternate.Ccy.2 | The second alternate currency in which the deposit amount is paid back, that is, this field enables the triple currency investment. On exercise of option FOREX gets created between Trade Ccy and Alternate Ccy 2 . The option trade between Trade Ccy and Alternate Ccy 1 is expired. |
| Exercise Expire | When the field is set to EXERCISE the option contract is exercised and when set to EXPIRE the option contract is expired. The value to the field can be manually determined. When not the fixing event determines the value to this field. The fixing routine to have 2 parameter which are outcoming. The 1st to hold the EXERCISE or EXPIRE as value saying the decision and the second to hold the Exercise Ccy, if suppose the decision is to exercise the option contract. |
| Exercise Ccy | The currency in which the forex is created when it is Alternate Ccy 1 then the DX.TRADE is exercised. When it is Alternate Ccy 2 then it means the DX.TRADE between trade and first alternate currency is expired and a new FX gets created between Trade Ccy and Alternate Ccy 2 . |

**Misc**

| Element | Description |
|---|---|
| Value date | Effective date of the deposit |
| Deposit currency | Currency of the deposit |
| Deposit amount | The principal investment amount |
| Alternate currency | Alternate currency used |
| Strike exchange rate | Agreed forward exchange rate between the deposit currency and the alternate currency |
| Interest rate | Enhanced interest rate for the deposit |
| Fixing date | The date on which, the spot exchange rate is compared against the strike price and exercise or expire decision is made. |
| Maturity date | Maturity date of the deposit or contract |
| Alternate currency 2 | Applicable for TCI contracts only. This is the other alternate currency. |
| Strike exchange rate 2 | Applicable for TCI contracts only. Agreed forward exchange rate between the deposit currency and alternate currency. |

**Misc**

| Event | Description |
|---|---|
| Inception | The contract is recorded in the system. The underlying deposit and option transaction are created. |
| Fixing | Decision event. The spot exchange rate is compared against the strike exchange rate. The user decides whether to exercise or expire the currency option. |
| Maturity | The Deposit matures and depending on the fixing decision, the redemption amount, is either converted to the alternate currency (through a FX Spot Deal) or redeemed in the deposit currency. This event is scheduled to run on the maturity. |
| Unwinding | Unwinding is an early termination event, where the maturity date can be advanced to an earlier date. |

**Misc**

| Variant | Description |
|---|---|
| Precious metal investments | In this variant, either the deposit currency or the alternate currency, is a precious metal defined as a currency in the system. DCI with barriers - In this variant, the currency option is a barrier option. Option can have knock-in or knock-out features. In Temenos Transact terms, this is defined as an exotic option. |
| Principal only conversion | In this variant, if the option is exercised, then only the principal is converted to the alternate currency. The interest amount is repaid in the deposit currency. |
| Tripe currency investment | In this variant, there are two alternate currencies. The redemption can be in the deposit currency or in any of the alternate currencies. |

**Misc**

| Term sheet element | Description |
|---|---|
| Value Date | Commences the contractual obligation from this date |
| Underlying security | Denotes the underlying security which is accumulated or decumulated over the tenor of the contract |
| Strike Price | Denotes the forward price at which the underlying security is purchased or sold |
| Knock out price | Denotes the barrier price. When the spot price of the underlying security breaches this barrier, the contract gets knocked out (terminated). |
| Daily units | Denotes the number of shares that must be accrued on a daily basis |
| Gearing Factor | Applies on the days, when the spot price of the underlying is unfavorable to the investor comparing the strike price |
| Fixing Frequency | Denotes the periodicity at which the settlement of accumulated or decumulated shares occur |
| Maturity Date | Denotes the date on which the contractual obligation ends |

**Misc**

| Event | Description |
|---|---|
| Inception | Commences contractual obligation for the investor. The contract is recorded in the system and the underlying option trade is created. |
| Accrual | Units (of the underlying security) are accrued on a daily basis. For contracts with gearing factor, the gearing factors are applied on the days when the spot price of the underlying is unfavourable to the investor comparing the strike price of the contract. |
| Fixing | Effects the settlement of the accumulated or decumulated shares. The underlying option is exercised and this creates the SEC.TRADE transaction for the underlying security. This is a scheduled periodic event. |
| Knockout | Occurs when the price barrier is breached, that is, when the spot price of the underlying touches the knock-out price. When this event occurs, the contract is terminated. |
| Unwinding | Terminates the contract either fully or partially. In a full unwind, the contract is terminated earlier. In a partial unwind, the contract continues to be active, but the obligation (that is, daily accrual units) is reduced for the rest of the contract period. |
| Novation | Transfers the contract between customers and banks. Internal novation - Contract is transferred from one customer account to another External novation - Contract is transferred from customer account in one bank to another |
| Maturity | Indicates the end date of the contract. The contractual obligation ceases on this date. |

**Misc**

| Variant | Description |
|---|---|
| Non-leveraged accumulator or decumulator | Denotes the plain vanilla accumulator without a gearing factor |
| Leveraged accumulator | Holds an additional attribute that is, gearing factor. Gearing factor is applied to the accrual on the days when the spot price is unfavourable to the customer, comparing the strike price. The potential loss to the investor is higher in this variant, compared to the plain vanilla variant. |
| Guaranteed accumulator or decumulator | Assures the investor of guaranteed accumulation. That is, a certain number of underlying shares might be accumulated or decumulated and settled, even if the knock-out price barrier is breached early in the life of the accumulator contract. |

**Misc**

| Field | Description |
|---|---|
| Product Type | This field indicates this is an accumulator or decumulator contract. |
| Contract Status | The status of the contract is updated in this field. When the contract is created, the status is ACTIVE, subsequently as the contract undergoes various life cycle events, the status is updated as below. |
| Option Type | This field holds the option type of the underlying option. This is auto populated based on the Product Type field. For accumulator contract, the underlying is a PUT option, for decumulator contract, the underlying is a CALL option. |
| Trade Date | This field holds the trade date of the contract. Trade date cannot be forward dated and should fall between the First Date and Last Date of the corresponding product definition record. |
| Maturity Date | Maturity date is the termination date of the contract. Maturity date is defaulted based on Term and Value Date . |
| Daily Units | This field holds the number of units (nominal) to be accrued per day. The value should be a multiple of contract size of the underlying DX.CONTRACT.MASTER . |
| Fixing Frequency | The Accumulator and Decumulator contracts accrue the underlying security on a daily basis. The accrued units are settled periodically (This periodic settlement is known as fixing). |

**Misc**

| Element | Description |
|---|---|
| Value Date | Contractual obligation commences from this date. |
| Underlying security | The underlying security which is accumulated or decumulated over the tenor of the contract. |
| Strike Price | The forward price at which the underlying security is purchased or sold. |
| Knock out price | This is the barrier price, when the spot price of the underlying security breaches this barrier, the contract gets knocked out (terminated). |
| Daily units | The number of shares that must be accrued on a daily basis. |
| Gearing factor | The gearing factor is applied on the days when the spot price of the underlying is unfavourable to the investor when compared to the strike price. |
| Fixing drequency | Settlement of accumulated or decumulated shares occur at this periodicity. |
| Maturity Date | The contractual obligation ends at this date. |

**Misc**

| Event | Description |
|---|---|
| Inception | Contractual obligation commences for the investor. The contract is recorded in the system and the underlying option trade is created. |
| Accrual | Units (of the underlying security) is accrued on a daily basis. For contracts with gearing factor, the gearing factors are applied on those days when the spot price of the underlying is unfavourable to the investor when compared against the strike price of the contract. |
| Fixing | Settlement of the accumulated or decumulated shares are effected through this event. The underlying option is exercised and this creates the SEC.TRADE transaction for the underlying security. This is a scheduled periodic event. |
| Knockout | This event can occur when the price barrier is breached, that is, when the spot price of the underlying touches the knock-out price. When this event occurs, the contract is terminated. |
| Unwinding | The contract can be unwound either fully or partially. In a full unwind, the contract is terminated early. In a partial unwind, the contract continues to be active, but the obligation (that is, daily accrual units) are reduced for the rest of the contract period. |
| Novation | The contract can also be novated, which is transferred from one customer account to another customer account (Internal novation) or transferred to a different bank (external novation). |
| Maturity | It is the end date of the contract. The contractual obligation ceases on this date. |

**Misc**

| Variant | Description |
|---|---|
| Non leveraged accumulator or decumulator | This is the plain vanilla accumulator without a gearing factor. |
| Leveraged Accumulator | This variant has an additional attribute, which is, gearing factor. Gearing factor is applied to the accrual on those days where the Spot Price is unfavorable to the customer, when compared to the strike price. The potential loss to the investor is higher in this variant as compared to the plain vanilla variant. |
| Guaranteed accumulator or decumulator | This variant assures the investor of guaranteed accumulation. That is, a certain number of underlying shares might be accumulated or decumulated and settled, even if the knock-out price barrier is breached early in the life of the accumulator contract. |

**XF**

| Event | Description |
|---|---|
| Inception | The contract is recorded in the system. The underlying option deals are created |
| Rollover | Roll over of the contract |
| Maturity | On maturity date, the contract ceases to exist |

**XF**

| Term Sheet Element | Description |
|---|---|
| Value Date | Indicates the effective date of the contract |
| Deposit Currency | Indicates the currency of the deposit |
| Deposit Amount | Indicates the amount of the deposit in deposit currency |
| Loan Currency | Indicates the currency of the loan |
| Loan Amount | Indicates the loan amount in loan currency |
| Deposit Interest Rate | Indicates the interest rate for the deposit |
| Loan Interest Rate | Indicates the interest rate for the loan |
| Maturity Date | Indicates the maturity date of the contract |

**XF**

| Field | Description |
|---|---|
| Valuation Routine | Values the structured product based on the routine attached |
| Sweep Acct | System sweeps the transactions automatically from the customer segregated account to the customer source account, when this field is set to Yes |
| Sy Exclude Valuation | Reports the structured product deal only when this field is set to Yes. Otherwise, all transactions created by the structured product along with the structured product deal will be displayed. |
| Event | Displays the list of events that can occur in the product life cycle such as CREATE, INPUT, AUTHORISE, ROLLOVER etc and each event can be mapped with dependencies |
| Eb Activity | Invites the user to specify events that requires any delivery message(s) to be invoked |
| Cob Phase | Indicates the COB stage in which the associated event will be processed. For scheduled and/or rolling events the close of business processing will be invoked. |
| First Date and Last Date | Indicates the first and last date on which a deal for this product can be accepted into the system |
| Suppress Underlying | Denies the system from creating underlying transactions, when set to Yes and when set to No the underlying transactions are not suppressed and is created from the structured product contract. The life cycle events of the product is processed by Temenos Transact . |
| Sub Asset Type | Maps the valid record in Sub Asset Type with the application possibly |
| Fixing Routine | Holds a value only if Supress Underlying is set to No. Validation routines can be attached for fixing. |
| Mtm Routine | Facilitates attaching a routine for MTM (Mark to Market) or the user can manually define it by mentioning the categories |
| Ca Impact | Indicates whether Corporate Action is applicable or not for this definition |

**PT**

| S. No | Term Sheet Element | Description |
|---|---|---|
| 1. | Value Date | Effective date of the contract |
| 2. | Currency bought | The currency the investor buys |
| 3. | Currency sold | The currency sold by the investor |
| 4. | Call amount | The amount bought in each settlement period |
| 5. | Put amount | The amount sold in each settlement period |
| 6. | Fixing schedule | Periodical settlement frequency |
| 7. | Strike exchange rate | The strike exchange rate for the option |
| 8. | Knock out price | When this barrier price is breached, the option is knocked out. |
| 9. | Maturity date | Maturity date of the contract |

**PT**

| S. No | Event | Description |
|---|---|---|
| 1. | Inception | The contract is recorded in the system. The underlying option deals are created. |
| 2. | Fixing | This is the periodical settlement event. The spot exchange rate is compared against the strike exchange rate, the decision is made to either exercise the long option or assign the short option. If the long option is partially exercised, then the short option needs to be partially expired. If the short option is partially assigned, then the long option needs to be partially expired. |
| 3. | Knock out | Both the long option and the short option can have knock-out features. When both the options are knocked out, the contract itself can be knocked out. |
| 4. | Unwinding | The contract can be terminated early. |
| 5. | Maturity | On maturity date, the contract ceases to exist. |

**PT**

| S. No | Variant | Description |
|---|---|---|
| 1. | PF | In this variant, the PF or TARKO contract gets knocked out when the knock-out barrier is breached. |
| 2. | TARKO | In this variant, the PF or TARKO contract gets knocked out when the accumulated profit reaches a pre-defined level. |
| 3. | With Vanilla option | Some variants include a vanilla option which does not have a knock-out feature. |
| 4. | FX Accumulator or Decumulator | In this variant, the fixing schedule of the long and short option is the same. The notional amount of the short option would be the leveraged notional amount. |

**PT**

| Field | Description |
|---|---|
| Variant | Refers to a particular variant, then the variant can be linked in this field. Once linked, the parameters and configurations defined for the variant would be used in processing the life cycle of the contract. |
| Currency Bought | Holds the currency that the customer buys |
| Currency Sold | Holds the currency that the customer sells |
| Trade Date | Holds the trade date of the contract. Trade date cannot be forward dated and should fall between the First Date and Last Date of the corresponding product definition record. |
| Maturity Date | Maturity date is the termination date of the contract. Maturity date will be defaulted based on Term and Value Date . |
| Premium Pay Receive | Indicates whether the customer have to pay or receive the premium amount |

**PT**

| Element | Description |
|---|---|
| Value Date | Effective date of the contract |
| Currency bought | The currency the investor buys |
| Currency sold | The currency sold by the investor |
| Call amount | The amount bought in each settlement period |
| Put amount | The amount sold in each settlement period |
| Fixing schedule | Periodical settlement frequency |
| Strike exchange rate | The strike exchange rate for the option |
| Knock out price | When this barrier price is breached, the option is knocked out. |
| Maturity date | Maturity date of the contract |

**PT**

| Event | Description |
|---|---|
| Inception | The contract is recorded in the system. The underlying option deals are created. |
| Fixing | This is the periodical settlement event. The spot exchange rate is compared against the strike exchange rate, the decision is made to either exercise the long option or assign the short option. If the long option is partially exercised the short option needs to be partially expired. If the short option is partially assigned the long option needs to be partially expired. |
| Knock out | Both the long option and the short option can have a knock out features, when both the options are knocked out, the contract itself can be knocked out. |
| Unwinding | The contract can be early terminated. |
| Maturity | On maturity date, the contract ceases to exist. |

**PT**

| Variant | Description |
|---|---|
| PF | In this variant, the Participating Forwards and TARKO contract gets knocked out when the knock out barrier is breached. |
| TARKO | In this variant, the Participating Forwards and TARKO contract gets knocked out when the accumulated profit reaches a pre-defined level. |
| With vanilla option | Some variants include a vanilla option, which does not have a knock out feature. |
| FX Accumulator and Decumulator | In this variant, the fixing schedule of the long and short option is the same. The notional amount of the short option is the leveraged notional amount. |

**CommonFlow**

| Fields from SY.ACCU.DECU or PWM.PO.PARAMETER | Fields in PAYMENT.ORDER | Conditional Mapping |
|---|---|---|
| T24 Bank BIC | Ordering Customer Bic | NA |
| Po Susp Categ in PWM.PO.PARAMETER | Debit Account | NA |
| Premium Currency or Unwind Chg Ccy or Delivery Currency | Debit Ccy | Depends on the event type. For example, for unwinding event system maps the Unwind Chg Ccy field |
| Value date | Debit Value Date | NA |
| @ID ( SY.ACCU.DECU Reference) | Ordering Reference | NA |
| Ben Acct | Beneficiary Account No | NA |
| Bic of Beneficiary Bank | Beneficiary Bic | NA |
| Beneficiary Bank | Beneficiary Customer | NA |
| Name of Beneficiary Bank | Beneficiary Name | System maps the name from CUSTOMER application. |
| Bic of Cpty No | Acct With Bank Bic | NA |
| Cpty No | Acct With Bank Customer | NA |
| Cpty Add | Acct With Bank Swift Addr | NA |
| Bic of Intr Bank | Intermed Bic | NA |
| Intr Bank | Intermed Bank Customer | NA |
| Intr Add | Intermed Swift Addr | NA |
| Premium Currency or Unwind Chg Ccy or Delivery Currency | Payment Currency | Depends on the event type. For example, for unwinding event system maps the Unwind Chg Ccy field. |
| Cpty Prem Amt or Cpty Prem Amt + Cpty Fee Amt , Cpty Unwind Chg Amt Cpty Sett Amt | Payment Amount | When the contract is authorised: In case of Agency Model - Cpty Prem Amt + Cpty Fee Amt In case of non-agency model - Cpty Prem Amt In case of Unwinding: Cpty Unwind Chg Amt In case of Fixing roll - Cpty Sett Amt . When Cpty Sett Amt is null, then accumulator = last price - strike price and decumulator = strike price - last price |
| Value Date | Required Credit Value Date | NA |
| NA | Bank to Bank Info | NA |
| NA | Internal Order Details | NA |
| Bank | Order Type | NA |
| Mapped from PWM.PO.PARAMETER if set | Order Initiation Type Payment Category Payment Method Payment Purpose | NA |
| Counterparty Acc or Premium Acc or Unwind Chg Acc or Temenos Payments to determine | Credit Nostro Account | If Counterparty Acc or Premium Acc or Unwind Chg Acc is a Nostro account which does not belong to the counterparty, then system defaults the value in that field. If Counterparty Acc or Premium Acc or Unwind Chg Acc is an internal category account formed using the Po Susp Categ, then system does not populate any value in this field. Temenos Payments determine the nostro account. |
| Bic of Counterparty Acc or Premium Acc or Unwind Chg Acc or Temenos Payments to determine | Receiver Bic | If Counterparty Acc or Premium Acc or Unwind Chg Acc is a Nostro account which does not belong to the counterparty, then system defaults the Bic of these accounts. If Counterparty Acc or Premium Acc or Unwind Chg Acc is an internal category account formed using the Po Susp Categ, then system does not populate any value in this field. Temenos Payments determines the receiver of the message. |

**CommonFlow**

| Fields from SY.DCI | Fields in PAYMENT.ORDER | Conditional Mapping |
|---|---|---|
| T24 Bank BIC | Ordering Customer Bic | NA |
| Po Susp Categ in PWM.PO.PARAMETER | Debit Account | NA |
| Premium Ccy or Unwind Chg Ccy | Debit Ccy | Depends on the event type |
| Value Date | Debit Value Date | NA |
| @ID ( SY.DCI Reference) | Ordering Reference | NA |
| Dep Ccy Ben Acct or Alt Ccy Ben Acct | Beneficiary Account No | NA |
| Bic of Dep Ccy Ben Bank or Alt Ccy Ben Bank | Beneficiary Bic | NA |
| Dep Ccy Ben Bank or Alt Ccy Ben Bank | Beneficiary Customer | NA |
| Name of Dep Ccy Ben Bank or Alt Ccy Ben Bank | Beneficiary Name | System maps the name from CUSTOMER application |
| Bic of Dep Ccy Cpty No or Alt Ccy Cpty No | Acct With Bank Bic | NA |
| Dep Ccy Cpty No or Alt Ccy Cpty No | Acct With Bank Customer | NA |
| Dep Ccy Cpty Add or Alt Ccy Cpty Add | Acct With Bank Swift Addr | NA |
| Bic of Dep Ccy Intr Bank or Alt Ccy Intr Bank | Intermed Bic | NA |
| Dep Ccy Intr Bank or Alt Ccy Intr Bank | Intermed Bank Customer | NA |
| Dep Ccy Intr Add or Alt Ccy Intr Add | Intermed Swift Addr | NA |
| Premium Currency or Unwind Chg Ccy | Payment Currency | NA |
| Premium Amt + Deposit Amt Cpty Prem Amt + Deposit Amt + Cpty Fee Amt Unwind Chg Amt | Payment Amount | When record is authorised Dealer book - Premium Amt + Deposit Amt Agency booking model - Cpty Prem Amt + Deposit Amt + Cpty Fee Amt Unwinding: Unwind Chg Amt |
| Value Date | Required Credit Value Date | NA |
| NA | Bank to Bank Info | NA |
| NA | Internal Order Details | NA |
| Bank | Order Type | NA |
| Mapped from PWM.PO.PARAMETER if set | Order Initiation Type Payment Category Payment Method Payment Purpose | NA |
| Cparty Deposit Acc , Cparty Alt Currency Account 1 , Counterparty Alt Currency Account 2 and Unwind Chg Acc or Temenos Payments to determine | Credit Nostro Account | If the account is a Nostro account which does not belong to the counterparty, then system defaults the value in the respective field. If it is an internal category account formed using the Po Susp Categ, then system does not populate any value in this field. Temenos Payments determines the Nostro account |
| Bic of Cparty Deposit Acc , Cparty Alt Currency Account 1 , Cparty Alt Currency Account 2 and Unwind Chg Acc or Temenos Payments to determine | Receiver Bic | If the account is a Nostro account which does not belong to the counterparty, then system defaults the BIC in the respective field. If it is an internal category account formed using the Po Susp Categ, then system does not populate any value in this field. Temenos Payments determines the receiver of the message |

**CommonFlow**

| Fields from SY.FX.FORWARDS | Fields in PAYMENT.ORDER | Conditional Mapping |
|---|---|---|
| T24 Bank BIC | Ordering Customer Bic | NA |
| Po Susp Categ in PWM.PO.PARAMETER | Debit Account | NA |
| Premium Currency or Fx Payout Currency | Debit Ccy | Depends on the event |
| Value Date | Debit Value Date | NA |
| @ID ( SY.FX.FORWARDS Reference) | Ordering Reference | NA |
| NA | Beneficiary Account No | NA |
| Bic of Cp Bccy Ben Bank or Cp Sccy Ben Bank | Beneficiary Bic | NA |
| Cp Bccy Ben Bank or Cp Sccy Ben Bank | Beneficiary Customer | NA |
| Name of Cp Bccy Ben Bank or Cp Sccy Ben Bank | Beneficiary Name | System maps the name from CUSTOMER application. |
| Bic of Cp Bccy Cpty No or Cp Sccy Cpty No | Acct With Bank Bic | NA |
| Cp Bccy Cpty No or Cp Sccy Cpty No | Acct With Bank Customer | NA |
| Cp Bccy Cpty Add or Cp Sccy Cpty Add | Acct With Bank Swift Addr | NA |
| Bic of Cp Bccy Intr Bank or Cp Sccy Intr Bank | Intermed Bic | NA |
| Cp Bccy Intr Bank or Cp Sccy Intr Bank | Intermed Bank Customer | NA |
| Dep Ccy Intr Addr or Alt Ccy Intr Addr | Intermed Swift Addr | NA |
| Premium Currency or Fx Payout Currency | Payment Currency | Depends on the event. |
| Premium Amt Cpty Premium Amt + Cpty Fee Amt B Settlement Amt B Cpty Sett Amount S Settlement Amt S Cpty Sett Amount Vb Settlement Amt Vb Cpty Sett Amount Unwind Chg Amt Cpty Unwind Chg Amt | Payment Amount | When authorised Dealer book - Premium Amt Agency model - Cpty Premium Amt + Cpty Fee Amt ‘Fixing Buy' / 'Knockout Buy' Dealer book - B Settlement Amt Agency model - B Cpty Sett Amount Fixing Sell / Knockout Sell Dealer book - S Settlement Amt Agency model - S Cpty Sett Amount Fixing Vanila Buy Dealer book - Vb Settlement Amt Agency model - Vb Cpty Sett Amount Unwind Terminator Dealer book - Unwind Chg Amt Agency model - Cpty Unwind Chg Amt |
| Value Date | Required Credit Value Date | NA |
| NA | Bank to Bank Info | NA |
| NA | Internal Order Details | NA |
| Bank | Order Type | NA |
| Mapped from PWM.PO.PARAMETER if set | Order Initiation Type Payment Category Payment Method Payment Purpose | NA |
| Cparty Buy Ccy Acct or Cparty Sell Ccy Acct or Temenos Payments to determine | Credit Nostro Account | If it is a Nostro account which does not belong to the counterparty, then system defaults the value in the field. If it is an internal category account formed using the Po Susp Categ, then system does not populate any value in this field. Temenos Payments determines the Nostro account |
| Cparty Buy Ccy Acct or Cparty Sell Ccy Acct or Temenos Payments to determine | Receiver Bic | If it is a Nostro account which does not belong to the counterparty, then system defaults the BIC of the account holder. If it is an internal category account formed using the Po Susp Categ , then system does not populate any value in this field. Temenos Payments determines the receiver of the message. |

**CommonSetup**

| Event | Description |
|---|---|
| sySystemAuthorise | Generic authorise plug in |
| sySystemAuthoriseReversal | Generic authorise reversal plug in |
| sySystemReverse | Generic reversal plug in |
| sySystemDelete | Generic delete plug in |
| sySystemDeleteAmendment | Generic delete amendment plug in |

**CommonSetup**

| Field | Description |
|---|---|
| Asset Class | Holds the asset class of the underlying. For equity accumulator or decumulator contract, the value is Equity. For FX accumulator or decumulator contract, the value is FX. |
| Mnemonic | Holds the mnemonic, which is an alternative easy mean to reference the master |
| Underlying | Holds the underlying equity instrument. This field is not editable for FX related products, if the Asset Class is not set to Equity. |
| Currency1 | Holds the first currency in the currency pair. This field is not editable for equity products, if the Asset Class is set to Equity. |
| Currency2 | Holds the second currency in the currency pair. This field is not editable for equity products, if the Asset Class is set to Equity. |
| Use Master Sat | Indicates sub asset type associated with this master. This field is used for reporting purposes. |
| Risk Company | Accepts a valid company ID or ALL |
| Risk Level | Holds the product risk rating associated with the underlying of the associated company |

**Delivery**

| Event Type | Description | Trigger Point |
|---|---|---|
| Trade initiation | Triggering an email alert on authorisation of SY contract | Authorise (event) - trade authorisation |
| Trade fixing | Fixing event of a SY is processed | Fixing (event) - fixing event is run |
| Trade exercise | Processing exercise event of a SY | Exercise (event) - exercise event |
| Trade expire | Expiration of SY | Mature (event) - expire event |
| Trade reversal | Reversal of SY deal | Reverse (event) - trade reversal |
| Trade amendment | Amendment of SY deal | Amend (event) - trade amendment |
| Knock in | Knocking in the product | Knock in (event) - Knock In set to Yes |
| Knock out | Knocking out the product | Knock out (event) - Knock Out set to Yes |
| Unwinding | Triggering unwinding | Unwinding (event) - unwinding product |
| Rollover | Triggering rollover | Rollover (event) - rollover product |
| Accrual | Accruing underlying units | Accrual (event) - accrue units |
| Corporate actions | Implementing the changes in terms of structure | Amend (event) - Corporate Action (CA) run |


### Derivatives_Structured_Products - XF (XF)


**XF**

| Event | Description |
|---|---|
| Inception | The contract is recorded in the system. The underlying option deals are created |
| Rollover | Roll over of the contract |
| Maturity | On maturity date, the contract ceases to exist |

**XF**

| Term Sheet Element | Description |
|---|---|
| Value Date | Indicates the effective date of the contract |
| Deposit Currency | Indicates the currency of the deposit |
| Deposit Amount | Indicates the amount of the deposit in deposit currency |
| Loan Currency | Indicates the currency of the loan |
| Loan Amount | Indicates the loan amount in loan currency |
| Deposit Interest Rate | Indicates the interest rate for the deposit |
| Loan Interest Rate | Indicates the interest rate for the loan |
| Maturity Date | Indicates the maturity date of the contract |

**XF**

| Field | Description |
|---|---|
| Valuation Routine | Values the structured product based on the routine attached |
| Sweep Acct | System sweeps the transactions automatically from the customer segregated account to the customer source account, when this field is set to Yes |
| Sy Exclude Valuation | Reports the structured product deal only when this field is set to Yes. Otherwise, all transactions created by the structured product along with the structured product deal will be displayed. |
| Event | Displays the list of events that can occur in the product life cycle such as CREATE, INPUT, AUTHORISE, ROLLOVER etc and each event can be mapped with dependencies |
| Eb Activity | Invites the user to specify events that requires any delivery message(s) to be invoked |
| Cob Phase | Indicates the COB stage in which the associated event will be processed. For scheduled and/or rolling events the close of business processing will be invoked. |
| First Date and Last Date | Indicates the first and last date on which a deal for this product can be accepted into the system |
| Suppress Underlying | Denies the system from creating underlying transactions, when set to Yes and when set to No the underlying transactions are not suppressed and is created from the structured product contract. The life cycle events of the product is processed by Temenos Transact . |
| Sub Asset Type | Maps the valid record in Sub Asset Type with the application possibly |
| Fixing Routine | Holds a value only if Supress Underlying is set to No. Validation routines can be attached for fixing. |
| Mtm Routine | Facilitates attaching a routine for MTM (Mark to Market) or the user can manually define it by mentioning the categories |
| Ca Impact | Indicates whether Corporate Action is applicable or not for this definition |


---
