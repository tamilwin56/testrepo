
# Temenos Transact — General_Ledger_Accounting Module Documentation


> **Comprehensive User Guide**
> Generated: 13 April 2026
> Content: Configuration | Reference | Field Descriptions | Glossary


## Table of Contents

  - [General_Ledger_Accounting Module Overview](#general_ledger_accounting-module-overview)
    - [Sub-Module Summary](#sub-module-summary)
    - [How to Use This Guide](#how-to-use-this-guide)
  - [Chapter 1: General_Ledger_Accounting - PC](#chapter-1-general_ledger_accounting---pc)
    - [Features in General_Ledger_Accounting - PC](#features-in-general_ledger_accounting---pc)
    - [1.1  Accounting Process in PostClosing](#11-accounting-process-in-postclosing)
    - [1.2  Automatic Opening of Post-Closing Periods](#12-automatic-opening-of-post-closing-periods)
    - [1.3  Back Dated Adjustment Financial Management](#13-back-dated-adjustment-financial-management)
    - [1.4  Generating Reports From PCDatabase](#14-generating-reports-from-pcdatabase)
    - [1.5  Misc](#15-misc)
    - [1.6  Post Closing Process](#16-post-closing-process)
    - [1.7  Using the PC Database](#17-using-the-pc-database)
  - [Chapter 2: General_Ledger_Accounting - RE](#chapter-2-general_ledger_accounting---re)
    - [Features in General_Ledger_Accounting - RE](#features-in-general_ledger_accounting---re)
    - [2.1  Accounting System](#21-accounting-system)
    - [2.2  Addition of Local Reference Fields for External Interface](#22-addition-of-local-reference-fields-for-external-interface)
    - [2.3  Banking Framework Exit Point](#23-banking-framework-exit-point)
    - [2.4  Company-Specific Grouping Conditions](#24-company-specific-grouping-conditions)
    - [2.5  Currency Position](#25-currency-position)
    - [2.6  Default or Catch All or Unallocated Line](#26-default-or-catch-all-or-unallocated-line)
    - [2.7  Display of Reversal Entries in CRF Report](#27-display-of-reversal-entries-in-crf-report)
    - [2.8  Enforcing Balanced Accounting Entries](#28-enforcing-balanced-accounting-entries)
    - [2.9  Extraction of GL Information to Disk](#29-extraction-of-gl-information-to-disk)
    - [2.10  Financial Accounting](#210-financial-accounting)
    - [2.11  General Ledger Reports](#211-general-ledger-reports)
    - [2.12  Generating and Recording the Accounting Entries](#212-generating-and-recording-the-accounting-entries)
    - [2.13  Grouping Conditions for Accounting Entries](#213-grouping-conditions-for-accounting-entries)
    - [2.14  Maintenance of Line Balance Details](#214-maintenance-of-line-balance-details)
    - [2.15  Misc](#215-misc)
    - [2.16  Multi-Company Reporting](#216-multi-company-reporting)
    - [2.17  Multi GAAP](#217-multi-gaap)
    - [2.18  Position Accounting](#218-position-accounting)
    - [2.19  Printing Back-Dated Reports from CRB](#219-printing-back-dated-reports-from-crb)
    - [2.20  Printing BackDated Reports from CRB](#220-printing-backdated-reports-from-crb)
    - [2.21  Printing the Report](#221-printing-the-report)
    - [2.22  Producing Report in Non-Local Currency](#222-producing-report-in-non-local-currency)
    - [2.23  Producing Report in NonLocal Currency](#223-producing-report-in-nonlocal-currency)
    - [2.24  Recording the Contract Balances](#224-recording-the-contract-balances)
    - [2.25  Recreation of CRB](#225-recreation-of-crb)
    - [2.26  Revaluation](#226-revaluation)
    - [2.27  Soft Accounting](#227-soft-accounting)
    - [2.28  Transaction Journal Reporting](#228-transaction-journal-reporting)
    - [2.29  US GAAP Reporting](#229-us-gaap-reporting)
    - [2.30  Utility Files for Report Generation](#230-utility-files-for-report-generation)
    - [2.31  Utility for Consolidation of Accounting Entries](#231-utility-for-consolidation-of-accounting-entries)
    - [2.32  Utility for End of Year Procedure PLCLOSEOUT](#232-utility-for-end-of-year-procedure-plcloseout)
  - [Appendix A: Glossary of T24 Applications & Fields](#appendix-a-glossary-of-t24-applications-fields)
    - [Applications](#applications)
    - [Fields Referenced](#fields-referenced)
  - [Appendix B: Consolidated Field Reference](#appendix-b-consolidated-field-reference)
    - [General_Ledger_Accounting - PC (PC)](#general_ledger_accounting---pc-pc)
    - [General_Ledger_Accounting - RE (RE)](#general_ledger_accounting---re-re)

---


## General_Ledger_Accounting Module Overview


This document provides comprehensive documentation for the **General_Ledger_Accounting** module of Temenos Transact. It covers **2 sub-modules** with a total of **39 feature areas**.


### Sub-Module Summary


| # | Sub-Module | Code | Features | Description |
|---|-----------|------|----------|-------------|
| 1 | **General_Ledger_Accounting - PC** | `PC` | 7 | General_Ledger_Accounting - PC module of Temenos Transact |
| 2 | **General_Ledger_Accounting - RE** | `RE` | 32 | General_Ledger_Accounting - RE module of Temenos Transact |


### How to Use This Guide


Each feature in this document is organized into the following sections:

- 📖 **Introduction** — Overview and purpose of the feature
- ⚙️ **Configuration** — How to set up and configure the feature
- 🔧 **Working With** — Operational usage and field descriptions
- 📋 **Tasks** — Step-by-step procedures
- 📊 **Outputs** — Reports, enquiries, and generated outputs

Each feature includes a **Quick Reference Card** at the top with application names, key fields, prerequisites, and a summary. Appendices provide a full glossary, consolidated field tables, and end-to-end use-case scenarios.

---


## Chapter 1: General_Ledger_Accounting - PC


General_Ledger_Accounting - PC module of Temenos Transact


### Features in General_Ledger_Accounting - PC


| # | Feature | Sections |
|---|---------|----------|
| 1.1 | Accounting Process in PostClosing | Intro, Confi, Tasks, Outpu |
| 1.2 | Automatic Opening of Post-Closing Periods | Intro, Confi, Tasks, Outpu |
| 1.3 | Back Dated Adjustment Financial Management | Intro, Confi, Worki, Tasks, Outpu |
| 1.4 | Generating Reports From PCDatabase | Intro, Confi, Tasks, Outpu |
| 1.5 | Misc | Intro |
| 1.6 | Post Closing Process | Intro, Confi, Tasks, Outpu |
| 1.7 | Using the PC Database | Intro, Confi, Tasks, Outpu |


### 1.1  Accounting Process in PostClosing


> **📇 Quick Reference Card**
> 
> **Purpose:** *Accounting entries are raised for the adjustments made to the PC.PERIOD databases.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Accounting entries are raised for the adjustments made to the PC.PERIOD databases.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

There are no Tasks available for Accounting Process in Post-Closing feature.


#### 📊 Outputs

There are no Outputs available for Accounting Process in Post-Closing feature.

---


### 1.2  Automatic Opening of Post-Closing Periods


> **📇 Quick Reference Card**
> 
> **Purpose:** *Temenos Transact provides an ability for banks to schedule a frequency on which the system automatically opens the Post-Closing period (records in the PC.PERIOD application) and creates a Post-Closing database.*
> 
> **Applications:** `PC.PARAMETER`
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Temenos Transact provides an ability for banks to schedule a frequency on which the system automatically opens the Post-Closing period (records in the PC.PERIOD application) and creates a Post-Closing database.


#### ⚙️ Configuration

PC.PARAMETER is a high-level parameter application to define the configurations related to Post-Closing in Temenos Transact. Using this application, banks can define the frequency for each lead company at which the Post-Closing periods are to be automatically opened by the system. The following frequencies are supported:

- Monthly
- Quarterly
- Semi-Annually/Half-Yearly
- Annually/Yearly

Banks can define a specific reoccurrence day along with the above said frequencies. For example, the bank can define the frequency as the last day of every month, April 31 of every year or last day of every quarter (three months). Based on the frequency defined, the system automatically determines the first date of occurrence.


#### 📋 Tasks

There are no Tasks available for the Automatic Opening of Post-Closing Periods feature.


#### 📊 Outputs

There are no Outputs available for the Automatic Opening of Post-Closing Periods feature.


> **Related Applications:** `PC.PARAMETER`

---


### 1.3  Back Dated Adjustment Financial Management


> **📇 Quick Reference Card**
> 
> **Purpose:** *The post-closing process can be automated using the BFBACK license code for contract adjustments and accrual splits. This feature also enables the identification of adjustment entries that are applied to the post-closing sub-ledger by enriching the relevant accounting date and PC period into those e...*
> 
> **Applications:** `CATEG.ENTRY`, `Cycle Frequency`, `EB.ACCRUAL`, `FT.COMMISSION.TYPE`, `LMM.ACCOUNT.BALANCES`, `LMM.INSTALL.CONDS`, `PC.CATEG.ADJUSTMENT`, `PC.CONSOL.ADJUSTMENT` ... +6 more
> 
> **Key Fields:** *Accounting Date*, *Charge Code*, *Dbase Name*, *Deal Date*, *Last Pc Date*, *Pc Adjust For Contract*, *Pc Applied*, *Pc Period* ... +5 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The post-closing process can be automated using the BFBACK license code for contract adjustments and accrual splits. This feature also enables the identification of adjustment entries that are applied to the post-closing sub-ledger by enriching the relevant accounting date and PC period into those entries.


#### ⚙️ Configuration

This section explains the configuration required for Back Dated Adjustment Financial Management.


##### Enabling Post-closing Adjustments for Contracts

To support the post-closing adjustments for contracts, the user needs to set the Pc Adjust For Contract field in PC.PARAMETER as Yes. The Pl Category Pm Py field accepts valid category codes and allows the system determine if the accrual entry belongs to the prior period.


##### Enabling Post-closing Database Update

The system enables automatic creation of the post-closing database and triggers the update process when you define the Dbase Name field in PC.PARAMETER .

> **⚠️ Note:** This field is optional only when the BFBACK license is available. The post-closing process cannot be disabled, once it is enabled by defining the value in the Dbase Name field.


##### Parameterising PL Code for Prior Period inFT.COMMISSION.TYPE

The Pl Category Prev Mth and Pl Category Prev Year fields in the FT.COMMISSION.TYPE application are used to record the accrual and amortisation details for the previous month and previous year. These fields can be entered only with the availability of BFBACK license.


##### Recording Prior Period Category inEB.ACCRUAL

When a backdated contract with an upfront fee is created, the details of the upfront fee are recorded in the EB.ACCRUAL table. The Pl Category Prev Mth and Pl Category Prev Year fields contain the PL category code used to record the accrual and amortisation details for the previous month and year.


#### 🔧 Working With

This section explains the process for amortisation and accrual adjustment.


##### Post Closing Adjustment to Fee Amortisation

The diagram below provides the workflow in the core accounting mechanism to generate amortisation entries.


##### Amortisation and Accrual Adjustment

The core accounting framework automatically triggers the accrual and amortisation process, calculating the accrual and amortisation split for each affected period and recording these details in the EB.ACCRUAL table for backdated contracts with fees or commissions.

Entries are generated based on the availability of different P&L codes; for example, if only the P&L code for the current month is configured, the system raises one entry for the current month. However, if P&L codes for both the current month and prior periods are available, entries are generated for both periods.


##### Amortisation Split for Previous Month or Year and Current Month

The diagram below shows the high-level workflow of fee amortisation split for the previous year.

The accounting system automatically manages the split for fee amortisation through P&L entries when:

- The post-closing adjustments for contracts are enabled.
- The P&L category of the accrual entry matches the P&L category specified for the corresponding product in PC.PARAMETER .

When the above conditions are met, the system updates the P&L entry with details indicating that these entries should be applied to the latest post-closing period. The updates include:

- The accounting date with the value date available in the P&L entry. If the value date is the same as the booking date, the accounting date is updated to the last day of the month.
- The Pc Period field is updated with the latest open PC period date, which is a month-end.

A special entry is generated as a contra entry to the P&L, with a new asset type in the PCXXXXX format (For example, PC51002), the accounting date, and the Pc Period field is updated in the P&L entry.

A balancing offsetting entry is generated for the current period with the same asset type as the special entry, but without an accounting date Pc Period.

The entries with accounting dates are updated in the adjustment tables and applied to the latest open post-closing period if enabled, ensuring that all transactions are recorded in the appropriate accounting period.

Refer the example Backdated New Deposit (MM) with Upfront Fee for more information on backdated contract creation with upfront fee.


##### Post-Closing Adjustment to Interest Accruals

The diagram below shows the high-level workflow of accrual split for prior period.

The accounting system automatically manages the split for accruals through P&L entries when:

- The post-closing adjustments for contracts are enabled.
- The P&L category of the accrual entry matches the P&L category specified for the corresponding product in PC.PARAMETER .

When the above conditions are met, the system updates the P&L entry with details indicating that these entries should be applied to the latest post-closing period. These updates include:

- The accounting date with the value date available in the P&L entry. If the value date is the same as the booking date, the accounting date is updated to the last day of the month.
- The Pc Period field is updated with the latest open PC period date, which is month-end.

A special entry is generated as a contra entry to the P&L, with a new asset type in the PCXXXXX format (For example, PC51002), the accounting date, and the Pc Period updated in the P&L entry.

A balancing offsetting entry is generated for the current period with the same asset type as the special entry, but without an accounting date.

The entries with accounting dates are updated in the adjustment tables and applied to the latest open post-closing period if enabled.

Refer the example Backdated New deposit (MM) without Upfront Fee for more information on backdated contract creation.


##### Special Entries for Principal Adjustments from Backdated Transactions to Contracts

The diagram below provides the high-level workflow of principal adjustment from backdated transactions to contracts.

The core accounting mechanism identifies special entries related to the backdated adjustment of principal balance based on the value date and Asset Type (For example, LIVEDB and LIVECR for Money Market). If the value date in the entry is less than the latest post-closing period, then the system updates the accounting date and Pc Period in the special entry.

This entry, updated with the accounting date, is then recorded in the adjustment table for contracts, and undergoes the post-closing process to update the post-closing period if the adjustment for contracts is enabled. The system disregards any special entries related to accruals since these have already been accounted for.

In the RE.CONSOL.SPEC.ENTRY application, the Accounting Date field contains the accounting date, which serves as the back value date. This date is crucial during the post-closing process as it determines if an entry should be allocated to the post-closing (PC) period. The Pc Period End field specifies the post-closing period (s) relevant to the entry. The Pc Applied field indicates whether the entry is applied to the corresponding post-closing period. If the entry has been applied, this field is marked with a ‘Y’.

Refer the example Backdated New deposit (MM) without Upfront Fee for more information on backdated contract creation.


##### Account-based Entries from Backdated Transactions

The diagram below provides the high-level workflow of handling account based entries from backdated transactions.

The core accounting mechanism updates the accounting date with the value date and the PC period with the latest Pc Period date for all account-based entries that have a value date before the latest PC period date. These entries are then recorded in the corresponding adjustment table and processed through the post-closing process to update the post-closing period.

Refer the example Backdated New deposit (MM) without Upfront Fee for more information on backdated contract creation.


##### Auto-creation and Closure of Post-Closing Period

This section explains the process involved in the auto-creation and closure of the post-closing period.

Post-Closing Period Creation

This process creates a new record in the PC.PERIOD table according to the frequency set in the PC.PARAMETER table. This process also updates the latest Pc Period date and the status of the newly created record in PC.PERIOD in the Last Pc Date field in the PC.PARAMETER table.

If the database path is not defined, the process skips the creation of a record in PC.PERIOD . However, the frequency cycle continues, and the latest date is still updated in the parameter table.

Post-Closing Database Creation

This process creates a database for post-closing activities, governed by the database path specified in the PC.PARAMETER table. If the database path is not defined, this process skips the creation of the post-closing database.

Post-closing Database Update

This process triggers only if the user enables it. When triggered, it updates all contract adjustments, including those in the PC.CONSOL.ADJUSTMENT table to the post-closing database. It also updates the Pc Applied field for all adjustment entries relevant to the post-closing period. After updating the database with these adjustments, the system generates the reports.

To generate PC.PERIOD , the user must run either CREATE.PC.SERVICE or COB. This process creates the period according to the Cycle Frequency defined in PC.PARAMETER .

| From/To | Debit/Credit | Amount | Value Date | Accounting Date | Pc Period | Entry category |
|---|---|---|---|---|---|---|
| Asset Type (LIVECR) | Credit | USD120000 | 12-May-24 | 12-May-24 | 31-May-24 | RE.CONSOL.SPEC.ENTRY |
| Drawdown Account | Debit | USD120000 | 12-May-24 | 12-May-24 | 31-May-24 | STMT.ENTRY |
| Charge account | Debit | USD5000 | 12-May-24 | 12-May-24 | 31-May-24 | STMT.ENTRY |
| Asset type for fees received in advance | Credit | USD5000 | 12-May-24 | 12-May-24 | 31-May-24 | RE.CONSOL.SPEC.ENTRY |

Post-Closing Database Closure

At the start of a new post-closing cycle, the system automatically generates a PC.PERIOD record and the PC database, provided that both post-closing adjustments for contracts and the post-closing process are enabled. This process also closes any other open post-closing periods, as adjustments can no longer be posted to those periods.

| From/To | Debit/Credit | Amount | Value Date | Accounting Date | PC Period | Adjustment table (Conditional update) |
|---|---|---|---|---|---|---|
| Asset Type (LIVECR) | Credit | USD100,000 | April 10, 24 | April 10, 24 | April 30, 24 | PC.CONSOL.ADJUSTMENT |
| Drawdown account | Debit | USD100,000 | April 10, 24 | April 10, 24 | April 30, 24 | PC.STMT.ADJUSTMENT |

| From/To | Debit/Credit | Amount | Value Date | Accounting Date | PC Period | Adjustment table (Conditional update) |
|---|---|---|---|---|---|---|
| Asset Type (LIVECR) | Credit | USD 100,000 | April 10, 24 | April 10, 24 | April 30, 24 | PC.CONSOL.ADJUSTMENT |
| Drawdown Account | Debit | USD 100,000 | April 10, 24 | April 10, 24 | April 30, 24 | PC.STMT.ADJUSTMENT |
| Charge Account | Debit | USD 5000 | April 10, 24 | April 10, 24 | April 30, 24 | PC.STMT.ADJUSTMENT |
| Asset type for Fees Received in Advance | Credit | USD 5000 | April 10, 24 | April 10, 24 | April 30, 24 | PC.CONSOL.ADJUSTMENT |


#### 📋 Tasks

There are no Tasks available for the Back Dated Adjustment Financial Management feature.


#### 📊 Outputs

There are no Outputs available for the Back Dated Adjustment Financial Management feature.


> **Related Applications:** `CATEG.ENTRY`, `Cycle Frequency`, `EB.ACCRUAL`, `FT.COMMISSION.TYPE`, `LMM.ACCOUNT.BALANCES`, `LMM.INSTALL.CONDS`, `PC.CATEG.ADJUSTMENT`, `PC.CONSOL.ADJUSTMENT`, `PC.PARAMETER`, `PC.PERIOD`, `PC.STMT.ADJUSTMENT`, `PC.UPDATE.REQUEST`, `RE.CONSOL.SPEC.ENTRY`, `STMT.ENTRY`

---


### 1.4  Generating Reports From PCDatabase


> **📇 Quick Reference Card**
> 
> **Purpose:** *Reports are generated from the Post-Closing database after updating the database with the adjustment entries for various regulatory requirements.*
> 
> **Key Fields:** *Output Mode*, *PC Period End*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Reports are generated from the Post-Closing database after updating the database with the adjustment entries for various regulatory requirements.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

Related topics:

- Update General Ledger and Close Post Closing Period

Reports are generated from the post-closing database after updating the database with the adjustment entries for various regulatory requirements. After a PC database is created and updated, information can be extracted for reports. This is achieved through verification of the RE.STAT.REQUEST application, either to print out a report or store the information in HOLD.CONTROL, depending on the settings in the Output Mode field.


##### Workflow

This section helps the user to perform the below tasks:

RE.STAT.REQUEST application helps to generate and print the required report from PC Database.

To generate a report, follow the below steps:

1. Print Report .
2. In the RE.STAT.REQUEST screen, update the date in the PC Period End field.
3. Click the Validate icon to check for overrides.
4. Click the Commit icon.
5. Click the Verify icon to generate the report.


#### 📊 Outputs

There are no Outputs available for Generating Reports from PC database feature.

---


### 1.5  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Post-Closing application enables the posting of accounting adjustments and back-valued transactions to the current database, which can then be reflected in historic databases. In effect, this means that a financial period can be updated after the closing date of that period.*
> 
> **Applications:** `COLLATERAL`, `CUSTOMER`, `LIMIT`, `RE.STAT.LINE.BAL`, `RE.STAT.LINE.MVMT`
> 
> **Key Fields:** *Cycle frequency*, *Last PC Date*, *Next Frequency Date*, *Status*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- Temenos Transact Services

The Post-Closing application enables the posting of accounting adjustments and back-valued transactions to the current database, which can then be reflected in historic databases. In effect, this means that a financial period can be updated after the closing date of that period.

Databases are created to hold the closing general ledgers and background information for specified periods. These may be set to any period end position for the bank and is deemed as Open until officially closed by a member of the accounts or audit department. While month end positions are kept Open, backdated adjustments can be made through FUNDS.TRANSFER , DATA.CAPTURE , and Generic Accounting Interface (GAI) request where the accounting date can be specified. This adjusts both current reports and the reports based on open periods.

The Post-Closing module has been designed to aid in the maintenance of accurate accounts.

> **⚠️ Note:** Some aspects of retrospective transactions are not included in this module.

- GL line change to reflect sign change of Account balances, and GL Line balance, or opposite line with backdated adjustments.
- CRB (contract level balance) extract for the post-closing period(s) is not available.
- The post-closing period does not maintain the RE.STAT.LINE.BAL and RE.STAT.LINE.MVMT for post-closing adjustment
- Static changes to contracts and the CUSTOMER (for example, change of CATEGORY code and SECTOR code in the CUSTOMER) are allowed but do not cause adjustment to the post-closing figures.
- Post-closing transactions are reflected in the current LIMIT and COLLATERAL but are not reflected in LIMIT and COLLATERAL in the post-closing database.
- POSITION MANAGEMENT is not reproduced at period end dates and is not adjusted.
- Customer statements are not reproduced to show the period end position, adjustments are shown in the next statement.
- Forward cash flows of accounts are not available for the PC Period.


##### Illustrating Model Parameters

The model parameters for Post-closing are explained below:

| S.NO | Parameters | Description |
|---|---|---|
| 1 | PC.PARAMETER | It allows the user to configure the frequency for post-closing periods. Users can define the DataBase Path for master company alone and for other lead companies, DataBase Path fetches from master company. Cycle frequency is mandatory for lead companies and optional for master company. Last PC Date , Status and Next Frequency Date fields gets updated automatically upon successful creation of PC.PERIOD . |


##### Illustrating Model Products

Model Products are not applicable for this module.


> **Related Applications:** `COLLATERAL`, `CUSTOMER`, `LIMIT`, `RE.STAT.LINE.BAL`, `RE.STAT.LINE.MVMT`

---


### 1.6  Post Closing Process


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Post-Closing application can be installed using the standard release procedure.*
> 
> **Key Fields:** *Open PC Period*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The Post-Closing application can be installed using the standard release procedure.

> **⚠️ Note:** When the Post-Closing application is installed, it must be added to every lead company in the system, even if it is not to be used in all of them. User can then specify (in the Post-Closing application) the lead companies that make use of the functionality, but due to the potential sharing of relevant files between companies, it is important to ensure that the application is installed completely.


#### ⚙️ Configuration

PC.PERIOD application is used to define a series of open periods. For each period, it is possible to define the following:

- When the period is closed.
- When the final books are produced.

Each period must be set to the day before a period end date or on a month end date.

For each series of open periods, a mini database of Central Reporting Base (CRB) files, certain applications are maintained reflecting the state at the period end date. This mini-database forms a subset of the Temenos Transact database.

All adjustments made to these period end databases also raise entries in the live database. This ensures that a full audit trail can be produced at any time from the live system including all period end adjustments. As a result, override processing and account movements to update the live database occur in the usual manner.


#### 📋 Tasks

Related topics:

- Define Post Closing Periods
- Book Adjustment Entries

The Post-Closing application enables the posting of accounting adjustments and back-valued transactions to the current database, which can then be reflected in historic databases. PC.PERIOD application is used to define a series of open periods. For each period, it is possible to define the following:

- When the period is closed
- When the final books are produced

Adjustments entries to period end databases are only possible for accounts and profit and loss. It is not possible to adjust contracts in the period end database. Adjustments can be made only to post-closing open periods through transactions in FUNDS.TRANSFER , DATA.CAPTURE , and Generic Accounting Interface (GAI) request.


##### Workflow

In Transact, the user can perform the following activities:

This enquiry enables the user to define open periods.

To create a new period, follow the below steps:

1. Define Open Period .
2. In the contract screen, enter or select a value in the Open PC Period field.
3. In the Open PC PERIOD screen, enter values in the following fields: Company (Lead Company) Comp Status Database Path
4. Click the Validate icon to check for overrides and errors
5. Click the Commit icon to create the record.

This enquiry helps the user to make the adjustment entries to accounts and profit & loss.

To capture an adjustment entry using DATA.CAPTURE application, follow the below steps:

1. Adjustment to A/cs/PL by DC .
2. In the contract screen, click the New Deal icon to create a record.
3. In the Post Closing Entries screen, enter values in the following fields: Debit/Credit Transaction Code Currency Amount Category Product
4. Click the Validate icon to check for overrides and errors.
5. Click the Commit icon to create the record.

This enquiry helps the user to make the adjustment entries to accounts and profit & loss.

To capture an adjustment entry using FUNDS.TRANSFER application, follow the below steps:

1. Adjustment to A/cs/PL by FT .
2. In the contract screen, click the New Deal icon to create a record.
3. In the Post Closing Entries screen, enter values in the following fields: Debit Account Debit Currency Debit Value Date Total Debit Amount Credit Account Credit Currency Credit Amount Credit Value Date Accounting Date
4. Click the Validate icon to check for overrides and errors.
5. Click the Commit icon to create the record.

| SCREENS | WORKFLOW |
|---|---|
|  | Authorise/Delete PC by DC . |
| Unauthorised Post Closing Adjustment Entries | Click the Authorise icon of a corresponding record. |
| Post Close | Click the Authorise icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Authorise/Delete PC by FT . |
| Unauthorised Post Closing Adjustment Entries | Click the Authorise icon of a corresponding record. |
| Authorise/Delete Funds Transfer | Click the Authorise icon. |

This screen helps the user to configure and perform PC period closing.

To close a period, follow the below steps:

1. Define Closed Period .
2. In the contract screen, enter or select a value in the Open PC Period field.
3. In the Close PC PERIOD screen, enter values in the following fields: Company Comp Status Database Path
4. Click the Validate icon to check for overrides and errors
5. Click the Commit icon to close the PC Period.


#### 📊 Outputs

There are no Outputs available for Post-Closing Process feature.

---


### 1.7  Using the PC Database


> **📇 Quick Reference Card**
> 
> **Purpose:** *Adjustment entries on the PC.PERIOD database are raised through DATA.CAPTURE , FUNDS.TRANSFER , and Generic Accounting Interface (GAI) request.*
> 
> **Applications:** `BATCH.NEW.COMPANY`, `PC.PERIOD`, `PC.UPDATE.REQUEST`
> 
> **Key Fields:** *Accounting Date*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Adjustment entries on the PC.PERIOD database are raised through DATA.CAPTURE , FUNDS.TRANSFER , and Generic Accounting Interface (GAI) request.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

The PC.PERIOD database can be updated either through DATA.CAPTURE , FUNDS.TRANSFER , and Generic Accounting Interface (GAI) request. Both applications contain the Accounting Date field. The system calculates the PC.PERIOD records that are to be triggered based on the date specified in Accounting Date, and adjusts the databases accordingly. The PC.UPDATE.REQUEST application allows users to update the post-closing database with the adjustment transactions raised either for the single or all available companies based on setup.


##### Workflow

This section helps the user to perform the below tasks:

This PC.UPDATE.REQUEST service must be run at the Installation level, and it will process all the lead companies as specified in the PC.UPDATE.REQUEST record. This service will apply all the adjustments to the post-closing database. Please ensure that there is a record in BATCH.NEW.COMPANY and it must be at the INT level.

Please ensure there is a background service only for the master company.

The PC.UPDATE.REQUEST application enables the user to update PC database.

To update PC Database, follow the below steps:

1. Update PC Database
2. In the PC.UPDATE.REQUEST screen, enter values in the required fields.
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon.
5. Ensure that the service ' PC.UPDATE.REQUEST ' is running in the background.

> **⚠️ Note:** It is not recommended to run the service while the close of business is running.


#### 📊 Outputs

There are no Outputs available for Using the PC Database feature.


> **Related Applications:** `BATCH.NEW.COMPANY`, `PC.PERIOD`, `PC.UPDATE.REQUEST`

---


---


## Chapter 2: General_Ledger_Accounting - RE


General_Ledger_Accounting - RE module of Temenos Transact


### Features in General_Ledger_Accounting - RE


| # | Feature | Sections |
|---|---------|----------|
| 2.1 | Accounting System | Intro, Confi, Tasks, Outpu |
| 2.2 | Addition of Local Reference Fields for External Interface | Intro, Confi, Tasks, Outpu |
| 2.3 | Banking Framework Exit Point | Intro, Confi, Tasks, Outpu |
| 2.4 | Company-Specific Grouping Conditions | Intro, Confi, Tasks, Outpu |
| 2.5 | Currency Position | Intro, Confi, Tasks, Outpu |
| 2.6 | Default or Catch All or Unallocated Line | Intro, Confi, Tasks, Outpu |
| 2.7 | Display of Reversal Entries in CRF Report | Intro, Confi, Tasks, Outpu |
| 2.8 | Enforcing Balanced Accounting Entries | Intro, Confi, Tasks, Outpu |
| 2.9 | Extraction of GL Information to Disk | Intro, Confi, Worki, Tasks, Outpu |
| 2.10 | Financial Accounting | Intro, Confi, Tasks, Outpu |
| 2.11 | General Ledger Reports | Intro, Confi, Tasks, Outpu |
| 2.12 | Generating and Recording the Accounting Entries | Intro, Confi, Tasks, Outpu |
| 2.13 | Grouping Conditions for Accounting Entries | Intro, Confi, Tasks, Outpu |
| 2.14 | Maintenance of Line Balance Details | Intro, Confi, Tasks, Outpu |
| 2.15 | Misc | Intro |
| 2.16 | Multi-Company Reporting | Intro, Confi, Tasks, Outpu |
| 2.17 | Multi GAAP | Intro, Confi, Tasks, Outpu |
| 2.18 | Position Accounting | Intro, Confi, Tasks, Outpu |
| 2.19 | Printing Back-Dated Reports from CRB | Intro, Confi, Tasks, Outpu |
| 2.20 | Printing BackDated Reports from CRB | Intro |
| 2.21 | Printing the Report | Intro, Confi, Tasks, Outpu |
| 2.22 | Producing Report in Non-Local Currency | Intro, Confi, Tasks, Outpu |
| 2.23 | Producing Report in NonLocal Currency | Intro |
| 2.24 | Recording the Contract Balances | Intro, Confi, Tasks, Outpu |
| 2.25 | Recreation of CRB | Intro, Confi, Tasks, Outpu |
| 2.26 | Revaluation | Intro, Confi, Tasks, Outpu |
| 2.27 | Soft Accounting | Intro, Confi, Tasks, Outpu |
| 2.28 | Transaction Journal Reporting | Intro, Confi, Tasks, Outpu |
| 2.29 | US GAAP Reporting | Intro, Confi, Tasks, Outpu |
| 2.30 | Utility Files for Report Generation | Intro, Confi, Tasks, Outpu |
| 2.31 | Utility for Consolidation of Accounting Entries | Intro, Confi, Tasks, Outpu |
| 2.32 | Utility for End of Year Procedure PLCLOSEOUT | Intro, Confi, Tasks, Outpu |


### 2.1  Accounting System


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Accounting system or Accounting Base Mode determines the accounting treatment to be followed for cash based transactions for movements with future dates (value date or processing date).*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The Accounting system or Accounting Base Mode determines the accounting treatment to be followed for cash based transactions for movements with future dates (value date or processing date).

This is used to determine when a future dated movement is considered booked for the bank’s reporting purposes.


#### ⚙️ Configuration

The Accounting system (or Accounting Base) can be configured in Temenos Transact in the ACCOUNT.PARAMETER table. The value defined in Value Dtd Acctng field determines the accounting treatment for the transactions.

The following Accounting Systems are supported in Temenos Transact :

- Trade Dated Accounting (TDA)
- Value Dated Accounting (VDA)
- Trade Dated General Ledger Accounting (TDGL)
- Process Dated Accounting (PDA)


#### 📋 Tasks

There are no Tasks available for Accounting System feature.


#### 📊 Outputs

Temenos Transact allows the user to record the accounting entries of each transaction posted in the system. These records can be used for reconciliation of entries and regulatory reporting purposes. The user can view the below list of enquiries and reports pertaining to Recording the Accounting entries in the core banking system.


##### Enquiries and Reports

The user can access the below enquiries and reports:

System Summary

This enquiry generates the accounting entries summary report for the day and displays the General Ledger (GL) difference in local currency.

Unauthorised Entries

This enquiry displays the accounting entries, which are in the unauthorised status.

Transaction Entries-MB

This enquiry displays the accounting entries of the authorised transactions for any account or contract in Temenos Transact .


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


### 2.2  Addition of Local Reference Fields for External Interface


> **📇 Quick Reference Card**
> 
> **Purpose:** *Additional data fields for the use of external systems can be added to the three Temenos Transact accounting entry files.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Additional data fields for the use of external systems can be added to the three Temenos Transact accounting entry files.

A locally customisable program attached are invoked during the core accounting process. The core system allows the user defined fields on accounting entries such as STMT.ENTRY , CATEG.ENTRY and RE.CONSOL.SPEC.ENTRY to be populated. This is achieved through a user exit that allows a locally developed API to determine what values are stored.

Local Reference fields are added in the entry tables to hold the required additional information for each movement. The values returned from the local API are stored in the local reference fields in the entries.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

There are no Tasks available for Addition of Local Reference Fields for External Interface feature.


#### 📊 Outputs

There are no Outputs available for Addition of Local Reference Fields for External Interface feature.

---


### 2.3  Banking Framework Exit Point


> **📇 Quick Reference Card**
> 
> **Purpose:** *Banking Framework Event is a structured component exit point built in the Integration Framework designer to extract the data from the transaction system through Data Event Streaming. It is the currently available exit point, which contains the entry event that exposes the data for a statement entry ...*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Banking Framework Event is a structured component exit point built in the Integration Framework designer to extract the data from the transaction system through Data Event Streaming. It is the currently available exit point, which contains the entry event that exposes the data for a statement entry ( STMT.ENTRY ).

The entry event contains the details of a STMT.ENTRY enriched with the underlying transaction that has triggered the entry.


#### ⚙️ Configuration

This section explains the design time and run time configurations required to enable this functionality.


##### Design Time configuration

The Integration Framework Designer provides the ability to configure a structured component exit point for an entry event with the basic details of a STMT.ENTRY and the enrichment from the underlying transaction.

The following table shows the list of entry events that are available:

| Entry Event | Description | Base Table for Entry Event | Transaction Table Available for Enrichment |
|---|---|---|---|
| ENTRY.DEFAULT | This is the default entry event with all the details from STMT.ENTRY if a specific entry event is not identified. | STMT.ENTRY | - |
| ENTRY.FT | This entry event is triggered if the SYSTEM.ID from the entry is FT. | STMT.ENTRY | FUNDS.TRANSFER |
| ENTRY.AAAA | This entry event is triggered if the SYSTEM.ID from the entry is AAAA. | STMT.ENTRY | AA.ARRANGEMENT.ACTIVITY |
| ENTRY.DX | This entry event is triggered if the SYSTEM.ID from the entry is DX. | STMT.ENTRY | DX.TRADE |
| ENTRY.SCCA | This entry event is triggered if the SYSTEM.ID from the entry is SCCA. | STMT.ENTRY | ENTITLEMENT |
| ENTRY.FX | This entry event is triggered if the SYSTEM.ID from the entry is FX. | STMT.ENTRY | FOREX |
| ENTRY.SCSP | This entry event is triggered if the SYSTEM.ID from the entry is SCSP. | STMT.ENTRY | SEC.TRADE |

The data flow and configuration for each of those entry events are configured in the Integration Framework Designer and is recorded in the IF.INTEGRATION.FLOW.CATALOG table. The entry events are flagged for streaming.

The following screenshots show the creation of a Banking Framework Event for entry event ENTRY.FT in Integration Framework Designer.

1. Choose ‘Banking Framework Event’ in the Exit Point Type field.

1. Choose the event type in Exit Type and the event name in Banking Framework Event .

1. For the event name chosen, select the fields from STMT.ENTRY and the underlying transaction table (in this case FUNDS.TRANSFER ) and select the Streaming Event option in the Flow Attributes , for the data to be streamed to DATA.EVENTS table.

1. After adding the fields, display name and the respective table name will appear in the Flow Enrichments tab.
2. Save the event and flow and publish the event. This will create records in IF.EXIT.POINT S and IF.INTEGRATION.FLOW.CATALOG tables.

The IF. INTEGRATION . FLOW . CATALOG records for the entry events have been deployed with all the fields from the STMT.ENTRY table and corresponding transaction table. The user can modify the content of each entry event with the selected list of system or local fields through the Integration Framework Designer if it is licensed.

The following screenshot shows a sample record for the default entry event in IF.INTEGRATION.FLOW.CATALOG .


##### Run Time configuration

The entry event is triggered near real time outside the transaction boundary from a background accounting service and the HVT (High Volume Transaction) service if the Use Data Events field in AC.STMT.PARAMETER is set as Y, as shown in the following screenshot.


#### 📋 Tasks

There are no Tasks available for Banking Framework Exit Point feature.


#### 📊 Outputs

There are no Outputs available for Banking Framework Exit Point feature.

---


### 2.4  Company-Specific Grouping Conditions


> **📇 Quick Reference Card**
> 
> **Purpose:** *The parameterisation of grouping conditions is system-wide. However if required, company-specific records can be created to vary the default conditions. Company-specific set-up will have a different ID to that of the default set-up. Company specific record will have the company ID suffixed to the re...*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The parameterisation of grouping conditions is system-wide. However if required, company-specific records can be created to vary the default conditions. Company-specific set-up will have a different ID to that of the default set-up. Company specific record will have the company ID suffixed to the record as follows:

- ASSET&LIAB.CCCCCCCCC
- PROFIT&LOSS.CCCCCCCCC

Where, CCCCCCCCC refers to the Company Code.


#### ⚙️ Configuration

This is defined in the ASSET&LIAB and PROFIT&LOSS records in the CONSOLIDATE.COND parameter file.

- After setting up the ASSET&LIAB and PROFIT&LOSS default records in CONSOLIDATE.COND , which serve as Master or Default records, company specific records are set.
- Key parameters defined in default records are re-defined.
- Company-specific Consolidation Parameters have the company code appended to the ID as shown below: ASSET&LIAB.CCCCCCCCC PROFIT&LOSS.CCCCCCCCC

Where, CCCCCCCCC refers to the Company Code and it can be set, if the field Cons Key Co in the COMPANY record is blank or has CCCCCCCCC value.

Any number of companies can share consolidation parameters of one company (say CCCCCCCCC) if the Cons Key Co field in their COMPANY record is set as CCCCCCCCC.

Company-Specific Redefinition of Variable Parameters:

The CONSOLIDATE.COND application defines the variable parameters. The asset and liability base parameters are defined in the record with the ASSET&LIAB key, and the profit and loss base parameters are defined in the record with a PROFIT&LOSS key. These are the default records. It is possible that some of the variable parameters need to be redefined at company level. The company level definitions are stored in the records with the ASSET&LIAB.xxxxxxxxx and PROFIT&LOSS.xxxxxxxxx keys, where xxxxxxxxx is the COMPANY record key.


#### 📋 Tasks

There are no Tasks available for Company-Specific Grouping Conditions feature.


#### 📊 Outputs

There are no Outputs available for Company-Specific Grouping Conditions feature.

---


### 2.5  Currency Position


> **📇 Quick Reference Card**
> 
> **Purpose:** *A currency position is created when a transaction involves two or more currencies. For example, when a customer deposits USD into a GBP account. Here, the bank is ‘buying’ USD and ‘selling’ GBP. This creates a position in USD for the bank. Holding USD gives rise to currency exchange risk in that, wh...*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction


##### Position Management

A currency position is created when a transaction involves two or more currencies. For example, when a customer deposits USD into a GBP account. Here, the bank is ‘buying’ USD and ‘selling’ GBP. This creates a position in USD for the bank. Holding USD gives rise to currency exchange risk in that, when the exchange rate moves, the bank may incur a revaluation gain or loss. This risk is managed by a banks treasury function.

Temenos Transact provides functionality to manage the risk by providing up to date currency positions.


##### Currency Position Management

Maintenance of currency positions is a part of the core accounting functionality and does not need parameterisation.

The POSITION file is updated automatically, only when a transaction in non-local currency impacts position of the particular currency, that is, when a transaction either increases or decreases the position held in a particular currency in the event of a cross currency transaction. If a transaction involves the same foreign currency, that is, debit and credit are in the same foreign currency and in the same amount, position entries will not be raised.

> **⚠️ Note:** There are no real physical accounting entries behind the POSITION file in Temenos Transact .

POSITION file is extensively used by the Forex (FX) module and enquiries are used predominantly by dealers.


#### ⚙️ Configuration

Recording of Currency Positions is an integral part of Temenos Transact and a position is automatically created when a cross currency transaction is recorded. There is no configurability.


#### 📋 Tasks

There are no Tasks available for Currency Position feature.


#### 📊 Outputs

There are no Outputs available for Currency Position feature.

---


### 2.6  Default or Catch All or Unallocated Line


> **📇 Quick Reference Card**
> 
> **Purpose:** *Where a CRF Key fails to meet the mapping criteria set in Report Line RE.STAT.REP.LINE, the system defaults such CRF keys a ‘Catch All’ (sometimes called Unallocated Lines) section of the GL report so that the report balances. User must investigate the reason the CRF key falling into ‘Catch All’. Mo...*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Where a CRF Key fails to meet the mapping criteria set in Report Line RE.STAT.REP.LINE, the system defaults such CRF keys a ‘Catch All’ (sometimes called Unallocated Lines) section of the GL report so that the report balances. User must investigate the reason the CRF key falling into ‘Catch All’. Most likely reason is the creation of a new CRF whose components have not been captured in the RE.STAT.REP.LINE mapping.

There can be multiple CRF keys in ‘Catch All’.


#### ⚙️ Configuration

A ‘Catch All’ Line is created in the same way as any line using RE.STAT.REP.LINE . It can be created at the outset or added later on.

The impact of the creation of new report lines can be seen after COB process.


#### 📋 Tasks

There are no Tasks available for Default or Catch All or Unallocated Line feature.


#### 📊 Outputs

There are no Outputs available for Default or Catch All or Unallocated Line feature.

---


### 2.7  Display of Reversal Entries in CRF Report


> **📇 Quick Reference Card**
> 
> **Purpose:** *The transaction entries reflected in Central Reporting Files (CRF) for Debit/Credit movement depends on the sign of the numeric entry. If the sign of the transaction amount is negative, it is shown as a debit movement. If it is positive, it is shown as a credit movement.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The transaction entries reflected in Central Reporting Files (CRF) for Debit/Credit movement depends on the sign of the numeric entry. If the sign of the transaction amount is negative, it is shown as a debit movement. If it is positive, it is shown as a credit movement.

The settings of the parameter fields Crf Reversal Flag in ACCOUNT.PARAMETER and the Rev Marker for REV record in RE.TXN.CODE gives the functionality to reflect reversal entries in CRF in two different ways. One is to treat the reversal entries like the non-reversals, where the movements are exaggerated in their respective direction of their signs of the transactions involved. This does not set off the movement of the original entry. In the other, unlike the non-reversals, the reversal entry movements are not exaggerated in their respective directions. They not only reflect in the same direction as the original entries, but also nullify the total movement of the whole transaction.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

There are no Tasks available for Display of Reversal Entries in CRF Report feature.


#### 📊 Outputs

There are no Outputs available for Display of Reversal Entries in CRF Report feature.

---


### 2.8  Enforcing Balanced Accounting Entries


> **📇 Quick Reference Card**
> 
> **Purpose:** *To maintain the financial integrity of the system, all applications generate balancing entries. Temenos Transact performs a check if the accounting entries raised by an application balance.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

To maintain the financial integrity of the system, all applications generate balancing entries. Temenos Transact performs a check if the accounting entries raised by an application balance.

The following applications are an exception to this rule, for they can genuinely raise one-sided entries. The system can force the balancing leg if parameterised to do so.

| Application | Description |
|---|---|
| DATA.CAPTURE (DC) | Journaling functionality that can raise one-sided entry. There is a mechanism to stop unbalanced batches already in place. |
| FIDUCIARY (FD) | Can make two separate calls to accounting. |
| REVALUATION.AL | Generates one sided entries during the COB. |


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

There are no Tasks available for Enforcing Balanced Accounting Entries feature.


#### 📊 Outputs

There are no Outputs available for Enforcing Balanced Accounting Entries feature.

---


### 2.9  Extraction of GL Information to Disk


> **📇 Quick Reference Card**
> 
> **Purpose:** *For scenarios where the reports are maintained outside Temenos Transact or if the reports have to be maintained for longer period of time, the information is extracted and maintained in external storage.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

For scenarios where the reports are maintained outside Temenos Transact or if the reports have to be maintained for longer period of time, the information is extracted and maintained in external storage.


#### ⚙️ Configuration

This topic covers the configuration required for the extraction of GL information to disk.


##### RE.EXTRACT.PARAMS

This application is used to set up the details required for creating output file from the RE.RETURN.EXTRACT routine. This file provides the details of the information to be stored in the file created by the RE.RETURN.EXTRACT routine.

The RE.RETURN.EXTRACT routine is used to create a disk output file for any CRF report. The details to be stored in this output file are decided by the parameters set up in the RE.EXTRACT.PARAMS table.

The key to this file is the report name. The output file created by RE.RETURN.EXTRACT stores the components of consolidation key, line narratives and associated amounts. These details are to be specified here for the required report.


#### 🔧 Working With

This topic covers the extraction of GL information to disk.


##### RE.RETURN.EXTRACT

This table is used to load details of the CRF reports that must be extracted to a disk file in the batch run. It provides an additional option, which allows balances and details from the underlying contracts to be generated in the created extract file. This option may be required when producing an extract file based on a CRB report for handoff to a local reporting package.

If the Contract Details field (in RE.EXTRACT.PARAMS ) is set to Yes, the details of the underlying Asset and Liability contracts are generated as separate records. The following fields are appended to the end of the output record:

- ID Sequence Number * Contract / Account Id * Asset Type
- Customer number
- Deal Balance for Asset Type in Deal Currency
- Deal Balance for Asset Type in Local Currency
- Interest Rate (or Exchange Rate in the case of FX deals)
- Value Date
- Maturity Date
- Initial Term in Days
- Remaining Term in Days

> **⚠️ Note:** The records will still be created for each CONSOLIDATE.ASST.LIAB/PRFT.LOSS record as before, with no contract details. These records do not contain any contract reference or asset type in the key.


##### Automatic Build of Dictionary for Extract File

An option to build the dictionary for the CRB extract file is created when the RE.RETURN.EXTRACT application is available. If the field Build Dictionary is set to Yes, a record in STANDARD.SELECTION for the extract file RE.CRF.XXX (where XXX is the report name) is created or amended. Fields are built based on the contents of the associated record in RE.EXTRACT.PARAMS .

Existing user-defined fields in the STANDARD.SELECTION are not amended by the rebuild of the dictionary.


#### 📋 Tasks

There are no Tasks available for Extraction of GL Information to Disk feature.


#### 📊 Outputs

There are no Outputs available for Extraction of GL Information to Disk feature.

---


### 2.10  Financial Accounting


> **📇 Quick Reference Card**
> 
> **Purpose:** *The accounting process is a series of activities that begins with creating accounting entries for each transaction and ends with the closing of the books of accounts. As this process is repeated during each accounting period, it is referred as Accounting Cycle.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The accounting process is a series of activities that begins with creating accounting entries for each transaction and ends with the closing of the books of accounts. As this process is repeated during each accounting period, it is referred as Accounting Cycle.

In Temenos Transact , some of the activities in the Accounting Cycle occur concurrently as well as sequentially.

- After a transaction is authorised in the product module, information is handed over to the accounting processing.
- Accounting entries (sometimes also known as journal entries) are posted to accounts/contracts and the balances of the individual ledger accounts are updated automatically.
- Accounting entries for interest and charge accruals, revaluations and deferred items are raised, posted during Close of Business. These are known as Special ‘Spec’ entries in Temenos Transact .
- Check reports are generated to check the integrity of the GL, verifying the accounting accuracy of transactions processed during the day.
- General Ledger is generated with the balances from the individual ledger accounts.
- There is no core month-end Closure procedure. If required the optional module, Post Closure can be deployed to meet the client’s month-end requirements.
- To facilitate the year end reporting, the year-end procedure must be run. It generates accounting entries to move the Profit and Loss to internal account identified in the year-end configuration parameters. Profit and Loss are zeroed out getting the GL ready for the new year.

Banks verify the accounting accuracy by viewing the financial reports. Based on the transactions processed during the day (online and COB), the balances of the account or contract is updated and the General Ledger (GL) report is generated to ensure that the system is balanced with the assets and liabilities positions.

Temenos Transact uses the Central Reporting Base (CRB), built from the accounting entries and contract balances.

Temenos Transact Transact does not have a predefined set of chart of accounts. The GL Accounts in Temenos Transact are referred to as GL Consolidation Keys. They are formed based on the grouping conditions defined in the CONSOLIDATE.COND table.


#### ⚙️ Configuration

The configuration for accounting is done at the outset when the system is installed and is a combination of interacting settings. It includes:

- Configuring Accounting Period.
- Configuring General Ledger Account Structure. Read Company-Specific Grouping Conditions for more details.
- Configuring Accounting Base Type – Trade Dated (TD), Value Dated (VD), Trade Dated GL (TDGL) or Process Dated Accounting. Read Accounting System for more details.

> **⚠️ Note:** General Ledger has a dependency on the configuration of a number of core systems tables like, Currency, Category, Sector, Industry, Country, Holiday, Account Officer and so on. These are used in the construction of GL accounts. This is covered later in this UG.


##### Configuring the Accounting Period

An accounting period is the span of time covered by a set of financial statements. This period defines the time range over which business transactions are accumulated into financial statements and is needed by investors and lenders so that they can compare the results of successive time periods. An accounting period is one month for internal financial reporting and 12 months for external reporting.

The screenshot below indicates that the year-end closes 31 Dec every 12 months, for GB-001-0001.


#### 📋 Tasks

There are no Tasks available for Financial Accounting feature.


#### 📊 Outputs

There are no Outputs available for Financial Accounting feature.

---


### 2.11  General Ledger Reports


> **📇 Quick Reference Card**
> 
> **Purpose:** *The following diagram is an overview of how low level raw data is converted into meaning full data for reporting purposes. The main source for the GL reports are two files which hold the aggregated CRF keys:*
> 
> **Applications:** `ASSET.TYPE`
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The following diagram is an overview of how low level raw data is converted into meaning full data for reporting purposes. The main source for the GL reports are two files which hold the aggregated CRF keys:

- CONSOLIDATE.ASST.LIAB (CAL)
- CONSOLIDATE.PRFT.LOSS (CPL)

The following diagram shows a conceptual view of data flow:


#### ⚙️ Configuration

A set of tools are used to construct the general ledger report. The Temenos Transact Model Bank comes with template settings that can be modified to suit the client’s needs or a new General Ledger report can be constructed from scratch.

The tool box consists of tools that can be used to produce a variety of reports for internal and external purposes. A GL consists of columns, rows, sub-totals and totals.


##### Layout of the General Ledger Report

This section explains the layout and components of the GL Report.

| REPORT HEADER – For example, General Ledger for ABC Bank as at close of YYYYMMDD |  |  |  |  |
|---|---|---|---|---|
| Reporting Line | COLUMN 1 | COLUMN 2 | COLUMN 3 | COLUMN 4 |
|  | Opening Balance | Debits | Credits | Closing Balance |
| Line 1 |  |  |  |  |
| Line 2 |  |  |  |  |
| Line 3 |  |  |  |  |
| Sub Total |  |  |  |  |
| Line 4 |  |  |  |  |
| Line 5 |  |  |  |  |
| Line 6 |  |  |  |  |
| Sub Total |  |  |  |  |
| GRAND TOTAL |  |  |  |  |


##### Components of the GL Report

There are three main components to the GL report:

- Column – This represents the characteristics of the columns to be printed on the report.
- Header – This represents the region of the report that contains the Title, Date and Time of printing the report and Column names.
- Line – This represents the detailed chart of accounts.

To produce reports, the user can configure columns to be printed, the report headings, the totals to be printed and the details to be printed on a particular line (row).

For GL to balance, the balances have to be in a common currency, which most banks is in the local or base currency. Therefore, such balances will be reported in the local equivalent. The system also has the ability to produce GL in foreign currency if required.

| Content of the Column (#TYPE.1) | Nature of Balance Held(#TYPE.2) | Currency Represented(#TYPE.3) | Column Range(#TYPE.4) |
|---|---|---|---|
| Asset/LiabilityProfit/LossBothPLCMPLYTD | Net Credit Debit | AllLocalForeignCurrencyProfit.Currency*Currency Code | Contains the range of values to be included or excluded by the column based on the set up in RE.STAT.COLUMN.RANGE file. |

Nature of Balance held (#TYPE.2)

- Opening – represents the closing balance of previous day.
- Net – net of debit and credit movements.
- Credit – credit movements only.
- Debit – debit movements only.
- Shutting – closing balance.
- Equivalent Local currency equivalent of closing balance.

> **⚠️ Note:** Other characteristics are not applicable to the ‘Movement’ Group Column because the content of the column includes both AL and PL and the currency of the column is always the Local Currency Equivalent.

This table contains the heading details indicating the columns to be printed, the amount size, report heading, whether reports are by single currency or all currencies and if entries are to be printed. The field in this table include:

- Title of the Report – Defined in Gb Heading field.
- Descriptive Columns – The size and description are defined in Line Narr Size , Gb Narr Hd 1 and Gb Narr Hd 2 fields.
- Financial Columns – Defined in the Column Type field, which links it to the RE.STAT.COLUMN.TYPE file.
- Total and Calc Columns – The Column Type field is used to define columns, which perform a summation or calculation based on any of the financial columns using the operands such as ADD, SUBTRACT, MULTIPLY and DIVIDE.

- In the screenshot shown below, the CALC column performs the calculation of percentage movement, which is:

(Net of closing and opening balance)/ (Opening balance) X 100

Other Features of RE.STAT.REPORT.HEAD :

- This file controls the sections of the report and their print sequence with respect to the currency content using the Split field, which can contain any one of the following values: All - One section containing local and equivalent of foreign currencies. Currency - One section per currency including local currency. Local - One section containing local currency only. By Foreign - One section per currency without local currency. Total Foreign - One section containing the equivalent of foreign currencies only.
- The RE.STAT.REPORT.HEAD file controls the currency in which profit and loss is reported. Though P&L transactions are booked only in local currency, the information pertaining to the original source currency and amount are also maintained in the accounting entry files of Temenos Transact . Hence, reports can be generated based on the local currency or in the original Source Currency, if required.
- It controls the calculation basis of time bands and reporting of deals maturing on the last day of the time band. A value ‘Y’ in the MAT.TO.MONTH.END file indicates that time bands are calculated from the last day of the month and ’NO’ indicates that the time bands are calculated from the last working day of the month. A value ‘Y’ in the Mat Inclusive field indicates that the deals contracts maturing on the last day of the time band are printed in that time band and ’N’ indicates that last date maturity goes to the next time band.
- It controls the amount format of the financial columns of the report.
- It controls the printing of Chart of Accounts with zero value on the report.
- Indicates whether balance movement details of the Chart of Accounts should be maintained at a Summary or Detailed level and the period for which it should be maintained, Using the Maintain Balance and Detail Months fields.
- To produce reports based on multiple reporting rules such as GAAP or IFRS, the RE.STAT.REPORT.HEAD can be configured to select the types that are to be allowed in the Incl Gaap Type field, which links it to the FX.POS.TYPE application.

| Chart of Accounts | Type of Line | Total Accumulator | Total Print |
|---|---|---|---|
| CASH | HEADING |  |  |
| Cash in Hand | DETAIL | 1 |  |
| ATM Cash | DETAIL | 1 |  |
| Traveler’s Cheques | DETAIL | 1 |  |
| TOTAL CASH | TOTAL | 2 | 1 |

A pre-defined range of values can be defined in this file, which is linked to the appropriate grouping element in the RE.STAT.REP.LINE .

Line ranges can be defined:

- For a specific application
- For all applications
- On any parameter included in CONSOLIDATE.COND Any ASSET.TYPE ASSET.CURRENCY PROFIT.CURRENCY

This file creates records containing data for specific lines being identical in several reports.

For example, Cash on hand, Cash with central bank

To use this content in a line, this ID must be picked and entered in the Consol Name field. The system then defaults information.

When modifications for a line are to be effected, RE.STAT.NAME can be modified for the concerned line to effect changes in all reports.

This application contains the details about the presentation of entries, which are to be included in a movement type report.

The Amount field specifies the amount that must be printed from underlying entries and has the following values:

- LCY.CREDIT is the local currency and local currency equivalent credit amount.
- LCY.DEBIT is the local currency and local currency equivalent debit amount.
- LOCAL is the local currency and local currency equivalent of both credit and debit amounts.
- CCY.CREDIT is the foreign currency credit amount.
- CCY.DEBIT is the foreign currency debit amount.
- CURRENCY is the foreign currency amount (includes both credits and debits).

This application contains the narrative to be printed in a specified user language at the top of a report describing how the amounts are shown in the report.

The record ID of RE.AMT.ABBREV is then added to the Amount Unit field in RE.STAT.REPORT.HEAD application.

The reporting module allows the output of details to a sequential disk file in place of the standard printed output. RE.STAT.OUTPUT is used to define the content and layout of this output file.

The output is written to a sequential file under the directory RE.CRF.EXTRACT. It is redirected to disk by specifying the name of a record in RE.STAT.OUTPUT in the Output Mode field in the RE.STAT.REQUEST report request file.

The record in RE.STAT.OUTPUT defines the structure of data extracted from the report in terms of line. The types of report line available for printing or data extraction are:

- HEADING
- DETAIL or LINK in which, the line details and amounts are printed
- CCY that prints out the currency for that line
- TOTAL that are used to print running totals

The Bypass Txn Journal and Bypass Journal Sum fields in ACCOUNT.PARAMETER allow the user to bypass updating the Bypass Txn Jounral and Bypass Journal Summary for high volume sites. The value Yes means the reports are not generated in the COB. If the value No is entered, then the reports are generated during the COB.

The TXN.JOURNAL is a file that is used to produce the TRANSACTION.JOURNAL report, which is the list of all entries for the day by application. If the user decides that the TXN.JOURNAL report is not required to be produced from Temenos Transact after consultation with the banks' auditors, the Bypass Txn Journal field is set to Yes.

EB.JOURNAL.SUMMARY is a file that contains the record for each day, which gives the totals by debits and credits that are passed by each application. The user can decide if this is not required and in which case, this can be switched off using the Bypass Journal Sum field.


#### 📋 Tasks

There are no Tasks available for General Ledger Reports feature.


#### 📊 Outputs

There are no Outputs available for General Ledger Reports feature.


> **Related Applications:** `ASSET.TYPE`

---


### 2.12  Generating and Recording the Accounting Entries


> **📇 Quick Reference Card**
> 
> **Purpose:** *Product modules pass information to the accounting processes which creates accountings entries, updates posts to accounts and updates the accounting entry tables. The system maintains three such tables holding low level accounting entries. These are:*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Product modules pass information to the accounting processes which creates accountings entries, updates posts to accounts and updates the accounting entry tables. The system maintains three such tables holding low level accounting entries. These are:


#### ⚙️ Configuration

There is no specific configuration for this feature. The accounting entries are generated by background processes based on the information passed by the underlying application.


#### 📋 Tasks

There are no Tasks available for Generating and Recording Accounting Entries feature.


#### 📊 Outputs

Temenos Transact allows the user to record the various General Ledger (GL) account balances, which is used for Profit and Loss calculation of the company and reporting purpose. The reporting file holds the balances of the GL accounts related to assets, liabilities, owner’s equity, income and expenses. The user can view the below enquiry and report pertaining to Recording the GL Account Balances in the core banking system.


##### Enquiries and Reports

The user can access the below enquiries and reports:

GL Balance Overview - GL Short

This enquiry displays the summarised General Ledger report and helps the user to identify the differences, if any.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


### 2.13  Grouping Conditions for Accounting Entries


> **📇 Quick Reference Card**
> 
> **Purpose:** *Temenos Transact Transact has a unique, highly flexible functionality to create the accounts for general ledger. Once configured, the system automatically creates a GL account even when a new data element, for Grouping Conditions for Accounting Entries example, a new currency, is added.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Temenos Transact Transact has a unique, highly flexible functionality to create the accounts for general ledger. Once configured, the system automatically creates a GL account even when a new data element, for Grouping Conditions for Accounting Entries example, a new currency, is added.

- Temenos Transact uses the virtual GL (General Ledger) accounts, which are user-definable groupings driven by the reporting requirements.
- The grouping conditions are set up at the outset. It is important the structure is well thought out before the system goes live. Changing the conditions, although technically possible, is not recommended as the history data will not take on new conditions.
- The user must take their existing Chart of Accounts into consideration when selecting grouping conditions. If Chart of Accounts do not exist for a new bank, Temenos Transact Model Bank comes with an example that may be used as a starting point.
- In Temenos Transact , grouping conditions form the basis for the Chart of Accounts which are created dynamically. Temenos Transact holds accounting entries at a very base level from which the data is aggregated into GL Accounts during the end-of day processing.
- These dynamic GL accounts are held in the form of Keys called Consolidated Reporting File Key (or CRF). They are also referred to as Consol Keys. These keys can be used to construct any financial reporting using the RE reporting tools covered in a separate section on reporting.
- Every accounting entry passed will fall under one of the GL accounts based on the grouping condition. The Consol Key field in the entry table represents the GL account to which the accounting entry movement is updated.


#### ⚙️ Configuration

The parameterisation of the conditions is system-wide. CRF key structure is applicable to all companies set up in that instance of Temenos Transact . However if required, company-specific records can be created.

The GL Account grouping conditions are composed of data attributes sourced from:

- Customer related information such as the sector, industry, nationality, residency of a customer.
- Product related information from the products the customer uses such as loan, currency of the loan, term/tenor of the loan.

And it has:

- Balance descriptors, for example, Debit, Credit, Interest accrual, Income, Expense.

The grouping structure is defined in CONSOLIDATE.COND parameter file. It forms the basis on which the low level raw accounting data is aggregated into more meaningful information.

The CONSOLIDATE.COND parameter consists of two records covering the grouping conditions for consolidation of:

- Assets and Liabilities – ASSET&LIAB
- Profit and Loss – PROFIT&LOSS

The parameterisation is system-wide in that the CRF key structure will be applicable to all companies set up in that instance of Temenos Transact . However, company-specific records can be created, if required.


##### Assets & Liabilities’ Grouping Conditions

This is defined in the ASSET&LIAB record in the CONSOLIDATE.COND parameter file. The CRF key can have up to sixteen data elements, four of which are system defined and fixed. The remainder can be user-definable.

Once created, the CRF keys are stored in CONSOLIDATED.ASST.LIAB (CAL). This file is the source of information for the construction of GL.

- Fixed parameters are: Product Application, such as AC, LD, MM, FX. Currency – 99 currency markets can be consolidated further into nine currency markets. Position Type – TR position type currently used. Currency – of accounting entry
- User-definable parameters can be chosen from a single value field in GENERAL or LOCAL files. General file (CUSTOMER) Customer Classification like Industry, Sector, Nationality, Residence Local files (any contract or account file) Product category, Account Manager (DAO), Tenor/Time and so on. Local reference fields allowed

> **⚠️ Note:** Tenor/Time is the original term of a contract. The residual maturity is set up the in the Reporting functionality

The following screenshot shows the ASSET&LIAB record in CONSOLIDATE.COND .

In the above screenshot:

- The Name field refers to the name of the data element.
- The File Name field can be LOCAL or CUSTOMER (General file). The value LOCAL means that the value of the data element is available in different fields in different product modules.

For the data element CATEGORY, the value is available in the

field in the

file for the AC Module,

field in the

file for the MG module and the

field in the

file for the LC module.

- Hence, for data elements having LOCAL as the file name, the reference data is defined in the fields such as Multi Value No , Application , Local File Name and Local Field Name .
- The Multi Value No refers to the multi value number of the Name field, in which the data element is defined and acts as the connector between the data element and respective the reference data fields.


##### Profit & Loss Grouping Conditions

This is defined in the PROFIT&LOSS record in the CONSOLIDATE.COND parameter file. The CRF key can have up to thirteen data elements –one of which is system defined and fixed and the remainder twelve can be user-definable.

Once created, the CRF keys are stored in CONSOLIDATED.PRFT.LOSS (CPL). This file is the source of information for the construction of the PL.

- Fixed parameter is either PL or CP, where: CP is the under value dated accounting for future value dated items. PL is used for all other PL items. With Multi-GAAP reporting, this is set according to the values from the relevant FX.POS.TYPE as mentioned below: Non-contingent entries – The first component of the CPL key is mapped from the Pl Prefix field of the relevant record in FX.POS.TYPE . Contingent entries – The first component of the CPL key is mapped from the Pl Cont Code field of the relevant record in FX.POS.TYPE . Self-balancing entries – The first component of the CPL key is mapped from the Pl Self Bal field of the relevant record in FX.POS.TYPE .
- User definable parameters can be selected from a single value field. General files ( CUSTOMER or CATEG.ENTRY ) Customer Classification like Industry, Sector, Nationality, Residence Local files (any contract / account file) Product category, Tenor, Dealing officer. The choice for Local files are dependent on the Local files used for Assets and Liability consolidation.

The Local key components used for A/L records can be mapped into the P&L record. The user must ensure that the Assets and Liabilities, Profit and Loss keys share same local file components. User must also ensure the following:

- File name is specified as LOCAL.
- Mapping is done for select applications in the Application field. The following are the values allowed in the mentioned field: Local File Name – Only AL allowed. Local field No – Serial number of the variable choice in CONSOLIDATE.COND for AL.

The following screenshot shows the PROFIT&LOSS record in CONSOLIDATE.COND .


##### Asset Types or Balance Types

In addition to the fixed and variable attributes of CRF key, the system attaches another attribute that describes the nature of the balance, for example, an account with a deposit balance would have Credit at the end of the CAL key. Asset Types are hard coded whereas Balance Types are soft coded and predominantly used in the Arrangement Architecture. Balance Types are covered in the section on Soft Accounting section of the user guide.

These types define the nature of the balance. For example, whether the balance is Debit, Credit, Debit Accrual, Credit Accrual and so on. Each module will have its own Asset Types which are hard coded for the non-AA modules. Modules may share these. For example, a loan recorded on LD module and the one on Mortgage module will share the same Asset Types; the differentiating factor will the module ID at the beginning of the key and the product code.


#### 📋 Tasks

There are no Tasks available for Grouping Conditions for Accounting Entries feature.


#### 📊 Outputs

There are no Outputs available for Grouping Conditions for Accounting Entries feature.

---


### 2.14  Maintenance of Line Balance Details


> **📇 Quick Reference Card**
> 
> **Purpose:** *Line information is retained in the form of Summary (with only KEY level information) or in Detail (along with account or contract level information). Line Balance field can be set as Null, Summary (or) Detail, NULL option does not retain Line information.*
> 
> **Key Fields:** *Asset*, *Asset Type*, *PL Applic ID*, *PL Category*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Line information is retained in the form of Summary (with only KEY level information) or in Detail (along with account or contract level information). Line Balance field can be set as Null, Summary (or) Detail, NULL option does not retain Line information.

This is used in cases where the user needs to maintain information only on selective lines of a report. If users need to maintain information on all the lines of a report, it can be done at Report Head level.

The information is maintained in the RE.STAT.LINE.BAL and RE.STAT.LINE.MVMT files. These files can be used to generate the sub-ledger information and other useful reports based on the GL accounts.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

There are no Tasks available for Maintenance of Line Balance feature.


#### 📊 Outputs

Temenos Transact allows the user to map the set of accounts or contracts to specific General Ledger (GL) lines and set the Line Balance as Null, Summary or Detail. Selecting the NULL option does not retain Line information. These files can be used to generate the sub-ledger information and other useful reports based on the GL accounts.


##### Enquiries and Reports

The navigation and uses of each enquiry is given in the drop-downs:

GL Line Mapping

This enquiry displays the details about mapping of the General ledger lines. This enquiry fetches the data from RE.STAT.REP.LINE table. GL Line mapping is performed based on the Asset and Asset Type for the respective GL lines given.

PL Line Mapping

This enquiry displays the details about mapping of the Profit & Loss (PL) report lines. PL line mapping is performed based on the PL Applic ID and PL Category for the respective GL line given.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


### 2.15  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *A general ledger (GL) is a set of numbered accounts a business uses to keep track of its financial transactions and to prepare financial reports. Each account is a unique record summarising each type of asset, liability, equity, revenue and expense.*
> 
> **Applications:** `ARCHIVE`, `CATEG.ENTRY`, `MS.PARAMETER`, `RE.CONSOL.SPEC.ENTRY`, `STMT.ENTRY`
> 
> **Key Fields:** *Arc Filename*, *Archive Data*, *Emit Business Event*, *Retention Period*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- APIs
- Temenos Transact Services

A general ledger (GL) is a set of numbered accounts a business uses to keep track of its financial transactions and to prepare financial reports. Each account is a unique record summarising each type of asset, liability, equity, revenue and expense.

It is a central repository for accounting data transferred from all sub-ledgers. GL is usually divided into at least seven main categories. These categories generally include assets, liabilities, owner's equity, revenue, expenses, gains and losses. For banks, the sub ledgers could be loans, deposits, current and Nostro accounts, interest and charges payable or receivable, provisions, fixed assets, depreciation and income and expenses.

An organization's statement of financial position and the statement of income are both derived from the general ledger.

The posting to the accounts occur in general ledger. Posting is the process of recording amounts as credits and debits.

A chart of accounts is a listing of the names of the accounts that a company has identified and made available for recording transactions in its general ledger. A company has the flexibility to tailor its chart of accounts to best suit its needs, including adding accounts as needed.

Within the chart of accounts you will find that the accounts are typically listed in the following order:

The extraction of account balances from the GL is called a trial balance. The purpose of the trial balance is a preliminary stage of the financial statement preparation process, to ensure the equality of the total debits and credits.

At the heart of accounting is the system known as double entry bookkeeping. Because each bookkeeping entry debits one account and credits another account in an equal amount, the double-entry bookkeeping system helps ensure that the general ledger is always in balance, thus maintaining the accounting equation:

This user guide is laid out in three sections covering Financial Accounting, Financial Reporting and Utility Tools in Temenos Transact Transact.


##### Financial Accounting and Financial Reporting

Financial Accounting is a specialised branch of accounting that keeps track of a company's financial transactions. Using standardised guidelines, the transactions are recorded, summarised, and presented in a Financial Report or financial statement such as an income statement or a balance sheet. The aggregation of low level data into GL Accounts as described in Financial Accounting forms the basis of financial reporting including the Balance Sheet and the Income Statement (Profit and Loss).

The following diagram shows the conceptual view of accounting and reporting in Temenos Transact Transact.

Compliance is more of a reporting function. If the row data is available, a compliance reporting tool can be deployed in Temenos Transact and use Temenos Transact ’s offerings or data can be exported to an external system. Both these are available for users. Temenos Transact complies with the specific accounting policies and procedures required by International Financial Reporting Standards (IFRS) for the generation of raw data. It also supports reporting based on local or other GAAPs (Generally Accepted Accounting Principles), which are the standards set by a country’s regulator or accounting standards body. This is termed as Multi-GAAP.

The functionality is covered in detail in this user guide under the section on Multi GAAP including IAS and US local GAAP.

For the month end closing, Temenos Transact has an optional Post Closure (PC) module.

Please refer to section End of Year Procedure – PL.CLOSE.OUT


###### Utility Tools

The system provides a number of utility tools that can be deployed for specific tasks.


##### GL Feature Grouping

Financial Accounting

Financial Accounting Accounting System Generating and Recording Accounting Entries Addition of Local Reference Fields for External Interface Grouping Conditions for Accounting Entries Company-Specific Grouping Conditions Recording the Contract Balances Enforcing Balanced Accounting Entries Currency Position Position Accounting Revaluation Soft Accounting Banking Framework Exit Point Financial Reporting General Ledger Reports Multi-company Reporting Multi GAAP US GAAP Reporting Utility Files for Report Generation Printing Back-Dated Reports from CRB Producing Report in Non-Local Currency Maintenance of Line Balance Details Default or Catch All or Unallocated Line Printing the Report Display of Reversal Entries in CRF Report Recreation of CRB Transaction Journal Reporting Utility Tools Utility for End of Year Procedure – PL.CLOSE.OUT Utility for Consolidation of Accounting Entries Extraction of GL Information to Disk


##### Business Events

When the Emit Business Event field in MS.PARAMETER is set as ‘Yes’, the business events representing the state change are emitted.

The following business events are emitted for Financial Accounting related tables.

| Business Event | Description |
|---|---|
| financialAccounting.UpdateAccountingJournalEntries.AccountingJournalEntriesUpdated | The accounting event is generated when the Transact accounting process authorises a transaction. The generated accounting event contains the details of the generated accounting entries, along with account and contract static information, account balances extracted from the Contract Balance record, the booking and value -dated account balances from the Account Balance Activity record. |
| financialAccounting.UpdateContractBalances.ContractBalancesUpdated | The balance update event is generated when the Contract Balance record is updated by other process other than the accounting process. The generated balance update event contains account and contract static information, and the account balances. |

Refer Temenos Event Explorer for more information on Event catalogue.


##### Archival of Accounting Entries

The user can archive the accounting entries in STMT.ENTRY , CATEG.ENTRY , RE.CONSOL.SPEC.ENTRY , and the related netted entries using the Transact Standard or Data Lifecycle Management (DLM) archival.

The DL module must be installed for the user to initiate the archival service to archive the closed account and the related data records to a Read-only (RO) database. Otherwise, the user moves the data records to the $ARC file using the Standard archival method. The Retention Period is defined in ARCHIVE application for the respective accounting entry table. When the processing date of the accounting entry crosses the retention period, it is selected for archival. Retention Period is calculated from the processing date of the respective accounting entry.

Sample screenshots of ARCHIVE for the accounting entry tables are shown below.

- STMT.ENTRY.DETAIL
- CATEG.ENTRY
- SPECIAL.ENTRY

When Retention Period ends and the user runs the archival service, the files mentioned in Arc Filename are archived.

> **⚠️ Note:** The user must set Archive Data as Y to archive the record. If the user sets it as N, the record is deleted instead of archiving, which results in loss of data.

Read Archiving for more details regarding Transact Standard archival process. Read Data Life Cycle Management for more details regarding DLM Archiving process.


##### Illustrating Model Parameters

This section covers the high-level parameterization of Financial Reporting module, which controls the update of Central Reporting Base with the data passed from different Temenos Transact applications and the production of the reports.

Consolidation Parameters:

| S.No. | Parameters | Description |
|---|---|---|
| 1. | CONSOLIDATE.COND | This application allows the user to define the parameter setup to consolidate data under two categories – Asset and Liability, Profit and Loss. The Asset and Liability consolidation file key is made up of four mandatory parameters – Application, Currency market, Position Type and Currency. The Profit and Loss consolidation file key is made up of one mandatory parameter, that is, Forex position type. |

Report Generation Parameters:

| S.No. | Parameters | Description |
|---|---|---|
| 1. | RE.STAT.COLUMN.TYPE | This application allows the user to define the details for each column to be printed. These details indicate if the balance amount or movement amount must be printed for local currencies, foreign currencies or for all currencies. |
| 2. | RE.STAT.REPORT.HEAD | This application allows the user to define the heading details indicating the column to be printed, amount size, reports for currencies, report heading and if entries have to be printed. |
| 3. | RE.STAT.REP.LINE | This application allows the user to define the details containing the different line and line of contents. It also contains details about totaling, spacing of the lines, and types of Central Reporting Base records to be printed. |
| 4. | RE.STAT.ENT.FORMAT | This application allows the user to define the file containing details about the presentation and format of entries to be included in a report. Titles, headers and columns are described and special masks can be specified. |
| 5. | RE.STAT.RANGE | This application allows the user to define a record containing a range of values or a set of individual values for a report line content definition. User can also set up a ‘standard’, often used for virtual views as a help or short cut in the report line definition process. |
| 6. | RE.STAT.NAME | This application allows the user to group different consolidation conditions under a common mnemonic name. The purpose is to provide a shortcut for definition of reporting line contents, which are repetitive within one or among several reports. |
| 7. | RE.AMT.ABBREV | This application allows the user to define the file that holds the descriptions for amount format displays to be printed in a specified user language at the top of a report. |
| 8. | RE.STAT.OUTPUT | This application allows the user to define the content and layout of this output file. The user can generate output to a sequential disk file or in the standard printed output. |


> **Related Applications:** `ARCHIVE`, `CATEG.ENTRY`, `MS.PARAMETER`, `RE.CONSOL.SPEC.ENTRY`, `STMT.ENTRY`

---


### 2.16  Multi-Company Reporting


> **📇 Quick Reference Card**
> 
> **Purpose:** *In a multi-company set up, the system will be configured to produce general ledger for each company. These companies can be consolidated to produce general ledger for the group, provided that the companies are part of the group and on the same instance of Temenos Transact .*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

In a multi-company set up, the system will be configured to produce general ledger for each company. These companies can be consolidated to produce general ledger for the group, provided that the companies are part of the group and on the same instance of Temenos Transact .


#### ⚙️ Configuration

RE.CONSOL.COMPANY functionality is used to consolidate GLs of multi companies. The consolidation tool has the flexibility to consolidate existing business units ( Temenos Transact companies) into an existing company or create a separate company solely for financial reporting purposes.

A bank as 3 business units X, Y and Z all set up as companies in Temenos Transact . Y and Z can be consolidated into X. It can also create a reporting company W into which it can consolidate X, Y and Z.


#### 📋 Tasks

There are no Tasks available for Multi-Company Reporting feature.


#### 📊 Outputs

There are no Outputs available for Multi-Company Reporting feature.

---


### 2.17  Multi GAAP


> **📇 Quick Reference Card**
> 
> **Purpose:** *Temenos Transact complies with the specific accounting policies and procedures required by International Financial Reporting Standards (IFRS). It also supports reporting based on local or other GAAPs (Generally Accepted Accounting Principles) which are the standards set by a country’s regulator or a...*
> 
> **Key Fields:** *Ccymkt Postype*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Temenos Transact complies with the specific accounting policies and procedures required by International Financial Reporting Standards (IFRS). It also supports reporting based on local or other GAAPs (Generally Accepted Accounting Principles) which are the standards set by a country’s regulator or accounting standards body. This is termed as Multi-GAAP.

The functionality aims at having a common base for all the entries generated by the system according to the different GAAPs. The entries can be fetched from the common base maintained whenever required for the purpose of reporting, which can be displayed or suppressed as per the requirement of a report.

A bank collects a charge while disbursing a loan to a customer. As per the local GAAP of the country, this charge must be charged to the revenue when the loan is disbursed. However, if the bank has to follow the reporting as per the IFRS standards, the charge collected needs to be amortised over the term of the contract. In this case, the bank has to prepare the financial statements following the local GAAP of the country according to the IFRS standards.

There are two solutions to Multi-GAAP within Temenos Transact :

- A manual process, where entries are entered into the system using the FUNDS.TRANSFER and DATA.CAPTURE applications.
- System generated entries, using API routines to calculate positions for IAS GAAP. This is detailed under the IAS GAAP feature.


#### ⚙️ Configuration

The following set-up is required regardless of whether manual or system generated entries are required.


##### FX POSITION TYPE

The FX.POS.TYPE application is used to split the position and accounting of the bank into logical divisions. In particular, the usage of this application is mandatory when using GAAP or IFRS financial reporting. Although prefixed by FX, the table is commonly used in Temenos Transact and is referred to by CATEGORY, ACCOUNT and many accounting or position parameter applications.

When used for GAAP reporting, it is recommended that the two-digit ID is set to the same ID used by the country (that is, IN for India, GB for the UK, CH for Switzerland and so on). The TR record is the original and default record used by Temenos Transact and must be available. The IF record is used for IFRS reporting and must be available if IFRS reporting is required.

In common usage, the ID of the table is used but for contingent and self-balancing an extended id identifier is needed. It is recommended that the following style of values is followed:

- For PL, prefix the position type with PL (for example, PLIF).
- For Contingent P/L, prefix the position type with CP (for example, CPIF).
- For self-balancing P/L, prefix the position type with CB (for example, CBIF).

The user can define their own values of up to four digits for each of these.

> **⚠️ Note:** The RE.PL.PREFIXES system control table stores a cross-reference of all the prefixes that prevents the duplication of any user or system defined values.


##### CATEGORY

For each FX.POS.TYPE , category codes must be set up, which are used by the DC.PARAMETER and PL.CLOSE.OUT applications. The Position Type field in CATEGORY determines which GAAP the category belongs to. If left blank, the system automatically defaults to TR, and once the value is set, this field cannot be changed.

To populate the Position Type field, the Category code must be in the 10000 – 19999 range, to create internal accounts.

If an internal account already exists for the Category, the system does not allow the Position Type field to be amended.


##### PL.CLOSE.PARAMETER

In the PL.CLOSE.PARAMETER , the following multi-value set provides the functionality to define categories to be used for the year-end close out process for each FX.POS.TYPE .

- Position Type
- Close Category

In the following example, these fields have been multi-valued so that both TR and IN FX.POS.TYPE are included.


##### REVALUATION.PARAMETER

If revaluation entries are required for different FX.POS.TYPE entries, the REVALUATION.PARAMETER must be updated with a new multi-value set. The Applic Id field must contain the value AL.XX, where XX is FX.POS.TYPE . In this example, the IN FX.POS.TYPE has been added. The required CATEGORY and TRANSACTION codes need to be set up prior to this.


##### EB.POSITION.PARAMETER

If position accounting entries are required for different FX.POS.TYPE entries, the Ccymkt Postype field in the EB.POSITION.PARAMETER must be updated with the required category for the specific position type. The 'Postype' in Ccymkt Postype must be a valid FX.POS.TYPE . This is used to form position accounts based on the currency market and position types populated in the currency position entries.


##### Internal Accounts

New internal accounts must be opened for the Categories created for the different FX.POS.TYPE s. The category range should be between 10000 and 19999. If internal accounts are opened in the system, the Position Type field is defaulted to TR.

In this example, an internal account is created for the IN FX.POS.TYPE . This account is used to raise suspense entries created by the system during the COB.


#### 📋 Tasks

There are no Tasks available for Multi-GAAP feature.


#### 📊 Outputs

There are no Outputs available for Multi-GAAP feature.

---


### 2.18  Position Accounting


> **📇 Quick Reference Card**
> 
> **Purpose:** *Temenos Transact offers a parameterisable functionality when banks require real physical accounting entries or balance sheet. Position accounting runs in parallel with Position Maintenance above.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Temenos Transact offers a parameterisable functionality when banks require real physical accounting entries or balance sheet. Position accounting runs in parallel with Position Maintenance above.

Unlike Position Maintenance, Position Accounting is optional. Each currency position account will have a corresponding account in local currency.


#### ⚙️ Configuration

Position Accounting is triggered when the Position Entry field in the ASSET&LIAB record of parameter table CONSOLIDATE.COND is set to Account as shown in the screenshot below. The configuration can be done at any time (need not be set at the outset of setting the system). Before the functionality becomes live, it is necessary to exit the system. The functionality becomes active after the user signs in.


##### ConfiguringEB.POSITION.PARAMETER

The key to this record is the Company Id. In a multi-book environment, it is necessary to create a separate record for each lead company in existence.

Position Account categories are defined for:

- AL – (Non contingent)
- ALFWD – (Contingent)
- FXSP – (Contingent)
- FXFW – (Contingent)

The category codes created for ALFWD, FXSP and FXFWD need to be made contingent. This is done by entering the category codes in the ACCOUNT.PARAMETER record, as shown in the following screenshot:

The Ent Type field in the EB.POSITION.PARAMETER application allows accrual transactions to be posted to a different Dealer Desk for position accounts. Thus, the user can enter ACC, which is an overall request and then enter ACC-MM, which means that for MM, the user wants to do something different. The field is used in conjunction with the Change Dd and Dealer Desk fields. In this example, EB.POSITION.PARAMETER has been created with a different Dealer Desk to be used for MM (Money Market) transactions.

The Jour Print Exc Rvn field in EB.POSITION.PARAMETER is set to Yes, if the revaluation entries (that is, the RV section of the report) are to be excluded from being printed in the TXN.JOURNAL report.

An internal account is created for each of the new category codes configured for position accounting. The currency of the account must be the same as the first currency in the ID.

In an internal account USDCHF1055100010001, the currency must be USD. The system then uses this as a template to open further accounts whenever required. When opening the first position account for a currency, the DDSS part of the account number must be entered as 00, where 00 is for Dealer Desk followed by sequence 01 as above, USDCHF1055100010001, example account record. Sub accounts can be used and the maximum number of sub accounts allowed for a position account is 98, meaning that a sequence number can have the values 01 to 99 with 01 being the master or main account and 02 to 99 are the sub accounts.

With positions maintained through position accounts, statements can be produced on any frequency required by the user. These movements are available as of any date or within any date range with an opening and closing balance.


#### 📋 Tasks

There are no Tasks available for Position Accounting feature.


#### 📊 Outputs

There are no Outputs available for Position Accounting feature.

---


### 2.19  Printing Back-Dated Reports from CRB


> **📇 Quick Reference Card**
> 
> **Purpose:** *The CRB module allows the user to maintain historic information so that it is possible to print reports for a past date. This feature is optional and can be switched on when required.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The CRB module allows the user to maintain historic information so that it is possible to print reports for a past date. This feature is optional and can be switched on when required.


#### ⚙️ Configuration

The following actions must be performed to switch on the feature:

- RE.STAT.REPORT.HEAD – The Maintain Balance field can be set either to Summary or Detail in order to allow the system to build balance level information (or) balance and underlying movement level information respectively. This field is relevant to the entire report.
- RE.STAT.REP.LINE – The Line Balance field can be set either to Summary or Detail in order to allow the system to build balance level information (or) balance and underlying movement level information respectively. This field is relevant only to the particular line in a report.

To refer the CRB report lines easily, a mnemonic is added to the record in RE.STAT.REP.LINE .

An optional mnemonic field is added to CATEGORY, which can be used to refer a P&L code in Funds Transfer, Data Capture and Teller applications.

To allow enrichment of CRB transaction codes, the RE.TXN.CODE file allows CRB transaction codes to be defined together with a description. These codes are recorded solely for information purposes and cannot be used as transaction codes in applications.


#### 📋 Tasks

There are no Tasks available for Printing Back-Dated Reports from CRB feature.


#### 📊 Outputs

There are no Outputs available for Printing Back-Dated Reports from CRB feature.

---


### 2.20  Printing BackDated Reports from CRB


> **📇 Quick Reference Card**
> 
> **Purpose:** *The CRB module allows the user to maintain historic information so that it is possible to print reports for a past date. This feature is optional and can be switched on when required.*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

The CRB module allows the user to maintain historic information so that it is possible to print reports for a past date. This feature is optional and can be switched on when required.

---


### 2.21  Printing the Report


> **📇 Quick Reference Card**
> 
> **Purpose:** *The reports can be printed online or during the COB process.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The reports can be printed online or during the COB process.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

There are no Tasks available for Printing the Report feature.


#### 📊 Outputs

Temenos Transact allows the user to print the report either online or during Close of Business (COB) process. Reports can be printed using the below mentioned enquiries.


##### Enquiries and Reports

The navigation and uses of each enquiry is given in the drop-downs:

End of Day Errors

This enquiry displays the error reports during End of Day processing.

General Exceptions

This enquiry allows to generate the report of unauthorised entries for a particular company and date.

Key Balance Sheet Reports

General Ledger report displays the closing balances of all customer accounts, internal accounts and contracts held by the bank as on a particular day.

PL Reports

This enquiry displays the details of Income and Expense of the bank during a specific period. It is a movement type report i.e. the report contains the opening balance, debit movement, credit movement and closing balances.

This tab consits of the following sub-tabs:

Country

This enquiry displays the general ledger report of limit country and it fetches the exception entries generated for the given country.

Currency

This enquiry displays the general ledger report of limit currency and it fetches the exception entries generated for the given currency.

Product

This enquiry displays the general ledger report of limit commodity or product and it fetches the exception entries generated for the given commodity.

General Errors

This enquiry displays the general errors in Limit report. This report contains the date and time of report generation, company and report name, hold Id and Batch status.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


### 2.22  Producing Report in Non-Local Currency


> **📇 Quick Reference Card**
> 
> **Purpose:** *Users can produce CRB/CRF reports in a currency other than the local currency.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Users can produce CRB/CRF reports in a currency other than the local currency.


#### ⚙️ Configuration

This topic covers the application required to produce CRB/CRF reports in a non-local currency.


##### RE.BASE.CCY.PARAM

This file contains the information required to produce CRB/CRF reports in a currency other than the local currency.

To convert a report, key of this record must be entered in the Base Ccy Param field of the appropriate record in the RE.STAT.REQUEST file.


#### 📋 Tasks

There are no Tasks available for Producing Report in Non-Local Currency feature.


#### 📊 Outputs

There are no Outputs available for Producing Report in Non-Local Currency feature.

---


### 2.23  Producing Report in NonLocal Currency


> **📇 Quick Reference Card**
> 
> **Purpose:** *Users can produce CRB/CRF reports in a currency other than the local currency.*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Users can produce CRB/CRF reports in a currency other than the local currency.

---


### 2.24  Recording the Contract Balances


> **📇 Quick Reference Card**
> 
> **Purpose:** *EB.CONTRACT.BALANCES maintains the account or contract balance. It is updated with the opening balance at the start of day and the corresponding accounting movements to the balance types.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

EB.CONTRACT.BALANCES maintains the account or contract balance. It is updated with the opening balance at the start of day and the corresponding accounting movements to the balance types.

It is possible to extract current balance and the balance at the close of the last working day. Balances are updated real-time at the authorisation stage of a transaction.

For certain balance types, unauthorized movements are held too. The data in the record is cycled, as the record is updated on a daily basis to avoid potentially time consuming COB processing. The balances are updated from the core accounting processing based on the accounting entries raised by the underlying application (there is no direct update from the underlying application). This ensures that the balance is always a true reflection of the accounting entries raised by the application.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

There are no Tasks available for Recording the Contract Balances feature


#### 📊 Outputs

In Temenos Transact , EB.CONTRACT.BALANCES application maintains the account or contract balance. It is updated with the opening balance at the start of the day and the corresponding accounting movements to the balance types. Balances are grouped based on the nature or type of the asset and liability. The user can view the below enquiry and report pertaining to Recording the Contract Balances in the core banking system.


##### Enquiries and Reports

The user can view the below enquiry and report pertains to Recording the Contract Balances in the core banking system.

Contract wise balances

The system records the accounting entries made in Temenos Transact for balancing of debits and credits. This enquiry displays the contract wise balances for all the accounts and contracts in Temenos Transact .


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


### 2.25  Recreation of CRB


> **📇 Quick Reference Card**
> 
> **Purpose:** *For any application (module), it is possible to recreate the Central Reporting Base (CRB). Options available are:*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

For any application (module), it is possible to recreate the Central Reporting Base (CRB). Options available are:

- Specific application
- Assets and Liabilities
- Profit and Loss
- Asset and Liability as well as Profit and Loss.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

There are no Tasks available for Recreation of CRB feature.


#### 📊 Outputs

There are no Outputs available for Recreation of CRB feature.

---


### 2.26  Revaluation


> **📇 Quick Reference Card**
> 
> **Purpose:** *At the end of COB that is run prior to report production, all non-contingent foreign currency records are re-valued. That is, all details except those that refer to forward loans and deposits and those referring to any foreign exchange deal.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

At the end of COB that is run prior to report production, all non-contingent foreign currency records are re-valued. That is, all details except those that refer to forward loans and deposits and those referring to any foreign exchange deal.


#### ⚙️ Configuration

This is covered as part of FX module configuration in the REVALUATION.PARAMETER parameter file. No specific configuration is required in the accounting and reporting which accepts data from the underlying module.


#### 📋 Tasks

There are no Tasks available for Revaluation feature.


#### 📊 Outputs

At the end of Close of Business (COB) process, all non-contingent foreign currency records are re-valued before the report generation. It involves revaluing each currency record by type.


##### Enquiries and Reports

The user can access the below enquiries and reports:

AL Revaluation

This enquiry displays the revaluation of the Asset and Liability Currency Position report generated in COB for the day.

The user can access the below FX Revaluation related enquiries and reports:

FX Reval Summary

This enquiry displays the summary report on revaluation of the FX contracts generated during COB for the day.

FX Reval Detail

This enquiry displays the detailed position revaluation report generated during COB for the day.

FX Reval NPV

This enquiry displays the detailed revaluation report (at net present value) generated during COB for the day.

FX Reval NPV Deals

This enquiry displays the deal wise net revaluation report (at net present value) generated during COB for the day.

The user can access the below Swap Revaluation related enquiries and reports:

Swap CCY Reval

This enquiry displays the summary report on revaluation of the FX contracts produced in COB.

Swap NPV Reval

This enquiry displays the COB report, which prints NPV revaluation on swap contracts by currency.

The user can access the below FRA Revaluation related enquiries and reports:

FRA Hedge Reval

This enquiry displays the COB report, which prints the revaluation on FRA Hedge Contracts.

FRA Trade Reval

This enquiry displays the COB report, which prints the revaluation on FRA Trade Contracts.

Trading Position Revaluation

This enquiry displays the trading position revaluation report, which is generated during COB for the day.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


### 2.27  Soft Accounting


> **📇 Quick Reference Card**
> 
> **Purpose:** *With the advent of Arrangement Architecture (AA), Temenos Transact introduced soft accounting. Prior to AA, Asset Types (Balance Types) were hard-coded, which is still used by non-AA modules.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

With the advent of Arrangement Architecture (AA), Temenos Transact introduced soft accounting. Prior to AA, Asset Types (Balance Types) were hard-coded, which is still used by non-AA modules.

Soft Accounting introduced rules based accounting and is extensively used by the Arrangement Architecture modules. The arrangements are comprised of a series of balances that can be defined by product type. As a result, the accounting process is extremely flexible to reflect the rules of the underlying products. Balance types represent the financial components of a product, where the definition of the product specifies which balance types the product should be comprised of.


#### ⚙️ Configuration

This section explains the configuration of Soft Accounting.


##### Configuring Balance Types

Traditionally, balance types have been hard coded within Temenos Transact . The AC.BALANCE.TYPE application enables the user to create additional balance types, and to define the relevant characteristics of the balance types.

Some of these characteristics include the ability to:

- Decompose balance types.
- Post or to suppress entries for internal balance types.
- Post to internal balance types.

In the Reporting Type field, balance types can be defined as types to be reported or as types that are not used for reporting.

- Types to be reported CONTINGENT NON-CONTINGENT
- Types that are not used for reporting INTERNAL VIRTUAL

> **⚠️ Note:** Existing hard-coded balance types used by the system cannot be changed using this application.

The following screenshot shows the CURACCOUNT record in AC.BALANCE.TYPE , where the Reporting Type is Non-contingent and Entry Type is STMT (for STMT.ENTRY ).

The Activity Update field is used to determine whether any updates are made to other dated tables. For example, ACCT.ACTIVITY must be updated for this balance type.

For specific balance types, the Ifp Balance field in AC.BALANCE.TYPE allows the system to consider an off-balance sheet (reporting) amount in addition to a base balance in the Credit Check process (Cover Control). This amount (memo balance) is calculated if the SHADOW component (optional balance component) is attached to a record in AC.CREDIT.CHECK . For the system to consider the memo balance in the Cover Control process of an arrangement account, this amount needs to be updated by a business application.


#### 📋 Tasks

There are no Tasks available for Soft Accounting feature.


#### 📊 Outputs

There are no Outputs available for Soft Accounting feature.

---


### 2.28  Transaction Journal Reporting


> **📇 Quick Reference Card**
> 
> **Purpose:** *Temenos Transact produces transactional reports grouped by the current working day and application. The transactional reports display the total debits and credits by application. The total debits per application should equal the total credits, which is displayed as a net total. The final totals for ...*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Temenos Transact produces transactional reports grouped by the current working day and application. The transactional reports display the total debits and credits by application. The total debits per application should equal the total credits, which is displayed as a net total. The final totals for the day are also displayed.


#### ⚙️ Configuration

Entries applicable to the current working day are those that are actually booked to the CRF (Central reporting files - CONSOLIDATE.ASST.LIAB and CONSOLIDATE.PRFT.LOSS ). In a value date system, forward entries are booked on the current bank date but does not impact the CRF until the value date, so they do not appear in the reports until the value date. The Process Date field on the entry indicates the date on which the entries become active.

If the reports are in balance, then the total debits for all applications should equal the total credits. The reports are produced for each independent financial entity, or company, which could be a lead company or a branch.

The individual entries are stored in the following tables:

- STMT.ENTRY – Updates to accounts
- CATEG.ENTRY – Updates to profit and loss
- RE.CONSOL.SPEC.ENTRY – Updates to CONSOLIDATE.ASST.LIAB

The following tables contain a list of the current bank date entries and are used for various reports:

- ACCT.ENT.LWORK.DAY
- CATEG.ENT.LWORK.DAY
- SPEC.ENT.LWORK.DAY

If the bank has setup Multi-GAAP reporting, a report is generated for each Position Type used.


#### 📋 Tasks

Temenos Transact produces transactional reports grouped by the current working day and application. The transactional reports display the total debits and credits by application. The total debits per application should equal the total credits, which is displayed as a net total. The final total for the day is also displayed.


##### Workflow

This section allows the user to perform the below activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Catch All Details . |
| Catch All Items | Click the Line Input icon to capture or amend the report line of catch all items. |
| Report Line | Enter values in the required fields. Click the Validate icon to check for errors and overrides. Click the Commit icon to create the record. |


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to Transaction Journal Reporting in the core banking system.


##### Enquiries and Reports

This section allows the user to view the below enquiries and reports:

Balancing Account Statement

This enquiry allows the finance user to view the Account statement of the Balancing account for both IF and TR (Trading) positions. Users can drilldown to view the statement entries raised today and entries as per the last statement date.

EOD Balancing Entries Details

The enquiry allows the finance user to view all the balancing entries raised by the system during the Close of Business (COB).


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


### 2.29  US GAAP Reporting


> **📇 Quick Reference Card**
> 
> **Purpose:** *To support the US GAAP (Generally Accepted Accounting Practices) reporting in Country Model Bank, some of the Temenos Transact core applications provide the data to meet the minimum reporting requirements for US GAAP.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

To support the US GAAP (Generally Accepted Accounting Practices) reporting in Country Model Bank, some of the Temenos Transact core applications provide the data to meet the minimum reporting requirements for US GAAP.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

There are no Tasks available for US GAAP Reporting feature.


#### 📊 Outputs

There are no Outputs available for US GAAP Reporting feature.

---


### 2.30  Utility Files for Report Generation


> **📇 Quick Reference Card**
> 
> **Purpose:** *These files help in generating the reports in Temenos Transact and store information required for generating the closing and movement reports.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

These files help in generating the reports in Temenos Transact and store information required for generating the closing and movement reports.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

There are no Tasks available for Utility Files for Report Generation feature.


#### 📊 Outputs

There are no Outputs available for Utility Files for Report Generation feature.

---


### 2.31  Utility for Consolidation of Accounting Entries


> **📇 Quick Reference Card**
> 
> **Purpose:** *Consolidation of Accounting entries is an optional functionality to cater for high volume low value transactions. The AC.CONSOLIDATE.COND application is used to facilitate this functionality. The user can use the default records or create their own customised records. These records can be reversed i...*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

> **⚠️ Note:** Not to be confused with consolidation of accounting data discussed earlier in the guide.

Consolidation of Accounting entries is an optional functionality to cater for high volume low value transactions. The AC.CONSOLIDATE.COND application is used to facilitate this functionality. The user can use the default records or create their own customised records. These records can be reversed if consolidation is not required.


#### ⚙️ Configuration

The system supports the consolidation of records in STMT.ENTRY , (F) STMT.ENTRY , CATEG.ENTRY and RE.CONSOL.SPEC.ENTRY applications.

The following default records are available in Temenos Transact :

| Record Name | Description |
|---|---|
| CLDEFAULT | Consolidating STMT.ENTRY records over a customer account |
| DEFAULT | Consolidating STMT.ENTRY records over nostro and internal accounts |
| PLDEFAULT | Consolidating CATEG.ENTRY records for IC (Interest & Charges) only |
| REDEFAULT | Consolidating RE.CONSOL.SPEC.ENTRY records |

The number at which consolidation is defaulted can be changed in each record, using the No Entries Start field.


##### Archiving

The detailed entries that have been consolidated are archived every six months. These entries are extracted from the consolidated statement entry ID in the ACCT.STMT.PRINT table. The STMT.ENTRY.DETAIL record in ARCHIVE defines the archiving details for the detailed statement entries.


#### 📋 Tasks

There are no Tasks available for Utility for Consolidation of Accounting Entries feature.


#### 📊 Outputs

There are no Outputs available for Utility for Consolidation of Accounting Entries feature.

---


### 2.32  Utility for End of Year Procedure PLCLOSEOUT


> **📇 Quick Reference Card**
> 
> **Purpose:** *PL Close Out is the process whereby the system performs the period end closing of balances in the Profit and Loss (PL) accounts and moves the same to the internal Assets and Liabilities (AL) account.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

PL Close Out is the process whereby the system performs the period end closing of balances in the Profit and Loss (PL) accounts and moves the same to the internal Assets and Liabilities (AL) account.

Each day, when a General Ledger report is produced, it is possible to monitor both the balances and movements over the PL accounts and as such at the year end, the finance division of the bank needs to evidence the totals or net of profit/loss made by the bank. This is transferred to an internal account and the PL account balances will be re-initiated to 0 to start updating the new financial year’s movements.


#### ⚙️ Configuration

The PL.CLOSE.PARAMETER application has six main configurations:

- Reports
- Year End
- Excluded Types
- Grouping
- Halt Process
- Multi-GAAP


##### Reports

The reports section has three related fields - Report Type , Report and Report Data . These fields control the reports produced during the close out process. The reports can be ENQUIRY , REPGEN.CREATE or program driven. Report Type is used to specify the type (CRF, RTN, RPG or ENQ). Report contains the key to REPGEN.CREATE , ENQUIRY.REPORT , RE.STAT.REQUEST or a valid compiled program name. Report Data field allows the program-driven routines to be passed a parameter.

PL.CLOSE.PARAMETER report fields are shown in the screenshot below:


##### Year End

The financial period end is defined in the Close Freq Date field. This is usually a month-end date with a frequency to cycle to the next period end. The frequency can be Monthly, Quarterly, Semi-Annual or Annual.


##### Excluded Types

Certain Profit and Loss (PL) categories are used for non-financial purposes. These are normally not included in the close out, but they are parameterised (in case there is a specific need to include them). TYPES.TO.EXCLUD field contains the types that should not be included. By default, the following types are excluded:

- CP – Contingent
- CI – IAS P&L
- CL – Local Gap P&L


##### Grouping

The structure of the keys in the CONSOLIDATE.PRFT.LOSS file is set in PROFIT&LOSS record in CONSOLIDATE.COND . The essential elements are preset as ‘PL’ for the application id, ‘CURRENCY’ of the transaction and so on. Al Grouping field can be set to group the entries based on the user configured elements.

By default, the entries produced are based on the CATEGORY/CURRENCY and one entry is passed to the internal account (as defined in the PLCLOSE in ACCOUNT.CLASS ). Each of these entries is the sum of all the records in CONSOLIDATE.PRFT.LOSS matching the combination of CATEGORY and CURRENCY.

To produce entries summed at different group levels, user can add the additional elements from the profit&loss key so that the entries are summed for all records matching the same PLCATEGORY/CURRENCY/PLNATIONALI/PLSECTOR/PLINDUSTRY or whatever local settings the user has defined.


##### Halt Process

Close Hlt Prcss flag allows the Close of Business (COB) process to be halted just before the close out process is run. This allows the users to access reports or files to extract key financial data they require, before the files are updated by the process. If left unchecked, the process runs without halting.

> **⚠️ Note:** Though the halt field is included in each record of PL.CLOSE.PARAMETER , there will be only one halt to the COB processing. This happens once all the companies have finished this stage of the PL close out processing.


##### Multi-GAAP

For multiple reporting scenarios (IA, IFRS, Multi-GAAP and so on), the PL.CLOSE.PARAMETER provides the option to define the Category for each Position Type in the Position Type and Close Category fields.


#### 📋 Tasks

Related topics:

- Maintain Year End Parameters

General Ledger is a central repository for accounting data transferred from all sub-ledgers. PL Close Out is the process whereby the system performs the year end closing of balances in the Profit and Loss (PL) accounts and moves the same to the internal Assets and Liabilities (AL) account. PL account balances will be re-initiated to 0 to start updating the new financial year’s movements.


##### Workflow

This section helps the user to perform the below tasks:

This PL.CLOSE.OUT application controls the year-end financial process for the various companies available. It helps to define the financial year-end date, grouping of the totals and required reports to be run.

To setup year-end financial process, follow the below steps:

1. PL Close Parameter .
2. In the contract screen, enter company ID and click Enter.
3. In the PL CLOSE OUT PARAMETER screen, enter values in the following fields: Report Type Report Close Freq Date Position Type Close category
4. Click the Validate icon to check for overrides and errors.
5. Click the Commit icon.


#### 📊 Outputs

There are no Outputs available for Utility for End of Year Procedure – PL.CLOSE.OUT feature.

---


---


## Appendix A: Glossary of T24 Applications & Fields


This glossary lists all T24/Transact application names and field names referenced throughout this document, with descriptions where available.


### Applications


| Application | Description |
|------------|-------------|
| `ARCHIVE` | T24 application: ARCHIVE |
| `ASSET.TYPE` | T24 application: ASSET.TYPE |
| `BATCH.NEW.COMPANY` | T24 application: BATCH.NEW.COMPANY |
| `CATEG.ENTRY` | T24 application: CATEG.ENTRY |
| `COLLATERAL` | T24 application: COLLATERAL |
| `CUSTOMER` | T24 application: CUSTOMER |
| `Cycle Frequency` | T24 application: Cycle Frequency |
| `EB.ACCRUAL` | T24 application: EB.ACCRUAL |
| `FT.COMMISSION.TYPE` | T24 application: FT.COMMISSION.TYPE |
| `LIMIT` | T24 application: LIMIT |
| `LMM.ACCOUNT.BALANCES` | T24 application: LMM.ACCOUNT.BALANCES |
| `LMM.INSTALL.CONDS` | T24 application: LMM.INSTALL.CONDS |
| `MS.PARAMETER` | T24 application: MS.PARAMETER |
| `PC.CATEG.ADJUSTMENT` | T24 application: PC.CATEG.ADJUSTMENT |
| `PC.CONSOL.ADJUSTMENT` | T24 application: PC.CONSOL.ADJUSTMENT |
| `PC.PARAMETER` | T24 application: PC.PARAMETER |
| `PC.PERIOD` | T24 application: PC.PERIOD |
| `PC.STMT.ADJUSTMENT` | T24 application: PC.STMT.ADJUSTMENT |
| `PC.UPDATE.REQUEST` | T24 application: PC.UPDATE.REQUEST |
| `RE.CONSOL.SPEC.ENTRY` | T24 application: RE.CONSOL.SPEC.ENTRY |
| `RE.STAT.LINE.BAL` | T24 application: RE.STAT.LINE.BAL |
| `RE.STAT.LINE.MVMT` | T24 application: RE.STAT.LINE.MVMT |
| `STMT.ENTRY` | T24 application: STMT.ENTRY |


### Fields Referenced


| Field | Field | Field |
|-------|-------|-------|
| `Accounting Date` | `Arc Filename` | `Archive Data` |
| `Asset` | `Asset Type` | `Ccymkt Postype` |
| `Charge Code` | `Cycle frequency` | `Dbase Name` |
| `Deal Date` | `Emit Business Event` | `Last PC Date` |
| `Last Pc Date` | `Next Frequency Date` | `Open PC Period` |
| `Output Mode` | `PC Period End` | `PL Applic ID` |
| `PL Category` | `Pc Adjust For Contract` | `Pc Applied` |
| `Pc Period` | `Pc Period End` | `Pl Category Pm Py` |
| `Pl Category Prev Mth` | `Pl Category Prev Year` | `Principal` |
| `Retention Period` | `Status` |  |


---


## Appendix B: Consolidated Field Reference


This appendix consolidates all field description tables from across the documentation, grouped by sub-module. This provides a single reference for all field definitions.


### General_Ledger_Accounting - PC (PC)


**Misc**

| S.NO | Parameters | Description |
|---|---|---|
| 1 | PC.PARAMETER | It allows the user to configure the frequency for post-closing periods. Users can define the DataBase Path for master company alone and for other lead companies, DataBase Path fetches from master company. Cycle frequency is mandatory for lead companies and optional for master company. Last PC Date , Status and Next Frequency Date fields gets updated automatically upon successful creation of PC.PERIOD . |


### General_Ledger_Accounting - RE (RE)


**Banking Framework Exit Point**

| Entry Event | Description | Base Table for Entry Event | Transaction Table Available for Enrichment |
|---|---|---|---|
| ENTRY.DEFAULT | This is the default entry event with all the details from STMT.ENTRY if a specific entry event is not identified. | STMT.ENTRY | - |
| ENTRY.FT | This entry event is triggered if the SYSTEM.ID from the entry is FT. | STMT.ENTRY | FUNDS.TRANSFER |
| ENTRY.AAAA | This entry event is triggered if the SYSTEM.ID from the entry is AAAA. | STMT.ENTRY | AA.ARRANGEMENT.ACTIVITY |
| ENTRY.DX | This entry event is triggered if the SYSTEM.ID from the entry is DX. | STMT.ENTRY | DX.TRADE |
| ENTRY.SCCA | This entry event is triggered if the SYSTEM.ID from the entry is SCCA. | STMT.ENTRY | ENTITLEMENT |
| ENTRY.FX | This entry event is triggered if the SYSTEM.ID from the entry is FX. | STMT.ENTRY | FOREX |
| ENTRY.SCSP | This entry event is triggered if the SYSTEM.ID from the entry is SCSP. | STMT.ENTRY | SEC.TRADE |

**Enforcing Balanced Accounting Entries**

| Application | Description |
|---|---|
| DATA.CAPTURE (DC) | Journaling functionality that can raise one-sided entry. There is a mechanism to stop unbalanced batches already in place. |
| FIDUCIARY (FD) | Can make two separate calls to accounting. |
| REVALUATION.AL | Generates one sided entries during the COB. |

**Misc**

| Business Event | Description |
|---|---|
| financialAccounting.UpdateAccountingJournalEntries.AccountingJournalEntriesUpdated | The accounting event is generated when the Transact accounting process authorises a transaction. The generated accounting event contains the details of the generated accounting entries, along with account and contract static information, account balances extracted from the Contract Balance record, the booking and value -dated account balances from the Account Balance Activity record. |
| financialAccounting.UpdateContractBalances.ContractBalancesUpdated | The balance update event is generated when the Contract Balance record is updated by other process other than the accounting process. The generated balance update event contains account and contract static information, and the account balances. |

**Misc**

| S.No. | Parameters | Description |
|---|---|---|
| 1. | CONSOLIDATE.COND | This application allows the user to define the parameter setup to consolidate data under two categories – Asset and Liability, Profit and Loss. The Asset and Liability consolidation file key is made up of four mandatory parameters – Application, Currency market, Position Type and Currency. The Profit and Loss consolidation file key is made up of one mandatory parameter, that is, Forex position type. |

**Misc**

| S.No. | Parameters | Description |
|---|---|---|
| 1. | RE.STAT.COLUMN.TYPE | This application allows the user to define the details for each column to be printed. These details indicate if the balance amount or movement amount must be printed for local currencies, foreign currencies or for all currencies. |
| 2. | RE.STAT.REPORT.HEAD | This application allows the user to define the heading details indicating the column to be printed, amount size, reports for currencies, report heading and if entries have to be printed. |
| 3. | RE.STAT.REP.LINE | This application allows the user to define the details containing the different line and line of contents. It also contains details about totaling, spacing of the lines, and types of Central Reporting Base records to be printed. |
| 4. | RE.STAT.ENT.FORMAT | This application allows the user to define the file containing details about the presentation and format of entries to be included in a report. Titles, headers and columns are described and special masks can be specified. |
| 5. | RE.STAT.RANGE | This application allows the user to define a record containing a range of values or a set of individual values for a report line content definition. User can also set up a ‘standard’, often used for virtual views as a help or short cut in the report line definition process. |
| 6. | RE.STAT.NAME | This application allows the user to group different consolidation conditions under a common mnemonic name. The purpose is to provide a shortcut for definition of reporting line contents, which are repetitive within one or among several reports. |
| 7. | RE.AMT.ABBREV | This application allows the user to define the file that holds the descriptions for amount format displays to be printed in a specified user language at the top of a report. |
| 8. | RE.STAT.OUTPUT | This application allows the user to define the content and layout of this output file. The user can generate output to a sequential disk file or in the standard printed output. |

**Utility for Consolidation of Accounting Entries**

| Record Name | Description |
|---|---|
| CLDEFAULT | Consolidating STMT.ENTRY records over a customer account |
| DEFAULT | Consolidating STMT.ENTRY records over nostro and internal accounts |
| PLDEFAULT | Consolidating CATEG.ENTRY records for IC (Interest & Charges) only |
| REDEFAULT | Consolidating RE.CONSOL.SPEC.ENTRY records |


---
