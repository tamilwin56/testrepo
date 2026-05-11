
# Temenos Transact — Limits_Collateral Module Documentation


> **Comprehensive User Guide**
> Generated: 13 April 2026
> Content: Configuration | Reference | Field Descriptions | Glossary


## Table of Contents

  - [Limits_Collateral Module Overview](#limits_collateral-module-overview)
    - [Sub-Module Summary](#sub-module-summary)
    - [How to Use This Guide](#how-to-use-this-guide)
  - [Chapter 1: Limits_Collateral - CO](#chapter-1-limits_collateral---co)
    - [Features in Limits_Collateral - CO](#features-in-limits_collateral---co)
    - [1.1  AdvanceCollateral CrossPledging](#11-advancecollateral-crosspledging)
    - [1.2  Collateral Advance Ratio](#12-collateral-advance-ratio)
    - [1.3  Collateral and Limits](#13-collateral-and-limits)
    - [1.4  Collateral Exclusion](#14-collateral-exclusion)
    - [1.5  CollateralExclusionAdvanceRatioConcentrationCap](#15-collateralexclusionadvanceratioconcentrationcap)
    - [1.6  CollateralPledgeReduction](#16-collateralpledgereduction)
    - [1.7  ConcentrationChecksClientPortfolio](#17-concentrationchecksclientportfolio)
    - [1.8  Corporate Collateral Pool](#18-corporate-collateral-pool)
    - [1.9  Creating Collateral Item](#19-creating-collateral-item)
    - [1.10  External Collateral Assets](#110-external-collateral-assets)
    - [1.11  Group Concentration Cap](#111-group-concentration-cap)
    - [1.12  Limit Collateral Allocation](#112-limit-collateral-allocation)
    - [1.13  Loan to Value calculation](#113-loan-to-value-calculation)
    - [1.14  Margin Valuation through Credit Policy Structure](#114-margin-valuation-through-credit-policy-structure)
    - [1.15  Misc](#115-misc)
    - [1.16  OffBalanceSheetAccountingforCollaterals](#116-offbalancesheetaccountingforcollaterals)
    - [1.17  Other Internal Collateral Assets](#117-other-internal-collateral-assets)
    - [1.18  Pre-tradeBuyingPowerChecks](#118-pre-tradebuyingpowerchecks)
    - [1.19  Preferential LTV DiversifiedPortfolio](#119-preferential-ltv-diversifiedportfolio)
    - [1.20  Real-time Portfolio Collateral Valuation](#120-real-time-portfolio-collateral-valuation)
    - [1.21  Right to Link the Collateral](#121-right-to-link-the-collateral)
    - [1.22  Support for Wealth Credits](#122-support-for-wealth-credits)
    - [1.23  Third Party Pledge](#123-third-party-pledge)
  - [Chapter 2: Limits_Collateral - LI](#chapter-2-limits_collateral---li)
    - [Features in Limits_Collateral - LI](#features-in-limits_collateral---li)
    - [2.1  Misc](#21-misc)
    - [2.2  Non-Stop Processing](#22-non-stop-processing)
    - [2.3  Chrg Acct Fees Chrgs on Limit](#23-chrg-acct-fees-chrgs-on-limit)
    - [2.4  Collateral Allocation to Limit](#24-collateral-allocation-to-limit)
    - [2.5  Creating Cross Limits](#25-creating-cross-limits)
    - [2.6  Creating Customer Liability Structure](#26-creating-customer-liability-structure)
    - [2.7  Creating Limit Products](#27-creating-limit-products)
    - [2.8  Credit Checking](#28-credit-checking)
    - [2.9  Credit Limits](#29-credit-limits)
    - [2.10  Cus Rsk Grp For Mt Jt Cus Lim](#210-cus-rsk-grp-for-mt-jt-cus-lim)
    - [2.11  Customer Grouping](#211-customer-grouping)
    - [2.12  Customer Sub-Group in Risk Exposure](#212-customer-sub-group-in-risk-exposure)
    - [2.13  Externalise Transact Limit Exposure](#213-externalise-transact-limit-exposure)
    - [2.14  Impact of Loan Repayment](#214-impact-of-loan-repayment)
    - [2.15  Intraday Limit](#215-intraday-limit)
    - [2.16  Joint Owned Limits](#216-joint-owned-limits)
    - [2.17  Liability Structure Limit Sharing Group](#217-liability-structure-limit-sharing-group)
    - [2.18  Limit Change Utility](#218-limit-change-utility)
    - [2.19  Limit Sub-Allocation](#219-limit-sub-allocation)
    - [2.20  Linking Collaterals to Limit](#220-linking-collaterals-to-limit)
    - [2.21  Misc](#221-misc)
    - [2.22  Monitoring Credit Exposure](#222-monitoring-credit-exposure)
    - [2.23  Neutral Revolving Limit Structure](#223-neutral-revolving-limit-structure)
    - [2.24  Offsetting Credit Balance Accounts](#224-offsetting-credit-balance-accounts)
    - [2.25  Overdraft Limits to Accounts](#225-overdraft-limits-to-accounts)
    - [2.26  Reporting of Breach to Validation Limit](#226-reporting-of-breach-to-validation-limit)
    - [2.27  Restricted Allowed Customers](#227-restricted-allowed-customers)
    - [2.28  Risk Exposure Overview Enquiry](#228-risk-exposure-overview-enquiry)
    - [2.29  Sec Lim Coll](#229-sec-lim-coll)
    - [2.30  Special Limit Processing for Foreign Exchange](#230-special-limit-processing-for-foreign-exchange)
    - [2.31  Time Banding of Limits](#231-time-banding-of-limits)
    - [2.32  Update Approved](#232-update-approved)
    - [2.33  Updating Limit Exposure](#233-updating-limit-exposure)
    - [2.34  Utilisation of Limits](#234-utilisation-of-limits)
  - [Chapter 3: Limits_Collateral - OV](#chapter-3-limits_collateral---ov)
    - [Features in Limits_Collateral - OV](#features-in-limits_collateral---ov)
    - [3.1  Misc](#31-misc)
    - [3.2  Direct](#32-direct)
    - [3.3  Facility Based Lending](#33-facility-based-lending)
    - [3.4  Misc](#34-misc)
    - [3.5  RealTimeValuation](#35-realtimevaluation)
  - [Appendix A: Glossary of T24 Applications & Fields](#appendix-a-glossary-of-t24-applications-fields)
    - [Applications](#applications)
    - [Fields Referenced](#fields-referenced)
  - [Appendix B: Consolidated Field Reference](#appendix-b-consolidated-field-reference)
    - [Limits_Collateral - CO (CO)](#limits_collateral---co-co)
    - [Limits_Collateral - LI (LI)](#limits_collateral---li-li)
    - [Limits_Collateral - OV (OV)](#limits_collateral---ov-ov)

---


## Limits_Collateral Module Overview


This document provides comprehensive documentation for the **Limits_Collateral** module of Temenos Transact. It covers **3 sub-modules** with a total of **62 feature areas**.


### Sub-Module Summary


| # | Sub-Module | Code | Features | Description |
|---|-----------|------|----------|-------------|
| 1 | **Limits_Collateral - CO** | `CO` | 23 | Limits_Collateral - CO module of Temenos Transact |
| 2 | **Limits_Collateral - LI** | `LI` | 34 | Limits_Collateral - LI module of Temenos Transact |
| 3 | **Limits_Collateral - OV** | `OV` | 5 | Limits_Collateral - OV module of Temenos Transact |


### How to Use This Guide


Each feature in this document is organized into the following sections:

- 📖 **Introduction** — Overview and purpose of the feature
- ⚙️ **Configuration** — How to set up and configure the feature
- 🔧 **Working With** — Operational usage and field descriptions
- 📋 **Tasks** — Step-by-step procedures
- 📊 **Outputs** — Reports, enquiries, and generated outputs

Each feature includes a **Quick Reference Card** at the top with application names, key fields, prerequisites, and a summary. Appendices provide a full glossary, consolidated field tables, and end-to-end use-case scenarios.

---


## Chapter 1: Limits_Collateral - CO


Limits_Collateral - CO module of Temenos Transact


### Features in Limits_Collateral - CO


| # | Feature | Sections |
|---|---------|----------|
| 1.1 | AdvanceCollateral CrossPledging | Intro, Confi, Worki, Tasks, Outpu |
| 1.2 | Collateral Advance Ratio | Intro, Confi, Worki, Tasks, Outpu |
| 1.3 | Collateral and Limits | Intro, Tasks, Outpu |
| 1.4 | Collateral Exclusion | Intro, Confi, Worki, Tasks, Outpu |
| 1.5 | CollateralExclusionAdvanceRatioConcentrationCap | Intro, Confi, Worki, Tasks, Outpu |
| 1.6 | CollateralPledgeReduction | Intro, Confi, Worki, Tasks, Outpu |
| 1.7 | ConcentrationChecksClientPortfolio | Intro, Confi, Worki, Tasks, Outpu |
| 1.8 | Corporate Collateral Pool | Intro, Confi, Tasks |
| 1.9 | Creating Collateral Item | Intro, Tasks, Outpu |
| 1.10 | External Collateral Assets | Intro, Confi, Tasks, Outpu |
| 1.11 | Group Concentration Cap | Intro, Confi, Tasks, Outpu |
| 1.12 | Limit Collateral Allocation | Intro, Tasks, Outpu |
| 1.13 | Loan to Value calculation | Intro, Confi, Tasks, Outpu |
| 1.14 | Margin Valuation through Credit Policy Structure | Intro, Confi, Worki, Tasks, Outpu |
| 1.15 | Misc | Intro |
| 1.16 | OffBalanceSheetAccountingforCollaterals | Intro, Confi, Worki, Tasks, Outpu |
| 1.17 | Other Internal Collateral Assets | Intro, Confi, Tasks, Outpu |
| 1.18 | Pre-tradeBuyingPowerChecks | Intro, Confi, Worki, Tasks, Outpu |
| 1.19 | Preferential LTV DiversifiedPortfolio | Intro, Confi, Worki, Tasks, Outpu |
| 1.20 | Real-time Portfolio Collateral Valuation | Intro, Confi, Tasks, Outpu |
| 1.21 | Right to Link the Collateral | Intro, Tasks, Outpu |
| 1.22 | Support for Wealth Credits | Intro, Confi, Worki, Tasks, Outpu |
| 1.23 | Third Party Pledge | Intro, Tasks, Outpu |


### 1.1  AdvanceCollateral CrossPledging


> **📇 Quick Reference Card**
> 
> **Purpose:** *A collateral can be cross-pledged, that is, the collateral asset of the main customer is pledged to cover own liability and other customer liability. This is achieved by linking the other customer’s liability to the collateral right of the main customer whose asset is pledged as collateral.*
> 
> **Applications:** `CO.ALLOCATION.DETAILS`, `CO.ASSET.DETAILS`, `CO.DEFICIT`, `CO.VALUATION.PARAMETER`, `COLLATERAL.RIGHT`, `LIMIT.COL.ALLOC.WORK`
> 
> **Key Fields:** *Allocation*, *Type*, *Value*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

A collateral can be cross-pledged, that is, the collateral asset of the main customer is pledged to cover own liability and other customer liability. This is achieved by linking the other customer’s liability to the collateral right of the main customer whose asset is pledged as collateral.

To apply the advance collateral ratio and concentration cap for cross-pledged collateral, the collateral asset details, the collateral allocation details and collateral deficit, if any, are maintained at the collateral right level instead of customer level.

This feature requires the CX module to be installed in addition to the CO and MV modules.


#### ⚙️ Configuration

The following fields in the CO.VALUATION.PARAMETER application flags the base for collateral allocation to calculate the advance ratio and concentration checks.


##### Allocation Type

- Determines whether the advance collateral is applied based on customer or collateral right link. The options in this field are Customer or Alloc.Work.
- When this field is set to Customer, the tables required for calculating advance collateral like CO.ASSET.DETAILS , CO.ALLOCATION.DETAILS and CO.DEFICIT are updated at the customer level.
- When this field is set to Alloc Work, the tables required for calculating advance collateral like CO.ASSET.DETAILS , CO.ALLOCATION.DETAILS and CO.DEFICIT are updated with the ID as LIMIT.COL.ALLOC.WORK table based on the collateral right of the main customer.


##### Allocation Value

- Determines the limit amount to be considered for advance collateral allocation. The options in this field are Maximum Total or Total Os.
- When this field is set to Maximum Total, the collateral allocation is for the maximum total amount of the limit.
- When this field is set to total Os, the collateral allocation is for the utilised or outstanding amount of the limit.


#### 🔧 Working With

The collateral allocation after applying advance collateral ratio and concentration cap is updated and maintained based on either one of the following options:

- Customer – When it is maintained at customer level, only the collateral coverage to the main customer’s liability is maintained in the CO.ASSET.DETAILS and CO.ALLOCATION.DETAILS , and third party limits attached to the collateral right of the main customer is not considered.
- Alloc Work – When it is maintained at allocation work level, the advance ratio, concentration checks, allocation and deficit details are maintained based on the liabilities linked to the collateral right, which includes the third party limits, if any, linked to the collateral right of the main customer.

> **⚠️ Note:** This is configured in the Allocation Type field in the CO.VALUATION.PARAMETER application.


##### Application of Collateral Advance Ratio and Concentration Cap for Cross-Pledged Collateral:

To apply collateral advance ratio and concentration cap on cross-pledged collateral, the Allocation Type field must be set to Alloc Work in CO.VALUATION.PARAMETER .

When the collateral allocation is by limit, the Allocation Value field can be set to Maximum Total or Total.Os, which indicates the amount to be covered during the collateral allocation.

Cross-pledging is achieved by linking other customer’s liability to the collateral right of the main customer whose asset is pledged as collateral.

After the collateral right of the main customer is in place, to apply the advance ratio and concentration cap, the CO.CALC.CUST.COLLATERAL service is run. This service:

- Applies the collateral advance ratio and concentration cap, if any, and updates the CO.ASSET.DETAILS table with the collateral value of the asset.
- Performs the collateral allocation for the liabilities linked to the collateral right in CO.ALLOCATION.DETAILS table.
- Updates the collateral deficit, if any, in the CO.DEFICIT table.

The above mentioned tables are updated with the LIMIT.COL.ALLOC.WORK identifier and not with the customer identifier.

While applying the advance ratio and concentration cap, the collateral allocation occurs in the following sequence:

- The execution value of the collateral pledge is arrived based on the margin rate (also referred to as High Advance Ratio or HAR) applicable to the asset.
- The single concentration cap (if any) defined for the asset or the standard concentration cap (if any) defined in the CO.VALUATION.PARAMETER is applied on the execution value to arrive at the collateral value after concentration cap.
- This is the collateral value that is allocated to the liabilities in the order of priority defined in the collateral right of the main customer. This information is stored in the CO.ALLOCATION.DETAILS table.
- After allocating the collaterals to the attached liabilities, if any surplus available on the collateral value, it is maintained after applying the adjusted margin rate (also referred to as Low Advance Ration or LAR), if any defined for the collateral asset.
- On the other hand, if the collateral is not sufficient to cover the attached liabilities, the collateral deficit is updated in the CO.DEFICIT table.

The following example having collateral of Customer 190201 cross-pledged to cover own liability as well as the liability of Customer 190202:

COLLATERAL.RIGHT of Customer 190201 is:

Collateral asset pledged by Customer 190201 is:

The collateral asset is allocated as shown in the below screen shot when the service CO.CALC.CUST.COLL.SERVICE is run:

- CO.ASSET.DETAILS is updated with the Alloc Work ID, showing the collateral asset value after applying advance ratio and concentration cap as applicable for the asset pledged.
- CO.ALLOCATION.DETAILS is updated with the Alloc Work ID, showing the collateral allocation after applying advance ratio and concentration cap as applicable for the asset pledged to the own liability and cross pledged liability.
- CO.DEFICIT is updated with the Alloc Work ID, showing the collateral deficit after allocating the collateral.


#### 📋 Tasks

There are no Tasks available for Advance Collateral and Cross Pledging feature.


#### 📊 Outputs

There are no Outputs available for Advance Collateral and Cross Pledging feature.


> **Related Applications:** `CO.ALLOCATION.DETAILS`, `CO.ASSET.DETAILS`, `CO.DEFICIT`, `CO.VALUATION.PARAMETER`, `COLLATERAL.RIGHT`, `LIMIT.COL.ALLOC.WORK`

---


### 1.2  Collateral Advance Ratio


> **📇 Quick Reference Card**
> 
> **Purpose:** *Collateral Advance Ratio is a functionality wherein the Collateral value is derived after applying the advance rate and concentration threshold, if any.*
> 
> **Applications:** `ASSET.BY.CATEG`, `ASSET.TYPE`, `CO.ALLOCATION.DETAILS`, `CO.ASSET.DETAILS`, `CO.CONC.CAP.EXCESS`, `CO.DEFICIT`, `CO.ELIGIBILITY`, `CO.MGN.ALERT` ... +9 more
> 
> **Key Fields:** *Account As Liab*, *Advance Message*, *Allocated Amt*, *Applied Date*, *Ar Drop Alert*, *Avail Amt*, *Bond Cap*, *Bond Ranking* ... +32 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Collateral Advance Ratio is a functionality wherein the Collateral value is derived after applying the advance rate and concentration threshold, if any.

An advance rate is the maximum percentage of the value of a collateral that a lender is willing to extend for a loan. The advance rate helps a borrower determine what kind of collateral to bring to the table in order to secure the desired loan amount, and helps to minimise a lender's loss exposure when accepting collateral that can fluctuate in value.

Collateral helps lenders minimise risks and to offer affordable interest rates to borrowers. By setting an advance rate, a lender can build a cushion into the loan transaction by ensuring that if the value of the collateral drops and the loan goes into default, there is still adequate protection from the loan principal loss. If a lender has an advance rate of 75% and the value of collateral presented is $100,000, then the maximum loan the borrower can receive is $75,000.

Concentration risk is the level of risk in a bank's portfolio arising from concentration to a single counterparty, sector, country or currency. The risk arises from the observation that more concentrated portfolios are less diverse and therefore the returns on the underlying assets are more correlated. Concentration risk is usually monitored by risk functions, committees and boards within commercial banks and is normally only allowed to operate within proscribed limits. It is also monitored by banking regulators and generally attracts a higher capital charge in banking regulation.

Most financial institutions have policies to identify and limit concentration risk. This typically involves setting certain thresholds for various types of risk. Once these thresholds are set, they are managed by frequent and diligent reporting to assess concentration areas and identify elevated thresholds.

A key component to the management of concentration risk is accurately defining thresholds across various concentrations to minimise the combined risks across concentrations.

This feature requires the CX module to be installed in addition to the CO and MV modules.


#### ⚙️ Configuration

The collateral advance ratio considers the high advance ratio, low advance ratio and concentration cap, if defined, to derive the lending value of the collateral.

The high advance ratio is referred as margin rate and the low advance rate is referred as adjusted margin rate in Temenos Transact .

In order to enable the collateral advance ratio functionality, the CO.VALUATION.PARAMETER application must be configured appropriately.


##### ConfiguringCO.VALUATION.PARAMETER

This is a company level parameter, which controls the application of advance ratio and concentration checks to the collateral.

The following fields are configured to enable the advance ratio calculation:

| Field Name | Description |
|---|---|
| Use Advance Ratio | When this field is set to Yes, the collateral execution value is calculated based on the Margin Rate defined for the linked asset at various levels |
| Account As Liab | Accounts linked to limits with negative balance are considered as liabilities when calculating the collateral deficit value, if this field is set to Yes |
| Update Online | If this field is set to Yes, then the advance ratio setup is considered while calculating collateral value online |

The following fields control the application of concentration cap:

| Field Name | Description |
|---|---|
| Conc Cap Level | This is a multi-valued field. This field contains different concentration cap levels used by the system in the order they are processed. This is an optional input. If this field is left blank, then concentration cap processing will not be carried out. Duplicates are not allowed. |
| Std Max Conc Cap | This is an optional field. Any input must be a number from 0 to 100. Any other input is not allowed. It contains the standard maximum concentration cap. |
| Bond Ranking | This is an optional multi-valued field associated with the Bond Cap field. Duplicates (that is, the same value in more than one multi-value) are not allowed. |
| Bond Cap | This is an optional multi-valued field associated with the Bond Ranking field. Any input must be a number from 0 to 100. Any other input is not allowed. |
| Co Allocation | Defines whether the allocation of assets is configured for limits or liabilities. The allowed values are Limits or Contracts. |

If a portfolio is attached as collateral and the Use Advance Ratio flag is set to Yes, then the system automatically takes into account all the assets owned by the portfolio when calculating the portfolio based on the relative margin rates and concentration caps defined on the system, without adding or removing any records in COLLATERAL .


##### Understanding the Hierarchy of Margin Rate and Adjusted Margin Rate

The margin rate and adjusted margin rate is defined at different levels in Temenos Transact and the following hierarchy is considered to get the applicable advance ratio.


##### Understanding the Hierarchy of Concentration Cap

The concentration cap is configured in different applications in Temenos Transact and the following hierarchy is considered to get the applicable concentration cap.

- SC.CUSTOMER.MARGIN for portfolio
- SC.CUSTOMER.MARGIN for customer
- If Security asset, SC.SECURITY.MARGIN SECURITY.MASTER
- If non-security asset, ASSET.BY.CATEG for company ASSET.BY.CATEG
- SUB.ASSET.TYPE for company
- SUB.ASSET.TYPE
- ASSET.TYPE for company
- ASSET.TYPE

> **⚠️ Note:** For discretionary portfolio, the Std Max Conc Cap field in CO.VALUATION.PARAMETER application is considered for concentration cap.


##### Understanding Collateral Eligibility and Ranking

The CO.ELIGIBILITY application is used to define the eligibility rules of the collaterals against a liability. Eligibility is defined based on the collateral type, asset type, sub asset type, and security master.

The key to the CO.ELIGIBILITY application is the Limit product. The Limit product of the liability is obtained and CO.ELIGIBILITY of the corresponding limit product is referred to identify the eligible collaterals.

The CO.RANKING application holds the ranking rules for the collaterals against Limit products. It enables the user to define the order of collaterals for allocation against liabilities.


#### 🔧 Working With

After setting up the COLLATERAL.RIGHT for the main customer, run the CO.CALC.CUST.COLLATERAL service, to apply the advance ratio and concentration cap. This service:

- Applies the collateral advance ratio and concentration cap, if any, and updates the CO.ASSET.DETAILS table with the collateral value of the asset.
- Performs the collateral allocation for the liabilities linked to the collateral right in CO.ALLOCATION.DETAILS table.
- Updates the collateral deficit, if any, in the CO.DEFICIT table.

While applying the advance ratio and concentration cap, the collateral allocation occurs in the following sequence:

- The execution value of the collateral pledge is arrived based on the margin rate (also referred as HAR (High Advance Ratio)) applicable to the asset.
- The single concentration cap (if any) defined for the asset or the standard concentration cap (if any) defined in the CO.VALUATION.PARAMETER application, is used to cap the execution value of the collateral.
- This is the collateral value that is allocated to the liabilities in the order of priority, defined in the COLLATERAL.RIGHT application. This information is stored in the CO.ALLOCATION.DETAILS table.
- After allocating the collaterals to the attached liabilities, if any surplus is available on the collateral value, it is maintained after applying the Adjusted Margin Rate (also referred to as LAR (Low Advance Ratio)), if any is defined for the collateral asset.

On the other hand, if the collateral is not sufficient to cover the attached liabilities, the collateral deficit is updated in the CO.DEFICIT table.

The CO.RECALC.CUST.COLLATERAL service is triggered when there is a change to the margin rate.

The following tables are updated while processing the advance ratio and concentration cap:


##### Collateral Asset Details –CO.ASSET.DETAILS

This table is updated with the details of the collateral assets pertaining to the customer. The information in this table is used for collateral allocation after applying advance ratio and concentration cap.

| Field | Description |
|---|---|
| Customer Id | The ID of the customer |
| Collateral Ccy | Currency of collateral |
| Coll Type | Collateral type ID as in the collateral record |
| Coll Country | Country of the collateral |
| High Adv Ratio | High advance ratio defined for the collateral asset |
| Low Adv Ratio | Low advance ratio defined for the collateral asset |
| Margin Value | Margin value of the collateral |
| Contract Id | Contract linked to the collateral |
| Asset Type | Asset type of the contract linked to collateral |
| Sub Asset Type | Sub Asset type of the contract linked to collateral |
| Sc Industry | Industry code as in record of SECURITY.MASTER . |
| Concentration Cap | Single concentration cap set for the asset |
| No Conc Cap | This field is updated when the collateral type is set not to apply concentration cap |
| Tot Cust Coll | Total value of the collateral in local currency |
| Exch Rate | This field displays the exchange rate for the given asset. It is defined for each asset under the collateral. The exchange rate updated is calculated considering different factors defined in the corresponding record in the CURRENCY application, and it is not necessarily match with the value in the Mid Reval Rate field in the record in the CURRENCY application. The CO.RECALC.CUST.COLL service must be run once to update the exchange rate in the existing record in CO.ASSET.DETAILS . |


##### Collateral Allocation Details –CO.ALLOCATION.DETAILS

This table holds the details of customer assets allocation to customer liabilities.

| Field | Description |
|---|---|
| Customer Id | Valid customer ID |
| Liability Id | Contract ID for which allocation is done |
| Liability Ccy | Currency of contract |
| Liability Amount | Contract amount |
| Liability Categ | Contract category |
| Reserved | Contract reserved |
| Collateral Id | Collateral ID from which amount is allocated to the above contract |
| Collateral Ccy | Collateral currency |
| Avail Amt | Contract amount available in collateral currency |
| Allocated Amt | Contract amount allocated to the above contract in collateral currency |
| Unallocated Amt | Contract amount unallocated |
| Reserved | Collateral reserved |
| Total Alloc | Total amount allocated to contract in contract currency |
| Total Unalloc | Total amount unallocated to contract in contract currency |


##### Collateral Deficit –CO.DEFICIT

This table records customers with a collateral deficit after allocating the available collateral. It is used for collateral deficit reporting and for alerts that are sent to the Relationship Manager.

| Field | Description |
|---|---|
| Customer Id | ID of the customer |
| Deficit Ccy | Currency of deficit amount (local currency of customer company) |
| Total Deficit | Deficit amount (total deficit amount for the customer in LCCY) |
| Buffer Deficit | If the deficit amount is less than buffer specified in OV parameter, then this field is updated |
| Top Up Deficit | If the deficit amount is GE Top up % specified in OV parameter then, this field is updated |
| Sell Out Deficit | If the deficit amount is GE Sell out % specified in OV parameter, then this field is updated |
| Deficit Date | Date on which first CO.DEFICIT is updated |
| Update Date | Date on which the deficit is re-calculated |
| Advance Message | Messages due to advance ratio change |
| Tot Deficit Lar | Total deficit before applying Group concentration cap |


##### Concentration Cap Details -CO.CONC.CAP.EXCESS

This table holds the details of the collateral, which are reduced due to concentration cap setup.

| Field | Description |
|---|---|
| Customer Id | The ID of the customer |
| Conc Cap Level | This is the level of the concentration cap that has been exceeded. This values are: Customer Currency Security Bond Ranking Asset By Categ Asset Type Sub Asset Type Industry |
| Conc Cap Defn | Value of the concentration cap that has been applied. For example, the country code of the country or the currency code of the currency |
| Collateral Id | ID of the collateral for which concentration cap is applied |
| Old Level | Percentage of collateral before the concentration cap is applied |
| Old Value | Value of the collateral before the concentration cap is applied |
| New Level | Percentage of collateral after the concentration cap is applied |
| New Value | Value of the collateral after the concentration cap is applied |
| Applied Date | Date the concentration cap was exceeded |


##### Updating Concentration Cap Excess

The CO.CONC.CAP.EXCESS table is updated only when there is excess in the latest collateral updated. If no cap is applied in the latest collateral update, then the record in CO.CONC.CAP.EXCESS table is deleted.


##### Alerting Deficit Due to Change in Advance Ratio

When a high advance ratio or low advance ratio rate is reduced, it has an impact on the collateral value. The reduction in rates in turn reduce the collateral values which affect the allocation and may lead to deficit as well.

Whenever there is a deficit due to the reduction in HAR or LAR value, or if the deficit has increased due to the reduction, then the CO.MGN.ALERT table is updated with the details about the old HAR or LAR value, the new HAR or LAR value and the collateral value.

The Ar Drop Alert field in the CO.VALUATION.PARAMETER updates the CO.MGN.ALERT table. This table is updated only when this field is set to Yes.


##### Calculating LTMV and LTCV ratio

Banks and financial institutions use the Loan to Market Value (LTMV) and Loan to Collateral Value (LTCV) ratios to assess the lending risk.

Understanding Loan to Market Value

The formula for calculating Loan to Market Value Ratio (LTMV) ratio :

LTMV = (Total Outstanding Liabilities / Total Market Value of the portfolio), where:

- The total outstanding liabilities is the total amount of loans and other liabilities held by the customer.
- The total market value of the portfolio is the value of the portfolio before the application of advance ratio and concentration caps (total nominal value of collaterals).

The formula for calculating Loan to Market Value Ratio (LTMV) ratio :

LTCV = (Total Outstanding Liabilities / Total Collateral Value of the portfolio), where:

- Total outstanding liabilities is the total amount of loans and other liabilities held by the customer.
- Total collateral value of the portfolio is the value of the portfolio after the application of advance ratio and concentration caps (total nominal value of collaterals).

The Loan to Market Value (LTMV) and Loan to Collateral Value (LTCV) are calculated during the collateral valuation services CO.CALC.CUST.COLLATERAL and CO.RECALC.CUST.COLLATERAL. The obtained ratio is stored in the LTMV and LTCV fields in the CO.ASSET.DETAILS record.

| Asset | Value | Currency | High AR | Secured Value | Percentage |
|---|---|---|---|---|---|
| Cash | 100,000 | USD | 90% | $ 90,000 | 7.35% |
| Equities | 400,000 | USD | 80% | $320,000 | 26.23% |
| Equities | 400,000 | USD | 80% | $320,000 | 26.23% |
| Equities | 400,000 | USD | 80% | $320,000 | 26.23% |
| US Treasury Bond | 200,000 | USD | 85% | $170,000 | 11.99% |

| Asset | Value | Currency | High AR | Secured Value | Percentage |
|---|---|---|---|---|---|
| Cash | 100,000 | USD | 90% | $ 90,000 | 7.35 % |
| Equities | 400,000 | USD | 80% | $ 320,000 | 26.23 % |
| Equities | 400,000 | USD | 80% | $ 320,000 | 26.23 % |
| Equities | 400,000 | USD | 80% | $ 320,000 | 26.23 % |
| US Treasury Bond | 200,000 | USD | 85% | $ 170,000 | 11.99 % |


#### 📋 Tasks

There are no Tasks available for Collateral Advance Ratio feature.


#### 📊 Outputs

There are no Outputs available for Collateral Advance Ratio feature.


> **Related Applications:** `ASSET.BY.CATEG`, `ASSET.TYPE`, `CO.ALLOCATION.DETAILS`, `CO.ASSET.DETAILS`, `CO.CONC.CAP.EXCESS`, `CO.DEFICIT`, `CO.ELIGIBILITY`, `CO.MGN.ALERT`, `CO.RANKING`, `CO.VALUATION.PARAMETER`, `COLLATERAL`, `COLLATERAL.RIGHT`, `OV`, `SC.CUSTOMER.MARGIN`, `SC.SECURITY.MARGIN`, `SECURITY.MASTER`, `SUB.ASSET.TYPE`

---


### 1.3  Collateral and Limits


> **📇 Quick Reference Card**
> 
> **Purpose:** *Collateral items can be linked to LIMIT application.*
> 
> **Applications:** `COLLATERAL.RIGHT`, `LIMIT`
> 
> **Key Fields:** *Limit Reference*
> 
> **Sections:** 📖 Introduction | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

A limit can be:

- Secured – Limit is secured, when the collateral is linked to a limit.
- Partly secured – Limit is partly secured, when the value of collateral may not cover the limit amount.
- Unsecured – Limit is unsecured, if there is no collateral coverage.

Collateral items can be linked to LIMIT application.

A mortgage may be linked to a loan limit. The link can either be used for information only (that is, fixed limit), or the value of collateral can be used to determine the availability of limit (that is, variable limit). Thus, a limit can be set to fixed or variable, where it is secured by collateral.

The following flowchart explains the collateral and limit structure.

The link between limits and collateral are established by entering the LIMIT ID or LIMIT KEY in Limit Reference field in COLLATERAL.RIGHT application.

Collateral module supports linking of Limits in the Old key format, that is, Customer based key as well as the New key format, that is, random alpha-numeric key.


#### 📋 Tasks

There are no Tasks available for Collateral and Limits feature.


#### 📊 Outputs

Collateral can be linked to the Limit module, and allows the definition and control of collateralised limits. Collateral Items which are available within Temenos Transact , can be valued automatically by the system periodically. The value of collateral items are updated in regular intervals and the customer’s exposure is calculated based on this value. System sends the alerts to the respective Relationship Manager, whenever the collateral value falls deficit.


##### Enquiries and Reports

The user can view the below list of enquiries and reports:

View Collateral Deficit Alerts

This enquiry lists out the collateral deficit details along with the alert details that are sent to the relationship managers. It helps the Relationship Manager to monitor the collaterals, which falls deficit and make corrective action to reduce the risk of the financial institution.

Main Collateral expiry

This enquiry displays the summary of limits, collaterals of the customer and details of customer’s credit exposure to the company.

View Collateral Asset Details

This enquiry displays the collateral asset details of the customer, which includes value of collateral, loan to market value and margin.

View Collateral Deficit Details

When the customer over utilise the limit, then the respective collateral linked to the limit becomes deficit. This enquiry displays the list of collateral deficits for the each customer’s liability.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA


> **Related Applications:** `COLLATERAL.RIGHT`, `LIMIT`

---


### 1.4  Collateral Exclusion


> **📇 Quick Reference Card**
> 
> **Purpose:** *The bank may decide to exclude certain collaterals from being considered for processing (either partly or fully) as security for the credit facility, based on the economic and market conditions of the collateral asset.*
> 
> **Applications:** `CO.ASSET.DETAILS`, `COLLATERAL`, `COLLATERAL.EXCLUSION`, `COLLATERAL.TYPE`, `COUNTRY`, `SC.INDUSTRY`, `SC.POS.ASSET`, `SECURITY.MASTER`
> 
> **Key Fields:** *Application Id*, *Asset Type*, *Collateral Type*, *Counterparty*, *Country*, *Currency*, *Exclude All*, *Exclusion ID* ... +7 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The bank may decide to exclude certain collaterals from being considered for processing (either partly or fully) as security for the credit facility, based on the economic and market conditions of the collateral asset.


#### ⚙️ Configuration

Temenos Transact provides the functionality to exclude the collateral by defining appropriate exclusion criteria in the COLLATERAL.EXCLUSION application.

When the collateral is created and is available as security for one or more credit facilities, the status changes to CUR (currently active). However, when it is excluded for collateral processing, the status changes to EXC (excluded).


##### Defining the Collateral Exclusion criteria

Collateral exclusion is defined in the COLLATERAL.EXCLUSION application. The criteria for exclusion can be defined in the fields, as mentioned below:

| Field Name | Description |
|---|---|
| Country | Country of the collateral to be excluded. Must be a valid record in COUNTRY application |
| Currency | Collateral's currency, which is to be excluded |
| Security Code | Collaterals that have the security master as asset. Must be a valid record in SECURITY.MASTER application |
| Issuer | Issuer of the security whose collaterals are to be excluded. This is an optional field |
| Industry | Specifies the industry to which the asset belongs. Must be a valid record in SC.INDUSTRY application |
| Counterparty | Counterparty of the asset. Must be a valid Customer record |

The COLLATERAL.EXCLUSION application is defined to exclude collaterals in EUR currency is shown in the below screenshot.


#### 🔧 Working With

This topic details the various ways in which a collateral can be excluded from valuation.


##### Triggering the Collateral Exclusion

The collateral exclusion can be triggered for the COLLATERAL.EXCLUSION application in the following ways:

The Exclude All field can be set to Yes to exclude all the collaterals with the defined criteria. All the collaterals with the defined criteria are updated with the record ID of COLLATERAL.EXCLUSION in the Exclusion Id field in COLLATERAL application, during the execution of online service CO.EXCLUDE.SERVICE.

The below screenshots show that two collaterals (100407.1.1 and 190200.1.2) in EUR currency have been marked for exclusion, after CO.EXCLUDE.SERVICE is executed.

If the user does not want to exclude all the collaterals having EUR currency, the Exclude All field in the COLLATERAL.EXCLUSION application should be unchecked. The user can run the respective COLLATERAL.EXCLUSION application in Verify function (refer the below screenshot), which launches the Exclude Collaterals fast path enquiry with the list of collaterals that satisfies the criteria (that is, the data defined in the COLLATERAL.EXCLUSION application). The collaterals that must be excluded can be selected from the fast path enquiry and committed. It updates the collateral exclusion ID in the Exclusion Id field in the COLLATERAL application.

> **⚠️ Note:** The Verify function is allowed only when Exclude All field is not set to Yes.

The EXCL.CCY record in COLLATERAL.EXCLUSION application is verified as shown in the below screenshot.

The below screenshot displays the Exclude Collaterals fast path enquiry being launched based on the criteria defined in COLLATERAL.EXCLUSION application for the EXCL.CCY record. This enquiry helps the user to select the appropriate collaterals that have to be excluded.

Manually input the collateral record and link the record in COLLATERAL.EXCLUSION in the Exclusion Id field and validate the collateral.

> **⚠️ Note:** The Exclusion Id field is a multi-value field, which allows the user to link multiple exclusion criteria.


##### Removing Exclusion

The exclusion on collaterals can be removed in the following ways:

- Reverse the record in COLLATERAL.EXCLUSION . While running the CO.EXCLUDE.SERVICE, the reversed COLLATERAL.EXCLUSION ID is removed or delinked from the collateral records.
- Input a COLLATERAL.EXCLUSION ID as the selection criteria in the Remove Excluded Collaterals fast path enquiry. Then manually clear the Exclusion Id field for the required collaterals displayed in the enquiry result. Then select the Commit option. The exclusion ID is removed from the record in COLLATERAL .
- Manually remove the COLLATERAL.EXCLUSION ID from the record in COLLATERAL .


##### Understanding Collateral Exclusion for Portfolio Linked as Collateral

A portfolio can be given as collateral, either partly or fully. In other words, the portfolio can be linked as collateral in the following ways:

| Description | Application.ID in Collateral | Example |
|---|---|---|
| Entire portfolio as collateral | - | 190200-1 |
| Specific sub asset type and asset type in the portfolio as collateral | - . . | 190200-1.300.30 |
| Specific security instrument in the portfolio as collateral | - . . * | 190200-1.300.30*800000-006 |


##### Excluding the Entire Portfolio as Collateral

If the entire portfolio is pledged as collateral, it can be flagged for exclusion depending on the nature of the portfolio, whether it is discretionary or non-discretionary.

- The exclusion criteria in COLLATERAL.EXCLUSION can be defined at the currency level for the portfolio reference currency.
- In the record of COLLATERAL application, attach the COLLATERAL.EXCLUSION ID in the Exclusion Id field.
- On authorisation, the status moves to EXC (excluded).

This is because, for a discretionary portfolio, the assets making up the portfolio are under the banks control and investments would not normally be made in assets that are considered too great a risk to be held as collateral. If given as collateral, the whole portfolio is considered as a single asset when attached to the collateral.

Instead, if the bank wants to exclude a discretionary portfolio from being used as a collateral (for whatever reason), the whole portfolio could be excluded.

- When all the underlying assets in the portfolio have same currency, the above-mentioned steps for the discretionary portfolio applies to this as well.
- When the currencies of the underlying assets are different: The exclusion criteria in COLLATERAL.EXCLUSION application can be defined at the collateral country level. In the record in COLLATERAL , attach the collateral exclusion ID in the Exclusion Id field. On authorisation, the status moves to EXC (excluded).

This is because, for a non-discretionary portfolio, the individual underlying assets of the portfolio could be those which the bank does not want to use as collateral. If exclusion criteria is based on the currency, only those underlying assets of the portfolio that matches with the currency in exclusion criteria are excluded, thus resulting in partial exclusion of the portfolio.

A scenario to exclude a non-discretionary portfolio is explained below:

- COLLATERAL.EXCLUSION displaying country level criteria set to US.

- The above COLLATERAL.EXCLUSION application is linked to the 2000.1.1 record in COLLATERAL in the Exclusion ID field and the status is updated as EXC indicating that the collateral is excluded.

- The entire portfolio has been excluded. Hence margin value of all the assets within that portfolio is updated as zero in CO.ASSET.DETAILS table.


##### Excluding Based on Security Master as Collateral

The COLLATERAL.EXCLUSION application can also be used to exclude the portfolio instruments based on the country, currency or security master.

- In order to exclude a specific portfolio instrument as collateral, the security master ID of the respective instrument must be defined as criteria in the Security Code field.

- Attach the exclusion ID and security master detail in the Exclusion ID field of COLLATERAL to exclude the same as shown in the below screenshot.

- Only the specific underlying asset of the portfolio has been excluded. Hence, margin value of the excluded underlying asset alone is updated as zero in the CO.ASSET.DETAILS table, as shown in the below screenshot.

In order to exclude the security master from all the collaterals, where it is linked as collateral (either directly or through the portfolio), the Exclude All field in the respective COLLATERAL.EXCLUSION application is enabled and then re-run the online service CO.EXCLUDE.SERVICE. This marks all the collaterals that has this security master as excluded. The exclusion can be viewed in the CO.ASSET.DETAILS table, where the margin value corresponding to the security master excluded is updated as 0.


##### Excluding Based on Asset Type and Sub Asset Type

It is also possible to include or consider only specific Asset Type and or Sub Asset Type as collateral, by placing the restriction in the COLLATERAL.TYPE application, as shown in the below screenshot.

The specific asset types to be included are defined in the Asset Type field and the specific sub asset types to be included are defined in the Sub Asset Type field.

The underlying assets in the portfolio that matches the defined asset type or sub asset type is considered only as collateral. The other underlying assets in the portfolio are considered as excluded.

The below screenshot displays a portfolio (190201-1) linked as collateral with Collateral Type - 103, which places a restriction of the inclusive asset type and sub asset type.

The screenshot below displays the list of SC.POS.ASSET for the portfolio:

The CO.ASSET.DETAILS table is updated only for the inclusive asset types and sub asset types defined for the collateral type.

> **⚠️ Note:** The underlying assets (190201-1.1.1 and 190201-1.302.30), are excluded from being considered as collateral though they are part of the portfolio.


#### 📋 Tasks

There are no Tasks available for Collateral Exclusion feature.


#### 📊 Outputs

There are no Outputs available for Collateral Exclusion feature.


> **Related Applications:** `CO.ASSET.DETAILS`, `COLLATERAL`, `COLLATERAL.EXCLUSION`, `COLLATERAL.TYPE`, `COUNTRY`, `SC.INDUSTRY`, `SC.POS.ASSET`, `SECURITY.MASTER`

---


### 1.5  CollateralExclusionAdvanceRatioConcentrationCap


> **📇 Quick Reference Card**
> 
> **Purpose:** *This functionality enables the exclusion of specific collateral type and portfolio typefrom advance concentration cap and advance ratios calculation.*
> 
> **Applications:** `ACCOUNT`, `ASSET.TYPE`, `CO.ALLOCATION.DETAILS`, `CO.ASSET.DETAILS`, `CO.VALUATION.PARAMETER`, `COLLATERAL.EXCLUSION`, `COLLATERAL.RIGHT`, `MANAGED` ... +4 more
> 
> **Key Fields:** *Disc*, *Excl Collateral*, *Excl Collateral Type*, *Exclude All*, *No Conc Cap*, *No Port Valuation*, *Portfolio*, *Portfolios* ... +2 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

This functionality enables the exclusion of specific collateral type and portfolio typefrom advance concentration cap and advance ratios calculation.

While processing collateral exclusions, if a portfolio is attached as collateral, then the underlying assets are excluded from the portfolio value that is used in calculating the collateral value of the portfolio, provided:

- The underlying asset matches the exclusion criteria.
- The portfolio is not a discretionary portfolio.

This feature requires the CX module to be installed in addition to the CO and MV modules.


#### ⚙️ Configuration

The following fields in CO.VALUATION.PARAMETER application enable the configuration of collateral allocation and exclusion criteria for specific or all the collateral types:

- Excl Collateral Type – Contains the list of collateral types excluded from the advance collateral functionality. The allowed valid value is Collateral Type or All. If All is defined, then the system excludes all the collateral types while applying the advance ratio. and this, in turn, behaves like Use Advance Ratio field set to No.
- No Conc Cap – Configured with the portfolio type or the collateral type on which concentration cap is not applied. The record in MANAGED.ACCOUNT , which represents the portfolio type must be prefixed with M and the collateral type must be prefixed with C before the ID (as shown in the below screenshot).

The No Port Valuation field is checked if the portfolio pledged as collateral must be excluded from advance collateral process.


#### 🔧 Working With


##### Exclusion of Collateral Type while applying Advance Ratio

The collateral assets pledged by the customer that come under the collateral type defined in Excl Collateral field is excluded from applying the advance ratio and concentration cap. To exclude the collateral type from the concentration cap alone, it has to be defined in No Conc Cap field prefixed with C (to indicate collateral type). For example, C-557.

| Collateral ID | Collateral Type | Collateral Ccy | Nominal Value | Execution Value |
|---|---|---|---|---|
| 100025.1.1 | 561 | USD | 50,000 | 50,000 |
| 100025.1.2 | 562 | USD | 10,000 | 10,000 |
| 100025.1.3 | 563 | USD | 15,000 | 15,000 |


##### Exclusion of Portfolio for applying Advance Ratio

The portfolio can be discretionary or non-discretionary in nature. This depends on how the portfolio is managed.

- Discretionary Portfolio – Many banks offer a discretionary service to investors, whereby the bank's officers have the power of attorney over decisions affecting the portfolio account (that is, what and when, to buy or sell, and at what price). They also decide the content of that portfolio with regard to its holdings in, for example, equities and bonds. In this case, the entire portfolio is considered as a single asset when attached to the collateral.
- Non-Discretionary Portfolio – Some customers insist on running their own portfolios and these would be set up as non-discretionary accounts. In this case, each asset linked to the portfolio is considered separately when attached to a collateral.

The Disc Portfolio field is used to configure the list of managed accounts that corresponds to discretionary portfolios.

When selecting assets to exclude from the collateral, the system checks if the asset is held as part of a discretionary portfolio. If yes, then the asset continues to be included in the collateral and its value is not excluded from the collateral available to the customer who owns the discretionary portfolio.

The workflow is explained below:

1. The collateral exclusion is entered.
2. When the system selects a collateral for exclusion, it checks whether the asset is linked to a portfolio.
3. If the asset is linked to a portfolio, then the MANAGED . ACCOUNT of the portfolio is checked against the list of portfolio types held in the Disc Portfolios field in the record of CO.VALUATION.PARAMETER .
4. If the asset is owned by a discretionary portfolio, then it is not excluded from the collateral and the value of the asset continues to be included in the collateral offered by the customer.
5. If the entire discretionary portfolio matches the exclusion criteria, then the entire portfolio is excluded and its collateral value is set to zero.

The processing is based on the below considerations:

- For non-discretionary and discretionary portfolios, the margin value is calculated for each asset, that is, HAR rate can be from different levels based on its respective hierarchy.
- For a non-discretionary portfolio, LAR is obtained from the same hierarchy of applications as done for HAR.
- For discretionary portfolio, LAR is always from MANAGED.ACCOUNT .
- When rates are defined in SC.CUSTOMER.MARGIN for a customer or portfolio (or) in MANAGED.ACCOUNT , then all the records in SC.POS.ASSET in the portfolio refer to the same application for rates, where the rates are stored in CO.ASSET.DETAILS table for a discretionary portfolio. If the rates are from different levels, then the rate cannot be maintained in the CO.ASSET.DETAILS table, so in that case HAR has to be Null for the discretionary portfolio and LAR has to be from SC.CUSTOMER.MARGIN or MANAGED.ACCOUNT.
- If there is a change in rates in ASSET.TYPE or SUB.ASSET.TYPE , it is reflected for portfolio assets only when it is mirrored in SC.POS.ASSET table through the Portfolio Valuation Cost enquiry or OV service. Collateral with portfolio always refers to the rates from SC.POS.ASSET table.
- Asset based exclusion happens only through CO.EXCLUDE.SERVICE when Exclude All field is set to Yes in the COLLATERAL.EXCLUSION and in the manual exclusion.


#### 📋 Tasks

There are no Tasks available for Collateral Exclusion for Advance Ratio and Concentration Cap feature.


#### 📊 Outputs

There are no Outputs available for Collateral Exclusion for Advance Ratio and Concentration Cap feature.


> **Related Applications:** `ACCOUNT`, `ASSET.TYPE`, `CO.ALLOCATION.DETAILS`, `CO.ASSET.DETAILS`, `CO.VALUATION.PARAMETER`, `COLLATERAL.EXCLUSION`, `COLLATERAL.RIGHT`, `MANAGED`, `MANAGED.ACCOUNT`, `SC.CUSTOMER.MARGIN`, `SC.POS.ASSET`, `SUB.ASSET.TYPE`

---


### 1.6  CollateralPledgeReduction


> **📇 Quick Reference Card**
> 
> **Purpose:** *This section covers the overview of this feature.*
> 
> **Applications:** `COLLATERAL.PARAMETER`, `LIMIT`, `LIMIT.PARAMETER`
> 
> **Key Fields:** *Available Amount*, *Check*, *Coll*, *Dda Limit Excess Check*, *Tolerance*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

This section covers the overview of this feature.


##### Generating Override for Insufficient Pledge on Utilised Part of a Variable Limit

All Temenos applications that generate cash and securities movements, except for the corporate actions, generate an override when it affects the value of at least one collateral used to cover the variable limit.

When a transaction is input, the system recalculates the values of collaterals for all the involved variable limits to which the collaterals are linked considering the current transaction value. Among all variable limits impacted, if one is not sufficiently covered by the collaterals, then the system generates an override. Considering that the current transaction is not yet authorised, its impact on the collateral values and available amounts work like simulation.


##### Setting Tolerance on Limit

In Temenos Transact , the security prices or exchange rates might not be up to date, so there is an option to define tolerance on limit.

The tolerance value can either be positive, negative or zero.


#### ⚙️ Configuration

This topic covers the configuration to setup the collateral pledge reduction functionality.


##### Generating Override for Insufficient Pledge on Utilised Part of a Variable Limit

The Coll Check field in the COLLATERAL.PARAMETER application is used to control whether to raise a detailed override during breach of collateral pledged against the variable limit. If this field is set to Yes, the system generates additional and detailed override message on collateral breaches against the variable limit.

The override can be a single override or multiple limit excess override, based on the setup in Dda Limit Excess Check field in the LIMIT.PARAMETER application.


##### Setting up Tolerance on Limit

For the system to cater to the fluctuations in security prices or exchange rates, a percentage of tolerance on the limit needs to be defined. This percentage is defined in the Tolerance field in the COLLATERAL.PARAMETER application. Definition of tolerance is allowed only when Coll Check field is set to Yes.


#### 🔧 Working With

The system detects online breaches in the variable limits granted when inputting any operation that changes the valuation of collaterals linked to these variable limits. After system detects insufficient pledge, it generates an override at the operation input level.

Whenever there is a debit transaction on the asset linked as collateral, the system raises an override in the following scenarios:

- Asset attached as collateral is linked to variable limit.
- The latest collateral value post the current transaction is not able to cover the: Utilized portion of the limit (assuming no tolerance is defined). Utilized portion of the limit + Tolerance % defined in COLLATERAL.PARAMETER .

If the current operation is not authorised, its impact on collateral values and available limit amounts is like a simulation.

The format of the override is as follows:

- LIMIT XXXXX.XXX.N breached
- Amount available is NNNN CCY
- New total value of collaterals is NNN CCY

The above override format includes the following:

- List of the limit IDs whose utilised portion is not covered by the collateral.
- Available amount of limit before the current transaction (outstanding (minus) the amount allocated from collateral to this limit). This information is taken from the Available Amount field in the LIMIT application.
- Latest amount of collateral including the current transaction that is allocated to the limit.

An override indicating the reduction in the collateral that is pledged is raised in the following scenarios:

- Only when the current transaction has an impact on the collateral.
- Only for any debit to collaterals not credit to collaterals.
- When a limit in a structure is already in deficit, that is, there is insufficient collateral to cover the limit, more debits to that collateral raise this override even if there is no impact to the limit.
- An override is raised for the limits if there is a breach even if it is not directly linked to collateral.

The transaction with the override is routed to the Department Account Officer (DAO) according to the appropriate settings for approval, based on the breach amount.

An override is not raised or considered for:

- Fixed limits
- Existing revaluation process.

The latest value can only be simulated with no update in the tables. The below listed functionality are not impacted.

- HVT accounts
- Non-sufficient funds
- Revised limit features involving validation limits, utilisation limits and reporting limits
- Group limits
- Advance collateral


##### Understanding Transaction Workflow

Temenos Transact simulates the collateral value based on the current transaction amount, reallocates limits based on the latest collateral value, allocates only the utilised amount of limit, checks for breaches and raises override in case of variable limit.

| Limit Id | Linked Collateral rights | Underlying collaterals |
|---|---|---|
| 42000.2010.01 | 42000.1 | 42000.1.1 |
| 42000.1.2 |  |  |
| 42000.2 | 42000.2.1 |  |
| 42000.2.2 |  |  |
| 42000.2.3 |  |  |
| 42000.2010.02 | 42000.1 | 42000.1.1 |
| 42000.1.2 |  |  |
| 42000.2 | 42000.2.1 |  |
| 42000.2.2 |  |  |
| 42000.2.3 |  |  |
| 42000.2010.03 | 42000.2 | 42000.2.1 |
| 42000.2.2 |  |  |
| 42000.2.3 |  |  |

| Limit ID | Collateral ID |
|---|---|
| 44000.100.01 | 44000.01 |
| 44000.02 |  |
| 44000.100.02 | 44000.02 |


#### 📋 Tasks

There are no Tasks available for Collateral Pledge Reduction feature.


#### 📊 Outputs

There are no Outputs available for Collateral Pledge Reduction feature.


> **Related Applications:** `COLLATERAL.PARAMETER`, `LIMIT`, `LIMIT.PARAMETER`

---


### 1.7  ConcentrationChecksClientPortfolio


> **📇 Quick Reference Card**
> 
> **Purpose:** *Concentration cap is applied to mitigate the risk associated with the collateral by capping single counter holding and ensuring a basket of holding.*
> 
> **Applications:** `CO.VALUATION.PARAMETER`, `SC.PARAMETER`, `SC.POS.ASSET`, `SEC.ACC.MASTER`, `SECURITY.MASTER`
> 
> **Key Fields:** *Bef*, *Cap*, *Ccy*, *Conc*, *Include Concentration Cap*, *M*, *Margin*, *Margin Value* ... +13 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Concentration cap is applied to mitigate the risk associated with the collateral by capping single counter holding and ensuring a basket of holding.

The application of concentration cap may not be required for all customer portfolios. Some banks may want to apply the concentration cap only on portfolio that is pledged as collateral, whose value is greater than a configured threshold value.

It is also possible to exclude specific assets of the portfolio from application of concentration check.

This feature requires the CX module to be installed in addition to the CO and MV modules.


#### ⚙️ Configuration

The user configures the following parameter, to apply concentration checks for validating the eligibility of a portfolio that is pledged as collateral.


##### ConfiguringSC.PARAMETER

The Include Concentration Cap field is set to Yes in the SC.PARAMETER application. If this field is not set to Yes, then the concentration checks do not apply to the collateral value (margin value) of the portfolio.


##### ConfiguringCO.VALUATION.PARAMETER

The threshold or qualifying currency and the value is configured in the Pf.Qual.Ccy and Pf.Qual.Value fields respectively.

The values defined in these fields determine if the portfolio qualifies for application of concentration check.

The Include Concentration Cap field in SC.PARAMETER application must be set to Yes to allow the definition of appropriate values in Pf Qual Ccy and Pf Qual Value fields. Otherwise, an error message is displayed while validating the record in CO.VALUATION.PARAMETER .

If the value is Null in these fields, it indicates that concentration check is not applicable to any of the portfolio that is pledged as collateral.

If a bank wants to apply concentration checks on all the pledged portfolio irrespective of the value of the portfolio, the Pf Qual Value field must be set to 0 (zero).

The following screenshot shows the

field set to USD and

field set to 400,000.

This configuration implies that any portfolio, whose collateral value (margin value) is greater than USD 400,000 qualifies for the application of concentration check.


#### 🔧 Working With

The Temenos Transact Collateral module provides the framework to apply the concentration cap on the risk assets that are part of the portfolio, attached as collateral. It caters to trimming the Collateral Lending Value (CLV) of the assets in the portfolio based on the applicable concentration cap after applying the High Advance Ratio (HAR) (also referred as margin rate in Temenos Transact ).

The single concentration cap, if defined, is applied on the CLV of the asset that is attached as collateral. If the CLV of any asset in the portfolio is greater than the single concentration cap value, it is trimmed to the extent of a single concentration cap value and the total CLV gets reduced to that extent.

The asset or liability currency matching or allocation for same currency liability takes place after applying the single concentration cap. The unallocated collateral lending value (liability not allocated against the asset of the same currency) is re-calculated based on the Low Advance Ratio (LAR) (also referred as adjusted margin rate in Temenos Transact ). In other words, HAR is applied for an asset if it is allocated against the liability in the same currency. On the other hand, LAR is applied on an asset if it is allocated against the liability in a different currency. In case where residual (that is, unallocated) amount is left after allocation of an asset against a liability in the same currency, a LAR is applied on the unallocated amount. However, defining a LAR is optional and it is based on the banking practices followed.

The value of the assets and liabilities linked to the portfolio are represented in the reference currency of the portfolio. The margin rate or HAR is applied to determine the CLV or margin value. During the valuation process, the CLV is updated as the margin value of the asset in the SC.POS.ASSET table. The consolidated margin value or CLV of the portfolio is updated in the Margin Value field in the SEC.ACC.MASTER application.

The portfolio threshold or qualification check is carried out whenever the collateral valuation takes place considering the CLV of the portfolio while performing the valuation.


##### When the Value of Portfolio Qualifies for Concentration Check

If the value of the portfolio is greater than or equal to the value defined in the Pf Qual Value field in the CO.VALUATION.PARAMETER application, the portfolio qualifies for concentration check.

In other words, if the margin value of the portfolio at HAR (that is, margin rate applicable) is greater than the parameterised threshold value, then the M argin V alue field in the SC.POS.ASSET table is updated with the value after applying concentration cap. That is if the margin value is greater than the cap amount, the margin value is trimmed to the extent of the concentration cap amount. The margin value at HAR gets updated in the Mv Bef Conc Cap field in the SC.POS.ASSET table for the respective asset.

The following screenshot shows the update of Margin Value and Mv Bef Conc Cap fields for a portfolio whose value is greater than the defined threshold value.


##### When the Value of Portfolio Does Not Qualify for Concentration Check

If the value of the portfolio is lesser than the value defined in the Pf Qual Value field in the CO.VALUATION.PARAMETER application, the portfolio does not qualify for application of concentration check.

In other words, if the margin value of the portfolio at HAR (that is, margin rate applicable) is lesser than the parameterised threshold value, the Margin Value field in the SC.POS.ASSET table is updated with the same value as the margin value at HAR without applying the concentration cap. In this case, the values in the Margin Value and Mv Bef Conc Cap fields in the SC.POS.ASSET table for the respective asset is the same as in HAR (or margin rate).

The following screenshot shows the update of Margin Value and Mv Bef Conc Cap fields for a portfolio whose value is lesser than the defined threshold value.

The Margin Value of the portfolio in SEC.ACC.MASTER is the sum of Margin Values of the individual SC.POS.ASSET table.


##### When the Reference Currency of Portfolio is Different from Qualifying Currency

The value of a portfolio is calculated in the reference currency of the portfolio. If the reference currency of the portfolio is different from the Pf Qual Ccy defined in the parameter, the value of the portfolio in the reference currency is converted to the currency entered in the Pf Qual Ccy at the prevailing mid-rate for comparing with the threshold value, and then the checks are applied.


##### Excluding Assets for Concentration Check

The portfolio also include assets that are to be excluded from the application of concentration cap. If the bank wishes to exclude any asset(s) from application of concentration cap, the concentration cap must be marked as 100% for the respective asset in the SECURITY.MASTER .

The asset level concentration cap is defined as 30% for shares. However, the bank wants to exclude the shares of a company from concentration cap checks. The same can be achieved by marking the concentration cap as 100% for that company stock in the respective record in

, as shown in the following screenshot.

If the asset is part of any client portfolio that is attached as collateral, the concentration cap is not applied on the asset because the contribution of this asset cannot be greater than 100% of the CLV. Thus, it gets excluded from the application of the concentration cap.


#### 📋 Tasks

There are no Tasks available for Concentration Checks for Client Portfolio feature.


#### 📊 Outputs

There are no Outputs available for Concentration Checks for Client Portfolio feature.


> **Related Applications:** `CO.VALUATION.PARAMETER`, `SC.PARAMETER`, `SC.POS.ASSET`, `SEC.ACC.MASTER`, `SECURITY.MASTER`

---


### 1.8  Corporate Collateral Pool


> **📇 Quick Reference Card**
> 
> **Purpose:** *As corporate lending involves high risk exposures, banks request their corporate customers to provide appropriate collateral coverage to mitigate the risk. This results in the need to handle large number of collateral assets of varied nature.*
> 
> **Key Fields:** *Account Level Haircut*, *Allocation Option*, *Allocation Work Id*, *Collateral Account ID*, *Collateral Account Ranking*, *Collateral Item*, *Collateral Pool Reference*, *Collateral Provider* ... +15 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks


#### 📖 Introduction

As corporate lending involves high risk exposures, banks request their corporate customers to provide appropriate collateral coverage to mitigate the risk. This results in the need to handle large number of collateral assets of varied nature.

The collateral pool functionality helps corporates to pool the huge amount of available collaterals to cover the risk exposures at one place. The collateral items provided by the customer are grouped in a structured manner, based on the volatility and ranking of the collateral assets and pooled together to cover the risk exposures.

Thus, the collateral pool brings together the collateral items of one or more providers to cover the risk exposures of one or more borrowers.

By bringing the collateral items and exposures under one pool, it is possible to calculate the collateral sufficiency of the pool. This enables the bank user to:

- Request for additional collateral cover, if it falls short, (or)
- Plan the usage of collateral to cover other exposures of the corporate if the collateral is in excess.

Collaterals linked to the pool are allocated to cover the risk exposures in the pool and hence, the same collateral item cannot be used in different pools. Similarly, the risk exposure linked to a pool cannot be linked to another collateral pool.

This feature requires COPOOL module to be installed in addition to the CO module.

The COPOOL (Collateral Pool) module enables the following with respect to Collateral Pool functionality:

- Configuration of Sufficiency Threshold, Default Pool Allocation, Purge Period for Sufficiency Breach and Pool Exceptions in the COLLATERAL.PARAMETER .
- Creation of Collateral Account.
- Creation of Collateral Pool.


#### ⚙️ Configuration

The collateral pool is designed to pool the collaterals provided by the borrower(s) to cover one or more of the risk exposures.

In Temenos Transact , the individual collateral items are captured in the COLLATERAL application and corporate risk exposures are captured in the ARRANGEMENT application.

In the case of corporate risk exposures, the value of credit exposure is high and the collateral can be provided by many customers who are associated with the exposure. The individual collateral items provided by the respective customer are grouped into a logical structure, based on their ranking and volatility and other market regulations, into a collateral account.

The collateral account of the associated customers are then pooled together in a collateral pool to cover the associated risk exposure(s).

The following image shows a sample collateral pool structure.


#### 📋 Tasks

Related topics:

- Create And Link Collateral

The COLLATERAL.ACCOUNT application allows the bank user or customer to group collaterals together from the same customer or provider, for maintenance and management purposes.

The individual items of collateral of the provider need to be structured or bundled based on the quality and ranking or rating. These structured collaterals can be used in the collateral pool to cover the exposure of one or more owner(s).

The COLLATERAL.POOL application allows the bank user to group collaterals together, recorded within different Collateral Account’s and link them with multiple risk exposures.

The COLLATERAL application is used to keep a track of the securities received from the customer in T24. A group of relevant collateral records are mapped under a collateral account.

The system performs the Collateral Allocation process using the Collateral Ranking and Collateral Codes as parameters.


##### Workflow

This sections allows the user to perform the below activities:

Collateral Account module allows the user to create and maintain collateral accounts.

To create a collateral account, follow the below steps:

1. Create Collateral Account .
2. Enter values in the following fields: Nomination Currency GB Account Description Collateral Provider Relationship Officer Collateral Item Account Level Haircut Collateral Account Ranking Start Date End Date Review Date Frequency Collateral Status Collateral Pool Reference
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon to submit the record. Upon committing the record, system creates the collateral item in unauthorised status.

This enquiry lists all unauthorised collateral account records with details such as, Collateral Account ID, Customer, Collateral Type, Collateral Account Status, Collateral Account Currency, Collateral Value, Collateral Code, Collateral Items and so on.

To authorise a Collateral Account, follow the below steps:

1. Authorise/Delete Collateral Accounts .
2. Click the Authorise icon corresponding to a record, in the Unauthorised Collateral Account section.
3. Click the Authorise icon in the Collateral Account Details screen.

To delete a Collateral Account, follow the below steps:

1. Authorise/Delete Collateral Accounts .
2. Click the Delete icon corresponding to a record, in the Unauthorised Collateral Account section.
3. Click the Delete icon in the Collateral Account Details screen.
4. Click OK button in the message box that appears.

Collateral Pool module allows the user to create and maintain collateral Pool.

To create a Collateral Pool, follow the below steps:

1. Create Collateral Pool .
2. Enter values in the following fields : GB Description Reference Currency Collateral Account ID Pool Level Haircut Exposure ID Risk Exclusion ID Sufficiency Ratio Start Date Review Date Frequency Expiry Date Allocation Option Status Allocation Work Id
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon to submit the record. Upon committing the record, system creates the Collateral Pool in unauthorised status.

This enquiry lists all unauthorised collateral pool records along with details such as, Collateral Pool ID, Collateral Account ID, Currency, Start Date, Expiry Date, Review Date Frequency and so on.

To authorise a Collateral Pool, follow the below steps:

1. Authorise/Delete Collateral Pools .
2. Click the Authorise icon corresponding to a record in the Unauthorised Collateral Pool section.
3. Click the Authorise icon in the Collateral Pool Details screen.

To delete a Collateral Pool, follow the below steps:

1. Authorise/Delete Collateral Pools .
2. Click the Delete icon corresponding to a record, in the Unauthorised Collateral Pool section.
3. Click the Delete icon in the Collateral Account Details screen.
4. Click OK in the message box that appears.

This COLLATERAL.ACCOUNT application enables the user to make entry of collaterals under a single account.

To amend a collateral account, follow the below steps:

1. Amend Collateral Accounts .
2. In the Amend Collateral account screen, click the Edit button corresponding to a record.
3. In the Create collateral account screen, enter values in the required fields.
4. Click the Validate icon and accept overrides, if any.
5. Click the Commit icon.

To view a collateral account, follow the below steps:

1. Amend Collateral Accounts .
2. In the Amend Collateral account screen, click the View button corresponding to a record.
3. In the Create collateral account screen, verify the values in the respective fields.

---


### 1.9  Creating Collateral Item


> **📇 Quick Reference Card**
> 
> **Purpose:** *The asset provided or pledged by the customer to secure a loan or liability is referred as collateral item or collateral asset. Collateral becomes mandatory for a secured loan, while it is optional for an unsecured loan. However, bank can stipulate the items accepted as collateral. The customer can ...*
> 
> **Key Fields:** *Application.ID*, *Collateral Details*, *Collateral.Code*, *Collateral.Type*, *Country*, *Currency*, *Execution.Value*, *Expiry.Date* ... +4 more
> 
> **Sections:** 📖 Introduction | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The asset provided or pledged by the customer to secure a loan or liability is referred as collateral item or collateral asset. Collateral becomes mandatory for a secured loan, while it is optional for an unsecured loan. However, bank can stipulate the items accepted as collateral. The customer can provide items of collateral maintained outside the bank ( residential property, art and artifacts, jewellery and the like) or can provide items that are maintained by the bank (fixed deposit, portfolio, guarantees and the like).

In Temenos Transact Collateral items can be created before or after creating a Right on the Collateral.


#### 📋 Tasks

Related topics:

- Create And Link Collateral

In Temenos Transact , Collateral file is used to record the details of collateral submitted by a customer. Generally, collateral is provided by the customer to avail the credit facility from a financial institution. The collateral item is defined on the COLLATERAL application which contains details of review frequency, value date and expiry of the collateral. Each collateral object belongs to a COLLATERAL.RIGHT application. This is implicit in the item-id structures of the file.


##### Workflow

To amend, authorise and delete a collateral, perform the steps given in the below procedures:

Collateral module allows the user to create and maintain collateral details, monitor and control the limits with collateral.

To create a collateral, follow the below steps:

1. Create Collateral .
2. In the Contract Screen, select a record from the Collateral Details field.
3. Click the Edit icon and provide values in the following fields: Collateral.Type field defines the broader type of collateral objects provided by the customer and content of this field must be a valid number defined on the COLLATERAL.TYPE file. Collateral.Code field explains the sub classification of collateral objects, which are mapped to the each collateral rights. Currency field is used to capture the collateral currency. Application.ID helps to fetch the collaterals values which are within Temenos Transact especially in cases such as a Deposit Account, fixed term Deposit, and Client portfolio of stocks. Country field is used to capture the country where the collateral item is originally located or available. Nominal.Value is the overall original or nominal value of the collateral and this is for information purpose only. This value is not involved in any of the collateral processing which takes place in the system. Execution.Value is the accepted or final execution value of the collateral which is used for collateral processing. Value.Date is the date on which the collateral values were accepted and/or recorded in the system Review.Frequency field is to capture the date and frequency of collateral review. A combined date & frequency field which is automatically cycled by the system as part of the collateral application's end-of-day Expiry.Date field provides the option to enter the date of expiry on both COLLATERAL item and the controlling COLLATERAL.RIGHT . Once the COLLATERAL expiry date is reached, the value is no longer useable by the system. Industry field enables the user to capture the industry of the security collateral.
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon to submit the record. Upon committing the record, system creates the collateral item in unauthorised status.

This enquiry lists all unauthorised collateral records along with customer details such as Collateral ID, Collateral Customer, Collateral Type, Collateral Code, Currency, Nominal Value, Status and Inputter.

To authorise a Collateral, follow the below steps:

1. Collateral .
2. In the Unauthorised Collateral screen, click the Authorise icon.
3. In the Collateral Details screen, click the Authorise icon.

To delete a Collateral, follow the below steps:

1. Collateral .
2. In the Unauthorised Collateral screen, click the Delete icon.
3. In the Collateral Details screen, click the Delete icon.
4. Click the OK button.


#### 📊 Outputs

There are no Outputs available for Create Collateral Item feature.

---


### 1.10  External Collateral Assets


> **📇 Quick Reference Card**
> 
> **Purpose:** *External assets such as assignments, floating charges, fixed charges and life insurances are not maintained in Temenos Transact core applications. The information related to these external assets may be maintained in bank-specific local tables. These external assets are provided as collateral for se...*
> 
> **Key Fields:** *Application*, *Execution Value*, *Ext Currency*, *Ext Execution Value*, *Ext Margin Rate*, *Ext Nominal Value*, *External Table*, *Nominal* ... +1 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

External assets such as assignments, floating charges, fixed charges and life insurances are not maintained in Temenos Transact core applications. The information related to these external assets may be maintained in bank-specific local tables. These external assets are provided as collateral for securing a certain facility or liability in Temenos Transact. The user can configure these external assets as collaterals to be processed by the Collateral module in Temenos Transact.


#### ⚙️ Configuration

The external asset must be linked to the COLLATERAL.TYPE application. The Application field in COLLATERAL.TYPE must be set to External for the external asset to be treated as a collateral. The other fields related to the external asset should also be updated.

For linking an external asset to the Collateral module in Temenos Transact, the following are necessary:

- The External Table field is mandatory if the Application field is set to External. The external asset defined in the External Table field must be a valid external asset application name.
- All the fields mapped from the external asset in COLLATERAL.TYPE must be valid field names in the External asset application.
- The Ext Nominal Value field is mandatory if the Nominal or Execution Value field is set to F (Fed).
- The Ext Margin Rate and Ext Execution Value fields are mutually exclusive fields. Both the fields cannot be updated together.
- The Ext Margin Rate or Ext Execution Value field is mandatory if Execution Value is set to FM (Fed/Margin).
- When Nominal Value and Execution Value are given as FM, either the Ext Nominal Value field along with the Ext Margin Rate can be defined or only the Ext Execution Value can be defined.
- The Ext Currency field is mandatory if Ext Nominal Value or Ext Execution Value (in case Execution Value is FM) is defined.
- Multiple applications (like accounts, guarantees, arrangement architecture and customer portfolio) are not allowed in COLLATERAL.TYPE if the option chosen in Application is External. Also, the option External cannot be given multiple times in a given COLLATERAL.TYPE .
- The bank-specific local table (where the external asset details are maintained) as well as COLLATERAL.TYPE must be available in the same company, if they are being linked.

The following screenshot shows the COLLATERAL.TYPE application with the fields to link the external asset:


#### 📋 Tasks

CO.REG.INSURANCE , ASSET.REG.PROPERTY and CO.REG.MORTGAGE tables are designed to capture external assets like Mortgages, Assignments, Floating Charges, fixed charges and life insurance details. These tables are linked with the Temenos Transact collateral module to secure given facility or liability.


##### Workflow

This feature allows the user to perform the following tasks:

CO.REG.INSURANCE is an application to capture the details of Life insurance policy provided as collateral.

To create an insurance record, follow the below steps:

1. Input Insurance- Asset Register .
2. Enter values in all or relevant fields: Description Life Insurance Type Policy Number Insurance Owner Insured Customer Insurance Company Currency Insured Amount Surrender Value Insurance Premium Coefficient Adjusted Market Value Suggested Adjusted Market Value Contract Start Date Contract Expiry Date
3. Click the Validate icon to check for overrides and errors.
4. Click the Commit icon to create the record.

This enquiry allows the user to view or amend the existing Insurance records.

To amend an Insurance general details record, follow the below steps:

1. View/Amend Insurance Details .
2. In the Insurance General Details screen, click the Amend icon corresponding to a record.
3. Amend the required details.
4. Click the Validate icon to check for overrides and errors.
5. Click the Commit icon to amend the record.

To view Insurance general details records, follow the below steps:

1. View/Amend Insurance Details .
2. In the Insurance General Details screen, click the View icon to view the corresponding record in detail.


#### 📊 Outputs

There are no Outputs available for External Collateral Assets feature.

---


### 1.11  Group Concentration Cap


> **📇 Quick Reference Card**
> 
> **Purpose:** *Group concentration caps are set at a percentage level and apply to all assets that match the criteria of the group concentration cap.*
> 
> **Applications:** `CO.COUNTRY`, `CO.COUNTRY.GROUP`, `CO.CURRENCY`, `CO.INDUSTRY`, `CO.VALUATION.PARAMETER`, `COUNTRY`, `CURRENCY`, `SC.INDUSTRY`
> 
> **Key Fields:** *Adj Margin Rate*, *Concentration Cap*, *Country*, *Description*, *Emerging Market*, *Emerging Market Group*, *Margin Rate*, *Prd Adj Margin Rate* ... +2 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Group concentration caps are set at a percentage level and apply to all assets that match the criteria of the group concentration cap.

A group concentration cap is defined in the following applications:

- CO.CURRENCY
- CO.COUNTRY
- CO.COUNTRY.GROUP
- CO.INDUSTRY

The order in which the group concentration cap is applied is defined in CO.VALUATION.PARAMETER application. The group concentration cap is applied during the CO.CALC.CUST.COLLATERAL service.

This feature requires the CX module to be installed in addition to the CO and MV modules.


#### ⚙️ Configuration

Group concentration cap is defined at currency, country, country group and industry levels.


##### Currency –CO.CURRENCY

This application holds the rules defined to modify the advance ratio of assets valued in a currency. It is entered in the currency code and contains percentages that increase or decrease the advance ratio used to calculate the collateral.

> **⚠️ Note:** Note: The application ID is a currency and it must be a valid record in CURRENCY application.

| Field | Description |
|---|---|
| Margin Rate | Allows the modification of the advance ratio based on the currency of the asset. It allows ‘+’ or ‘-‘ followed by a number between 0 and 100. This amends the advance ratio for assets valued in the currency by the number of percentage points, either increasing (+) or decreasing (-), depending on the sign of the number. This is an optional field. |
| Adj Margin Rate | Allows the modification of the advance ratio based on the currency of the asset. It allows ‘+’ or ‘-‘ followed by a number between 0 and 100. This amends the advance ratio for assets valued in the currency by the number of percentage points, either increasing (+) or decreasing (-), depending on the sign of the number. This is an optional field. |
| Product | This field is associated with Prd Margin Rate and Prd Adj Margin Rate fields. These fields allow exceptional advance ratio and lower advance ratio rates to be defined for specific products linked to the country. This is an optional multi-value field. |
| Prd Margin Rate | Allows modification of the advance ratio based on the currency of the asset for the associated product. It allows ‘+’ or ‘-‘ followed by a number between 0 and 100. This amends the advance ratio for assets in this product valued in the currency by the number of percentage points, either increasing (+) or decreasing (-), depending on the sign of the number. This is a multi-value field. |
| Prd Adj Margin Rate | Allows modification of the lower advance ratio based on the currency of the asset for the associated product. It allows ‘+’ or ‘-‘ followed by a number between 0 and 100. This amends the lower advance ratio for assets in this product valued in the currency by the number of percentage points, either increasing (+) or decreasing (-), depending on the sign of the number. This is an optional multi-value field. |
| Concentration Cap | Defines the concentration cap for the currency. |


##### Country –CO.COUNTRY

This application holds the concentration cap rules defined for the collateral country.

> **⚠️ Note:** The ID must be a valid record in COUNTRY application. It indicates the collateral country for which the concentration cap is defined.

| Field | Description |
|---|---|
| Concentration Cap | Contains the concentration cap to be applied to assets associated with this risk country. Input must be a number from 0 to 100. This is an optional field. |
| Emerging Market | Indicates if the country is considered as an emerging market. If set to Yes, the country is defined as an emerging market. |


##### Country Group –CO.COUNTRY.GROUP

The countries that are configured as emerging markets in CO.COUNTRY application are automatically grouped under the Emerging Market Group in the CO.COUNTRY.GROUP application. This enables the user to define specific concentration cap that is applicable on the group of countries that form the emerging market. Currently, the grouping of county is enabled only for emerging markets.

> **⚠️ Note:** The application ID is EMERGING.MARKET and this is created by the system when the Emerging Market field in CO.COUNTRY is set for any specific countries.

| Field | Description |
|---|---|
| Description | Contains the description for the country group. This is an optional field. |
| Concentration Cap | Indicates the concentration cap that is applied to assets linked to countries in the group. Input must be a number from 0 to 100. |
| Country | Multi-valued field defaulted from CO.COUNTRY and contains the list of countries linked to the country group. |


##### Industry –CO.INDUSTRY

This application is used to setup concentration cap at industry level for security assets.

> **⚠️ Note:** The application ID must be a valid record in SC.INDUSTRY application.

| Field | Description |
|---|---|
| Concentration Cap | Indicates the concentration cap to be considered for the sub asset type. |


#### 📋 Tasks

There are no Tasks available for Group Concentration Cap feature.


#### 📊 Outputs

The user can view the below enquiries and reports pertaining to Create Collateral Item in the core banking system.


##### Enquiries and Reports

This section allows the user to view the below enquiries and reports:

View Excess Concentration Cap Details

The concentration cap is applied to mitigate the risk associated with the collateral by capping collateral value. This enquiry displays collateral values, which are exceeded the concentration cap.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA


> **Related Applications:** `CO.COUNTRY`, `CO.COUNTRY.GROUP`, `CO.CURRENCY`, `CO.INDUSTRY`, `CO.VALUATION.PARAMETER`, `COUNTRY`, `CURRENCY`, `SC.INDUSTRY`

---


### 1.12  Limit Collateral Allocation


> **📇 Quick Reference Card**
> 
> **Purpose:** *The order in which collaterals need to be sorted to cover the liabilities of a customer can be achieved by following anyone of the below setups:*
> 
> **Sections:** 📖 Introduction | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The order in which collaterals need to be sorted to cover the liabilities of a customer can be achieved by following anyone of the below setups:

- Default collateral allocation process.
- Collateral allocation priority by parameter setup.
- Collateral allocation priority by manual setup.

In the absence of any specific setup, either parameter or manual, system follows the default process of allocating collaterals to the liabilities of the customer.


#### 📋 Tasks

There are no Tasks available for Limit Collateral Allocation Process feature.


#### 📊 Outputs

There are no Outputs available for Limit Collateral Allocation Process feature.

---


### 1.13  Loan to Value calculation


> **📇 Quick Reference Card**
> 
> **Purpose:** *LTV is a lending risk assessment ratio often used by financial institutions and lenders prior to approving a mortgage. High LTV ratios are generally deemed to be higher risk; making the cost of borrowing more for the borrower.*
> 
> **Applications:** `COLLATERAL`, `LIMIT`, `LIMIT.REFERENCE`
> 
> **Key Fields:** *Authorised*, *Balance*, *Execution*, *Execution Value*, *Highest*, *LTV denominator*, *Limit*, *Loan* ... +14 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

LTV is a lending risk assessment ratio often used by financial institutions and lenders prior to approving a mortgage. High LTV ratios are generally deemed to be higher risk; making the cost of borrowing more for the borrower.

LTV is the ratio of loan to collateral value. The loan value and the collateral value are considered for calculating this ratio and this is configurable in Temenos Transact .

The following events trigger the LTV calculation:

- Revaluation of collateral
- Recalculation of the market value of the collateral
- Changes to the loan balance, which could be a repayment, a drawdown or interest calculation
- Changes to purchase price of collateral
- Changes to the authorised limit amount


#### ⚙️ Configuration

This topic covers the parameter setup for configuring LTV calculation.


##### LIMIT.REFERENCE

The following fields in this application are used in configuring the parameters for LTV calculation:

- Ltv Numerator – Details the rules to define which numerator is used in the LTV calculation.
- Ltv Denominator – Details the rules to define which denominator is used in the LTV calculation.
- Ltv Local Denominator – Contains the name of the local reference field on collateral that contains the value used in the denominator.
- Ltv Lowest Fields – A multi-valued field, which contains a list of fields that are compared to see which is the lowest when calculating the LTV denominator .
- Ltv Highest Fields – A multi-valued field, which contains a list of fields that are compared to see which is the highest when calculating the LTV denominator .

The Ltv Numerator and Ltv Denominator fields are optional. However, if one field is populated, then the other becomes mandatory (as both fields are required for LTV calculation).

The allowed values for the Ltv Numerator field are:

- Loan Balance – If the numerator is loan balance, then the value for the numerator is taken from the outstanding loan balance of the loans linked to the limit.
- Authorised Limit – If the numerator is authorised limit, then the value for the numerator is taken from the Maximum Total field of the record in LIMIT .

The allowed values for the Ltv Denominator field are:

- Purchase Price – The purchase price is recorded against the underlying asset (for example, the purchase price of the property on which the loan was taken).
- Execution Value – If the denominator is Execution Value, then the denominator is taken from the Execution Value field in the record of COLLATERAL allocated to the limit. This is the Collateral Value option.
- Nominal Value – If the denominator is Nominal Value, then the denominator is taken from the Nominal Value field in the record of COLLATERAL allocated to the limit. This is equivalent to using the pledged collateral value and is the Market Value option.
- Highest – If the denominator is Highest, then the denominator used is the highest from the fields identified in the field Ltv Highest Fields .
- Lowest – If the denominator is Lowest, then the denominator used is the lowest from the fields identified in the field Ltv Lowest Fields .
- Local – If the denominator is Local, then the value of the local field identified in the Ltv Local Denominator field is used as the denominator. If the economic value is added as a local field in the record of COLLATERAL , this option is used to choose the economic value as the denominator.


##### COLLATERAL

The Purchase Price field is used to define and store the purchase price of the collateral, which is used to calculate the loan to value ratio, if it is defined in the Ltv Local Denominator field in the LIMIT.REFERENCE application.


#### 📋 Tasks

There are no Tasks available for Loan To Value Calculation feature.


#### 📊 Outputs

There are no Outputs available for LTV Calculation feature.


> **Related Applications:** `COLLATERAL`, `LIMIT`, `LIMIT.REFERENCE`

---


### 1.14  Margin Valuation through Credit Policy Structure


> **📇 Quick Reference Card**
> 
> **Purpose:** *Portfolios, accounts and deposits are some of the assets that can be pledged against to get a loan. However, these assets carry a certain amount of risk. The risk associated is based on various market factors like category, country, currency, fixed tenor, remaining tenor, issuer, market, sector, ind...*
> 
> **Key Fields:** *Addl Criteria Field*, *Apply Credit Policy*, *Asset Ccy*, *Avg Daily Trd Vol*, *Cap Type*, *Cap Value*, *Cap Value Ccy*, *Category* ... +24 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Portfolios, accounts and deposits are some of the assets that can be pledged against to get a loan. However, these assets carry a certain amount of risk. The risk associated is based on various market factors like category, country, currency, fixed tenor, remaining tenor, issuer, market, sector, index, bond type, credit ratings, fund type, fund size and issue size.

- Users can define a special condition for attributes to calculate the margin rate (HAR) and adjusted margin rate (LAR). This is calculated on various asset classes linked to collaterals. The attributes or criteria can be used individually or in combination to arrive at a margin rate.
- Users can apply additional caps, such as price cap, quantity caps and volume caps, which are the first-level threshold to be applied on the asset class, sub asset class or security instrument, to identify the applicable LTV rate. In the advance collateral processing, if the currency of the liability is different from that of the collateral asset, the system looks for the cross-currency matrix. If defined, the cross-currency pair haircut is applied on the remaining collateral to arrive at the final collateral value.


#### ⚙️ Configuration

Configure the Apply Credit Policy field in the CO.VALUATION.PARAMETER application to enable the credit policy system. This configuration is applicable system-wide and hence can be entered only in the SYSTEM record of the CO.VALUATION.PARAMETER application. The Apply Credit Policy field cannot be manually entered in the company-specific record in this application.

The allowed values are:

- Yes – If set as Yes, the margin rates are determined based on the credit policy structure for the supported applications.
- No – If set as No, the margin rates are determined based on the default hierarchy.

The following screenshot shows the SYSTEM record in the CO.VALUATION.PARAMETER application, where the Apply Credit Policy field is enabled.


#### 🔧 Working With

This section provides details about how the LTV rates are identified in a credit policy structure and the advance collateral processing is performed considering the concentration pool and cross-currency haircut percentage, if defined, in the credit policy structure.


##### Defining Margin Rules

The margin rate or lending ratio, also known as LTV, is a percentage that is applied on any asset to arrive at a margin value. This value is the maximum amount that can be borrowed against that asset. The asset can be a portfolio, deposit, a guarantee or a money market instrument.

The MV.MARGIN.RULES application allows users to assign margin rates on asset classes based on a certain condition and stores the details of the criteria along with its value, associated margin rates and adjusted margin rates in Temenos Transact.

- The ID of this application is ! , for example, A-40!STANDARD.
- Asset code can be Asset Type, Sub Asset Type, Security Number, Account or Contract Id, and ALL. The ID can be in any of the following format:

- Company-specific rules for the Asset Type and Sub-asset Type can be configured in the following format: ! , for example, A-1*US0010001!Standard ! , for example, S-100*US0010001!Standard

> **⚠️ Note:** If margin rates are defined at asset type, sub asset type and contract, account or instrument level, then the rates defined at the contract, account or instrument level take precedence over the asset type and sub asset type. If rates are defined at sub asset type and asset type level, then the rates at the sub asset type take precedence over the asset type.

Some of the critical fields and its implications are described in the following table:

| Fields | Description |
|---|---|
| Criteria | The user can define any meaningful name for the criteria that is to be used in the LTV evaluation. |
| Criteria Type | Holds the attributes that define the margin rates. The attributes are Amount, Category, Country, Currency, Fixed.Tenor, Remaining.Tenor, Price, Date and Any. |
| Operation | Defines the operand for the given criteria (for example, equal or greater than) |
| Value | Holds the value of the Criteria field. In this example, when the amount is defined in the Criteria field, users must define the value, that is, 50,000. |
| Value Ccy | When the Criteria Type is Amount or Price, the associated currency should be defined in Value Ccy . |
| Joints | AND/OR are joints used to define the link between multiple attributes based on which the margin rate is defined. |

The following table shows the description and operands supported for each criterion.

| Criteria Type | Description | Supporting Operands |
|---|---|---|
| Amount | All the attributes indicated in terms of amount like balance and fund size are part of this criterion. | ALL [EQ, LT, LE, GT, GE, Range (Rg), NE] |
| Category | All the attributes pertaining to the category of the asset class, sub asset class, contract or security instrument. | ALL |
| Country | Any attribute related to the country of the asset class, sub asset class, contract and security instrument is part of this criterion. | EQ, NE |
| Currency | All the attributes related to the currency of the asset class, sub asset class, contract or security instrument are part of this criterion. | EQ, NE |
| Fixed.Tenor | Those attributes that indicate the time of the asset class, sub asset class or contract are part of this criterion. | ALL except Rg |
| Remaining.Tenor | Those attributes that indicate the remaining period left for the asset class, sub asset class or contract are part of this criterion. | ALL except Rg |
| Price | Those attributes related to the price of the security instrument (for example, price of a share) are part of this criterion. | ALL |
| Date | Those attributes related to the date of the asset class, sub asset class, contract or security instrument are part of this criterion. | ALL |
| Any | Those criteria that do not require any specific validation fit into the ‘Generic’ criteria type. For example, attributes like Index (S&P Global 100) or the Security Market (New York Stock Exchange) can use the ‘Generic’ criteria type. | All operands are applicable for numeric values. Only EQ and NE applicable for non-numeric values. |

For example, the following rule is defined for the asset class – Cash accounts:

If the currency is USD and category is 6001 (savings account) or accounts with balance greater than USD 50,000, the applicable margin rate is 95%.

The system evaluates the rule in the order in which it is defined. Hence, it first evaluates the AND joint and then the OR joint to apply the given margin rate as shown in the following screenshot.

The following associated fields are used to define the application that fetches the data for the defined criteria:

| Fields | Description |
|---|---|
| Criteria Name | Validates those criteria defined above (amount, category and currency in the above example) in the suitable application. |
| Criteria Appln | The system refers the ACCOUNT application to validate the criteria defined for the above example. |
| Criteria Field | Field name from where the data is taken for the associated criteria application, for example, when the criteria is defined as ‘Category’, the Category field in the ACCOUNT application is referred to fetch the data. |
| Addl Criteria Field | In certain cases, additional criteria values for processing are required. This is mandatory when the Criteria Type is set to FIXED.TENOR, AMOUNT or PRICE. Not allowed for other criteria types. If Criteria Type is set to Fixed.Tenor, the user has to configure the start and end date. The Start date field can be configured in the Criteria Field and the End date field can be configured in the Addl Criteria Field. Similarly, the User can configure the associated currency for the Criteria Type ‘Amount’ and ‘Price’, in this field. |

The default rates for the asset, that is, default margin rate, default adjusted margin rate, default preferential margin rate, default loss margin rate, default top up margin rate, default sell out margin rate and default concentration cap can also be defined and applied if the criteria-based margin rates do not apply to the given asset class.


##### Defining Credit Policy

The credit policy structure comprises of one or more rules based on which the LTV rate of the collateral asset is determined. The MV.CREDIT.POLICY application is used to define the credit policy structure. The LTV rules defined in MV.MARGIN.RULES are attached in this application. The ID of MV.CREDIT.POLICY is a meaningful text.

In the credit policy, the margin rules are attached in the Ltv Rules field, that is, it holds only the valid record from MV.MARGIN.RULES .

The default margin rates are defined in the credit policy. These rates are considered for those assets for which a rule-based LTV rate is not available. Apart from the default margin rates, the user can also define concentration cap at the credit policy level.


##### Determining LTV in a Credit Policy Structure

The rules or conditions defined in MV.MARGIN.RULES on various asset classes (asset type, sub-asset type, contract no and security no) are validated against the respective applications such as AC, LD, MD, MM and FD.

- If the first condition does not match and the AND/OR joints are also not provided for the next condition, then the system validates the next condition for matching. If the conditions are satisfied, the corresponding margin rate and adjusted rates are applied.
- If none of the defined conditions match, then the default margin rates and default adjusted margin rates for the rule (if defined) are applied.
- If the default margin rate and default adjusted margin rate are not defined in MV.MARGIN.RULES , the default rates defined in MV.CREDIT.POLICY are applied.

The flowchart for evaluating the margin rate based on the definition in MV.MARGIN.RULES and MV.CREDIT.POLICY is as follows:

An account with the following information is provided as the collateral asset:

- Account ID: 12345
- Category: 5001
- Currency: USD
- Working Balance: 10,000

The following rules are configured for the cash account:

| Criteria | Criteria Type | Operand | Value |
|---|---|---|---|
| Categ | Category | Eq | 6001 |
| Margin rate | 90% |  |  |
| Adjusted margin rate | 85% |  |  |
| CCY | Currency | Eq | GBP, EUR, USD |
| Margin rate | 80% |  |  |
| Adjusted margin rate | 75% |  |  |

The LTV rate is evaluated considering the sequence in which the criteria are defined. In this example, the Categ criteria is evaluated first. As the category of the account is 5001, it does not satisfy the first criteria. Hence, the evaluation process checks the next condition, that is, currency = GBP, USD or EUR. Since the second condition satisfies the criteria with the account currency being USD, the applicable margin rate is 80% and adjusted margin rate is 75% for the account 12345.

> **⚠️ Note:** The collateral values are recalculated during close of business (COB) or amendment of a collateral, if a user decides to change the structure from a non-credit policy to a credit policy framework.


##### Applying Exposure Caps in a Credit Policy Structure

A portfolio consists of multiple assets that can be volatile due to market fluctuations. To minimise the risk, certain additional level of caps are applied on these assets. The following caps can be set on a given asset:

- Price cap – The market price of the asset can be capped so that if the market price of the asset breaches the capped price, the system uses the capped price to calculate the margin value.
- Quantity cap – The system can cap the quantity or nominals of shares at certain quantity. The system uses the capped quantity to calculate the collateral value.

These caps are applied at the asset class, sub-asset class or security instrument level and are the first level of cap applied on the asset class. The concentration cap, if defined, is the second level of cap applied on the asset to derive the collateral value.

The following fields in MV.MARGIN.RULES application support the definition of price and volume cap.

- Cap Type – Holds different types of caps that are applied on the price or the quantity of the asset class, sub asset class or security instrument.

- Price cap – The share price is capped at 1,000 GBP and market price is at 1,500 GBP, with 100 shares. The estimated market value after price cap is calculated using the capped price: 100 * 1000 * 80% = 80,000 GBP, as shown in the following table:

| Cap | Currency | Nominal | Price | Market Value | Margin Rate | Price Cap | Estimated Market Value after Price Cap |
|---|---|---|---|---|---|---|---|
| Price Cap | USD | 100 | 1,500 | 150,000 | 80% | 1,000 | 80,000 |

- Quantity cap – The quantity of a share is capped at 80 units on overall quantity of 100 units. Then, the estimated market value is calculated using the capped quantity: 80 * 1,500 * 80% = 96,000 GBP, as shown in the following table:

| Cap | Currency | Nominal | Price | Market Value | Margin Rate | Quantity Cap | Collateral Value |
|---|---|---|---|---|---|---|---|
| Quantity Cap | USD | 100 | 1,500 | 150,000 | 80% | 80 | 96,000 |

- Cap Value – Holds the value to be assigned to the respective cap chosen in the Cap Type field. This field is associated with the Cap Type multi-value set.
- Cap Value Ccy – Holds the currency of the amount defined in the Cap Value field. This field is mandatory when the Cap Type is Price Cap. This field is associated with the Cap Type multi-value field set.

Volume and Minimal Price: The volume cap rule (ADTV) and the minimal price caps can also be configured as criteria in the margin rule application.

- Volume Cap – Average daily trading volume (ADTV) is a parameter that measures the average number of shares traded within a day in each stock. Capping is done on ADTV and if the value of ADTV falls below the capped value, the collateral value is zero. The Avg Daily Trd Vol field in SECURITY.MASTER can be mapped for the criteria ANY for validation.
- Minimal Price – A minimum price can be set on the asset so that if the price of the asset falls below the price, the collateral value is zero.


##### Applying Concentration Pool in a Credit Policy Structure

Concentration pool is a pool of instruments from the customer’s portfolio that are eligible for concentration cap. Concentration pool can be created by defining asset types that must be either excluded or included to calculate the concentration cap.

Some banks may want to exclude or include certain types of assets from calculating the concentration cap. The asset value of the excluded asset should not be considred for the concentration cap calculation. Also, the concentration cap is not applied on these excluded assets.

The following fields in the CO.VALUATION.PARAMETER application support this functionality:

- Exclude Conc Cap Pool
- Include Conc Cap Pool

Both the fields are multivalued fields to allow the user to enter asset types or sub-asset types whenever required. These options are mutually exclusive, meaning that one or more asset types or sub-asset types can be either included or excluded, but not both.

The valid record ID of ASSET.TYPE or SUB.ASSET.TYPE is prefixed with A or S, respectively. For example, if the bank wants to exclude Cash deposits (for example, Asset Type -1) and Preference share (for example, Sub Asset Type- 6), it can be configured as follows:

- Exclude Asset Type 1: A – 1
- Exclude Sub Asset Type 2: S – 6

Similarly, if the bank wants to include Cash deposits (Asset Type 1) and Preference share (Sub asset type 6), it can be configured as follows:

- Include Asset Type 1: A – 1
- Include Sub Asset Type 2: S – 6

| SC CUSTOMER MARGIN | 190355 |  |
|---|---|---|
| COLLATERAL | CO21106YYTW0 | CO21106YYTW0 |
| ASSETS | 190355-1.300.30*830187-001 (Shares) | 117129 (Cash account) |
| ASSET TYPE | 30 | 1 |
| SUB ASSET TYPE | 300 | 1 |
| MARGIN RATE/ADJ MARGIN RATE | 90/80 | 90/80 |

| SC CUSTOMER MARGIN | 190355 |  |
|---|---|---|
| COLLATERAL | CO21106YYTW0 | CO21106YYTW0 |
| ASSETS | 190355-1.300.30*830187-001 (Shares) | 117129 (Cash account) |
| ASSET TYPE | 30 | 1 |
| SUB ASSET TYPE | 300 | 1 |
| MARGIN RATE/ADJ MARGIN RATE | 90/80 | 90/80 |


##### Currency Pair Haircut in a Credit Policy Structure

At times, collaterals that are pledged against a liability are denoted in a different currency. In such cases, cross-currency rates are applied on the collateral to arrive at the final value.

- In the process of advance ratio calculations, the system allocates collateral against the liabilities of the same currency after a single concentration cap is applied.
- After matching the same currency liability and collateral, the system converts the unallocated collateral amount to LAR (using the adjusted margin rate value) before allocating the collateral to other currencies' liabilities.
- Temenos Transact supports the ability to define the cross-currency haircut for a pair of currency (where the asset currency is different from the liability currency) and discounts the remaining collateral by cross-currency pair haircut rate.The MV.CREDIT.POLICY application supports the definition of cross-currency haircut matrix. The haircut percent is applied on the remaining collateral after matching the liability. The fields that support the matrix are as follows:

| Fields | Description |
|---|---|
| Ccy Pair Perc | Denotes the haircut that is applicable when a collateral asset and liability are in two different currencies. The value defined can be an absolute percentage value. For example, the cross-currency haircut can be defined as 10%. During the currency matching process, the adjusted margin rate is derived by deducting the respective cross-currency pair percentage from the applicable margin rate. |
| Asset Ccy | Denotes the currency of the asset and is associated with the Ccy Pair Perc field. |
| Liab Ccy | Denotes the currency of the liability and is associated with the Ccy Pair Perc field. |

For example, the asset and liability of the customer is as follows:

| Asset | Currency | Value | Liability | Currency | Value |
|---|---|---|---|---|---|
| Cash | USD | 40,000 | Loan 1 | CAD | 40,000 |

The following currency pair percent can be defined in MV.CREDIT.POLICY :

The cross-currency pair percentage defined for the currency pair USD/CAD is 10%. Hence, the adjusted margin rate considering the currency pair haircut for USD/CAD is derived as - . If the applicable HAR is 90%, the adjusted margin rate for the currency pair USD/CAD is 90 – 10 = 80% .

If the haircut percentage is not defined in the matrix, the default adjusted margin rate defined in the credit policy is considered. If there is no rate defined in the credit policy, the system evaluates the margin rules to identify the applicable adjusted margin rate.

The following example shows the complete calculation of collateral valuation when the currency pair haircut is defined.

A customer has the following collateral and rates set up in MV.CREDIT.POLICY :

| SC CUSTOMER MARGIN | 190368 |
|---|---|
| COLLATERAL | CO211061D9D6 |
| ASSETS | 117258 |
| MARGIN RATE | 90 |
| ADJ MARGIN RATE | 70 |
| CCY HAIR CUT LAR 1 | 10% |

| CCY | Liability | Exchange rate | Final Value (in USD) |
|---|---|---|---|
| CAD | 20000 | 1.265633 | 15802.37 |
| OTHER CCY LIAB |  |  | 15802.37 |

| Asset | Asset Ccy | Market Value |
|---|---|---|
| AS1 | USD | 40000 |

The calculation is explained below:

| Asset | Asset Ccy | Market Value | HAR/Margin Rate | Margin Value | Exch Rate | Margin Value (Lcy) |  | Single Cap Value | Margin Value after Single Cap | Same Currency Liab Alloc | Remaining Collateral (MV After Same CCY) | LAR | MV after Cross Ccy Pair Haircut | Other Ccy Liab at LAR | Unallocated Collateral at LAR | Execution Value of Collateral Tot Col After |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|  |  |  |  |  |  |  | Single Cap |  |  | 0 |  |  |  | 15802.37 |  |  |
| AS1 | USD | 40000 | 90% | 36000 | 1 | 36000 | 0% | 36000.00 | 36000.000 | 0.00 | 36000.00 | 80% | 32000.00 | 15802.37 | 16197.63 | 32000.00 |

The other liability currency is USD 15802.37 (that is, CAD 20,000 converted to asset currency USD). When a currency pair haircut is defined in MV.CREDIT.POLICY , the adjusted margin rate is calculated as Margin Rate - Ccy Pair Haircut) / Margin Rate.

Thus, the value in the MV after Cross Ccy Pair Haircut column in this example is calculated as, the MV Aft Same Ccy Alloc * (HAR - Ccy Pair Haircut) / HAR, that is, 36,000*(90%-10%)/90 = 32,000. The CAD liability converted to the asset currency USD 15802.87 is allocated from 32,000.


#### 📋 Tasks

There are no Tasks available for the Margin Valuation through Credit Policy Structure feature.


#### 📊 Outputs

There are no Outputs available for the Margin Valuation through Credit Policy Structure feature.

---


### 1.15  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *Collateral is the asset pledged by the customer as security for a financial facility provided by the financial institution.*
> 
> **Applications:** `CODE`, `COLLATERAL`, `COLLATERAL.CODE`, `COLLATERAL.RIGHT`, `COLLATERAL.TYPE`, `CUSTOMER.COLLATERAL.TYPE`, `TYPE`
> 
> **Key Fields:** *Application*, *Application Input*, *Cash Collateral*, *Central Bank Value*, *Collateral Right*, *Collateral Right Id*, *Execution Value*, *General Ledger Value* ... +8 more
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- API
- Temenos Transact Services

Collateral is the asset pledged by the customer as security for a financial facility provided by the financial institution.

- Ship
- House
- Painting
- Sculpture
- Single stamp (or an entire collection)
- Customer deposit
- Portfolio

These collateral items are revalued against the prevailing market value on a regular or ad hoc basis. A right or link to collateral items are established to cover the liabilities of the customer.

Collateral items maintained in Temenos Transact can be valued automatically.

- Deposit account
- Fixed term deposit
- All or part of customer portfolio stocks and shares


##### Product Configuration

The following table lists the module and product information for the Collateral functionality in Temenos Transact :

| Module/Product | Usage |
|---|---|
| CO | The Collateral (CO) product needs to be installed to use the basic Collateral functionality in Temenos Transact . |
| MV | The Margin Valuation (MV) product needs to be installed to configure and use the CO.VALUATION.PARAMETER application in the Advance Collateral processing. The CO product or SC product is a pre-requisite for installing the MV module. |
| CX | The Advance Collateral (CX) product needs to be installed to use the advance collateral features and derive the collateral value considering the concentration cap and currency hair-cut, as applicable to the collateral asset. The CO product and MV product are pre-requisites for installing the CX module. |
| COPOOL | The Collateral Pool (COPOOL) module enables the Corporate Collateral Pool functionality. The CO product is a pre-requisite for installing the COPOOL module. |

Configure the following parameters to use the Collateral module in Temenos Transact :

This is a company level application, which sets out high-level parameters that control the Collateral module. The parameters include:

- Maintaining the number of changes to collateral revaluation in the COLLATERAL application
- Considering account balance when deposit account is given as collateral
- Online update of cash collaterals (if required)
- Online collateral valuation (if required)
- Defining the currency and forex risk margin to cover the currency conversion risk factor
- Contract sequence routine defined in EB.API can be attached in the Contract Seq Rtn field.

The contract sequence routine instructs the system to apply a different collateral allocation order for the contracts returned, compared to the standard pro-rata allocation.

In this example, a contract sequence routine has been set up in COLLATERAL.PARAMETER , which returns the contracts in the order in which the transactions take place. The collateral amount is not allocated based on pro-rata allocation; instead, it is allocated based on the execution value for each Limit. This means that when more than one Limit is linked to the same Collateral Right , the amount assigned to each Limit is used by contracts. One Limit is not borrowed from another Limit’s assigned collateral amount. The following Limit structure has been created:

- Validation Limit LI0000101030 with Internal Amount = 50,000.
- Utilisation Limit LI0000101031 with Internal Amount = 30,000, but with an Online Limit = 22,500 based on the Execution Value of the collateral linked to the Limit.
- Utilisation Limit LI0000101032 with Internal Amount = 20,000, and an Online Limit equal to the Internal Amount ; both this and the previous Limit are linked to the same Collateral Right .
- Collateral Right COR09362S124H showing the two Utilisation Limits linked to it and the collateral to which they pertain.
- Collateral CO09362G674G showing the total Execution Value of the two Utilisation Limits and the Collateral Right Id to which they are linked:
- Collateral Allocation showing the allocated amount (that is, Execution Value ) for each of the Utilisation Limits:
- The two records in the LIMIT.TXNS application showing the contracts that utilised each Limit:

By disbursing the above contracts and running LI.CONTRACT.ALLOCATION.SERVICE, ECB displays the following details for each contract:

- Contract 10017194202 is disbursed for 6,000 by utilising Limit LI0000101031; given that Online Limit = 22,500, the system allocates the full amount for the transaction:
- Contract 10017194203 is disbursed for 15,000 by utilising Limit LI0000101031; given that Online Limit = 16,500, the system allocates the full amount for the transaction:
- Contract 10017194204 is disbursed for 25,000 by utilising Limit LI0000101032; given that Online Limit = 20,000, the system could have allocated a total of 21,500 for the transaction since there are still 1,500 not utilised for Limit LI0000101031; however, because of the contract sequence routine that has been initiated, the system allocates only the 20,000 assigned for this Limit:

| ID | Type | Description |
|---|---|---|
| 100 | CASH | All types of Cash, Accounts, Money Market (MM), Loans & Deposits (LD) and Deposit Contracts |
| 200 | HOUSE | All forms of property; from domestic to industrial properties |
| 300 | ART | Includes paintings, sculpture, jewellery and so on |
| 400 | SHARES | Value of a customer's shares |

This application is used whenever the Execution Value field (if defined as a percentage of Nominal Value field in the COLLATERAL.TYPE application) is different for specific customers. To input a record in this application, the Execution Value field in the main COLLATERAL.TYPE application must be defined in the %N format. The record ID format of this application is - .

COLLATERAL.TYPE ID– 600

If the Nominal Value is F, the Execution Value is 100%N and when a real estate worth USD 100,000 is attached to a collateral belonging to this type, then the Nominal Value field defaults to USD 100,000 and the Execution Value field is also USD 100,000 (that is 100%N).

For customer 190201, if the Execution Value is desired as 65%N, then a record with ID 190201-600 is created in the CUSTOMER.COLLATERAL.TYPE application and the Execution Value is defined as 65%N.

For the same collateral defined above, the Execution Value for the customer 190201 is calculated as USD 65,000 (that is, 65% of the Nominal Value ).

| COLLATERAL . TYPE | Description | COLLATERAL . CODE | Description |
|---|---|---|---|
| 100 | Cash | 101 | MM Deposits |
| 102 | LD Deposits |  |  |
| 103 | Savings Accounts |  |  |
| 200 | Houses | 201 | Business Property |
| 202 | Domestic Property |  |  |


##### Illustrating Model Parameters

This section covers the high-level parameterisation setup that defines and controls the collateralised limits.

| S.No. | Parameters | Description |
|---|---|---|
| 1. | COLLATERAL.PARAMETER | This application allows the user to define the company-level system parameter. User can define if address is to be defaulted from CUSTOMER application. To cover the currency conversion risk factor, margin for the collateral currency is also defined when limit currency is different from collateral currency. To retain collateral records in live table, retention period value must be defined in the collateral parameter setup. Specification to determine which balance from EB.CONTRACT.BALANCES table to be considered for updating in collateral record. |
| 2. | COLLATERAL.TYPE | This application allows the user to define different types of collaterals like building stocks and guarantees and so on. Information in this table enables the client to arrive at collateral value, revaluation of collateral value and linking to other applications in Temenos Transact . Market value or face value of the collateral, value for general ledger purpose, third party value (value of collateral item outside Temenos Transact ) are specified in this table. |
| 3. | COLLATERAL.CODE | This application allows the user to determine how collateral values are re-allocated across central bank reporting lines. Enables the system to perform recalculation of percentage of collateral cover applicable. Enables the system to mention the default review frequency. Enables the system to mention the default review frequency. Enables to update Allocated Balance type, Utilized balance type and Unutilized balance type. |
| 4. | COLLATERAL.EXCLUSION | This application allows the user to define the criteria for the exclusion of collaterals. CURRENCY, COUNTRY, SECURITY.CODE, INDUSTRY, ISSUER and COUNTERPARTY values are used to define the criteria. |
| 5. | CO.CURRENCY | This application allows the user to define the rules to modify the lower advance ratio of the assets valued in a currency. Enables the user to define the currency level concentration cap. Enables the user to define the specific margin rates at product level. |
| 6. | CO.VALUATION.PARAMETER | This application allows the user to define the margin calculation, asset allocation, asset valuation for the collateral process. Enables the user to specify if the collateral is allocated against limits or liabilities. Enables the user to mention the discretionary portfolios. |
| 7. | CUSTOMER.COLLATERAL.TYPE | This application allows the user to define specific collateral execution value for specific customers. |
| 8. | CO.ELIGIBILITY | This application allows the user to define the eligibility rules for collateral against the limit products to which the collateral is linked. |
| 9. | CO.INDUSTRY | This application allows the user to define the concentration cap at industry levels for security assets. |
| 10. | CO.RANKING | This application allows the user to define the ranking rules for the collaterals against limit products. |
| 11. | CO.COUNTRY | This application allows the user to define the concentration cap rules for the collateral country. |
| 12. | CO.COUNTRY.GROUP | This application allows the user to define the concentration cap rules for a group of countries. |


> **Related Applications:** `CODE`, `COLLATERAL`, `COLLATERAL.CODE`, `COLLATERAL.RIGHT`, `COLLATERAL.TYPE`, `CUSTOMER.COLLATERAL.TYPE`, `TYPE`

---


### 1.16  OffBalanceSheetAccountingforCollaterals


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Collateral attached to any credit facility minimises the risk to the maximum extent. But the booking of this mitigation process is an off balance sheet process. To achieve this, the Temenos Transact system allows the booking of collateral accounting entries and reports it in the system.*
> 
> **Key Fields:** *Coll Booking Frequency*, *Collateral Code*, *Collateral Right Id*, *Collateral Right Ids*, *Consol key*, *Reporting Type*, *Transaction Code*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The Collateral attached to any credit facility minimises the risk to the maximum extent. But the booking of this mitigation process is an off balance sheet process. To achieve this, the Temenos Transact system allows the booking of collateral accounting entries and reports it in the system.

The GL accounting for Collaterals is raised based on the Limit exposures that are being covered by the collaterals linked through the Right of the Customer. The accounting is raised for collateral amount that is allocated, utilised and unutilised for the corresponding Limit exposure.


#### ⚙️ Configuration

The following setup is done to record accounting entries for Collateral:

- Accounting Treatment and Booking Frequency
- Configuring Balance Types
- Collateral Code for GL Posting

The Collateral GL Accounting booking frequency and GL Treatment are configured in the LIMIT.PARAMETER application. Configuring the fields are pre-requisites for Collateral GL Accounting.

The GL treatment for collateral provides in two options:

- In Out – The system fully reverses the previously created positions and performs new bookings for the full amount.
- Adjustment – The system compares the current position with the previously booked and posts the adjustment for the difference.

The posting of the accounting entry is performed by an automatically run online background service on a periodic basis. This service runs according to the Coll Booking Frequency set in LIMIT.PARAMETER . The LI.COLLATERAL.ACCOUNTING service is run to perform calculations and postings of collateral utilisation by underlying limits and assets underneath those Limits.

This service is run on-line on a periodic basis and calculates Allocated, Unutilised and Utilised portions of the collateral value allocated to the limit. Calculated balances are posted against the Consolidation key created for the record in LIMIT where LIMIT Utilisation balances are currently booked ( EB.CONTRACT.BALANCES ).

The AC.BALANCE.TYPE application in Temenos Transact allows banks to configure balances that are used by the system. These balances are created as part of the system configuration to allow booking and reporting of collateral balances.

These balances are configured with Reporting Type as Contingent.

Off balance sheet postings are expected not for all types of collaterals. The bank needs accounting to only be raised for certain types of 'external' collaterals such as property, insurance, personal guarantee and securities portfolio received as collateral. Internal cash collaterals such as cash on account at the bank and term deposits at the bank do not require off balance sheet accounting.

The COLLATERAL.CODE application defines the following Balance Types to be used when posting collateral balances to a GL.

- Allocated portion
- Utilised portion
- Unutilised portion


#### 🔧 Working With

The method for booking of the collateral entries, that is, In Out or Adjustment, and the booking frequency, is selected from LIMIT.PARAMETER . The balance type ( AC.BALANCE.TYPE ) created for the booking and reporting of collateral balances are attached to the COLLATERAL.CODE of a specific collateral. The following collateral balances are considered when posting the collateral balances to GL.

- Allocated portion of the Execution Value
- Utilised portion
- Unutilised portion

The collateral values are allocated to the limit exposures using the standard Temenos Transact collateral allocation mechanism and the allocation details are stored in the LIMIT.COL.ALLOC.WORK table. Balances related to collateral allocation and utilisation are booked against the same limit consolidation keys, to which the limit utilisation is booked.

The collateral allocation details are recorded in the LIMIT.COL.ALLOC.WORK table, as shown below.

The calculated amount for the allocated, utilised and unutilised portion is posted against the Consol key of the respective LIMIT . This amount is updated in the corresponding Limit key in EB.CONTRACT.BALANCES (ECB).

The EB.CONTRACT.BALANCES (ECB) for the Limit is updated post COB. The Allocated, Utilised and unutilised collateral amount is updated in ECB for the LIMIT after the service LI.COLLATERAL.ACCOUNTING is run.

The screenshot of ECB shown below contains the details prior to running the service, LI.COLLATERAL.ACCOUNTING.

After running the service, the allocated, utilised and unutilised collateral amount is updated in EB.CONTRACT.BALANCES as shown in the screenshot below.

The following list of accounting entries are generated for Collateral Accounting based on allocation to the Limit in RE.CONSOL.SPEC.ENTRY .

The GL accounting treatment is the IN OUT method and the following Transaction Code is used in the accounting entries raised for collaterals

- CAL (Collateral Allocated)
- CUT (Collateral Utilised)
- CUN (Collateral Unutilised)

- If the booking method is Adjustment, the following is the entry in ECB: Revolving Limit is USD 100,000 Collateral Amount is USD 150,000 Loan Disbursed is USD 100,000

| Column 1 | Column 2 | Column 3 | Column 4 |
|---|---|---|---|
|  | Allocated (in USD) | Utilised (in USD) | Unutilised (in USD) |
| After the LI.COLLATERAL.ACCOUNTING Service is run |  |  |  |
| Collateral | 100,000 | 100,000 |  |
| After partial repayment of 60,000 |  |  |  |
| Collateral | 100,000 | 100,000 |  |
| Collateral | 100,000 | 40,000 | 60,000 |

For the repaid amount, new entries are raised in the RE.CONSOl.SPEC.ENTRY table. The existing LIMIT entries are untouched.

- If the user repays the loan amount for a revolving limit, the utilised and the unutilised amounts in the ECB change post repayment. The unutilised amount is increased by the repayment amount. For example: Revolving Limit is USD 100,000 Collateral Amount is USD 150,000 Loan Disbursed is USD 100,000

| Column 1 | Column 2 | Column 3 | Column 4 |
|---|---|---|---|
|  | Allocated (in USD) | Utilised (in USD) | Unutilised (in USD) |
| After the LI.COLLATERAL.ACCOUNTING Service is run |  |  |  |
| Collateral | 100,000 | 100,000 |  |
| After partial repayment of 60,000 |  |  |  |
| Collateral | 100,000 | 40,000 | 60,000 |

After the repayment of USD 60,000, the unutilised amount is increased by 60,000. Original Spec entries are reversed and new Spec entries are raised for new amounts after the repayment of the same limit amount. The following accounting entries are generated:

| Column 1 | Column 2 | Column 3 | Column 4 |
|---|---|---|---|
|  | Allocated(in USD) | Utilised(in USD) | Unutilised(in USD) |
| After the LI.COLLATERAL.ACCOUNTING Service is run |  |  |  |
| Collateral | 100,000 Cr | 100,000 Dr |  |
| After partial repayment of 60,000 |  |  |  |
| Collateral | 100,000 Dr | 100,000 Cr |  |
| Collateral | 100,000 Cr | 40,000 Dr | 60,000 Dr |

- If the user repays the loan in the case of a non- revolving limit, the utilised amount is reflected. For example: Revolving Limit is USD 100,000 Collateral Amount is USD 150,000 Loan Disbursed is USD 100,000

| Column 1 | Column 2 | Column 3 | Column 4 |
|---|---|---|---|
|  | Allocated (in USD) | Utilised (in USD) | Unutilised (in USD) |
| After the LI.COLLATERAL.ACCOUNTING Service is run |  |  |  |
| Collateral | 100,000 | 100,000 |  |
| After partial repayment of 60,000 |  |  |  |
| Collateral | 100,000 | 40,000 |  |

After the repayment of USD 60,000, the utilised amount is decreased by 60,000.

The following accounting entries are generated:

| Column 1 | Column 2 | Column 3 | Column 4 |
|---|---|---|---|
|  | Allocated(in USD) | Utilised(in USD) | Unutilised(in USD) |
| After the LI.COLLATERAL.ACCOUNTING Service is run |  |  |  |
| Collateral | 100,000 Cr | 100,000 Dr |  |
| After partial repayment of 60,000 |  |  |  |
| Collateral | 100,000 Dr | 100,000 Cr |  |
| Collateral | 40,000 Cr | 40,000 Dr |  |
| USD 60,000 is Unallocated. |  |  |  |

- If more than one collateral is attached to a single limit, the ECB is updated with all the collaterals that are linked.

| Column 1 | Column 2 | Column 3 |
|---|---|---|
| Limit A | Collateral Right 1 | Collateral 1 |
| Collateral Right 2 | Collateral 2 |  |

The Allocation of Collateral takes place on priority basis as mentioned in CO.ALLOCATION.PARAMETER .

The following screen shot shows an ECB for limit and the two Collateral Rights attached to a single limit with the allocated, utilised and unutilised balance.

In the above case, the collateral code is the same for both the Collateral Rights. If the collateral codes are different for multiple Collateral Rights, the ECB is updated in the same manner.

- In the case of multiple limits attached to a single collateral, separate ECBs are generated for the given limits. The collateral is allocated to these multiple limits based on the priority given in the CO.ALLOCATION.PARAMETER and COLLATERAL.RIGHT applications.
- The ECB is also affected when the value of either the limit or collateral or both is increased or decreased.

| Column 1 | Column 2 |
|---|---|
| Limit | USD 10,000 |
| Collateral Amount | USD 15,000 |
| Loan Disbursed | USD 8,000 |

| Column 1 | Column 2 |
|---|---|
| Limit | USD 10,000 |
| Collateral Amount | USD 15,000 |
| Loan Disbursed | USD 8,000 |


#### 📋 Tasks

There are no Tasks available for Off Balance Sheet Accounting for Collaterals feature.


#### 📊 Outputs

There are no Outputs available for Off Balance Sheet Accounting for Collaterals feature.

---


### 1.17  Other Internal Collateral Assets


> **📇 Quick Reference Card**
> 
> **Purpose:** *Temenos Transact supports assets like immovable property and mortgage. Based on the setup defined in the COLLATERAL.TYPE application, the system captures all the details with respect to these assets. These assets can also be used by other modules in Temenos Transact such as Collateral.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Temenos Transact supports assets like immovable property and mortgage. Based on the setup defined in the COLLATERAL.TYPE application, the system captures all the details with respect to these assets. These assets can also be used by other modules in Temenos Transact such as Collateral.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

ASSET.REG.PROPERTY and CO.REG.MORTGAGE tables are designed to capture external assets like Mortgages, Assignments, Floating Charges and fixed charges. These tables are linked with the Temenos Transact collateral module to secure given facility or liability.


##### Workflow

This feature allows the user to perform the following tasks:

CO.REG.MORTGAGE is an application to capture the details of Mortgage provided as collateral such as Collateral information, Property information, and Asset values.

To create a Mortgage record, follow the below steps:

1. Input Mortgage- Asset Register .
2. Enter values in all or relevant fields: Description Currency Land Registry District Registration Number Contract Ref Registration Date Reg Completed Date Mortgage Rank Interest Rate Notes CLA Number Customer Agreement Date Value Date End Date Property Ref Prop Val Ccy Prop District Market Value Tot Market Value Cur Tot Market Value Comp Forced Sale Value Cur Forced Sale Value Comp Coefficient Adj Market Value Sug Adj Market Value
3. Click the Validate icon to check for overrides and errors.
4. Click the Commit icon to create the record.

This enquiry allows the user to view or amend the existing Insurance records.

To amend a mortgage general details record, follow the below steps:

1. View/Amend Mortgage Details .
2. In the Mortgage General Details screen, click the Amend icon corresponding to a record.
3. Amend the required details.
4. Click the Validate icon to check for overrides and errors.
5. Click the Commit icon to amend the record.

To view Mortgage general details records, follow the below steps:

1. View/Amend Mortgage Details .
2. In the Mortgage General Details screen, click the View icon to view the corresponding record in detail.

ASSET.REG.PROPERTY is an application to capture the details of immovable property provided as collateral such as Property Details, Location Details, values and Lease Details.

To create a property record, follow the below steps:

1. Input Property- Asset Register .
2. Enter values in all or relevant fields applicable: Description Contract of Sale Asset Owner Owning Percentage Asset ID Asset Type Land Registry Number Registration Date Plot No Size Location Address Street Village Town District Country Postal Code Asset Currency Market Value Open Market Value Cur Open Market Value Comp Forced Sale Value Cur Coefficient Adj Market Value Sug Adj Market Value Start Date Expiry Date Asset Rank Notes Lease Id Original Owner Lease Start Date Lease Expiry Date Lease Tenor Renewal Right Renewal Tenor
3. Click the Validate icon to check for overrides and errors.
4. Click the Commit icon to create the record.

This enquiry allows the user to view or amend the existing Insurance records.

To amend a Property general details record, follow the below steps:

1. View/Amend Property Asset Register .
2. In the Property General Details screen, click the Amend icon corresponding to a record.
3. Amend the required details.
4. Click the Validate icon to check for overrides and errors.
5. Click the Commit icon to amend the record.

To view Property general details records, follow the below steps:

1. View/Amend Property Asset Register .
2. In the Property General Details screen, click the View icon to view the corresponding record in detail.


#### 📊 Outputs

There are no Outputs available for Other Internal Collateral Assets feature.

---


### 1.18  Pre-tradeBuyingPowerChecks


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Buying Power (BP), also referred as Purchasing Power (PP), calculation ensures that the additional risk of an order is covered by sufficient BP. To achieve this, the execution of the order is simulated and the effects on the new purchase is calculated. Only if the BP is greater than the order am...*
> 
> **Applications:** `OV.PARAMETER`, `SC.ORDER.SESSION`, `SC.PARAMETER`, `SEC OPEN ORDER`, `SEC.OPEN.ORDER`, `theCO.VALUATION.PARAMETER`, `theSC.PARAMETER`
> 
> **Key Fields:** *B*, *Buying*, *Buying Power = Cash*, *Buying Power.1.1*, *Buying Power.1.2*, *Buying.Power.1.1 and Buying.Power.1.2*, *Estimation value of other Liabilities.*, *Incl Clv Cap* ... +11 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The Buying Power (BP), also referred as Purchasing Power (PP), calculation ensures that the additional risk of an order is covered by sufficient BP. To achieve this, the execution of the order is simulated and the effects on the new purchase is calculated. Only if the BP is greater than the order amount, the order is accepted and processed further. The system displays a warning message in case of insufficient buying power.

The approval process applies to all new orders and to the amendment of pending orders. Pending orders are orders that are approved already but are not yet traded.

A portfolio that qualifies for the concentration checks considers the concentration cap in calculating the collateral lending value of the portfolio, which is used in BP calculation.

For a margin lending portfolio pledged as collateral, the bank determines the amount of loan that can be given to the customer portfolio for purchasing the new asset based on the buying power. This includes the collateral contribution of all the assets in the portfolio including the new incoming asset.

This feature requires the CX module to be installed in addition to the CO and MV modules.


#### ⚙️ Configuration

The following configurations are required for pre-trade BP checks to apply the concentration cap on the existing assets and the new incoming asset to arrive at the BP for the new asset order.

- The Include Concentration Cap field in the SC.PARAMETER application must be set to Yes.
- The Pf Qual Ccy and Pf Qual Value fields in the CO.VALUATION.PARAMETER application must be configured with the respective qualifying currency and value, if the concentration check needs to be applied only on qualifying portfolios.
- The Buying Power field must be set in the OV.PARAMETER application.


#### 🔧 Working With

The Buying Power (BP), also referred as Purchasing Power (PP), calculation ensures that additional risk of an order is covered by sufficient BP. To achieve this, the execution of the order is simulated and the effects on the new purchase is calculated. Only if the BP is greater than the order amount, the order is accepted and processed further. The system displays a warning message in case of insufficient buying power.

The approval process applies to all new orders and to the amendment of pending orders. Pending orders are orders that are approved already but are not yet traded.


##### Calculating Buying Power UsingSC.PARAMETER

For a given portfolio, the BP calculation depends on the Incl Clv Cap field in the SC.PARAMETER . This field determines if a concentration cap must be applied on the margin value of assets in the portfolio and whether the collateral value of the new incoming asset must be considered for BP calculation.

BP checks are configured in SC.PARAMETER application using the Incl Clv Cap field.

Where the bank has not configured to apply the concentration cap on the margin value of the assets in the portfolio, the BP is calculated as shown below:

Buying Power = Cash B alances + L ending value of Securities + Margin value of other assets – P ending orders – Estimation value of other Liabilities.

Where:

- The lending value of securities refers to the margin value of the securities arrived after applying the margin rates (HAR).
- The other assets are the other transactions or positions linked to the portfolio.
- Other liabilities denotes the loans or overdrafts of the portfolio.

To apply concentration cap and threshold checks, Incl Clv Cap field in SC.PARAMETER must be configured to Yes.

In this scenario, the BP for an order is calculated based on the following values:

- Collateral value of cash account in the portfolio, if it is not the funding account for the purchase order. Collateral value of securities assets in the portfolio.
- Collateral value of pending orders for the portfolio.
- Liabilities in the portfolio.
- Collateral value of the new asset being purchased.


##### Understanding Collateral Contribution of Cash Account in Portfolio

If there is cash account in the portfolio and if this account is used as the funding account for the order, the new asset purchase utilises the cash to the extent available. So, balance in the cash account becomes zero and only the remaining collateral value contributed by other assets in the portfolio is considered for margin lending. On the other hand, if the order is funded by an account that is not part of the portfolio, the collateral value of the cash account in the customer portfolio is considered for buying power calculation.

| Asset type | Single counter cap | Nominal | Price per share | Currency | MV | FX rate | MV (in Ref Ccy - USD) | LTV% | CLV (in Ref Ccy – USD) | CLV after Concap (in Ref Ccy – USD) |
|---|---|---|---|---|---|---|---|---|---|---|
| Cash | 100% | 10000 | 1 | USD | 10000 | 1 | 10000 | 100% | 10000 | 10000 |
| German Equity | 30% | 10000 | 20 | EUR | 200000 | 1.12 | 224000 | 80% | 179200 | 179200 |
| US Equity | 30% | 10000 | 10 | USD | 100000 | 1 | 100000 | 80% | 80000 | 80000 |
| US Treasury Bond | 30% | 5000 | 103 | USD | 515000 | 1 | 515000 | 85% | 437750 | 212085 |
| TOTAL |  |  |  |  |  |  | 849000 |  | 706950 | 481285 |

| Asset Type | Single counter cap | Nominal | Price per share | CCY | MV | FX rate | MV (in Ref CCy - USD) | LTV% | CLV (in Ref Ccy – USD) | CLV after Concap (in Ref Ccy – USD) |
|---|---|---|---|---|---|---|---|---|---|---|
| Cash | 100% | 10000 | 1 | USD | 10000 | 1 | 10000 | 100% | 10000 | 10000 |
| German Equity | 30% | 10000 | 20 | EUR | 200000 | 1.12 | 224000 | 80% | 179200 | 179200 |
| US Equity | 30% | 10000 | 10 | USD | 100000 | 1 | 100000 | 80% | 80000 | 80000 |
| US Treasury Bond | 30% | 5000 | 103 | USD | 515000 | 1 | 515000 | 85% | 437750 | 212085 |
| TOTAL |  |  |  |  |  |  | 849000 |  | 706950 | 481285 |


##### Order Originating in Triple A Plus (TAP)

If the order originates in Wealth Front Office Suite TAP, then Temenos Transact performs the pre-trade checks for buying power as part of the order validation process.

If the order amount exceeds the buying power, the system displays an override message as shown in the below screenshot.

The buying power and the allowed order nominal is stored in the Buying.Power.1.1 and Buying.Power.1.2 fields respectively in the SEC OPEN ORDER application, and is available for the user originating the order in TAP to check.

The below screenshot of the

application for the customer 190200 shows the buying power (

) and the allowed order nominal (

field).

Concentration cap checks are also applied for a set of orders received (from TAP) through the SC.ORDER.SESSION application. After validation, Temenos Transact calculates the margin value of individual positions, the total margin value, collateral surplus or deficit and provides an update whether the credit check has been cleared. If required, the margin value or calculated CLV is adjusted based on concentration checks.

The following flowchart explains how the order that originated in TAP is processed in the SEC.OPEN.ORDER and SC.ORDER.SESSION applications.


#### 📋 Tasks

There are no Tasks available for Pre-trade Buying Power Check feature.


#### 📊 Outputs

There are no Outputs available for Pre-trade Buying Power Check feature.


> **Related Applications:** `OV.PARAMETER`, `SC.ORDER.SESSION`, `SC.PARAMETER`, `SEC OPEN ORDER`, `SEC.OPEN.ORDER`, `theCO.VALUATION.PARAMETER`, `theSC.PARAMETER`

---


### 1.19  Preferential LTV DiversifiedPortfolio


> **📇 Quick Reference Card**
> 
> **Purpose:** *Under the ELVA program (name of an sample investment program), a higher LTV is applicable against the pre-approved LTV for some securities subject to the portfolio meeting certain diversification conditions on the number of securities.*
> 
> **Applications:** `ASSET.TYPE`, `ASST.BY.CATEG`, `INVESTMENT`, `INVESTMENT.PROGRAM`, `MANAGED.ACCOUNT`, `MANAGED.ACCOUNTS`, `MARGIN.CONTROL`, `OV.PARAMETER` ... +7 more
> 
> **Key Fields:** *Adj*, *Adj Margin Rate*, *Basis*, *C*, *Ccy*, *Co*, *Co Mv Check*, *Count* ... +14 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Under the ELVA program (name of an sample investment program), a higher LTV is applicable against the pre-approved LTV for some securities subject to the portfolio meeting certain diversification conditions on the number of securities.

The credit admin in the bank records the securities marked under the ELVA program. These securities are then recorded and maintained under a separate portfolio. Additionally, this portfolio is marked for diversification so that a higher margin rate, that is, a preferential rate is applied as compared to the standard margin rate.

Around 20 securities are identified under ELVA and held as a single portfolio. The portfolio is then enabled for diversification. The diversification condition is set to the portfolio having a minimum of five ELVA securities traded under this portfolio, which are considered as diversified. This portfolio, having satisfied the diversification condition, qualifies for a preferential rate when traded. Therefore, this preferential rate is applied in the place of a standard margin rate when the portfolio is diversified for LTV computations.

Therefore, it is possible to explicitly define a preferential rate for the diversified portfolio. Further, where a portfolio is attached as collateral and that the collateral currency is not the same as limit currency, cross currency haircut percentage (as a percentage deductible from preferential or standard margin rate) can be defined, which is applied to calculate the final LTV. This cross currency haircut percentage, if defined is applicable on diversified or non-diversified portfolios (whichever the scenario is).

This feature requires the CX module to be installed in addition to the CO and MV modules.


#### ⚙️ Configuration


##### Defining Preferential Rate to be Applied on a Diversified Portfolio

The Adj Margin Rate field available in the following applications defines the rate applicable when a portfolio is classified as Diversified.

- SC.SECURITY.MARGIN
- SC.CUSTOMER.MARGIN
- MARGIN.CONTROL
- SUB.ASSET.TYPE
- ASSET.TYPE
- MANAGED.ACCOUNTS
- SECURITY.MASTER

The Adj Margin Rate field is also used to define the Lower Margin Rate (LAR) for collateral or margin value calculations. When a transaction involves a cross currency (that is, limit currency is not the same as the collateral currency), a lower rate than the standard margin rate is applied as haircut. There is a challenge when a diversified portfolio also requires a cross currency haircut. Both rate for diversified portfolio and cross currency haircut cannot refer to Adj Margin Rate field.

Hence, P refntl Margin Rate field is used to define the preferential rate. This is an optional field. Where a portfolio qualifies to be a diversified portfolio after the diversification conditions are met, the preferential rate defined in Prefntl Margin Rate field is applied for LTV computations in the place of standard margin rate, provided the Co Mv Check field is set to Yes in the SC.PARAMETER application.

The value for P refntl Margin Rate field can be a rate (a fixed value) ranging between 0.00 and 100.00. A value without the + sign indicates a revised HAR or the preferential LTV.

The value can also be an incremental value.

If the value +10 is entered in this field, then it indicates that the incremental value must be added to the margin rate obtained from the relevant applications. A value preceded with +, indicates the incremental value. The preferential rate specified here computes and arrives at the enhanced LTV for diversified portfolio.


##### Understanding the Changes Regarding Future Effective Dated Rates

Sometimes it is necessary to define margin rates, which takes effect on a future date. On defining the future dated rates, it allows the system to effect the new rates automatically on the system reaching the future effective date. Therefore, the applications listed in the preceding section have the provision enabled to record future rates including the preferential rate. Therefore, the preferential margin rate and currency haircut percentage are part of this multivalued association, except the MANAGED.ACCOUNT application, as the application does not support effective date feature.

> **⚠️ Note:** The future dated effective rates, which are applicable at the SECURITY.MASTER level must be defined in the SC.SECURITY.MARGIN application.


##### Defining Cross Currency Haircut as a Percentage Deductible from the Margin Rate or Preferential Rate

The Ccy Haircut Perc field is an optional field and is entered when the Co Mv C heck field is set to Yes in the SC.PARAMETER application and the Adj Margin Rate field in the respective application does not have a value. This field is available in the following applications:

- SC.SECURITY.MARGIN
- SC.CUSTOMER.MARGIN
- MARGIN.CONTROL
- SUB.ASSET.TYPE
- ASSET.TYPE
- MANAGED.ACCOUNTS
- SECURITY.MASTER
- ASST.BY.CATEG

The Ccy Haircut Perc field accepts a percentage value. Therefore, when this field is defined, the haircut percentage is applied to the standard margin rate or preferential rate (if given in case of diversified portfolio) and to that extent reduce the margin rate or preferential margin rate. This revised rate (LTV% after hair cut) is computed to derive the revised Collateral Lending Value (CLV) calculations.


##### Grouping and Recording the Securities under ELVA Program

This is an optional configuration. If the securities of ELVA need to be grouped, then the below can be considered through this configuration, as it only serves as information with no functionality attached to it. Using the INVESTMENT.PROGRAM application, the user can create a record to store the valid list of securities qualifying under the ELVA program.

> **⚠️ Note:** Banks need to adapt a local process through its operations to ensure that ELVA securities alone are traded using the specified portfolio enabled for diversification. The INVESTMENT . PROGRAM is a record which links the model to a portfolio.


##### Activating the Diversification for Portfolio

The Diversification field in the SEC.ACC.MASTER application must be set to Yes, to activate the diversification for that portfolio.


##### Defining the Diversification Condition for Portfolio

The diversification conditions are defined in the OV.PARAMETER application. In this application, the user can specify the number of stocks that a portfolio must hold for it to be considered a diversified portfolio. The Stock Count Basis field in OV.PARAMETER is set as All and the Stock Held field is set as any numeric (for example, five).

> **⚠️ Note:** As a prerequisite, ELVA securities are maintained as a separate portfolio and enabled for diversification. Then, this portfolio exclusively trades only ELVA securities.


#### 🔧 Working With


##### Computing Preferential Rate

Temenos Transact is capable of fetching the preferential rate defined for diversified portfolios if the diversification condition is met. Then the system uses the preferential rate to compute the enhanced or revised LTV.

| Asset | MV | Enhanced LTC (preferential margin rate) | CLV | Cross CCy Haircut (%) | New CLV |
|---|---|---|---|---|---|
| ENT ABC XYZ | 1000 | 55 | 550 | 5.5 | 495 |
| KINGDOM OF THAI | 1000 | 65 | 650 | 6.5 | 585 |
| CAR ABC | 1000 | 65 | 650 | 6.5 | 585 |
| AKA MOTORS LTD | 1000 | 65 | 1300 | 6.5 | 1170 |
| SOFTBLOCK GROUP | 1000 | 65 | 650 | 6.5 | 585 |
| Total | 6000 |  | 3800 |  | 3500 |


##### Treating Cross Currency Haircut

In the process of advance ratio calculations, the system’s allocation precedence is towards liabilities of the same currency after single concentration cap is applied and then the system subsequently converts the unallocated amount to LAR (using the Adj Margin Rate value ) before allocating to other currency’s liabilities.

The execution value in collateral is derived using the below formula.

Same currency allocations in HAR + other currency allocations using LAR + unallocated amount (in LAR)


#### 📋 Tasks

There are no Tasks available for Preferential LTV for Diversified Portfolio feature.


#### 📊 Outputs

There are no Outputs available for Preferential LTV for Diversified Portfolio feature.


> **Related Applications:** `ASSET.TYPE`, `ASST.BY.CATEG`, `INVESTMENT`, `INVESTMENT.PROGRAM`, `MANAGED.ACCOUNT`, `MANAGED.ACCOUNTS`, `MARGIN.CONTROL`, `OV.PARAMETER`, `PROGRAM`, `SC.CUSTOMER.MARGIN`, `SC.PARAMETER`, `SC.SECURITY.MARGIN`, `SEC.ACC.MASTER`, `SECURITY.MASTER`, `SUB.ASSET.TYPE`

---


### 1.20  Real-time Portfolio Collateral Valuation


> **📇 Quick Reference Card**
> 
> **Purpose:** *Temenos Transact reworks the portfolio collateral allocation automatically, when there is a change in the value of the portfolio. Portfolio value change is due to:*
> 
> **Applications:** `COLLATERAL.PARAMETER`
> 
> **Key Fields:** *Online Update*, *Realtime Alloc*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Temenos Transact reworks the portfolio collateral allocation automatically, when there is a change in the value of the portfolio. Portfolio value change is due to:

- New buy or sell in the portfolio.
- Change in the price of the portfolio.

Any new transaction to the portfolio triggers the portfolio valuation online, when the OV module is installed. The portfolio valuation triggers the collateral valuation, which happens through the COLLATERAL.ONLINE.REVALUATION service.

The online collateral revaluation happens even for the portfolio price change event. This real-time valuation is applicable only for the assets that are attached to the portfolio.


#### ⚙️ Configuration

Online revaluation of collateral happens only when Realtime Alloc field is set in the COLLATERAL.PARAMETER application.

Collateral revaluation or recalculation is also run online, when Client Details and Limit Summary/Customer Liability enquires are executed. It also runs at specific intervals that is specified in the COLLATERAL.PARAMETER application.

The Realtime Alloc field can be set to:

- Yes - Performs collateral revaluation when every customer portfolio is revaluated or when the Client Details and Limit Summary/Customer Liability enquires are executed.
- No - Does not perform the portfolio collateral revaluation online (it is done in COB by default).
- 1-99 - Time interval for collateral valuation to be performed online. It can be a number between 1-99.

This collateral and limit reallocation happens only when the Online Update field is set in the following applications:

- LIMIT
- COLLATERAL.TYPE
- COLLTERAL.PARAMETER


#### 📋 Tasks

There are no Tasks available for Real-time Portfolio Collateral Valuation feature.


#### 📊 Outputs

There are no Outputs available for Real-time Portfolio Collateral Valuation feature.


> **Related Applications:** `COLLATERAL.PARAMETER`

---


### 1.21  Right to Link the Collateral


> **📇 Quick Reference Card**
> 
> **Purpose:** *The COLLATERAL.RIGHT application is used to record the status of a security right and to indicate against which customer outstanding the right applies to. The link between the COLLATERAL.RIGHT application and the collateral object itself is implicit in the structure of identifiers between the two ap...*
> 
> **Applications:** `COLLATERAL.RIGHT`
> 
> **Sections:** 📖 Introduction | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The COLLATERAL.RIGHT application is used to record the status of a security right and to indicate against which customer outstanding the right applies to. The link between the COLLATERAL.RIGHT application and the collateral object itself is implicit in the structure of identifiers between the two applications.


#### 📋 Tasks

Related topics:

- Create And Link Collateral

The collateral Right file is used to record the ownership of the collateral and helps to link the collateral item with the respective limit reference. Collateral right covers the liabilities of the customer at Contract Level, Limit Level and Customer level.


##### Workflow

This section allows the user to view the below activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Authorise/ Delete Collateral Right . |
| Unauthorised Collateral Right | Click the Authorise icon corresponding to a record. |
| Collateral Link | Click the Authorise icon to verify the record. |


#### 📊 Outputs

There are no Outputs available for Right to Link the Collateral feature.


> **Related Applications:** `COLLATERAL.RIGHT`

---


### 1.22  Support for Wealth Credits


> **📇 Quick Reference Card**
> 
> **Purpose:** *Wealth Credits are facilitated by pledging the customer portfolio (part or full).*
> 
> **Key Fields:** *Actual Value*, *Asset Cap*, *Asset Id*, *Collateral Id*, *Collateral Provided*, *Instrument ID*, *Instrument Id*, *Percentage* ... +4 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Wealth Credits are facilitated by pledging the customer portfolio (part or full).

The Share Margin Financing (SMF) is one of the wealth credit facilities offered by banks to the customers, where the customer can pledge a part of the portfolio to avail the margin for trading. Hence, when a customer pledges the portfolio as a collateral for any other credit facility in future, the positions pledged for SMF is excluded while calculating the collateral value of the portfolio pledged.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 🔧 Working With

The Collateral (CO) module captures the details of the pledged portfolio (part or full) as collateral for the wealth credit facility. A customer can pledge the full or part of the portfolio as collateral to purchase additional shares. The pledge for Share Margin Financing (SMF) can be held:

- Full or part of nominals in specific securities (SC) assets or securities position.
- As a specific or full percentage of a non-securities asset position.
- As a specific percentage or the entire portfolio.

The SC.FACILITY.APPLN application captures the Wealth facilities (including SMF). The COLLATERAL application supports the pledge details for SMF and allows to link the same portfolio to multiple collaterals, when the pledging is done through SC.FACILITY.APPLN . Based on the SMF, the collateral values are calculated with valuation changes.


##### Capturing Wealth Credit Facility inSC.FACILITY.APPLN

The fields that support collateral pledge in SMF are described below.

| Field Name | Description |
|---|---|
| Pledged Quantity | Indicates the quantity of shares pledged as collateral. This field is enabled only if the value in the Collateral Provided field is a security instrument |
| Collateral Provided | Links the portfolio to SMF with the below ID’s: For pledging non-security asset like cash accounts, the SC.POS.ASSET ID is used to link the asset For pledging security asset, the security Instrument ID in the portfolio is used for linking For pledging the entire portfolio, Portfolio ID ( SEC.ACC.MASTER ID ) is used for linking |
| Percentage | Indicates the percentage of portfolio pledged as collateral. This field is enabled only if the value in the Collateral Provided field is pledging portfolio and non-security instruments |
| Collateral Id | Generated by system automatically when portfolios are pledged through SMF |

> **⚠️ Note:** If 100% of the portfolio is already pledged through the SC.FACILITY.APPLN , the User would still be able to create another wealth facility through SC.FACILITY.APPLN by pledging a specific position of the portfolio (in part or full).

A portfolio can be pledged as collateral either through the COLLATERAL or SC.FACILITY.APPLN application. An error is prompted when a user tries to create a collateral directly by linking the portfolio (part or full) that is already pledged through the SC. FACILITY.APPLN . Similarly, an error is prompted when a portfolio (part or full) that is linked directly to the COLLATERAL application is pledged again through the SC.FACILITY.APPLN .


##### Creating Collateral for the Pledged Portion

The collateral is automatically created for the asset pledged through the SC.FACILITY.APPLN application. Such collaterals are not allowed for manual amendment. Any changes to the collateral associated with the SMF must be initiated only through the SC.FACILITY.APPLN application.

The list of fields below support SMF in the COLLATERAL application:

| Field Name | Description |
|---|---|
| Asset Id | Indicates the Instrument Id or Portfolio Id |
| Asset Cap | Indicates the number of nominal of security or percentage of portfolio pledged in SC.FACILITY.APPLN |
| Sc Facility App Id | Indicates the respective record ID in SC.FACILITY.APPLN |


##### Updating theCO.ASSET.DETAILS

When 50% of non-security asset in a portfolio is pledged in SMF, only 50% (24928 ,refer the table below) of the total value (49858) is considered for margin value calculation and for allocation process.

When 50% of the nominal of security assets are pledged, only 50% (that is 100 nominal * price (166.69 = 16669 refer the table below) is considered for margin value calculation and for allocation process.

| PF | Nominals | Price | Total Value | Pledge% | Available Nom | Value considered for allocation |
|---|---|---|---|---|---|---|
| Cash | NA | NA | 49858 | 50% | P-50 | 24928 |
| Shares | 200 | 166.7 | 33338 | 50% | N-100 | 16669 |

The pledged value for shares and cash accounts for Actual Value field in CO.ASSET.DETAILS are shown in the below screenshots.


#### 📋 Tasks

There are no Tasks available for Support for Wealth Credits feature.


#### 📊 Outputs

There are no Outputs available for Support for Wealth Credits feature.

---


### 1.23  Third Party Pledge


> **📇 Quick Reference Card**
> 
> **Purpose:** *This feature enables the user to cover liabilities of a group of customers, with the pledge offered by one or more customers. Customers may generally pledge their assets (held in their portfolio) in favour of other customers. Each pledge has different priorities and amount allocated to each customer...*
> 
> **Sections:** 📖 Introduction | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

This feature enables the user to cover liabilities of a group of customers, with the pledge offered by one or more customers. Customers may generally pledge their assets (held in their portfolio) in favour of other customers. Each pledge has different priorities and amount allocated to each customer is calculated dynamically rather than based on fixed percentages.


#### 📋 Tasks

There are no Tasks available for Third Party Pledges feature.


#### 📊 Outputs

There are no Outputs available for Third Party Pledges feature.

---


---


## Chapter 2: Limits_Collateral - LI


Limits_Collateral - LI module of Temenos Transact


### Features in Limits_Collateral - LI


| # | Feature | Sections |
|---|---------|----------|
| 2.1 | Misc | Intro |
| 2.2 | Non-Stop Processing | Confi |
| 2.3 | Chrg Acct Fees Chrgs on Limit | Intro, Confi, Worki, Tasks, Outpu |
| 2.4 | Collateral Allocation to Limit | Intro, Confi, Tasks, Outpu |
| 2.5 | Creating Cross Limits | Intro, Confi, Tasks, Outpu |
| 2.6 | Creating Customer Liability Structure | Intro, Confi, Worki, Tasks, Outpu |
| 2.7 | Creating Limit Products | Intro, Confi, Tasks, Outpu |
| 2.8 | Credit Checking | Intro, Confi, Tasks, Outpu |
| 2.9 | Credit Limits | Intro, Confi, Tasks, Outpu |
| 2.10 | Cus Rsk Grp For Mt Jt Cus Lim | Intro, Confi, Worki, Tasks, Outpu |
| 2.11 | Customer Grouping | Intro, Confi, Tasks, Outpu |
| 2.12 | Customer Sub-Group in Risk Exposure | Intro, Confi, Tasks, Outpu |
| 2.13 | Externalise Transact Limit Exposure | Intro, Confi, Worki, Tasks, Outpu |
| 2.14 | Impact of Loan Repayment | Intro, Confi, Tasks, Outpu |
| 2.15 | Intraday Limit | Intro, Confi, Tasks, Outpu |
| 2.16 | Joint Owned Limits | Intro, Confi, Tasks, Outpu |
| 2.17 | Liability Structure Limit Sharing Group | Intro, Confi, Worki, Tasks, Outpu |
| 2.18 | Limit Change Utility | Intro, Confi, Tasks, Outpu |
| 2.19 | Limit Sub-Allocation | Intro, Confi, Tasks, Outpu |
| 2.20 | Linking Collaterals to Limit | Intro, Confi, Tasks, Outpu |
| 2.21 | Misc | Intro |
| 2.22 | Monitoring Credit Exposure | Intro, Confi, Tasks, Outpu |
| 2.23 | Neutral Revolving Limit Structure | Intro, Confi, Worki, Tasks, Outpu |
| 2.24 | Offsetting Credit Balance Accounts | Intro, Confi, Tasks, Outpu |
| 2.25 | Overdraft Limits to Accounts | Intro, Confi, Tasks, Outpu |
| 2.26 | Reporting of Breach to Validation Limit | Intro, Confi, Tasks, Outpu |
| 2.27 | Restricted Allowed Customers | Intro, Confi, Tasks, Outpu |
| 2.28 | Risk Exposure Overview Enquiry | Intro, Confi, Tasks, Outpu |
| 2.29 | Sec Lim Coll | Intro, Confi, Worki, Tasks, Outpu |
| 2.30 | Special Limit Processing for Foreign Exchange | Intro, Confi, Tasks, Outpu |
| 2.31 | Time Banding of Limits | Intro, Confi, Tasks, Outpu |
| 2.32 | Update Approved | Intro, Confi, Tasks, Outpu |
| 2.33 | Updating Limit Exposure | Intro, Confi, Tasks, Outpu |
| 2.34 | Utilisation of Limits | Intro, Confi, Tasks, Outpu |


### 2.1  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *Account is an integral part of banking business. The functional components of the Account (AC) module involves the creation, maintenance and closure of accounts. The AC and Interest and Charges (IC) module together caters the creation, maintenance and control of all types of accounts handled by Teme...*
> 
> **Applications:** `#PGM.AUTOM.ID`, `AC.SYS.CODES`, `ACCOUNT`, `ACCOUNT.CLASS`, `ACCOUNT.CREDIT.INT`, `ACCOUNT.DEBIT.INT`, `ACCOUNT.PARAMETER`, `ACCT.CAPITALISATION` ... +29 more
> 
> **Key Fields:** *; Use Pay Rec Sys*, *Acc*, *Account*, *Acct*, *Acct Checkdig Type*, *Arc Filename*, *Archive Data*, *Basis* ... +53 more
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- APIs
- Temenos Transact Services

Account is an integral part of banking business. The functional components of the Account (AC) module involves the creation, maintenance and closure of accounts. The AC and Interest and Charges (IC) module together caters the creation, maintenance and control of all types of accounts handled by Temenos core banking.

Temenos Transact AC module is Non-Stop (NS module) compatible. If NS module is installed, the account balances are updated real-time to ensure that the latest transaction impact is fully included from the customer perspective. Read Non-Stop Processing User Guide for more information on the specific applications compatible with NS processing.


##### Product Configuration

This topic covers the setup and usage of the applications used in AC module.

| Field Name | Usage |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| Cash Flow Days | Specifies the number of calendar days forward for which the cash flow balances are to be maintained for the purpose of accounting overrides and cash flow processing. The number of days entered here determines the window period that cash flow balances are to be maintained on each account record. Each forward dated entry generated for an account impacts the cash flow balances, if the date of the entry falls within this period. If the number of days entered is 10, then any forward dated entry raised online that has the value date less than 10 calendar days from current date will update the accounts cash flow balances. If this update causes either a limit to be exceeded or an unauthorised overdraft to occur, then an override message appears on the transaction input. All entries raised online that fall outside the window do not update the account balances immediately and no override messages appear. But when their value dates fall within the window, the start of day process (SOD.CASH.FLOW) updates the account cash flow balances. If an exception occurs at this stage, then the CASH.FLOW.EXCEPTION table is updated to indicate this. If the value is not entered in this field, then only the nostro accounts have cash flow maintained and a default of 10 calendar days is used for this. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Value Dated Acctng | A switch to set value dated accounting as On or Off or Trade Dated General Ledger (TDGL). If a value dated accounting system is required, then this field must be set to Y. In trade dated accounting system, the cash based transactions update the customer’s account and the bank’s position on the date in which the transaction is processed in the system, irrespective of the value date assigned to the transaction. In value dated accounting system, the cash based transactions update the customer’s account and the bank’s position on the value date assigned to the transaction. It is held as off balance sheet until the value date. In TDGL accounting system, the cash based transactions update the customer’s account and the bank’s position on the value date assigned to the transaction. It is held under payable or receivable until the value date. Cash based transactions follow the accounting treatment based on this setup. However, the accounting treatment can be switched from one system to another and the system permits any of the following switch. Switching of Accounting System Treatment of cash based transactions can be switched from one system to another, any combination of the setup is possible. Original Accounting Setup Target Accounting Setup Trade dated Value dated Trade dated Trade dated GL Value dated Trade dated Value dated Trade dated GL Trade dated GL Trade dated Trade dated GL Value dated The new accounting system switch applies to new transactions only. The existing cash based transactions with a future date follows the setup applied when the transaction were raised. The Tdgl Details field in the STMT.ENTRY application holds the details of the accounting method followed for the transaction. Exceptions to the above is SEC.TRADE – Actual Settlement: If contract input is in existing setup and authorised in the modified setup, then the system follows the modified setup. | Original Accounting Setup | Target Accounting Setup | Trade dated | Value dated | Trade dated | Trade dated GL | Value dated | Trade dated | Value dated | Trade dated GL | Trade dated GL | Trade dated | Trade dated GL | Value dated |
| Original Accounting Setup | Target Accounting Setup |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Trade dated | Value dated |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Trade dated | Trade dated GL |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Value dated | Trade dated |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Value dated | Trade dated GL |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Trade dated GL | Trade dated |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Trade dated GL | Value dated |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Use Pay Receive | This field is used to flag the suspense processing at system Level, in the case of value dated or TDGL accounting setup. Under these accounting setup, the value of the transaction is suspended in a temporary account till the split value date is reached. The allowed values are : Yes – Suspended to GL accounts pay or receive as special entries and reported as on-balance sheet item in the general ledger (GL) report. No – This is the default setup where the suspense processing posts the entry to the internal suspense account. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Pay Rec Allwd | This field works in conjunction with Use Pay Receive . It is used when a customer wants to decide if payable or receivable are to be reported with account attributes or against underlying customer attributes based PR.CUSTOMER.BALANCE application. Value in this field should be valid record ID of AC.DEFINE.PAY.RECV.ALLOWED application. This field is available at different levels such as System level, System Id (sub-system) level, Category level and System ID with Category level. In the AC.DEFINE.PAY.RECV.ALLOWED application, the users can create their own records using any of the following options in the Pay Recv Options field. The ID of the application record can be a meaningful alpha-numeric name. Broker – This option decides the customer to whom the payable or receivable is to be booked in the PR.CUSTOMER.BALANCE . If this option is set, the payable or receivable is booked against the third party customer (for example, broker) passed from the application. If this option is not set, the payable or receivable is booked against the customer passed in the original entry from the underlying application. Contract – If this option is selected, all the payables or receivables are reported under the PR.CUSTOMER.BALANCE . Customer – If the target account passed from the underlying application is a customer account and the Customer option is set, then the payables or receivables are reported under PR.CUSTOMER.BALANCE . Internal – This option works similar to Use Pay Recv set to Yes. If the entry is posted as an internal (suspense) account and the target account is passed from the application, then the original STMT entry to internal (suspense) account is converted to special entry with asset type as PAYSUS or RECEIVESUS. Nostro – If the target account passed from the underlying application is a NOSTRO account, and the Customer option is set, then the payables or receivables are reported under PR.CUSTOMER.BALANCE . NULL – If no option is set, then the system continues to work as usual. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Val Date Sys Id; Val Date By Sys ; Use Pay Rec Sys | Enables the definition of accounting treatment for specific cash-based applications, where it is different from the default accounting treatment. If the default accounting system is trade dated, for the application mentioned in Val Date Sys Id , a different accounting system can be defined. For example, if SEC.TRADE is to follow TDGL accounting system, the Val Date Sys Id is defined as SCTR and Val Date By Sys is defined as TDGL. The Use Pay Rec Sys field can be flagged as Yes or No, which is used in the suspense processing for the specific application. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Vd Cat Start; Vd Cat End; Val Date By Cat; Use Pay Rec Cat | Enables the definition of accounting treatment for specific category or range of categories, where it is different from the default accounting treatment and application specific (if defined) accounting treatment. The category level definition takes precedence over the system level and application level definition. The Use Pay Rec Cat field can be set to Yes or No, which is used in the suspense processing for the specific category. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Vd Cat Sys Id; Vd Cat Sys Start; Vd Cat Sys End; Val Date By Cat Sys; Use Pay Receive Cat Sys | If the accounting system for specific categories of an application is different from the default accounting system, it can be setup using these set of fields. The application can be defined in Vd Cat Sys Id , the category or range of categories can be defined in the Vd Cat Sys Start and Vd Cat Sys End fields. The accounting system applicable to this setup are defined in the Val Date By Cat Sys field. The Use Pay Receive Cat Sys field can be set to Yes or No, which is used in the suspense processing for the specific category. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Entry Category; Sus Category; Suspense Txn In; Suspense Txn Out; Suspense History | The format of Entry Category can either be CATEGORY-FX.POS.TYPE or CATEGORY, which determines the suspense account to be used when operating in a value dated accounting system. If the position type for the Entry Category does not exist, then the entry category alone is used to determine the suspense category. Else, the default suspense category is used. When a split value dated transaction is processed in a value dated accounting system then the first leg is balanced against a suspense account. This is washed out when the second leg reaches its value date. The suspense account that is used is determined by the category of the second leg entry. The Entry Category field and its associated field Sus Category defines this relationship. Example XX.1 ENTRY.CATEGORY YY.1 SUS.CATEGORY 19998 XX.2 ENTRY.CATEGORY 5000-XX YY.2 SUS.CATEGORY 19999 Entry Category is a start of range value. Hence in this example, second leg entries with a category in the range 0 - 4999 uses account LCL199980001 (where LCL is the local currency code) and entries with a category 5000 and above uses LCL199990001 for suspense processing. To define a default suspense account for all the entries, configure as shown below: XX.1 ENTRY.CATEGORY YY.1 SUS.CATEGORY 19998 The purpose of defining different suspense category is to allow the splitting of suspense movements, for value dated accounting, within the CRB. For example, it is possible to report suspense entries for nostro accounts separately from suspense entries for current accounts. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Sys Code; Nostro Default; Def Override; Use First Acct; Default Order | These set of fields are used for defaulting the settlement nostro account applicable to the transaction defined in the Sys Code field. The Sys Code field is a combination of Application-Nature of transaction, for example, LD-PRIN or LD-INT. These values must be defined upfront in AC.SYS.CODES application. The Nostro Default field is used to specify how settlement accounts are defaulted when using a nostro account for the associated Sys Code . A null value implies that the nostro account is always defaulted. The following are the options in this field: AGENCY – Defaults only when agency conditions exist. NONE – No nostro account is to be defaulted. The Def Override field defines whether an override is required when the default account number does not match the account number entered on the deal. Additionally, if the account with bank, intermediary bank or beneficiary account number differs from the default derived from the information on the agency file, then an override is raised if this field is set to Yes. The Use First Acct field defines whether an account is to be defaulted when more than one possible default account exists. The following options are available in this field: Yes – First account of the customer in any company is defaulted. No – If more than one account is present in the current company, then no defaulting takes place. In a multi-book setup, the following additional options are available for this field: CUR – First account of the customer in current company is only defaulted. FRS – First account of the customer in the current company as first choice followed by first available account in any company is defaulted. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Cheque Register; Chq Dep Txn; Def Coll Susp; Chq Col Txn; Chq Ret Txn; Def Ret Susp; Return Txns; Return Susp Cat | The Cheque Register field indicates whether or not the cheque issue and management functionality within Temenos Transact has been activated. The Yes or No value entered in this field controls the defaulting of cheque type in DATA CAPTURE (DC) or FUNDS TRANSFER (FT) or TELLER (TT) application as well as payment stop processing. The list of transaction code for cheque on collection, clearing and returned cheque and the corresponding suspense accounts where the value of cheque needs to be parked in the clearing process can be defined in these set of fields. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Net Od Appl; Net Od Override; Net Locked Override | The Net Od Appl field specifies the Temenos Transact application for which debit and credit entries to an account in a transaction must be netted for displaying the overdraft and cash flow overrides. The allowed applications are LOANS AND DEPOSITS (LD), TELLER (TT), COLLATERAL (CO), FUNDS TRANSFER (FT), ARRANGEMENT ARCHITECTURE (AA) or ALL. When this field is set to ALL, the functionality is applied for all transaction irrespective of the application. The pre-condition for the suppression of overrides is to set the Net Od Override field as Yes. If Net Od Appl holds the value ALL, the system does not permit any other multi-value to be input. Either applications are manually input in a multi-value block or ALL value is used. For example, if the Net Od Appl field is set to ALL and the Net Od Override field is set to Yes and a transaction is made using the same account as both debit and credit account, no override is generated for any excess amount. Suppression of Unnecessary Overrides: If a single contract creates both credits and debits to an account, if the net effect of the contract is to credit the account, it is possible to suppress the override generated for the debit side of the transaction. Example If a discounted loan is arranged for a customer, whereby the customer has a balance of £10, receives a credit of $1000 for the loan, but also a debit of $100 for the upfront payment of interest. The system usually generates an override specifying that the customer is debited $100 and the customer is being overdrawn by $90. However, it is possible by configuring the Net Od Appl as LD and Net Od Override fields as Yes in the ACCOUNT.PARAMETER to net off the differences, so as the credit of $1000 exceeds the debit of $100 and the override is suppressed. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Retain Ac Balances | Defines whether balances need to be maintained in ACCOUNT or not. When set to Yes the balances are updated in ACCOUNT and EB.CONTRACT.BALANCES . When set to N the balances are not updated in ACCOUNT , but updated only in EB.CONTRACT.BALANCES . Default value is Yes. Changing this setup from Yes to No clears the existing account balances automatically. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Booked Balance | Defines which booked balance is recorded in the STMT.ENTRY record when the transaction is booked. The following are the options available in this field. Online Actual Bal – Records the account balance from the GL perspective, this means that future dated movements are not included. Traded Dated Gl Bal – Records the account balance from a customer perspective, which means that future dated movements recorded as PAY or RECEIVE are included. The enhanced transaction search uses the value in this field to display the output in Booked Balance column of the enquiries |  |  |  |  |  |  |  |  |  |  |  |  |  |  |

In order to open or create a customer account, the account holder must first be registered as a customer in Temenos Transact with all the relevant information required for KYC. The following details and other important information pertaining to the customer is captured in this application.

- Name
- Address
- Age
- Residence
- Sector
- Language
- Industry
- Status
- Joint holder’s name
- Signature(s)

Certain static attributes like name and contact details of the ACCOUNT is defaulted from the CUSTOMER . Some attributes from the CUSTOMER application, like Sector and Residence are used in grouping the accounts.

| Dedicated Category Ranges for ACCOUNT module in Temenos Transact | Recommended Usage of CATEGORY CODES |  |  |
|---|---|---|---|
| Category Range | Banking Product | Category Range | Recommended Break-up of Banking Product |
| 1000-8999 | Non-Contingent client accounts |  |  |
|  |  | 1000-1999 | Demand or current accounts |
|  |  | 2000-2999 | Vostro accounts |
|  |  | 3000-3999 | Loan accounts (used for AA and Islamic loan accounts) |
|  |  | 4000-4999 | Margin accounts |
|  |  | 5000-5999 | Nostro accounts |
|  |  | 6000-6999 | Savings accounts (used for regular SB accounts and AA deposit accounts) |
|  |  | 7000-7999 | Provision (specific provision on loans) |
|  |  | 8000-8999 | Other client accounts (like sundry debtors, sundry creditors and the like) |
| 9000-9999 | Contingent client accounts |  | Contingent client accounts (like cheque sent on collection, off balance sheet limit and the like.) |
| 10000-18999 | Internal accounts to maintain bank's assets and liabilities |  |  |
|  |  | 10000-10999 | Cash and cash equivalents (includes cheque clearing accounts, traveler’s cheques) |
|  |  | 11000-11999 | Fixed and movable assets |
|  |  | 12000-12999 | Transit assets (includes all income receivables, prepaid expenses, petty cash and the like) |
|  |  | 13000-13999 | Other assets |
|  |  | 14000-14999 | Suspense accounts |
|  |  | 15000-15999 | Liabilities (includes monetary papers, general or specific provisions) |
|  |  | 16000-16499 | Provision for depreciation |
|  |  | 16500-16599 | Internal margin accounts |
|  |  | 16600-16999 | Other open internal accounts |
|  |  | 17000-17999 | Transit liabilities (includes all expense or accounts payable and income received in advance) |
|  |  | 18000-18999 | Capital liabilities (includes owner's equity, statutory or other reserves and retained earnings) |
| 19000-19999 | Internal contingent accounts |  |  |

The operating currency is the currency in which the account is operated. It must be one of the currencies defined in CURRENCY application. Once the account is authorised, the currency cannot be changed as the balances of the account is maintained in this currency. In other words, the account holder can make or receive payments in any currency other than the operating currency but when the account balance is updated for these payments, it is converted into the operating currency of the account.

The operating currency of account 84506 is EUR. If the customer wants to make a payment to the beneficiary in USD from the account 84506, it is possible. The balance in account 84506 would be impacted to the extent of EUR equivalent of the payment amount in USD.

| Group ID | Group Name | Category | Sector | Residence |
|---|---|---|---|---|
| 1 | Current account – Individual | 1001 | 1001 |  |
| 2 | Current account – Staff | 1001 | 1002 |  |
| 3 | Savings account – Resident | 6001 |  | UK |
| 4 | Savings account – Non-Resident | 6001 |  |  |
| 5 | Nostro account | 5001 | 3001 |  |
| 5002 | 3002 |  |  |  |
| 5003 | 3003 |  |  |  |

The account specific interest and charge conditions are defined in the ACCOUNT.DEBIT.INT (ADI), ACCOUNT.CREDIT.INT (ACI) and ACCT.CAPITALISATION applications. The ID format of this application is - . For example, 12165-20170321.

Bank may want to specify a differential interest and charge condition for specific accounts in the group. For such accounts, the interest and charge conditions can be defined in the ACCOUNT.DEBIT.INT and ACCOUNT.CREDIT.INT applications. This supersedes the conditions defined at the group level.

On a later date, if the account has to be reverted to the group specific conditions, the Interest Day Basis field in the ADI or ACI record must be set to GENERAL. This change is effective from the date on the ID of the ADI or ACI record. Similarly, some account holders may request for an interest capitalisation date different from that of the group. For such accounts, the interest capitalisation date and frequency can be defined in ACCT.CAPITALISATION application.

| Key | Description |
|---|---|
| TFLC | Letter of credit |
| DDSTD | Direct debit standalone |
| BROKER | Brokerage to be paid |
| DDSUSP | Direct debit suspense |
| LCDIFF | Letter of credit difference |
| RCSUSP | Suspense category for RC |
| SLDIFF | SL Skim account |
| SUSPPD | Suspense Past Due |
| SYFUND | SY Fund |
| ACERROR | Currency mismatch suspense |
| DDCLAIM | Direct debit claim |
| EXCHADJ | Forex Revaluation profit and loss |
| IACLOSE | IA profit and loss year end closeout |
| INTERCO | Inter branch |
| LCAMORT | Letter of credit amortisation |
| LCLSUSP | Letter of credit suspense |
| LGCLOSE | LG profit and loss year end closeout |
| MDCLAIM | MD fee settlement |
| MERGEMM | MM merge |
| NETTING | Netting suspense |
| PDREPAY | PD repayment |
| PLCLOSE | Profit and loss year end closeout |
| SWREVAL | Swap revaluation profit and loss |
| U-AAWOF | AA loan write-off |
| CONTDIFF | Contingent difference suspense |
| CONTSUSP | Contingent suspense |
| CUSDEBIT | Sight discount suspense |
| LDCANCEL | LD cancellations |
| NDFGIVEN | NDF given |
| NDFTAKEN | NDF taken |
| OFFLIMIT | Off balance sheet limit |
| RESFWDCR | Foreign exchange reserve – forward credit |
| RESFWDDR | Foreign exchange reserve – forward debit |
| SCCASUSP | SC corporate act suspense |
| SUSPENSE | Suspense |
| SUSPFXCR | Suspense credit FX |
| SUSPFXDR | Suspense debit FX |
| SUSPSCCR | Suspense securities credit |
| SUSPSCDR | Suspense securities debit |
| EXCHALFWD | Asset and liability forward revaluation |
| ICASUSPCR | ICA suspense credit accounting |
| ICASUSPDR | ICA suspense debit accounting |
| LCPARTACC | Syndicated LC part account category |
| MARKETING | MKT exchange |
| OFFSUSPCR | Non-utilisation fee credit |
| OFFSUSPDB | Non-utilisation fee debit |
| RESSWAPCR | Foreign exchange reserve - SWAP credit |
| RESSWAPDR | Foreign exchange reserve - SWAP debit |
| SUSPDEBIT | Suspense debit accounting |
| SUSPLMMCR | Suspense credit MM and LD |
| SUSPLMMDR | Suspense debit MM and LD |
| AASUSPENSE | Suspense for AA transactions |
| DIFFERENCE | Daily difference on data capture |
| INTERCO-IA | Inter branch - IA |
| INTERCO-IF | Inter branch - IF |
| SLROLLOVER | For SL rollover |
| SUSPCREDIT | Suspense credit accounting |
| SUSPDXCGCR | DX charge tax suspense credit |
| SUSPDXCGDR | DX charge tax suspense debit |
| SUSPDXIMCR | DX initial margin suspense credit |
| SUSPDXIMDR | DX initial margin suspense debit |
| SUSPDXMTCR | MTM suspense credit |
| SUSPDXMTDR | MTM suspense debit |
| SUSPDXOMCR | DX option variation margin suspense credit |
| SUSPDXOMDR | DX option variation margin suspense debit |
| SUSPDXPRCR | DX option premium suspense credit |
| SUSPDXPRDR | DX option premium suspense debit |
| SUSPDXRPCR | DX realised profit and loss suspense credit |
| SUSPDXRPDR | DX realised profit and loss suspense credit |
| SUSPDXVMCR | DX variation margin suspense credit |
| SUSPDXVMDR | DX variation margin suspense debit |
| SUSPFTBULK | Suspense for bulk FT or STO |
| SUSPFTINWD | Funds Transfer inward |
| U-AACAPTURE | AA take over charge |
| U-CLGSUSPCR | Inward clearing credit suspense |
| U-CLGSUSPDR | Inward clearing suspense |
| U-AASUSPENSE | Suspense for AA adjustments |

| Value | Description |
|---|---|
| 1 | When the Local Currency field value starts with BE (identifies Belgium). |
| 2 | When the Local Currency field value starts with LU (identifies Luxembourg). |
| 3 | For 10 digit account numbers with a modules 11 check. |
| 4 | For 11 digit account numbers constructed with a two digit bank number prefix defined in the Acc Bkno Prefix field , followed by seven identifying digits and a two digit mod 11 check digit. The prefix may contain leading zeros. |
| 5 | For a standard check, digit calculation with the account numbers zero filled to the Account Mask field. |
| 6 | For a 12-14 digit number with two check digits, the first 6 digits, and the second on the remaining digits. The check digits are calculated using mod 11. |
| 99 | No check digit calculation with the account number zero filled to the Account Mask field. |
| @routine name | Where a local subroutine performs the check digit calculation. |
| Blank | In all other cases. |


##### Business Events

When the Emit Business Event field in MS.PARAMETER is set as ‘Yes’, the business events representing the state change are emitted.

The following business events are emitted for Account Funds Authorization (ACFA) table.

| Business Event | Description |
|---|---|
| accounts.updatefundsAuthorization.fundsAuthorizationApproved | Event to be emitted when bank user approves funds authorisation for accounts |
| accounts.updatefundsAuthorization.fundsAuthorizationRejected | Event to be emitted when bank user rejects funds authorisation for accounts |
| deposits.updatefundsAuthorization.fundsAuthorizationApproved | Event to be emitted when bank user approves funds authorisation for deposits |
| deposits.updatefundsAuthorization.fundsAuthorizationRejected | Event to be emitted when bank user rejects funds authorisation for deposits |


##### Archival of Account and Related Tables

The closed account and the related data can be archived using the Transact Standard archival or Data Lifecycle Management (DLM) archival.

The DL module must be installed for the user to initiate the archival service to archive the closed account and the related data records to a Read-only (RO) database. Otherwise, the user moves the data records to the $ARC file using the Standard archival method. If the closed account crosses Retention Period (defined in ARCHIVE ), it is archived along with the related data. The retention period is calculated from the closure date of the account.

A sample screenshot of ARCHIVE for the ACCOUNT record is shown below.

When Retention Period ends and the user runs the archival service, the files mentioned in Arc Filename are archived.

> **⚠️ Note:** The user must set Archive Data as Y to archive the record. If the user sets it as N, the record is deleted instead of archiving, which results in loss of data.

Read Archiving for more details regarding Transact Standard archival process. Read Data Life Cycle Management for more details regarding DLM Archiving process.


##### Illustrating Model Parameters

This section covers the high-level specifications required for ACCOUNT .

| S.No. | Parameters | Description |
|---|---|---|
| 1. | ACCOUNT.PARAMETER | It has the information pertaining to cash flow, accounting method, generation of alternate identifier to account number, account level balance maintenance, netting and cheque issue management and so on. |
| 2. | CUSTOMER | To create a user account, the account holder should be registered as a customer in Temenos Transact . The information like name, address, age, residence, sector, language, industry, signature and so on, pertaining to the user is captured in the application. |
| 3. | CATEGORY | Based on the business needs, category codes defined in Temenos Transact has to classify financial transactions. Use of the codes together with personal customer characteristics enables the bank to produce balance sheets and returns reflecting a coordinated and structured view of its operation, by directing business transactions to their appropriate report. |
| 4. | CURRENCY | It allows the user to capture the operating currency of the account and it should be a record or value in the currency application. Account currency cannot be changed once the account is authorised as the balances are maintained in the currency. |
| 5. | ACCT.GEN.CONDITION | It allows the user to define the grouping condition for accounts for which the same conditions of interests and charges apply. Based on the business needs, category codes along with CUSTOMER attributes like Sector and Residence enable grouping of accounts. These attributes and their order of priority is defined in CONDITION.PRIORITY application for ACCOUNT record. |
| 6. | ACCT.GROUP.CONDITION | It allows the user to define the rules for accounts belonging to a group and specific currency mentioned in the table. Some examples for rules defined are Notice withdrawals, account violations, deferring interest and charges, rounding rules for interest and premium interest, automatic IBAN generation and so on. |
| 7. | ACCOUNT.DEBIT.INT | It allows the user to define special debit interest conditions when the corresponding group interest conditions are not suitable. The user can define Interest to be calculated on daily, average using value dated balance and interest rate to fixed or linked to basic rates. |
| 8. | ACCOUNT.CREDIT.INT | It allows the user to define special credit interest conditions when the corresponding group credit interest conditions are not suitable. Credit interest rates can be specified for different balance levels. Rates can apply to the entire balance or a part between the two-balance levels. |
| 9. | ACCT.CAPITALISATION | It allows the user to specify the next date and subsequent frequency of application of debit and credit interest capitalisation for a specific account. |
| 10. | GROUP.DEBIT.INT | It allows the user to specify the calculation method of debit interest for a group of accounts and provides the link to the GENERAL.CHARGE , where the charges applicable to the same groups of accounts are specified. The user can also specify negative interest and tax on interest. |
| 11. | GROUP.CREDIT.INT | It allows the user to specify the calculation method of credit interest for groups of accounts. The user can also specify second interest on the account with different capitalisation frequency. |
| 12. | GROUP.CAPITALISATION | It allows the user to specify the next date and subsequent frequency of application of debit and credit interest capitalisation for a group of accounts. |
| 13. | ACCOUNT.CLASS | It allows the user to define the account class records, which can be used by other Temenos Transact applications to construct account number or to check the account number for a particular group. |
| 14. | ACCOUNT.ACCRUAL | At company level, it provides the system with information on how and when to process accruals of interests and charges on customer accounts. Accrual process can be specified at Account Category and Account Group for which the associated interest accrual parameters are defined. |
| 15. | SAVINGS.PREMIUM | It enables the user to pay premium on the savings deposits if the savings account qualify the eligibility criteria defined in this table. |
| 16. | AC.FUNDS.DIVERSION.PARAM | The funds diversion is setup from the off-balance sheet Transaction Account to the on-balance sheet Diversion Account. The system provides flexible options that allows the bank to control the ability to suppress the funds diversion processing for specific transactions for Transaction accounts setup for funds diversion. The bank will be able to define the following options for funds diversion: The default funds diversion behaviour. To suppress Funds Diversion processing for specific activities by mentioning or defining the associated transactions code as an exception to the default rule. |
| 17. | ACSWIT.PARAMETER | This parameter table stores the validity period decided by the bank for the switch out service. The validity period can be defined in days or months. The ID of this record represents the Temenos Transact Company ID. |
| 18. | DDA.SERVICE.PARAMETER | This table helps the bank to decide whether the payment made by the account holder in a specific currency is allowed or not. Also, enables the Bank to change the core decision for Account Currency and to return the Payment Currency. |
| 19. | AC.ACCOUNTING.PARAM | This table helps to parameterise the accounting related processes based on the Max No Of Splits defined. |


##### Illustrating Model Products

Accounts are classified based on the financial transaction according to business needs. Some of the Account products available in Model bank are listed below.

| S.No. | Product Name | Product Attributes |
|---|---|---|
| 1. | Demand / Current Account | Current Account can be created using category code between 1000-1999 Feature of availing overdraft facility Mode of operation - single or joint Interest liquidation option |
| 2. | Savings Account | Savings account can be created using the category code ranging between 6000-6999 Regular SB accounts AA deposit accounts Overdraft facility Mode of operation - single or joint Interest liquidation option Alert subscription Mandate registration Passbook facility |
| 3. | Loan Accounts | Loan accounts can be created using the category code between 3000-3999 Islamic loan accounts AA loan accounts |


> **Related Applications:** `#PGM.AUTOM.ID`, `AC.SYS.CODES`, `ACCOUNT`, `ACCOUNT.CLASS`, `ACCOUNT.CREDIT.INT`, `ACCOUNT.DEBIT.INT`, `ACCOUNT.PARAMETER`, `ACCT.CAPITALISATION`, `ACCT.GEN.CONDITION`, `ACCT.GROUP.CONDITION`, `ARCHIVE`, `ARRANGEMENT ARCHITECTURE`, `AUTO.ID.START`, `CASH.FLOW.EXCEPTION`, `CATEGORY`, `COLLATERAL`, `COMPANY`, `CONDITION.PRIORITY`, `CURRENCY`, `CUSTOMER`, `Category`, `DATA CAPTURE`, `EB.CONTRACT.BALANCES`, `EB.OBJECT`, `FUNDS`, `FUNDS TRANSFER`, `GENERAL.CHARGE`, `GROUP.CAPITALISATION`, `GROUP.CREDIT.INT`, `GROUP.DEBIT.INT`, `LOANS AND DEPOSITS`, `MS.PARAMETER`, `SAVINGS.PREMIUM`, `SEC.TRADE`, `Sector`, `TELLER`, `TRANSFER`

---


### 2.2  Non-Stop Processing


> **📇 Quick Reference Card**
> 
> **Sections:** ⚙️ Configuration


#### ⚙️ Configuration

Financial transactions can happen any time round the clock. This document explains how Non-Stop (NS) processing is supported in Temenos Transact .

In NS mode, there is no restriction for:

- Modifying, reversing or deleting existing contracts
- Back values, forward values and so on.

There is no impact on transactions in unauthorised state (like INAU, RNA and so on) before the COB is initiated. Such contracts are automatically moved to HLD.

The non-stop processing functions for both new and existing contracts as explained below.


##### New Contracts Only

Core banking can enter, amend and authorise new contracts in this mode. However, back valued transactions are not allowed. The contracts unauthorised before the COB are moved to HLD during the COB process, but new contracts are not impacted.


##### New and Existing Contracts

Customer and contract balances are updated real time to ensure that the latest customer transaction is included. For Securities, the customer positions is updated real time.

Non-stop transactions do not impact financial closing position of the bank as:

- GL (CAL/CPL) include no movements from these transactions, which are included in the next COB
- Currency positions are updated to include the impact of cross-currency non-stop transactions, but the COB revaluation excludes the value of these transactions.

---


### 2.3  Chrg Acct Fees Chrgs on Limit


> **📇 Quick Reference Card**
> 
> **Purpose:** *When a LIMIT record is linked to an arrangement contract, the applicable fees and charges can be calculated at the level of a different (user defined) arrangement account instead of the contract level. To facilitate this, the LIMIT application allows linking an Arrangement Account to a LIMIT record ...*
> 
> **Key Fields:** *Charge Debit Account*, *Maintain Time Code Bal*, *Time Bal Eff Date*, *Time Code*, *Time Code Id*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

When a LIMIT record is linked to an arrangement contract, the applicable fees and charges can be calculated at the level of a different (user defined) arrangement account instead of the contract level. To facilitate this, the LIMIT application allows linking an Arrangement Account to a LIMIT record for calculation of fees and charges on either the zero time band or any other defined time band.

Balance Types for utilised limit amount, unutilised limit amount, original limit amount and overdraft limit amount will be posted to the linked AA account. Any fees and charges parametrised in Interest or Charge product conditions will be calculated on the level of this AA Account for the respective balance types.


#### ⚙️ Configuration

The Charge Debit Account field in LIMIT application must be configured with the appropriate arrangement account that is used for calculation of fees and charges along with the Time Code field to identify the time band.

The charge account can be either one of the AA Accounts that utilises the Limit, or a separate dedicated off-balance sheet account. For example, if a LIMIT record L1 is utilised by arrangements A1, A2 and A3, then the following options are available for setting up the charge account:

- Option 1 – One of the arrangements A1, A2 or A3 can be defined as the charge account.
- Option 2 – An additional user configured off-balance sheet AA Account can be used as the charge account.

Whenever a charge account is specified, the following fields in the LIMIT application will allow the user to input:

- Maintain Time Code Bal – This field indicates whether time code Limit balances are to be maintained based on the time code defined in the LI.TIME.CODE record. Available options are: No or Null – This is the default option. No balances are maintained for time band charge calculation. Yes – Balances are maintained based on time codes defined in the LI.TIME.CODE record. Once this field is set to Yes, Maintain Time Code Bal field becomes no input.
- Time Code Id – This field is part of the Time Code multi-value set of fields. It holds a valid LI.TIME.CODE record ID.
- Time Bal Eff Date – This is a no input field, which holds the date when Maintain Time Code Bal field is set to Yes.

When defining a time code in LI.TIME.CODE table, it is necessary to give an alpha or alphanumeric record ID and input a description together with a time code in number of days, as shown below:


#### 🔧 Working With

Once Limit products are created in the LIMIT.REFERENCE application, LIMIT records can also be created and a charge account can be linked to each of them. When the Limit is linked to a contract and when the contract is charged, all the relevant Limit balances are posted against the charge account specified in the LIMIT record and charges are being calculated.

Account arrangement with account reference 87394 is created as shown in the below screenshot:

In the LI.TIME.CODE table, two records are created, one for short-term time band (less than one year) and one for long-term time band (anything exceeding one year), as shown below:

When creating a LIMIT record, the above account can be attached to it as the charge account, Maintain Time Code Bal can be set to Yes and the Time Code Id for the short-term time band can be set to LESS.1Y:

Similarly, the long-term time band can be defined using the previously defined ‘ABOVE.1Y’ record from the LI.TIME.CODE application.

If the above Limit record is attached to a contract against which interest and charges are being calculated (such as a Personal Loan, for example) for utilised, unutilised or even original limit amount of either zero band, short-term or long-term time band, the system will post the respective limit balances against the account 87394 and calculate any charges on the level of this account:


#### 📋 Tasks

There are no Tasks available for Charge Account for Fees and Charges on Limit feature.


#### 📊 Outputs

There are no Outputs available for Charge Account for Fees and Charges on Limit feature.

---


### 2.4  Collateral Allocation to Limit


> **📇 Quick Reference Card**
> 
> **Purpose:** *The order to sort the collaterals to cover the liabilities of a customer, can be achieved by any one of the following setups:*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The order to sort the collaterals to cover the liabilities of a customer, can be achieved by any one of the following setups:

- Default collateral allocation process
- Collateral allocation priority by parameter setup
- Collateral allocation priority by manual setup

In the absence of any specific setup (either through parameter or manual), the system follows the default process of allocating collaterals to the liabilities of the customer.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

There are no Tasks available for Collateral Allocation to Limit feature.


#### 📊 Outputs

There are no Outputs available for Collateral Allocation to Limit feature.

---


### 2.5  Creating Cross Limits


> **📇 Quick Reference Card**
> 
> **Purpose:** *In this section, the reference to limits and limit references concern only the cross limit structure, unless specifically stated.*
> 
> **Key Fields:** *Cross Limit*, *Limit Band Level*, *Limit Percentage*, *Limit Subroutine*, *Maturity Period*, *Maturity Period Perc*, *Perc calc Basis*, *Percentage Cap* ... +5 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

In this section, the reference to limits and limit references concern only the cross limit structure, unless specifically stated.

A cross limit structure has three types of limit references:

- The PRODUCT limit references
- The CROSS limit references
- The SUB-PRODUCT limit references

The limit references that are used in a cross limit structure are different from those which are used in a normal limit structure.

> **⚠️ Note:** The three types of limit references or limits are specified in upper case in this document to distinguish their usage in a cross limit structure.

Cross limits provide a flexible limit structure with consolidation of limits at multiple levels, with the hierarchy of limits linked through the Record Parent field. It is possible to create more than one limit for a sub-product (with different sequence numbers) and attach them to the same PRODUCT or CROSS limit, which is not possible in case of normal limits.

More than one limit can be defined for a SUB-PRODUCT (under a PRODUCT or CROSS limit) to limit the exposure based on different conditions.

Under the

record 500101.1800.01, more than one limit can be defined for the SUB-PRODUCT 1860,

500101.1860.01 for customers 500101 and 500102 (both having liability customer 500101), and

500101.1860.02 for customers 500103 and 500104 (both having liability customer 500101).

This facility can also be used to define separate limits for a SUB-PRODUCT based on currency or company restrictions.

To limit the exposure in two different companies the following

(s) can be entered –

- 500101.1870.01 with restriction for use in first company and
- 500101.1870.02 with restriction for use in second company

Both companies have a Record Parent of 500101.1800.01.

When entering limits top to down, user must input only the PRODUCT or CROSS limits and Temenos Transact automatically creates or modifies the SUB-PRODUCT limits depending on the allowed products ( Product Allowed ) and customers, subject to some restrictions. SUB-PRODUCT limits can also be entered without entering the parent PRODUCT limits and Temenos Transact automatically creates the PRODUCT limits, which is transparent to the user.


#### ⚙️ Configuration

This section covers the configuration of product, cross and sub-product limit references.


##### Product Limit References

Since the processing and validations related to limits in a cross limit structure are different from those of the normal limits, it is necessary to distinguish at LIMIT.REFERENCE level, if a limit reference can be used in a cross limit structure. To use limit references in a cross limit structure, they must be specifically defined as explained below.

The PRODUCT limit references for cross limits are similar to that of normal limits, that is, ending with 00’s or 000’s and with a maximum of four digits.

In particular, a global limit reference (such as, 10000) cannot be used in a cross limit structure, or in a limit reference in a cross limit structure.


##### Cross Limit References

Any limit reference with a value greater than the PRODUCT limit reference and less or equal to the value of Top Cross Ref can be used as a CROSS limit reference. In the above example, LIMIT.REFERENCE IDs greater than 1100 and less or equal to 1140 can be used as CROSS limit references. However, when CROSS limits are input, Temenos Transact validates that they are entered only in ascending order. The above example validates that the first CROSS limit under a PRODUCT limit of 1001.1100.01 is 1001.1101.01, then 1001.1102.01, and so on.


##### Sub-product Limit References

Any LIMIT.REFERENCE ID with a value greater than the Top Cross Ref and whose ID matches with the PRODUCT limit reference (first digit in case of three digit limit references and first and second digits in case of four digit limit references) is used as a SUB-PRODUCT limit reference. In the above example, LIMIT.REFERENCE IDs greater than 1140 and less than 1200 can be used as limit references for SUB-PRODUCT limits under the PRODUCT limit reference of 1100.


##### Setting up Cross Limit Structure

1. The first step in setting a cross limit structure is creating the LIMIT.CROSS.PARAM record for the PRODUCT limit reference. A record must be entered for each PRODUCT limit reference in a cross limit structure in the LIMIT.CROSS.PARAM application.

In the following example, to use 1100 as a PRODUCT limit reference in a cross limit structure, a record with ID 1100 must be entered in the LIMIT.CROSS.PARAM application. LIMIT.REFERENCE record with ID in the range 1100-1199 must not be entered (or present), before the record with ID 1100 is entered in LIMIT.CROSS.PARAM application.

In this application, the Top Cross Ref field specifies the maximum value of a cross limit reference that can be used in the PRODUCT limit reference specified in the ID.

1. The next step is to enter the required SUB-PRODUCT LIMIT.REFERENCE records. When a SUB-PRODUCT LIMIT.REFERENCE record is entered, the Cross Limit field is automatically updated to PROD value. When a hierarchy of limits in a cross limits structure is linked through their record parents, value cannot be entered in Sub Product Level field.

1. Then, the PRODUCT limit reference record are entered and the SUB-PRODUCT limit references are attached to it using the Reference Child field. In case of a PRODUCT limit reference, the Cross Limit field is automatically updated as TOP.

1. Then, the required CROSS limit reference records are entered. Since a CROSS limit reference is a consolidating limit reference similar to a PRODUCT limit reference, values cannot be entered in the following fields: Limit Percentage Limit Band Level Maturity Period Maturity Period Perc Limit Subroutine Percentage Cap Percentage Floor Perc calc Basis

In case of a CROSS limit reference, the Cross Limit field is automatically updated as CROSS.

1. Finally, in LIMIT.PARAMETER , the SUB-PRODUCT limit references are set up as limit products in the Product No field.


#### 📋 Tasks

There are no Tasks available for Creating Cross Limits feature.


#### 📊 Outputs

There are no Outputs available for Creating Cross Limits feature.

---


### 2.6  Creating Customer Liability Structure


> **📇 Quick Reference Card**
> 
> **Purpose:** *This functionality allows users to define a Customer Liability structure by using the functionality of a Customer Group.*
> 
> **Key Fields:** *Customer Number*, *Group Purpose*, *Key Type*, *Liability Customer*, *Liability No.*, *Limit Product*, *Limit Type*, *Risk Group Id*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

This functionality allows users to define a Customer Liability structure by using the functionality of a Customer Group.

This gives all the benefits that CUSTOMER.GROUP application offers, to the Liability Group as well. The bank can maintain Party Relationships, using a designated Liability Relation. Also, existing validations which allow customers to be part of only one risk group are applicable for Liability Group.

Limit Banking Capability supports creating customer group and its purpose and fetching its details through API. It also emits events for creating and updating the activities of customer group. Customer group is created with the Party and its relation details supplied directly in the API so Limit TBC does not support importing party relationship.


#### ⚙️ Configuration

This functionality allows users to define a Customer Liability Structure using the CUSTOMER.GROUP application. To enable this functionality, user must select the ‘Liability’ option in the Group Purpose field in the CUSTOMER.GROUP application when creating a customer group. The user can also define the lead customer of the Customer Liability group by entering the respective customer number in the Liability Customer field in CUSTOMER.GROUP .

The Liability Customer field in the LIMIT application can now be used to specify the customer group ID, which has been defined with Group Type = ‘Liability’. This indicates that the given Limit structure is part of the Customer Liability Structure.

To create a Customer Liability structure, a new record must be defined in the CUST.GROUP.PURPOSE parametrisation table.

This allows users to create Customer Group records with Group Type = Liability. To define Limit records that are part of the Customer Liability structure, the Limit Type field must be blank and the Key Type field must be set to Txn Ref in Limit Products.

For example, the user can set a child Limit Product in the LIMIT.REFERENCE application as shown in the below screenshot.

The corresponding parent Limit Product is shown below.


#### 🔧 Working With

This section explains how to create a Customer Liability structure with an example.

The following image shows an example of Limit Product setup.

After parametrisation is done in the CUST.GROUP.PURPOSE table, the user can create a Customer Group in CUSTOMER.GROUP application with the Group Purpose field set to LIABILITY and a valid customer ID set in the Liability Customer field.

After parametrisation is done in the LIMIT.REFERENCE application, the user can create limit records in the LIMIT application with the above Customer Group ID set in both the Risk Group Id and Liability No. fields.

For example, the user can define the top-level Limit record (which constitutes the overall Limit Product cap) by setting both the Risk Group Id and Liability No. fields to CUSTLIB29, the Limit Product field to 5400 and leaving the Customer Number field blank.

The user can then define the lower-level Limit record (which constitutes the Limit Sub-Product cap) by setting both the Risk Group Id and Liability No. fields to CUSTLIB29, the Limit Product field to 5401 and leaving the Customer Number field blank.

After this, the user can also set Limit records for customers. For example, the user can define a Limit record, which constitutes the Limit Product cap for a given customer, by setting both the Risk Group Id and Liability No. fields to CUSTLIB29, the Limit Product field to 5400 and the Customer Number field to 148968.

Finally, the user can define the lowest level Limit record, which constitutes the Limit Sub-Product cap for a given customer, by setting both the Risk Group Id and Liability No. fields to CUSTLIB29, the Limit Product field to 5401 and the Customer Number field to 148968.

It is the lowest level of the structure that gets linked to a contract. The difference between this type of Limit structure and the utilisation/validation Limit structure is that the Limit check is performed from the bottom way up across all levels of the structure, not just the lowest one.


#### 📋 Tasks

There are no Tasks available for Creating Customer Liability Structure feature.


#### 📊 Outputs

There are no Outputs available for Creating Customer Liability Structure feature.

---


### 2.7  Creating Limit Products


> **📇 Quick Reference Card**
> 
> **Purpose:** *A Limit (LI) product is an area of business for which the bank creates line of credit. LI products are defined in the LIMIT.REFERENCE application and are linked to the underlying business using the LIMIT.PARAMETER application. The Limit Type field in the LIMIT.REFERENCE application allows users to c...*
> 
> **Key Fields:** *Collateral Code*, *Currency*, *Internal Amount*, *Liability Number*, *Limit Mnemonic*, *Limit Product*, *Product Allowed*, *Rejection Reason*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

A Limit (LI) product is an area of business for which the bank creates line of credit. LI products are defined in the LIMIT.REFERENCE application and are linked to the underlying business using the LIMIT.PARAMETER application. The Limit Type field in the LIMIT.REFERENCE application allows users to create the following types of Limit records:

- Utilisation
- Validation
- Standalone

The Standalone option allows the user to link Limit records to Club Loan Facility arrangements. The LIMIT.REFERENCE application allows users to also suppress accounting to avoid double accounting entries for Limits linked to Club Loan Facility arrangements and mark the exposure created against these limits as belonging to a third-party financial institution instead of the bank’s own exposure.


#### ⚙️ Configuration

This section covers configuring limit products and linking them to underlying business.


##### Configuring Limit Products

The LIMIT.REFERENCE application links various limit products to the business application. The ID to this application is the product, defining the product hierarchy which is the second dimension to limits.

Each limit product ( LIMIT.REFERENCE within the system) can be defined as being part of a hierarchy and consists of a

- Global limit
- Product limit
- Sub-product limit

Global limits and their products must be defined in this application.

This application is also used for defining if the LIMIT.REFERENCE requires checking each time, or it is updated for information purposes only.

The Margin Level field represents the percentage ratio between the limit amount utilised by underlying transactions and the value of the collateral available for the limit.

Potential values associated with the Margin Event field are defined by setting up the EB.LOOKUP application with records prefixed with ID LI.MARGIN.EVENT * .


##### Limit Reference ID Change

The LIMIT.REFERENCE application supports alphanumeric key as its record ID. This alphanumeric key allows the creation of an unlimited number of limit product levels within the same structure.

The top-level holds a Validation Limit product, but its underlying Utilisation Limit products can go up to as many levels as the user needs, with a Utilisation Limit product being a parent of another Utilisation Limit product, regardless if it is a part of a shared structure or not.

For example, when creating a new Limit product, the user can enter any alphanumeric ID.

The Limit Mnemonic field supports up to 12 alphanumeric characters. It is defaulted to the LIMIT.REFERENCE record ID, if left blank when validating or committing the record.

User must follow the below steps to create the Limit product structure with alphanumeric ID.

1. First, the lowest level of the limit product structure must be created. Utilisation Limit product 5EDGHU765RE created for study loans. Utilisation Limit product 90SDF3IVS49X is created for car loans. Utilisation Limit product KD034JG0WRL4 for short term loans can be created as a parent for previously created study loans and car loans. Similarly, Utilisation Limit product 9DR56JV3OB81 is created for mortgage loans. Utilisation Limit product LSN435SDV02W is created for construction loans. Utilisation Limit product LF09362VKXTH for long term loans can be created as a parent for previously created mortgage loans and construction loans.
2. After all the Utilisation Limit products have been created, the top-level parent Validation Limit product can be created.
3. After all the Limit products are created and the lowest level products are parametrised accordingly in LIMIT.PARAMETER application, actual limit records can be created and the lowest level of the structure can be linked to contracts or accounts.


##### Linking Limit Products to Underlying Business

The limit products valid for a particular contract or account are defined in the LIMIT.PARAMETER application. As limit products are user-defined (on LIMIT.REFERENCE ), the process of linking contracts and accounts to these products also need to be user-defined. It is based upon any characteristic of the contract or account including the local reference fields (if required).

The parameter defines the limit products that are valid for a contract or account. If input is not made the limit product is defaulted. The following screenshot shows the limit parameter structure.

The following screenshot shows the LIMIT.PARAMETER section applicable to the MM.MONEY.MARKET (MM) application. If an MM contract has a Category of 21077, then the valid limit product ( Product No ) is 3020.

Two limit products are valid for loans:

- A secured loan
- An unsecured loan

The user must distinguish between the two when the loan is entered. If no distinction is made, then Temenos Transact applies a default of the first applicable product.

If the loan does not meet any of the above criteria, then the limit product corresponding to the ‘parent’ product is used. Temenos Transact insists that there is always a default specification for each application being used. It can appear anywhere on LIMIT.PARAMETER . All other specifications for the application are checked in the LIMIT.PARAMETER record. When a match is found, the checking stops.


##### Configuring Standalone Limit Products

Before creating standalone Limit records, the user must first create a Limit product.

5954 and 5955 are standalone Limit products.

- 5955 is for standalone Limits which hold bank’s exposure. So, the Third Party Exposure and (for demonstration purposes) the Suppress Accounting fields are set to No:
- 5954 is for standalone Limits that do not hold bank’s exposure. So, the Third Party Exposure and Suppress Accounting fields are set to Yes:


#### 📋 Tasks

Related topics:

- Set Up Limit (Corporate)
- Maintain or Reverse Limit (Corporate)
- Lending Processes (Corporate)

Limit product is an area of business for which the bank creates line of credit. Limit (LI) products are defined in the LIMIT.REFERENCE application and are linked to the underlying business by using the LIMIT.PARAMETER application.


##### Workflow

This section helps the user to perform the below tasks:

| SCREENS | WORKFLOW |
|---|---|
|  | Maintain/Reverse Limit . |
| Maintain/Reverse Limits | Click the Amend icon of a corresponding record. The system opens the record to amend. |
| Maintain Limit | Enter or modify the field values that require amendment. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

| SCREENS | WORKFLOW |
|---|---|
|  | Secured Limit . |
| Contract Screen | Click the New icon. |
| Secured Limit | Enter values in the following fields: Currency Liability Number Limit Product Internal Amount Product Allowed Collateral Code Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

| SCREENS | WORKFLOW |
|---|---|
|  | Limit . |
| Unauthorised Limits | Click the Authorise icon of a corresponding record. The system opens the record to be authorised. |
| Limit | Click the Authorise icon. |


#### 📊 Outputs

There are no Outputs available for Creating Limit Products feature.

---


### 2.8  Credit Checking


> **📇 Quick Reference Card**
> 
> **Purpose:** *A credit check is made whenever a debit transaction is*
> 
> **Key Fields:** *Credit Check*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

A credit check is made whenever a debit transaction is

- Validated (or)
- Validated and authorised at the same time

Credit checking for an account is set against working balance and cash flows or available balance using the Credit Check field in ACCOUNT.PARAMETER application. Read the Accounts User Guide for more details regarding credit checking.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

There are no Tasks available for Credit Checking feature.


#### 📊 Outputs

There are no Outputs available for Credit Checking feature.

---


### 2.9  Credit Limits


> **📇 Quick Reference Card**
> 
> **Purpose:** *A limit can be recorded against any customer using the LIMIT application. A simple limit ID consists of three components which are:*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

A limit can be recorded against any customer using the LIMIT application. A simple limit ID consists of three components which are:

- The ID of the customer (in CUSTOMER application) to whom the credit line is available.
- The product of the limit which is the type of business products that can utilise this limit.
- A serial number enabling more than one limit of the same type to be maintained for a customer.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

There are no Tasks available for Credit Limits feature.


#### 📊 Outputs

Limits indicate the assessed range within which the company can disburse credit products to the customer based on the due diligence done by the user on the risk capacity of the customer.


##### Enquiries and Reports

The user can view the below list of enquiries and reports pertaining to collateral and limits in the core banking system.

Customer Position Summary

This enquiry displays the details of all the contracts available for a customer.

LIAB Enquiry

This enquiry displays the details of all the liability products opted by a customer.

Collateral Right Review

This enquiry displays the details of various collateral issued by the customer and exposed to the company.

Credit lines expired

This enquiry displays the details of expired limits of the customer.

Credit lines to be Reveiwed

This enquiry displays the details of customer’s limits to be revisited by the user.

Liablity Amendments

This enquiry displays the details of old and new limits for a customer.

Limit & collateral Excess

This enquiry displays the details of the value above customer’s usage of credit products.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


### 2.10  Cus Rsk Grp For Mt Jt Cus Lim


> **📇 Quick Reference Card**
> 
> **Purpose:** *The banks can have multi-customer Limit products, with or without joint liability, where the applicants to a multi-customer limit need not be part of credit risk group. The Temenos Transact Limit module provides the flexibility that enables the user to configure rules for credit risk group based on ...*
> 
> **Key Fields:** *Allow Mult Group*, *Def Joint*, *Def Risk Group Mand*, *Joint*, *Multi*, *Risk Group Mand*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The banks can have multi-customer Limit products, with or without joint liability, where the applicants to a multi-customer limit need not be part of credit risk group. The Temenos Transact Limit module provides the flexibility that enables the user to configure rules for credit risk group based on the customer segment (that is, private individuals, corporate, sole traders and so on).

The joint or multi-customer limits can be created in the following combinations for applicants in the Household customer segment:

- If the joint applicants are not part of any credit risk group.
- If one of the joint applicants is part of a credit risk group while the other is not part of any credit risk group.
- If the joint applicants are part of different credit risk groups.
- If the joint applicants are part of different credit risk groups and the groups are merged by the bank, if required. After the merger, the groups become part of the same credit risk group.

The joint or multi-customer limits can be created in the following combinations for applicants in Corporate customer segment:

- If the joint applicants are part of the same credit risk group.
- If the joint applicants are part of different credit risk groups and the groups are merged by the bank, if required. After the merger, the groups become part of the same credit risk group.


#### ⚙️ Configuration

The rules for multi-customer limits are configured in the LI.MULTI.CUSTOMER.LIMIT.PARAMETER application. The bank can configure the following rules in this parameter table, which has only one record (SYSTEM):

The bank can configure the following rules in this parameter table, which has only one record (SYSTEM):

- The default pre-condition for mandatory risk group
- Applicability of the default rules, that is, whether it is applicable to multi, joint or both
- Whether joint applicants to the limit can be part of different risk groups
- The customer segment specific, that is, segments for which rules differ from the default pre-condition
- Applicability of the segment-specific rules like: If the risk group is mandatory If it is applicable to multi, joint or both If the joint applicants to the limit can be part of different risk groups for the segment-specific rule

The following fields in the parameter table are used to configure the rules for multi-customer limits:

The following screenshot shows the fields that are used together to define the default rule that is applicable to the multi or joint customer limits system-wide:

The following screenshot shows the fields that are used together to define the segment-specific rule that is applicable to the multi or joint customer limits for applicants belonging to the specific customer segment:


#### 🔧 Working With

For multi and joint customer Limit, the system will configure rules for credit risk group based on the customer segment.

The bank may configure the below rules:

- Multi-Customer limit with joint liability for corporate customer segment, here the joint applicants should be part of the same credit risk group.
- Multi-Customer limit with joint liability for household customer segment, here the joint applicants need not be part of the credit risk group.

This can be achieved by configuring the LI.MULTI.CUSTOMER.LIMIT.PARAMETER application as shown in the screenshot below.

In this configuration, the default rule for multi-customer limit, with or without joint liability, is not to have mandatory credit risk group, hence the Def Risk Group Mand field is set as No. However, for Corporate customer segment (represented by sector 2001), the credit risk group is mandatory for multi or joint customer limits and the co-applicants should be part of the same credit risk group, hence the Risk Group Mand field is set as Yes and Allow Mult Group field is set as No. When a multi or joint customer limit is created and if the applicant customers fall in the household sector, the system will allow the creation of the limit even if the applicant customers are not part of any credit risk group.

When a multi or Joint customer limit is created and the applicant customers fall in the corporate sector (that is, sector 2001), the system will allow the creation of the limit only if the co-applicants are part of the same credit risk group. If the co-applicants are not part of the same credit risk group, an override message will be prompted and will not allow the creation of the multi or joint customer limit.

It is also possible to define separate rules for multi-customer limits with joint liability and multi-customer limits without joint liability. This can be achieved by choosing the appropriate option in the Def Joint or Multi field (for default rules) and Joint or Multi field (for segment-specific rules). If the rule is applicable for both, ‘Both’ option can be used. The rules configured can be modified. The amendment or modification to the rules are applied only on the new multi-customer (with or without joint liability) limits created after the amendment.


#### 📋 Tasks

There are no Tasks available for Customer Risk Group Rules for Multi or Joint Customer Limit feature.


#### 📊 Outputs

There are no Outputs available for Customer Risk Group Rules for Multi or Joint Customer Limit feature.

---


### 2.11  Customer Grouping


> **📇 Quick Reference Card**
> 
> **Purpose:** *A single credit limit can be given to a single customer or to a group of customers. The most common example is when the bank has a business relationship with various companies within a group. In this case, bank wishes to manage its credit risk exposure to the entire group. This is achieved using the...*
> 
> **Key Fields:** *Define Priority*, *GRP.CREDIT.LIMIT*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

A single credit limit can be given to a single customer or to a group of customers. The most common example is when the bank has a business relationship with various companies within a group. In this case, bank wishes to manage its credit risk exposure to the entire group. This is achieved using the Customer Liability Number.


#### ⚙️ Configuration

To manage the exposure for a group of customers, the following must be done:

1. One member of the group of customers must be identified as the lead customer. This usually is the head office of the group of companies.
2. Then, the Customer Liability field on all the CUSTOMER records must be set to the number of this lead customer.
3. The Customer Liability field must also be defined for the lead customer by linking itself in this field.

> **⚠️ Note:** Once the customer records are committed and approved, the Customer Liability field cannot be amended using the customer record. Changes to the Customer Liability can only be processed and updated during the Temenos Transact overnight batch using the LIMIT.CHANGE application.

The following image shows an example for structure of customer grouping:

In the above example, the Liability No is 100094, which is the Customer No of the head office. Then, limits are granted to this liability number in exactly the same way as the bank grants the limit to a single customer in the previous example.


#### 📋 Tasks

Related topics:

- Lending Processes (Corporate)

A limit can be recorded against any customer by using the LIMIT application. A single credit limit can be given to a single customer or to a group of customers. Customer Grouping helps the financial institution to reduce the risk of exposure by creating the customer group for the related customers and assign the single limit to it.


##### Workflow

This section allows the user to perform the below tasks:

| SCREENS | WORKFLOW |
|---|---|
|  | Create Limit Group . |
| Contract Screen | Click the NEW icon. |
| Create Group | Enter values in the following fields: Description Allowed Customer Allowed Product Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

| SCREENS | WORKFLOW |
|---|---|
|  | Define Limit Priority . |
| Contract Screen | Enter or select a value in the Define Priority field and click the Edit icon. |
| Create Group | In the Input tab, enter values in the following fields: Group Priority Customer Priority Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to Customer Grouping in the core banking system.


##### Enquiries and Reports

This section allows the user to view the below list of enquiries and reports:

Customer Group Details

This enquiry displays the list of customers and their linked Limit Sharing Group respectively.

Limit Sub Group Details

This enquiry displays the list of main groups and the sub groups linked to Limit Sharing Group.

Master Group Details .

This enquiry displays the list of Master Group ID, Group Customer and details of the customer priority.


##### SWIFT

NA


##### Advices

NA


##### Alerts

NA

---


### 2.12  Customer Sub-Group in Risk Exposure


> **📇 Quick Reference Card**
> 
> **Purpose:** *This feature enables the end-user can check the limit risk exposure for targeted customers using the customer sub-group. If a customer group has 100 customers with multiple sub-groups, a particular customer’s limit exposure level can be viewed using the customer sub group.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

This feature enables the end-user can check the limit risk exposure for targeted customers using the customer sub-group. If a customer group has 100 customers with multiple sub-groups, a particular customer’s limit exposure level can be viewed using the customer sub group.

In addition, the user can amend the first customer in limit and the consolidation key is updated accordingly. User can also view the customer group in limit risk exposure without creating a limit record for the customer.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

Customer sub-group feature helps the user to check the limit risk exposure for targeted customers who are part of the customer group. For example, if a customer group has 100 customers with multiple sub-groups, a particular customer’s limit exposure level can be viewed using the customer sub group.

The Risk and Exposure Overview (CUSTOMER.SCV.CHECK) enquiry helps to view exposure details of the given customer or customer group. This enquiry displays single customer view or customer group view based on the selection input provided.


##### Workflow

This section helps the user to perform the below tasks:

| SCREENS | WORKFLOW |
|---|---|
|  | View Sub Group . Displays the Customer Sub Group details based on the input. |
| LI Sub Group | Click the Risk Exposure icon of a corresponding record. Displays the list of exposures available for the Customer/Group. |
| Sub Group Customer Limit Exposure | Click the Amend Limit Details icon of a corresponding record. |
| Ac Pre Closure Details Input | In the selected Limit Record, capture the details to be amended. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |


#### 📊 Outputs

The customer sub-group feature helps the user to check the limit risk exposure for targeted customers who are part of the customer group. For example, if a customer group has 100 customers with multiple sub-groups, a particular customer’s limit exposure level can be viewed using the customer sub group.

The Risk and Exposure Overview (CUSTOMER.SCV.CHECK) enquiry helps to view exposure details of the given customer or customer group. It displays single customer view or customer group view based on the input provided.


##### Enquiries and Reports

This section allows the user to view the below enquiries and reports:

View Sub Group

This enquiry helps the user to view the sub-group limit exposure, amend the limit details, and limit transaction or account details.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


### 2.13  Externalise Transact Limit Exposure


> **📇 Quick Reference Card**
> 
> **Purpose:** *Banks using Transact for credit limits and managing contracts and exposures in an external system, can capture exposure from an external system into Transact. Externalising Transact Limit Exposure enables Transact to store the external contract or exposure details, allowing the corresponding externa...*
> 
> **Applications:** `CATEGORY`, `EB.PRODUCT`, `LI.EXTERNAL.CONTRACT`, `LI.EXTERNAL.TRANSACTION`, `LI.EXTERNAL.TRANSACTIONS`, `LIMIT`, `LIMIT.DAILY.OS`, `LIMIT.PARAMETER` ... +2 more
> 
> **Key Fields:** *ADDITIONAL.DETAILS.LABLE*, *ADDITIONAL.DETAILS.VALUE*, *ALLOW.EXTERNAL.ONLY*, *Account
 Officer*, *Allow External Only*, *Allow external*, *Applicatio*, *Application* ... +39 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Banks using Transact for credit limits and managing contracts and exposures in an external system, can capture exposure from an external system into Transact. Externalising Transact Limit Exposure enables Transact to store the external contract or exposure details, allowing the corresponding external system contract or exposure to utilise the limits created in Transact.

> **⚠️ Note:** The LIMEXT product license enables the bank to use this functionality.


#### ⚙️ Configuration

Configure the ALLOW.EXTERNAL.ONLY field in the LIMIT.REFERENCE application to allow the limit to be utilized only by external exposure.

- When the Allow External Only flag is set as ‘Yes’ in the limit product, the exposure is allowed only from an external system and the child limit products can have exposures only from an external system.
- When the Allow External Only flag is set as ‘No’ or ‘Null’ in the limit product, the exposure is allowed from both internal and external systems. The child limit products can also have exposures from both internal and external systems.

External contract details are captured in the LI.EXTERNAL.CONTRACT application. The limit products configured by setting the Allow External Only flag as "Yes", can only be defined for linking to the external exposures captured through LI.EXTERNAL.CONTRACT . Hence, for such products, the Application field in LIMIT.PARAMETER can only be defined as LI.EXTERNAL.CONTRACT .

The user can link the limit products that allow the utilisation of both internal and external exposures to other Transact business applications as well as the LI.EXTERNAL.CONTRACT application.


##### Configuring Parameter for External Forex

Forex deals maintained externally can be captured in Transact using LI.EXTERNAL.TRANSACTIONS . To link the external system with limit products in Transact, the following configuration is required in LIMIT.PARAMETER .

- To link the external Forex deals to the appropriate limit product, the user can define LI.EXTERNAL.TRANSACTIONS in the Applicatio n field or as record ID itself and, the related Limit Product can be defined in the Product No field.
- Only the Limit Product with the Fx Or Timeband field set as FX can be linked to LI.EXTERNAL.TRANSACTIONS in LIMIT.PARAMETER .


#### 🔧 Working With

Exposures from an external system can utilise the limit created in the Transact system. The LI.EXTERNAL.CONTRACT application in Transact captures and maintains the details of the external exposures, facilitating the utilization of limits, by linking them to the appropriate limit lines. The Risk Exposure Overview report enables the user to monitor such exposure details in the Transact system. The LI.EXTERNAL.TRANSACTION application captures and monitors the movements on the external exposure.

The Transact Limit System allows linking the external exposures with both shared and non-shared limit structures.

The following steps illustrate the process flow required to link the external contracts or exposures to the limits in Transact.

Linking of external contract or exposures involves creation of the Limit product, attaching it to the required business applications through the limit parameter, creation of limit, followed by linking of limit while capturing the static details of contracts and finally capturing the transaction movements to update the credit exposure against the limit within Transact.

1. Create a limit product using the LIMIT.REFERENCE application exclusively for updating the exposure of external contracts by setting Allow External only as Yes.
2. Link the limit with the contract from the external business application, limit product created exclusively for external exposure must be linked with the Transact’s business application namey LI.EXTERNAL.CONTRACT using the LIMIT.PARAMETER application. The screenshot below shows the limit product created in step1 linked to the business application.
3. Post linking the limit product to the business application, create the limit using the limit product created for external exposure. Linking of limit with external contract through LI.EXTERNAL.CONTRACT is continued under capturing external exposure.


##### Capturing External Exposure

The LI.EXTERNAL.CONTRACT application stores the contract or exposure details from the external system. This application can be updated manually by the bank user or through an API call from the external system. The below table lists some of the important fields in the LI.EXTERNAL.CONTRACT application used to record the contract details.

| Field Name | Description |
|---|---|
| EXTERNAL.CONTRACT.ID | Indicates the unique identifier |
| CONTRACT.APPLICATION | Indicates the name of the application where the contract is initiated |
| CONTRACT.ID | Indicates the contract ID from the external system |
| CURRENCY | Indicates the currency of the contract |
| START.DATE | Indicates the start date or value date of the contract |
| MATURITY.DATE | Indicates the maturity date of the contract |
| BOOKING.DATE | Indicates the date in which the contract is booked in the source system |
| CATEGORY | Indicates the product category of the contract. It should be a valid record from the CATEGORY application. |
| CUSTOMER.IDS | Indicates the customer of the contract. If there are multiple customers defined, the primary customer is identified based on the value of the associative REPORTING.CUSTOMER field. If the REPORTING.CUSTOMER field is set as ‘Yes’, the respective customer is treated as primary customer for the contract. |
| REPORTING.CUSTOMER | Indicates whether the customer (mentioned in the CUSTOMER.IDS field) is a reporting customer (YES) or not. If there are multiple customers defined for the contract, the primary customer is identified with the help of this field. |
| LIMIT.ID | Indicates the limit ID to which the contract is linked. |
| LIMIT.PRODUCT | Indicates the limit product ID linked to the contract. It should be a valid record from the LIMIT.REFERENCE application. |
| SYSTEM.ID | Indicates the module ID of the application, if the contract is originated from Standalone Transact System. It should be a valid record from the EB.PRODUCT application. |
| SOURCE.SYSTEM | Indicates the identifier of the source system from where the contract is initiated. |
| ADDITIONAL.DETAILS.LABLE | Allows the user to map additional field name from external application through which the data can be sent to Transact Limit System. |
| ADDITIONAL.DETAILS.VALUE | Allows the user to map the additional field value from external application through which data can be sent to Transact Limit System. |

The LIMIT.ID field in LI.EXTERNAL.CONTRACT is used to link the limit created in the Transact system to an external exposure. The LIMIT.TXNS table is used to maintain the utilisation of the exposures (internal and external).

The Transact system emits the following business events for the updates on the LI.EXTERNAL.CONTRACT application, that can be consumed by the external system for further processing.

| Event Name | Description |
|---|---|
| creditLimits.updateContractTerm.contractTermUpdated | Indicates the change in contract terms |
| creditLimits.updateContractProperties.contractDetailsUpdated | Indicates the change in properties of the contract |
| creditLimits.updateContractOwners.contractOwnersUpdated | Indicates the change in the owner of the contract |
| creditLimits.updateContractLimit.contractLimitUpdated | Indicates the change in the limit of the contract |
| creditLimits.recordContractLink.contractRecorded | Indicates the contract linkage with the limit |
| creditLimits.recordContractClosure.contractClosed | Indicates the closure of the limit |
| creditLimits.delinkContract.contractDelinked | Indicates the delinked contract from the limit |

In continuation to the limit product creation for external exposure and linking the limit product to business application, the below process explains how an external business application can invoke the createLimitContractLink API and update the static details of the contract by linking the limit. The system processes the API request and creates a new record in the LI.EXTERNAL.CONTRACT application.

The external system sends a request to Transact to create a contract association with the credit limit with all the static information such as contract type, reference, maturity, customers, and system details. The below screenshot shows the static details of the contract along with the limit ID to be linked to the contract passed as an API request to Transact .

On receiving the API request, Transact creates a record in the LI.EXTERNAL.CONTRACT application. This establishes a link between the contract from the external business application and the credit limit. During this process, the system validates if the contract is applicable to be linked against specified limit based on rules defined for the credit line product in limit parameter. The screenshot below shows the record created in LI.EXTERNAL.CONTRACT as a result of the API request from the external system.


##### Capturing Movements on External Exposures

Banks can manually record the exposure movements in the LI.EXTERNAL.TRANSACTIONS application or through an API call based on the request from the external system.

- When Transact receives any API or manual request for utilisation of limits from the external system, it validates the details of the contract and its respective limit details in LI.EXTERNAL.CONTRACT to allow utilisation.
- The Commitment Contract and Drawing Contract fields in LI.EXTERNAL.TRANSACTIONS help to indicate whether the request received from the external system is for commitment only update or for drawing transaction.
- Whenever there is a utilisation of the limit through LI.EXTERNAL.TRANSACTIONS (both commitment and drawing update), both LIMIT.TXNS and LIMIT are updated with the exposure details.
- The below event gets emitted from Transact after a successful exposure update. Event Name Description creditLimits.updateExposure.exposureUpdated Indicates the updation of exposure details

The below table lists some of the important fields from the LI.EXTERNAL.TRANSACTIONS application that gets updated while recording the exposure details.

| Field Name | Description |
|---|---|
| LIMIT.ID | Contains the Limit ID to which the contract is linked |
| TRANSACTION.APPLICATION | Contains the name of the application from where the transaction is initiated |
| TRANSACTION.REFERENCE | Contains the transaction reference |
| CONTRACT.ID | Contains the contract ID for which the transaction is initiated. It should be the ID of the LI.EXTERNAL.CONTRACT application. |
| CONTRACT.COMPANY | Contains the company in which the contract resides |
| TRANSACTION.CURRENCY | Contains the currency in which the transaction is initiated from the source system |
| TRANSACTION.AMOUNT | Contains the exposure amount to be updated as part of the transaction from the source system |
| CR.DR.MARKER | Indicates the sign of the transaction based on which the exposure is debited or credited |
| COMMITMENT.CONTRACT | Flag to indicate whether the contract is to update commitment only |
| DRAWING.CONTRACT | Flag to indicate the drawing transaction. When a commitment is not set, it is taken as a ‘yes’, by default. |
| DELETE.REASON | Contains the reason of deleting the exposure passed from the source system |

In continuation to linking of external contract to the Transact limit through LI.EXTERNAL.CONTRACT , the process below explains the capturing of exposures or movements of the external contract against the credit limit linked. The external system invokes the createLimitTransactions API with the movement details to be updated in the limit. Transact processes the request and creates a record in LI.EXTERNAL.TRANSACTIONS application.

The external system sends a request to store the movements on credit limit. The screenshots below show the details captured such as transaction reference, amount, value date, revolving nature of contract and credit or debit indicator for contracts upon commitment or utilisation or repayment of credit limit.

On receiving the request, the system creates a record in the LI.EXTERNAL.TRANSACTIONS application in Unauthorised state.

> **⚠️ Note:** Setting the Commitment Contract flag as Yes indicates that exposure update is requested for the commitment portion of the contract, whereas setting the Drawing Contract flag as Yes indicates the exposure update is requested for the utilisation of the available balance of limit.

As the Drawing Contract flag is set as Yes, post receiving the transaction details from external system through API and creation of new record in LI.EXTERNAL.TRANSACTIONS , the system updates the respective Limit record outstanding and available amount. The LIMIT.TXNS application also gets updated with the details of transaction movement.

The newly created record in LI.EXTERNAL.TRANSACTIONS application is in Unauthorised state and hence the external system can send a request again to Transact for authorisation.


##### Linking Transact Limit to External Forex Exposure

The Forex deals created and maintained in an external system can be linked to the Transact limit to monitor the risk exposure of the Forex deal by capturing the relevant details of the external Forex deal and in the LI.EXTERNAL.TRANSACTIONS application, through the API framework.

The below table lists some of the relevant fields from the LI.EXTERNAL.TRANSACTIONS application, where the Forex exposure details are captured and stored.

| Field Name | Description |
|---|---|
| Category | Indicates the category code of the deal |
| Currency Market | Indicates the currency market corresponding to the contract. |
| Customer Id | Indicates the counterparty ID |
| Account Officer | Indicates the treasury department officer for the deal |
| Limit Product | Indicates the limit product linked to the deal |
| Limit Id | Indicates the Limit that will be linked to the FX deal |
| Transaction Currency | Indicates the bought currency |
| Transaction Amount | Indicates the bought currency original amount |
| Fx Other Currency | Indicates the sold currency |
| Fx Other Amount | Indicates the sold currency amount |
| Booking Date | Indicates the Forex deal date |
| Value Date | Indicates the value date of bought currency of the deal |

The external system where the Forex deals are maintained can invoke the Transact API to provide the Forex deal details to be linked with the Transact Limit.

- Whenever an exposure request is recorded in Transact from an external system for Forex deals, the system validates the limit product configuration for the LI.EXTERNAL.TRANSACTIONS application in the LIMIT.PARAMETER .
- In addition to the exposure details being updated in LI.EXTERNAL.TRANSACTIONS , the LIMIT.DAILY.OS application is also updated with details such as Buy currency, Buy currency amount, Sell currency, Sell currency amount, Clean risk amount, and Total outstanding after netting for all external Forex contracts of the respective limit.
- The limit netting process is also supported for Forex deals from external systems.

When a client uses an external system to perform FX transactions, and all credit limits are maintained in Transact, the exposure utilised by these FX transactions must be stored in the Transact Limit application. The following steps outline the process to capture and store external FX exposure in Transact .

1. Create a Limit Product with the FXorTb field set to FX and the Allow external field set to Yes.
2. To link the limit with forex contract from the external business application, link the limit product created exclusively for external exposure with the Transact’s business application namely LI.EXTERNAL.TRANSACTIONS using the LIMIT.PARAMETER application. The screenshot below shows the limit product created in step1 linked to the business application.
3. Create a Limit record with the Limit product created in step 1 to support the exposure of external forex contract. The external system sends a request to store the movements on credit limit. The screenshots below show the details captured such as transaction reference, amount, value date, revolving nature of contract and credit or debit indicator for contracts upon commitment or utilisation or repayment of the credit limit. As a result, Transact receives the request and creates a new record in the LI.EXTERNAL.TRANSACTIONS application and updates the LIMIT , LIMIT.TXNS and LIMIT.DAILY.OS applications with the utilisation details. The screenshot below shows the authorisation request sent by the external business application through API to Transact.


##### API and Events for Limit

The following APIs are exposed from the Transact system. The external system can invoke the APIs to push the exposure details.

| API URL | Description |
|---|---|
| /holdings/creditLimits/accounts/{accountId} | Creates a contract with static information such as contract type, reference, maturity, customers and system details. This establishes a link between contract static data and the credit limit and checks if the contract is applicable to be linked against specified limit based on rules defined for the credit line product. |
| /holdings/creditLimits/accounts/transactions/{transactionId} | Creates movements on credit limits with details such as transaction reference, amount, value date, revolving nature of contract and credit or debit indicator for contracts upon commitment or utilization or repayment of credit limit. |
| /holdings/creditLimits/forex/transactions/{transactionId} | Creates movements on credit limits with details such as transaction reference, buy currency, buy amount, value date, sell currency, sell amount for forex transactions. |

Transact emits the following events during limit creation, amendment, and reversal. The external system can subscribe to these events for further action.

| Event Name | Description |
|---|---|
| CreditLimits.CreateSecuredLimit.SecuredLimitCreated | Indicates the creation of secured limit |
| CreditLimits.CreateUnsecuredLimit.UnsecuredLimitCreated | Indicates the creation of unsecured limit |
| CreditLimits.CreateGroupSecuredLimit.GroupSecuredLimitCreated | Indicates the creation of group secured limit |
| CreditLimits.CreateGroupUnsecuredLimit.GroupUnsecuredLimitCreated | Indicates the creation of group unsecured limit |
| CreditLimits.CreateLiabilityGroupLimit.LiabilityGroupLimitCreated | Indicates the creation of customer liability group |
| CreditLimits.CancelLimit.LimitCancelled | Indicates cancellation of the limit |
| CreditLimits.ReverseGroupUnsecuredLimit.GroupUnsecuredLimitReversed | Indicates the reversal of group unsecured limit |
| CreditLimits.ReverseGroupsecuredLimit.GroupSecuredLimitReversed | Indicates the reversal of group secured limit |
| CreditLimits.ReverseLiabilityGroupLimit.LiabilityGroupLimitReversed | Indicates the reversal of liability group limit |


#### 📋 Tasks

There are no Tasks available for Externalising Transact Limit Exposure feature.


#### 📊 Outputs

There are no Outputs available for Externalising Transact Limit Exposure feature.


> **Related Applications:** `CATEGORY`, `EB.PRODUCT`, `LI.EXTERNAL.CONTRACT`, `LI.EXTERNAL.TRANSACTION`, `LI.EXTERNAL.TRANSACTIONS`, `LIMIT`, `LIMIT.DAILY.OS`, `LIMIT.PARAMETER`, `LIMIT.REFERENCE`, `LIMIT.TXNS`

---


### 2.14  Impact of Loan Repayment


> **📇 Quick Reference Card**
> 
> **Purpose:** *The LIMIT.PARAMETER and LIMIT applications contains fields and logic meant to parametrize if the limit amount gets automatically reduced or not upon repayment of a non-revolving limit.*
> 
> **Key Fields:** *Advised Amount*, *Internal Amount*, *Reduce Limit Amt*, *Repaid Amount*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The LIMIT.PARAMETER and LIMIT applications contains fields and logic meant to parametrize if the limit amount gets automatically reduced or not upon repayment of a non-revolving limit.


#### ⚙️ Configuration

The Reduce Limit Amt field in the LIMIT.PARAMETER application can be configured with the following values:

- Yes – This option maintains the existing functionality where the Internal Amount and Advised Amount fields are automatically reduced by the system each time a repayment is done against a non-revolving limit.
- No – This option maintains the original values of the Internal Amount and Advised Amount fields and makes Risk and Exposure Overview reports use the value from the Repaid Amount field in the CUSTOMER.LIMITS application to dynamically calculate and display the reduced limit amounts.
- Null – This option is similar to the Yes value.


#### 📋 Tasks

There are no Tasks available for Impact of Loan Repayment on Non-Revolving Limit feature.


#### 📊 Outputs

There are no Outputs available for Impact of Loan Repayment on Non-Revolving Limit feature.

---


### 2.15  Intraday Limit


> **📇 Quick Reference Card**
> 
> **Purpose:** *When a limit is granted, the functionality for setting up an intraday limit amount in the system is added to the available balance of a customer’s account.*
> 
> **Key Fields:** *Allow Intraday Limit*, *End Time*, *Start Time*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

When a limit is granted, the functionality for setting up an intraday limit amount in the system is added to the available balance of a customer’s account.

The intraday limit (IDL) is set on the level of the LIMIT record. For this, the IDL is allowed on the level of the limit product in the LIMIT.REFERENCE application.


#### ⚙️ Configuration

The intraday limit is configured in the LIMIT.REFERENCE application using the following fields:

- Allow Intraday Limit – If this field is set to Yes, then an intraday limit can be setup on the limit. If this field is set to No or blank, then an intraday limit is not allowed.
- Start Time – This field defines the time of day when the intraday limit amount becomes available for use.
- End Time – This field defines the time of day when the intraday limit amount becomes unavailable.


#### 📋 Tasks

There are no Tasks available for Intraday Limit feature.


#### 📊 Outputs

There are no Outputs available for Intraday Limit feature.

---


### 2.16  Joint Owned Limits


> **📇 Quick Reference Card**
> 
> **Purpose:** *The joint owned limits enables the multiple customers to own the limit jointly.*
> 
> **Key Fields:** *Customer No*, *Joint Liability*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The joint owned limits enables the multiple customers to own the limit jointly.


#### ⚙️ Configuration

The multi-customer limit with joint liability is enabled only when the Key Type field in the LIMIT.PARAMETER application is set to Txn Ref. The Limit Property Class arrangement captures the alphanumeric limit key. The Customer Property Class arrangement uses the Limit Alloc Perc field for all owners of an arrangement. The underlying AA.CUSTOMER.ROLE application must be changed to enable the same functionality.

The Customer No is a mandatory multi-value field holding customer record ID(s) that share the given limit amount. Customers linked to the LIMIT record using this field share the limit amount but they are joint and severally liable only based on the value of Joint Liability field. Duplicate customer numbers are not allowed in this field.

Customers with status as Prospect are not allowed for the values in this field. Customers with status as Active, Fictive and Prospect Limit status are allowed for the values in this field. The customers entered in this field must belong to the same customer group.

If a

record is created with customers 190195, 190196, 190197 belonging to it, then those same customers can be linked to the same

record:

Joint Liability is an optional field which specifies if the joint customers are severally liable for the given limit amount or not.

This field has the following values:

- Yes – Customers entered in Customer No field are all joint and severally liable for the given limit.
- No – Customers entered in Customer No field are not joint and severally liable for the given limit but they share it.
- Null – Similar to the No value.

If multiple customers are linked to a

record and they are liable for the entire limit amount, then the

field is set to Yes. If those customers share only the limit, then this field is set to No or left blank.


#### 📋 Tasks

There are no Tasks available for Joint Owned Limits – Limit Structure feature.


#### 📊 Outputs

There are no Outputs available for Joint Owned Limits – Limit Structure feature.

---


### 2.17  Liability Structure Limit Sharing Group


> **📇 Quick Reference Card**
> 
> **Purpose:** *This functionality allows the user to define a Liability Limit structure using the Limit Sharing Group functionality. The LIMIT application allows the user to setup a Limit Sharing Group as being liable for the exposure created against a Limit record.*
> 
> **Key Fields:** *Allowed Customer*, *Allowed Product*, *GB Description*, *Liability No.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

This functionality allows the user to define a Liability Limit structure using the Limit Sharing Group functionality. The LIMIT application allows the user to setup a Limit Sharing Group as being liable for the exposure created against a Limit record.


#### ⚙️ Configuration

To create a Liability Limit structure for a Limit Sharing Group, the user needs to define the Limit Products in the LIMIT.REFERENCE application. This allows in defining the Limit Products in the Limit Sharing Group and creating Limit records.

For example, the user can set a child Limit Product as shown in the below screenshot:

The corresponding parent Limit Product is shown below.


#### 🔧 Working With

After Limit Products are created in the LIMIT.REFERENCE application, the user can create Limit Sharing Groups in the LIMIT.SHARING.GROUP application.

The following table shows an example of a Limit Sharing Group structure for Limit Products 5400 and 5401, where the limits are shared among customers 147294, 147295 and 147296:

| Limit ID | Liability ID | Product | Customer ID | Record Parent | Notes |
|---|---|---|---|---|---|
| LI0000100821 | M000000110 | 5400 |  |  | Overall group limit |
| LI0000100822 | M000000110 | 5401 |  | LI0000100821 | 5401 product cap for all customers |
| LI0000100823 | M000000110 | 5400 | 147294 | LI0000100821 | Customer 147294 level cap for product 5400 |
| LI0000100824 | M000000110 | 5401 | 147294 | LI0000100823 | Product 5401 and customer 147294 cap |
| LI0000100825 | M000000110 | 5400 | 147295 | LI0000100821 | Customer 147295 level cap for product 5400 |
| LI0000100826 | M000000110 | 5401 | 147295 | LI0000100825 | Product 5401 and customer 147295 cap |
| LI0000100827 | M000000110 | 5400 | 147296 | LI0000100821 | Customer 147296 level cap for product 5400 |
| LI0000100828 | M000000110 | 5401 | 147296 | LI0000100827 | Product 5401 and customer 147296 cap |
| LI0000100829 | S000000012 | 5400 |  | LI0000100821 | Cap for customers 147294 and 147295 |
| LI0000100830 | S000000013 | 5400 |  | LI0000100821 | Cap for customers 147294 and 147296 |

The user creates the Limit Sharing Groups as follows:

- Main Sharing Group M000000110 for all three customers and the parent Limit Product.
- Sub-group S000000012 for customers 147294 and 147295 and the child Limit Product.
- Sub-group S000000013 for customers 147294 and 147296 and the child Limit Product.

After creating Limit Sharing Groups in the LIMIT.SHARING.GROUP application, the user can create Limit records in the LIMIT application. This is performed by setting the above Limit Sharing Group record IDs in the Liability No. field as follows:

- Overall Sharing Group Limit record LI0000100821 for Main Sharing Group M000000110 and parent Limit Product 5400.
- Limit record LI0000100822 holds the cap for Limit Product 5401 for all customers.
- Limit record LI0000100823 holds the cap for Limit Product 5400 for customer 147294.
- Limit record LI0000100824 holds the cap for Limit Product 5401 for customer 147294.
- Limit record LI0000100825 holds the cap for Limit Product 5400 for customer 147295.
- Limit record LI0000100826 holds the cap for Limit Product 5401 for customer 147295.
- Limit record LI0000100827 holds the cap for Limit Product 5400 for customer 147296.
- Limit record LI0000100828 holds the cap for Limit Product 5401 for customer 147296.
- Limit record LI0000100829 holds the cap for customers 147294 and 147295 together, based on the Limit Sharing sub-group S000000012 (which holds these two customers).
- Limit record LI0000100830 holds the cap for customers 147294 and 147296 together, based on the Limit Sharing sub-group S000000013 (which holds these two customers).


#### 📋 Tasks

This enquiry allows the user to define a Liability Limit structure using the Limit Sharing Group functionality. The LIMIT application allows the user to setup a Limit Sharing Group, as being liable for the exposure created against a Limit record.


##### Workflow

This section helps the user to perform the below tasks:

LIMIT.SHARING.GROUP table helps the user to create the limit sharing group. To create a liability limit structure for a Limit Sharing Group, the user needs to define the limit products in the LIMIT.REFERENCE application. This enquiry allows the user to define the limit products in the Limit Sharing Group and creating Limit records.

To create a limit sharing group, follow the below steps:

1. Create Limit Group .
2. In the Create Group screen, click the New Deal icon.
3. Enter values in the below fields: GB Description Allowed Customer Allowed Product
4. Click the Validate icon to check for errors and overrides
5. Click the Commit icon to submit the record.


#### 📊 Outputs

This enquiry allows the user to define a Liability Limit structure using the Limit Sharing Group functionality. The LIMIT application allows the user to setup a Limit Sharing Group, as being liable for the exposure created against a Limit record.


##### Enquiries and Reports

This section allows the user to view the below enquiries and reports:

Sharing Group Details

This enquiry displays the list of Limit Sharing Group details based on customer.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


### 2.18  Limit Change Utility


> **📇 Quick Reference Card**
> 
> **Purpose:** *The limit system is complex. There are a large number of connections and relationships within the data and other Temenos Transact applications. Consequently, amendments to some limit information may cause extensive adjustments and recalculations. The LIMIT.CHANGE application is used to make the chan...*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The limit system is complex. There are a large number of connections and relationships within the data and other Temenos Transact applications. Consequently, amendments to some limit information may cause extensive adjustments and recalculations. The LIMIT.CHANGE application is used to make the changes to limit.


#### ⚙️ Configuration

The following amendments can be made either during the COB or online using the verify function in the LIMIT.CHANGE application.

- Add or change a customer liability.
- Change Currency and Check Limit fields in a LIMIT record.
- Modify the Limit Percentage in a LIMIT.REFERENCE record.

> **⚠️ Note:** However, the amendment to enable or disable FX limit netting can be done only during the COB.

There is one record in this application, that is, SYSTEM.


#### 📋 Tasks

There are no Tasks available for Limit Change Utility feature.


#### 📊 Outputs

There are no Outputs available for Limit Change Utility feature.

---


### 2.19  Limit Sub-Allocation


> **📇 Quick Reference Card**
> 
> **Purpose:** *Sub-allocations are the transfer of limit amount to or from a limit.*
> 
> **Applications:** `LIMIT.PARAMETER`
> 
> **Key Fields:** *Auto Restore Alloc*, *Commit*, *Effective Date*, *Max Sub Alloc*, *Notes*, *Temp Limit*, *Validate*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Sub-allocations are the transfer of limit amount to or from a limit.

- A transfer from a limit is known as a ‘sub-allocation given’ and reduces the available value of the limit.
- A transfer to a limit is a ‘sub-allocation received’ and increases the available value of a limit.

The Effective Date field from the LIMIT.SUB.ALLOC application now accepts a future date. In such cases, funds from the source limit are booked instantly to ensure their availability when the sub-allocation becomes effective.

The Auto Restore Alloc field from the LIMIT.SUB.ALLOC application now has a value called Maximum. In case of either revolving or non-revolving limits, when the sub-allocation expires, funds returned to source limit is always capped with the target limit’s available amount. If the available amount is less than the sub-allocated amount, only what is left of the available amount is reverted.

Separate charges and interest rate conditions can be set up for the amount sub-allocated from the Reservation Limit to the Utilisation Limit. Besides the existing two limit tiers (one for limit amount, one for excess overdraft), the system has been enhanced to maintain an additional third interest tier for the temporarily sub-allocated funds. The ACCOUNT.DEBIT.LIMIT application has been enhanced with a field called Temp Limit , which keeps the sub-allocated amount. This field is used to derive the interest threshold in the AA arrangement for this amount.

Limit Banking Capability supports creation of limit sub-allocations through API and communicates with different business applications through events.


#### ⚙️ Configuration

The user sets the Max Sub Alloc field in the LIMIT.PARAMETER application to define the maximum number of sub-allocations that can be either given or taken from an individual limit. The allowed values of this field range from 01 to 25. Any value outside this range result in an error.

> **⚠️ Note:** The system provides a sub-allocation ID and expiry date in the limit record only when this field is configured. If not configured, the system nets the sub-allocation values based on the date and currency.

When the limit sub-allocation is created, the following logics are used to calculate if the sub-allocation breaches the maximum number:

- From the perspective of the limit giving the sub-allocation, the system considers the total number of sub-allocations given by that limit.
- From the perspective of the limit receiving the sub-allocation, the system considers the total number of sub-allocations received by that limit.

Example for calculating max sub-allocations:

When a user initiates a sub-allocation from Limit A to Limit B, the system first checks the total number of sub-allocations assigned to Limit A. If this number is below twenty five, the system then checks Limit B. If both limits have fewer than twenty five sub-allocations, the system allows the creation of a new sub-allocation. However, if either limit has reached or exceeded twenty five sub-allocations, the system displays an error message indicating that the maximum number of sub-allocations has been reached.

Example for calculating max sub-allocation in hierarchy:

In multi-level sub-product limit structures, the top-level limit tracks the total count of all sub-allocations across subordinate sub-products. For instance, if a limit is created using sub-product 2310 and has two subordinate limits under sub-products 2311 and 2312, any sub-allocations given or received by these subordinate limits contribute to the sub-allocation count at the top level. If the sub-allocations at level 02 exceed the maximum allowed, the excess is also reflected in the count at level 01.


#### 📋 Tasks

Related topics:

- Sub-allocate Limit
- Lending Processes (Corporate)

Sub-allocation is the process of sharing of one limit amount with another limit. Sub-allocations can be performed in the same group or different groups.


##### Workflow

This section helps the user to perform the below tasks:

This screen allows the user to create the Limit sub-allocation record.

To create a Limit Sub Allocation, follow the below steps:

1. Sub Allocate Limit .
2. In the Limit Sub Allocation screen, enter values in the following mandatory fields: Sub Alloc From Sub Alloc To Notes Effective Date Expiry Date Online Limit Currency
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon to create the record.

| SCREENS | WORKFLOW |
|---|---|
|  | Sub Allocate Limit . |
| Unauthorised Limit Sub Allocation Records | Click the Authorise icon of a corresponding record. The system opens the record to be authorised. |
| Limit Sub Allocation | Click the Authorise icon to authorise the record. |


#### 📊 Outputs

There are no Outputs available for Limit Sub-Allocations feature.


> **Related Applications:** `LIMIT.PARAMETER`

---


### 2.20  Linking Collaterals to Limit


> **📇 Quick Reference Card**
> 
> **Purpose:** *The limit becomes secured when a collateral is linked to a limit.*
> 
> **Key Fields:** *Collateral Code*, *Collateral Priority*, *Customer*, *Fix/Variable*, *Limit Reference*, *Percentage Allocation*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Limit can be:

- Fully Secured
- Partly Secured
- Unsecured

The limit becomes secured when a collateral is linked to a limit.

The limit is partly secured when the value of the collateral does not cover the limit amount. If the collateral is not covered, then the limit is unsecured.


#### ⚙️ Configuration

The COLLATERAL records can be linked to LIMIT records. For example, a mortgage can be linked to a loan limit. The link can be used for information only (a fixed limit). The value of collateral can also be used to determine the availability of the limit (a variable limit). The respective settings (fixed or variable) are performed in the LIMIT record. The following flowchart shows the collateral and limit structure.

The link is made by entering the LIMIT ID in the COLLATERAL.RIGHT record.


#### 📋 Tasks

Related topics:

- Create And Link Collateral

Limit can be either secured or unsecured. A limit becomes secured when a collateral is linked to a limit. Linking of collateral and limit is achieved by the COLLATERAL.RIGHT application.

Limits (LI) module helps to attach a limit with collateral to make it secured. When a limit is linked to a collateral, the limit must be defined either as fixed or variable in the Fix/Variable field in the LIMIT record. Limit record must be created before creating Collateral Right record.


##### Workflow

This section helps the user to perform the below tasks:

COLLATERAL.RIGHT table helps the user to link Limit to the collateral and makes it secured limit.

To create collateral link, follow the below steps:

1. Collateral Link .
2. In the Collateral screen, click the New Deal icon.
3. Enter values in the below fields: Collateral Code Limit Reference Customer Percentage Allocation Collateral Priority
4. Click the Validate icon to check for errors and overrides
5. Click the Commit icon to submit the record.

| SCREENS | WORKFLOW |
|---|---|
|  | Authorise/Delete Collateral Right . |
| Unauthorised Collateral Right | Click the Authorise icon corresponding to a record. |
| Collateral Link | Click the Authorise to verify the record. |


#### 📊 Outputs

There are no Outputs available for Linking Collaterals to Limit feature.

---


### 2.21  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *The term Credit Limit refers to the maximum amount of credit a financial institution extends to a customer. A lending institution extends a credit limit on a line of credit. Usually, the lenders set the credit limits based on information in the application of the person seeking credit, that is, borr...*
> 
> **Applications:** `MS.PARAMETER`
> 
> **Key Fields:** *Check Validation Limit Breach*, *Emit Business Event*, *LIMIT.TYPE*, *Pro Data Calculation*, *SUPPRESS.ACCOUNTING*, *THIRD.PARTY.EXPOSURE*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- APIs
- Temenos Transact Services

The term Credit Limit refers to the maximum amount of credit a financial institution extends to a customer. A lending institution extends a credit limit on a line of credit. Usually, the lenders set the credit limits based on information in the application of the person seeking credit, that is, borrowers. Credit limit is one of the factors that affect the consumers' credit scores and can impact their ability to get credit in the future. A lender generally gives lower-credit limits to high-risk borrowers because they may not be able to repay the debt. Low-risk borrowers usually get higher credit limits, giving them higher flexibility to spend.

The limits are determined by banks, alternative lenders and credit card companies based on the information related to the borrower, such as

- Borrower's credit rating
- Personal income
- Loan repayment history and other factors

The line of credit is the maximum amount of money a lender allows a borrower to spend on a revolving or non-revolving credit limits.

The Limit (LI) module provides the credit limit or line of credit in Temenos Transact . All the business applications in Temenos Transact refer to the LI module for creation and maintenance of the line of credit facility applicable to the business scenario.


##### Product Configuration

Credit limits are held by customer and product. Simple limits can be defined for a single customer and single product. However, more complex limits can also be configured with multiple levels.

Limits are held by the customer at two levels:

- Individual
- Liability group

Also, limits can be held by the product as 12 levels:

- 10 levels of sub-product
- Product
- Global

Thus, an individual trade can be updated as six limits.

In this example, bank provides an unsecured loan to ABC Ltd of 3 million USD. ABC Ltd is a part of the larger group, ABC International. Bank monitors the limits at both company and group levels. Unsecured loans are a sub-product within loans and the limits are monitored at both levels. Finally, the bank sets a limitation on all business with ABC Ltd and with ABC International, and these limits are held at the global-level.

Consequently, the unsecured loan has updated six limits. If any limit is exceeded, an override is raised during the input of loan.

- LIMIT application holds the credit limits.
- LIMIT.REFERENCE application holds sub-products, products and global definitions.
- CUSTOMER application holds the customers and customer liability definitions.
- LIMIT.PARAMETER application defines the various high-level parameters regarding the application. It links contracts and accounts to LIMIT.REFERENCE .

The main limit parameters are shown in the below flowchart.

Limits can also be set to monitor the exposure against currencies, countries and industries. These limits are monitored overnight. The LIMIT application uses the parameter and product tables to define the structure of limits.

This application defines the parameters that determine the way in which the limit system operates. LIMIT.PARAMETER record can have the ID as ‘SYSTEM’. The LIMIT.PARAMETER application controls the following:

- An indicator to specify if the foreign exchange contracts must be netted before limit comparison.
- A 'number of days' to define how many days prior to Limit Expiry Date and Review Date (can be fixed in the Review Frequency field) in the LIMIT application, the approach of these events must be reported.
- A date and cycle to indicate when the first revaluation occurs and at what frequency thereafter.
- A date and cycle to indicate when a central liability report (including those liability numbers which did not move) must be produced in the back-end process.
- A date and cycle to indicate when the commodity, country and currency reports must be produced.
- A ‘number of days’, administrative Extension Days, define the maximum number of days by which the expiry date of a limit can be ’administratively’ extended before a new expiry date must be assigned to the limit.
- The LIMIT application is defined according to the specific requirements of the bank. The most important feature of this application is that it allows the bank (for each financial application) to define the precise rules applicable to an environment. In this way, the limit verification process can be established by the bank according to a bank’s own set of rules without any program maintenance.

The product group definition that allows the bank to specify the different products, (in bank’s opinion) must be part of the commodity, country and currency exposure.

Creation of Other Record IDs:

The LIMIT.PARAMETER application allows the creation of other record IDs besides SYSTEM. These record IDs can have a valid legacy application (that is, ACCOUNT, LD, MM and FOREX) as ID. The purpose of these records is to move their parametersation, which was initially done in the SYSTEM record, to new individual records for each application to improve system performance.

For example, for the ACCOUNT application, the user can create a new record, which includes all the necessary parametrisation for this particular application.


##### Business Events

When the Emit Business Event field in MS.PARAMETER is set as ‘Yes’, the business events representing the state change are emitted.

The following business events are emitted for Limit related tables.

| Business Event | Description |
|---|---|
| creditLimits.createLimitParameter.limitParameterCreated | Event to create limit parameter |
| creditLimits.updateLimitParameter.limitParameterUpdated | Event to amend limit parameter |
| creditLimits.createProduct.productCreated | Event to create limit product |
| creditLimits.createUtilisationProduct.utilisationProductCreated | Event to create utilisation limit product |
| creditLimits.createValidationProduct.validationProductCreated | Event to create validation limit product |
| creditLimits.createIntradayProduct.intradayProductCreated | Event to create intraday limit product |
| creditLimits.createReservationProduct.reservationProductCreated | Event to create reservation limit product |
| creditLimits.updateLimitProduct.productUpdated | Event to amend limit product |
| creditLimits.updateIntradayProduct.intradayProductUpdated | Event to amend intraday limit product |
| creditLimits.cancelLimitProduct.productCancelled | Event to cancel limit product |
| creditLimits.createSecuredLimit.securedLimitCreated | Event to create secured limit |
| creditLimits.createUnsecuredLimit.unsecuredLimitCreated | Event to create unsecured limit |
| creditLimits.createGroupSecuredLimit.groupSecuredLimitCreated | Event to create secured group limit |
| creditLimits.createGroupUnsecuredLimit.groupUnsecuredLimitCreated | Event to create unsecured group limit |
| creditLimits.createReportingLimits.customerReportingLimitsCreated | Event to create reporting credit limit |
| creditLimits.updateIntradayLimit.intradayLimitUpdated | Event to amend intraday credit limit |
| creditLimits.createReservationLimit.reservationLimitCreated | Event to create reservation limit |
| creditLimits.limitExpiryDueDate.expiryDue | Event for limit expiry due date |
| creditLimits.limitExpiryFailure.expiryFailed | Event for limit expiry failure |
| creditLimits.limitReviewDate.reviewDateReached | Event to review limit on review date |
| creditLimits.limitReviewDueDate.reviewDue | Event to review limit |
| creditLimits.updateLimit.limitUpdated | Event to amend limit |
| creditLimits.updateLimitAmount.limitAmountUpdated | Event to update limit amounts |
| creditLimits.updateLimitAvailability.limitAvailabilityUpdated | Event to update limit availability |
| creditLimits.updateExpiryDate.limitExpiryDateUpdated | Event to update expiry date of limit |
| creditLimits.reportLimitIncrease.limitIncreased | Event to increase limit schedule |
| creditLimits.reportLimitDecrease.limitDecreased | Event to decrease limit schedule |
| creditLimits.reportLimitExpiry.limitExpired | Event to indicate limit expiry |
| creditLimits.reportLimitBreach.validationLimitBreached | Event to validate limit breach |
| creditLimits.cancelLimit.limitCancelled | Event to cancel limit |
| creditLimits.updateExposure | Transaction command event for exposure update |
| creditLimits.updateExposure.exposureUpdated | Event to update exposure in the limit |
| creditLimits.deleteExposure | Transaction command event for exposure delete |
| creditLimits.delinkContract | Event to be emitted when limit is delinked from contract |
| creditLimits.delinkContract.contractDelinked | Event to delink contract from the limit |
| creditLimits.recordContractClosure | Event to be emitted when contract is linked to limit closed |
| creditLimits.recordContractClosure.contractClosed | Event for limit contract closure |
| creditLimits.recordContractLink | Event to be emitted for the limit and contract link |
| creditLimits.recordContractLink.contractRecorded | Event to link contract to the limit |
| creditLimits.updateContractLimit | Event to be emitted to update limit property linked with contract |
| creditLimits.updateContractLimit.contractLimitUpdated | Event to update limit in limit contract |
| creditLimits.updateContractOwners | Event to be emitted when customer changes the contract linked to limit |
| creditLimits.updateContractOwners.contractOwnersUpdated | Event to update owner in limit contract |
| creditLimits.updateContractProperties | Event to be emitted when there is a change in contract linked to limit |
| creditLimits.updateContractProperties.contractDetailsUpdated | Event to update limit contract properties |
| creditLimits.updateContractTerm | Event to be emitted when there is a change in contract term |
| creditLimits.updateContractTerm.contractTermUpdated | Event to update term in limit contract |
| creditLimits.updateTransactionStatus | Transaction command event to authorise exposure |


##### Illustrating Model Parameters

This section covers the high-level specification required for Limits (LI) module.

| S.No. | Parameters | Description |
|---|---|---|
| 1. | LIMIT.PARAMETER | This application allows the user to define the parameter that determine the way in which LI module operates. It also allows the user to define the following: If foreign exchange contracts are to be netted. The date and frequency at which the revaluation occurs. The date and frequency at which the currency, commodity and country reports must be produced. The date and frequency at which central liability report must be produced in the back end process. Defining the frequency at which the collateral accounting service should be run. Defining the accounting type based on which entries would be booked in Limit's EB.CONTRACT.BALANCES record, depending on the Balance types specified in respective Collateral Codes. |
| 2. | LIMIT.REFERENCE | This application allows the user to define the parameter, which links accounts and contracts to Limits (LI) products. In addition, it allows the user to define margin level or percentage ration between the limit amount utilised and the value of collateral available. It allows the user to define different limit amounts for contracts on different maturity dates. When the LIMIT.TYPE field is set to: Utilisation - The Limit product holds the Utilisation Limit records. Validation - The Limit product holds the Validation Limit records, which constitutes the maximum cap allowed for the underlying Utilisation Limits within a Limit structure. Standalone - The Limit product holds the Standalone Limit records, which have the same functionality as Utilisation Limit records apart from the fact that they hold no parent or child Limits. SUPPRESS.ACCOUNTING field is set to ‘Yes’ to suppress any GL accounting performed against the Limit records under the Limit product. This field accepts the input when the Limit record has nothing set in the Reference Child field. When the THIRD.PARTY.EXPOSURE field set to ‘Yes’, it marks the given Limit records under the Limit product to hold the third party exposure for their Customer(s). Any exposure created against these Limit records are excluded from the bank’s risk reports. |
| 3. | LIMIT.COMMODITY | This application allows the user to define the limits by commodity (industry type). |
| 4. | LIMIT.COMMODITY.GRP | This application allows the user to define the commodity industry groupings. |
| 5. | LIMIT.COUNTRY | This application allows the user to define the limits by countries or group of countries. |
| 6. | LIMIT.COUNTRY.GRP | This application allows the user to define country groupings. |
| 7. | LIMIT.CURRENCY | This application allows the user to define limits by currency. |
| 8. | LIMIT.CHANGE | This application allows the user to make changes to the existing limit records. User can add or change customer liability, currency and limit percentage. |
| 9. | LIMIT.REPORTING.PARAMETER | This application allows the user to enable the reporting of breach on the internal amount of the validation limit. Pro Data Calculation field mentions whether pro-rata calculation has to be done irrespective of manual percentage in Common Exposure Reports. Check Validation Limit Breach field indicates if breaches to validation limits have to be reported in a separate file. |
| 10. | LIMIT.NETTING.PARAM | This application allows the user to activate or deactivate the foreign exchange limit netting option, when required. |
| 11. | LI.MULTI.CUSTOMER.LIMIT.PARAMETER | This application allows the user to configure the rules for multi- customer limits without joint liability rules based on customer segments. Using this parameter, Users can configure the rules for Joint/Multi Customer Limit based on customer segment. Multi-Customer limits can be created with customers belonging to different risk groups or no group based on this parameter setup. |
| 12. | LI.TIME.CODE | This application allows the user to configure the charges based on the level of designated AA account for the respective balance types and the possibility to calculate charges per each time band amount. |
| 13. | ADMIN.LIMIT.PARAMETER | This application allows to set up limit parameters, application wise. It lists the limit parameter application records (if exists) and also user can amend the record (with limited fields, like Application, Decision to fields). |


##### Illustrating Model Products

The following are few examples of the LI products in the LIMIT.REFERENCE application.

| S.No. | Products |
|---|---|
| 1. | Advances for Current Account |
| 2. | Loans Secured |
| 3. | Loans Unsecured |
| 4. | Commercial Loans |
| 5. | Term Loans |
| 6. | Project Finance Secured |
| 7. | Project Finance Unsecured |
| 8. | Packing Credit Secured |
| 9. | Packing Credit Unsecured |
| 10. | Bills of Exchange |
| 11. | Securities |
| 12. | Facility Limit |
| 13. | Packing Credit |


> **Related Applications:** `MS.PARAMETER`

---


### 2.22  Monitoring Credit Exposure


> **📇 Quick Reference Card**
> 
> **Purpose:** *Credit exposures can be monitored by commodity, country and currency and appropriate reports can be generated at regular intervals.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Credit exposures can be monitored by commodity, country and currency and appropriate reports can be generated at regular intervals.


#### ⚙️ Configuration

Limits can be monitored against the following reports that are produced during COB at a frequency that is defined in the LIMIT.PARAMETER record:

- Commodity limits
- Country limits
- Currency exposure

Commodity, country and currency limits are set against groups of products in LIMIT.PARAMETER . For example, group of products can be defined as ALL-LINES which indicates the maximum exposure for the products.


#### 📋 Tasks

There are no Tasks available for Monitoring Credit Exposure feature.


#### 📊 Outputs

There are no Outputs available for Monitoring Credit Exposure feature.

---


### 2.23  Neutral Revolving Limit Structure


> **📇 Quick Reference Card**
> 
> **Purpose:** *Neutral limits represent a dynamic limit structure that adapts its nature based on the underlying accounts or contracts it is linked to. Unlike conventional revolving or non-revolving limits, their status is derived from the lowest-level configuration in the limit hierarchy (such as a drawing or dis...*
> 
> **Applications:** `LIMIT.REFERENCE`
> 
> **Key Fields:** *Limit Type*, *Reducing Limit*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Neutral limits represent a dynamic limit structure that adapts its nature based on the underlying accounts or contracts it is linked to. Unlike conventional revolving or non-revolving limits, their status is derived from the lowest-level configuration in the limit hierarchy (such as a drawing or disbursement). This ensures that the limit structure is flexible and responsive to the specific needs of financial arrangements.

For example, consider an AA (Arrangement Architecture) product set-up with the same utilisation limit and is linked to both the facility product and its underlying drawing products.

The above diagram demonstrates a hierarchical limit structure where a facility is the parent entity encompassing multiple drawings. Each drawing represents a disbursement level tied to the facility. The limit structure operates under a neutral revolving limit configuration, where the revolving or non-revolving nature of limits propagates based on the linked contracts or accounts.

The facility limit governs the overall limit, while each drawing has its own drawing commitment outstanding and disbursement amounts. Additionally, non-contingent OS values are computed to ensure proper utilisation of the tracking. The above diagram indicates that the nature of these limits (revolving or non-revolving) depends on the lowest-level configuration of the structure. If the lowest-level (for example, a drawing) is set to ‘Neutral’, this status cascades up to all higher levels, ensuring consistency in how the limits are managed and utilised.


#### ⚙️ Configuration

The ‘Neutral’ option in the Reducing Limit field (in the LIMIT.REFERENCE table) is used to configure the Neutral Revolving Limit Structure.

The values available for this field are:

- Yes – The limit product holds non-revolving (reducing) Limit records.
- No – The limit product holds revolving (non-reducing) Limit records.
- Cascade – The LIMIT records of the limit product inherit a revolving or non-revolving nature from its underlying child limit product, which is available for input only when the Limit Type field is set as Validation.
- Neutral – The LIMIT records of the limit product inherit a revolving or non-revolving nature from the contract or account they are linked to. This status is propagated from the lowest level of limit structure up to the highest level. If the lowest level is set as Neutral, the system accepts all the upper levels to be only Neutral.

For example, this can be an AA (Arrangement Architecture) product set-up with the same utilisation limit linked to both the facility product and its underlying drawing products.

The LIMIT.REFERENCE table (as part of the single-level facility linked to a limit) enables the creation of a neutral limit structure across all levels of the hierarchy.

- When a limit is defined as neutral and the linked contract nature is revolving, then the limit inherits a revolving nature.
- Similarly, if the limit is defined as neutral and the linked contract nature is non-revolving, then the limit inherits a non-revolving nature.

The following screenshot shows the Neutral option checked in the Reducing Limit field in the LIMIT.REFERENCE table.


#### 🔧 Working With

To create the below revolving neutral limit product structure,

The lowest level of the limit product structure is first created.

- Shared limit product 1111
- Shared limit product 1112
- Shared technical limit product 1120 with1111 and 1112 as child products
- Standalone limit product 1130

> **⚠️ Note:** The parent validation limit product can be created only after all the utilisation limit products are created.

The neutral status is particularly useful when the bank or the financial institution needs to dynamically determine the nature of the limits (revolving or non-revolving) without rigidly defining them at the product level. Below is the configuration for a neutral limit product structure.

Consider a scenario where limits are created using the neutral limit structure with the initial limit setup as follows:

- Credit Facilities (Validation Limit) is created with an Internal Amount of 1,000,000. This acts as the overall cap or validation limit for credit utilisation, ensuring the total usage under all connected facilities does not exceed this amount. Validation Limit is linked to the facility contract.
- Utilization Limit (Parent/Technical Shared) is created with an Internal Amount of 800,000. This is a technical or shared limit derived from the validation limit and allocated for further distribution on individual drawings level. Two revolving facility drawings are created, each with a commitment amount of 400,000 and are linked to the utilisation limit as shown below.

Consider one of the drawing contracts has utilised an amount of 100,000 USD, after which the limit hierarchy reflects the balances as shown below.

When the utilised amount is completely paid back to the facility drawing, the same is reflected in the limit structure which is restored, as the limit has inherited its revolving nature from the drawing contract.

Unlike revolving contracts, non-revolving facility and drawings are created and attached to the validation limits and utilisation limits using the same limit product hierarchy as shown in Example 1.

Consider one of the drawing contracts has utilised an amount of 100,000 USD, after which the limit hierarchy reflects the balances as shown below.

When the utilised amount is completely paid back to the facility drawing, it is not reflected in the limit structure, as the limit has inherited its non-revolving nature from the drawing contract.

> **⚠️ Note:** The actual limit records can be created and linked to contracts or accounts only after all the limit products are created.


#### 📋 Tasks

There are no Tasks available for Neutral Revolving Limit Structure feature.


#### 📊 Outputs

There are no Outputs available for Neutral Revolving Limit Structure feature.


> **Related Applications:** `LIMIT.REFERENCE`

---


### 2.24  Offsetting Credit Balance Accounts


> **📇 Quick Reference Card**
> 
> **Purpose:** *Credit balances are used within the limit function on accounts to offset lending on debit balance accounts. The overall net balance on all accounts is used to determine if a limit is exceeded or not. Lending contracts can be included within the limit structure, so that credit balances on accounts ca...*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Credit balances are used within the limit function on accounts to offset lending on debit balance accounts. The overall net balance on all accounts is used to determine if a limit is exceeded or not. Lending contracts can be included within the limit structure, so that credit balances on accounts can be offset against a lending product or a combined account and lending product limit.


#### ⚙️ Configuration

To offset the limits with the credit balance accounts, the Allow Netting field in the LIMIT application is set to Yes and the Allow Netting flag in the ACCOUNT record for all accounts included in this limit (which can be used for offset), is set to Yes.


#### 📋 Tasks

There are no Tasks available for Offsetting of Limits with Credit Balance Accounts feature.


#### 📊 Outputs

There are no Outputs available for Offsetting of Limits with Credit Balance Accounts feature.

---


### 2.25  Overdraft Limits to Accounts


> **📇 Quick Reference Card**
> 
> **Purpose:** *Overdraft (OD) limits facility is available for certain types of customer and corporate accounts. These limits are created in the Limit module and linked to the appropriate account. The account holder is allowed to overdraw to the extent of the OD limit amount. When the overdraft amount exceeds the ...*
> 
> **Key Fields:** *Limit Reference*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Overdraft (OD) limits facility is available for certain types of customer and corporate accounts. These limits are created in the Limit module and linked to the appropriate account. The account holder is allowed to overdraw to the extent of the OD limit amount. When the overdraft amount exceeds the OD limit, the user decision is required to process the transaction.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

Related topics:

- Create and Link Collateral (Corporate)
- Lending Processes (Corporate)

The term Credit Limit refers to the maximum amount of credit a financial institution extends to a customer. A lending institution extends a credit limit on a line of credit.

A Limit (LI) product is an area of business for which the bank creates line of credit. LI products are defined in the LIMIT.REFERENCE application and are linked to the underlying business by using the LIMIT.PARAMETER application.


##### Workflow

This section allows the user to perform the below activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Attach Limit to Overdraft Account . |
| Contract Screen | Select or enter the overdraft account that requires to be linked and click the Edit icon. |
| Attach Limit to Overdraft Account | In the Basic tab, enter a value in the Limit Reference field. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

| SCREENS | WORKFLOW |
|---|---|
|  | Authorise/Delete Attach Limit . |
| Unauthorised Limits Attached to Accounts | Click the Authorise icon of a corresponding record. The system opens the record to be authorised. |
| Attach Limit to Overdraft Account | Click the Authorise icon. |


#### 📊 Outputs

There are no Outputs available for Overdraft Limits to Accounts feature.

---


### 2.26  Reporting of Breach to Validation Limit


> **📇 Quick Reference Card**
> 
> **Purpose:** *In the new limit structure, the limits are aggregated from bottom to top in the limit hierarchy. Thus, the internal amount of utilisation limits must not exceed the internal amount of the validation limit in the hierarchy. Any breach to the internal amount of the validation limit is monitored and re...*
> 
> **Key Fields:** *Check Val Lim Breach*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

In the new limit structure, the limits are aggregated from bottom to top in the limit hierarchy. Thus, the internal amount of utilisation limits must not exceed the internal amount of the validation limit in the hierarchy. Any breach to the internal amount of the validation limit is monitored and reported.


#### ⚙️ Configuration

To enable the reporting of breach on the internal amount of the validation limit, the Check Val Lim Breach field in the LIMIT.REPORTING.PARAMETER application must be set to Yes.


#### 📋 Tasks

There are no Tasks available for Reporting of Breach to Validation Limit feature.


#### 📊 Outputs

There are no Outputs available for Reporting of Breach to Validation Limit feature.

---


### 2.27  Restricted Allowed Customers


> **📇 Quick Reference Card**
> 
> **Purpose:** *If a limit is being set for a group of customers at liability-level, some customers within the group can be allowed to utilise the limit. On the other hand, customers within the group can be restricted, while allowing the others in the group to utilise the limit.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

If a limit is being set for a group of customers at liability-level, some customers within the group can be allowed to utilise the limit. On the other hand, customers within the group can be restricted, while allowing the others in the group to utilise the limit.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

There are no Tasks available for Restricted and Allowed Customers feature.


#### 📊 Outputs

There are no Outputs available for Restricted and Allowed Customers feature.

---


### 2.28  Risk Exposure Overview Enquiry


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Risk & Exposure Overview (CUSTOMER.SCV.CHECK) enquiry offers the ability to view exposure details per customer or per customer group. It displays only LIMIT records that have an alphanumeric ID and the AA accounts that have a credit balance.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The Risk & Exposure Overview (CUSTOMER.SCV.CHECK) enquiry offers the ability to view exposure details per customer or per customer group. It displays only LIMIT records that have an alphanumeric ID and the AA accounts that have a credit balance.


#### ⚙️ Configuration

For the enquiry to have data to consolidate, one or more Limit products ( LIMIT.REFERENCE records) must be created, as well as one or more Limits ( LIMIT records) for the respective customer(s).

Read the following sections for more information on how to create Limit products or Limits:

- Creating Limit Products
- Update of Approved and Advised Limit Based on Umbrella Limit Structure
- Joint Owned Limits – Limit Structure


#### 📋 Tasks

The Risk and Exposure Overview ( CUSTOMER.SCV.CHECK ) enquiry helps to view exposure details of the given customer or customer group. It displays only LIMIT records that have an alphanumeric ID and the AA accounts that have a credit balance. This enquiry displays single customer view or customer group view based on the input provided.


##### Workflow

This section helps the user to perform the below tasks:

| SCREENS | WORKFLOW |
|---|---|
|  | Limit Risk Exposure . |
| Customer/Group Risk Exposure | In the contract screen, enter the Customer ID/Group ID. Click the Risk Exposure icon of a corresponding record. |
| Customer Risk Exposure | Click the Amend Limit Details icon of a corresponding record. |
| Maintain Joint Limit | In the selected Limit record, capture the details that to be amended. Click the Validate icon to check for errors and overrides. Click the Commit icon to modify the record. |


#### 📊 Outputs

The Risk and Exposure Overview ( CUSTOMER.SCV.CHECK ) enquiry helps to view exposure details of the given customer or customer group. It displays only LIMIT records that have an alphanumeric ID and the AA accounts that have a credit balance. This enquiry displays single customer view or customer group view based on the input provided.


##### Enquiries and Reports

This section allows the user to view the below enquiries and reports:

Limit Risk Exposure

This enquiry helps to view the list of limit records available for the customer or customer group. Each LIMIT record has drill-downs, which allow the user to,

- View the LIMIT record
- View the transactions that have drawn from the Limit and their details
- View Collateral Allocation details
- View the details of all sub-allocations given to and/or taken from the Limit, Limit Cap Percentage details
- View Buffer Limit details


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


### 2.29  Sec Lim Coll


> **📇 Quick Reference Card**
> 
> **Purpose:** *When the bank maintains collaterals in an external system, the user can capture collateral value and feed into Temenos Transact . This feature enables the user to feed the external collateral value to secure Temenos Transact limit. It gives the flexibility to use the collateral maintained in the Tem...*
> 
> **Applications:** `LIMIT`
> 
> **Key Fields:** *External Collateral Currency*, *External Collateral Value*, *External Collateral value*, *Maximum Total*, *Maximum Unsecured*, *Total Ext Collateral Value*, *Total External Collateral Value*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

When the bank maintains collaterals in an external system, the user can capture collateral value and feed into Temenos Transact . This feature enables the user to feed the external collateral value to secure Temenos Transact limit. It gives the flexibility to use the collateral maintained in the Temenos Transact and the external collateral system to secure the limit in Temenos Transact .


#### ⚙️ Configuration

The configuration is covered as a part of Product configuration.


#### 🔧 Working With

If collaterals are maintained in Temenos Transact , the user can secure the limit by linking the collateral. However, if they are maintained in the external system, the user can feed the collateral values into the Transact Limit system through REST API.

The user can secure a limit in Temenos Transact using,

- Collaterals maintained in Temenos Transact
- Collaterals maintained in external system
- Combining the value of collaterals from Temenos Transact and external collateral system.

The user can feed the external collateral values into Temenos Transact Limit using the below methods.

- External system can invoke the API to create a secured limit in Temenos Transact by providing external collateral values and other required values in the API payload.
- External system can invoke the API to update the secured limit if already created in Temenos Transact with the external collateral values.

The external collateral values are fed into the below-mentioned fields in LIMIT .

| Field | Description |
|---|---|
| External Collateral Currency | Specifies the currency of the collateral from external system. |
| External Collateral Value | Specifies the value of collateral from external system. |
| Total External Collateral Value | Specifies the total collateral value in limit currency. |

The user can update External Collateral Currency and External Collateral Value only through the below APIs.

- createSecuredLimit - The external system or the user can invoke this API to create secured limit in Transact Limit System along with external collateral values.
- updateSecuredLimit - The external system or the user can invoke this API to amend an existing secured limit in Transact Limit System to update the external collateral values.

To use multiple external collaterals in different currencies, the user needs to pass the net collateral value per currency from the external system that is updated in the External Collateral Currency and External Collateral Value multi-valued fields based on the external collateral currency.

For example, if the user wants to use the following external collaterals to cover the secured limit in Temenos Transact .

| Collateral | Currency | Amount |
|---|---|---|
| Ext Coll 1 | USD | 10000 |
| Ext Coll 2 | USD | 5000 |
| Ext Coll 3 | EUR | 8000 |

The user must provide the following details for supplying the external collateral values through API.

- External Collateral Currency – USD
- External Collateral Value – 15000 (10000+5000)
- External Collateral Currency – EUR
- External Collateral value - 8000

> **⚠️ Note:** Total Ext Collateral Value is a system-maintained field to hold the sum of external collateral value in the currency of limit.

Temenos Transact emits the business event to create or update the limit and the external collateral system can subscribe it.

The external collateral system supplies any changes to the external collateral value by invoking the update API to limit.

When the internal and external collateral values are used to secure the Limit, the system prioritises the external collateral during collateral allocation process. If the entire amount cannot be covered by external collateral, the system uses internal collateral to cover the remaining amount.

For a Limit with Maximum Total of USD 10,000 to be secured. It has External Collateral value of USD 6,000 and internal collateral of USD 7,000.

The allocation happens as given below.

- External collateral – USD 6,000
- Internal Collateral – USD 4,000
- Total – USD 10,000

In this scenario, USD 3,000 from internal collateral is unutilised.


##### Deriving the Online Limit with External Collaterals

When the collateral values stored in external system secure the limit, the system derives the online limit as mentioned below.

- When the external system maintains the collateral, then the system derives the online limit by the least of the following limit amounts: Maximum Total Sum of External collateral value ( Total External Collateral Value ) + Maximum Unsecured Amount ( Maximum Unsecured )
- When the collaterals from both Temenos Transact and External system secure the limit, then the system derives the online limit by the least of the following limit amounts: Maximum Total Sum of Secured Amount (Secured Amt) + Value secured by External collateral ( Total Ext Collateral Value ) + Maximum unsecured amount ( Maximum Unsecured )


#### 📋 Tasks

There are no Tasks available for Securing Limits with External Collaterals feature.


#### 📊 Outputs

There are no Outputs available for Securing Limits with External Collaterals feature.


> **Related Applications:** `LIMIT`

---


### 2.30  Special Limit Processing for Foreign Exchange


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Buy-side of FX contracts is used in the LIMIT application. The bought amount is converted to the currency of the limit and monitoring is performed in the usual way.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The Buy-side of FX contracts is used in the LIMIT application. The bought amount is converted to the currency of the limit and monitoring is performed in the usual way.

Foreign exchange limit netting is optional and can be activated or deactivated when required. If FX limit netting is active, then all foreign exchange deals that are equal and opposite are netted.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

There are no Tasks available for Special Limit Processing for Foreign Exchange feature.


#### 📊 Outputs

There are no Outputs available for Special Limit Processing for Foreign Exchange feature.

---


### 2.31  Time Banding of Limits


> **📇 Quick Reference Card**
> 
> **Purpose:** *This facility enables the different limit amounts to be applied to contracts with different maturity dates. This is based on the concept that ‘the further forward the maturity date of a transaction, the greater the associated risk’. The whole limit is therefore available for the most immediate time ...*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

This facility enables the different limit amounts to be applied to contracts with different maturity dates. This is based on the concept that ‘the further forward the maturity date of a transaction, the greater the associated risk’. The whole limit is therefore available for the most immediate time slice and the amount decreases as the maturity increases.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

There are no Tasks available for Time Banding of Limits feature.


#### 📊 Outputs

There are no Outputs available for Time Banding of Limits feature.

---


### 2.32  Update Approved


> **📇 Quick Reference Card**
> 
> **Purpose:** *The umbrella structure and processing defines the limit hierarchies where top level limits (marked as reporting limits) are an aggregation of the lower level limits which the credit committee approves (marked as validation limits). The latter limits can be split into several layers of utilisation li...*
> 
> **Key Fields:** *Advised Amount*, *Amount*, *Default Advised*, *Default Max Total*, *Internal*, *Internal Amount*, *Key Type*, *Limit Type*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The umbrella structure and processing defines the limit hierarchies where top level limits (marked as reporting limits) are an aggregation of the lower level limits which the credit committee approves (marked as validation limits). The latter limits can be split into several layers of utilisation limits (marked accordingly).

The LIMIT.REFERENCE and LIMIT applications have both been enhanced with the Reservation option in their Limit Type field. This facilitates the creation of Reservation Limit products, respectively, Reservation Limit records.

Such limits have the role of reserving funds from the Validation Limit and allowing them to be sub-allocated to the lowest level Utilisation Limit. The Reservation Limit cannot be linked directly to a contract.


#### ⚙️ Configuration

The Non-shared limit structure uses the alpha-numeric limit keys.


##### Configuring Limit Parameter for Alphanumeric Limit Key

To create LIMIT records with alphanumeric limit key, the SYSTEM record of the LIMIT.PARAMETER application must have Key Type field set to Txn Ref. Further, the Default Advised field must be set to Internal and Default Max Total field must be set to Advised.

If an existing user wants to adopt the alphanumeric limit key, then he has to set the Key Type field in the SYSTEM record to Txn Ref in the LIMIT.PARAMETER application. This still allows the user to use the existing LIMIT records that have the original key type or even create new ones with original key type but with the condition that an already defined Limit product is used, or new Limit products are created with Key Type set to Limit Key and Limit Type field is left blank (in the LIMIT.REFERENCE application).

- Key Type field in LIMIT.PARAMETER application becomes a no input field after record is committed and authorised.
- Key Type field in LIMIT.REFERENCE offers the flexibility to create Limit products that hold limits with either original or alphanumeric limit key. Parent and child products must have the same value of this field, mixed values are restricted in the same product structure.

If an existing user wants to use the original limit key structure, he has to set the Key Type field in SYSTEM record to Limit Key in the LIMIT.PARAMETER application, or leave it blank.


##### Configuring the Classification of a Limit Product

The LIMIT.REFERENCE application enables the classification of a Limit product via the Limit Type field and indicates whether a buffer limit can be extended to a given Limit product.

The Limit Type field allows the classification of a Limit product. It can be classified as follows:

- Validation – Limits in this reference follow the validation limit processing rules, that is, only Internal Amount can be entered and constitutes the parent of utilisation limits under it. Credit check is not performed for limits of this limit type.
- Utilisation – Limits in this reference follow the utilisation limit processing rules, that is, both Internal Amount and Advised Amount must be filled. Credit check is performed on these limits and can be linked to arrangements and contracts.
- Null – Limits in this reference are not part of a structure that holds validation and utilisation limits.

If a

with ID 1100 holds the validation level and

with IDs 1130 and 1180 holds the utilisation level, the following structure can be created:

- Reference 1100 with designated children 1130 and 1180.

- References 1130 and 1180.

The LIMIT application has two similar fields to classify the limit records for the limit types and for the creation and maintenance of buffer limits.


##### Configuring Reservation Limit

In order to create Reservation Limit records, first Reservation Limit products have to be created for them. For this, a limit product has to be created in the LIMIT.REFERENCE application, with the Limit Type field set as Reservation:

Funds reserved can consist either funds approved at the Validation Limit level but not granted to the customer, either funds approved at the Buffer Limit level and sub-allocated to the Validation Limit, either both.

When sub-allocating from the Buffer Limit to the Validation Limit with a future date, funds are reserved on the level of the Buffer Limit in order to ensure their availability when the sub-allocation becomes effective.


#### 📋 Tasks

There are no Tasks available for Non-Shared Limit Structure feature.


#### 📊 Outputs

There are no Outputs available for Non-Shared Limit Structure feature.

---


### 2.33  Updating Limit Exposure


> **📇 Quick Reference Card**
> 
> **Purpose:** *The exposure against the Limit can be updated in near real time by using the Delay Txn Update field in the LIMIT.PARAMETER application. This is offered as an alternative to the real-time update of the Limit and it has effect only on Limit records which have been created under Limit products that hav...*
> 
> **Key Fields:** *Check Limit*, *Default Check*, *Delay Txn Update*, *Fx Or Time Band*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The exposure against the Limit can be updated in near real time by using the Delay Txn Update field in the LIMIT.PARAMETER application. This is offered as an alternative to the real-time update of the Limit and it has effect only on Limit records which have been created under Limit products that have been parametrized to be for information purposes only.

This reduces the effect of locking contention between parallel processes in scenarios where the bank does not use Temenos Transact Limits module for credit checking purposes.


#### ⚙️ Configuration

To stop updating the exposure against a Limit in real time and avoid locking contention, a near real-time service can be used instead. This has effect only on Limits which have been created under Limit products that have been parametrized with Fx Or Time Band set to ‘In’. The Default Check field determines whether Online Limit check takes place or not, whether excess overrides are generated or not and whether exception log is updated or not.

The Limit products (that is, LIMIT.REFERENCE records) which are created for this purpose must be correctly parametrized in the LIMIT.PARAMETER application to the appropriate application they will be used for.

When the Delay Txn Update field in the LIMIT.PARAMETER application is set to Yes, it triggers a service that will record and maintain all the exposure details of a Limit and then update the LIMIT record with all the exposure in a near real-time manner.

The system has been modified as follows:

- LIMIT records created under Limit products with Fx Or Time Band set to ‘In’ and Default Check set to Suppress will not be updated at all – neither directly by transactions in real time nor by the dedicated service in near real time.
- LIMIT records created under Limit products with Fx Or Time Band set to ‘In’ and Default Check set to No or Null will not be updated directly by transactions in real time; instead, they will be updated by the dedicated service in near real time, as long as the service has been activated (that is, Delay Txn Update = Yes in LIMIT.PARAMETER ). No online Limit check takes place, no excess overrides are generated and no exception log is updated.
- If the service is activated, then LIMIT records created under Limit products with Fx Or Time Band set to ‘In’ and Default Check set to Y will also be updated by the dedicated service in near real time. The difference is that Online Limit check takes place, excess overrides are generated and exception log is updated.

The following table shows a more detailed view of how the system will behave based on the value set in the Default Check field from the Limit products defined in the LIMIT.REFERENCE application and the value set in the Delay Txn Update field from the LIMIT.PARAMETER application:

| Default Check | Delay Txn Update | System Behaviour |
|---|---|---|
| Y | Yes | Online Limit check takes place. Exposure is updated via service. Excess overrides are generated and exception log is updated. |
| No/Null | Online Limit check takes place. Exposure is updated directly on Limit record. Excess overrides are generated and exception log is updated. |  |
| Suppress | Yes | Parametrization is disregarded. No online Limit check takes place. Exposure is not updated at all. |
| No/Null |  |  |
| No/Null | Yes | No online Limit check takes place. Exposure is updated via service. No excess overrides are generated and no exception log is updated. |
| No/Null | No online Limit check takes place. Exposure is updated directly on Limit record. No excess overrides are generated and no exception log is updated. |  |

In case of manually created LIMIT records, if the user does not set any value in the Check Limit field, then upon validation/commit, the system will default its value from the Default Check field of the LIMIT.REFERENCE record linked to the Limit. Otherwise, if the user manually sets in the Check Limit field any other value than the one from the Default Check field of the LIMIT.REFERENCE record, then the value set in the Check Limit field will take precedence.

In case of automatically (system) created Limit records, the value in the Check Limit field will be inherited by default from the Default Check field of the LIMIT.REFERENCE record.


#### 📋 Tasks

There are no Tasks available for Updating Limit Exposure through Dedicated Service feature.


#### 📊 Outputs

There are no Outputs available for Updating Limit Exposure through Dedicated Service feature.

---


### 2.34  Utilisation of Limits


> **📇 Quick Reference Card**
> 
> **Purpose:** *The limit is utilised by the business application linked to it. Limit amount can be utilised:*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The limit is utilised by the business application linked to it. Limit amount can be utilised:

- Directly by the linked contract
- Percentage of contract value
- In the same or different currency from the limit currency


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

There are no Tasks available for Utilisation of Limits feature.


#### 📊 Outputs

There are no Outputs available for Utilisation of Limits feature.

---


---


## Chapter 3: Limits_Collateral - OV


Limits_Collateral - OV module of Temenos Transact


### Features in Limits_Collateral - OV


| # | Feature | Sections |
|---|---------|----------|
| 3.1 | Misc | Intro |
| 3.2 | Direct | Intro, Confi, Worki, Tasks, Outpu |
| 3.3 | Facility Based Lending | Intro, Confi, Worki, Tasks, Outpu |
| 3.4 | Misc | Intro |
| 3.5 | RealTimeValuation | Intro, Confi, Worki, Tasks, Outpu |


### 3.1  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *Collateral is the asset pledged by the customer as security for a financial facility provided by the financial institution.*
> 
> **Applications:** `CODE`, `COLLATERAL`, `COLLATERAL.CODE`, `COLLATERAL.RIGHT`, `COLLATERAL.TYPE`, `CUSTOMER.COLLATERAL.TYPE`, `TYPE`
> 
> **Key Fields:** *Application*, *Application Input*, *Cash Collateral*, *Central Bank Value*, *Collateral Right*, *Collateral Right Id*, *Execution Value*, *General Ledger Value* ... +8 more
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- API
- Temenos Transact Services

Collateral is the asset pledged by the customer as security for a financial facility provided by the financial institution.

- Ship
- House
- Painting
- Sculpture
- Single stamp (or an entire collection)
- Customer deposit
- Portfolio

These collateral items are revalued against the prevailing market value on a regular or ad hoc basis. A right or link to collateral items are established to cover the liabilities of the customer.

Collateral items maintained in Temenos Transact can be valued automatically.

- Deposit account
- Fixed term deposit
- All or part of customer portfolio stocks and shares


##### Product Configuration

The following table lists the module and product information for the Collateral functionality in Temenos Transact :

| Module/Product | Usage |
|---|---|
| CO | The Collateral (CO) product needs to be installed to use the basic Collateral functionality in Temenos Transact . |
| MV | The Margin Valuation (MV) product needs to be installed to configure and use the CO.VALUATION.PARAMETER application in the Advance Collateral processing. The CO product or SC product is a pre-requisite for installing the MV module. |
| CX | The Advance Collateral (CX) product needs to be installed to use the advance collateral features and derive the collateral value considering the concentration cap and currency hair-cut, as applicable to the collateral asset. The CO product and MV product are pre-requisites for installing the CX module. |
| COPOOL | The Collateral Pool (COPOOL) module enables the Corporate Collateral Pool functionality. The CO product is a pre-requisite for installing the COPOOL module. |

Configure the following parameters to use the Collateral module in Temenos Transact :

This is a company level application, which sets out high-level parameters that control the Collateral module. The parameters include:

- Maintaining the number of changes to collateral revaluation in the COLLATERAL application
- Considering account balance when deposit account is given as collateral
- Online update of cash collaterals (if required)
- Online collateral valuation (if required)
- Defining the currency and forex risk margin to cover the currency conversion risk factor
- Contract sequence routine defined in EB.API can be attached in the Contract Seq Rtn field.

The contract sequence routine instructs the system to apply a different collateral allocation order for the contracts returned, compared to the standard pro-rata allocation.

In this example, a contract sequence routine has been set up in COLLATERAL.PARAMETER , which returns the contracts in the order in which the transactions take place. The collateral amount is not allocated based on pro-rata allocation; instead, it is allocated based on the execution value for each Limit. This means that when more than one Limit is linked to the same Collateral Right , the amount assigned to each Limit is used by contracts. One Limit is not borrowed from another Limit’s assigned collateral amount. The following Limit structure has been created:

- Validation Limit LI0000101030 with Internal Amount = 50,000.
- Utilisation Limit LI0000101031 with Internal Amount = 30,000, but with an Online Limit = 22,500 based on the Execution Value of the collateral linked to the Limit.
- Utilisation Limit LI0000101032 with Internal Amount = 20,000, and an Online Limit equal to the Internal Amount ; both this and the previous Limit are linked to the same Collateral Right .
- Collateral Right COR09362S124H showing the two Utilisation Limits linked to it and the collateral to which they pertain.
- Collateral CO09362G674G showing the total Execution Value of the two Utilisation Limits and the Collateral Right Id to which they are linked:
- Collateral Allocation showing the allocated amount (that is, Execution Value ) for each of the Utilisation Limits:
- The two records in the LIMIT.TXNS application showing the contracts that utilised each Limit:

By disbursing the above contracts and running LI.CONTRACT.ALLOCATION.SERVICE, ECB displays the following details for each contract:

- Contract 10017194202 is disbursed for 6,000 by utilising Limit LI0000101031; given that Online Limit = 22,500, the system allocates the full amount for the transaction:
- Contract 10017194203 is disbursed for 15,000 by utilising Limit LI0000101031; given that Online Limit = 16,500, the system allocates the full amount for the transaction:
- Contract 10017194204 is disbursed for 25,000 by utilising Limit LI0000101032; given that Online Limit = 20,000, the system could have allocated a total of 21,500 for the transaction since there are still 1,500 not utilised for Limit LI0000101031; however, because of the contract sequence routine that has been initiated, the system allocates only the 20,000 assigned for this Limit:

| ID | Type | Description |
|---|---|---|
| 100 | CASH | All types of Cash, Accounts, Money Market (MM), Loans & Deposits (LD) and Deposit Contracts |
| 200 | HOUSE | All forms of property; from domestic to industrial properties |
| 300 | ART | Includes paintings, sculpture, jewellery and so on |
| 400 | SHARES | Value of a customer's shares |

This application is used whenever the Execution Value field (if defined as a percentage of Nominal Value field in the COLLATERAL.TYPE application) is different for specific customers. To input a record in this application, the Execution Value field in the main COLLATERAL.TYPE application must be defined in the %N format. The record ID format of this application is - .

COLLATERAL.TYPE ID– 600

If the Nominal Value is F, the Execution Value is 100%N and when a real estate worth USD 100,000 is attached to a collateral belonging to this type, then the Nominal Value field defaults to USD 100,000 and the Execution Value field is also USD 100,000 (that is 100%N).

For customer 190201, if the Execution Value is desired as 65%N, then a record with ID 190201-600 is created in the CUSTOMER.COLLATERAL.TYPE application and the Execution Value is defined as 65%N.

For the same collateral defined above, the Execution Value for the customer 190201 is calculated as USD 65,000 (that is, 65% of the Nominal Value ).

| COLLATERAL . TYPE | Description | COLLATERAL . CODE | Description |
|---|---|---|---|
| 100 | Cash | 101 | MM Deposits |
| 102 | LD Deposits |  |  |
| 103 | Savings Accounts |  |  |
| 200 | Houses | 201 | Business Property |
| 202 | Domestic Property |  |  |


##### Illustrating Model Parameters

This section covers the high-level parameterisation setup that defines and controls the collateralised limits.

| S.No. | Parameters | Description |
|---|---|---|
| 1. | COLLATERAL.PARAMETER | This application allows the user to define the company-level system parameter. User can define if address is to be defaulted from CUSTOMER application. To cover the currency conversion risk factor, margin for the collateral currency is also defined when limit currency is different from collateral currency. To retain collateral records in live table, retention period value must be defined in the collateral parameter setup. Specification to determine which balance from EB.CONTRACT.BALANCES table to be considered for updating in collateral record. |
| 2. | COLLATERAL.TYPE | This application allows the user to define different types of collaterals like building stocks and guarantees and so on. Information in this table enables the client to arrive at collateral value, revaluation of collateral value and linking to other applications in Temenos Transact . Market value or face value of the collateral, value for general ledger purpose, third party value (value of collateral item outside Temenos Transact ) are specified in this table. |
| 3. | COLLATERAL.CODE | This application allows the user to determine how collateral values are re-allocated across central bank reporting lines. Enables the system to perform recalculation of percentage of collateral cover applicable. Enables the system to mention the default review frequency. Enables the system to mention the default review frequency. Enables to update Allocated Balance type, Utilized balance type and Unutilized balance type. |
| 4. | COLLATERAL.EXCLUSION | This application allows the user to define the criteria for the exclusion of collaterals. CURRENCY, COUNTRY, SECURITY.CODE, INDUSTRY, ISSUER and COUNTERPARTY values are used to define the criteria. |
| 5. | CO.CURRENCY | This application allows the user to define the rules to modify the lower advance ratio of the assets valued in a currency. Enables the user to define the currency level concentration cap. Enables the user to define the specific margin rates at product level. |
| 6. | CO.VALUATION.PARAMETER | This application allows the user to define the margin calculation, asset allocation, asset valuation for the collateral process. Enables the user to specify if the collateral is allocated against limits or liabilities. Enables the user to mention the discretionary portfolios. |
| 7. | CUSTOMER.COLLATERAL.TYPE | This application allows the user to define specific collateral execution value for specific customers. |
| 8. | CO.ELIGIBILITY | This application allows the user to define the eligibility rules for collateral against the limit products to which the collateral is linked. |
| 9. | CO.INDUSTRY | This application allows the user to define the concentration cap at industry levels for security assets. |
| 10. | CO.RANKING | This application allows the user to define the ranking rules for the collaterals against limit products. |
| 11. | CO.COUNTRY | This application allows the user to define the concentration cap rules for the collateral country. |
| 12. | CO.COUNTRY.GROUP | This application allows the user to define the concentration cap rules for a group of countries. |


> **Related Applications:** `CODE`, `COLLATERAL`, `COLLATERAL.CODE`, `COLLATERAL.RIGHT`, `COLLATERAL.TYPE`, `CUSTOMER.COLLATERAL.TYPE`, `TYPE`

---


### 3.2  Direct


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Online Valuation (OV) module handles the margin lending and buying power functionalities.*
> 
> **Applications:** `ASSET.BY.CATEG`, `ASSET.CODE`, `ASSET.TYPE`, `COLLATERAL`, `COLLATERAL.TYPE`, `CUSTOMER.COLLATERAL.TYPE`, `DX.PARAMETER`, `DX.PARAMETER(N)` ... +12 more
> 
> **Key Fields:** *Account No*, *Adj Margin*, *Adj Short Pos*, *Approved Issuer*, *Asset Type*, *Buffer*, *Buy*, *Buying Power* ... +81 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The Online Valuation (OV) module handles the margin lending and buying power functionalities.

Margin lending is a type of loan that allows you to borrow money to invest, by using your existing shares, managed funds, cash or your entire portfolio holding as security. It is a type of gearing, which is borrowing money to invest. The amount that can be borrowed depends on the loan to value ratio (margin rates) of the portfolio assets.

There are two margin lending solutions:

- Old – The entire portfolio is assumed to be pledged. There is no collateral created. The value of the portfolio is evaluated based on settings in OV.PARAMETER and margin rates and the buying power is calculated on the assumption that the entire portfolio is pledged.
- New – Any part of the portfolio or any instruments alone can be pledged. The module supports the margin lending workflow starting from a customer applying for a margin loan and specifying the assets he wishes to pledge, sanctioning of the same by the bank, creating a collateral with the assets pledged by the customer, creating a loan linked to the collateral and tracking the utilisation of the same.

It also calculates the buying power available to the customer when an order is placed, based on which loan is utilized to place the order.

This user guide describes the old margin lending functionality.


#### ⚙️ Configuration

The following section describes the parameter configuration for this feature.


##### ConfiguringOV.PARAMETER

The Margin Lending field in OV.PARAMETER record should be set to YES, which enables the buying power and loan eligibility calculations . There is also a field for margin lending in SEC.ACC.MASTER to identify the margin lending portfolios. It is set only if the Margin Lending field is set in OV.PARAMETER record.

Other settings in OV.PARAMETER are explained in the Working with section.


##### Setting up Margin Rates

The first configuration is to set up the margin rates to be used to evaluate the lending value of a portfolio. These can be set at different levels as shown in the diagram below.


###### ConfiguringASSET.TYPE

This application is used to define the top-level division of the assets and liabilities of a portfolio. Transact modules linked to the Portfolio Management system (other than Securities), must be defined as an application record in the ASSET.TYPE application shown below. This must be done before the module is included in the Portfolio Management system as shown in the below screen shot.

If a module is not set-up on the ASSET.TYPE file, no assets or liabilities for that module is recorded in the Portfolio Management files, even if the transaction is linked to a portfolio. Input the module in the Interface To field. Only those applications that appear in the drop-down in the Interface To field are linked to the Securities (SC) module.

The Report Sub Total field is linked to the SC.VAL.REP.SUB.TOTAL application and allows the user to group ASSET.TYPE records together for reporting purposes. If this field is blank for an ASSET.TYPE record that is used to define a group of accounts, then any account linked to this ASSET.TYPE is considered by the Portfolio Management system for information alone and have a zero value. ASSET.TYPE records linked to assets and liabilities (which are not part of the SC module), only use the Margin Rate field. The ASSET.TYPE for SC application - Shares is shown below.

ASSET.TYPE records for the Securities module are used to define a type of security such as shares or bonds as shown in the above example. Thus the ASSET.TYPE application is the top-level portfolio asset and liability file. For example, if the user wants to separate Bonds, so that fixed and variable rate instruments belong to different ASSET.TYPEs.

To provide even detailed descriptions of each ASSET.TYPE, Transact uses the SUB.ASSET.TYPE application. A new field called Concentration Cap is introduced to capture concentration cap.


###### ConfiguringSUB.ASSET.TYPE

The SUB.ASSET.TYPE allows a more granular definition of asset types. Instruments can be classified in multiple ways and this can be achieved using this application. It can also be used to define fees and taxes and for various reporting.

Any number of SUB.ASSET.TYPES can be defined for asset types that pertain to securities.

For modules other than Securities, each module requires a default SUB.ASSET.TYPE record to be set-up, which must be linked to the ASSET.TYPE record for that module (as shown above). If this default SUB.ASSET.TYPE record is not set-up, then no assets or liabilities for that module is recorded in the Portfolio Management files, even if the transaction is linked to a portfolio. An example of such a SUB.ASSET.TYPE - Non-SC application record is shown in the below screen shot.

For these non-SC application SUB.ASSET.TYPE records, only one per ASSET.TYPE is permitted. There is no facility, for example, to enable the splitting of, say, loans, deposits, leases etc. Therefore, if the Loans and Deposits (LD) module is linked to the securities module in this way, all LD transactions in respect of the portfolio are listed together.

Each SECURITY.MASTER record (which defines an individual Security on Transact - see the Securities User Guide) has to be linked to a SUB.ASSET.TYPE record. As each SUB.ASSET.TYPE in turn has to be linked to an ASSET.TYPE record then this defines the breakdown of a portfolio’s Securities assets and liabilities.

The SUB.ASSET.TYPE application provides the user with an opportunity to separate the various security types into meaningful types of paper that in turn enables structured revaluations, statements (both by enquiry and by report) and so on. The user can set-up as many SUB.ASSET.TYPE records as possible and unlike the non-SC applications, any number may be linked to one ASSET.TYPE record.

A SUB.ASSET.TYPE record ID may be set-up to comprise of up to five either/or/both alpha and numeric characters. Each SUB.ASSET.TYPE-SC application record must be linked to the Securities module as shown in the screenshot below:

The SUB.ASSET.TYPE application also contains attributes that are common to the particular class or group of instruments. These values are defaulted to equivalent fields in the individual instrument master (SECURITY.MASTER or DX.CONTRACT.MASTER) records, that belong to this SUB.ASSET.TYPE . However, they can be changed at the individual instrument master level.


###### ConfiguringASSET.BY.CATEG

In addition to using the default ASSET.TYPE and SUB.ASSET.TYPE the assets and liabilities of a particular CATEGORY can be linked to a specific SUB.ASSET.TYPE (and hence to a corresponding ASSET.TYPE) by using the ASSET.BY.CATEG application shown below.

In the above screenshot, forward forex contracts (Category 20000) are linked to SUB.ASSET.TYPE ID 2 rather than use the default SUB.ASSET.TYPE for the FOREX module. Another use of this file is to link different types of ACCOUNT(identified by having different cetegory codes) to different SUB.ASSET.TYPE records thereby allowing the system to report on them separately.

A new field called Concentration Cap ( to be considered for the sub asset type) is introduced to capture concentration cap.


###### Individual Customer Margins

SC.CUSTOMER.MARGIN specifies at portfolio and customer levels, the margin rate used for computing the margin value of a security holding. The values specified in this file is the first level of validation for calculating margin value for the various assets/liabilities held by the portfolio. If the margin is defined for a specified security, sub-asset type, asset type or for all securities (by specifying ALL in ASSET.CODE ), this is used in the order mentioned above for computation of margin. It takes precedence over the margin specified at the security, sub-asset type or asset type level. Depending upon whether a valuation must include or exclude liabilities (based on Margin Value in SC.PARAMETER record), either the Loss Margin Rate or the Margin Rate field is used to calculate the margin value.

The priorities used when obtaining the margin percentage are as follow:

| Instruments | File Definition | Priority |
|---|---|---|
| Security Instruments | SC.CUSTOMER.MARGIN table – Portfolio level – Security Master | 1 |
|  | SC.CUSTOMER.MARGIN table – Portfolio level – Sub Asset Type | 2 |
|  | SC.CUSTOMER.MARGIN table – Portfolio level – Asset Type | 3 |
|  | SC.CUSTOMER.MARGIN table – Portfolio level – ALL | 4 |
|  | SC.CUSTOMER.MARGIN table - Customer Number – Security Master | 5 |
|  | SC.CUSTOMER.MARGIN table - Customer Number -Sub Asset Type | 6 |
|  | SC.CUSTOMER.MARGIN table - Customer Number – Asset Type | 7 |
|  | SC.CUSTOMER.MARGIN table - Customer Number - ALL | 8 |
|  | Security Master | 9 |
|  | Sub Asset Type | 10 |
|  | Asset Type | 11 |
| Money Market, FX etc. (i.e. not Securities or Fiduciaries) | SC.CUSTOMER.MARGIN table – Portfolio level – Sub Asset Type | 1 |
|  | SC.CUSTOMER.MARGIN table – Portfolio level – Asset Type | 2 |
|  | SC.CUSTOMER.MARGIN table – Portfolio level – ALL | 3 |
|  | SC.CUSTOMER.MARGIN table – Customer Number – Sub Asset Type | 4 |
|  | SC.CUSTOMER.MARGIN table – Customer Number – Asset Type | 5 |
|  | SC.CUSTOMER.MARGIN table – Customer Number – ALL | 6 |
|  | Security Master | 7 |
|  | Sub Asset Type | 8 |
|  | Asset Type | 9 |
| Fiduciaries | Contract level | 1 |
|  | SC.CUSTOMER.MARGIN table – Customer Number – Sub Asset type | 2 |
|  | SC.CUSTOMER.MARGIN table – Customer Number – Asset type | 3 |
|  | SC.CUSTOMER.MARGIN table – Customer Number – ALL | 4 |
|  | FID parameter level | 5 |
|  | Sub Asset Type | 6 |
|  | Asset type | 7 |

> **⚠️ Note:** It is possible to specify within individual portfolios whether or not margining is to be performed. Within the portfolio ( SEC.ACC.MASTER ), the Margin Allowed field is set to a value of NONE, in which case no margin calculations are done. If the user leaves this filed blank, then the rules discussed above are applicable.

As explained earlier, the valuations and their margined equivalents are stored in the SC.POS.ASSET file. If these assets are to be used as collaterals, these values are updated into the COLLATERAL application. Depending upon the settings in COLLATERAL.TYPE , either ESTIMATED or MARGIN values are picked up by the Collateral system.

Further margins are applied to the execution value – using the COLLATERAL.TYPE application. The collateral type level margins are defined for a particular customer at the CUSTOMER.COLLATERAL.TYPE application.

Read Collateral user guide, for more information.

The SC.CUSTOMER.MARGIN application allows the definition of specific advance ratios for a given customer and security combination. It can also be used to define advance ratios for a customer at the level of products. New fields are introduced in SC.CUSTOMER.MARGIN for this purpose:

| Field | Description |
|---|---|
| Xx-Xx | Value in the field must be greater than the previous field, that is, value of 2nd sub-value must be less than first sub value |
| Xx-Xx-Tier Margin Rate | Value must be within 0 to 100 |
| Tier Adj Margin Rate | Value must be within 0 to 100 |
| Concentration Cap | Concentration cap for each asset |
| Customer Ccy | Currency in which Deficit / Surplus has to be reported |


###### Customer Level Margin Rates

The example below explains how to set up the expiry and effective dates. Consider a scenario where a customer needs a short-term loan of 550k in a month’s time for a period of three months. The customer pledges a bond he holds as a collateral. The face value of the bond is 700k. The customer is highly regarded, considered a good credit risk by the bank and so enjoys preferential treatment.

- Current Date - 01/04/2017
- Effective Date - 01/05/2017
- Expiry Date - 31/07/2017
- Default Margin Rate for the corporate bond - 75%
- Customer Specific Margin Rate - 80%

The first revaluation on the Effective Date (1/05/2017) the bond is valued at 560 (80% of 700k). On the expiry date, the system defaults to the default margin rate and is revalued to 525 (75% of 700k).


#### 🔧 Working With

The following section describes the margin calculation methods, margin checks, buying power and other related features.


##### Margin Calculation

This section describes the standard and alternative margin calculation methods.

|  | Securities | Non Securities Assets | Non Securities Liabilities |
|---|---|---|---|
| 1 | SC.CUSTOMER.MARGIN - See table below for defaulting order | ASSET.BY.CATEG - Based on Margin Rate field | ASSET.BY.CATEG - Based on Margin Rate field |
| 2 | SC.SECURITY.MARGIN | SUB.ASSET.TYPE - Based on Sec Margin Rate field | SUB.ASSET.TYPE - Based on Sec Margin Rate field |
| 3 | SECURITY.MASTER - Based on Margin Rate field | ASSET.TYPE - Based on Margin Rate field | ASSET.TYPE - Based on Margin Rate field |
| 4 | SUB.ASSET.TYPE - Based on Sec Margin Rate field | Else Margin Rate = 0 | Else Margin Rate = 0 |
| 5 | ASSET.TYPE - Based on Margin Rate field |  |  |
| 6 | Else Margin Rate = 0 |  |  |

|  | Securities | Non Securities Assets | Non Securities Liabilities |
|---|---|---|---|
| 1 | SC.CUSTOMER.MARGIN - See table below for defaulting order | ASSET.BY.CATEG - Based on Margin Rate field | ASSET.BY.CATEG - Based on Loss Margin Rate field |
| 2 | SC.SECURITY.MARGIN | SUB.ASSET.TYPE - Based on Sec Margin Rate field | SUB.ASSET.TYPE - Based on Loss Margin Rate field |
| 3 | SECURITY.MASTER - Based on Margin Control field | ASSET.TYPE - Based on Margin Rate field | ASSET.TYPE - Based on Loss Margin Rate field |
| 4 | SUB.ASSET.TYPE - Based on Sec Margin Rate field | Else Margin Rate = 0 | Else Margin Rate = 0 |
| 5 | ASSET.TYPE - Based on Margin Rate field |  |  |
| 6 | Else Margin Rate = 0 |  |  |

|  | Securities | Non Securities Assets | Non Securities Liabilities |
|---|---|---|---|
| 1 | SC.CUSTOMER.MARGIN - See table below for defaulting order | ASSET.BY.CATEG - Based on Margin Rate field | Margin Rate = 0 |
| 2 | SC.SECURITY.MARGIN | SUB.ASSET.TYPE - Based on Sec Margin Rate field |  |
| 3 | SECURITY.MASTER - Based on Margin Control field | ASSET.TYPE - Based on Margin Rate field |  |
| 4 | SUB.ASSET.TYPE - Based on Sec Margin Rate field | Else Margin Rate = 0 |  |
| 5 | ASSET.TYPE - Based on Margin Rate field |  |  |
| 6 | Else Margin Rate = 0 |  |  |


##### Margin Calculation of Derivative Positions

For derivative positions, a different approach is used for margin calculation apart from the above mentioned process.

While calculating the margin value of a portfolio, the value of derivative positions can be totally ignored. However, if there is a negative exposure on account of derivative positions, then the same can be treated as a liability by including the exposure in the Short Pos Margin field in SEC.ACC.MASTER record. DX.PARAMETER is shown below.

- Margin Calc Rtn - Defines the routine to be used for margin rate calculations.
- Netting Reqd - If set to YES, then the Same Strik e, Maturity Days and Exposure Calc fields are imputable.
- Same Strike -If is set to YES, then the contracts which have the same strike are netted together. Else, the system does not consider the strike price while netting.
- Maturity Days - Specifies the days which considers for netting parameter and all transactions within that No.of days which is grouped together for netting.
- Exposure Calc - Allowed values are MAX NEGATIVE or TOTAL NEGATIVE, if Maximum Negative or Total Negative exposure needs to be considered.

To calculate the negative exposure on account of derivative positions, the following calculations are done by the Transact.

1. Positions are grouped together, if they have the same:

1. In each group, if there are any covered calls, these transactions are ignored to the extent that they are covered.
2. In each group, similar positive positions can be netted against similar negative positions. For example; a buy call can be netted against a sell call. If the net value is positive, it shall be ignored. If the net value is negative, then it is added as an exposure.
3. The final negative exposure depends on the parameter value in Exposure Calc field. If this is set to TOTAL NEGATIVE, then the sum total of all Negative Exposures calculated in Step 3 is considered and updated to the Short Pos Mgn Amt field in SEC.ACC.MASTER record.

If the field is set as MAX.NEGATIVE, then the maximum of all the negative exposures alone are updated to the Short Pos Mgn Amt field in SEC.ACC.MASTER application.

The Short Pos Mgn Amt field is important to determine the liabilities of the portfolio and is used in calculating the security margin ratio of a portfolio. Any addition to this field on account of negative DX exposure results in reducing the overall collateral value of the portfolio.

> **⚠️ Note:** For this functionality to work the Adj Short Pos field in OV.PARAMETER record, must be set to NO.

Read Short Positions and Other Liabilities, for more information on short positions.


##### Currency Volatility Margins

The maximum amount that can be borrowed against the portfolio is called the security value of the portfolio and is determined by applying Loan to Value Ratio (LVR) assigned to each security or group of securities or assets or liabilities in the portfolio. The security value is also known as the margin value and the LVR is also known as margin rate.

For example, if a customer holds a security with market value of USD 5000 and a margin rate of 80%, then the security value of the portfolio is USD 4000 (5000 * 80%).

Margin rates can be customer specific (portfolio or customer level), instrument or asset type specific (sub-asset type, asset type).

If there is a requirement to specify currency wise margins (for example, a lower margin rate for a JPY account, when compared to an USD account), the same can be set in SUB.ASSET.TYPE or ASSET.TYPE or ASSET.BY.CATEG . It allows specification of different margins for the same asset class based on the currency of the asset. The currency-wise margins are used to automatically adjust the lending value depending on the currency of the asset (for example, lower lending value for currencies with high volatility).

| Instrument | Market Value | Margin Rate | Margin (Security) Value |
|---|---|---|---|
| USD Stock | 10000 (USD) | 80% | 8000 (USD) |
| JPY Stock | 100000 (JPY) | 70% | 70000 (JPY) |
| EUR Stock | 10000 (EUR) | 75% | 7500 (EUR) |


##### Buying Power

The concept of buying power summarises the liquidity of the portfolio. It offers a portfolio wide view of the available amount to invest. It is more comprehensive than the cash flow checks that are currently carried out as part of the order validation process.

The buying power calculation ensures that the additional risk of an order is covered by sufficient buying power. To achieve this, the execution of the order is simulated and the effects on the buying power are computed. Only if the buying power is greater than the order amount, the order is accepted and processed further. This approval process applies to all new orders as well as to the amendment of pending orders. Pending orders are orders that are already approved, but are for some reason not yet traded (for example, limit orders).

The customer’s cash accounts (including Term Money), the margin value of the customer’s securities and other assets create the buying power. Pending securities orders and other obligations reduce the buying power.

The user can set the Buying Power field in OV.PARAMETER , to ensure that the buying power validation is carried out as part of the order valuation process.

Before an order is processed, the buying power calculation engine determines whether there is sufficient buying power to meet the cost of execution. This is done by simulating the execution amount and comparing it with the buying power calculated. If the order amount is less than the buying power amount, then the system raises an override to that effect.

The overall principle of buying power validation is governed by risk aversion. Therefore, only the pending purchase orders are included in the buying power calculation and not the potential positive cash flows on account of sell orders.

The following events, trigger the buying power calculations: New orders – purchase Amendment of pending orders – purchase (only for nominal or price change)

The following events do not trigger the buying power validation: Sell order Cancellation of pending orders

Buying power is the potential amount that a customer can invest, including the cash balances, credit lines (if any) and lending value of securities (hair-cut). For a given portfolio, the buying power is calculated as:

The lending value of securities is the margin value of securities arrived at after applying the margin rates. The other assets are the other module transactions or positions linked to the portfolio and other liabilities are the other module liabilities (for example, loans) of the portfolio.

The buying power is always calculated in the reference currency of the portfolio. The calculated buying power is compared against the order amount (to determine whether sufficient buying power exists).

For example, consider Portfolio A has the following assets

- Cash balance = 354,500 USD
- Lending value of Securities = 695,000 USD
- Deposits = 200,000 USD

There is also a prior pending order for an amount of USD 5,600

The buying power of Portfolio A considering the above is USD 1243900 (354500 + 695000 + 200000 – 5600).

An adjustment factor can be applied to the purchasing power so calculated to arrive at the final amount that needs to be compared against the order amount. This adjustment factor is at the portfolio level ( Pp Adj Factor ) and is expressed as a percentage.

For example, if the calculated purchasing power is USD 600,000 and at the portfolio level, the overall adjustment factor is set as 90%, then the buying power is adjusted to USD 540,000. If no customer level adjustment is set, then the buying power is retained as USD 600,000

> **⚠️ Note:** The Pp Adj Factor field can only be set if the buying power validations are enabled. Except the adjustment factor cannot be set, if Margin Lending is set to YES in OV.PARAMETER record.

In this case, if the order amount is less than the buying power, then the order is processed straight away. Else, an override for the buying power shortfall is raised. Overrides are raised, if the calculated buying power is negative.

In the above example, buying power is calculated where no customer facilities or margins are involved. In the subsequent sections, the customer facilities, initial margins and maintenance margins are explained in detail.


##### Margin Lending

The concept of borrowing against a portfolio is described in this section.

The maximum amount that can be borrowed against the portfolio is called the Total Loan Value (TLV) of the portfolio and is determined by applying Loan to Value Ratio (LVR) assigned to each security or group of securities or assets or liabilities in the portfolio. The TLV is also known as the margin value and the LVR is also known by the Term Margin Rate.

If a portfolio holds a security (margin rate of 80%) whose market value is USD 5000, the maximum amount that can be borrowed against the portfolio is USD 4000 (5000 * 80%). Now consider another portfolio that has a position in more than one security:

|  | Market Value | Margin Rate | Loan or Margin Value |
|---|---|---|---|
| Stock A | 10000 | 70% | 7000 |
| Stock B | 15000 | 80% | 12000 |
| Bond A | 10000 | 100% | 10000 |
| Total | 35000 |  | 29000 |

Even though the total market value of the portfolio is USD 35000, the maximum amount the bank can lend against the portfolio is only USD 29000, on account of the LVRs applied to each holding.

If the customer decides to purchase more securities in the above example, then the maximum amount that he can purchase is based on the margin rate or LVR of the new security that he intends to purchase.

For example, with a margin value of USD 29000, the maximum amount of security with a LVR of 75% that can be purchased (without the customer contributing any cash) is USD 116000, as calculated below:

Buying Power =Margin Value/(1-LVR) = 29000/ (1-75%) = USD 116000

This amount is significantly higher than the amount the customer can borrow with the same loan value; as the new security that is purchased has increases the value of the portfolio. In the above example, USD 116000 is the maximum amount that the bank can lend for the stock purchase, or in other words the maximum that the customer can purchase without contributing cash by borrowing against his investments.

The portfolio position, after the purchase is explained in the below table:

|  | Market Value | Margin Rate | Loan or Margin Value |
|---|---|---|---|
| Stock A | 10000 | 70% | 7000 |
| Stock B | 15000 | 80% | 12000 |
| Bond A | 10000 | 100% | 10000 |
| Stock C (purchase) | 116000 | 75% | 87000 |
| Total | 151000 |  | 116000 |
| Loan |  |  | 116000 |

> **⚠️ Note:** The loan eligibility or buying power is calculated on the net margin value of the portfolio (after adjusting for loans or other liabilities and pending orders).

Another example of a portfolio with other liabilities and pending orders is as follows:

|  | Market Value | Margin Rate | Loan or Margin Value |
|---|---|---|---|
| Stock A | 10000 | 70% | 7000 |
| Stock B | 15000 | 80% | 12000 |
| Bond A | 10000 | 100% | 10000 |
| FX/010/120/00005 |  |  | (3000) (Estimation) |
| Stock C | (5000) |  | (5000)(Short Position) |
| Total |  |  | 21000 |

There is also an earlier pending order for purchase of 500 shares of Stock D (price – USD 10 and margin rate of 75%).

The margin value of the portfolio is adjusted to take into account the expected inflows from the pending order execution (500*10*75%) and also the order amount outflow (USD 5000).

Adjusted Loan Value = 21000 + 3750 – 5000 = USD 19750

The buying power of the portfolio (with base amount of USD 19750) for a security with 75% LVR is USD 79000 (=19750/ (1-75%)).

Basically, this is the concept of margin lending which is a form of gearing. The user can set the Margin Lending field in OV.PARAMETER record to Yes, which enables the buying power and loan eligibility calculations as shown above. There is also a field for margin lending in SEC.ACC.MASTER to identify the margin lending portfolios. It is set only if the Margin Lending field is set in OV.PARAMETER record.

As explained above, there are two distinct uses for the above calculations: To determine how much can be borrowed against a portfolio and To determine additional securities that can be purchased without cash using the existing portfolio

A customer who purchases securities may either pay for the securities in full or borrow part of the amount from the bank. The portion of the consideration that the customer pays is the customer’s equity.

While borrowing (as mentioned above) has the potential to increase the returns, the losses can also potentially increase. Falls in the market value of the portfolio can make the portfolio value less than the loan amount borrowed. This results in bank raising a demand on the investor for depositing additional cash/securities or selling off securities/repaying loan for bringing the portfolio back on track. This results in what is normally known as the margin call.

A margin lending portfolio (with loans availed) is shown in the below screen shot.

Consider the portfolio value decreases on account of fall in the market value of securities.

As against the loan amount of USD 696,000 availed, the TLV of the portfolio is now only USD 674,407.50 resulting in a margin call situation. The customer must now deposit additional cash or bring in new securities to meet the margin obligation within the time stipulated for clearing the margin call.

A margin call tracker for the above portfolio is shown in the below screen shot.

If the margin call situation is not addressed within the stipulated time, then the bank constrains to 'force sell' some of the customer’s holdings.

In some cases, customers are provided a buffer which enables them to manage the portfolios into a suitable position.

This buffer can either be a percentage of the market value or the margin value of the portfolio. For example, there is a 10% buffer on the margin value (USD 67,440.75). If this is considered, then the combined value (margin + buffer) is above the loan value (USD 741,848.25 as against loan value of USD 696,000). Therefore, no margin call is triggered in this case.

To lower the chance of a margin call, caps are imposed on the maximum amount that can be borrowed against a portfolio. If the gearing level is lower, then the margin call obligation arises only if the prices fall substantially. To create a cushion against margin calls, the customers can choose to gear their portfolio at a lower level. In such cases, they receive a margin call only if the portfolio value falls substantially. The gearing levels are controlled by the Gearing field in SEC.ACC.MASTER record. In case Gearing is set for buying power, then it is calculated as:

Where, Gearing is the gearing set in SEC.ACC.MASTER record (expressed as a percentage) and LVR is the LVR of the new security being purchased.

The following sections explain the customer facility and initial and maintenance margins.

|  | Market Value | Margin Rate | Loan or Margin Value |
|---|---|---|---|
| Stock A | 31250 | 80% | 25000 |
| Cash | 50000 | 100% | 50000 |

The Adj Short Pos field in OV.PARAMETER record controls the handling of short positions and other liabilities (components with negative estimation).

If Adj Short Pos is set to: YES - Then the securities short position and other liabilities (excluding loans) and components with negative estimation is reduced from the margin value of the assets held by the portfolio. The resultant amount (net margin value) is compared against the loan amount to determine whether there is a margin call or not. NO - Then the short position and other liabilities (excluding loans) and components with negative estimation are added to the loan amount. It is compared against the eligible margin value of the assets held by theportfolio.

The following example and screen shot explains in detail.

Since the Adj Short Pos field is set as YES, the short position is reduced from the margin value. The loan amount is then compared against this adjusted margin value to determine whether there is a margin call or not. If it is set to NO, then the short position value (USD 5625) is added to the loan amount.

Adj Short Pos field has an impact on the calculations (as above), only if Facility or Initial Margin is set in OV.PARAMETER record.

The margin value or the total loan value of a portfolio is dependent on the LVRs or margin rates specified for the instrument or the asset group.

Except the standard LVRs discussed in the earlier sections, it is also be possible to define a top-up LVR and sell-out LVR. If these are defined, then the margin value of the portfolio is calculated using the top-Up LV% and sell-out LV%. The top-up and sell-out margins can be specified at all levels where the standard LVRs can be set using the Margin Control, Sub Asset Type, Asset Type and SC Customer Margin fields.

Another example of top-up and sell-out margins, but at the sub-asset type level is shown in the below screen shot.

These are additional validations governing the type of action which must be taken in case of a margin call. If the top-up and sell-out margins are specified, it is higher than the standard margin rates and this provides the customer with a buffer to manage the portfolio into a suitable position.

For example, if the margin value of the portfolio (applying the standard LVR) goes below the loan availed on any given day, then there is no action taken; in case if the top-up and sell-out margins are also specified.

- If the top-up level is breached (margin value goes below the loan amount with Top up LV %), then a top-up margin call is made. The customer is asked to pay more cash or reduce the cash or transfer in additional eligible securities within a stipulated timeframe.
- If Sell-out level is breached, it is a more serious situation demanding immediate action. A sell-out margin call is made and the bank may even initiate and take action to sell some of the securities to cover the deficit.

> **⚠️ Note:** The buying power calculations are based on standard LVRs. The Top-up and Sell-out LVRs are only used to determine the action required in respect of margin calls.

Since this is also another form of buffer, the Buffer field in OV.PARAMETER record is not set, if these margins are specified and vice versa.

Margin value (or security value) denotes the maximum amount that can be borrowed against the portfolio.

Diversification is a feature that rewards customers who diversify their portfolios. Diversification can be based on any number of criteria (number of stocks held in the portfolio, holding in a particular stock or holding in a particular group of stocks). The diversified feature allows the customers to access a greater number of securities which they can invest in and receive an LVR (or margin rate) for; and higher LVRs on most securities. The benefit to the customer is that this increases their security value (and in turn their funds available to invest) and choose between using this as a cushion between them and a margin call or increase the amount they invest.

For example, consider a portfolio that has holdings in different securities:

Even though the total market value of the portfolio is USD 151000, the maximum amount the bank lends against the portfolio is only USD 116000 on account of the LVRs applied to each holding.

In the previous example, if the customer is eligible for diversified margins, then the diversified margin value of the portfolio is as per the below screen shot.

As against the standard margin value of USD 116000, the customer is now eligible for a borrowing 130100 USD, based on the diversification margins applied. If the customer now decides to purchase more securities, the customer has to invest more. Because of the higher margin rates, the customer also has more cushion when compared to standard portfolios as regards margin call is concerned. The higher LVRs increase how far the client’s portfolio would need to fall before he receives a margin call.

The Diversified Margins can be specified in the SC.CUSTOMER.MARGIN, MARGIN.CONTROL, SUB.ASSET.TYPE, ASSET.TYPE and ASSET.BY.CATEG records by populating it in the Adj Margin field, which specifies the diversified margin rate. If specified the diversified margin rate, it is always more than or equal to standard margin rates.

There are certain stocks with diversified LVR but no standard LVR, meaning they are eligible for margin lending (or borrowing) only, if they are part of a diversified portfolio. These stocks are called Restricted stocks and are eligible for no margins in the normal course. The restricted stocks are identified based on the settings in the Restricted field in SECURITY.MASTER application. If this field is set to YES, then the stock is considered a restricted stock.

Diversification as a feature must be activated. By simply complying with the diversification criteria, portfolio are not eligible for diversified margins. If a portfolio is not eligible for diversified margins, the security value of the portfolio is determined by applying the standard margin rates; even though the portfolio complies with all the requirements of a diversified portfolio. A portfolio is considered eligible for diversification, if the Diversification field is set to YES in SEC.ACC.MASTER record.

A portfolio can be identified as diversified based on its compliance with:

- Number count rule
- Holdings rule

If the number of securities held in the portfolio is equal to or more than the number of securities required for meeting the diversification criteria, then all the holdings (for which diversified margin is specified) is eligible for diversified margins in determining the security or margin value of the portfolio. The number of stocks required for considering the portfolio as diversified is specified in Stock Held field in the OV.PARAMETER application.

The number of securities could mean:

- All the holdings of the portfolio (stocks, bonds, managed funds)
- All the eligible securities excluding the restricted securities or
- All eligible Securities including those in the restricted list.

The Stock Count Basis field in the OV.PARAMETER application controls the securities that are considered for determining the compliance with the number of stocks rule.

The diversification can also be determined based on the holding levels of a particular stock in a portfolio. For example, the higher diversified LVRs can be applied to all the stocks in the portfolio; if no stock exceeds 25% of the total value of the diversified portfolio. If any stock exceeds 25%, then the following three options are available:

- Treat the entire portfolio as a standard portfolio and apply standard LVRs on all the holdings;
- Treat the entire holding in the stock as standard and apply standard LVR on that particular holding;
- Treat the excess holding (in excess of the percentage specified) as standard and apply standard LVR on the excess and diversified LVR on the rest. In this case, there is a requirement to apply two LVRs on the same holding (currently not supported) and report them independently.

The holding cap is set in the Holding Percent field of the OV.PARAMETER application. In the Holding Action field (PORTFOLIO, POSITION and EXCESS are the allowed values), the options available, in case the holding exceeds the cap, are specified.

If both these rules are specified, then the system validates the number of stocks held first. Once this is complied, the system validates the holding caps and applies the diversified margin only when both these conditions are met.

> **⚠️ Note:** If Issuer Diversification is set, other diversifications explained above do not work.

Margin value of portfolios that are over exposed to a single or few issuers, are suitably reduced to offset any potential credit risk.

An issuer can be set for every security. The issuer need not necessarily be a Transact customer. Rules are applied to validate, if a portfolio is sufficiently diversified. If exposure to a single issuer or few issuers are very high, then the margin value is suitably reduced to manage the potential risk if any.

The user can create issuers using the SC.ISSUER application, for issuers who are not opened as Transact customers. A SC issuer record is shown below.

SECURITY.MASTER

SHARES record

An issuer can be set for every security. The Ov Issuer field accepts values C-XXXX; where XXXX is a valid CUSTOMER record or I-XXXX; where XXXX is a valid SC.ISSUER record.

> **⚠️ Note:** Issuer Diversification validation applies only based on the Issuer set in this field. Issuer set in the Issuer field is not used for this purpose.

The user must manually specify the value in the Issuer Except field, if the security is to be excluded from issuer diversification validation. A record in OV.PARAMETER is shown below and the fields are described too.

- Issuer Diverfn - Validates if issuer diversification must be performed based on margin value validation, net equity validation (or) both.
- Issuer Percentage - Holds the maximum allowed percentage for issuers (above which diversification is applied).
- Approved Issuer - Holds the list of approved Issuers.
- Except Sub Asset - Holds the list of excepted sub asset types.
- No Of Issuer - Margin value check is performed, if the number of issuer for a portfolio exceeds the setup here.
- Issuer Diverfn Rtn - Specifies the local routine for performing issuer diversification must be specified.

Three types of margin value calculations are possible based on issuer diversification, depending on the values in Diversification Type field in OV.PARAMETER record.

1. B, value A is considered as the margin value. If A
2. Net Equity Check - If set as EQUITY, net equity value of a portfolio excluding liabilities and exposures are calculated and percentage specified in parameter is applied on it, to calculate the amount that is maximum value allowed per issuer (Value A). The market value per issuer is calculated by adding market values of all the instruments pertaining to the same issuer (value B). If market value (B) A, then the margin value for each instrument is calculated using the formula: Exceptions stated above is be applicable for Net Equity validation also.
3. Both - If BOTH option is set, then lesser margin values between margin and net equity validation is the final margin value.


##### Margin Checks for Portfolio

Based on market values received for a set of positions belonging to a portfolio, Transact can calculate the margin value (based on margin rates) and check for margin surplus or shortfall (collateral availability).

The customer, portfolio, currency, security and market valuedetails are entered in the SC.ORDER.SESSION application. On validating, the system calculates the position margin value, portfolio margin value, checks the same against liabilities and flags whether credit check is cleared or not.

Upon setting the above record, Transact calculates the margin value of individual positions and the total margin value. Then these are compared against the liabilities to determine whether there is sufficient collateral.


##### Security Margin Ratio

Security Margin Ratio can be used as a credit monitoring tool for portfolios which are pledged as collateral for credit facilities availed. This ratio is compared with top-up and sell-out ratios defined at global or portfolio level and helps the bank to validate if their exposure is sufficiently covered.

The Security Margin Ratio is calculated for individual portfolios and for a group of portfolios based on second market value, margin value and liabilities.

Second Market Value is the market value of all the assets. However, assets with zero margin value is not included.

Liabilities is the total of all the negative positions including loans, overdrawn accounts and so on.

Lombard Value is the margin value of the portfolio after all haircuts. This is the total of the values in the Margin Value field in SC.POS.ASSET or SC.GROUP.POS.ASSET application.

When a customer has more than one portfolio or the portfolio of another customer is pledged to cover the liabilities of a master portfolio, then the portfolios can be grouped together for a margin call follow-up.

Using portfolio grouping, margin value of the child portfolio is linked and used by the master portfolio for any credit facility provided to the master portfolio.

The linking is done using the SC.VALUATION.GROUP application . SC.VALUATION.GROUP - The ID of this record is the master portfolio.

Grouping Portfolios for Valuation

- Child Portfolio – Holds child portfolios
- Link Type – Values can be FIXED, VARIABLE, NETTING.

For Fixed link type, the fixed amount is taken as margin value irrespective of the portfolio’s value. Only pledge amount can be defined.

For Variable link type, either the pledge amount or percentage can be defined. If pledge percentage is defined then the percentage is applied on the margin value. If pledge amount is defined then either the portfolio's margin value or pledge amount whichever is lower is considered as margin value.

For Netting Link type, the system considers the transactions of the child and the master Portfolio that can be netted and arrive at the margin value for the master portfolio. And for derivatives, additional setup are done in DX.PARAMETER .

- Pledge Pct – This percentage is applied on Margin Value field of SEC.ACC.MASTER .
- Pledge Amt – Pledge amount in reference currency of child portfolio that is considered if it is less than the Margin Value in SEC.ACC.MASTER .
- Global Limit - Holds the global limit
- Status – Needs to be set as INACTIVE to exclude the Group for Valuation
- Run Valuation – To be set as YES for online valuation of master portfolio.
- Child Valuation – Either ALL or list of portfolios that can be specified for which child valuation has to be performed.
- Last Valuation Run – Date and time of online valuation run.
- Master Portfolio - Lists the master portfolios to which this group portfolio record is pledged as the child portfolio.

Further, the global level top-up and sell-out margin rates can be set in OV.PARAMETER . These are only for information purpose and can be compared with the security margin ratio to decide on margin calls.

OV.PARAMETER

The Online Valuation parameter and its fields are explained below.

- Top Up Mgn Rate – Holds margin rate for top-up
- Sell Out Mgn Rate – Holds margin rate for sell out.
- Pricing Days – Holds cut of day of calculating pricing date. Any position where the last price is available beyond these days, is excluded from the Second Market Value
- Global Limit – Specifies the global limit (that is, in the format 10000.xxx)

SC.POS.ASSET

These fields hold Second Mrkt Value, Init Mgn Value, Top Up Margin, Sell Out Margin, Mv Margin Amt, Eq Margin Amt and their respective values.

- Init Mgn Value - Holds the original margin value calculated normally
- Margin Value - Holds the margin value after applying haircuts based on issuer diversification

SEC.ACC.MASTER

The fields in this table are: Master Portfolio – Holds parent portfolio reference Second Mrkt Value – Holds second market value Init Mgn Value – Holds initial margin value (that is; the margin value prior to adjustment for diversification) Sec Margin Ratio – Holds computed sec margin ratio Grp Estimation – Holds total group estimation Grp Sec Mkt Value – Holds second market value for group Grp.Margin.Value – Holds margin value of group Grp Init Mgn Value – Holds initial margin value of group Grp Liability – Holds liability of group Grp Sec Margin Ratio – Holds sec margin ratio for group Top Up Mgn Rate – Holds margin rate of top-up Sell Out Mgn Rate – Holds margin rate of sell out Global Limit – Specifies the global limit

SC.GROUP.POS.ASSET

This file gets updated for portfolio groups and fields are similar to SC.POS.ASSET . The Index field is updated only if application in SC.VALUE is SECURITY.NO*DEPOSITORY.

For a single portfolio, margin value, second margin value, security margin ration and so on are updated by the usual Valuation process that is; by running SC.VAL.COST service.

For a group of portfolios, margin value, second margin value, liabilities, security margin ratio and so on, are updated during COB. To update these online, the SC.GROUP.VALUATION and SC.GROUP.VALUATION.MARGIN services must be run. These services updates the SC.GROUP.POS.ASSET files and the SEC.ACC.MASTER application of the master portfolio.

The user can define negative loss margin rates to apply mark-up rate on Liabilities in Sc Customer Margin , Sub Asset Type or Asset Type fields.

The user can view the final values by running the enquiries Portfolio Lombard Value and Group Lombard Value. Some valuation update pages are shown below.


#### 📋 Tasks

Related topics:

- Manage Margin Call for Wealth Lending
- Trading Processes

Margin lending is a type of loan that allows the user to borrow money to invest by using the existing shares, managed funds and/or cash as security. It is a type of gearing, which is borrowing money to invest. Margin lending functionality allows a customer to pledge their portfolio in partial or full or to pledge select few instruments or positions to secure a Margin loan.

This module supports the margin lending workflow as follows:

1. Customer specifies the assets to pledge to apply for a margin loan.
2. Bank sanctions the loan.
3. Bank creates a collateral with the pledged assets.
4. Bank allows the user to create a loan and utilise the same for purchase of shares.


##### Workflow

This section allows the user to perform the below tasks:

| SCREENS | WORKFLOW |
|---|---|
|  | Security Margin Rates . |
| Instrumentwise Margin Rates | Enter or select values in the required fields and then click the FIND button. |
| Instrumentwise Margin Rates | Select the Amend Asset Type option from the drop-down and then click the Launch icon. |
| Asset Type | Enter values in the fields, which require amendment. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Customer Margin Rates . |
| Customer Margin Rates | Enter values in the required fields and then click the FIND button. |
| Customer Margin Rates | Click the Amend Margin icon. |
| Portfolio Margin | Enter values in the fields, which require amendment. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Margin Lending Portfolios . |
| Margin Lending Portfolios | Select the Portfolio Margin Status option from the drop-down and then click the Launch icon. The enquiry displays the list of securities along with the market price, margin value and other required details. |
| Margin Availability with Buffer | Verify the record details. |

| SCREENS | WORKFLOW |
|---|---|
|  | Eligibility Calculator . |
| Eligibility Calculator | Enter values in the Portfolio field and then click the FIND button. |
| Portfolio Details | Click the Eligibility Calculator icon. |
| Eligibility Calculator | Enter values in the mandatory fields in the enquiry selection table. The system calculates the lending eligibility for the specified portfolio. |

| SCREENS | WORKFLOW |
|---|---|
|  | Group portfolios for Lending . |
| Contract Screen | Enter or select a value in the Grouping Portfolios for Valuation field and then click the Perform Action icon. |
| Grouping Portfolios for Valuation | Enter values in the following fields: Child Portfolio.1 Link Type.1 Pledge Amt.1 Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Update Issuer . |
| Contract Screen | Enter or select a value in the SC Issuer field and then click the Perform Action icon. |
| SC Issuer | Enter a value in the Description.1 field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to real time valuation and margin lending in the core banking system.


##### Enquiries and Reports

The section helps the user to view the below enquiries and reports:

Margin Lending Portfolios(With Facility)

This enquiry displays the list of portfolios that are opted for margin lending and also enjoys the facility with the bank.

Top Up Sell Out Margin Status Report

This enquiry displays the availability of portfolio margins with top up and sell out margins at instruments and asset group levels for a given portfolio.

Margin Call Follow Up – Child

This enquiry displays the list of security margin ratios calculated for child portfolios.

Margin Call Follow Up – Master

This enquiry displays the list of security margin ratios calculated for master portfolios.

Margin Call Report

This enquiry displays the list of customers who breached the margin call as on date with the deficit details.

Top Up Margin Call Report

This enquiry displays the list of customers who breached the top up margin call as in date.

Sell Out Margin Call Report

This enquiry displays the list of customers who breached the sell out margin call as in date.

Portfolio- Lombard Value

This enquiry displays the list of positions of a single portfolio in the selected currency or portfolio reference currency.

Group- Lombard Value

The enquiry displays the list of positions of a master portfolio in the selected currency or portfolio reference currency.

Limit and Pledge Control - Portfolio

This enquiry displays the list of customers who have breached the global limit. These reports are generated either in selected currency or portfolio reference currency.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA


> **Related Applications:** `ASSET.BY.CATEG`, `ASSET.CODE`, `ASSET.TYPE`, `COLLATERAL`, `COLLATERAL.TYPE`, `CUSTOMER.COLLATERAL.TYPE`, `DX.PARAMETER`, `DX.PARAMETER(N)`, `OV.PARAMETER`, `SC.CUSTOMER.MARGIN`, `SC.GROUP.POS.ASSET`, `SC.ISSUER`, `SC.ORDER.SESSION`, `SC.PARAMETER`, `SC.POS.ASSET`, `SC.SECURITY.MARGIN`, `SC.VALUATION.GROUP`, `SEC.ACC.MASTER`, `SECURITY.MASTER`, `SUB.ASSET.TYPE`

---


### 3.3  Facility Based Lending


> **📇 Quick Reference Card**
> 
> **Purpose:** *Margin Lending is a type of loan that allows you to borrow money to invest, by using your existing shares, managed funds, cash or your entire portfolio holding as security. It is a type of gearing, which is borrowing money to invest. The amount that can be borrowed depends on the loan to value ratio...*
> 
> **Applications:** `ACCOUNT`, `SC.FACILITY.APPLN`, `SC.FACILITY.PARAM`, `SC.POS.ASSET`, `SECURITY.POSITION`
> 
> **Key Fields:** *Amount*, *Avail Amt*, *Available Nom*, *Client*, *Collateral Code*, *Collateral Id.1*, *Collateral Pledged*, *Collateral Provided* ... +18 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Margin Lending is a type of loan that allows you to borrow money to invest, by using your existing shares, managed funds, cash or your entire portfolio holding as security. It is a type of gearing, which is borrowing money to invest. The amount that can be borrowed depends on the loan to value ratio (margin rates) of the portfolio assets.

This functionality allows a customer to:

- Pledge his portfolio in part or full
- Pledge a chosen few instruments or positions to secure a margin loan.

This Online Valuation(OV) or Real Time Valuation module supports the following margin lending workflow: Applying for a margin loan by a customer Specifying the asset he wishes to pledge Sanctioning of the loan by the bank Creating a collateral with the assets pledged by the customer Allowing the user to create a loan and utilize the same for purchase of shares.

This module works closely with the Collateral (CO) module to ensure detailed evaluation of the assets pledged as collateral. It has reports that track the utilisation of the loan and highlights any collateral shortfall or margin call situation. It also calculates the buying power available to the customer when an order is placed, based on which loan is utilised to place the order.


#### ⚙️ Configuration

The following are some parameters that must be configured for margin lending products.

The Use Facility Application field in OV.PARAMETER must be set to YES, to enable the enhanced margin lending functionality.

The type of facilities or loans that private wealth customers are allowed to avail is captured in SC.FACILITY.PARAM application (Example: Lombard, Margin Loans, etc). It is used to parameterise a set of questions that need to appear on the SC.FACILITY.APPLN .The details in this application are used while updating the facility application received from a client.

> **⚠️ Note:** This application allows input only if the Use Facility Application field is set to Yes in OV.PARAMETER The system allows a record to be created in SC.FACILITY.APPLN, only if the CO module is installed in the company where the facility is being created. In a multi-company setup, when the portfolio ( SEC.ACC.MASTER ID) is entered in SC.FACILITY.APPLN , the system checks if the CO module is installed in the portfolio company ( Port Comp Id ) If a record in the SC.COLLATERAL application already exists for the portfolio created through the non-facility process, then a record in SC.FACILITY.APPLN cannot be created. Then, the collateral has to be liquidated and pledged through SC.FACILITY.APPLN again.


#### 🔧 Working With

This section describes the workflow for creating a lending product using the SC.FACILITY.APPLN application. The below flowchart indicates the step-by-step workflow for creating a lending product within wealth suite.


##### Applying for Margin Loan

The SC.FACILITY.APPLN application captures the basic details of the credit facility request initiated by the private wealth customer. When the private wealth customer of the bank requests for a facility, this application can be used to record the portfolio details, requested amount and assets pledged as collateral. Subsequently, the bank’s credit officer can sanction the loan based on the assets pledged. It also contains a set of questions that need to be responded to by the bank’s customer who avails the loan, details of documents received. Also, the assets that the customer is willing to pledge towards the loan are specified in this application.

A customer can provide a percentage of his portfolio or full portfolio as collateral. A position or part of a position can also be attached as collateral. Thus, the Collateral Provided field in this application accepts the records from SC.POS.ASSET or SEC.ACC.MASTER or SECURITY.MASTER .

The Percentage field indicates the percentage of the portfolio or position pledged as collateral. A percentage can be given only if the asset pledged is a non-security asset.

The Pledged Quantity field indicates the quantity of shares pledged as collateral. This field is allowed only if the value in the Collateral Provided field is a SECURITY.MASTER ID.

Thus, a customer can pledge fixed quantities of instruments in his SECURITY.POSITION and percentage of holdings of other non-security positions or portfolio.

The validations of Collateral Provided field are as follows:

- If a part or full of the portfolio is being pledged, the Collateral Provided field accepts a record from SEC.ACC.MASTER . In this case, the collateral value is based on the Percentage Pledged field.
- When a portfolio or percentage of a portfolio is pledged, no other position or security can be pledged in the same SC.FACILITY.APPLN record.
- If a securities asset is pledged (for example: shares or bonds) the Collateral Provided field accepts a valid record from SECURITY.MASTER . Only a quantity can be specified if a security is pledged. A part or whole of a securities asset (in SC.POS.ASSET ) can also be pledged. When a security is pledged, then a SC.POS.ASSET of that security cannot be pledged in the same SC.FACILITY.APPLN record. Example: Consider 200 units of 100027-000 security are pledged. It falls under the record in SC.POS.ASSET with asset type 30 and sub-asset type 302. Then when the customer is pledging his assets for a different facility, Portfolio.30.302 record in SC.POS.ASSET cannot be pledged If a non-security asset is pledged (for example: cash or deposits) the Collateral Pledged field accepts a record from SC.POS.ASSET . The percentage of the collateral pledged is specified in the Percentage Pledged field..
- If a non-security asset is pledged (for example: cash or deposits) the Collateral Pledged field accepts a record from SC.POS.ASSET . The percentage of the collateral pledged is specified in the Percentage Pledged field.

In example 1 described below, the customer 100265 (portfolio 100265-1) has requested USD 500000. The customer has pledged 50% of his cash account as collateral in the SC.FACILITY.APPLN application as shown in the below screenshot.

If portfolio or non-security assets are pledged, then the system validates that the overall pledged percentage does not exceed 100% across various facilities.


###### Example 1

If 40% of a portfolio is pledged for one share margin facility, only 60% is allowed for another margin loan or lombard loan facility. Similarly, the system ensures that available nominal can only be pledged when a security is being pledged.


###### Example 2

Consider a customer holds 500 units of Amazon share. If the customer has pledged 300 units of Amazon share for share margin facility, then only 200 units are allowed for margin loan.


##### Sanctioning of Loan

Once the credit desk sanctions the loan, the Facility Sanctioned field must be set to Sanctioned. This acts as a trigger to create a record in COLLATERAL automatically. The ID of the record created in COLLATERAL is updated in the SC.FACILITY.APPLN application.

Immaterial of the number of securities or number of positions that are pledged, the system creates a single record in COLLATERAL . Each security or position pledged is updated as a line with P-xxx or N-xxx to indicate if it is a percentage or quantity that is pledged. The record in COLLATERAL holds the record of SC.FACILITY.APPLN .

The record in SC.COLLATERAL that is built from COLLATERAL also holds the breakup.


##### Creating Margin Loan

The back-office user must perform the following steps to create the margin loan manually:

1. Create a limit for the sanctioned amount.
2. Link the collateral created to the limit using the COLLATERAL.RIGHT application.
3. Create a margin loan using AA Loans with the limit attached.
4. Once the loan is created, update the loan ID in SC.FACILITY.APPLN for reporting purposes (this step in optional).


##### Utilising the loan

When an AA margin loan is created for the portfolio it creates an arrangement account that can then be used for purchasing stocks.

When an Order is input through SEC.OPEN.ORDER , the customer or user can decide if they prefer to use their regular cash account or fund the order from a margin loan. If they decide to utilise the margin loan, then the Facility Funded field must be set to Yes.

A context enquiry is available in SEC.OPEN.ORDER to show the different margin loans available and the balance available against each. The user can select the appropriate loan account. Loan accounts that are related to margin loans alone are displayed in the enquiry.

If the Facility Funded field is set to Yes and the account in SEC.OPEN.ORDER is not a margin loan account, then an override is raised.

Once the account is selected and trade is authorised, the system automatically generates an AA Activity to debit the AA loan account. The loan account shows a negative balance and gets evaluated as part of the portfolio valuation.


##### Evaluating Collateral Value

The CO module evaluates each collateral by applying margin rates, concentration caps, haircuts and so on. Read the Collateral User Guide for more information.

For the same portfolio a part of the security is pledged for a loan and the rest of the portfolio is pledged for another loan, only the unpledged positions must be evaluated while determining the collateral value of the portfolio.

To facilitate this, every time a security or position is pledged in SC.FACILITY.APPLN , the system automatically updates SC.POS.ASSET . The Available Nom field in SC.POS.ASSET ( against the security pledged) is updated with the available details for further pledging.

If a percentage of the position is pledged, the Available Nom field is updated with P-nn, where nn is the available balance percentage.

If a quantity is pledged, the Available Nom field is updated N-nn, where nn is the remaining quantity available for further pledging.

In this below example, the customer 100256 (portfolio 100256-1) has pledged some nominal of the share 700100-000 that the customer holds.

The system updates the Available Nom field with the balance quantity in the respective record in SC.POS.ASSET .

- If the customer has pledged the entire or a portion of the portfolio ( SEC.ACC.MASTER ), the system does not update the value in the Available Nom field in SC.POS.ASSET .
- If there is a quantity cap or if there are any blocked positions, the Available Nom field gets updated after considering the quantity cap and excluding any blocked nominal.
- To overcome rounding issues, the units are rounded down to the nearest trading units when Available Nom field is updated. This field is updated every time the SC.POS.ASSET is rebuilt.

The CO module evaluates the collateral as explained in the Collateral user guide.


##### Checking Buying Power

The concept of buying power summarises the liquidity of the portfolio. It offers a portfolio wide view of the available amount to invest. It is more comprehensive than the cash flow checks that are currently carried out as part of the order validation process.

The buying power calculation ensures that the additional risk of an order is covered by sufficient buying power. To achieve this, the execution of the order is simulated and the effect on the buying power are computed. The order is accepted and processed, only if the buying power is greater than the order amount. This approval process applies to all new orders and to the amendment of pending orders. The pending orders are orders that are already approved, but are for some reason not yet traded (for example, limit orders).

Before an order is processed, the buying power calculation engine determines whether there is sufficient buying power to meet the cost of execution. This is done by simulating the execution amount and comparing it with the calculated buying power. If the order amount is less than the buying power amount, then the system raises an override to that effect.

The overall principle of buying power validation is governed by risk aversion. Therefore, only the pending purchase orders are included in the buying power calculation and not the potential positive cash flows on account of sell orders. The following events trigger the buying power calculations:

- New orders – Purchase
- Amendment of pending orders – Purchase (only for nominal or price change)

On the other hand, the following events does not trigger the buying power validation:

- Sell order
- Cancellation of pending orders

When a record in SEC.OPEN.ORDER is created, the system performs a buying power check as follows:

- If the account is not an AA account, then the buying power is calculated as: Online Actual Bal (in ACCOUNT ) - Pending orders on the account
- If the account is an AL account (sub-application in ACCOUNT must be AL), the buying power check is based on the collateral pledged. If it is not a portfolio or a SC.POS.ASSET record belonging to this security (part or full) the buying power is based on the record in LIMIT specified in the ACCOUNT record. The buying power is calculated as: Avail Amt + Online Actual Bal – Pending orders for that account . If the customer has pledged SC.POS.ASSET of the security that is being purchased, the formula to calculate buying power is: Maximum Total - Online Actual Bal( in ACCOUNT ) - Pending orders.


#### 📋 Tasks

A private wealth customer can avail a credit facility based on their profile. The granted facility can be used for different types of liabilities (for example, drawdown a margin loan (one time or multiple drawdown) or derivative exposure, etc.) The liability must be within the limit amount and must be covered based on the pledged assets as collateral as defined in the credit facility.


##### Workflow

This section allows the user to perform the below tasks:

| SCREENS | WORKFLOW |
|---|---|
|  | Create New Facility . |
| Credit Facility Details | Enter values in the following fields: Client Portfolio Facility Product Collateral Type Collateral Code Collateral Provided.1 Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Amend Facility . |
| Amend an application(prior to submission for approval) | Enter or select values in the applicable fields and then click the FIND button. Click the Update icon. Enter values in the applicable fields requiring amendment. Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Approve Facility . |
| Authorise Facility application | Enter or select values in the applicable fields and then click the FIND button. |
| Authorise Facility application | Click the View icon corresponding to a record. The system displays the record in view mode. |
| Credit Facility application | View the facility application record details. |

| SCREENS | WORKFLOW |
|---|---|
|  | Sanctioned Facility . |
| Sanctioned PWM facilities | Enter or select values in the applicable fields and then click the FIND button. |
| Sanctioned PWM facilities | Select the Create Limit option from the drop-down and then click the Launch icon. |
| Input Limit for Loan | Enter values in the applicable fields . Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

There are no Outputs available for Margin Lending feature.


> **Related Applications:** `ACCOUNT`, `SC.FACILITY.APPLN`, `SC.FACILITY.PARAM`, `SC.POS.ASSET`, `SECURITY.POSITION`

---


### 3.4  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Lombard Lending (OV) module handles real time valuation of portfolios as well as margin lending and calculation of buying power.*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

The Lombard Lending (OV) module handles real time valuation of portfolios as well as margin lending and calculation of buying power.

Margin lending is a type of loan that allows the user to borrow money to invest, by using the existing shares, managed funds, cash or the user's entire portfolio holding as security. It is a type of gearing, which is borrowing money to invest. The amount that can be borrowed depends on the loan to value ratio (margin rates) of the portfolio assets.

The module supports the margin lending workflow starting from a customer applying for a margin loan and specifying the assets he chooses to pledge, sanctioning of the same by the bank, creating a collateral with the assets pledged by the customer, creating a loan linked to the collateral and tracking the utilisation of the same.

It also calculates the buying power available to the customer when an order is placed.

The buying power summarises the liquidity of the portfolio. It offers a portfolio wide view of the amount available to invest and in that sense, more comprehensive than the cash flow validations which is based on the cash available to invest.

A customer who purchases securities may either pay for the securities in full or borrow part of the amount from the bank. The portion of the consideration that the customer pays is the customer’s equity. The buying power and eligibility is calculated on the basis of facility granted to the customer. While borrowing (as above), it has the potential to increase the returns, the losses can also potentially increase.

Margin calls are when due to falls in the market value of the portfolio the collateral value is less than the loan amount borrowed. This results in what is generally known as the margin call.

Lombard Lending Direct is a functionality where the entire portfolio is deemed to be available as margin for trades. This is an older functionality which has since been replaced by the margin lending functionality.

The real-time valuation is the automatic intra-day valuation of a portfolio based on triggers. The triggers are nothing but events that have an impact on the valuation of a portfolio. That is, any transaction or a static change that affects the portfolio value is a trigger for the valuation process. Based on these triggers, valuation is performed online for selected portfolios.


##### Product Configuration

The OV.PARAMETER which is the main configuration parameter for this module, has the settings for Real Time Valuation, Margin Lending and the old Lombard Lending functionalities. This is a company-level parameter for activating the online valuation based on triggers which hold the following details:

- Details of triggers excluded for valuation
- Rules governing buying power and margin trading.

The fields available in this parameter are listed below.

| Field | Description |
|---|---|
| Online Val | Indicates whether automatic online valuation needs to be activated |
| Exclude Events.1 | Events excluded during the online valuation process |
| Use Facility Application | Field to set if Margin Lending functionality is required or the old Lombard functionality is to be used |
| Priority Api | API to determine priority for online valuation |


##### Illustrating Model Parameters

OV.PARAMETER is configured in the model bank. The model bank configuration is to use the new margin lending functionality. The model bank settings for fields is as below:

| Field | Description |
|---|---|
| Online Val | This is set to Yes in Model Bank |
| Priority API | A core API called OV.PRIORITY.API is released. This checks if the trigger is a batch job or online job and handles valuation accordingly. |
| Use Facility Application | This is set to Yes in Model bank to ensure that Margin Lending functionality is used by default. |


##### Illustrating Model Products

An AA lending product called Margin Loans is available and can be modified by clients or new products can be created as required.

---


### 3.5  RealTimeValuation


> **📇 Quick Reference Card**
> 
> **Purpose:** *The portfolio value is used by banks for various decisions such are sanctioning of margin loans, applying preferential fees, classifying customers as HNIs, etc. The portfolio value should therefore always be real or near real.*
> 
> **Applications:** `OV.PARAMETER`, `SC.PARAMETER`, `SEC.ACC.MASTER`, `SECURITY.POSITION`
> 
> **Key Fields:** *Exc Events*, *Online Val*, *Portfolio*, *Prc Tol*, *Prc Tol Type*, *Priority Api*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The portfolio value is used by banks for various decisions such are sanctioning of margin loans, applying preferential fees, classifying customers as HNIs, etc. The portfolio value should therefore always be real or near real.

There are several intra-day events like security price movements, security position and account balance movements that may have an impact on the portfolio valuation. In a volatile market situation, the valuation swings can be huge and unless there is a mechanism to update the valuation automatically, the valuation based on which the decisions are made by the bank could be drastically different from the valuation at the time the decision made.

The real time valuation engine ensures that portfolios are evaluated in a systematic manner to ensure that they always hold real or near real values.


#### ⚙️ Configuration

The following section describes about configuring some important parameters for this feature.


##### ConfiguringOV.PARAMETER

The key parameter to enable online valuation is the OV.PARAMETER . Here, if the field Online Val is set to Yes, then the events that have an impact on the valuation are captured and the valuation process is initiated automatically for the portfolio(s).

The events that impact valuation or triggers, are nothing but events that have an impact on the valuation of a portfolio. That is, any transaction or a static change that affects the portfolio value is a trigger for the valuation process.

The real-time valuation process is initiated by identifying the triggers or events that have an impact on the valuation of a portfolio. Some examples of triggers or business events are securities transaction, cash deposit or withdrawals, security price changes and so on.

The timing of the trigger is influenced by certain other parameter settings, mainly Include Nau Txns field in SC.PARAMETER application.For example, if this is set to YES, then the trigger happens as and when the transaction is input. However, if this is set to NO, then the trigger happens only when the transactions are authorised. Except any material amendment to transactions (nominal change, etc.) and reversals or deletions also acts as triggers for the valuation process.

The Exc Events field in the OV.PARAMETER record contains the details of the events that must be excluded from the list of triggers. If the bank does not require a real-time valuation to be triggered for certain events, then these events can be input in this field. This ensures that the valuation is not triggered when these events are encountered.

Additionally, tolerance can be set for price movements. This is to ensure that the valuation is not triggered for minor price changes. Only if the price change is in excess of the tolerance set, the valuation is triggered. The tolerance can be set either in terms of Amount ( Prc Tol Type with input as AMOUNT) or Percentage ( Prc Tol Type with input as PERCENTAGE). If the tolerance is set in terms of Amount, then the valuation is triggered only if the price change is in excess of the amount in Prc Tol field. If the tolerance is expressed as a Percentage, then the Prc Tol field, holds the percentage and any price change in excess of the percentage specified, triggers the valuation.

It is possible to prioritise some of these triggers (for example, transactions over bulk updates like price). For example, when a price upload happens for a security, all the underlying portfolios holding a position in the security are revalued. If all the triggers are processed sequentially, any transaction input are reflected in valuation only after the valuation is complete for the bulk updates.

The Priority Api field in OV.PARAMETER is used to specify an API, wherein the logic for separating the bulk updates from the transactional updates can be built-in. The triggers, resulting from transactions, can be separated from bulk updates and valued separately using the below mechanism.


##### ConfiguringSEC.ACC.MASTER

It is very important to identify the portfolios that require real-time. The banks require this facility only for portfolios that are actively traded and where these intra-day movements has a considerable impact on the decision making process. For example, if a bank has 100,000 portfolios of which only 10,000 are actively traded, it is a huge drag on system performance to perform intra-day valuation for all the portfolios for an event like price change in a single security.

The portfolios that require real-time valuation are identified either through the OV.PARAMETER record in the portfolio or the Online Val field in SEC.ACC.MASTER . If the Portfolio field in OV.PARAMETER is set to ALL, then the online valuation is activated for all the portfolios. If not, then the online valuation for specific portfolios is activated by setting the Online Val field in the SEC.ACC.MASTER record to YES.

> **⚠️ Note:** The Online Val in SEC.ACC.MASTER is set to YES, only if the Online Val is set to YES in the OV.PARAMETER .

However, it is possible to move the portfolios in and out of this category at any stage. If a dormant portfolio becomes active suddenly and there is a need to automatically track valuation for this portfolio intra-day, then this feature can be activated for that portfolio. Similarly, this can also be switched-off at any time for a portfolio that moves from being active to dormant.


#### 🔧 Working With

The following section describes the valuation process in detail.


##### Valuation Components

The valuation process is divided into three major segments based on the application and nature of transaction that is being processed.

The value of a Portfolio ( SEC.ACC.MASTER ) in Transact is updated by different modules :

- Through an Account linked to the portfolio
- Through Securities module
- Through Non-Securities transactions linked to the portfolio


###### Updating a Portfolio from an Account

A customer portfolio can be linked to accounts in the system. It is necessary when opening a SEC.ACC.MASTER record to define the accounts that belong to the portfolio. When calculating the value of a portfolio, the balance of those accounts are included in the valuation.


###### Updating a Portfolio from the Securities Module

Any securities transaction must include one or more portfolios. The securities transactions can be Trade, Transfer or Corporate Action. If a securities movement is involved, the SECURITY.POSITION is updated with the details of the movement and the positions are included while calculating the value of a portfolio.


###### Updating a Portfolio from Other Modules

Other non-SC applications can update a portfolio, subject to being linked to the portfolio. In case the other assets and liabilities are linked to a portfolio, the portfolio valuation process includes these while revaluing the portfolio.


##### Automatic Intra-Day Valuation

Once OV.PARAMETER is configured, the near real-time valuation process is initiated by different triggers. The triggers are nothing but events that have an impact on the valuation of a portfolio. In other words, any transaction or a static change that affects the portfolio value is a trigger for the valuation process. The valuation process must be capable of tracking such events and revalue the portfolio(s) in run time.


###### Triggers for Valuation

The overview of the possible events triggers and their effects is shown below:

| Trigger/ Effect | Security price | Security Transaction | Cash Transaction | Other Transactions | DX Price | Haircut |
|---|---|---|---|---|---|---|
| Cash Account |  | X | X | X |  |  |
| Security Value/Margin Value | X | X |  |  |  | X |
| Contract Value |  |  |  | X |  |  |
| Pending security Orders | X |  |  |  |  |  |
| DX Value |  |  |  |  | X |  |

As shown above, some of these triggers have an effect only on one element (for example, haircut change affects only the margin value of that particular security or asset type) whereas others have an impact on multiple elements (a securities purchase impacts both the securities value and cash account balance). Some of these triggers are transaction based (securities transaction, funds transfer, etc.) and some are static in nature (haircut change, price change, etc.). There are also events that affect only a single portfolio (securities transaction, funds transfer, etc.) whereas there are others that could affect multiple portfolios (a price change of a security that is held by many portfolios).

The automatic valuation engine is capable of handling the various types of events as detailed below: Triggers based on static change – Haircut Transaction triggers – Securities purchase, Transfer, Deposit, Funds Transfer, etc Global triggers – Price change, Currency rate change, etc Triggers that impact more than one element – Securities purchase (for example)

The following table lists out the events, their origin points and their effects:

|  | Event | Single/Multiple Portfolios | Element(s) | Origin |
|---|---|---|---|---|
| 1 | Securities Purchase/Sale | Single | Cash/Securities value/margin value | SEC TRADE |
| 2 | Securities Transfer | Single | Cash/Securities value/margin value | SECURITY TRANSFER |
| 3 | Position Transfer – across portfolios | Multiple | Securities Value/margin value | POSITION.TRANSFER |
| 4 | CA – Cash event | Single | Cash | ENTITLEMENT |
| 5 | CA – Stock event | Single | Securities Value/margin value | ENTITLEMENT |
| 6 | CA – Combination of stock and cash | Single | Cash/Securities value/margin value | ENTITLEMENT |
| 7 | Securities Price change | Multiple | Securities value/margin value | SECURITY MASTER |
| 8 | Cash transaction | Single/Multiple | Cash Valuation | FUNDS TRANSFER/TELLER |
| 9 | Deposits (new, rollover) | Single | Cash/contract value | MONEY MARKET, LOANS.AND.DEPOSITS, ARRANGEMENT.ARCHITECTURE. |
| 10 | Loans (new, repayment) | Single | Cash/contract Value | LOANS.AND.DEPOSITS, ARRANGEMENT.ARCHITECTURE. |
| 11 | FX contract | Single | Cash/FX value | FOREIGN.EXCHANGE |
| 12 | Customer Margin/facility | Single | Margin value | SC CUSTOMER MARGIN |

> **⚠️ Note:** This is only an indicative list and not an exhaustive one. All transactions that impact the portfolio value (excluding exchange rate movements and margin rate changes at instrument or asset type level), triggers the online valuation to ensure the portfolio’s value is near real-time.


###### Component Level Valuation

The valuation process is divided into three major segments: Cash Accounts Security Positions Other Module Assets or Liabilities linked to the Portfolio

Any valuation carried out as part of COB or triggered online through enquiries, results in revaluing the entire portfolio even though only few of the elements (that make up the portfolio) has changed since the time valuation was last run. From a performance point of view, it is imperative that the valuation is run only for a particular element (an account or a security or a deposit) that has undergone a change instead of for all assets and liabilities are linked to a portfolio.

However, it must be mentioned that there are a few instances where more than one element is impacted resulting in a requirement to revalue more than one element. For example, a securities purchase does not only impact the securities position but also reduces the account balance. Two segments (accounts and securities position) needs to be revalued as a result of this transaction.

On the other hand, events like securities price change impacts only one element (a particular security position) and hence, only that element requires the revaluation.

A diagrammatic representation of the real-time valuation process is given below.

The real-time valuation engine identifies the element or elements that has/have undergone a change, as a result of a particular transaction and revalue only that particular component.

A work file is updated in case a triggering event is encountered for a portfolio that is set for real-time valuation.

The work file key for the various segments are as follows:

1. Cash account movements Key format - *
2. Securities Transactions Change in the portfolio holdings Key format - SC* . .
3. Other Module Transactions *

Once the work file is updated, the user can run the ONLINE.VAL.FINAL service to revalue the portfolio affected by the transaction. The valuation engine picks the key and performs the revaluation of the component impacted based on the key. The valuation details are updated in SEC.ACC.MASTER and SC.POS.ASSET records.


#### 📋 Tasks

There are no Tasks available for Real Time Valuation feature.


#### 📊 Outputs

There are no Outputs available for Real Time Valuation feature.


> **Related Applications:** `OV.PARAMETER`, `SC.PARAMETER`, `SEC.ACC.MASTER`, `SECURITY.POSITION`

---


---


## Appendix A: Glossary of T24 Applications & Fields


This glossary lists all T24/Transact application names and field names referenced throughout this document, with descriptions where available.


### Applications


| Application | Description |
|------------|-------------|
| `#PGM.AUTOM.ID` | T24 application: #PGM.AUTOM.ID |
| `AC.SYS.CODES` | T24 application: AC.SYS.CODES |
| `ACCOUNT` | T24 application: ACCOUNT |
| `ACCOUNT.CLASS` | T24 application: ACCOUNT.CLASS |
| `ACCOUNT.CREDIT.INT` | T24 application: ACCOUNT.CREDIT.INT |
| `ACCOUNT.DEBIT.INT` | T24 application: ACCOUNT.DEBIT.INT |
| `ACCOUNT.PARAMETER` | T24 application: ACCOUNT.PARAMETER |
| `ACCT.CAPITALISATION` | T24 application: ACCT.CAPITALISATION |
| `ACCT.GEN.CONDITION` | T24 application: ACCT.GEN.CONDITION |
| `ACCT.GROUP.CONDITION` | T24 application: ACCT.GROUP.CONDITION |
| `ARCHIVE` | T24 application: ARCHIVE |
| `ARRANGEMENT ARCHITECTURE` | T24 application: ARRANGEMENT ARCHITECTURE |
| `ASSET.BY.CATEG` | T24 application: ASSET.BY.CATEG |
| `ASSET.CODE` | T24 application: ASSET.CODE |
| `ASSET.TYPE` | T24 application: ASSET.TYPE |
| `ASST.BY.CATEG` | T24 application: ASST.BY.CATEG |
| `AUTO.ID.START` | T24 application: AUTO.ID.START |
| `CASH.FLOW.EXCEPTION` | T24 application: CASH.FLOW.EXCEPTION |
| `CATEGORY` | T24 application: CATEGORY |
| `CO.ALLOCATION.DETAILS` | T24 application: CO.ALLOCATION.DETAILS |
| `CO.ASSET.DETAILS` | T24 application: CO.ASSET.DETAILS |
| `CO.CONC.CAP.EXCESS` | T24 application: CO.CONC.CAP.EXCESS |
| `CO.COUNTRY` | T24 application: CO.COUNTRY |
| `CO.COUNTRY.GROUP` | T24 application: CO.COUNTRY.GROUP |
| `CO.CURRENCY` | T24 application: CO.CURRENCY |
| `CO.DEFICIT` | T24 application: CO.DEFICIT |
| `CO.ELIGIBILITY` | T24 application: CO.ELIGIBILITY |
| `CO.INDUSTRY` | T24 application: CO.INDUSTRY |
| `CO.MGN.ALERT` | T24 application: CO.MGN.ALERT |
| `CO.RANKING` | T24 application: CO.RANKING |
| `CO.VALUATION.PARAMETER` | T24 application: CO.VALUATION.PARAMETER |
| `CODE` | T24 application: CODE |
| `COLLATERAL` | T24 application: COLLATERAL |
| `COLLATERAL.CODE` | T24 application: COLLATERAL.CODE |
| `COLLATERAL.EXCLUSION` | T24 application: COLLATERAL.EXCLUSION |
| `COLLATERAL.PARAMETER` | T24 application: COLLATERAL.PARAMETER |
| `COLLATERAL.RIGHT` | T24 application: COLLATERAL.RIGHT |
| `COLLATERAL.TYPE` | T24 application: COLLATERAL.TYPE |
| `COMPANY` | T24 application: COMPANY |
| `CONDITION.PRIORITY` | T24 application: CONDITION.PRIORITY |
| `COUNTRY` | T24 application: COUNTRY |
| `CURRENCY` | T24 application: CURRENCY |
| `CUSTOMER` | T24 application: CUSTOMER |
| `CUSTOMER.COLLATERAL.TYPE` | T24 application: CUSTOMER.COLLATERAL.TYPE |
| `Category` | T24 application: Category |
| `DATA CAPTURE` | T24 application: DATA CAPTURE |
| `DX.PARAMETER` | T24 application: DX.PARAMETER |
| `DX.PARAMETER(N)` | T24 application: DX.PARAMETER(N) |
| `EB.CONTRACT.BALANCES` | T24 application: EB.CONTRACT.BALANCES |
| `EB.OBJECT` | T24 application: EB.OBJECT |
| `EB.PRODUCT` | T24 application: EB.PRODUCT |
| `FUNDS` | T24 application: FUNDS |
| `FUNDS TRANSFER` | T24 application: FUNDS TRANSFER |
| `GENERAL.CHARGE` | T24 application: GENERAL.CHARGE |
| `GROUP.CAPITALISATION` | T24 application: GROUP.CAPITALISATION |
| `GROUP.CREDIT.INT` | T24 application: GROUP.CREDIT.INT |
| `GROUP.DEBIT.INT` | T24 application: GROUP.DEBIT.INT |
| `INVESTMENT` | T24 application: INVESTMENT |
| `INVESTMENT.PROGRAM` | T24 application: INVESTMENT.PROGRAM |
| `LI.EXTERNAL.CONTRACT` | T24 application: LI.EXTERNAL.CONTRACT |
| `LI.EXTERNAL.TRANSACTION` | T24 application: LI.EXTERNAL.TRANSACTION |
| `LI.EXTERNAL.TRANSACTIONS` | T24 application: LI.EXTERNAL.TRANSACTIONS |
| `LIMIT` | T24 application: LIMIT |
| `LIMIT.COL.ALLOC.WORK` | T24 application: LIMIT.COL.ALLOC.WORK |
| `LIMIT.DAILY.OS` | T24 application: LIMIT.DAILY.OS |
| `LIMIT.PARAMETER` | T24 application: LIMIT.PARAMETER |
| `LIMIT.REFERENCE` | T24 application: LIMIT.REFERENCE |
| `LIMIT.TXNS` | T24 application: LIMIT.TXNS |
| `LOANS AND DEPOSITS` | T24 application: LOANS AND DEPOSITS |
| `MANAGED` | T24 application: MANAGED |
| `MANAGED.ACCOUNT` | T24 application: MANAGED.ACCOUNT |
| `MANAGED.ACCOUNTS` | T24 application: MANAGED.ACCOUNTS |
| `MARGIN.CONTROL` | T24 application: MARGIN.CONTROL |
| `MS.PARAMETER` | T24 application: MS.PARAMETER |
| `OV` | T24 application: OV |
| `OV.PARAMETER` | T24 application: OV.PARAMETER |
| `PROGRAM` | T24 application: PROGRAM |
| `SAVINGS.PREMIUM` | T24 application: SAVINGS.PREMIUM |
| `SC.CUSTOMER.MARGIN` | T24 application: SC.CUSTOMER.MARGIN |
| `SC.FACILITY.APPLN` | T24 application: SC.FACILITY.APPLN |
| `SC.FACILITY.PARAM` | T24 application: SC.FACILITY.PARAM |
| `SC.GROUP.POS.ASSET` | T24 application: SC.GROUP.POS.ASSET |
| `SC.INDUSTRY` | T24 application: SC.INDUSTRY |
| `SC.ISSUER` | T24 application: SC.ISSUER |
| `SC.ORDER.SESSION` | T24 application: SC.ORDER.SESSION |
| `SC.PARAMETER` | T24 application: SC.PARAMETER |
| `SC.POS.ASSET` | T24 application: SC.POS.ASSET |
| `SC.SECURITY.MARGIN` | T24 application: SC.SECURITY.MARGIN |
| `SC.VALUATION.GROUP` | T24 application: SC.VALUATION.GROUP |
| `SEC OPEN ORDER` | T24 application: SEC OPEN ORDER |
| `SEC.ACC.MASTER` | T24 application: SEC.ACC.MASTER |
| `SEC.OPEN.ORDER` | T24 application: SEC.OPEN.ORDER |
| `SEC.TRADE` | T24 application: SEC.TRADE |
| `SECURITY.MASTER` | T24 application: SECURITY.MASTER |
| `SECURITY.POSITION` | T24 application: SECURITY.POSITION |
| `SUB.ASSET.TYPE` | T24 application: SUB.ASSET.TYPE |
| `Sector` | T24 application: Sector |
| `TELLER` | T24 application: TELLER |
| `TRANSFER` | T24 application: TRANSFER |
| `TYPE` | T24 application: TYPE |
| `theCO.VALUATION.PARAMETER` | T24 application: theCO.VALUATION.PARAMETER |
| `theSC.PARAMETER` | T24 application: theSC.PARAMETER |


### Fields Referenced


| Field | Field | Field |
|-------|-------|-------|
| `; Use Pay Rec Sys` | `ADDITIONAL.DETAILS.LABLE` | `ADDITIONAL.DETAILS.VALUE` |
| `ALLOW.EXTERNAL.ONLY` | `Acc` | `Account` |
| `Account Officer` | `Account As Liab` | `Account Level Haircut` |
| `Account No` | `Acct` | `Acct Checkdig Type` |
| `Actual Value` | `Addl Criteria Field` | `Adj` |
| `Adj Margin` | `Adj Margin Rate` | `Adj Short Pos` |
| `Advance Message` | `Advised Amount` | `Allocated Amt` |
| `Allocation` | `Allocation Option` | `Allocation Work Id` |
| `Allow External Only` | `Allow Intraday Limit` | `Allow Mult Group` |
| `Allow external` | `Allowed Customer` | `Allowed Product` |
| `Amount` | `Applicatio` | `Application` |
| `Application Id` | `Application Input` | `Application.ID` |
| `Applied Date` | `Apply Credit Policy` | `Approved Issuer` |
| `Ar Drop Alert` | `Arc Filename` | `Archive Data` |
| `Asset Cap` | `Asset Ccy` | `Asset Id` |
| `Asset Type` | `Authorised` | `Auto Restore Alloc` |
| `Avail Amt` | `Available Amount` | `Available Nom` |
| `Avg Daily Trd Vol` | `B` | `BOOKING.DATE` |
| `Balance` | `Basis` | `Bef` |
| `Bkno` | `Bond Cap` | `Bond Ranking` |
| `Booked Balance` | `Booking Date` | `Buffer` |
| `Buffer Deficit` | `Buy` | `Buying` |
| `Buying Power` | `Buying Power = Cash` | `Buying Power.1.1` |
| `Buying Power.1.2` | `Buying.Power.1.1 and Buying.Power.1.2` | `C` |
| `CATEGORY` | `COMMITMENT.CONTRACT` | `CONTRACT.APPLICATION` |
| `CONTRACT.COMPANY` | `CONTRACT.ID` | `CR.DR.MARKER` |
| `CURRENCY` | `CUSTOMER.IDS` | `Cap` |
| `Cap Type` | `Cap Value` | `Cap Value Ccy` |
| `Cash Collateral` | `Cash Flow Days` | `Category` |
| `Ccy` | `Ccy Pair Perc` | `Central Bank Value` |
| `Charge Debit Account` | `Check` | `Check Limit` |
| `Check Val Lim Breach` | `Check Validation Limit Breach` | `Checkdig` |
| `Cheque Register` | `Child Portfolio` | `Child Portfolio.1` |
| `Child Valuation` | `Client` | `Co` |
| `Co Allocation` | `Co Mv Check` | `Coll` |
| `Coll Booking Frequency` | `Collateral Account ID` | `Collateral Account Ranking` |
| `Collateral Ccy` | `Collateral Code` | `Collateral Details` |
| `Collateral Id` | `Collateral Id.1` | `Collateral Item` |
| `Collateral Pledged` | `Collateral Pool Reference` | `Collateral Priority` |
| `Collateral Provided` | `Collateral Provided.1` | `Collateral Provider` |
| `Collateral Right` | `Collateral Right Id` | `Collateral Right Ids` |
| `Collateral Status` | `Collateral Type` | `Collateral.Code` |
| `Collateral.Type` | `Commit` | `Commitment Contract` |
| `Conc` | `Conc Cap Defn` | `Conc Cap Level` |
| `Concentration Cap` | `Consol key` | `Count` |
| `Counterparty` | `Country` | `Credit Check` |
| `Criteria` | `Criteria Appln` | `Criteria Field` |
| `Criteria Name` | `Criteria Type` | `Cross Ccy Haircut` |
| `Cross Limit` | `Currency` | `Currency Market` |
| `Customer` | `Customer Id` | `Customer Ccy` |
| `Customer Id` | `Customer No` | `Customer Number` |
| `Customer.1` | `DELETE.REASON` | `DRAWING.CONTRACT` |
| `Day` | `Dda Limit Excess Check` | `Def Joint` |
| `Def Override` | `Def Risk Group Mand` | `Default Advised` |
| `Default Check` | `Default Max Total` | `Deficit Ccy` |
| `Deficit Date` | `Define Priority` | `Delay Txn Update` |
| `Description` | `Description.1` | `Disc` |
| `Diversification` | `Diversification Type` | `Drawing Contract` |
| `EXTERNAL.CONTRACT.ID` | `Effective Date` | `Emerging Market` |
| `Emerging Market Group` | `Emit Business Event` | `End Date` |
| `End Time` | `Entry` | `Entry Category; Sus Category; Suspense Txn In; Suspense Txn Out; Suspense History` |
| `Estimation value of other Liabilities.` | `Exc Events` | `Except Sub Asset` |
| `Excl Collateral` | `Excl Collateral Type` | `Exclude All` |
| `Exclude Con Cap Pool` | `Exclude Conc Cap Pool` | `Exclusion ID` |
| `Exclusion Id` | `Execution` | `Execution Value` |
| `Execution.Value` | `Expiry Date` | `Expiry.Date` |
| `Exposure Calc` | `Exposure ID` | `Ext Currency` |
| `Ext Execution Value` | `Ext Margin Rate` | `Ext Nominal Value` |
| `External Collateral Currency` | `External Collateral Value` | `External Collateral value` |
| `External Table` | `Facility` | `Facility Funded` |
| `Facility Product` | `Fix/Variable` | `For a discretionary portfolio` |
| `For non-discretionary portfolio` | `Fx Other Amount` | `Fx Other Currency` |
| `Fx Or Time Band` | `GB Account Description` | `GB Description` |
| `GRP.CREDIT.LIMIT` | `Gearing` | `General Ledger Value` |
| `Global Limit` | `Group Purpose` | `Grouping Portfolios for Valuation` |
| `Grp Estimation` | `Grp Init Mgn Value` | `Grp Liability` |
| `Grp Sec Margin Ratio` | `Grp Sec Mkt Value` | `Grp.Margin.Value` |
| `Haircut` | `Held` | `Highest` |
| `Holding Action` | `Holding Percent` | `Incl Clv Cap` |
| `Include Con Cap Pool` | `Include Conc Cap Pool` | `Include Concentration Cap` |
| `Index` | `Industry` | `Init Mgn Value` |
| `Initial Margin` | `Instrument ID` | `Instrument Id` |
| `Interest` | `Interface To` | `Internal` |
| `Internal Amount` | `Issuer` | `Issuer Diverfn` |
| `Issuer Diverfn Rtn` | `Issuer Diversification` | `Issuer Except` |
| `Issuer Percentage` | `Joint` | `Joint Liability` |
| `Joints` | `Key Type` | `L` |
| `LIMIT.ID` | `LIMIT.PRODUCT` | `LIMIT.TYPE` |
| `LTCV` | `LTMV` | `LTV denominator` |
| `Last Valuation Run` | `Liab Ccy` | `Liability Amount` |
| `Liability Categ` | `Liability Ccy` | `Liability Customer` |
| `Liability Id` | `Liability No.` | `Liability Number` |
| `Limit` | `Limit Id` | `Limit Product` |
| `Limit Band Level` | `Limit Id` | `Limit Mnemonic` |
| `Limit Percentage` | `Limit Product` | `Limit Product with the Fx` |
| `Limit Reference` | `Limit Reference.1` | `Limit Serial` |
| `Limit Subroutine` | `Limit Type` | `Link Type` |
| `Link Type.1` | `Loan` | `Local` |
| `Loss Margin Rate` | `Lowest` | `Ltv Denominator` |
| `Ltv Highest Fields` | `Ltv Local Denominator` | `Ltv Lowest Fields` |
| `Ltv Numerator` | `Ltv Rules` | `M` |
| `MATURITY.DATE` | `Maintain Time Code Bal` | `Margin` |
| `Margin Allowed` | `Margin Calc Rtn` | `Margin Control` |
| `Margin Control, Sub Asset Type, Asset Type` | `Margin Lending` | `Margin Rate` |
| `Margin Value` | `Margin Values` | `Mask` |
| `Master Portfolio` | `Maturity Days` | `Maturity Period` |
| `Maturity Period Perc` | `Max Length` | `Max No Of Splits` |
| `Max Sub Alloc` | `Maximum Total` | `Maximum Unsecured` |
| `Minimal Price` | `Msg` | `Multi` |
| `Mv` | `Mv Bef Conc Cap` | `Net Od Appl` |
| `Net Od Appl; Net Od Override; Net Locked Override` | `Net Od Override` | `Netting Reqd` |
| `New Level` | `New Value` | `No Con Cap` |
| `No Conc Cap` | `No Of Issuer` | `No Port Valuation` |
| `Nominal` | `Nominal Value` | `Nominal.Value` |
| `Nomination Currency` | `Nostro Default` | `Notes` |
| `Old Level` | `Old Value` | `Online Actual Bal` |
| `Online Limit` | `Online Update` | `Online Val` |
| `Operation` | `Ov Issuer` | `P` |
| `Pay Rec Allwd` | `Pay Recv Options` | `Pending orders for that account` |
| `Pending orders on the account` | `Perc` | `Perc calc Basis` |
| `Percent Date Fqu` | `Percentage` | `Percentage Allocation` |
| `Percentage Cap` | `Percentage Cover` | `Percentage Floor` |
| `Percentage Pledged` | `Pf` | `Pf Qual Ccy` |
| `Pf Qual Value` | `Pf.Qual.Ccy` | `Pf.Qual.Value` |
| `Pledge Amt` | `Pledge Amt.1` | `Pledge Pct` |
| `Pledged Quantity` | `Pool Level Haircut` | `Port Comp Id` |
| `Portfolio` | `Portfolio ID` | `Portfolio Id` |
| `Portfolio No` | `Portfolios` | `Power` |
| `Pp Adj Factor` | `Prc Tol` | `Prc Tol Type` |
| `Prd Adj Margin Rate` | `Prd Margin Rate` | `Prefix` |
| `Prefntl Margin Rate` | `Price` | `Price Cap` |
| `Price cap` | `Pricing Days` | `Priority Api` |
| `Pro Data Calculation` | `Product` | `Product Allowed` |
| `Product No` | `Purchase` | `Purchase Price` |
| `Qual` | `Quantity Cap` | `Quantity cap` |
| `REPORTING.CUSTOMER` | `Rate` | `Realtime Alloc` |
| `Reduce Limit Amt` | `Reducing Limit` | `Reference Child` |
| `Reference Currency` | `Rejection Reason` | `Relationship Officer` |
| `Repaid Amount` | `Report Sub Total` | `Reporting Type` |
| `Reserved` | `Restricted` | `Retain Ac Balances` |
| `Retention Period` | `Review Date Fqu` | `Review Date Frequency` |
| `Review Fqu` | `Review.Frequency` | `Risk Exclusion ID` |
| `Risk Group Id` | `Risk Group Mand` | `Run Valuation` |
| `SC Customer Margin` | `SC Issuer` | `SOURCE.SYSTEM` |
| `START.DATE` | `SUPPRESS.ACCOUNTING` | `SYSTEM.ID` |
| `Same Strik` | `Same Strike` | `Sc Customer Margin` |
| `Sc Facility App Id` | `Sec Margin Rate` | `Sec Margin Ratio` |
| `Second Mrkt Value` | `Second Mrkt Value, Init Mgn Value, Top Up Margin, Sell Out Margin, Mv Margin Amt, Eq Margin Amt` | `Security Code` |
| `Security No` | `Sell Out Deficit` | `Sell Out Mgn Rate` |
| `Short Pos Margin` | `Short Pos Mgn Amt` | `Start Date` |
| `Start Time` | `Start date` | `Status` |
| `Std Max Conc Cap` | `Stock` | `Stock Count Basis` |
| `Stock Held` | `Sub Asset Type` | `Sub Division Code` |
| `Sub Product Level` | `Sufficiency Ratio` | `Sus Category` |
| `Sys Code` | `Sys Code; Nostro Default; Def Override; Use First Acct; Default Order` | `THIRD.PARTY.EXPOSURE` |
| `TRANSACTION.AMOUNT` | `TRANSACTION.APPLICATION` | `TRANSACTION.CURRENCY` |
| `TRANSACTION.REFERENCE` | `Tdgl Details` | `Temp Limit` |
| `Third Party Value` | `Time Bal Eff Date` | `Time Code` |
| `Time Code Id` | `Timeband` | `Tolerance` |
| `Top Cross Ref` | `Top Up Deficit` | `Top Up Mgn Rate` |
| `Tot Deficit Lar` | `Total Alloc` | `Total Deficit` |
| `Total Ext Collateral Value` | `Total External Collateral Value` | `Total Unalloc` |
| `Traded Dated Gl Bal` | `Transaction Amount` | `Transaction Currency` |
| `Transaction Code` | `Transfer` | `Type` |
| `Unallocated Amt` | `Update Date` | `Update Online` |
| `Use Advance Ratio` | `Use Facility Application` | `Use First Acct` |
| `Use Pay Rec Cat` | `Use Pay Rec Sys` | `Use Pay Receive` |
| `Use Pay Receive Cat Sys` | `Use Pay Recv` | `V` |
| `Val Date By Cat Sys` | `Val Date By Sys` | `Val Date Sys Id` |
| `Val Date Sys Id;` | `Validate` | `Value` |
| `Value Date` | `Value Ccy` | `Value Dated Acctng` |
| `Value.Date` | `Vd Cat Start; Vd Cat End; Val Date By Cat; Use Pay Rec Cat` | `Vd Cat Sys End` |
| `Vd Cat Sys Id` | `Vd Cat Sys Id; Vd Cat Sys Start; Vd Cat Sys End; Val Date By Cat Sys;` | `Vd Cat Sys Start` |
| `Volume Cap` | `Xx-Xx-Tier Margin Rate` | `Xx-Xx` |
| `Concentration Cap` | `Tier Adj Margin Rate` | `alances +` |
| `alue` | `argin` | `ending orders –` |
| `ending value of Securities + Margin value of other assets –` | `field` | `heck` |
| `margin value` | `refntl` | `value` |


---


## Appendix B: Consolidated Field Reference


This appendix consolidates all field description tables from across the documentation, grouped by sub-module. This provides a single reference for all field definitions.


### Limits_Collateral - CO (CO)


**Collateral Advance Ratio**

| Field Name | Description |
|---|---|
| Use Advance Ratio | When this field is set to Yes, the collateral execution value is calculated based on the Margin Rate defined for the linked asset at various levels |
| Account As Liab | Accounts linked to limits with negative balance are considered as liabilities when calculating the collateral deficit value, if this field is set to Yes |
| Update Online | If this field is set to Yes, then the advance ratio setup is considered while calculating collateral value online |

**Collateral Advance Ratio**

| Field Name | Description |
|---|---|
| Conc Cap Level | This is a multi-valued field. This field contains different concentration cap levels used by the system in the order they are processed. This is an optional input. If this field is left blank, then concentration cap processing will not be carried out. Duplicates are not allowed. |
| Std Max Conc Cap | This is an optional field. Any input must be a number from 0 to 100. Any other input is not allowed. It contains the standard maximum concentration cap. |
| Bond Ranking | This is an optional multi-valued field associated with the Bond Cap field. Duplicates (that is, the same value in more than one multi-value) are not allowed. |
| Bond Cap | This is an optional multi-valued field associated with the Bond Ranking field. Any input must be a number from 0 to 100. Any other input is not allowed. |
| Co Allocation | Defines whether the allocation of assets is configured for limits or liabilities. The allowed values are Limits or Contracts. |

**Collateral Advance Ratio**

| Field | Description |
|---|---|
| Customer Id | The ID of the customer |
| Collateral Ccy | Currency of collateral |
| Coll Type | Collateral type ID as in the collateral record |
| Coll Country | Country of the collateral |
| High Adv Ratio | High advance ratio defined for the collateral asset |
| Low Adv Ratio | Low advance ratio defined for the collateral asset |
| Margin Value | Margin value of the collateral |
| Contract Id | Contract linked to the collateral |
| Asset Type | Asset type of the contract linked to collateral |
| Sub Asset Type | Sub Asset type of the contract linked to collateral |
| Sc Industry | Industry code as in record of SECURITY.MASTER . |
| Concentration Cap | Single concentration cap set for the asset |
| No Conc Cap | This field is updated when the collateral type is set not to apply concentration cap |
| Tot Cust Coll | Total value of the collateral in local currency |
| Exch Rate | This field displays the exchange rate for the given asset. It is defined for each asset under the collateral. The exchange rate updated is calculated considering different factors defined in the corresponding record in the CURRENCY application, and it is not necessarily match with the value in the Mid Reval Rate field in the record in the CURRENCY application. The CO.RECALC.CUST.COLL service must be run once to update the exchange rate in the existing record in CO.ASSET.DETAILS . |

**Collateral Advance Ratio**

| Field | Description |
|---|---|
| Customer Id | Valid customer ID |
| Liability Id | Contract ID for which allocation is done |
| Liability Ccy | Currency of contract |
| Liability Amount | Contract amount |
| Liability Categ | Contract category |
| Reserved | Contract reserved |
| Collateral Id | Collateral ID from which amount is allocated to the above contract |
| Collateral Ccy | Collateral currency |
| Avail Amt | Contract amount available in collateral currency |
| Allocated Amt | Contract amount allocated to the above contract in collateral currency |
| Unallocated Amt | Contract amount unallocated |
| Reserved | Collateral reserved |
| Total Alloc | Total amount allocated to contract in contract currency |
| Total Unalloc | Total amount unallocated to contract in contract currency |

**Collateral Advance Ratio**

| Field | Description |
|---|---|
| Customer Id | ID of the customer |
| Deficit Ccy | Currency of deficit amount (local currency of customer company) |
| Total Deficit | Deficit amount (total deficit amount for the customer in LCCY) |
| Buffer Deficit | If the deficit amount is less than buffer specified in OV parameter, then this field is updated |
| Top Up Deficit | If the deficit amount is GE Top up % specified in OV parameter then, this field is updated |
| Sell Out Deficit | If the deficit amount is GE Sell out % specified in OV parameter, then this field is updated |
| Deficit Date | Date on which first CO.DEFICIT is updated |
| Update Date | Date on which the deficit is re-calculated |
| Advance Message | Messages due to advance ratio change |
| Tot Deficit Lar | Total deficit before applying Group concentration cap |

**Collateral Advance Ratio**

| Field | Description |
|---|---|
| Customer Id | The ID of the customer |
| Conc Cap Level | This is the level of the concentration cap that has been exceeded. This values are: Customer Currency Security Bond Ranking Asset By Categ Asset Type Sub Asset Type Industry |
| Conc Cap Defn | Value of the concentration cap that has been applied. For example, the country code of the country or the currency code of the currency |
| Collateral Id | ID of the collateral for which concentration cap is applied |
| Old Level | Percentage of collateral before the concentration cap is applied |
| Old Value | Value of the collateral before the concentration cap is applied |
| New Level | Percentage of collateral after the concentration cap is applied |
| New Value | Value of the collateral after the concentration cap is applied |
| Applied Date | Date the concentration cap was exceeded |

**Collateral Exclusion**

| Field Name | Description |
|---|---|
| Country | Country of the collateral to be excluded. Must be a valid record in COUNTRY application |
| Currency | Collateral's currency, which is to be excluded |
| Security Code | Collaterals that have the security master as asset. Must be a valid record in SECURITY.MASTER application |
| Issuer | Issuer of the security whose collaterals are to be excluded. This is an optional field |
| Industry | Specifies the industry to which the asset belongs. Must be a valid record in SC.INDUSTRY application |
| Counterparty | Counterparty of the asset. Must be a valid Customer record |

**Collateral Exclusion**

| Description | Application.ID in Collateral | Example |
|---|---|---|
| Entire portfolio as collateral | - | 190200-1 |
| Specific sub asset type and asset type in the portfolio as collateral | - . . | 190200-1.300.30 |
| Specific security instrument in the portfolio as collateral | - . . * | 190200-1.300.30*800000-006 |

**Group Concentration Cap**

| Field | Description |
|---|---|
| Margin Rate | Allows the modification of the advance ratio based on the currency of the asset. It allows ‘+’ or ‘-‘ followed by a number between 0 and 100. This amends the advance ratio for assets valued in the currency by the number of percentage points, either increasing (+) or decreasing (-), depending on the sign of the number. This is an optional field. |
| Adj Margin Rate | Allows the modification of the advance ratio based on the currency of the asset. It allows ‘+’ or ‘-‘ followed by a number between 0 and 100. This amends the advance ratio for assets valued in the currency by the number of percentage points, either increasing (+) or decreasing (-), depending on the sign of the number. This is an optional field. |
| Product | This field is associated with Prd Margin Rate and Prd Adj Margin Rate fields. These fields allow exceptional advance ratio and lower advance ratio rates to be defined for specific products linked to the country. This is an optional multi-value field. |
| Prd Margin Rate | Allows modification of the advance ratio based on the currency of the asset for the associated product. It allows ‘+’ or ‘-‘ followed by a number between 0 and 100. This amends the advance ratio for assets in this product valued in the currency by the number of percentage points, either increasing (+) or decreasing (-), depending on the sign of the number. This is a multi-value field. |
| Prd Adj Margin Rate | Allows modification of the lower advance ratio based on the currency of the asset for the associated product. It allows ‘+’ or ‘-‘ followed by a number between 0 and 100. This amends the lower advance ratio for assets in this product valued in the currency by the number of percentage points, either increasing (+) or decreasing (-), depending on the sign of the number. This is an optional multi-value field. |
| Concentration Cap | Defines the concentration cap for the currency. |

**Group Concentration Cap**

| Field | Description |
|---|---|
| Concentration Cap | Contains the concentration cap to be applied to assets associated with this risk country. Input must be a number from 0 to 100. This is an optional field. |
| Emerging Market | Indicates if the country is considered as an emerging market. If set to Yes, the country is defined as an emerging market. |

**Group Concentration Cap**

| Field | Description |
|---|---|
| Description | Contains the description for the country group. This is an optional field. |
| Concentration Cap | Indicates the concentration cap that is applied to assets linked to countries in the group. Input must be a number from 0 to 100. |
| Country | Multi-valued field defaulted from CO.COUNTRY and contains the list of countries linked to the country group. |

**Group Concentration Cap**

| Field | Description |
|---|---|
| Concentration Cap | Indicates the concentration cap to be considered for the sub asset type. |

**Margin Valuation through Credit Policy Structure**

| Fields | Description |
|---|---|
| Criteria | The user can define any meaningful name for the criteria that is to be used in the LTV evaluation. |
| Criteria Type | Holds the attributes that define the margin rates. The attributes are Amount, Category, Country, Currency, Fixed.Tenor, Remaining.Tenor, Price, Date and Any. |
| Operation | Defines the operand for the given criteria (for example, equal or greater than) |
| Value | Holds the value of the Criteria field. In this example, when the amount is defined in the Criteria field, users must define the value, that is, 50,000. |
| Value Ccy | When the Criteria Type is Amount or Price, the associated currency should be defined in Value Ccy . |
| Joints | AND/OR are joints used to define the link between multiple attributes based on which the margin rate is defined. |

**Margin Valuation through Credit Policy Structure**

| Criteria Type | Description | Supporting Operands |
|---|---|---|
| Amount | All the attributes indicated in terms of amount like balance and fund size are part of this criterion. | ALL [EQ, LT, LE, GT, GE, Range (Rg), NE] |
| Category | All the attributes pertaining to the category of the asset class, sub asset class, contract or security instrument. | ALL |
| Country | Any attribute related to the country of the asset class, sub asset class, contract and security instrument is part of this criterion. | EQ, NE |
| Currency | All the attributes related to the currency of the asset class, sub asset class, contract or security instrument are part of this criterion. | EQ, NE |
| Fixed.Tenor | Those attributes that indicate the time of the asset class, sub asset class or contract are part of this criterion. | ALL except Rg |
| Remaining.Tenor | Those attributes that indicate the remaining period left for the asset class, sub asset class or contract are part of this criterion. | ALL except Rg |
| Price | Those attributes related to the price of the security instrument (for example, price of a share) are part of this criterion. | ALL |
| Date | Those attributes related to the date of the asset class, sub asset class, contract or security instrument are part of this criterion. | ALL |
| Any | Those criteria that do not require any specific validation fit into the ‘Generic’ criteria type. For example, attributes like Index (S&P Global 100) or the Security Market (New York Stock Exchange) can use the ‘Generic’ criteria type. | All operands are applicable for numeric values. Only EQ and NE applicable for non-numeric values. |

**Margin Valuation through Credit Policy Structure**

| Fields | Description |
|---|---|
| Criteria Name | Validates those criteria defined above (amount, category and currency in the above example) in the suitable application. |
| Criteria Appln | The system refers the ACCOUNT application to validate the criteria defined for the above example. |
| Criteria Field | Field name from where the data is taken for the associated criteria application, for example, when the criteria is defined as ‘Category’, the Category field in the ACCOUNT application is referred to fetch the data. |
| Addl Criteria Field | In certain cases, additional criteria values for processing are required. This is mandatory when the Criteria Type is set to FIXED.TENOR, AMOUNT or PRICE. Not allowed for other criteria types. If Criteria Type is set to Fixed.Tenor, the user has to configure the start and end date. The Start date field can be configured in the Criteria Field and the End date field can be configured in the Addl Criteria Field. Similarly, the User can configure the associated currency for the Criteria Type ‘Amount’ and ‘Price’, in this field. |

**Margin Valuation through Credit Policy Structure**

| Fields | Description |
|---|---|
| Ccy Pair Perc | Denotes the haircut that is applicable when a collateral asset and liability are in two different currencies. The value defined can be an absolute percentage value. For example, the cross-currency haircut can be defined as 10%. During the currency matching process, the adjusted margin rate is derived by deducting the respective cross-currency pair percentage from the applicable margin rate. |
| Asset Ccy | Denotes the currency of the asset and is associated with the Ccy Pair Perc field. |
| Liab Ccy | Denotes the currency of the liability and is associated with the Ccy Pair Perc field. |

**Misc**

| ID | Type | Description |
|---|---|---|
| 100 | CASH | All types of Cash, Accounts, Money Market (MM), Loans & Deposits (LD) and Deposit Contracts |
| 200 | HOUSE | All forms of property; from domestic to industrial properties |
| 300 | ART | Includes paintings, sculpture, jewellery and so on |
| 400 | SHARES | Value of a customer's shares |

**Misc**

| COLLATERAL . TYPE | Description | COLLATERAL . CODE | Description |
|---|---|---|---|
| 100 | Cash | 101 | MM Deposits |
| 102 | LD Deposits |  |  |
| 103 | Savings Accounts |  |  |
| 200 | Houses | 201 | Business Property |
| 202 | Domestic Property |  |  |

**Misc**

| S.No. | Parameters | Description |
|---|---|---|
| 1. | COLLATERAL.PARAMETER | This application allows the user to define the company-level system parameter. User can define if address is to be defaulted from CUSTOMER application. To cover the currency conversion risk factor, margin for the collateral currency is also defined when limit currency is different from collateral currency. To retain collateral records in live table, retention period value must be defined in the collateral parameter setup. Specification to determine which balance from EB.CONTRACT.BALANCES table to be considered for updating in collateral record. |
| 2. | COLLATERAL.TYPE | This application allows the user to define different types of collaterals like building stocks and guarantees and so on. Information in this table enables the client to arrive at collateral value, revaluation of collateral value and linking to other applications in Temenos Transact . Market value or face value of the collateral, value for general ledger purpose, third party value (value of collateral item outside Temenos Transact ) are specified in this table. |
| 3. | COLLATERAL.CODE | This application allows the user to determine how collateral values are re-allocated across central bank reporting lines. Enables the system to perform recalculation of percentage of collateral cover applicable. Enables the system to mention the default review frequency. Enables the system to mention the default review frequency. Enables to update Allocated Balance type, Utilized balance type and Unutilized balance type. |
| 4. | COLLATERAL.EXCLUSION | This application allows the user to define the criteria for the exclusion of collaterals. CURRENCY, COUNTRY, SECURITY.CODE, INDUSTRY, ISSUER and COUNTERPARTY values are used to define the criteria. |
| 5. | CO.CURRENCY | This application allows the user to define the rules to modify the lower advance ratio of the assets valued in a currency. Enables the user to define the currency level concentration cap. Enables the user to define the specific margin rates at product level. |
| 6. | CO.VALUATION.PARAMETER | This application allows the user to define the margin calculation, asset allocation, asset valuation for the collateral process. Enables the user to specify if the collateral is allocated against limits or liabilities. Enables the user to mention the discretionary portfolios. |
| 7. | CUSTOMER.COLLATERAL.TYPE | This application allows the user to define specific collateral execution value for specific customers. |
| 8. | CO.ELIGIBILITY | This application allows the user to define the eligibility rules for collateral against the limit products to which the collateral is linked. |
| 9. | CO.INDUSTRY | This application allows the user to define the concentration cap at industry levels for security assets. |
| 10. | CO.RANKING | This application allows the user to define the ranking rules for the collaterals against limit products. |
| 11. | CO.COUNTRY | This application allows the user to define the concentration cap rules for the collateral country. |
| 12. | CO.COUNTRY.GROUP | This application allows the user to define the concentration cap rules for a group of countries. |

**Support for Wealth Credits**

| Field Name | Description |
|---|---|
| Pledged Quantity | Indicates the quantity of shares pledged as collateral. This field is enabled only if the value in the Collateral Provided field is a security instrument |
| Collateral Provided | Links the portfolio to SMF with the below ID’s: For pledging non-security asset like cash accounts, the SC.POS.ASSET ID is used to link the asset For pledging security asset, the security Instrument ID in the portfolio is used for linking For pledging the entire portfolio, Portfolio ID ( SEC.ACC.MASTER ID ) is used for linking |
| Percentage | Indicates the percentage of portfolio pledged as collateral. This field is enabled only if the value in the Collateral Provided field is pledging portfolio and non-security instruments |
| Collateral Id | Generated by system automatically when portfolios are pledged through SMF |

**Support for Wealth Credits**

| Field Name | Description |
|---|---|
| Asset Id | Indicates the Instrument Id or Portfolio Id |
| Asset Cap | Indicates the number of nominal of security or percentage of portfolio pledged in SC.FACILITY.APPLN |
| Sc Facility App Id | Indicates the respective record ID in SC.FACILITY.APPLN |


### Limits_Collateral - LI (LI)


**Misc**

| Field Name | Usage |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| Cash Flow Days | Specifies the number of calendar days forward for which the cash flow balances are to be maintained for the purpose of accounting overrides and cash flow processing. The number of days entered here determines the window period that cash flow balances are to be maintained on each account record. Each forward dated entry generated for an account impacts the cash flow balances, if the date of the entry falls within this period. If the number of days entered is 10, then any forward dated entry raised online that has the value date less than 10 calendar days from current date will update the accounts cash flow balances. If this update causes either a limit to be exceeded or an unauthorised overdraft to occur, then an override message appears on the transaction input. All entries raised online that fall outside the window do not update the account balances immediately and no override messages appear. But when their value dates fall within the window, the start of day process (SOD.CASH.FLOW) updates the account cash flow balances. If an exception occurs at this stage, then the CASH.FLOW.EXCEPTION table is updated to indicate this. If the value is not entered in this field, then only the nostro accounts have cash flow maintained and a default of 10 calendar days is used for this. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Value Dated Acctng | A switch to set value dated accounting as On or Off or Trade Dated General Ledger (TDGL). If a value dated accounting system is required, then this field must be set to Y. In trade dated accounting system, the cash based transactions update the customer’s account and the bank’s position on the date in which the transaction is processed in the system, irrespective of the value date assigned to the transaction. In value dated accounting system, the cash based transactions update the customer’s account and the bank’s position on the value date assigned to the transaction. It is held as off balance sheet until the value date. In TDGL accounting system, the cash based transactions update the customer’s account and the bank’s position on the value date assigned to the transaction. It is held under payable or receivable until the value date. Cash based transactions follow the accounting treatment based on this setup. However, the accounting treatment can be switched from one system to another and the system permits any of the following switch. Switching of Accounting System Treatment of cash based transactions can be switched from one system to another, any combination of the setup is possible. Original Accounting Setup Target Accounting Setup Trade dated Value dated Trade dated Trade dated GL Value dated Trade dated Value dated Trade dated GL Trade dated GL Trade dated Trade dated GL Value dated The new accounting system switch applies to new transactions only. The existing cash based transactions with a future date follows the setup applied when the transaction were raised. The Tdgl Details field in the STMT.ENTRY application holds the details of the accounting method followed for the transaction. Exceptions to the above is SEC.TRADE – Actual Settlement: If contract input is in existing setup and authorised in the modified setup, then the system follows the modified setup. | Original Accounting Setup | Target Accounting Setup | Trade dated | Value dated | Trade dated | Trade dated GL | Value dated | Trade dated | Value dated | Trade dated GL | Trade dated GL | Trade dated | Trade dated GL | Value dated |
| Original Accounting Setup | Target Accounting Setup |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Trade dated | Value dated |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Trade dated | Trade dated GL |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Value dated | Trade dated |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Value dated | Trade dated GL |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Trade dated GL | Trade dated |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Trade dated GL | Value dated |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Use Pay Receive | This field is used to flag the suspense processing at system Level, in the case of value dated or TDGL accounting setup. Under these accounting setup, the value of the transaction is suspended in a temporary account till the split value date is reached. The allowed values are : Yes – Suspended to GL accounts pay or receive as special entries and reported as on-balance sheet item in the general ledger (GL) report. No – This is the default setup where the suspense processing posts the entry to the internal suspense account. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Pay Rec Allwd | This field works in conjunction with Use Pay Receive . It is used when a customer wants to decide if payable or receivable are to be reported with account attributes or against underlying customer attributes based PR.CUSTOMER.BALANCE application. Value in this field should be valid record ID of AC.DEFINE.PAY.RECV.ALLOWED application. This field is available at different levels such as System level, System Id (sub-system) level, Category level and System ID with Category level. In the AC.DEFINE.PAY.RECV.ALLOWED application, the users can create their own records using any of the following options in the Pay Recv Options field. The ID of the application record can be a meaningful alpha-numeric name. Broker – This option decides the customer to whom the payable or receivable is to be booked in the PR.CUSTOMER.BALANCE . If this option is set, the payable or receivable is booked against the third party customer (for example, broker) passed from the application. If this option is not set, the payable or receivable is booked against the customer passed in the original entry from the underlying application. Contract – If this option is selected, all the payables or receivables are reported under the PR.CUSTOMER.BALANCE . Customer – If the target account passed from the underlying application is a customer account and the Customer option is set, then the payables or receivables are reported under PR.CUSTOMER.BALANCE . Internal – This option works similar to Use Pay Recv set to Yes. If the entry is posted as an internal (suspense) account and the target account is passed from the application, then the original STMT entry to internal (suspense) account is converted to special entry with asset type as PAYSUS or RECEIVESUS. Nostro – If the target account passed from the underlying application is a NOSTRO account, and the Customer option is set, then the payables or receivables are reported under PR.CUSTOMER.BALANCE . NULL – If no option is set, then the system continues to work as usual. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Val Date Sys Id; Val Date By Sys ; Use Pay Rec Sys | Enables the definition of accounting treatment for specific cash-based applications, where it is different from the default accounting treatment. If the default accounting system is trade dated, for the application mentioned in Val Date Sys Id , a different accounting system can be defined. For example, if SEC.TRADE is to follow TDGL accounting system, the Val Date Sys Id is defined as SCTR and Val Date By Sys is defined as TDGL. The Use Pay Rec Sys field can be flagged as Yes or No, which is used in the suspense processing for the specific application. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Vd Cat Start; Vd Cat End; Val Date By Cat; Use Pay Rec Cat | Enables the definition of accounting treatment for specific category or range of categories, where it is different from the default accounting treatment and application specific (if defined) accounting treatment. The category level definition takes precedence over the system level and application level definition. The Use Pay Rec Cat field can be set to Yes or No, which is used in the suspense processing for the specific category. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Vd Cat Sys Id; Vd Cat Sys Start; Vd Cat Sys End; Val Date By Cat Sys; Use Pay Receive Cat Sys | If the accounting system for specific categories of an application is different from the default accounting system, it can be setup using these set of fields. The application can be defined in Vd Cat Sys Id , the category or range of categories can be defined in the Vd Cat Sys Start and Vd Cat Sys End fields. The accounting system applicable to this setup are defined in the Val Date By Cat Sys field. The Use Pay Receive Cat Sys field can be set to Yes or No, which is used in the suspense processing for the specific category. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Entry Category; Sus Category; Suspense Txn In; Suspense Txn Out; Suspense History | The format of Entry Category can either be CATEGORY-FX.POS.TYPE or CATEGORY, which determines the suspense account to be used when operating in a value dated accounting system. If the position type for the Entry Category does not exist, then the entry category alone is used to determine the suspense category. Else, the default suspense category is used. When a split value dated transaction is processed in a value dated accounting system then the first leg is balanced against a suspense account. This is washed out when the second leg reaches its value date. The suspense account that is used is determined by the category of the second leg entry. The Entry Category field and its associated field Sus Category defines this relationship. Example XX.1 ENTRY.CATEGORY YY.1 SUS.CATEGORY 19998 XX.2 ENTRY.CATEGORY 5000-XX YY.2 SUS.CATEGORY 19999 Entry Category is a start of range value. Hence in this example, second leg entries with a category in the range 0 - 4999 uses account LCL199980001 (where LCL is the local currency code) and entries with a category 5000 and above uses LCL199990001 for suspense processing. To define a default suspense account for all the entries, configure as shown below: XX.1 ENTRY.CATEGORY YY.1 SUS.CATEGORY 19998 The purpose of defining different suspense category is to allow the splitting of suspense movements, for value dated accounting, within the CRB. For example, it is possible to report suspense entries for nostro accounts separately from suspense entries for current accounts. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Sys Code; Nostro Default; Def Override; Use First Acct; Default Order | These set of fields are used for defaulting the settlement nostro account applicable to the transaction defined in the Sys Code field. The Sys Code field is a combination of Application-Nature of transaction, for example, LD-PRIN or LD-INT. These values must be defined upfront in AC.SYS.CODES application. The Nostro Default field is used to specify how settlement accounts are defaulted when using a nostro account for the associated Sys Code . A null value implies that the nostro account is always defaulted. The following are the options in this field: AGENCY – Defaults only when agency conditions exist. NONE – No nostro account is to be defaulted. The Def Override field defines whether an override is required when the default account number does not match the account number entered on the deal. Additionally, if the account with bank, intermediary bank or beneficiary account number differs from the default derived from the information on the agency file, then an override is raised if this field is set to Yes. The Use First Acct field defines whether an account is to be defaulted when more than one possible default account exists. The following options are available in this field: Yes – First account of the customer in any company is defaulted. No – If more than one account is present in the current company, then no defaulting takes place. In a multi-book setup, the following additional options are available for this field: CUR – First account of the customer in current company is only defaulted. FRS – First account of the customer in the current company as first choice followed by first available account in any company is defaulted. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Cheque Register; Chq Dep Txn; Def Coll Susp; Chq Col Txn; Chq Ret Txn; Def Ret Susp; Return Txns; Return Susp Cat | The Cheque Register field indicates whether or not the cheque issue and management functionality within Temenos Transact has been activated. The Yes or No value entered in this field controls the defaulting of cheque type in DATA CAPTURE (DC) or FUNDS TRANSFER (FT) or TELLER (TT) application as well as payment stop processing. The list of transaction code for cheque on collection, clearing and returned cheque and the corresponding suspense accounts where the value of cheque needs to be parked in the clearing process can be defined in these set of fields. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Net Od Appl; Net Od Override; Net Locked Override | The Net Od Appl field specifies the Temenos Transact application for which debit and credit entries to an account in a transaction must be netted for displaying the overdraft and cash flow overrides. The allowed applications are LOANS AND DEPOSITS (LD), TELLER (TT), COLLATERAL (CO), FUNDS TRANSFER (FT), ARRANGEMENT ARCHITECTURE (AA) or ALL. When this field is set to ALL, the functionality is applied for all transaction irrespective of the application. The pre-condition for the suppression of overrides is to set the Net Od Override field as Yes. If Net Od Appl holds the value ALL, the system does not permit any other multi-value to be input. Either applications are manually input in a multi-value block or ALL value is used. For example, if the Net Od Appl field is set to ALL and the Net Od Override field is set to Yes and a transaction is made using the same account as both debit and credit account, no override is generated for any excess amount. Suppression of Unnecessary Overrides: If a single contract creates both credits and debits to an account, if the net effect of the contract is to credit the account, it is possible to suppress the override generated for the debit side of the transaction. Example If a discounted loan is arranged for a customer, whereby the customer has a balance of £10, receives a credit of $1000 for the loan, but also a debit of $100 for the upfront payment of interest. The system usually generates an override specifying that the customer is debited $100 and the customer is being overdrawn by $90. However, it is possible by configuring the Net Od Appl as LD and Net Od Override fields as Yes in the ACCOUNT.PARAMETER to net off the differences, so as the credit of $1000 exceeds the debit of $100 and the override is suppressed. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Retain Ac Balances | Defines whether balances need to be maintained in ACCOUNT or not. When set to Yes the balances are updated in ACCOUNT and EB.CONTRACT.BALANCES . When set to N the balances are not updated in ACCOUNT , but updated only in EB.CONTRACT.BALANCES . Default value is Yes. Changing this setup from Yes to No clears the existing account balances automatically. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Booked Balance | Defines which booked balance is recorded in the STMT.ENTRY record when the transaction is booked. The following are the options available in this field. Online Actual Bal – Records the account balance from the GL perspective, this means that future dated movements are not included. Traded Dated Gl Bal – Records the account balance from a customer perspective, which means that future dated movements recorded as PAY or RECEIVE are included. The enhanced transaction search uses the value in this field to display the output in Booked Balance column of the enquiries |  |  |  |  |  |  |  |  |  |  |  |  |  |  |

**Misc**

| Group ID | Group Name | Category | Sector | Residence |
|---|---|---|---|---|
| 1 | Current account – Individual | 1001 | 1001 |  |
| 2 | Current account – Staff | 1001 | 1002 |  |
| 3 | Savings account – Resident | 6001 |  | UK |
| 4 | Savings account – Non-Resident | 6001 |  |  |
| 5 | Nostro account | 5001 | 3001 |  |
| 5002 | 3002 |  |  |  |
| 5003 | 3003 |  |  |  |

**Misc**

| Key | Description |
|---|---|
| TFLC | Letter of credit |
| DDSTD | Direct debit standalone |
| BROKER | Brokerage to be paid |
| DDSUSP | Direct debit suspense |
| LCDIFF | Letter of credit difference |
| RCSUSP | Suspense category for RC |
| SLDIFF | SL Skim account |
| SUSPPD | Suspense Past Due |
| SYFUND | SY Fund |
| ACERROR | Currency mismatch suspense |
| DDCLAIM | Direct debit claim |
| EXCHADJ | Forex Revaluation profit and loss |
| IACLOSE | IA profit and loss year end closeout |
| INTERCO | Inter branch |
| LCAMORT | Letter of credit amortisation |
| LCLSUSP | Letter of credit suspense |
| LGCLOSE | LG profit and loss year end closeout |
| MDCLAIM | MD fee settlement |
| MERGEMM | MM merge |
| NETTING | Netting suspense |
| PDREPAY | PD repayment |
| PLCLOSE | Profit and loss year end closeout |
| SWREVAL | Swap revaluation profit and loss |
| U-AAWOF | AA loan write-off |
| CONTDIFF | Contingent difference suspense |
| CONTSUSP | Contingent suspense |
| CUSDEBIT | Sight discount suspense |
| LDCANCEL | LD cancellations |
| NDFGIVEN | NDF given |
| NDFTAKEN | NDF taken |
| OFFLIMIT | Off balance sheet limit |
| RESFWDCR | Foreign exchange reserve – forward credit |
| RESFWDDR | Foreign exchange reserve – forward debit |
| SCCASUSP | SC corporate act suspense |
| SUSPENSE | Suspense |
| SUSPFXCR | Suspense credit FX |
| SUSPFXDR | Suspense debit FX |
| SUSPSCCR | Suspense securities credit |
| SUSPSCDR | Suspense securities debit |
| EXCHALFWD | Asset and liability forward revaluation |
| ICASUSPCR | ICA suspense credit accounting |
| ICASUSPDR | ICA suspense debit accounting |
| LCPARTACC | Syndicated LC part account category |
| MARKETING | MKT exchange |
| OFFSUSPCR | Non-utilisation fee credit |
| OFFSUSPDB | Non-utilisation fee debit |
| RESSWAPCR | Foreign exchange reserve - SWAP credit |
| RESSWAPDR | Foreign exchange reserve - SWAP debit |
| SUSPDEBIT | Suspense debit accounting |
| SUSPLMMCR | Suspense credit MM and LD |
| SUSPLMMDR | Suspense debit MM and LD |
| AASUSPENSE | Suspense for AA transactions |
| DIFFERENCE | Daily difference on data capture |
| INTERCO-IA | Inter branch - IA |
| INTERCO-IF | Inter branch - IF |
| SLROLLOVER | For SL rollover |
| SUSPCREDIT | Suspense credit accounting |
| SUSPDXCGCR | DX charge tax suspense credit |
| SUSPDXCGDR | DX charge tax suspense debit |
| SUSPDXIMCR | DX initial margin suspense credit |
| SUSPDXIMDR | DX initial margin suspense debit |
| SUSPDXMTCR | MTM suspense credit |
| SUSPDXMTDR | MTM suspense debit |
| SUSPDXOMCR | DX option variation margin suspense credit |
| SUSPDXOMDR | DX option variation margin suspense debit |
| SUSPDXPRCR | DX option premium suspense credit |
| SUSPDXPRDR | DX option premium suspense debit |
| SUSPDXRPCR | DX realised profit and loss suspense credit |
| SUSPDXRPDR | DX realised profit and loss suspense credit |
| SUSPDXVMCR | DX variation margin suspense credit |
| SUSPDXVMDR | DX variation margin suspense debit |
| SUSPFTBULK | Suspense for bulk FT or STO |
| SUSPFTINWD | Funds Transfer inward |
| U-AACAPTURE | AA take over charge |
| U-CLGSUSPCR | Inward clearing credit suspense |
| U-CLGSUSPDR | Inward clearing suspense |
| U-AASUSPENSE | Suspense for AA adjustments |

**Misc**

| Value | Description |
|---|---|
| 1 | When the Local Currency field value starts with BE (identifies Belgium). |
| 2 | When the Local Currency field value starts with LU (identifies Luxembourg). |
| 3 | For 10 digit account numbers with a modules 11 check. |
| 4 | For 11 digit account numbers constructed with a two digit bank number prefix defined in the Acc Bkno Prefix field , followed by seven identifying digits and a two digit mod 11 check digit. The prefix may contain leading zeros. |
| 5 | For a standard check, digit calculation with the account numbers zero filled to the Account Mask field. |
| 6 | For a 12-14 digit number with two check digits, the first 6 digits, and the second on the remaining digits. The check digits are calculated using mod 11. |
| 99 | No check digit calculation with the account number zero filled to the Account Mask field. |
| @routine name | Where a local subroutine performs the check digit calculation. |
| Blank | In all other cases. |

**Misc**

| Business Event | Description |
|---|---|
| accounts.updatefundsAuthorization.fundsAuthorizationApproved | Event to be emitted when bank user approves funds authorisation for accounts |
| accounts.updatefundsAuthorization.fundsAuthorizationRejected | Event to be emitted when bank user rejects funds authorisation for accounts |
| deposits.updatefundsAuthorization.fundsAuthorizationApproved | Event to be emitted when bank user approves funds authorisation for deposits |
| deposits.updatefundsAuthorization.fundsAuthorizationRejected | Event to be emitted when bank user rejects funds authorisation for deposits |

**Misc**

| S.No. | Parameters | Description |
|---|---|---|
| 1. | ACCOUNT.PARAMETER | It has the information pertaining to cash flow, accounting method, generation of alternate identifier to account number, account level balance maintenance, netting and cheque issue management and so on. |
| 2. | CUSTOMER | To create a user account, the account holder should be registered as a customer in Temenos Transact . The information like name, address, age, residence, sector, language, industry, signature and so on, pertaining to the user is captured in the application. |
| 3. | CATEGORY | Based on the business needs, category codes defined in Temenos Transact has to classify financial transactions. Use of the codes together with personal customer characteristics enables the bank to produce balance sheets and returns reflecting a coordinated and structured view of its operation, by directing business transactions to their appropriate report. |
| 4. | CURRENCY | It allows the user to capture the operating currency of the account and it should be a record or value in the currency application. Account currency cannot be changed once the account is authorised as the balances are maintained in the currency. |
| 5. | ACCT.GEN.CONDITION | It allows the user to define the grouping condition for accounts for which the same conditions of interests and charges apply. Based on the business needs, category codes along with CUSTOMER attributes like Sector and Residence enable grouping of accounts. These attributes and their order of priority is defined in CONDITION.PRIORITY application for ACCOUNT record. |
| 6. | ACCT.GROUP.CONDITION | It allows the user to define the rules for accounts belonging to a group and specific currency mentioned in the table. Some examples for rules defined are Notice withdrawals, account violations, deferring interest and charges, rounding rules for interest and premium interest, automatic IBAN generation and so on. |
| 7. | ACCOUNT.DEBIT.INT | It allows the user to define special debit interest conditions when the corresponding group interest conditions are not suitable. The user can define Interest to be calculated on daily, average using value dated balance and interest rate to fixed or linked to basic rates. |
| 8. | ACCOUNT.CREDIT.INT | It allows the user to define special credit interest conditions when the corresponding group credit interest conditions are not suitable. Credit interest rates can be specified for different balance levels. Rates can apply to the entire balance or a part between the two-balance levels. |
| 9. | ACCT.CAPITALISATION | It allows the user to specify the next date and subsequent frequency of application of debit and credit interest capitalisation for a specific account. |
| 10. | GROUP.DEBIT.INT | It allows the user to specify the calculation method of debit interest for a group of accounts and provides the link to the GENERAL.CHARGE , where the charges applicable to the same groups of accounts are specified. The user can also specify negative interest and tax on interest. |
| 11. | GROUP.CREDIT.INT | It allows the user to specify the calculation method of credit interest for groups of accounts. The user can also specify second interest on the account with different capitalisation frequency. |
| 12. | GROUP.CAPITALISATION | It allows the user to specify the next date and subsequent frequency of application of debit and credit interest capitalisation for a group of accounts. |
| 13. | ACCOUNT.CLASS | It allows the user to define the account class records, which can be used by other Temenos Transact applications to construct account number or to check the account number for a particular group. |
| 14. | ACCOUNT.ACCRUAL | At company level, it provides the system with information on how and when to process accruals of interests and charges on customer accounts. Accrual process can be specified at Account Category and Account Group for which the associated interest accrual parameters are defined. |
| 15. | SAVINGS.PREMIUM | It enables the user to pay premium on the savings deposits if the savings account qualify the eligibility criteria defined in this table. |
| 16. | AC.FUNDS.DIVERSION.PARAM | The funds diversion is setup from the off-balance sheet Transaction Account to the on-balance sheet Diversion Account. The system provides flexible options that allows the bank to control the ability to suppress the funds diversion processing for specific transactions for Transaction accounts setup for funds diversion. The bank will be able to define the following options for funds diversion: The default funds diversion behaviour. To suppress Funds Diversion processing for specific activities by mentioning or defining the associated transactions code as an exception to the default rule. |
| 17. | ACSWIT.PARAMETER | This parameter table stores the validity period decided by the bank for the switch out service. The validity period can be defined in days or months. The ID of this record represents the Temenos Transact Company ID. |
| 18. | DDA.SERVICE.PARAMETER | This table helps the bank to decide whether the payment made by the account holder in a specific currency is allowed or not. Also, enables the Bank to change the core decision for Account Currency and to return the Payment Currency. |
| 19. | AC.ACCOUNTING.PARAM | This table helps to parameterise the accounting related processes based on the Max No Of Splits defined. |

**Misc**

| S.No. | Product Name | Product Attributes |
|---|---|---|
| 1. | Demand / Current Account | Current Account can be created using category code between 1000-1999 Feature of availing overdraft facility Mode of operation - single or joint Interest liquidation option |
| 2. | Savings Account | Savings account can be created using the category code ranging between 6000-6999 Regular SB accounts AA deposit accounts Overdraft facility Mode of operation - single or joint Interest liquidation option Alert subscription Mandate registration Passbook facility |
| 3. | Loan Accounts | Loan accounts can be created using the category code between 3000-3999 Islamic loan accounts AA loan accounts |

**Externalise Transact Limit Exposure**

| Field Name | Description |
|---|---|
| EXTERNAL.CONTRACT.ID | Indicates the unique identifier |
| CONTRACT.APPLICATION | Indicates the name of the application where the contract is initiated |
| CONTRACT.ID | Indicates the contract ID from the external system |
| CURRENCY | Indicates the currency of the contract |
| START.DATE | Indicates the start date or value date of the contract |
| MATURITY.DATE | Indicates the maturity date of the contract |
| BOOKING.DATE | Indicates the date in which the contract is booked in the source system |
| CATEGORY | Indicates the product category of the contract. It should be a valid record from the CATEGORY application. |
| CUSTOMER.IDS | Indicates the customer of the contract. If there are multiple customers defined, the primary customer is identified based on the value of the associative REPORTING.CUSTOMER field. If the REPORTING.CUSTOMER field is set as ‘Yes’, the respective customer is treated as primary customer for the contract. |
| REPORTING.CUSTOMER | Indicates whether the customer (mentioned in the CUSTOMER.IDS field) is a reporting customer (YES) or not. If there are multiple customers defined for the contract, the primary customer is identified with the help of this field. |
| LIMIT.ID | Indicates the limit ID to which the contract is linked. |
| LIMIT.PRODUCT | Indicates the limit product ID linked to the contract. It should be a valid record from the LIMIT.REFERENCE application. |
| SYSTEM.ID | Indicates the module ID of the application, if the contract is originated from Standalone Transact System. It should be a valid record from the EB.PRODUCT application. |
| SOURCE.SYSTEM | Indicates the identifier of the source system from where the contract is initiated. |
| ADDITIONAL.DETAILS.LABLE | Allows the user to map additional field name from external application through which the data can be sent to Transact Limit System. |
| ADDITIONAL.DETAILS.VALUE | Allows the user to map the additional field value from external application through which data can be sent to Transact Limit System. |

**Externalise Transact Limit Exposure**

| Event Name | Description |
|---|---|
| creditLimits.updateContractTerm.contractTermUpdated | Indicates the change in contract terms |
| creditLimits.updateContractProperties.contractDetailsUpdated | Indicates the change in properties of the contract |
| creditLimits.updateContractOwners.contractOwnersUpdated | Indicates the change in the owner of the contract |
| creditLimits.updateContractLimit.contractLimitUpdated | Indicates the change in the limit of the contract |
| creditLimits.recordContractLink.contractRecorded | Indicates the contract linkage with the limit |
| creditLimits.recordContractClosure.contractClosed | Indicates the closure of the limit |
| creditLimits.delinkContract.contractDelinked | Indicates the delinked contract from the limit |

**Externalise Transact Limit Exposure**

| Field Name | Description |
|---|---|
| LIMIT.ID | Contains the Limit ID to which the contract is linked |
| TRANSACTION.APPLICATION | Contains the name of the application from where the transaction is initiated |
| TRANSACTION.REFERENCE | Contains the transaction reference |
| CONTRACT.ID | Contains the contract ID for which the transaction is initiated. It should be the ID of the LI.EXTERNAL.CONTRACT application. |
| CONTRACT.COMPANY | Contains the company in which the contract resides |
| TRANSACTION.CURRENCY | Contains the currency in which the transaction is initiated from the source system |
| TRANSACTION.AMOUNT | Contains the exposure amount to be updated as part of the transaction from the source system |
| CR.DR.MARKER | Indicates the sign of the transaction based on which the exposure is debited or credited |
| COMMITMENT.CONTRACT | Flag to indicate whether the contract is to update commitment only |
| DRAWING.CONTRACT | Flag to indicate the drawing transaction. When a commitment is not set, it is taken as a ‘yes’, by default. |
| DELETE.REASON | Contains the reason of deleting the exposure passed from the source system |

**Externalise Transact Limit Exposure**

| Field Name | Description |
|---|---|
| Category | Indicates the category code of the deal |
| Currency Market | Indicates the currency market corresponding to the contract. |
| Customer Id | Indicates the counterparty ID |
| Account Officer | Indicates the treasury department officer for the deal |
| Limit Product | Indicates the limit product linked to the deal |
| Limit Id | Indicates the Limit that will be linked to the FX deal |
| Transaction Currency | Indicates the bought currency |
| Transaction Amount | Indicates the bought currency original amount |
| Fx Other Currency | Indicates the sold currency |
| Fx Other Amount | Indicates the sold currency amount |
| Booking Date | Indicates the Forex deal date |
| Value Date | Indicates the value date of bought currency of the deal |

**Externalise Transact Limit Exposure**

| API URL | Description |
|---|---|
| /holdings/creditLimits/accounts/{accountId} | Creates a contract with static information such as contract type, reference, maturity, customers and system details. This establishes a link between contract static data and the credit limit and checks if the contract is applicable to be linked against specified limit based on rules defined for the credit line product. |
| /holdings/creditLimits/accounts/transactions/{transactionId} | Creates movements on credit limits with details such as transaction reference, amount, value date, revolving nature of contract and credit or debit indicator for contracts upon commitment or utilization or repayment of credit limit. |
| /holdings/creditLimits/forex/transactions/{transactionId} | Creates movements on credit limits with details such as transaction reference, buy currency, buy amount, value date, sell currency, sell amount for forex transactions. |

**Externalise Transact Limit Exposure**

| Event Name | Description |
|---|---|
| CreditLimits.CreateSecuredLimit.SecuredLimitCreated | Indicates the creation of secured limit |
| CreditLimits.CreateUnsecuredLimit.UnsecuredLimitCreated | Indicates the creation of unsecured limit |
| CreditLimits.CreateGroupSecuredLimit.GroupSecuredLimitCreated | Indicates the creation of group secured limit |
| CreditLimits.CreateGroupUnsecuredLimit.GroupUnsecuredLimitCreated | Indicates the creation of group unsecured limit |
| CreditLimits.CreateLiabilityGroupLimit.LiabilityGroupLimitCreated | Indicates the creation of customer liability group |
| CreditLimits.CancelLimit.LimitCancelled | Indicates cancellation of the limit |
| CreditLimits.ReverseGroupUnsecuredLimit.GroupUnsecuredLimitReversed | Indicates the reversal of group unsecured limit |
| CreditLimits.ReverseGroupsecuredLimit.GroupSecuredLimitReversed | Indicates the reversal of group secured limit |
| CreditLimits.ReverseLiabilityGroupLimit.LiabilityGroupLimitReversed | Indicates the reversal of liability group limit |

**Misc**

| Business Event | Description |
|---|---|
| creditLimits.createLimitParameter.limitParameterCreated | Event to create limit parameter |
| creditLimits.updateLimitParameter.limitParameterUpdated | Event to amend limit parameter |
| creditLimits.createProduct.productCreated | Event to create limit product |
| creditLimits.createUtilisationProduct.utilisationProductCreated | Event to create utilisation limit product |
| creditLimits.createValidationProduct.validationProductCreated | Event to create validation limit product |
| creditLimits.createIntradayProduct.intradayProductCreated | Event to create intraday limit product |
| creditLimits.createReservationProduct.reservationProductCreated | Event to create reservation limit product |
| creditLimits.updateLimitProduct.productUpdated | Event to amend limit product |
| creditLimits.updateIntradayProduct.intradayProductUpdated | Event to amend intraday limit product |
| creditLimits.cancelLimitProduct.productCancelled | Event to cancel limit product |
| creditLimits.createSecuredLimit.securedLimitCreated | Event to create secured limit |
| creditLimits.createUnsecuredLimit.unsecuredLimitCreated | Event to create unsecured limit |
| creditLimits.createGroupSecuredLimit.groupSecuredLimitCreated | Event to create secured group limit |
| creditLimits.createGroupUnsecuredLimit.groupUnsecuredLimitCreated | Event to create unsecured group limit |
| creditLimits.createReportingLimits.customerReportingLimitsCreated | Event to create reporting credit limit |
| creditLimits.updateIntradayLimit.intradayLimitUpdated | Event to amend intraday credit limit |
| creditLimits.createReservationLimit.reservationLimitCreated | Event to create reservation limit |
| creditLimits.limitExpiryDueDate.expiryDue | Event for limit expiry due date |
| creditLimits.limitExpiryFailure.expiryFailed | Event for limit expiry failure |
| creditLimits.limitReviewDate.reviewDateReached | Event to review limit on review date |
| creditLimits.limitReviewDueDate.reviewDue | Event to review limit |
| creditLimits.updateLimit.limitUpdated | Event to amend limit |
| creditLimits.updateLimitAmount.limitAmountUpdated | Event to update limit amounts |
| creditLimits.updateLimitAvailability.limitAvailabilityUpdated | Event to update limit availability |
| creditLimits.updateExpiryDate.limitExpiryDateUpdated | Event to update expiry date of limit |
| creditLimits.reportLimitIncrease.limitIncreased | Event to increase limit schedule |
| creditLimits.reportLimitDecrease.limitDecreased | Event to decrease limit schedule |
| creditLimits.reportLimitExpiry.limitExpired | Event to indicate limit expiry |
| creditLimits.reportLimitBreach.validationLimitBreached | Event to validate limit breach |
| creditLimits.cancelLimit.limitCancelled | Event to cancel limit |
| creditLimits.updateExposure | Transaction command event for exposure update |
| creditLimits.updateExposure.exposureUpdated | Event to update exposure in the limit |
| creditLimits.deleteExposure | Transaction command event for exposure delete |
| creditLimits.delinkContract | Event to be emitted when limit is delinked from contract |
| creditLimits.delinkContract.contractDelinked | Event to delink contract from the limit |
| creditLimits.recordContractClosure | Event to be emitted when contract is linked to limit closed |
| creditLimits.recordContractClosure.contractClosed | Event for limit contract closure |
| creditLimits.recordContractLink | Event to be emitted for the limit and contract link |
| creditLimits.recordContractLink.contractRecorded | Event to link contract to the limit |
| creditLimits.updateContractLimit | Event to be emitted to update limit property linked with contract |
| creditLimits.updateContractLimit.contractLimitUpdated | Event to update limit in limit contract |
| creditLimits.updateContractOwners | Event to be emitted when customer changes the contract linked to limit |
| creditLimits.updateContractOwners.contractOwnersUpdated | Event to update owner in limit contract |
| creditLimits.updateContractProperties | Event to be emitted when there is a change in contract linked to limit |
| creditLimits.updateContractProperties.contractDetailsUpdated | Event to update limit contract properties |
| creditLimits.updateContractTerm | Event to be emitted when there is a change in contract term |
| creditLimits.updateContractTerm.contractTermUpdated | Event to update term in limit contract |
| creditLimits.updateTransactionStatus | Transaction command event to authorise exposure |

**Misc**

| S.No. | Parameters | Description |
|---|---|---|
| 1. | LIMIT.PARAMETER | This application allows the user to define the parameter that determine the way in which LI module operates. It also allows the user to define the following: If foreign exchange contracts are to be netted. The date and frequency at which the revaluation occurs. The date and frequency at which the currency, commodity and country reports must be produced. The date and frequency at which central liability report must be produced in the back end process. Defining the frequency at which the collateral accounting service should be run. Defining the accounting type based on which entries would be booked in Limit's EB.CONTRACT.BALANCES record, depending on the Balance types specified in respective Collateral Codes. |
| 2. | LIMIT.REFERENCE | This application allows the user to define the parameter, which links accounts and contracts to Limits (LI) products. In addition, it allows the user to define margin level or percentage ration between the limit amount utilised and the value of collateral available. It allows the user to define different limit amounts for contracts on different maturity dates. When the LIMIT.TYPE field is set to: Utilisation - The Limit product holds the Utilisation Limit records. Validation - The Limit product holds the Validation Limit records, which constitutes the maximum cap allowed for the underlying Utilisation Limits within a Limit structure. Standalone - The Limit product holds the Standalone Limit records, which have the same functionality as Utilisation Limit records apart from the fact that they hold no parent or child Limits. SUPPRESS.ACCOUNTING field is set to ‘Yes’ to suppress any GL accounting performed against the Limit records under the Limit product. This field accepts the input when the Limit record has nothing set in the Reference Child field. When the THIRD.PARTY.EXPOSURE field set to ‘Yes’, it marks the given Limit records under the Limit product to hold the third party exposure for their Customer(s). Any exposure created against these Limit records are excluded from the bank’s risk reports. |
| 3. | LIMIT.COMMODITY | This application allows the user to define the limits by commodity (industry type). |
| 4. | LIMIT.COMMODITY.GRP | This application allows the user to define the commodity industry groupings. |
| 5. | LIMIT.COUNTRY | This application allows the user to define the limits by countries or group of countries. |
| 6. | LIMIT.COUNTRY.GRP | This application allows the user to define country groupings. |
| 7. | LIMIT.CURRENCY | This application allows the user to define limits by currency. |
| 8. | LIMIT.CHANGE | This application allows the user to make changes to the existing limit records. User can add or change customer liability, currency and limit percentage. |
| 9. | LIMIT.REPORTING.PARAMETER | This application allows the user to enable the reporting of breach on the internal amount of the validation limit. Pro Data Calculation field mentions whether pro-rata calculation has to be done irrespective of manual percentage in Common Exposure Reports. Check Validation Limit Breach field indicates if breaches to validation limits have to be reported in a separate file. |
| 10. | LIMIT.NETTING.PARAM | This application allows the user to activate or deactivate the foreign exchange limit netting option, when required. |
| 11. | LI.MULTI.CUSTOMER.LIMIT.PARAMETER | This application allows the user to configure the rules for multi- customer limits without joint liability rules based on customer segments. Using this parameter, Users can configure the rules for Joint/Multi Customer Limit based on customer segment. Multi-Customer limits can be created with customers belonging to different risk groups or no group based on this parameter setup. |
| 12. | LI.TIME.CODE | This application allows the user to configure the charges based on the level of designated AA account for the respective balance types and the possibility to calculate charges per each time band amount. |
| 13. | ADMIN.LIMIT.PARAMETER | This application allows to set up limit parameters, application wise. It lists the limit parameter application records (if exists) and also user can amend the record (with limited fields, like Application, Decision to fields). |

**Sec Lim Coll**

| Field | Description |
|---|---|
| External Collateral Currency | Specifies the currency of the collateral from external system. |
| External Collateral Value | Specifies the value of collateral from external system. |
| Total External Collateral Value | Specifies the total collateral value in limit currency. |


### Limits_Collateral - OV (OV)


**Misc**

| ID | Type | Description |
|---|---|---|
| 100 | CASH | All types of Cash, Accounts, Money Market (MM), Loans & Deposits (LD) and Deposit Contracts |
| 200 | HOUSE | All forms of property; from domestic to industrial properties |
| 300 | ART | Includes paintings, sculpture, jewellery and so on |
| 400 | SHARES | Value of a customer's shares |

**Misc**

| COLLATERAL . TYPE | Description | COLLATERAL . CODE | Description |
|---|---|---|---|
| 100 | Cash | 101 | MM Deposits |
| 102 | LD Deposits |  |  |
| 103 | Savings Accounts |  |  |
| 200 | Houses | 201 | Business Property |
| 202 | Domestic Property |  |  |

**Misc**

| S.No. | Parameters | Description |
|---|---|---|
| 1. | COLLATERAL.PARAMETER | This application allows the user to define the company-level system parameter. User can define if address is to be defaulted from CUSTOMER application. To cover the currency conversion risk factor, margin for the collateral currency is also defined when limit currency is different from collateral currency. To retain collateral records in live table, retention period value must be defined in the collateral parameter setup. Specification to determine which balance from EB.CONTRACT.BALANCES table to be considered for updating in collateral record. |
| 2. | COLLATERAL.TYPE | This application allows the user to define different types of collaterals like building stocks and guarantees and so on. Information in this table enables the client to arrive at collateral value, revaluation of collateral value and linking to other applications in Temenos Transact . Market value or face value of the collateral, value for general ledger purpose, third party value (value of collateral item outside Temenos Transact ) are specified in this table. |
| 3. | COLLATERAL.CODE | This application allows the user to determine how collateral values are re-allocated across central bank reporting lines. Enables the system to perform recalculation of percentage of collateral cover applicable. Enables the system to mention the default review frequency. Enables the system to mention the default review frequency. Enables to update Allocated Balance type, Utilized balance type and Unutilized balance type. |
| 4. | COLLATERAL.EXCLUSION | This application allows the user to define the criteria for the exclusion of collaterals. CURRENCY, COUNTRY, SECURITY.CODE, INDUSTRY, ISSUER and COUNTERPARTY values are used to define the criteria. |
| 5. | CO.CURRENCY | This application allows the user to define the rules to modify the lower advance ratio of the assets valued in a currency. Enables the user to define the currency level concentration cap. Enables the user to define the specific margin rates at product level. |
| 6. | CO.VALUATION.PARAMETER | This application allows the user to define the margin calculation, asset allocation, asset valuation for the collateral process. Enables the user to specify if the collateral is allocated against limits or liabilities. Enables the user to mention the discretionary portfolios. |
| 7. | CUSTOMER.COLLATERAL.TYPE | This application allows the user to define specific collateral execution value for specific customers. |
| 8. | CO.ELIGIBILITY | This application allows the user to define the eligibility rules for collateral against the limit products to which the collateral is linked. |
| 9. | CO.INDUSTRY | This application allows the user to define the concentration cap at industry levels for security assets. |
| 10. | CO.RANKING | This application allows the user to define the ranking rules for the collaterals against limit products. |
| 11. | CO.COUNTRY | This application allows the user to define the concentration cap rules for the collateral country. |
| 12. | CO.COUNTRY.GROUP | This application allows the user to define the concentration cap rules for a group of countries. |

**Direct**

| Field | Description |
|---|---|
| Xx-Xx | Value in the field must be greater than the previous field, that is, value of 2nd sub-value must be less than first sub value |
| Xx-Xx-Tier Margin Rate | Value must be within 0 to 100 |
| Tier Adj Margin Rate | Value must be within 0 to 100 |
| Concentration Cap | Concentration cap for each asset |
| Customer Ccy | Currency in which Deficit / Surplus has to be reported |

**Misc**

| Field | Description |
|---|---|
| Online Val | Indicates whether automatic online valuation needs to be activated |
| Exclude Events.1 | Events excluded during the online valuation process |
| Use Facility Application | Field to set if Margin Lending functionality is required or the old Lombard functionality is to be used |
| Priority Api | API to determine priority for online valuation |

**Misc**

| Field | Description |
|---|---|
| Online Val | This is set to Yes in Model Bank |
| Priority API | A core API called OV.PRIORITY.API is released. This checks if the trigger is a batch job or online job and handles valuation accordingly. |
| Use Facility Application | This is set to Yes in Model bank to ensure that Margin Lending functionality is used by default. |


---
