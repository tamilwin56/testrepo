
# Temenos Transact — Trade_Management Module Documentation


> **Comprehensive User Guide**
> Generated: 13 April 2026
> Content: Configuration | Reference | Field Descriptions | Glossary


## Table of Contents

  - [Trade_Management Module Overview](#trade_management-module-overview)
    - [Sub-Module Summary](#sub-module-summary)
    - [How to Use This Guide](#how-to-use-this-guide)
  - [Chapter 1: Trade_Management - TFO](#chapter-1-trade_management---tfo)
    - [Features in Trade_Management - TFO](#features-in-trade_management---tfo)
    - [1.1  Misc](#11-misc)
    - [1.2  Misc](#12-misc)
    - [1.3  Blotter](#13-blotter)
    - [1.4  Dashboard](#14-dashboard)
    - [1.5  Deal Capture](#15-deal-capture)
    - [1.6  Exception Workflow Management](#16-exception-workflow-management)
    - [1.7  Limits](#17-limits)
    - [1.8  Misc](#18-misc)
    - [1.9  Positions](#19-positions)
  - [Appendix A: Glossary of T24 Applications & Fields](#appendix-a-glossary-of-t24-applications-fields)
    - [Applications](#applications)
    - [Fields Referenced](#fields-referenced)
  - [Appendix B: Consolidated Field Reference](#appendix-b-consolidated-field-reference)
    - [Trade_Management - TFO (TFO)](#trade_management---tfo-tfo)

---


## Trade_Management Module Overview


This document provides comprehensive documentation for the **Trade_Management** module of Temenos Transact. It covers **1 sub-modules** with a total of **9 feature areas**.


### Sub-Module Summary


| # | Sub-Module | Code | Features | Description |
|---|-----------|------|----------|-------------|
| 1 | **Trade_Management - TFO** | `TFO` | 9 | Trade_Management - TFO module of Temenos Transact |


### How to Use This Guide


Each feature in this document is organized into the following sections:

- 📖 **Introduction** — Overview and purpose of the feature
- ⚙️ **Configuration** — How to set up and configure the feature
- 🔧 **Working With** — Operational usage and field descriptions
- 📋 **Tasks** — Step-by-step procedures
- 📊 **Outputs** — Reports, enquiries, and generated outputs

Each feature includes a **Quick Reference Card** at the top with application names, key fields, prerequisites, and a summary. Appendices provide a full glossary, consolidated field tables, and end-to-end use-case scenarios.

---


## Chapter 1: Trade_Management - TFO


Trade_Management - TFO module of Temenos Transact


### Features in Trade_Management - TFO


| # | Feature | Sections |
|---|---------|----------|
| 1.1 | Misc | Intro |
| 1.2 | Misc | Intro |
| 1.3 | Blotter | Intro, Worki, Tasks, Outpu |
| 1.4 | Dashboard | Intro, Worki, Tasks, Outpu |
| 1.5 | Deal Capture | Intro, Worki, Tasks, Outpu |
| 1.6 | Exception Workflow Management | Intro, Worki, Tasks, Outpu |
| 1.7 | Limits | Intro, Worki, Tasks, Outpu |
| 1.8 | Misc | Intro |
| 1.9 | Positions | Intro, Worki, Tasks, Outpu |


### 1.1  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Foreign Exchange (FX) module is designed to meet the needs of dealing operations in the Foreign Exchange Market.*
> 
> **Key Fields:** *Cus Margin Default*, *FX Commission Group ID*, *FX Group Cond ID*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- APIs
- Temenos Transact Services

The Foreign Exchange (FX) module is designed to meet the needs of dealing operations in the Foreign Exchange Market.

The module offers comprehensive treasury solution starting from the deal capture in the front office to deal processing in back office, covering a wide range of FX products. The module covers entire deal life cycle of FX transactions including features such as recording of limited orders, online limit checking, position updating, revaluation of positions, accounting, brokerage, generation of SWIFT confirmations, payments and print advices. In addition, the module also helps generate reports for audit and risk management.

The above image illustrates spot, forward and swap deal types and its associated transaction types supported by the system, which caters to the business needs of Treasury.

Using FX module, a dealer can directly input a deal in the system with key elements, such as currencies, amount, rate, value date and counter-party. This avoids the need for hand-written deal tickets and ensures the real-time update of positions and risk, that is, counterparty’s liability or exposure, exchange position and daily foreign exchange movements reflects the dealer’s system inputted deal.

All elements of FX transactions have default values, except the key information that the dealer provides. Thus, for any given counterparty, payment methods and instructions are loaded automatically from user definable tables. If required, the back office user can confirm or exceptionally amend the deals.

The ability to arrive at intelligent defaults also has another benefit. For example, in a swap, all the default information on the second leg is derived from the first leg. Thus, dealer’s input of information is reduced to the minimum.

After the dealer provides their inputs, the deal slips are printed for the back-office. At the authorisation stage, the system invokes the following:

- Generating and delivering confirmations
- Passing any accounting entries such as brokerage, commissions and charges, and issue of any required pay or receive instructions

Otherwise, there are overnight processes that involve eventual settlement, revaluation and accruals, and exception or maturity reporting.

The FX application is supplied with initial input of the contract details with a few of them requiring any changes during remaining life cycle. Such changes, if any, are generally limited to settlement related. The brokerage calculation and processing of brokerage is handled by using BROKER application.


##### Product Configuration

This section describes the configuration options the system offers in FX.


##### FX Build Sequence

Implementation of FX module begins with configuration of various parameter tables.

The following list of files are required for FX main setup, and the mandatory files are suffixed with an *. The dependency tables are marked and stated alongside the parameter tables in their build sequence.


##### Illustrating Model Parameters

The model parameters consists of the following:

| S.No | Parameters | Description |
|---|---|---|
| 1 | FX.PARAMETERS | The rules that determined the Foreign Exchange (FX) transactions are defined in the following files: Classifies spot and forward contracts, according to local central bank and internal reporting rules. Defines the spot default value date. Uses the OFS.SOURCE ID present in this field to perform FX.BULK.ORDER . Uses the version ID present in this field as VERSION to populate or create FX BULK DEAL master records. Defines default category code for spot, forward and swap transactions. Defines the precious metal currency codes, hence, any number of currency codes can be defined. Conditions under which deals are entered with split value dates. Indicators show if Profit & Loss (P&L) and EXCHADS entries are booked when revaluation of forward and spot contracts takes place. Creates rounding rule for transactions. The Cus Margin Default field determines if the FX Group Cond ID corresponding to a customer is defined in a FX contract or not (subjected to the existence of the condition priority setup in FX margin). The values accepted are Yes, No and None. If set as Yes, the FX Group Cond ID defaults from SEC.ACC.MASTER ( SAM ). If it is not available in SAM , it defaults from CUSTOMER.CHARGE . If set as No or None, the FX Group Cond ID does not default from SAM or CUSTOMER.CHARGE . However, the user can still define the margin percentage manually (together with treasury rate) and derive the customer rate in FX deal. |
| 2 | FX.POS.TYPE | Assigns profit centre to the trading position, which can be amended as desired. |
| 3 | FX.TRANSACTION.TYPE | Classifies the deal types. A record in this application can control the default value for category codes, revaluation types, and allows delivery and types of options processing. The existing records can be amended and new records can be created. |
| 4 | FX.GEN.CONDITION | Identifies a specific group of customers, which can be cross-related to the group condition table, to define conditions applicable to that group. The groups are determined based on customer details such as sector and target. The criteria used and their priority are specified in the Condition Priority file in the record whose ID is FX.MARGIN. |
| 5 | FX.GROUP.CONDITION | Defines the spread or margin percentage for a specific customer, group of customers or default group. When a group customer is defined, the FX Gen Condition record needs to exist before any associated group condition is specified. For an individual customer, the ID is C , whereas, the default group ID is generally assigned as either 99 or 999. |
| 6 | FX.COMM.GROUP | Defines spread or margin based on currency, and the amount that falls in a range and is used in FX contracts. The FX Commission Group ID field in SAM is used in FX.BULK.ORDER application, and a reference to SAM is used in FX.GROUP.CONDITION . Hence, the margin is given in absolute terms or referred to FX Commission Group ID (based on which the margin is applied in an FX deal). |


##### Illustrating Model Products

The following products are available in the FX module:

| S.No | Parameters | Description |
|---|---|---|
| 1 | FX Spot | FX Spot is a contract of buying or selling a currency, commodity or security for immediate settlement (payment and delivery) on the spot date at a spot Rprice. |
| 2 | FX Forward | FX Forward is a contract of buying and selling an asset or a currency at a predetermined spot rate at a specified date in the future (which is greater than the spot date). The predetermined rate is called as the Forward Rate. |
| 3 | FX Swap | FX Swap is an agreement between counterparties to exchange currency. The agreement involves swapping of principal and interest payments between two different currencies. |
| 4 | Precious Metal Deal | Precious Metal Deals involve trading in various precious metals such as gold, silver, palladium, platinum and so on, in spot, forward or swap rates depending on the types of deals entered. |
| 5 | Single-rate Option | Single-Rate Option is the deal of exchanging one currency for another. The delivery takes place between two specified dates at customer’s choice without incurring any penalty cost. The option occurs when the customer decides to take delivery of all or part of the transaction before the final value date. |
| 6 | Multi-rate Option | Multi-rate Option is the deal of exchanging one currency for another. The delivery takes place between two different option dates with different rates. The option occurs when the customer decides to take delivery of all or part of the transaction before the final value date. In this, the applied rate depends on the period delivery. |
| 7 | Internal Deals | Internal Deals allow transfers between different positions or dealer desks. Hence, there is no need for accounting entries, payments, advices and so on. The system automatically updates the position, when an internal forex spot or a forward deal is entered. |
| 8 | Broker Deal | Broker Deals are entered when the counterparty is not known. The user needs to enter BR as sub-type and associated brokers deals. Once the counterparty name is known, BR is removed and the counterparty details are entered in the deal. |
| 9 | NDF Vanilla Deal | Non Deliverable Forward (NDF) Vanilla Deals is an hedging strategy, where parties in the contract agree to settle the profit or loss prior to the expiration date of the contract. A vanilla NDF transaction has an agreed rate fixing date, which is two working days before the settlement date. |
| 10 | NDF Exotic Deal | An Exotic NDF Deal allows in setting the fixing date as any date before the vanilla date in the tenure of the transaction. The fixing profit is discounted, if the NDF is fixed and settled early. The discount amount is amortised from the settlement date to the value date of the NDF. |

---


### 1.2  Misc


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


### 1.3  Blotter


> **📇 Quick Reference Card**
> 
> **Purpose:** *The trade blotter is a record of trades that are transacted over a period of time. The user can perform various actions, such as View, Delete, Amend, Reverse and execute FX Limit Orders.*
> 
> **Key Fields:** *List*, *Range*, *Value*
> 
> **Sections:** 📖 Introduction | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The trade blotter is a record of trades that are transacted over a period of time. The user can perform various actions, such as View, Delete, Amend, Reverse and execute FX Limit Orders.


#### 🔧 Working With

The user needs to perform the following actions to access the Blotter option:

1. Bank Demo .
2. To minimise the menu, on the upper-right corner of the left pane, click .


##### Blotter Features

This section explains the common features that help the user to navigate easily and to simplify the actions, these features are available on the right pane of the screen as shown below:

TFO allows the user to copy the link of the actual blotter selection to open in a new source or send to a third person.

1. To copy the link to the clipboard, click .
2. To open another page with the previous search, click the Search button.

The system copies the URL and deep link. On clicking the link copied on the dashboard, the system can apply all the searches, filters and conditions applied. In this way, the user can share or copy other machines specific searches or blotter criteria with the correspondent results.

- To add a favourite to the main Favourites, click .

> **⚠️ Note:** The user can rename the favourite. Also, remove it from the Favourites by clicking the cross next to the relative favourite.

- To edit the layout, click .

Blotter offers multiple actions for the user to provide high flexibility and customisation.

The user can reorder the headings based on their requirements.

1. To reorganise the layout, click the heading to be moved and drag it to the new position, as shown below.

The transaction heading is moved.

The user can rename the column headings. In the following example, Transaction heading is changed to Trans.

- To rename the heading, double-click the selected heading and then enter a new name.

> **⚠️ Note:** If the user tries to name the column or give a short name that already exists an error is displayed.

The user can resize the width of the columns.

- Click the vertical line that divides the headings and then drag it for the required size.

> **⚠️ Note:** The user cannot reduce the default minimum dimension for each heading.

The user can hide the headings based on their requirements, and create own versions of blotter where only some headings are displayed.

1. To hide the column, right-click the heading and then click Hide .
2. To unhide these columns, right-click the hidden heading and then click Show .

> **⚠️ Note:** The user can hide any number of headings.

1. To save the layout after editing, click .
2. To reset the default layout, click .

The user can clone a column layout from a specific user, instead of creating a new one.

1. To clone a blotter, click .
2. In the Search bar, type the username.
3. Click the Clone Layout button, the highlighted tab appears.
4. Enter the username of the user whose layout needs to be cloned (for example, John Smith). The layout is imported.

TFO allows the user to export the selected blotter in different formats. Further options are available in the More Options button.

The user can download the blotter in three different formats, which are shown below:

- PDF
- XLS
- CSV

This option allows the user to print the blotter directly.

The user can sort the transactions according to their needs. This feature is applicable to almost all the headings, and it enables to sort in ascending or descending order.

The below actions are to be followed to sort the transaction by the Rate1.

1. To sort the transaction in ascending order, click Rate 1 .
2. To sort in descending order, re-click Rate1 .

To perform this task:

1. Click the heading, a drop-down list is displayed.
2. Click a value in the drop-down list. For example, when ‘EXOTIC’ is selected, only NDF Exotic deals are displayed.

The user can filter the blotter in different ways. Single and multiple criteria can be entered by using the command line or specific criteria button. This section focuses on the different filter types and then the criteria are available.

The user can filter the blotter according to the requirements. A filter can be applied in many ways. However, after the input, they appear on the command line in three colours as follows:

- Blue – Server-side filters
- Green – Client-side filters
- Red – Error (when the system does not recognise the format of the filter)

This helps the Dealer to gather data based on one or more selected columns. To perform this, do the following:

1. Enter the column name or short name followed by a value.
2. Click the Apply button.

> **⚠️ Note:** The system does not automatically filter the results even after the criteria is selected. However, the user needs to apply the filter to display the data from the server.

The blotter is filtered and only the transactions with the Type as Spot are listed.

This filter applies a text search of the data available on the screen. Otherwise, it is used to search the blotter across all the columns.

This filter is identified in green. In the below example, the last server-side filter is provided, after the input of a client-side filter on the previous selection. Values for the selected blotter are:

- Type – SP
- Client-side filter – EUR

The above screenshot shows all the deals where Type is SP (Server-side) and EUR currency is included in the transaction.

Client-side filter does not use the

button, as direct interaction with the server is not required. However, it can be accessed by using the command line.

- They allow the user to directly search for full or partial parts of headings by only typing the desired value, without giving any input in the headers.
- This can be input on a server-side selection. However, the reverse is not allowed.

The first way to input a filter is by using the Criteria button. It allows the user to enter a filter in any of the headers directly.

The user can select any of the headers on the left pane and then input the Value, Range or List. These criteria represent server-side filters. Therefore, correct and full spelling of the headers is required.

The criteria button allows the user to access two main types of filters, which are single or multiple criteria search.

A single criteria is a search based on one header. In this header, the user can search for a single value, range or list of values.

- Value – A single value is provided in the search.
- Range – A deal is searched among a range of values. This appears on the command line with a string ‘-‘ between the values.
- List – To list more than one value for a single header. This represents the OR function. The user can input only three values using the Criteria button. However, once added on the command line, the user can list the values by using the format ‘value1, value2, value3’.

> **⚠️ Note:** All the cases of single criteria, inserted by using the Criteria button, represents a server-side filter. Therefore, to retrieve the results, it is required to click the Apply button. Each criteria is automatically reported on the command line as shown in the screenshots.

The user can input only one of the above fields. However, the system shows an error, when more fields are populated.

The user can automatically input a multi-criteria filter by repeating the previously mentioned operation two or more times using the Criteria Button.

For example, if the user wants to list all the transactions where the Ccy1 is EUR and Ccy2 is GBP, the process shown in the screenshot needs to be followed.

Another way to input search criteria is to type directly in the command line. The headers are identified only using two inputs:

The complete spelling. For example, Transaction, Type and Counterparty.

The predetermined short form of the above headers. They are found by hovering the mouse on the headers. For example, txn, ty and st.

The format of the command line input:

space

If a multi-criteria search is required, enter space before the second criteria:

space space space

This represents the AND function.

If a list of values for a single header is required, the format is:

space ,

This represents the OR function.

The format for inputting a range of values:

space -

space - = Lesser than value

space = Greater than value

The command line filter also allows a quick-filter search, based on a client-side filtering. This filters all the transactions that include the user’s input in any of the headers.

An example is shown below, where an input of FX1608 is given. The system checks the blotter and lists the transactions that match the input.

When the input is done on a client-side request, the system automatically lists the results without clicking the Apply button.

This feature allows the user to save different criteria for easy and efficient navigation.

1. To save a search, click .
2. Rename the saved search.

Blotter allows the user to identify and perform multiple actions on a single deal. The system can recognise the actions available for the user according to the record status.

The user can click the required transaction to select a deal. The system opens the first view of the above deal on the right side of the screen. This displays all the details of the deal with the Transaction ID.

After selecting the required transaction, the system automatically retrieves the possible actions available for the user. This feature is user-specific. The user can perform specific actions according to the privileges specified in the user application. The system can identify the deal and user-specific actions available for every single deal.

The above-highlighted buttons represent the actions that the user can perform.

> **⚠️ Note:** The copy function is not allowed for FX in Temenos Transact but in Front Office, as it takes the values from the copied deal. It also allows the Dealer to make changes and send the deal details to FX application.

In the case of generic blotter, the user can access more options.

1. To close the Deal screen, on the same line of the Transaction ID, click .
2. To download all the deal details in different formats (such as PDF, CSV and XLS), click .


#### 📋 Tasks

There are no Tasks available for Blotter feature.


#### 📊 Outputs

There are no Outputs available for Blotter feature.

---


### 1.4  Dashboard


> **📇 Quick Reference Card**
> 
> **Purpose:** *Dashboards provide at-a-glance views of key performance indicators (KPIs) relevant to a particular objective or business process.*
> 
> **Sections:** 📖 Introduction | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Dashboards provide at-a-glance views of key performance indicators (KPIs) relevant to a particular objective or business process.

Dashboards allow managers to do the following:

- Monitor the contribution of various departments in the organisation.
- Capture and report specific data points from each department within the organisation, thus providing a snapshot of the performance.
- Measure how an organisation performs.

The benefits of using digital Dashboards include the following:

- Visual presentation of performance measures
- I dentif ication and correct ion of negative trends
- Measurement of efficiencies or inefficiencies
- G enerat ion of detailed reports showing new trends and by saving time from running multiple reports
- D ecision making based on collected business intelligence
- Alignment of strategies and organi s ational goals
- T otal visibility of all systems instantly
- Quick identification of data outliers and correlations

The Treasury Front Office (TFO) Dashboard displays KPIs to a front office Dealer in the form of a widget.

- Dealer .


#### 🔧 Working With

The Treasury Front Office (TFO) Dashboard has the following features:

- C apability of creating multiple-dashboards and user- defined grouping of widgets
- On-demand addition or removal of widgets
- O ptions for the user to toggle the data in numerical or graphical (chart) format
- R e-arrang e widgets by drag-and-drop
- Automatic and manual resizing of widgets
- Option to set auto or manual refresh for the charts or numbers in the widgets
- Creat ion of on-the-fly widgets from supported TFO enquiries or blotter
- Ability to show parent enquiry from the widgets and capability to drill down to deal level data


##### Widgets

TFO Dashboard has default widgets, which provides various information to the Dealer. These widgets are differentiated according to the information given below.

The first group of widgets is connected with the Currency and Currency Pair positions of the Dealer. When the user clicks , the currency pair displays with a lighter background.

> **⚠️ Note:** In all the position related widgets, red represents the short position and blue identifies the long position.

There are three Currency position related widgets in the Dashboard, which are displayed below.

Dashboard considers the currencies and currency pairs set as Favourites in the FX Position section by default. Currency Position intra-day represents the positions related to the transactions entered today.

The user can change the Favourite currencies and pairs as given below.

The JPY, INR and SGD are selected as Favourites. Hence, the information in the relevant widgets of the Dashboard changes accordingly.

The Dealer can access the FX Currency Position and FX Currency Pair position from the Dashboard.

An example is given below.

To open FX Position by Currency Pair, the dealer clicks one of the currency pairs, as given below.

This navigation is allowed only Currency Pair Position, Currency Position and Currency Position Intra-day widgets.

The second group of widgets is Blotter related. These are displayed with a dark header background compared to the Currency Position widgets as highlighted below.

The red block on the chart represents unauthorised deals and blue block represents the deals with statuses other than INAU.

The Blotter widgets direct the user to the Blotter screen when the user clicks the displayed chart.

An example is given below:

To view the deals on the Blotter, the user clicks the Customer bar in the widget. The Blotter screen appears as a result of the applied filter criteria, to compile the widget as shown below:

The user can create Dashboard widgets from Blotter, which is completely user-defined. The features of such user-created Dashboard widgets are similar to other widgets.

The user performs the following:

1. On the Blotter screen, s elect the required filter criteria.
2. Save the Blotter view as Dashboard , where the represents the name of Dashboard w idget (user can name this according to their choice ) .
3. On the Dashboard screen , right - click the header of any already existing Dashboard w idget to select the created widget from the drop-down.
4. On the Blotter screen, enter the filter criteria as c1 USD c2 GBP ty SP. It displays the list of all the deals, where Currency 1 is USD, Currency 2 is GBP and Deal Type is Spot.
5. Click Save and name the saved view with free text, prefix with the word Dashboard. For example, ‘Dashboard Spot USD-GBP’.
6. On the Dashboard screen, right-click the header of any existing widget to select the newly created Dashboard widget from the drop-down.

> **⚠️ Note:** The user can perform the same action by clicking the highlighted widget.


##### Standard Widgets

This section explains all the default widgets.

FX has the following types of widgets:

This widget shows the count of various FX deals executed by the user.

The count of all trade types done by all the dealers.

> **⚠️ Note:** The total number of transactions available is displayed at the bottom of the screen.

This widget shows the total count of deals across all FX deal types in blue and unauthorised deals of those deal types in red.

> **⚠️ Note:** The total trade count is displayed at the bottom of the widget.

This screen has information about the FX Limit Order deals to be executed in the Blotter.

> **⚠️ Note:** The user can navigate directly to the Blotter to analyse these deals.

This widget shows the count of broker deals that await counterparty confirmation. The X-axis shows the Broker code and Y-axis shows the count of deals.

> **⚠️ Note:** The system also gives the total number of the transaction available at the bottom of the screen.

This shows the short and long position for the currencies set as favourite in the Currency Position view.

> **⚠️ Note:** The user can navigate directly to the Currency position screen from this widget.

This widget shows the short and long position for the currency pairs set as a favourite in the Currency Position view of TFO application.

> **⚠️ Note:** The user can navigate directly to the Currency position screen from this widget.

This widget shows the Intra-day Net position for the currencies set as a favourite in the Currency Position for the system date.

This widget displays a consolidated balance of Nostro accounts, currency-wise for five days from the current date.

The user can select any currency from the drop-down list to view the Nostro account balance.

This widget displays an overview of the liquidity gap for five days from the current date in the specified currency.

> **⚠️ Note:** The user can change the currency shown on the upper-right corner of the screen.

By entering a different currency, the displayed data changes accordingly, as shown below.

This widget displays an overview of the Interest Rate Gap for five days from the current date in the specified currency.

> **⚠️ Note:** The user can change the currency shown on the upper-right corner of the screen.

By entering a different currency, the displayed data changes accordingly, as shown below.

This widget displays an overview of the overall bank or single Dealer Desk Currency position.

> **⚠️ Note:** The user can change both currency and dealer desk shown on the upper-right corner of the screen at any stage.

By entering a different currency, the displayed data changes accordingly as shown below.

Additionally, the user can view the overall bank position (when all desks are specified) or the individual Dealer Currency position, as shown below.

The above screenshot shows the drop-down list from which the user can select a Dealer.

> **⚠️ Note:** This section shows all the valid record that a Dealer has in Temenos Transact DEALER.DESK table. By selecting the specific dealer desk, the data changes accordingly.

MM has the following types of widgets.

The widget displays all MM call and notice live placement contracts.

The widget displays all MM call and notice live taking contracts.

The widget displays all MM fixed-term live placement contracts.

The widget displays all MM fixed-term live taking contracts.

The widget lists all the fixed-term placement contracts whose maturity is within the next five days.

The widget lists all the fixed-term taking contracts whose maturity is within the next five days.

FRA has the following types of widgets:

This widget displays the count of all unauthorised FRA trades in the form of a chart, number and list.

This widget displays the count of all live FRA Trade Purchase deals in the form of a chart, number and list.

This widget displays the count of all live FRA Hedge Purchase trades in the form of a chart, number and list.

This widget displays the count of all live FRA Trade Sale trades in the form of a chart, number and list.

This widget displays the count of all live FRA Hedge Sale trades in the form of a chart, number and list.

This widget lists all live FRA deals whose rate-fixing date is within the next five days from today.

This widget displays the count of all FRA trades executed today in the form of a chart, number and list.

Swap has the following types of widgets:

This widget displays the count of all unauthorised swap deals in the form of a chart, number and list.

This widget displays the count of all live swap deals in the form of a chart, number and list.

This widget lists all live swap deals whose maturity date is within the next five days from today.

This widget displays the count of all swap deals executed today in the form of a chart, number and list.

The below security dashboard widgets are available on the Model Bank user login.

This widget displays the count of all security trades done today, which are categorised in different sub-asset types, such as treasury note, ordinary shares, and floating-rate notes. The widgets can be in the form of chart, number and list.

This widget displays all outstanding security trades categorised in different asset type.

This widget displays all outstanding security trades categorised in different sub-asset type.

This widget lists all live security trades booked in different trade currency. The widgets can be in the form of a chart, number and list.

This widget lists all live security trades booked in different Own Book Portfolio books. The widgets can be in the form of a chart, number, and list.

This widget displays the count of all security trades executed today, which are categorised in different asset types, such as bond and shares. The widgets can be in the form of a chart, number and list.

This widget shows the number of deals that are pending action from the user.

This widget displays the count of all REPO trades executed today.

This widget lists all the live REPO trades by type.

This widget lists all the live REPO trades by sub-type.

This widget lists all the REPO trades with fixing date as Today.


##### Customising the Widgets

The Dashboard presents a default screen where all the widgets are shown. However, the user can customise the setup of the screen according to the requirement or preference.

To manually refresh the information shown on each widget, the dealer can click .

The user can change the view of the specific widgets and also navigate to the pre-defined views available for all available widgets.

The below screenshot shows today’s deal widget.

1. Click . The display changes from chart form to a list.
2. In the list of all the transactions done today, to view the details of a specific deal, click the deal.
3. To change the view, re-click the Change Display button. It displays the number of transactions present in the screen.

- By clicking this button, the system automatically redirects the Dealer to Blotter.
- T here is a specific set of display for each screen , which differ s according to the features.

The Dealer can resize the widgets. To perform this action, click the S etting button of the specific widget, as shown below.

The size selection is displayed, as shown below.

The different widget size options available for selection are 1x1, 3x2, and 1x3. In the below example, the 3x3 widget size is selected.

> **⚠️ Note:** The system automatically aligns the other widgets and adjusts the screen according to the size of the widgets.

A second way to customise the screen is the ‘Drag and Drop’ option, which allows the Dealer to modify the position of the single widgets. The dealer performs the following:

1. Click the required section on the screen, as shown below.
2. Drag and drop the highlighted window from the upper-right to the lower-right of the screen.

The Dealer can change the chart type used on the Blotter widgets.

1. Click of the specific widgets, as shown below.
2. In the Chart Type drop-down list, select the required type..
3. In the Group By drop-down list, select the grouping rule to display the chart accordingly.

The Dealer can also remove one or more widgets to display only a few widgets. The Dealer performs the following:

1. On the upper-right corner of the screen, click .
2. To reopen the view, right-click any of the top bars of the widgets. A list of all the closed views is displayed.


#### 📋 Tasks

There are no Tasks available for Dashboard feature.


#### 📊 Outputs

There are no Outputs available for Dashboard feature.

---


### 1.5  Deal Capture


> **📇 Quick Reference Card**
> 
> **Purpose:** *The deal capture feature allows the following:*
> 
> **Applications:** `AGENCY`, `BASIC.INTEREST`, `BROKER`, `CCY.FOR.PAYMENT`, `CURRENCY`, `CUSTOMER`, `CUSTOMER.SECURITY`, `DEALER.DESK` ... +21 more
> 
> **Key Fields:** *Account Number*, *Accrued Interest*, *Action Buttons*, *Additional Agreements*, *Adjustments*, *Agreement*, *Agreement Type*, *Amount* ... +274 more
> 
> **Sections:** 📖 Introduction | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The deal capture feature allows the following:

- Booking of trades concluded by dealers across multiple asset classes.
- Manual input or STP using interface to dealing systems.
- Minimise the number of keystrokes required by a dealer to capture the deal.

> **⚠️ Note:** Unique deal capture screen is created for each sub-product within a product, hence, data fields relevant to the specific sub-product are only present.


#### 🔧 Working With

This section helps the user to understand the working of Deal Capture.


##### Generic UI Features

Treasury Front Office (TFO) offers generic features that apply to all deal capture screens. These features are explained in the below sections:

TFO allows the user to copy the link of a deal to open in a new window or to share it with another user. The system not only copies the URL but also the deep-link, which allows applying all the data, filters and other user conditions.

1. To copy a link, click the link icon. The system automatically copies the link to the clipboard.
2. To open the link in another window, paste the link on the main command line.
3. Click the Search button. The system automatically opens another screen with the previous deal inputs.

TFO allows the user to add a favourite to the main Favourites menu for quick access.

1. On the upper-right corner of the Deal Capture screen, click the Favorite icon.
2. Type a name in which the deal needs to be stored in the Favourite of the main application menu. This helps to access the Favourite screen quickly.

> **⚠️ Note:** The user can rename or remove the link from the Favourites. To remove, click Cross icon of the respective favourite.

This has the text explanation of the data input so far. This feature aims to provide a text of all key contractual data entered in the screen. An example is shown in the below screenshot.

The system sums up in a short sentence, which is the primary conditions of the deal.


##### What-If Deals

A user can enter a What-If deal by selecting the What If check box and clicking the Deal button. A What-If deal allows the user to simulate the impact of the deal on the positions, limits and P&L. Such deals are limited to the Front Office user and cannot be processed by the Back Office user.

Further, the system automatically reverses the What-If deals at COB on the booking date.

What-If deals are identified by the blue shade in the Blotter as shown in the screenshot below.


##### Foreign Exchange

TFO offers the deal capture functionality for the following Foreign Exchange (FX) deal types.

| Column 1 | Column 2 |
|---|---|
| Counterparty Limits |  |
| Dealer Limits |  |

| Counterparty |  |
|---|---|
| Known | Dealer can select the type as Counterparty and input the Counterparty name as mentioned above. Further, the Dealer can choose the Broker name from the Method field, which can enable the Broker Fee field for input. |
| Unknown | Dealer can select the counterparty type as Broker. The application displays all broker names in a drop-down list, from which the Dealer can select. These names are retrieved from the Temenos Transact BROKER table. It is mandatory to specify the Broker Fee. |

The TFO Limits tab on the deal capture screen is designed to display the availability and utilisation of Counterparty Credit Limits to enable real-time monitoring.

Enter the counterparty name in the Counterparty field and click the Credit Limits tab, to view the credit limit details of the counterparty. If the counterparty is changed in the Deal Capture screen, then click the Refresh icon in the Credit Limit tab to view the limit of the new counterparty.

The above screenshots show the live limits for the selected counterparty. Different limits are present according to the counterparty record.

The below screenshot shows that for every limit, the related limit application displays on the upper-left corner, while the limit currency on the upper-right corner.

> **⚠️ Note:** If the limit is not breached, the utilised amount is shown in green. If the limit is breached, it is shown in red.

This shows the ceiling amount in the defined limit currency on a counterparty. The system generates an override whenever the amount is exceeded by the limit outstanding for the currency.

This limit amount is displayed for each limit on the lower-left corner of the screen.

The system shows the actual utilisation of the limit in green. The user can enquire about the exact amount utilised by hovering the limit section.

The system provides information about the available amount, which is the difference between the limit amount and amount utilised. It is shown in the lower-right corner of the limit section.

If one or more limits are broken, the system warns the user by showing the limits in red.

In this case, the excess amount is demonstrated instead of the available amount.

Click the Dealer Limits tab to view the limit of the dealer selected. If the dealer is changed during the deal capture, then click Refresh in the Dealer Limits tab to view limits details of the new dealer.

- Select the Currency Pair , the limits widgets in the Dealer Limits are updated.
- An example of dealer limits displayed in the Deal Capture FX Spot screen.

> **⚠️ Note:** In case there is no dealer desk defaulted in FX screen while loading, the dealer desk attached to the user is considered for displaying the limits.

| Field | Description |
|---|---|
| Pay from A/C | Identifies which account (in the books) needs to be credited to settle the currency sold. On entering the counterparty and currency sold, the system displays the default account for the counterparty (if available). Otherwise, it uses the Nostro account. Input in this field is mandatory. To know more information, refer to help text of FX application in Temenos Transact . |
| Receive To A/C | Identifies which account (in the books) needs to be debited to the account for currency purchased. The defaulted account is based on SSI setup, which can be a customer, Nostro or Vostro account. However, the user can always override by typing or selecting from the drop-down list of the accounts present. Input in this field is mandatory. To know more, refer to help text of FX application in Temenos Transact . The system filters only the accounts with the same currency of the currency bought. |
| Counterparty SSI | Ensure to have the details of counterparty’s Nostro correspondent and account, when the settlement of the currency sold is done through a Nostro account. The system defaults this field when a record in AGENCY table is set for the Counterparty Customer ID along with their Nostro details. If not, it requires manual input except when the field Free Format address is used instead of this information. |
| Bank A/C Number | Holds the bank account number of the counterparty maintained with their correspondent. This information is used to send a payment message to the Nostro correspondent. Input in this drop-down field only accepts account number of the counterparty or beneficiary. |
| Free Format Address | Has the name in a free text format (maximum of 10 lines with up to 35 characters per line), when the counterparty’s correspondent bank does not have the customer ID. This information is then mapped to SWIFT confirmation and payment messages. |
| Bank To Bank Info | Provides instructions or additional information from the sending bank for the receiver. This field corresponds to Tag 72 on SWIFT messages and is not used for information for which another field is intended or instructions not required in a message. For contract confirmation using SWIFT mode, Bank to Bank information is mapped to Tag 72 of MT 300 and MT 600 messages. This field is used when the first multi-value has a code word followed by further information. All codewords need to be present on the SWIFT.CODE.WORDS file, and is enclosed between slashes ‘/’ at the beginning of the line. It allows a maximum of 6 lines of 35 characters (upper case alpha or numeric). |

| Field | Description |
|---|---|
| Agreement Type | Defines the contract's agreement type. The drop-down field displays all the valid records present in FX.AGREEMENT.TYPE table. This field is available for both spot and forward deals. |
| Revaluation Type | Identifies the revaluation method to be used on forward contracts. The system handles five types of revaluation, which are: RB – Rebate method SL – Straight line IN – Interest method IH – Interest/hedged SF – Straight line funding This field is available for forward and swap deals. For spot deals, the revaluation type applied is SP and hence not applicable. To know more information on the revaluation types, refer to the Temenos Transact user guide and help text. |
| Limit Reference | Has the limit reference number for the counterparty, which the system defaults. If the counterparty or customer has multiple limit references for the same product and sub-products, the user can manually provide the desired limit reference. To know more information on Limits and this field, refer to the Temenos Transact user guide and help text. |
| Buy Currency Interest Rate | Identifies the interest rate applicable to the currency purchased. This field is required when the revaluation type selected is other than RB. If the revaluation type is other than RB, the system defaults the interest rate from Periodic Rate table (for base currency) or derives the rate (for non-base currency) based on the forward rate and interest rate applicable to Sell Currency Interest Rate. Input is allowed in one of the two fields (that is, Buy or Sell currency interest rate) and not both. This field is available for forward and swap deals. To know more information on this field, refer to the Temenos Transact user guide and help text. |
| Sell Currency Interest Rate | Identifies the interest rate applicable to the currency sold. This field is required when the revaluation type selected is other than RB. If revaluation type is other than RB, the system defaults the interest rate from Periodic Rate table (for base currency) or derives the rate (for non-base currency) based on the forward rate and the interest rate applicable to buy Currency Interest Rate. Input is allowed in one of the two fields (that is, Buy or Sell currency interest rate) and not both. This field is available for forward and swap deals. To know more information on this field, refer to the Temenos Transact user guide and help text. |
| Mature at Start Of Day | Indicates whether maturity processing takes place at the Start of the Day. If this field is left blank, the maturity processing takes place at the End of the Day. The value in this field defaults from the Sod Mat field in FX.TRANSACTION TYPE (if setup). To know more information on this field, refer to the Temenos Transact user guide and help text. |
| Notes | Allows the Dealer to record any unique information or free-form narrative on the first level input, which is referred by the back office. These details benefit the back-office user or record purpose. The user is allowed to input a maximum of 10 lines with up to 35 characters per line. |

| Field | Description |
|---|---|
| Override | During the validation stage of an FX contract, the system provides the user with a series of screen override messages to indicate an anomaly. For example, the exchange rate varies by more than the variation tolerance predefined. |
| If the user confirms the override, the full text of the actual override message is stored for reference purposes only. |  |
| Record Status | Status of the record. Values are INAU, IHLD, INAO, RNAU and so on. |
| Current No | The number of times the record was edited. |
| Authori s er | The ID of the user who authorises the record. |
| Inputter | The ID of the user who inputs the record. |
| Date Time | Local zone date and time when the deal has been committed, according to the COMPANY table. |
| Company Code | Applicable company code on which the user is logged into. |
| Department Code | Defaults the user’s department code. |


##### Non-Deliverable Forward

A Non-Deliverable Forward (NDF) is classified as an event where a currency cannot be settled. The deal is fixed from a rate source arranged at the time of the original trade. When the rate is fixed on the valuation date, the settlement is the net settlement only for the deliverable currency. This is calculated by using the difference between the original FX rate and fixing rate.

Foreign Exchange NDF .

The following default screen appears.

| Field | Description |
|---|---|
| Counterparty | To know more, refer to Counterparty . |
| Exotic | ND DEAL application supports two types of NDF: Vanilla – A standard NDF transaction type with agreed rate and valuation date (usually two working days before settlement date). In this type, the user cannot change the valuation date. Exotic – A variation that allows the fixing date to be set at any date during the life of the transaction before the vanilla date. If the NDF is fixed and settled ‘early’, the fixing profit or loss is discounted. The discount amount is amortised from the settlement date to the value date of the NDF. The check box identifies the type of deal entered. In particular, the system always opens an NDF vanilla and provides opportunity to the user to switch the type of transaction to Exotic by selecting the checkbox. When Exotic is not selected, the valuation date is calculated automatically based on the days entered in Def Fix Days field in Temenos Transact ND.PARAMETER table. In this case, being a Vanilla NDF, the user cannot modify the valuation date. When Exotic is selected, the system automatically updates the other fields, making the valuation date an amendable deal. |
| Currency Pair | To know more, refer to Currency Pair . |
| Deal Currency | This identifies the NDF currency, which is configured in ND.PARAMETER table. To know more on the configuration of NDF currencies, refer to the NDF user guide in Temenos Transact . |
| Settlement Currency | This indicates the deliverable currency used for the settlement amount. |
| Buy or Sell | To know more, refer to Buy or Sell . |
| Amount Bought or Sold | To know more, refer to Amount Bought or Sold . |
| Value Date | To know more, refer to Value Date . |
| Live Rate | To know more, refer to Live Rate . |
| Contract Price | To know more, refer to Contract Price . |
| Settlement Rate Source | This allows the Dealer to enter up to two settlement rate sources from where the settlement rates are fixed on the valuation date. This is a drop-down field with all the valid records in ND.SETTL.RATE.SOURCE table. |
| Valuation Date | This defaults by the fixing date on which the exchange rate is fixed. The date defaulted or modified cannot be later than the value date. The system automatically defaults the date using the data from Fixing Days of the corresponding Fixing Currency from ND.PARAMETER table. In Vanilla deals, the defaulted value is not changeable. In particular, the system always defaults a date according to the above parameters compared with the settlement date. |
| Settlement Date | This indicates the settlement date of the NDF contract. The system automatically defaults the value date in this field. The user can modify the date defaulted by the system. However, the date entered needs to be greater than the deal date and not later than the value date. |
| Marketing Exchange | To know more, refer to Marketing Exchange . |
| Treasury Rate | To know more, refer to Treasury Rate . |
| Exchange Profit | To know more, refer to Exchange Profit . |
| Dealer | To know more, refer to Dealer . |
| Contract Date | To know more, refer to Contract Date . |
| Limits | To know more, refer to Limits . |

| Field | Description |
|---|---|
| Settlement Account | Indicates the settlement account. This is an account from which the settlement P&L amount is credited or debited.It is a drop-down field and the Dealer selects the required account. |
| Beneficiary | Used when the counterparty of the deal instructs to pay funds to another party who does not have an account with the bank. Entry in this field is accepted when the beneficiary is known to the bank (that is, it has a customer record for the beneficiary). |
| Counterparty Correspondent | Identifies the bank to which the counterparty wants to pay the settlement amount. This is either the bank of the counterparty or their nominated beneficiary. If the beneficiary is known to the bank (that is, a customer record exists), the customer number of the bank is entered in this field. If the beneficiary is not known, the details are entered in the Counterparty Correspondence Address field. |
| Counterparty Bank Account | Account number of the counterparty or nominated beneficiary at their correspondent bank. |
| Intermediary Bank | Identifies any intermediary bank involved in the transaction and is specified by the counterparty. If the intermediary is known (that is, there is an associated customer record), the customer number of the intermediary bank is entered in this field. If not, details are entered in the Intermediary Address field. |
| Receiver Bank | Receiver bank is the location where the funds are made available to the Receiver. |
| Counterparty Correspondence Address | Identifies the bank to which the counterparty wants to pay the settlement amount. This can either be the bank of the counterparty or their nominated beneficiary. If the bank is known (that is, a customer record exists), the details are entered in the Counterparty Correspondence No field. If the bank is not known, the address is entered in this multi-valued field, which has free-form text. |
| Bank to Bank Info | To know more, refer to Bank to Bank Info. |
| Beneficiary Address | Used when the counterparty of the deal directs to pay funds to another party who does not have an account with the bank. If the beneficiary is known to the Bank (that is, a customer record exists), the beneficiary details are entered in the Beneficiary No field. If the beneficiary is not known, the details are entered in this multi-value field, which has free-form text. |
| Intermediary Address | Identifies any intermediary bank involved in the transaction and is specified by the counterparty. If the intermediary is known to the bank (that is, an associated customer record exists), the customer number of the intermediary bank is entered in the Intermed Bk No field. If not, the details are entered in this field, which has free-form text. |
| Payment Narrative | Allows the user to enter free text narrative, which appears on payments related to the deal record. |
| Notes | To know more, refer to Notes. |
| Audit | To know more, refer to Audit . |


##### Money Market

Money Market .

| Field | Description |
|---|---|
| Currency | Currency information in which the MM deal is booked. ISO codes are used to standardise the structure of these records (that is, GBP, USD, AUD). Currency is a drop-down field. When the user clicks the currency field, all the existing records in CURRENCY is automatically listed in the dropdown. From here on, the user can select the desired record by clicking on the value. |
| Amount | Deal amount |
| Counterparty | Counterparty with whom the deal is made. Counterparty is an opposite party in a contract or financial transaction. A record needs to exist in the Temenos Transact CUSTOMER file. Any counterparty available on the Customer file is accepted. The customer record can be entered as a number or mnemonic. The liability number assigned to this counterparty in the customer file is used for the limit checking. The dealer can search for a counterparty by prefixing 'sn' (short name) or 'mn' (Mnemonic) with the search text which instantaneously performs a quick search for Counterparty Name, Short Name, or Mnemonic. The dealer can also search for a counterparty based on Counterparty ID. The below screenshots show the result of counterparty search with ‘mn’ and ‘sn’ as prefix followed by four letters. |
| Interest Rate and Margin | Interest rate related information of the MM deals. Type of interest rate can either be Fixed or Floating depending on the type of the contract. Rate is valid from the start of the current interest period or value date, for fixed maturity contracts and call or notice contracts. |
| Fixed Interest Rate | Fixed-rate to calculate the interest accrual, interest credit or debit from the counterparty. It is entered as a direct interest percentage: On the contract or as a fixed interest key mapped to PERIODIC.INTEREST table in Temenos Transact . Is inclusive of the margin, thus, the Margin field is not enabled for user inputs. If entered using a rate key, the user needs to specify the Margin (if required). The key can be entered as a valid PERIODIC.INTEREST record or selected from the drop-down list. It takes the rate automatically on selecting a valid PERIODIC.INTEREST key. |
| Floating Interest Rate | Floating rate at which the interest accrual, interest credit or debit from the counter are calculated. It is entered as an interest key, mapped to BASIC.INTEREST table or RFR record in PERIODIC.INTEREST table of Temenos Transact. If entered using a rate key, the margin needs to be specified (if required). The key can be entered as a valid rate key or selected from the drop-down list. The Total Interest field calculates the interest, on selecting a valid BASIC.INTEREST or RFR key. |
| Interest Schedule | Identifies the associated frequency of interest payment. The frequency of payments are as follows: Bullet Daily Weekly Fortnightly Monthly Quarterly Half-Yearly Yearly If it is defined as part of the EB.FREQUENCY table, the custom frequency needs to be entered. Bullet type of schedule is not available for call or notice maturity deals. |
| Interest Start Date | Start date of the current interest period. The user can input a value in this field, only when the value in the Interest Schedule field is not ‘Bullet’. |
| Negative Interest | Determines whether the interest rate can be negative. If the value is set as Yes, it enables the user to enter the negative interest rate. If set as No, the user is not allowed to enter any value. |
| Interest Basis | Describes the total interest computation. Special Interest Basis is available only for fixed maturity contracts. To know how to create a new interest basis or assign interest basis for the special category, refer to the Temenos Transact user guide. |
| Total Interest | Total amount of interest that the system calculates, when value date, principal amount, interest rate, period and day basis are given. |
| Method | Methods to book a deal. The deal can have a valid Broker Code (records available on the BROKER table of Temenos Transact ) or other methods (such as telex, Reuters, telephone) available on FX.DEAL.METHOD table of Temenos Transact . If the Broker is selected as the deal method, fields (such as brokerage currency and brokerage fees) are enabled for user input. |
| Broker Fee | Amount of brokerage paid to the broker account specified in the broker currency in BROKER table in Temenos Transact . The user can specify the flat amount to be credited to the broker account. This field is displayed only when the Broker is selected in the Counterparty drop-down list or Broker Name from the Method field. The Broker Fee currency highlighted is listed based on the currency specified in the CCY.FOR.PAYMENT in the Temenos Transact Broker record. The user can input any amount in a valid format for the currency specified above. |
| Dealer | Dealer desk position that needs to be updated by the deal being created. The dealer desk code is held on the position record, hence, the exchange position and PL can be shown at the dealer desk level. The logged-on user is assigned to a dealer desk, which is defaulted in this field. However, it can be modified. The user can click the star on the left of the dealer desk name to add items to the Favourites. To remove the item from the Favourites, the user can re-click the highlighted star. |
| Contract Date | Deal date of the contract that represents the agreed date between all the parties to the contract. This is usually the system date, and backdate value is allowed without an override. However, the system does not accept the forward contract date value during the input of the deal. |
| RF Rate | Stores the compounded Risk-Free Rate. This is a system updated field. |
| RFR Convention | Market convention for rate compounding or averaging. The MM application follows Lookback methodology. |
| RFR Lookback Type | Type of Lookback method applied for rate compounding or averaging. It has the following methods for rate calculation: Narrow Definition - Uses the original interest period day count with lookback For example, if Wednesday rate is used for Friday, apply the Friday’s weight (three days) to the Wednesday’s rate. Observation Shift - Uses the original day count of the lookback rate. For example, if Wednesday rate is used for Friday, apply the Wednesday’s weight (one day) to the Wednesday’s rate. |
| RFR Lookback Days | Number of Lookback days considered for RFR calculations. |

The functionality of the Limits tab is similar to the FX Deal Capture screens.

- Select the Place or Take and Currency, product limits are updated for the selected currency.
- An example of dealer limits displayed in the Deal Capture MM screen.
- Click on the Credit Limits tab to view the credit limit details of the counterparty. If a counterparty is changed during deal capture, then click on the refresh icon in the Credit limits section to view the limit of the new counterparty

> **⚠️ Note:** In case there is no dealer desk defaulted in MM screen while loading, the dealer desk attached to the user is considered for displaying the limits.

| Field | Description |
|---|---|
| Counterparty Reference | Reference number that a customer specifies for the Place or Take. This field can be used as an input to be printed on all Advice and Confirmations (along with the Bank’s contract number). Hence, so long as the delivery mapping and formatting tables are set up to use this field as input on Temenos Transact . |
| Credit Account | Helps to identify the account number ( source or destination account) to which the drawdown amount is settled on the value date. |
| Counterparty Correspondent Bank | Identifies the beneficiary bank that is used to settle one of the following when the counterparty has requested external delivery of the proceeds of the transaction: The principal amount of taking contract types at maturity Placement contract types at drawdown This is used when the counterparty does not require the funds to be credited in the current account, instead of requests an external delivery of the funds to a bank different from where the Nostro account is maintained. |
| Counterparty Correspondent Address | Full name and address of a beneficiary bank, along with the Principal Amount, where no account details are maintained. |
| Beneficiary Account | Account details (Name or the Number) of the beneficiary to which the principal amount needs to be credited. It has third-party transfers, where the counterparty requests for external delivery of funds. If the counterparty provides such information, it is entered in this field. Any amendment to this field after contract authorisation is displayed on future principal disbursements. |
| Bank to Bank Info | Provides instruction or additional information from sending bank for the receiver or intermediary account with institution or beneficiary institution. It corresponds to the 72 fields on SWIFT messages, and cannot be used for information for which another field is intended, or instructions are not required in a message. If a user inputs any details, it is sent to the Receiver. Even after authorisation, this field can be amended. The input is used for future confirmations and payments. If the amount is sent to re-generated, it does not perform any payments. |
| Send Payment Message | Controls whether to send or suppress the Swift messages (MT202 and MT210), after authorisation of the deal. |
| Principal Liquidation Account | Identifies the account number to which the entries are made for the reimbursement of the principal at liquidation or maturity date. |
| Interest Liquidation Account | Identifies the account number to which the entries are made for the reimbursement of the interest of deposit type contracts. The input is necessary when the disposal of the interest account is different from the disposal of the principal account. |

| Field | Description |
|---|---|
| Debit Account | Account number to which the debits are passed, to collect charges at drawdown date. It needs to be expressed in the currency of the contract. Thus, the liquidation account for the interest can also be expressed in the currency of the contract. |
| Code | Specifies the Profit and Loss category code (available as a record within Temenos Transact FT.CHARGE.TYPE or FT.COMMISSION.TYPE tables) where the amount of the charges, collected at drawdown, is credited. The charges can be handling fees, documentary tax stamps, drawdown fees, legal fees, and so on which are collected from the client directly on the drawdown date. |
| Amount | Identifies the flat amount of charges that need to be debited to the counterparty at the drawdown of the contract or when the principal is increased. The charges amount is defined in the currency of the contract. |

| Field | Description |
|---|---|
| Product Category | Allows the user to amend the product category code according to the requirement. |
| Mature at Start of the Day | Specifies whether the deal matures at the Start of Day (SOD). |
| RFR Calc Method | Calculation method for RFR averaging: Compound Simple |
| RFR Spread Treatment | Spread treatment method during RFR averaging: Spread-Inclusive - Uses the spread within the averaging calculation along with daily rates. Spread-Exclusive - Adds the spread separately after RFR averaging is done. |

This section is for audit purpose only. It is consistent across all Deal Capture screens.

The user can access the ‘MM Events to Date’ on a particular Deal Details screen of MM deal.

This displays a series of events that the MM contract undergoes, such as contract initiation, amendments, contract maturity and rollovers. A dealer on viewing the Events to Date tab can understand the different events that the contract has undergone and the related contractual information, payment and receipt entries. Additionally, the user can view various events related to the deal on the Events to Date tab.

TFO offers the deal capture functionality for the following MM deal types:

The user can click a specific event view the detailed event information on the subsequent screen.

This tab enables the user to view the progress of the contract.

To know more information on the view, refer to the MM.ETD enquiry in Temenos Transact .

| Field | Description |
|---|---|
| Currency | To know more, refer to Currency. |
| Amount | To know more, refer to Amount. |
| Counterparty | To know more, refer to Counterparty. |
| Interest Rate and Margin | To know more, refer to Interest Rate and Margin. |
| Interest Accrual and Maturity | On Fixed Maturity deals, the From field has the value date of the contract from which the system starts to accrue the interest. To know more information, refer to the Start Date user guide in Temenos Transact . The To field has the maturity date of the deal. |
| Interest Schedule | To know more, refer to Interest Schedule. |
| Interest Start Date | To know more, refer to Interest Start Date. |
| Negative Interest | To know more, refer to Negative Interest. |
| Capitalise Interest | This is part of Others tab as shown below: This indicates the requirement for automatic capitalisation of interest on interest due dates. If the value is selected as Yes, the system updates the principal amount automatically with the full amount of interest, and capitalisation continues until the final maturity date is reached. If the value is No, the capitalisation of interest is not allowed. |
| Interest Basis | To know more, refer to Interest Basis. |
| Total Interest | To know more, refer to Total Interest. |
| Method | To know more, refer to Method. |
| Broker Fee | To know more, refer to Broker Fee. |
| Dealer | To know more, refer to Dealer. |
| Contract Date | To know more, refer to Contract Date. |
| Limits | To know more, refer to Limits. |
| Settlement | To know more, refer to Settlement. |
| Charge | To know more, refer to Charge. |
| Other | To know more, refer to Other. |
| Audit | To know more, refer to Audit. |

| Field | Description |
|---|---|
| Currency | To know more, refer to Currency. |
| Amount | To know more, refer to Amount. |
| Counterparty | To know more, refer to Counterparty. |
| Interest Rate and Margin | To know more, refer to Interest Rate and Margin. |
| Interest Accrual and Maturity | In Call or Notice deals: The From field has the value date of the contract from which the system starts to accrue the interest. To know more information, refer to Start Date in the Temenos Transact user guide. The To field on call or notice deals has the maturity date of the deal. However, the user is specifically provided with an option to drill-down by Call or Notice type based on the deal type. On selecting a Call, the user cannot input a maturity date, whereas if it is a Notice deal, the user can input between 1 - 999 days. |

| Field | Description |
|---|---|
| Interest Schedule | To know more, refer to Interest Schedule. |
| Interest Start Date | To know more, refer to Interest Start Date. |
| Negative Interest | To know more, refer to Negative Interest. |
| Capitalise Interest | This is applicable for all the call or notice deals on the main Deal Details screen. The capitalisation of interest is not allowed when the negative interest rate is selected for the contract. |
| Liquidate Interest | The system requirement is that interest due date is specified for all call or notice contracts and Liquidate Interest field is applicable for all call or notice deals. This states whether interest is liquidated or deferred at the interest due date.\| The Interest fields control when the interest is due and whether the interest accrued is paid, received or not paid on this date. If the field is set to No, the system does not liquidate the interest on the due date but creates a new interest due date according to the input on Interest Schedule field. If set to Yes, the amount of interest is retained within the contract and liquidated on the next interest due date. |
| Interest Basis | To know more, refer to Interest Basis. |
| Total Interest | To know more, refer to Total Interest. |
| Method | To know more, refer to Method. |
| Broker Fee | To know more, refer to Broker Fee. |
| Dealer | To know more, refer to Dealer. |
| Contract Date | To know more, refer to Contract Date. |

| Field | Description |
|---|---|
| Auto Rollover | The contract is rolled automatically on its maturity date. A rollover happens indefinitely unless the rollover details are cleared to allow the contract to mature on the defined date or date entered in the Final Maturity Date field (which holds the last rollover period). |
| Auto Capitalise Interest | The contract is rolled to capitalise (add to the Principal) the interest. |
| Auto Rollover Term | The period for which the contract can be rolled over. The term can be expressed as a number of days, weeks or months, and system validation is applicable to check whether the date returned is a working day. |
| Rollover Interest Rate | The new interest rate applicable when the contract is rolled over on the auto-rollover term. If the field is left blank, it defaults the interest rate from the existing contract. |
| Final Maturity Date | The final maturity date for a fixed-term contract subject to Auto Rollover Term. If the contract is set for Auto Rollover, the date needs to be greater than the maturity date. On reaching the final maturity date, the contract stops automatically roll over and matures. The rollover advice is inhibited for each maturity subject to Auto Rollover Term , and the Final Maturity can be further extended (if required). |
| Charge | To know more, refer to Charge. |
| Other | To know more, refer to Other. |
| Audit | To know more, refer to Audit. |


##### Forward Rate Agreement

Forward Rate Agreement .

The layout of the FRA Deal Capture screen.

| Field | Description |
|---|---|
| FRA Type | Specifies the underlying strategy of the FRA transaction. The two main types, that is Hedge and Trade, are decided based on the respective accounting treatment, exposure to interest rate risk and revaluation of positions. The field value is selected as Trade, by default. |
| Buy Sell | Specifies whether it is a Buy or Sell FRA. The field value is selected as Buy, by default. |
| FRA Currency | Currency code in which the FRA deal is booked. ISO codes are used to standardise the structure of these records (that is, GBP, USD, AUD and so on). The user can choose from the existing records in CURRENCY by clicking the records in the list. |
| FRA Amount | FRA amount of the contract. |
| Counterparty | Counterparty of the deal. The counterparty is an opposite party in a contract or financial transaction and a record needs to be available in the Temenos Transact customer file. The customer record can be entered as a number or mnemonic. The liability number assigned to this counterparty in the customer file is used for checking the limits. The dealer can search for a counterparty by prefixing 'sn' (short name) or 'mn' (Mnemonic) with the search text which instantaneously performs a quick search for Counterparty Name, Short Name, or Mnemonic. The dealer can also search for counterparty based on Counterparty ID. The below screenshots show the result of counterparty search with ‘mn’ and ‘sn’ as prefix followed by four letters. |
| FRA Rate | Future fixed the interest rate on the notional FRA Principal. It is set at the time of the FRA transaction. |
| Agreement Type | Defines the FRA deal. This is a mandatory field. |
| Marketing Exchange | Specifies whether the customer is a treasury customer or not. Selecting this field states that the customer is a non-treasury customer. It also displays Treasury Rate and Exchange Profit fields in the FRA Deal Capture screen for user input. |
| FRA Period, Start Date and Maturity Date | Two drop-down fields with the start and maturity periods of the FRA contract. The value in the Start Date field can be 0 to 98 months and Maturity Date field is 1 to 99 months. The Start Date field updates the value based on the selection in the first box, similarly, the Maturity Date updates the contract’s maturity date based on the selection on the second box. The field when updated calculates the spot date and adds up the period specified to get both Start and Maturity Dates. |
| Reference Rate | The variance allowed is selected in the PERIODIC.INTEREST table. This reference rate needs to be a valid record in the table for the currency selected. |
| Fixing Date | Specifies the date on which the prevailing interest rate is determined. Transactions happen for: Foreign currency two days prior to the start date The local currency on the same day |
| No. of Days | Indicates the number of days between Start Date and Maturity Date. This is a no-input field. |
| Reference Price | Represents the interest rate on the cash market applicable to the longest period of the FRA. It is applicable only for hedge type of contracts and the rate input is selected in PERIODIC.INTEREST table. |
| Treasury Rate | Applicable only when the Marketing Exchange field is selected. The text box field specifies the rate in case the customer is not a treasury customer. |
| Exchange Profit | Marketing exchange profit or loss amount is calculated on the contract date for a non-treasury customer. This field is displayed only when the Marketing Exchange field is selected in the contract. This is a no input field. |
| Method | Methods using which a deal can be booked. The deal can have a valid broker code (records available on the BROKER table of Temenos Transact ) or other methods available in FX.DEAL.METHOD table of Temenos Transact , such as Telex, Reuters, Telephone and so on. |
| Broker Currency and Broker Fees | These fields are updated when the Method is selected as Brokerage. Broker Currency is a drop-down field whereas Broker Fees is a text box for manual input. |
| Dealer | This identifies the dealer desk associated with the contract. |
| Contract Date | This specifies the deal or trade date of the contract. |

The functionality of this tab is similar to the Forex Deal Capture screens.

| Field | Description |
|---|---|
| Receive To A/C | Account from which the settlement profit amount is received. The settlement account needs to match the currency of the contract. |
| Pay from A/C | Account from which the settlement loss amount is paid. The settlement account needs to match the currency of the contract. |
| Cpty Bank 1 | Counterparty bank where the payment of the settlement amount is made. Additionally, the customer requests for external delivery of funds and does not require it to be credited to the current account. |
| Cpty Bank 2 | Counterparty reference of the second beneficiary bank for the settlement amount. It is used where contracts involve four-party transfers of funds. |
| Beneficiary Address | Full name and address of a beneficiary bank along with the settlement amount, where no settlement details are maintained for the beneficiary account. |

| Field | Description |
|---|---|
| Portfolio | Portfolio number to which the FRA contract is linked. It links the deal to the customer portfolios for overall management. |
| Business Centre | Business centres of the contract. |
| Position | Applicable for all trade buy and sell contracts, and not for hedge contracts. It specifies whether the contract is entered to open (create) a new FRA position or close an existing open FRA position. |
| Limit Reference | Limit reference applicable to the FRA transaction. |
| Mature at Start of the Day | Specifies whether the deal matures at the Start of the Day. |

This is a read-only tab holds all the audit details for the executed trade, which is used for audit purpose. The tab is consistent across all the Deal Capture screens.


##### Interest Rate Swap

Interest Rate Swap ,

Layout of IRS Deal Capture screen.

| Field | Description |
|---|---|
| Swap Type | Type of swap Two main type includes Interest Rate Swap and Currency Interest Rate Swap, which decide the nature of the principal used, interest repayment obligation and so on. |
| Trade Type | Essential strategy of the swap transaction Two main types include Hedge and Trade, which decide the respective accounting treatment, exposure to interest rate risk and revaluation of positions. If the Swap Type is selected as Cirson, the Trade Type field automatically defaults to Hedge. |
| Marketing Exchange | Specifies whether the customer is a treasury customer Click the treasury rate fields to select both the legs of the Swap Deal Capture screen for user input. This is a non-mandatory field. |
| Start Date | Starting date of the swap contract Value date from which the system starts to accrue interest. Therefore, the date entered needs to be prior to the maturity date of the contract. |
| Maturity Date | Termination date of the swap contract and the date when the deal is liquidated During liquidation, all the corresponding amounts of principal (if appropriate) and interest passes to the appropriate accounts as designated within the transaction. |
| Agreement Type | Swap deal agreement type |
| Principal Exchange | Specifies if the deal involves principal exchange and triggers the Principal Exchange (PX) and Principal Re-Exchange (RX) schedules within the swap contract. |
| Portfolio | Portfolio number to which the swap contract is linked |
| Dealer | Dealer desk associated with the contract |
| Contract Date | Deal or trade date of the contract |


##### Securities Deal Capture

Bond /Equity .

TFO offers the deal capture functionality to record the securities deal and categorise it based on the type of asset class (Bond or Equity).

| Field | Description |
|---|---|
| Counterparty/Broker | Indicates trade is done with a counterparty or broker. This field filters the list of counterparties or only brokers based on the selection The dealer has an option to search for a counterparty by prefixing ‘sn’ (short name) or ‘mn’ (Mnemonic) with the search text which instantaneously performs a quick search for Counterparty Name, Short Name or Mnemonic. The dealer can also search for a counterparty based on the Counterparty ID. The below screenshots are an example of a counterparty search with ‘mn’ and ‘sn’ as prefix followed by four letters. |
| Counterparty/Broker Selection | Represents the Counterparty or Broker of the trade. Counterparty is a customer with whom the bank makes the contract. A valid record is on the Temenos Transact CUSTOMER.SECURITY file with the classification of the customer as Counterparty, Broker or Both. The dealer can search for a Counterparty or Broker by typing the Short Name and it does a text-based search for Counterparty/Broker Name, Short Name, Country Name or Counterparty/Broker Number. |
| Portfolio | The portfolio number or security account to which the security trade is linked. A valid record is available on the Temenos Transact SEC.ACC.MASTER application. The dealer can directly search for a portfolio by entering the Short Name or Portfolio Number. The dealer is directed to the portfolio inventory screen to view the portfolio holdings and valuation of the selected portfolios, on clicking the ellipsis icon (marked in brown) available next to the drop-down. |
| Side | This indicates whether the dealer buys or sells the security. |
| Security | Drop-down for bond selection to which the dealer has traded. A valid record is available on the Temenos Transact SECURITY.MASTER application with the classification as Bond. The dealer can search for a security by entering the Short Name or Security Number, ISIN, Sub Asset Type, Stock Exchange, cusipNumber and sedolNumber. The search is prefixed by ISIN, ST, EX, CUSIP or SEDOL. For example, to search for security using ISIN, the dealer must enter ISIN US0378331005. Dealer can view details of the security in the same deal capture window, click the first ellipsis icon (marked in brown) available next to the drop-down. Dealer is directed to the security inventory screen to view the security holdings and valuation across all the own book portfolios, click the second ellipsis icon (marked in brown). |
| Stock Exchange | Value defaults on selecting the security from the SECURITY.MASTER application. The value date and the charges and commissions for the trade are calculated based on the setup done in STOCK.EXCHANGE application. Dealer can change defaulted stock exchange at the trade level. |
| Trade Currency | The currency in which the transaction is dealt with the Broker or Counterparty concerned or the trade is settled. After security selection, the value defaults as the security currency from the SECURITY.MASTER application. |
| Nominal | Nominal amount (that is, the face value) of the security traded. |
| Price | The price at which the nominal is bought or sold. After security selection, the value defaults from the SECURITY.MASTER application. Dealer can change the defaulted price at the trade level. |
| Trade Date | This records the trade date. |
| Settlement Date | This records the date on which the settlement of the trade executed. Value defaults based on the setup available in STOCK.EXCHANGE application. |
| Interest Days | Number of days for which interest is accrued (from last payment date to settlement date) |
| Accrued Interest | Amount of interest accrued on the securities up to the settlement date. |
| Gross Amount | The gross value of the trade in trade currency terms. After entering the nominal and price, the system calculates the gross amount. To know more information on the calculation of the gross amount, refer to the Temenos Transact user guide. |
| Net Amount | The net value of the trade in trade currency terms. After entering the nominal and price, the system calculates the net amount. To know more information on the calculation of the gross amount, refer to the Temenos Transact user guide. |

| Field | Description |
|---|---|
| Counterparty or Broker | Indicates trade is done with a counterparty or broker. This field filters the list of counterparties or only brokers based on the selection. The dealer has an option to search for a counterparty by prefixing ‘sn’ (short name) or ‘mn’ (Mnemonic) with the search text which instantaneously performs a quick search for Counterparty Name, Short Name or Mnemonic. The dealer can also search for a counterparty based on the Counterparty ID. The below screenshots are an example of a counterparty search with ‘mn’ and ‘sn’ as prefix followed by four letters. |
| Counterparty or Broker Selection | Counterparty or broker of the trade. Counterparty is a customer with whom the bank makes the contract. A valid record is available on the Temenos Transact CUSTOMER.SECURITY file with the classification of the customer as Counterparty or Broker or Both. Dealer can search for a Counterparty or Broker by typing Short Name and it does a text-based search for Counterparty or Broker Name, Short Name, Country Name or Counterparty or Broker Number. |
| Portfolio | Portfolio number or security account to which the security trade is linked. A valid record is available on the Temenos Transact SEC.ACC.MASTER application. Dealer can directly search for a portfolio by entering the Short Name or Portfolio Number. Dealer is directed to the Portfolio Inventory screen to view the portfolio holdings and valuation of the selected portfolio, when clicking the ellipsis icon (marked in brown) available next to the drop-down. |
| Side | The dealer buys or sells the security. |
| Security | This helps to select the equity, which the Dealer has traded. A valid record is available on the Temenos Transact SECURITY.MASTER application with the classification as Share. The dealer can search for a security by entering the Short Name or Security Number, ISIN, Sub Asset Type, Stock Exchange, cusipNumber and sedolNumber. The search is prefixed using ISIN, ST, EX, CUSIP or SEDOL. For example, to search for security using ISIN, the dealer must enter ISIN US0378331005. Dealer can view details of the security in the same deal capture by clicking the first ellipsis icon available next to the drop-down. Dealer can view the security holdings and valuation across all the own book portfolios by clicking the second ellipsis icon. |
| Stock Exchange | Defaults on selecting the security from the SECURITY.MASTER application. The value date and the charges and commissions for the trade are calculated based on the setup in STOCK.EXCHANGE application. Dealer can change defaulted stock exchange at the trade level. |
| Trade Currency | Currency in which the transaction is dealt with the Broker or Counterparty concerned and trade is settled. After security selection, the value defaults as the security currency from the SECURITY.MASTER application. |
| Nominal | Nominal amount (that is the face value) of the security traded. |
| Price | Price at which the nominal is bought or sold. After security selection, the value defaults from the SECURITY.MASTER application. Dealer can change the defaulted price at the trade level. |
| Trade Date | Records the trade date. |
| Settlement Date | The date on which the settlement of the trade is executed. Value defaults based on the setup available in STOCK.EXCHANGE application. |
| Gross Amount | The gross value of the trade in trade currency terms. After entering the nominal and price, the system calculates the gross amount. To know more information on the calculation of the gross amount, refer to the Temenos Transact user guide. |
| Net Amount | The net value of the trade in trade currency terms. After entering the nominal and price, the system calculates the net amount. To know more information on the calculation of the net amount, refer to the Temenos Transact user guide |

This section represents a sub-menu to display Blotter and Mark-to-Market information for quick reference. This is referred to as mini blotter and a short representation of the main blotter.

This quick reference feature allows the user to view or copy a deal without navigating to the actual blotter.

The below section displays a limited number of recently input deals, irrespective of the deal status for quick reference. A user can also do the following with the data representation.

A user can classify the listing of deals as:

- All – All the recent input deals regardless of the user who inputs the deal.
- My – All the deals input by the specific logged on user.

- To perform a manual refresh of the Mini Blotter section, click the Refresh button.

> **⚠️ Note:** The system can automatically refresh the blotter at regular intervals, as defined in the system settings.Hence, there is no need to click the Refresh button for manual refresh.

To know more, refer to Blotter user guide.

The count of transactions available on the right of the Refresh button also undergoes a refresh each time along with the Blotter.

The Mini Blotter lists all the deals committed to ascending order of period (from the most recent input deal to the oldest). The user can perform the following actions:

- To open the record as shown below, select and then click the required deal.

> **⚠️ Note:** The user can to view the deal information or take a few actions on the deal according to the requirement. To know more information, refer to Post Deal Capture Actions section. Additionally, download the record in different formats. To know more, refer to the Blotter section.

This section describes the features, such as Deal Capture , View , Delete , Amend , Authorise and Reversal of a deal.

The below screenshot illustrates how to view a deal and capture it in the Deal Capture screen.

- To capture the deal and create a record as a line item on the Blotter and Mini Blotter, click the Deal button.

The following set of deal actions appear for the unauthorised deals (STATUS= INAU) when selected from the Mini B lotter .

- To open a record on the Deal Capture screen, click the View button.

> **⚠️ Note:** This button allows the user to view but not modify the deal. Hence, it is for information purpose only.

The below is an illustration of the feature.

The user performs the following:

- To replicate all the information of the selected deal to a new record, click the Copy button. A new record opens in the Deal Capture screen (with the header as ‘Copy Of the Selected Deal’) pre-filled with all the information provided on the already selected deal.

> **⚠️ Note:** Before committing the deal, the user can modify the details.

The below is an illustration of the Copy feature.

A copy of the selected deal (as highlighted in the header) is available on the upper-left of the screen.

This function allows the user to delete a committed record.

> **⚠️ Note:** This function is available only for those deals, which are not in the live table (authorised).

1. To delete a deal, click Delete button. The system displays the record and the message appears seeking confirmation, as seen below.
2. Click Confirm . The system permanently deletes the record and removes the deal from the Mini Blotter.

TFO allows the user to modify the fields that are in unauthorised status. The contractual level information of the deal can be modified, whereas information, such as deal type, deal currency and so on are greyed out from user modification. At this stage, a user can rely only on the reversal of deal when the deal is created by mistake. A privileged user needs to authorise the modification before it is moved to the live table.

An illustration of Amend feature is given below:

1. Click the Amend button of the deal, which is in INAU status. The record opens for modification.
2. To enable the Amend button to Commitment, do the required changes in the fields.

TFO allows the user to authorise all the unauthorised records from Blotter or Mini Blotter section.

An illustration of the feature is given below.

1. Click the Auth button on any of the unauthorised deals. The record opens for authorisation.
2. Click the Authorise button.
3. After authorisation, the deal moves to the live file.

> **⚠️ Note:** Does not allow self-authorisation (that is, the same user who inputs the deal cannot authorise the record for audit purpose). A different user (who has the privilege to authorise, as defined in the User table) needs to authorise to avoid INAU status. The error message appears on the screen when the user attempts self-authorisation on the deal.

The buttons applicable for the authorised deals are different from unauthorised records.

> **⚠️ Note:** The View, Amend and Copy deal are discussed above. However, amendment of unauthorised deals is different from amendments of authorised deals, as given below.

TFO allows the user to modify only selective fields on all the committed records in comparison to most fields on all unauthorised deals, for audit reasons.

An illustration of the feature is given below.

The no-change fields differ for the different product type and are greyed out from user modification.

- To amend the authorised record, click the Amend button.

The Amend screen is displayed.

> **⚠️ Note:** After modification, a different privileged user needs to authorise the record.

This allows the user to reverse an authorised deal and send it to the HISTORY table.

> **⚠️ Note:** This function is not available for deals that are not in the live table.

1. On the bottom-right corner of the deal, click the Reverse button.
2. On the Reverse screen displayed, to confirm the reverse action, click the Reverse button.

The record is moved to RNAU status.


##### REPO Deal Capture

Repurchase Agreement .

Layout of REPO Deal Capture screen.

| Field | Description |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| Deal Type | Characteristics of a REPO contract. The value entered determines whether the contract is REPO or reverse REPO. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Counterparty | Counterparty with whom the deal is made. A valid record needs to exist in the Temenos Transact customer file. The customer record can be entered as a number or mnemonic. The liability number assigned to this counterparty in the customer file is used for the limit checking. The Dealer has the option to search for a counterparty by prefixing 'sn' (short name) or 'mn' (Mnemonic) with the search text which instantaneously performs a quick search for Counterparty Name, Short Name or Mnemonic. The dealer can also search for the counterparty based on the Counterparty ID. The below screenshots show the result of the counterparty search with ‘mn’ and ‘sn’ as prefixes followed by four letters. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Own Book | Portfolio number to which the REPO trade is linked. A valid record needs to exist in the Temenos Transact SEC.ACC.MASTER application. The Dealer can perform the following: Search for a portfolio by entering the short name or portfolio number. Click the ellipsis icon next to the drop-down, to view the portfolio holdings and valuation of the selected portfolio in the Portfolio Inventory screen. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Trade Date | The date on which the trade is made. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Txn Type | Specifies whether the deal is cash or security-driven. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Currency | Currency in which the REPO deal is booked. The user can choose from the existing records in CURRENCY by clicking the records in the list. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Interest Basis | Basis considered for total interest computation. The basis can be given as follows: Fixed Term Call - Notice 360/360 360/360 366/360 366/360 366/365 366/365 365/365 365/365 252/252 252/252 21/252 21/252 360/365 360/365 SPECIAL - Special Interest Basis is available only for fixed interest rate contracts. To create a new or assign an Interest Basis for the Special category, refer to Temenos Transact user guide. | Fixed Term | Call - Notice | 360/360 | 360/360 | 366/360 | 366/360 | 366/365 | 366/365 | 365/365 | 365/365 | 252/252 | 252/252 | 21/252 | 21/252 | 360/365 | 360/365 | SPECIAL | - |
| Fixed Term | Call - Notice |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 360/360 | 360/360 |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 366/360 | 366/360 |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 366/365 | 366/365 |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 365/365 | 365/365 |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 252/252 | 252/252 |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 21/252 | 21/252 |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 360/365 | 360/365 |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| SPECIAL | - |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Agreement | Agreement type for the contract. This is applicable for both legs of Repo or Reverse Repo. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Issue Date | The date on which the trade is to be effected. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Issue Amount | Price for the first leg of the REPO contract, specified in the Currency field. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Repurchase Date | The date on which the Repo contract matures. The securities return to the Seller and Buyer receives the repurchase amount specified in the contract on this date. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Repurchase Amount | Price for the second leg of repo contract. If the value is not entered, it populates from Temenos Transact after validation. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Rate Type | Specifies whether the contract is a fixed or floating rate contract. The other related fields are no input field as shown in the below screenshots based on the Rate Type field. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Repo Rate | Rate of interest for the REPO contract. Applicable for fixed REPO contracts. In the case of floating rate REPOs, the total interest is displayed after validation and the same is made as no input field. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Rate Key Floating | Rate of interest for the REPO contract. Applicable for floating rate REPO contract. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Interest Term | Period or frequency to re-fix the REPO contract. Available as the number of days, weeks or months. Applicable for floating rate REPO contract. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Interest Spread | Spread associated to calculate the overall interest rate of the REPO contract. Applicable for floating rate REPO contract. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Rate Selection | Determines whether the rate is BID or OFFER from the Temenos Transact PERIODIC.INTEREST table. Applicable for floating rate REPO contract. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Next Fixing Date | The date on which the next rate change is applicable to the contract. Applicable for floating rate REPO contract. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |


##### Derivatives Deal Capture

- FXOTC Trade . The Derivatives Deal Capture – FX OTC screen is displayed.
- Exchange Traded Derivatives . The Derivatives Deal Capture – ETD screen is displayed.


##### Generic Deal Capture Actions

The following are the generic features in deal capture.

This section represents a sub-menu to display Blotter and Mark to Market information for quick reference. This is referred to as mini blotter and is a short representation of the main blotter.

This feature allows the user to view or copy a deal without navigating to the actual blotter.

The below section displays a limited number of recently inputted deals, regardless of its deal status for the user to have a quick reference. A user can also do the following with the data representation.

A user can classify the listing of deals as:

- All – Deals entered recently, regardless of the user who inputs the deal.
- My – Deals entered by the logged-on user.

To refresh the Mini Blotter section (manually), click the Refresh button.

> **⚠️ Note:** The system can automatically refresh the blotter at regular intervals, as defined in the system settings. To know more, refer to Blotter user guide. The count of transactions on the right of the Refresh button undergoes a refresh along with the blotter.

Mini Blotter lists all the deals committed to ascending order of period, that is, from the most recent input deal to the oldest. The user can perform the following actions:

- To open the record, search and click the deal.

The user can view the deal information or take a few actions on the deal based on the requirements. To know more, refer to Post Deal Capture Actions section. Additionally, can download the record in different formats. To know more, refer to Blotter.

This section explains the actions that a user can perform and the features (such as Deal Capture , View , Delete , Amend , Authorize and Reversal ) of a deal.

The below screenshot illustrates how a deal is viewed and captured on the Deal Capture screen.

The following set of deal actions appears for the unauthorised deals (STATUS= INAU) when selected from the mini blotter.

- To open the record on the Deal Capture screen, click the View button.

> **⚠️ Note:** The View button allows the user to view and not modify the deal. Thus, the Action button is for information purpose.

This allows the user to replicate all the information of the selected deal to a new record. The new record opens on the Deal Capture screen (with the header as ‘copy of the selected deal’) pre-filled with all the information as supplied on the already selected deal. The user can modify the details before committing the deal.

The below is an illustration of the copy feature.

A copy of the selected deal is highlighted on the header and available at the upper-left of the screen. The user can amend the values or data before committing the deal to create a new record.

This allows the user to delete a committed record.

> **⚠️ Note:** This function is available only for deals, which are not in the live table (authorised).

After confirmation from the user, the system permanently deletes the record. The deal is simultaneously removed from the mini blotter and the below is displayed on the header of Deal Capture screen.

TFO allows the user to amend most fields at the unauthorised status. The contractual level information of the deal can be modified when information, such as deal type, deal currency and so on is not available for user modification. At this stage, a user can only reverse a deal if a deal has been entered erroneously.

A different user with privilege needs to authorise the unauthorised deals that are amended before moving it to the live table. The below is an illustration of Amend feature.

- Click the Amend button of the deal, which is in INAU status to open the record for modification. The no-change fields are not available for amendment.

Amending any field level information on the deal enables Amend button to commitment.

> **⚠️ Note:** The deal is in INAU status until a different user with privilege authorises the deal.

TFO allows the user to authorise all the unauthorised records from the blotter.

The below is an illustration of the feature.

1. Click the Auth button on any of the unauthorised deals, the record opens for authorisation. The screen shows a confirmation of authorisation before authorising the record.
2. Click the Authorise button.

> **⚠️ Note:** At the stage of confirmation, a user cannot make any modifications to the deal.

The deal moves to the live file, after authorisation. Self-authorisation, that is the same user who inputs the deal cannot authorise the record for audit purpose. The deal requires authorisation from a different user (who has the privileges to authorise, as defined on the USER table) to avoid INAU status.

The following error displays, when the user attempts a self-authorisation on the deal.

The following is the illustration of an authorised deal when authorised by the privileged user.

The action buttons applicable for the authorised deals are different from unauthorised records. The below is an illustration of all the actions available on the authorised deals.

The difference between amendment of unauthorised deals and authorised deals is available below.

TFO allows the user to amend only selective fields on all the committed records in comparison to fields in unauthorised deals, for audit reasons. The no-change fields differ for different product type.

The no-change fields are not available for user modification.

- To initiate the amendment process of authorised record, click the Amend button.

> **⚠️ Note:** After the amendment, a different user with privilege needs to authorise the record.

The reverse function allows the user to reverse an authorised deal and send it to the History table.

> **⚠️ Note:** This function is not available for deals that are not in the live table.

1. Click the Reverse button. The following screen appears.
2. To confirm the reverse action, click the Reverse button.
3. Click the Reverse button and the header on the screen displays the below text and the record gets RNAU status.


#### 📋 Tasks

Related topics:

- Execute Forex Trade (TFO)

There are no Tasks available for Deal Capture feature.


#### 📊 Outputs

There are no Outputs available for Deal Capture feature.


> **Related Applications:** `AGENCY`, `BASIC.INTEREST`, `BROKER`, `CCY.FOR.PAYMENT`, `CURRENCY`, `CUSTOMER`, `CUSTOMER.SECURITY`, `DEALER.DESK`, `EB.FREQUENCY`, `FT.CHARGE.TYPE`, `FT.COMMISSION.TYPE`, `FX`, `FX.AGREEMENT.TYPE`, `FX.DEAL.METHOD`, `FX.PARAMETERS`, `FX.TRANSACTION TYPE`, `ND DEAL`, `ND.PARAMETER`, `ND.SETTL.RATE.SOURCE`, `OC.CUSTOMER`, `PERIODIC.INTEREST`, `SC.SETTLEMENT`, `SEC.ACC.MASTER`, `SECURITY.MASTER`, `STOCK.EXCHANGE`, `SWIFT.CODE.WORDS`, `TY.CURRENCY.PAIR`, `TY.MARKET.RATES`, `User`

---


### 1.6  Exception Workflow Management


> **📇 Quick Reference Card**
> 
> **Purpose:** *Treasury Exception Workflow Management allows defining rule-based exceptions management for treasury trades.*
> 
> **Key Fields:** *DeptOfficer*, *Group*, *Reassign Reason*, *User*
> 
> **Sections:** 📖 Introduction | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Treasury Exception Workflow Management allows defining rule-based exceptions management for treasury trades.

This helps t he user to pre-define any overrides that may happen during trade capture as exception events. This is done to change the trade workflow for authorisation ( by an approved authority ) . For example, the front Office Supervisor before the trade flows into the back office queue.

When there is an exception, it is sent to the queue of the exception handler who approve s or refer s the transaction to the source or originator of the deal.


#### 🔧 Working With

The user needs to perform the following actions:

1. O n capturing the deal that results in the overrides defined by the banks as an exception . The deal moves to the queue of the Chief Dealer for approval, instead of the normal flow that goes to the back office for authorisation.
2. C hief D ealer log s on to launch the worklist and then approve s or reassign s the deal to the D ealer.

- To reassign the deal, the click the Re-assign button. The Re-assign drop-down appears as shown below.

- In the following fields, e nter the required values:

3. D ealer can pick and modify th e deal according to the suggestions , and then resubmit the deal .

4. C hief D ealer pick s and authorise s the deal by clicking the Auth button in deal details . The deal appears as shown below.

5. Dealer and Chief Dealer can launch the worklist from the blotter by clicking the Worklist tab .

Alternatively, on the upper-right corner of the screen, click .

T he number of deals awaiting pending action or approval appear s in numerical format along with the user icon.


#### 📋 Tasks

Related topics:

- Capture Deal - With Exception Workflow (TFO)

There are no Tasks available for Exception Workflow Management feature.


#### 📊 Outputs

There are no Outputs available for Exception Workflow Management feature.

---


### 1.7  Limits


> **📇 Quick Reference Card**
> 
> **Purpose:** *Banks encounter different types of risks that causes negative effect on their business. It is essential to manage these risks from the lowest ( dealer who places the order and enters the trade ) to the highest (bank) level in a hierarchical manner .*
> 
> **Sections:** 📖 Introduction | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Banks encounter different types of risks that causes negative effect on their business. It is essential to manage these risks from the lowest ( dealer who places the order and enters the trade ) to the highest (bank) level in a hierarchical manner .

A credit limit is the limit imposed by a bank to cover its maximum exposure to a specified counterparty. It is setup to mitigate and manage the limit utilisation of the credit extended to a counterparty.

In dealer limit, a risk is manged at the dealer level to eliminate the possibility of the loss spreading across the bank . T o manage, mitigate and monitor the risk, the dealer limits framework allows the bank to define the following:

- Currency Position Limits ( intraday and overnight )
- Product Limits
- Deal Size Limits
- Stop - Loss Limits


#### 🔧 Working With

This section helps the user to understand the working of Limits.


##### Credit Limits

The report can be accessed from Limits link available on the menu.

This report shows all the limits and utilisation for a customer or customer liability group and the associated collateral. It works on the following Temenos Transact enquiries:

- LIAB – Limits for a Customer or Customer Liability Group
- CO.001 – Limits and Collateral Enquiry

This report has a drill-down option. If sub-products exist below the Limit product, once the bottom of the Limit structure is reached, then the transactions that have utilised the limit are shown.

The user inputs the Liability Number or Name of the Counterparty as shown in the below screenshot.

The report retrieves the Limits and Collateral information and displays them in separate tabs, Liability and Collateral as shown below.

The below example shows that the Global Line consists of sub-products, such as FX, IRS and MM.

The product lines available are shown below.

1. FX Limit set at USD 40,000 and USD 600 is utilised (shown under Outstanding) and therefore the available limit is USD 39,400. The expiry date for the FX Limits is 22 Mar 2017.
2. To drill-down to the next level, click FX Box . This shows the Limit details of each deal type (that is, Spot, Swaps, Forwards and NDFs).
3. To show the transactions that constitute the utilisation of limits, click the deal type as shown below.
4. To view the deal details, click a transaction.

When the user inputs the counterparty name, both Limits and Collateral information for the counterparty is retrieved and displayed in separate tabs. The below screenshot shows t the Collateral tab.

To know more information on Temenos Transact LIAB and CO.001 enquiries, refer to Temenos Transact user guides.

The user can save favourites or copy and share the link to another user who has the permission to view the report.

The user can save and access a favourite later from the Favourites menu.

The user needs to perform the following:

1. Click the Favourites button and enter a name for the favourite.
2. To save a favourite, click Save . The favourite is saved and can be accessed from the Favourites menu.
3. To launch the screen as saved, click the favourite item.

The user can copy the link, and click it to view the same screen.

It displays the screen that is saved in the link.


##### Dealer Limits

Dealer Limits .

First Level View

The Dealer Limits screen displays the Intraday, Overnight, Stop-Loss and Product limits widgets.

- Intraday and Overnight limits are displayed in the aggregate limit currency (based on the configuration in TY.POSITION.LIMITS )
- Stop-Loss limit is displayed in Stop-Loss currency

Adiitionally, it displays the total limit amount set, limit available and limit outstanding (utilised).

The intraday limit is set to ensure the dealer does not exceed the limit specified for a day. The dealer can trade during the day but has to square off the position before End of the Day (EOD).

This displays the individual currency-specific limits set across the bank along with its corresponding utilisations.

- To view, click the Intraday widget in the first level.
- The currencies in which intraday limits have been breached (limit utilized exceeded the limit amount) are highlighted in red.

This displays the intraday limits of the dealers along with the utilisations for a particular currency. The dealers for whom the utilisation has already exceeded the limit are highlighted in red.

This displays the transactions done by a particular dealer in a selected currency during the day.

- To view the additional information, click the individual trades.

> **⚠️ Note:** Additionally, it displays all the treasury transactions and non-treasury deals that are greater than the negotiable amount specified.

An overnight limit is a restriction on the total open currency position that a trader can carry over from one trading day to the next.

This displays the individual overnight currency position limits set across the bank along with its corresponding utilisations.

1. To perform this, click the Overnight widget in the first level.
2. . The currencies in which overnight limits have been breached (limit utilised exceeded the limit amount) are highlighted in red.

This displays the time bucket split-up of the overnight limits of the dealers along with the utilisations for a particular currency.

- .
- The dealers for whom the utilisation has already exceeded the limit are highlighted in red.

This displays all the treasury and non-treasury deals for the chosen currency and dealer, which includes the overnight position.

- To view the additional information, click the individual trade.

> **⚠️ Note:** Addionally, it displays the treasury and non-treasury deals that are greater than the negotiable amount.

Banks can set stop-loss limits at bank and dealer level. These limits are set to cover the losses on the positions taken by a dealer in adverse market conditions or currency volatility.

This displays the individual dealer’s stop-loss limits along with their corresponding MTMs.

- To view, click the Stop-Loss widget on the first level.
- The dealers whose stop-loss limit has been breached are highlighted in red.

This displays all the individual deals of a particular dealer along with their corresponding MTMs.

- To view the additional information, click the individual trades.


###### Online Revaluation

Stop-Loss limits are continuously assessed at regular time intervals with the help of a service that refreshes in the background at pre-defined intervals. This helps in evaluating the MTM and determining whether the positions have breached the stop-loss limit assigned against a particular dealer or across the bank.

- To trigger a request for online revaluation, click in the Stop-Loss widget.

It displays the following:

- If the MTM exceeds the stop-loss limit for a specific dealer, the notification flag turns red for that specific dealer. This notifies that the Stop-Loss has been breached.
- If the stop-loss limit is breached at bank’s level, the flag appears in red for all the dealers.

- If MTM does not exceed the stop-loss limit, the flag remains in blue.

> **⚠️ Note:** The TY.UPDATE.STOP.LOSS service needs to be set to Auto for the online revaluation.

Product limits are set to restrict exposure to particular products. For example, if the bank wants to restrict the maximum forward exposure that a dealer can take in GBP, then set the limits for the product as FX Forward.

This displays the different limit products that are assigned to the respective dealer (F5 in this case) and also the limit breaches (highlighted in red).

This displays the different currencies for which the limit has been setup for the dealer in a particular product.

This displays all the transactions that influences the product limit.

To view additional information, click the individual transactions.

The bank can define the deal size limits for every dealer. This restricts the dealers from taking huge positions in a single transaction. In the event of any breach of deal size limits, it is recorded as an override in the transaction.

These are generated during Close of Business (COB) and made available for the users to check the breaches in different limit definitions, such as intraday limit, overnight limit, stop loss, product limit and deal size limit.

- To access the corresponding breach reports, click .


#### 📋 Tasks

There are no Tasks available for Limits feature.


#### 📊 Outputs

There are no Outputs available for Limits feature.

---


### 1.8  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *Treasury Front Office (TFO) built on the Temenos platform helps bank’s treasurers to meet the challenges of complex global markets by catering to the needs of international treasury operations in a modern environment.*
> 
> **Key Fields:** *Admin Usernames*, *Auto Refresh Blotter*, *Auto Refresh FX Rates*, *Auto Refresh Positions*, *Auto Show Reuters Widget*, *Blotter Refresh Interval (S)*, *Chief Dealer Eqv*, *Counterparty Client Sector Filter* ... +31 more
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- APIs
- Temenos Transact Services

Treasury Front Office (TFO) built on the Temenos platform helps bank’s treasurers to meet the challenges of complex global markets by catering to the needs of international treasury operations in a modern environment.

It consolidates all the tools required by TFO users in a single location and delivers real-time control over the entire sales and trading desks. TFO combines advanced trader tools, risk management workflow, and real-time trade processing to help financial institutions in improving time-to-market, increase Straight-Through Processing (STP), and cut costs.

The solution is built in Temenos Transact Transact, which supports a wide range of instruments while delivering the following:

- High trade capacities
- Streamlined transaction processes
- Reliable and cost-effective risk management within a modern technological framework

TFO supports the following that is essential within a bank’s trading room:

- Deal capture
- Blotters
- Pricing
- Position and portfolio management
- Profitability reporting

TFO provides STP of deals done in the front office. Deals captured in TFO updates the trader positions and flow to the back office for approval without any user intervention.

The risk management facilities extend not just across the dealing room but the bank as a whole. Risk Managers can view the complete position of the bank in real-time.

This section provides an overview and explains the various front office features, such as Deal Capture, Position Monitoring, Dashboards, Exception Workflow and Trade Blotters.

Additionally, it offers a comprehensive overview of the front office and usability in a typical bank dealing room.

The intended audience of this module are as follows:

| Role | Function |
|---|---|
| Treasury Front Office Dealer | Executes deals with a counterparty and records the deal details in the system Views and manages the positions along with their performance |
| Treasury Front Office Supervisors | Monitors the positions across trading and banking books |
| Risk Manager | Enforces and monitors risk limits |
| IT Personnel | Maintains IT infrastructure, upgrades the application, system and user settings |


##### Navigation Menu

To access the TFO menu, click .

The following links are available on the TFO menu, which the user can drag and re-order:

- Favourites
- Deal Capture
- Positions
- Blotter
- Limits
- Dashboard
- Settings

Each item has sub-menu available. The sub-menu available for Blotter is given below.

The user can save any inquiry performed on the trade blotters, currency positions and others as a Favourite for repeated use. This helps to avoid entering search criteria when required.

Keyboard shortcuts are keys or combinations of keys that provide an alternative method to do something that user would typically do with a mouse.

Keyboard Shortcuts .

The user can select a specific shortcut from the drop-down list for each screen.

After choosing the shortcuts for the desired applications, the user can save the shortcut by clicking Save .

Selecting the shortcuts at any stage or on any screen opens the specific screen.

This section helps the user to open or close a tab.

| Feature | Shortcut |
|---|---|
| FX Forward | Alt + 1 |
| Profitability View | Alt + 2 |
| Keyboard Shortcuts | Alt + 3 |
| FX Swaps | Alt + 4 |
| Blotter | Alt + 5 |


##### Product Configuration

This section explains the following topics:

The following prerequisites are checked to install and run the TFO application:

- Access to the latest TFO.War file
- Access to the most recent TFO.IRIS.War file
- Install and run the Temenos Transact Model Bank version (201712 version and above)
- Presence of TY module in SPF
- Require parameterisation in TY module parameters and tables
- Development of versions and enquiries

The system and user settings are explained as follows:

1. Deployments ).
2. Paste the TFO.War file.

If a TFO.War already exists, then it is deleted along with its deployed War file and a new one is pasted in its place.

> **⚠️ Note:** This process is not followed during the first installation, as there is no existing TFO.War files. In this case, the user is only required to paste the file and wait until it is deployed.

1. Deployments ).
2. Delete the previous TFO.IRIS.War and undeployed TFO.IRIS.War .
3. Paste the new TFO.IRIS.War and ensure an ID is deployed.

> **⚠️ Note:** This process is not followed for the first installation, as there is no actual TFO.IRIS.War file. In this case, the user is only required to paste the file and wait until it is deployed.

| Field | Description |
|---|---|
| Language | Set the language for the system. The user has the option to switch between multiple languages. (Currently, it supports English and French ) |
| Auto Refresh FX Rates | Refresh system-wide FX rates automatically (set to Yes) or manually (set to No). |
| FX Rates Refresh Interval (S) | Set the FX rates to refresh interval in seconds. |
| Auto Refresh Blotter | Refresh the trade blotters automatically (set to Yes) or manually (set to No) to update the blotters with new trades. |
| Auto Refresh Positions | The option to refresh FX Positions to automatic (set to Yes) or manual (set to No). |
| Positions in Thousands | Show the amounts in thousands (set to Yes) or the full figures (set to No) on the Position screens in the system. |
| Auto Show Reuters Widget | Control the auto display of the Reuters widget on the upper-right of the Deal capture screen, when a user selects a Currency Pair. |
| Open Dashboard after Login | If set to Yes, the Dashboard is set on the homepage and appears after the user logs on to the system. |
| Fit Dashboard to Screen | If set to Yes, the Dashboard is auto-adjusted to fit the width of the browser. |
| Save | Save user settings. |

TFO is added with a new feature to customise the menu items and provide the links to launch the Versions, Enquiries, Composite screens from the Temenos Transact UXBP (new browser).

> **⚠️ Note:** To launch the Temenos Transact new browser screen without log on intervention, configure the Single Sign On option.

This section enables the user to add a composite screen by using Menu Customisation option. The user needs to perform the below actions:

1. Menu Customisation .
2. Select the menu item (for example, Deal Capture) in which a sub-menu needs to be added.
3. Right-click the existing sub-menu item to add a new section or item.
4. To save the details, click Apply .
5. To save the changes, click Save All Changes .

> **⚠️ Note:** Use the menu security to provide access rights to the respective user. To know more, refer to Menu Security .

This section enables the user to add an enquiry by using Menu Customisation. The user needs to perform the below actions:

1. Follow step 1, 2, 3 and 4 as stated in above section to create a sub-item or sub section.

> **⚠️ Note:** The format of the link needs to be new browser link followed by the screen name prefixed with either COS, ENQ, VER.

2. To save the changes, click Save All Changes .

> **⚠️ Note:** Use the menu security to provide access rights to the respective user. To know more, refer to Menu Security .

3. To launch the Temenos Transact new browser screen without log on intervention, log on to TFO and select the respective menu configured.

4. To end the SSO session, log off and close the browser window.

---


### 1.9  Positions


> **📇 Quick Reference Card**
> 
> **Purpose:** *The position and profitability views provide real time Profit and Loss (P&L) and Position Monitoring across the bank.*
> 
> **Key Fields:** *Adding Favourite Currency*, *Adding/Editing Columns*, *Amount1*, *Commas*, *Common Functionalities*, *Decimal Places*, *Decimals*, *Default Button* ... +22 more
> 
> **Sections:** 📖 Introduction | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The position and profitability views provide real time Profit and Loss (P&L) and Position Monitoring across the bank.

Real-time positions generated anywhere in the organisation are instantly available in the position views, to provide complete visibility of the banking and trading books.

Currently, the Treasury Front Office (TFO) supports the following position views:

- Currency position
- FX profitability
- FX overall position
- Nostro summary
- Cash flow position
- Interest rate gap position
- Swap revaluation
- Security position


#### 🔧 Working With

This section helps the user to understand the working of Currency Position.


##### Currency Position View

TFO offers a complete view of the currency positions along with with Mark to Market (MTM) revaluation, without emphasising the need to provide a view of the currency positions in trading, own or customer positions. This screen offers two tabs, (that is, by Currency and Currency Pair) and allows configuration of the following:

- Particular Dealer’s position
- Entire FX dealing desk
- Position for the bank as a whole

This feature does not permit the Dealer to have a representation of the actual positions but can make decisions. This can perform different actions, such as what-if analysis, spot differentiation from the forward position and so on.

FX .

The default screen appears as shown below.

The Currency Position screen has the following three submenus, which caters to different purposes of the user.

Main Screen

This has principal information of the currency positions (that is all the enabled actions available for the Dealer).

Favourite

This has information about the unrealised Profit and Loss (P&L) and total outstanding amount in the currency defined in the Reval Ccy field in TY.PARAMETER table. Additionally, it displays a graphical representation of the long and short position of the favourite currencies.

This submenu can only provide information, hence, the user cannot take any further actions.

Saved Position Views

This has all the previously saved views by the Dealer. This enables the Dealer to directly open a view that was saved in the past.

The Dealer can add any currency to the Favourites to get these currencies shown as default in the Favourite Position screen at the top of all the listed currencies.

- Right-click the selected currency and click the star that is shown. The currency is added to Favorites.

> **⚠️ Note:** The Dealer is not allowed to change the order of the currencies. Therefore, to modify the disposition of the Favourites, the Dealer removes all the currencies from the Favourites and then, re-adds them in the desired order.


###### FX Position by Currency

Generally, Positions arising out of customer transactions and asset-liability Positions are maintained by currency while there exists a preference to view the trading positions by currency pair.

The overall position in a particular currency is shown as long, short, and net columns. Weighted average cost and the corresponding market rate shows the MTM revaluation results in local currency, and in any other currency based on the parameter setting in TY.PARAMETER .

The overall position in a particular currency has the following three categories:

- Asset and liability positions in the bank’s balance sheet as of the previous day
- Current non-treasury positions
- Forex deals

The user can further drill-down each of the above categories in current non-treasury positions but not in asset and liability positions.

The market rates are fetched from TY.MARKET.RATES table. If an interface for market-rate feed exists to update this table, the MTM revaluation is a near real-time feature. In the absence of this interface, the market rates are based on Currency and Forward Rates tables. The MTM revaluation changes depending on the frequency with which the rates are refreshed.

In non-treasury positions, the list of underlying transactions is selected and shown based on a threshold limit set in each currency record in Negotiable Amount field for the following reasons:

- It is not required to show the number of smaller transactions which goes with card rates.
- It enables the Dealers to view the reported transactions for rates by branches for verification purpose.

The screen allows the user to add a new column and define a limit for each row to monitor. For example, stop loss or position excess against any particular currency.

The position screen offers the following three levels view:

| Option | Description |
|---|---|
| None | Does not show any value |
| Total | Adds or subtracts all the values present in the selected column to provide the total amount |
| Average | Displays the calculated mathematical average of all the values present in the selected column |
| Weighted Average | Displays the value calculated according to predefined parameters |
| Count | Counts the values present in the selected column |

This level is displayed only when a currency is selected to provide the composition of the position, such as asset and liability, current non-treasury and treasury positions.

The user needs to click the position type to display the relevant third level position. However, the user cannot perform further drill down for asset and liability position.

| Field | Description |
|---|---|
| New Column Name | Inputs any alphanumerical character |
| Width | Defines the width of the column |
| Right Align | Displays data to the right of the column |
| Place Column | Decides if the column shows at the end or before another column. The default setup cannot be modified. Therefore, the first created column always shows in the end. Dealer can modify the position of the added columns but not the default columns. |
| Default Formula | Creates a default formula, which is used for all the lines. Enters any numerical characters and inserts the column name Default formula is (Cost – Market Rate) * 100. Dealer can override this formula in the individual field, by right-clicking and inserting a new formula. |
| Decimal Places | Decides on the number of decimal places displayed |
| Commas | Decides whether the commas are shown or not. For example, 1000 or 1,000 |
| If Result is | Decides the formatting of the result. It allows the following values: less than , greater than and equals to Dealer can assign a format for each of these values |


###### FX Position by Currency Pair

This helps to view the position created using FX deals including non-deliverable forward deals.

All the features and scenarios analysed above are valid for the position by currency pair. There are a few differences, which are analysed as follows:

- To view the list of position by currency pair, click the FX Position by Currency Pair button.

This feature helps the Dealers in monitoring and customising the view of their position. Additionally, allows to square-off their positions in the same currency pair. They can add additional columns to introduce stop loss or position limits for each Currency Pair and monitor their positions.

Since the positions are related to FX deals only (including non-deliverable forwards), the Dealer cannot view the composition of the transactions in asset and liabilities, non-treasury and treasury transactions.

The system displays all the individual transactions in the currency pair position when clicking a given currency pair.

An example is given below.


##### FX Profitability View

A view of the dealers or Treasury Profitability is another important feature that TFO offers. This helps to measure the performance of a Dealer or the whole of FX desk.

FX profitability refers to the income generated from FX activity by the dealing room and FX transactions across the bank. It can have income from pure trading, interbank cover operations, and merchant or corporate transactions.

The profit numbers include the following:

- Realised Profit or Loss – Income on transaction completed and contracts matured
- Unrealised Profit or Loss – Estimated P&L relating to outstanding FX contracts

Profitability View .

It displays the default screen.

Two default views are available: Dealer Profitability (refers to the Dealer who logs into the system) and Treasury Profitability (provides an overview of the entire treasury).

The dealer desk associated with the user profile is selected to show profitability. It is assumed that the user who logs on is also the dealer for whom the profitability needs to be viewed.

This section provides information about the profitability of a single dealer.

- To access this feature, click the Dealer Profitability tab.

> **⚠️ Note:** It automatically selects the dealer desk attached to the user record and provides a set of information.

In the Dealer Profitability section shown below, some numbers are purposely shown in negative and red to differentiate between profit and loss numbers.

In the individual dealer view, the Dealer division has the name of the Dealer associated with the user record.

| Column 1 | Column 2 |
|---|---|
| Year till Month (YTM) | Derived from the sum of the P&L numbers from the beginning of the financial year to the end of the last month |
| Month till Date (MTD) | Derived from the sum of the P&L numbers from the beginning of the month to the previous day |
| Year till Date (YTD) | Represents the sum of the P&L numbers from the beginning of the year to the previous day of the system date It can also be calculated as YTM + MTD |

This section has all the estimated or locked P&L related to current FX transactions and outstanding FX contracts using online revaluation.

Only one value is recorded in this section and is analysed below.

Mark to Market (MTM)

This has the outstanding contracts for a given Dealer and also current transactions, such as FT, DR and SC, which involve FX rate. Numbers in this column change according to the movements of the market.

Total

This column has a total of the numbers present in the Dealer row and equivalent in GBP. YTD represents the sum of the unrealised and realised P&L present in the Profitability View.

Total P&L in LCY is also shown in GBP as opted by the user in TY.PARAMETER .

This tab provides information about the FX Profitability of the entire FX desk by consolidating the profitability of all the Dealers who are assigned to various activities within FX desks.

The FX desk or Treasury Profitability can be accessed using the corresponding tab.

In the Treasury Profitability view, the Dealer division has all the income sources available among all the Dealers, such as Trading, Interbank, Corporate and so on.

When one or more generic sources are present, each of these can be drilled down to have information regarding the individual Dealer positions.

> **⚠️ Note:** All the information is provided for both generic sources and individual dealers.

| Field | Description |
|---|---|
| New Column Name | Inputs any alphanumerical character |
| Width | Defines the width of the column |
| Right Align | Displays data to the right of the column |
| Place Column | Decides if the column shows at the end or before another column The default setup cannot be modified. Therefore, the first created column always shows in the end. Dealer can modify the position of the added columns but not the default columns. |
| Default Formula | Creates a default formula, which is used for all the lines Enters any numerical characters and inserts the column name Default formula is (Cost – Market Rate) * 100. Dealer can override this formula in the individual field, by right-clicking and inserting a new formula. |
| Decimal Places | Decides on the number of decimal places displayed |
| Commas | Decides whether the commas are shown or not. For example, 1000 or 1,000 |
| If Result is | Decides the formatting of the result It allows the following values: Less than Greater than and equals Dealer can assign a format for each of these values The colours of the new columns are not implemented. However, the system can display the colours according to the Dealer’s inputs. |


##### Nostro Summary View

Nostro Summary .

The user can perform the following:

1. View the currency-wise consolidated balance of Nostro accounts for five days from the current date.
2. Drill down further to view the account balances, and Nostro forward balances in multiple Nostro accounts for a selected currency.
3. Filter trades, create saved views, add or edit columns and perform other relevant actions as described in and blotter and currency position view

To know more, refer to Nostro Summary (NOSTRO.SUMMARY), Nostro Position (NOSTRO.POSITION) and Forward Account Statement (NOSTRO.FWD.BAL) enquiries in Temenos Transact .


##### FX Overall Position

FX Overall Position .

| Position | Description |
|---|---|
| AL | Related to matured deals |
| Spot | Deals that are due to mature in the spot period |
| Forward | Deals that are due to mature beyond the spot period |
| Net | Net of AL, Spot and Forward Positions |


##### Cash Flow Position

This feature helps the user to view by date, the amount of each currency flowing in and out of the bank and net movement by date, and also cumulative cash flow. This enables the user to control the funds efficiently and profitably.

The user can perform the following:

1. Cash Flow Position . The Cash Flow Position screen is displayed.
2. The user can choose a different Calendar (a valid calendar record in PM.CALENDAR of Temenos Transact ) record to view the same cash flow movement using a different series of time band buckets.
3. To view the transaction details for the selected period, click any one of the time band buckets.
4. Filter trades, create saved views, add or edit columns and perform other actions in the features.

To know more information on the view, refer to Cash Flow Position (PM.CAS) enquiry in Temenos Transact .

| Field | Description |
|---|---|
| Adding Favourite Currency | To know more, refer to Adding Favourite Currency |
| Sorting | To know more, refer to Sorting |
| Search | To know more, refer to Search |
| Adding/Editing Columns | To know more, refer to Adding or Editing Columns |
| Default Button | To know more, Refer to Default button |
| Common Functionalities | To know more, refer to Common Functionalities |
| Editing the Layout | To know more, refer to Editing the Blotter Layout |
| Downloading and Printing Position Views | To know more, refer to Downloading and Printing Position Views |


##### Interest Rate Gap

This feature helps the user to view for each currency by 'time bucket' and, the future amounts placed and taken, and at what with their average rate. Consequently, it calculates and displays the amount and rate, which would need to be taken or placed, in order to eliminate any mismatching, is calculated and displayed. Additionally, it shows the graph on top with the inflows and outflows across the calendar periods.

The user can perform the following:

1. Interest Rate Gap . The Interest rate Gap screen is displayed.
2. User can choose a different Calendar (a valid calendar record in PM.CALENDAR table of Temenos Transact ) record to view the same interest rate gap using a different series of time band buckets.
3. To view the transaction details within that time band bucket, click any one of the time band buckets.
4. Filter trades, create saved views, add or edit columns and perform other actions in the features.

To know more about the view, refer to Interest Mismatch (GAP) Position (PM.GAP) enquiry in Temenos Transact .

| Field | Description |
|---|---|
| Adding Favourite Currency | To know more, refer to Adding Favourite Currency |
| Search | To know more, refer to Search |
| Adding/Editing Columns | To know more, refer to Adding or Editing Columns |
| Default Button | To know more, refer to the Default button |
| Common Functionalities | To know more, refer to Common Functionalities |
| Display Graph | This allows the user to display or hide the graph when not required. To perform this, click . |
| Editing the Layout | To know more, refer to Editing the Blotter Layout |
| Downloading and Printing Position Views | To know more, refer to Downloading and Printing Position Views |


##### Swap Revaluation

The Swap Revaluation screen has two tabs to display Interest Rate Swap and Currency Interest Rate Swap revaluations.

- Swap Revaluation .

The IRS tab displays currency-wise revaluation of IRS contracts. The table shows the following columns:

- NPV Asset
- NPV Liability
- P&L To Date
- P&L Today
- Profit till Yesterday

The user can perform the following:

1. Click a particular currency. The underlying swap deals of the position and a graph with the P&L To Date value for the selected currency appear.
2. Click a deal. The deal and contact details appear.
3. To view the options in a particular deal, click .

The CIRS tab displays currency pair wise revaluation of CIRS contracts. The table shows the following columns:

- NPV Asset
- NPV Liability
- P&L To Date
- P&L Today
- Profit Till Yesterday

The user can perform the following:

1. Click a particular Currency Pair. The underlying swap deals of the position and a graph with the P&L To Date value for the selected currency pair appear.
2. Click a deal. The deal and contract details appear.
3. To view the options in a particular deal, click .

To know more information on Swap Revaluation, refer to Temenos Transact user guide.

| Field | Description |
|---|---|
| Search | To know more, refer to Search |
| Adding/Editing Columns | To know more, refer to Adding or Editing Columns |
| Default Button | To know more, refer to Default button |
| Common Functionalities | To know more, refer to Common Functionalities |
| Editing the Layout | To know more, refer to Editing the Blotter Layout |
| Downloading and Printing Position Views | To know more, refer to Downloading and Printing Position Views |


##### Security Position

Security Position .

The Security Position screen is displayed with Portfolios and Securities.

The Securities tab displays the consolidated position of individual securities.

The Securities Position Details (first level view) has the following information about the securities:

- Security Number
- Security Description
- Sub-Asset Type
- Security Currency
- Interest Rate
- Maturity Date
- Nominal
- Book Cost
- Unrealised P&L
- Realised P&L
- Accrued Interest
- Accrued Discount
- Last Trade

The Widget section displays the nominal share of securities based on different sub-asset type.

Buy or Sell Action

The user can buy or sell particular security by performing the following:

1. Right-click the respective security number from the Security Position screen.
2. Click Buy or Sell , the Securities Deal Capture screen of the respective asset type shows the static fields, such as Security Description , Stock Exchange , Trade Currency , Trade Date and so on.

> **⚠️ Note:** The values of these fields default from Security Position screen.

Mini Securities Inventory

The Security Description field is already available in the Deal Capture screen. The Mini Security Inventory section shows quick reference details for the stated security, before executing the transaction.

1. Click particular security available in Securities Position Details view. The screen shows a second-level view, that is, Own Book Position Details. The Own Book Position Details (second level view) has the following information about the securities in different Portfolio books: Security Number Security Description Sub-Asset Type Security Currency Interest Rate Maturity Date Nominal Book Cost Unrealised P&L Realised P&L Accrued Interest Accrued Discount Last Trade
2. To open the Portfolio tab in Security Position screen, click icon. The portfolio number is defaulted to view the respective portfolio’s valuation. The Widget section displays the contribution of security nominal available in different own book portfolio.

- To view the transactions, click a particular portfolio in Own Book Position Details section.

The Portfolio tab displays the consolidated position of all own book portfolio.

The Portfolio Position Details (first level view) provides all the vital information about the own book portfolio and their corresponding valuation.

The Widget section displays the bar for one of the selections:

- Investment Value
- Market Value
- Unrealised P&L

- To open the second level view, click the required portfolio in the consolidated portfolio position view. For example, Security Holdings in the Portfolio selected.

The Security Holding Details in the portfolio (second level view) have all the important information about the security holdings related to different asset types, position and valuation of each security.

The Widget section displays the pie chart for the nominal share of securities based on different sub-asset types.

Another widget displays the bar for one of the selections when the user clicks .

- Investment value
- Market value
- Unrealized P&L

If the user selects Unrealised P&L, the horizontal bar is displayed based on the profit or loss position of the security. In case it is in profit, the bar for the particular security position is displayed in green, else in red.

- Darker the gradient of green, the greater the profit from the position.
- Darker the gradient of red, the higher is the loss from the position.

- To open the third level view, click the required security in Security Holdings Details view. For example, Security Movements.
- To open the deal details of the particular transaction, click the security trade.

This level shows the price and date on which particular security is bought or sold.

- To buy or sell a particular security, on the Security Holdings screen, right-click the respective security number and select Buy or Sell option.

The Securities Deal Capture screen of the respective asset type displays static fields, such as Security Description , Stock Exchange , Trade Currency , Trade Date and so on, defaulted from Security Position screen.

| Feature | Description |
|---|---|
| Search | To know more, refer to Search |
| Adding or Editing Columns | To know more, refer to Adding or Editing Columns |
| Default Button | To know more, refer to the Default button |
| Common Functionalities | To know more, refer to Common Functionalities |
| Editing the Layout | To know more, refer to Editing the Blotter Layout |


##### Repo Position

Repo Position .

Repo Position Screen has three tabs to display Repo, Reverse Repo and Securities.

The Repo tab displays positions of all Repo trades underneath.

The Repo Position (first level view) has the following information:

- Position ID
- Portfolio
- Security ID
- Depository
- Nominal

With a click over a particular Position ID, the screen opens up the second level view, that is Repo Position Movements.

With a click over a particular Repo ID, the screen opens up the Repo contract as deal details sidebar.

The Reverse Repo tab displays positions of all Reverse Repo trades underneath.

The Reso Position (first level view) has the following information:

- Position ID
- Portfolio
- Security ID
- Depository
- Nominal

With a click over a particular Position ID, the screen opens up the second level view, that is, Reverse Repo Position Movements.

With a click over a particular Reverse Repo ID, the screen opens up the Reverse Repo contract as deal details sidebar.

| Field | Description |
|---|---|
| Search | To know more, refer to Search |
| Adding or Editing Columns | To know more, refer to Adding or Editing Columns |
| Default Button | To know more, refer to the Default button |
| Common Functionalities | To know more, refer to Common Functionalities |
| Editing the Layout | To know more, refer to Editing the Blotter Layout |


##### Derivatives Position

Derivatives Position .

The Derivatives Net Position screen is displayed.


#### 📋 Tasks

There are no Tasks available for Positions feature.


#### 📊 Outputs

There are no Outputs available for Positions feature.

---


---


## Appendix A: Glossary of T24 Applications & Fields


This glossary lists all T24/Transact application names and field names referenced throughout this document, with descriptions where available.


### Applications


| Application | Description |
|------------|-------------|
| `AGENCY` | T24 application: AGENCY |
| `BASIC.INTEREST` | T24 application: BASIC.INTEREST |
| `BROKER` | T24 application: BROKER |
| `CCY.FOR.PAYMENT` | T24 application: CCY.FOR.PAYMENT |
| `CURRENCY` | T24 application: CURRENCY |
| `CUSTOMER` | T24 application: CUSTOMER |
| `CUSTOMER.SECURITY` | T24 application: CUSTOMER.SECURITY |
| `DEALER.DESK` | T24 application: DEALER.DESK |
| `EB.FREQUENCY` | T24 application: EB.FREQUENCY |
| `FT.CHARGE.TYPE` | T24 application: FT.CHARGE.TYPE |
| `FT.COMMISSION.TYPE` | T24 application: FT.COMMISSION.TYPE |
| `FX` | T24 application: FX |
| `FX.AGREEMENT.TYPE` | T24 application: FX.AGREEMENT.TYPE |
| `FX.DEAL.METHOD` | T24 application: FX.DEAL.METHOD |
| `FX.PARAMETERS` | T24 application: FX.PARAMETERS |
| `FX.TRANSACTION TYPE` | T24 application: FX.TRANSACTION TYPE |
| `ND DEAL` | T24 application: ND DEAL |
| `ND.PARAMETER` | T24 application: ND.PARAMETER |
| `ND.SETTL.RATE.SOURCE` | T24 application: ND.SETTL.RATE.SOURCE |
| `OC.CUSTOMER` | T24 application: OC.CUSTOMER |
| `PERIODIC.INTEREST` | T24 application: PERIODIC.INTEREST |
| `SC.SETTLEMENT` | T24 application: SC.SETTLEMENT |
| `SEC.ACC.MASTER` | T24 application: SEC.ACC.MASTER |
| `SECURITY.MASTER` | T24 application: SECURITY.MASTER |
| `STOCK.EXCHANGE` | T24 application: STOCK.EXCHANGE |
| `SWIFT.CODE.WORDS` | T24 application: SWIFT.CODE.WORDS |
| `SYSTEM` | T24 application: SYSTEM |
| `TY.CURRENCY.PAIR` | T24 application: TY.CURRENCY.PAIR |
| `TY.MARKET.RATES` | T24 application: TY.MARKET.RATES |
| `User` | T24 application: User |


### Fields Referenced


| Field | Field | Field |
|-------|-------|-------|
| `Account Number` | `Accrued Interest` | `Action Buttons` |
| `Adding Favourite Currency` | `Adding/Editing Columns` | `Additional Agreements` |
| `Adjustments` | `Admin Usernames` | `Agreement` |
| `Agreement Type` | `Amount` | `Amount Bought or Sold` |
| `Amount1` | `Application Access Link` | `Application Access Type` |
| `Asset Amortisation Date` | `Asset Amount` | `Asset Currency` |
| `Asset Date` | `Asset Narrative` | `Asset Rate` |
| `Asset Treasury Rate` | `Audit` | `Aut Sc Ref` |
| `Authori` | `Authoriser` | `Auto` |
| `Auto Capitalise Interest` | `Auto Refresh Blotter` | `Auto Refresh FX Rates` |
| `Auto Refresh Positions` | `Auto Rollover Term` | `Auto Show Reuters Widget` |
| `Auto-Rollover` | `Bank A/C Number` | `Bank To Bank Info` |
| `Bank to Bank Info` | `Base and Counter Currency` | `Ben Acct` |
| `Ben Bank1` | `Ben Bank2` | `Beneficiary` |
| `Beneficiary Account` | `Beneficiary Address` | `Beneficiary No` |
| `Blotter` | `Blotter Refresh Interval (S)` | `Bond Deal Capture` |
| `Broker` | `Broker Currency` | `Broker Fee` |
| `Broker Fees` | `Broker Name` | `Broker Selection` |
| `Brokerage` | `Brokerage Base` | `Business Centre` |
| `Buy` | `Buy Sell` | `Buy or Sell` |
| `C` | `Calc Link (Y/N)` | `Capitalise Interest` |
| `Capitalised Interest` | `Ccy For Payment` | `Charge` |
| `Chief Dealer Eqv` | `Clean Price` | `Clear` |
| `Code` | `Commas` | `Common Functionalities` |
| `Company Code` | `Contract Date` | `Contract Price` |
| `Contract Type` | `Convention` | `Counterparty` |
| `Counterparty Bank Account` | `Counterparty Client Sector Filter` | `Counterparty Correspondence Address` |
| `Counterparty Correspondence No` | `Counterparty Correspondent` | `Counterparty Correspondent Address` |
| `Counterparty Correspondent Bank` | `Counterparty IB Sector Filter` | `Counterparty Reference` |
| `Counterparty SSI` | `Counterparty/Broker` | `Counterparty/Broker Selection` |
| `Cparty Corres Bank` | `Cpty Bank 1` | `Cpty Bank 2` |
| `Credit Account` | `Credit Category` | `Currency` |
| `Currency Name` | `Currency Pair` | `Current No` |
| `Cus Margin Default` | `Customer` | `Customer Margin` |
| `Date` | `Date Format` | `Date Time` |
| `Deal` | `Deal Action Bar` | `Deal Currency` |
| `Deal Text` | `Deal Type` | `Dealer` |
| `Dealer Eqv` | `Dealer Id` | `Debit` |
| `Debit Account` | `Decimal Places` | `Decimals` |
| `Def Fix Days` | `Default Button` | `Default Formula` |
| `Delivery Inst` | `Department Code` | `Department for Reval` |
| `Depository` | `DeptOfficer` | `Description` |
| `Desk` | `Dirty Price` | `Downloading and Printing Position Views` |
| `Drawdown A/C` | `Editing the Layout` | `Effective Date` |
| `Enable Customer Closure` | `Exception Workflow` | `Exchange` |
| `Exchange Profit` | `Execute Forward Rate` | `Exotic` |
| `Expiry Date` | `FIELD.NAME` | `FIELD.VALUE` |
| `FRA Amount` | `FRA Currency` | `FRA Period, Start Date and Maturity Date` |
| `FRA Rate` | `FRA Type` | `FX Commission Group ID` |
| `FX Group Cond ID` | `FX Rates Refresh Interval (S)` | `Final Maturity Date` |
| `Firm Book` | `Fit Dashboard to` | `Fixed Interest Rate` |
| `Fixing Currency` | `Fixing Date` | `Fixing Days` |
| `Floating Interest Rate` | `Forward Price` | `Forward Rate Key` |
| `Fractional Trade` | `Free Format Address` | `Frequency` |
| `From` | `Gross Amount` | `Group` |
| `Group Name` | `Hold` | `Hold Cash` |
| `Hold Stock` | `Holiday Calendar` | `INT.BASIS` |
| `IRIS Server` | `If Result is` | `Index` |
| `Initial Margin` | `Initial Margin Amt` | `Inputter` |
| `Interest` | `Interest Accrual and Maturity` | `Interest Basis` |
| `Interest Days` | `Interest Liquidation A/C` | `Interest Payment Frequency` |
| `Interest Rate and Margin` | `Interest Schedule` | `Interest Spread` |
| `Interest Start Date` | `Interest Term` | `Intermed Bk No` |
| `Intermediary Address` | `Intermediary Bank` | `Issue Amount` |
| `Issue Date` | `JH.ACCESS.LINK` | `JH.ACCESS.TYPE` |
| `Language` | `Liability Amortisation Date` | `Liability Amount` |
| `Liability Currency` | `Liability Date` | `Liability Narrative` |
| `Liability Rate` | `Liability Treasury Rate` | `Limit` |
| `Limit Reference` | `Limits` | `Link` |
| `Liquidate Interest` | `List` | `Live` |
| `Live Rate` | `M` | `MM Ref` |
| `Margin` | `Margin %` | `Margin Call Eff Date` |
| `Margin Call Trade Date` | `Margin Percentage` | `Margin Pips` |
| `Margin Portfolio` | `Marketing` | `Marketing Exchange` |
| `Mature at` | `Mature at Start of Day` | `Mature at Start of the Day` |
| `Maturity` | `Maturity Calendar` | `Maturity Date` |
| `Method` | `Ndf Allow Ccy` | `Near Leg Rate` |
| `Negative Interest` | `Negative Rates` | `Negotiable Amount` |
| `Net Amount` | `Netting` | `New Column Name` |
| `Next Fixing Date` | `No. of Days` | `Nominal` |
| `Notes` | `Number of Decimal Places` | `Numeric Currency Code` |
| `OPERAND` | `Open Dashboard after Login` | `Other` |
| `Other Details` | `Override` | `Own Book` |
| `P` | `PARTY.APPLICATION` | `Pay from A/C` |
| `Payment Narrative` | `Pips` | `Place Column` |
| `Portfolio` | `Portfolio and Security Description` | `Positions Refresh Interval (S)` |
| `Positions in Thousands` | `Price` | `Prin Increase` |
| `Principal Exchange` | `Principal Liquidation Account` | `Principle Liquidation A/C` |
| `Product Category` | `R` | `RF Rate` |
| `RFR Calc Method` | `RFR Convention` | `RFR Lookback Days` |
| `RFR Lookback Type` | `RFR Online Maturity` | `RFR Spread Treatment` |
| `Range` | `Rate` | `Rate Key Floating` |
| `Rate Provider` | `Rate Reset Frequency` | `Rate Selection` |
| `Rate Source` | `Rate Type` | `Reassign Reason` |
| `Receive To A/C` | `Receiver Bank` | `Record Status` |
| `Reference` | `Reference Price` | `Reference Rate` |
| `Repo Interest` | `Repo Rate` | `Repurchase Amount` |
| `Repurchase Date` | `Result` | `Reval Ccy` |
| `Revaluation` | `Revaluation Type` | `Right Align` |
| `Rollover` | `Rollover Interest Rate` | `Rollover Term` |
| `SYSTEM.ID` | `Save` | `Screen` |
| `Search` | `Security` | `Security Description` |
| `Sell` | `Sell or Buy` | `Send Payment Message` |
| `Service Name` | `Settlement` | `Settlement Account` |
| `Settlement Currency` | `Settlement Date` | `Settlement Rate Source` |
| `Side` | `Sign-On Name` | `Sorting` |
| `Special Notes` | `Split Value Currency` | `Spot Internal` |
| `Spot Market` | `Spot Rate` | `Spread` |
| `Start` | `Start Date` | `Start Of Day` |
| `Stock Exchange` | `Sub Account` | `Swap Points` |
| `Swap Type` | `T` | `Text` |
| `Third-Party` | `To` | `Total Interest` |
| `Total Settlement` | `Trade Currency` | `Trade Date` |
| `Trade Type` | `Treasury Front Office Root URL (for deep links)` | `Treasury Rate` |
| `Treasury Rate, Margin %` | `Txn Type` | `Type` |
| `User` | `Val` | `Valuation Date` |
| `Value` | `Value Date` | `Value Date 1` |
| `View Errors` | `View Warnings` | `What If` |
| `Whatif Update` | `Width` | `argin` |
| `ate` | `equals to` | `equity deal capture` |
| `er` | `greater than` | `less than` |
| `or` | `ounterparty` | `rofit` |
| `s` | `ue Date` | `ype` |


---


## Appendix B: Consolidated Field Reference


This appendix consolidates all field description tables from across the documentation, grouped by sub-module. This provides a single reference for all field definitions.


### Trade_Management - TFO (TFO)


**Misc**

| S.No | Parameters | Description |
|---|---|---|
| 1 | FX.PARAMETERS | The rules that determined the Foreign Exchange (FX) transactions are defined in the following files: Classifies spot and forward contracts, according to local central bank and internal reporting rules. Defines the spot default value date. Uses the OFS.SOURCE ID present in this field to perform FX.BULK.ORDER . Uses the version ID present in this field as VERSION to populate or create FX BULK DEAL master records. Defines default category code for spot, forward and swap transactions. Defines the precious metal currency codes, hence, any number of currency codes can be defined. Conditions under which deals are entered with split value dates. Indicators show if Profit & Loss (P&L) and EXCHADS entries are booked when revaluation of forward and spot contracts takes place. Creates rounding rule for transactions. The Cus Margin Default field determines if the FX Group Cond ID corresponding to a customer is defined in a FX contract or not (subjected to the existence of the condition priority setup in FX margin). The values accepted are Yes, No and None. If set as Yes, the FX Group Cond ID defaults from SEC.ACC.MASTER ( SAM ). If it is not available in SAM , it defaults from CUSTOMER.CHARGE . If set as No or None, the FX Group Cond ID does not default from SAM or CUSTOMER.CHARGE . However, the user can still define the margin percentage manually (together with treasury rate) and derive the customer rate in FX deal. |
| 2 | FX.POS.TYPE | Assigns profit centre to the trading position, which can be amended as desired. |
| 3 | FX.TRANSACTION.TYPE | Classifies the deal types. A record in this application can control the default value for category codes, revaluation types, and allows delivery and types of options processing. The existing records can be amended and new records can be created. |
| 4 | FX.GEN.CONDITION | Identifies a specific group of customers, which can be cross-related to the group condition table, to define conditions applicable to that group. The groups are determined based on customer details such as sector and target. The criteria used and their priority are specified in the Condition Priority file in the record whose ID is FX.MARGIN. |
| 5 | FX.GROUP.CONDITION | Defines the spread or margin percentage for a specific customer, group of customers or default group. When a group customer is defined, the FX Gen Condition record needs to exist before any associated group condition is specified. For an individual customer, the ID is C , whereas, the default group ID is generally assigned as either 99 or 999. |
| 6 | FX.COMM.GROUP | Defines spread or margin based on currency, and the amount that falls in a range and is used in FX contracts. The FX Commission Group ID field in SAM is used in FX.BULK.ORDER application, and a reference to SAM is used in FX.GROUP.CONDITION . Hence, the margin is given in absolute terms or referred to FX Commission Group ID (based on which the margin is applied in an FX deal). |

**Misc**

| S.No | Parameters | Description |
|---|---|---|
| 1 | FX Spot | FX Spot is a contract of buying or selling a currency, commodity or security for immediate settlement (payment and delivery) on the spot date at a spot Rprice. |
| 2 | FX Forward | FX Forward is a contract of buying and selling an asset or a currency at a predetermined spot rate at a specified date in the future (which is greater than the spot date). The predetermined rate is called as the Forward Rate. |
| 3 | FX Swap | FX Swap is an agreement between counterparties to exchange currency. The agreement involves swapping of principal and interest payments between two different currencies. |
| 4 | Precious Metal Deal | Precious Metal Deals involve trading in various precious metals such as gold, silver, palladium, platinum and so on, in spot, forward or swap rates depending on the types of deals entered. |
| 5 | Single-rate Option | Single-Rate Option is the deal of exchanging one currency for another. The delivery takes place between two specified dates at customer’s choice without incurring any penalty cost. The option occurs when the customer decides to take delivery of all or part of the transaction before the final value date. |
| 6 | Multi-rate Option | Multi-rate Option is the deal of exchanging one currency for another. The delivery takes place between two different option dates with different rates. The option occurs when the customer decides to take delivery of all or part of the transaction before the final value date. In this, the applied rate depends on the period delivery. |
| 7 | Internal Deals | Internal Deals allow transfers between different positions or dealer desks. Hence, there is no need for accounting entries, payments, advices and so on. The system automatically updates the position, when an internal forex spot or a forward deal is entered. |
| 8 | Broker Deal | Broker Deals are entered when the counterparty is not known. The user needs to enter BR as sub-type and associated brokers deals. Once the counterparty name is known, BR is removed and the counterparty details are entered in the deal. |
| 9 | NDF Vanilla Deal | Non Deliverable Forward (NDF) Vanilla Deals is an hedging strategy, where parties in the contract agree to settle the profit or loss prior to the expiration date of the contract. A vanilla NDF transaction has an agreed rate fixing date, which is two working days before the settlement date. |
| 10 | NDF Exotic Deal | An Exotic NDF Deal allows in setting the fixing date as any date before the vanilla date in the tenure of the transaction. The fixing profit is discounted, if the NDF is fixed and settled early. The discount amount is amortised from the settlement date to the value date of the NDF. |

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

**Deal Capture**

| Field | Description |
|---|---|
| Pay from A/C | Identifies which account (in the books) needs to be credited to settle the currency sold. On entering the counterparty and currency sold, the system displays the default account for the counterparty (if available). Otherwise, it uses the Nostro account. Input in this field is mandatory. To know more information, refer to help text of FX application in Temenos Transact . |
| Receive To A/C | Identifies which account (in the books) needs to be debited to the account for currency purchased. The defaulted account is based on SSI setup, which can be a customer, Nostro or Vostro account. However, the user can always override by typing or selecting from the drop-down list of the accounts present. Input in this field is mandatory. To know more, refer to help text of FX application in Temenos Transact . The system filters only the accounts with the same currency of the currency bought. |
| Counterparty SSI | Ensure to have the details of counterparty’s Nostro correspondent and account, when the settlement of the currency sold is done through a Nostro account. The system defaults this field when a record in AGENCY table is set for the Counterparty Customer ID along with their Nostro details. If not, it requires manual input except when the field Free Format address is used instead of this information. |
| Bank A/C Number | Holds the bank account number of the counterparty maintained with their correspondent. This information is used to send a payment message to the Nostro correspondent. Input in this drop-down field only accepts account number of the counterparty or beneficiary. |
| Free Format Address | Has the name in a free text format (maximum of 10 lines with up to 35 characters per line), when the counterparty’s correspondent bank does not have the customer ID. This information is then mapped to SWIFT confirmation and payment messages. |
| Bank To Bank Info | Provides instructions or additional information from the sending bank for the receiver. This field corresponds to Tag 72 on SWIFT messages and is not used for information for which another field is intended or instructions not required in a message. For contract confirmation using SWIFT mode, Bank to Bank information is mapped to Tag 72 of MT 300 and MT 600 messages. This field is used when the first multi-value has a code word followed by further information. All codewords need to be present on the SWIFT.CODE.WORDS file, and is enclosed between slashes ‘/’ at the beginning of the line. It allows a maximum of 6 lines of 35 characters (upper case alpha or numeric). |

**Deal Capture**

| Field | Description |
|---|---|
| Agreement Type | Defines the contract's agreement type. The drop-down field displays all the valid records present in FX.AGREEMENT.TYPE table. This field is available for both spot and forward deals. |
| Revaluation Type | Identifies the revaluation method to be used on forward contracts. The system handles five types of revaluation, which are: RB – Rebate method SL – Straight line IN – Interest method IH – Interest/hedged SF – Straight line funding This field is available for forward and swap deals. For spot deals, the revaluation type applied is SP and hence not applicable. To know more information on the revaluation types, refer to the Temenos Transact user guide and help text. |
| Limit Reference | Has the limit reference number for the counterparty, which the system defaults. If the counterparty or customer has multiple limit references for the same product and sub-products, the user can manually provide the desired limit reference. To know more information on Limits and this field, refer to the Temenos Transact user guide and help text. |
| Buy Currency Interest Rate | Identifies the interest rate applicable to the currency purchased. This field is required when the revaluation type selected is other than RB. If the revaluation type is other than RB, the system defaults the interest rate from Periodic Rate table (for base currency) or derives the rate (for non-base currency) based on the forward rate and interest rate applicable to Sell Currency Interest Rate. Input is allowed in one of the two fields (that is, Buy or Sell currency interest rate) and not both. This field is available for forward and swap deals. To know more information on this field, refer to the Temenos Transact user guide and help text. |
| Sell Currency Interest Rate | Identifies the interest rate applicable to the currency sold. This field is required when the revaluation type selected is other than RB. If revaluation type is other than RB, the system defaults the interest rate from Periodic Rate table (for base currency) or derives the rate (for non-base currency) based on the forward rate and the interest rate applicable to buy Currency Interest Rate. Input is allowed in one of the two fields (that is, Buy or Sell currency interest rate) and not both. This field is available for forward and swap deals. To know more information on this field, refer to the Temenos Transact user guide and help text. |
| Mature at Start Of Day | Indicates whether maturity processing takes place at the Start of the Day. If this field is left blank, the maturity processing takes place at the End of the Day. The value in this field defaults from the Sod Mat field in FX.TRANSACTION TYPE (if setup). To know more information on this field, refer to the Temenos Transact user guide and help text. |
| Notes | Allows the Dealer to record any unique information or free-form narrative on the first level input, which is referred by the back office. These details benefit the back-office user or record purpose. The user is allowed to input a maximum of 10 lines with up to 35 characters per line. |

**Deal Capture**

| Field | Description |
|---|---|
| Override | During the validation stage of an FX contract, the system provides the user with a series of screen override messages to indicate an anomaly. For example, the exchange rate varies by more than the variation tolerance predefined. |
| If the user confirms the override, the full text of the actual override message is stored for reference purposes only. |  |
| Record Status | Status of the record. Values are INAU, IHLD, INAO, RNAU and so on. |
| Current No | The number of times the record was edited. |
| Authori s er | The ID of the user who authorises the record. |
| Inputter | The ID of the user who inputs the record. |
| Date Time | Local zone date and time when the deal has been committed, according to the COMPANY table. |
| Company Code | Applicable company code on which the user is logged into. |
| Department Code | Defaults the user’s department code. |

**Deal Capture**

| Field | Description |
|---|---|
| Counterparty | To know more, refer to Counterparty . |
| Exotic | ND DEAL application supports two types of NDF: Vanilla – A standard NDF transaction type with agreed rate and valuation date (usually two working days before settlement date). In this type, the user cannot change the valuation date. Exotic – A variation that allows the fixing date to be set at any date during the life of the transaction before the vanilla date. If the NDF is fixed and settled ‘early’, the fixing profit or loss is discounted. The discount amount is amortised from the settlement date to the value date of the NDF. The check box identifies the type of deal entered. In particular, the system always opens an NDF vanilla and provides opportunity to the user to switch the type of transaction to Exotic by selecting the checkbox. When Exotic is not selected, the valuation date is calculated automatically based on the days entered in Def Fix Days field in Temenos Transact ND.PARAMETER table. In this case, being a Vanilla NDF, the user cannot modify the valuation date. When Exotic is selected, the system automatically updates the other fields, making the valuation date an amendable deal. |
| Currency Pair | To know more, refer to Currency Pair . |
| Deal Currency | This identifies the NDF currency, which is configured in ND.PARAMETER table. To know more on the configuration of NDF currencies, refer to the NDF user guide in Temenos Transact . |
| Settlement Currency | This indicates the deliverable currency used for the settlement amount. |
| Buy or Sell | To know more, refer to Buy or Sell . |
| Amount Bought or Sold | To know more, refer to Amount Bought or Sold . |
| Value Date | To know more, refer to Value Date . |
| Live Rate | To know more, refer to Live Rate . |
| Contract Price | To know more, refer to Contract Price . |
| Settlement Rate Source | This allows the Dealer to enter up to two settlement rate sources from where the settlement rates are fixed on the valuation date. This is a drop-down field with all the valid records in ND.SETTL.RATE.SOURCE table. |
| Valuation Date | This defaults by the fixing date on which the exchange rate is fixed. The date defaulted or modified cannot be later than the value date. The system automatically defaults the date using the data from Fixing Days of the corresponding Fixing Currency from ND.PARAMETER table. In Vanilla deals, the defaulted value is not changeable. In particular, the system always defaults a date according to the above parameters compared with the settlement date. |
| Settlement Date | This indicates the settlement date of the NDF contract. The system automatically defaults the value date in this field. The user can modify the date defaulted by the system. However, the date entered needs to be greater than the deal date and not later than the value date. |
| Marketing Exchange | To know more, refer to Marketing Exchange . |
| Treasury Rate | To know more, refer to Treasury Rate . |
| Exchange Profit | To know more, refer to Exchange Profit . |
| Dealer | To know more, refer to Dealer . |
| Contract Date | To know more, refer to Contract Date . |
| Limits | To know more, refer to Limits . |

**Deal Capture**

| Field | Description |
|---|---|
| Settlement Account | Indicates the settlement account. This is an account from which the settlement P&L amount is credited or debited.It is a drop-down field and the Dealer selects the required account. |
| Beneficiary | Used when the counterparty of the deal instructs to pay funds to another party who does not have an account with the bank. Entry in this field is accepted when the beneficiary is known to the bank (that is, it has a customer record for the beneficiary). |
| Counterparty Correspondent | Identifies the bank to which the counterparty wants to pay the settlement amount. This is either the bank of the counterparty or their nominated beneficiary. If the beneficiary is known to the bank (that is, a customer record exists), the customer number of the bank is entered in this field. If the beneficiary is not known, the details are entered in the Counterparty Correspondence Address field. |
| Counterparty Bank Account | Account number of the counterparty or nominated beneficiary at their correspondent bank. |
| Intermediary Bank | Identifies any intermediary bank involved in the transaction and is specified by the counterparty. If the intermediary is known (that is, there is an associated customer record), the customer number of the intermediary bank is entered in this field. If not, details are entered in the Intermediary Address field. |
| Receiver Bank | Receiver bank is the location where the funds are made available to the Receiver. |
| Counterparty Correspondence Address | Identifies the bank to which the counterparty wants to pay the settlement amount. This can either be the bank of the counterparty or their nominated beneficiary. If the bank is known (that is, a customer record exists), the details are entered in the Counterparty Correspondence No field. If the bank is not known, the address is entered in this multi-valued field, which has free-form text. |
| Bank to Bank Info | To know more, refer to Bank to Bank Info. |
| Beneficiary Address | Used when the counterparty of the deal directs to pay funds to another party who does not have an account with the bank. If the beneficiary is known to the Bank (that is, a customer record exists), the beneficiary details are entered in the Beneficiary No field. If the beneficiary is not known, the details are entered in this multi-value field, which has free-form text. |
| Intermediary Address | Identifies any intermediary bank involved in the transaction and is specified by the counterparty. If the intermediary is known to the bank (that is, an associated customer record exists), the customer number of the intermediary bank is entered in the Intermed Bk No field. If not, the details are entered in this field, which has free-form text. |
| Payment Narrative | Allows the user to enter free text narrative, which appears on payments related to the deal record. |
| Notes | To know more, refer to Notes. |
| Audit | To know more, refer to Audit . |

**Deal Capture**

| Field | Description |
|---|---|
| Currency | Currency information in which the MM deal is booked. ISO codes are used to standardise the structure of these records (that is, GBP, USD, AUD). Currency is a drop-down field. When the user clicks the currency field, all the existing records in CURRENCY is automatically listed in the dropdown. From here on, the user can select the desired record by clicking on the value. |
| Amount | Deal amount |
| Counterparty | Counterparty with whom the deal is made. Counterparty is an opposite party in a contract or financial transaction. A record needs to exist in the Temenos Transact CUSTOMER file. Any counterparty available on the Customer file is accepted. The customer record can be entered as a number or mnemonic. The liability number assigned to this counterparty in the customer file is used for the limit checking. The dealer can search for a counterparty by prefixing 'sn' (short name) or 'mn' (Mnemonic) with the search text which instantaneously performs a quick search for Counterparty Name, Short Name, or Mnemonic. The dealer can also search for a counterparty based on Counterparty ID. The below screenshots show the result of counterparty search with ‘mn’ and ‘sn’ as prefix followed by four letters. |
| Interest Rate and Margin | Interest rate related information of the MM deals. Type of interest rate can either be Fixed or Floating depending on the type of the contract. Rate is valid from the start of the current interest period or value date, for fixed maturity contracts and call or notice contracts. |
| Fixed Interest Rate | Fixed-rate to calculate the interest accrual, interest credit or debit from the counterparty. It is entered as a direct interest percentage: On the contract or as a fixed interest key mapped to PERIODIC.INTEREST table in Temenos Transact . Is inclusive of the margin, thus, the Margin field is not enabled for user inputs. If entered using a rate key, the user needs to specify the Margin (if required). The key can be entered as a valid PERIODIC.INTEREST record or selected from the drop-down list. It takes the rate automatically on selecting a valid PERIODIC.INTEREST key. |
| Floating Interest Rate | Floating rate at which the interest accrual, interest credit or debit from the counter are calculated. It is entered as an interest key, mapped to BASIC.INTEREST table or RFR record in PERIODIC.INTEREST table of Temenos Transact. If entered using a rate key, the margin needs to be specified (if required). The key can be entered as a valid rate key or selected from the drop-down list. The Total Interest field calculates the interest, on selecting a valid BASIC.INTEREST or RFR key. |
| Interest Schedule | Identifies the associated frequency of interest payment. The frequency of payments are as follows: Bullet Daily Weekly Fortnightly Monthly Quarterly Half-Yearly Yearly If it is defined as part of the EB.FREQUENCY table, the custom frequency needs to be entered. Bullet type of schedule is not available for call or notice maturity deals. |
| Interest Start Date | Start date of the current interest period. The user can input a value in this field, only when the value in the Interest Schedule field is not ‘Bullet’. |
| Negative Interest | Determines whether the interest rate can be negative. If the value is set as Yes, it enables the user to enter the negative interest rate. If set as No, the user is not allowed to enter any value. |
| Interest Basis | Describes the total interest computation. Special Interest Basis is available only for fixed maturity contracts. To know how to create a new interest basis or assign interest basis for the special category, refer to the Temenos Transact user guide. |
| Total Interest | Total amount of interest that the system calculates, when value date, principal amount, interest rate, period and day basis are given. |
| Method | Methods to book a deal. The deal can have a valid Broker Code (records available on the BROKER table of Temenos Transact ) or other methods (such as telex, Reuters, telephone) available on FX.DEAL.METHOD table of Temenos Transact . If the Broker is selected as the deal method, fields (such as brokerage currency and brokerage fees) are enabled for user input. |
| Broker Fee | Amount of brokerage paid to the broker account specified in the broker currency in BROKER table in Temenos Transact . The user can specify the flat amount to be credited to the broker account. This field is displayed only when the Broker is selected in the Counterparty drop-down list or Broker Name from the Method field. The Broker Fee currency highlighted is listed based on the currency specified in the CCY.FOR.PAYMENT in the Temenos Transact Broker record. The user can input any amount in a valid format for the currency specified above. |
| Dealer | Dealer desk position that needs to be updated by the deal being created. The dealer desk code is held on the position record, hence, the exchange position and PL can be shown at the dealer desk level. The logged-on user is assigned to a dealer desk, which is defaulted in this field. However, it can be modified. The user can click the star on the left of the dealer desk name to add items to the Favourites. To remove the item from the Favourites, the user can re-click the highlighted star. |
| Contract Date | Deal date of the contract that represents the agreed date between all the parties to the contract. This is usually the system date, and backdate value is allowed without an override. However, the system does not accept the forward contract date value during the input of the deal. |
| RF Rate | Stores the compounded Risk-Free Rate. This is a system updated field. |
| RFR Convention | Market convention for rate compounding or averaging. The MM application follows Lookback methodology. |
| RFR Lookback Type | Type of Lookback method applied for rate compounding or averaging. It has the following methods for rate calculation: Narrow Definition - Uses the original interest period day count with lookback For example, if Wednesday rate is used for Friday, apply the Friday’s weight (three days) to the Wednesday’s rate. Observation Shift - Uses the original day count of the lookback rate. For example, if Wednesday rate is used for Friday, apply the Wednesday’s weight (one day) to the Wednesday’s rate. |
| RFR Lookback Days | Number of Lookback days considered for RFR calculations. |

**Deal Capture**

| Field | Description |
|---|---|
| Counterparty Reference | Reference number that a customer specifies for the Place or Take. This field can be used as an input to be printed on all Advice and Confirmations (along with the Bank’s contract number). Hence, so long as the delivery mapping and formatting tables are set up to use this field as input on Temenos Transact . |
| Credit Account | Helps to identify the account number ( source or destination account) to which the drawdown amount is settled on the value date. |
| Counterparty Correspondent Bank | Identifies the beneficiary bank that is used to settle one of the following when the counterparty has requested external delivery of the proceeds of the transaction: The principal amount of taking contract types at maturity Placement contract types at drawdown This is used when the counterparty does not require the funds to be credited in the current account, instead of requests an external delivery of the funds to a bank different from where the Nostro account is maintained. |
| Counterparty Correspondent Address | Full name and address of a beneficiary bank, along with the Principal Amount, where no account details are maintained. |
| Beneficiary Account | Account details (Name or the Number) of the beneficiary to which the principal amount needs to be credited. It has third-party transfers, where the counterparty requests for external delivery of funds. If the counterparty provides such information, it is entered in this field. Any amendment to this field after contract authorisation is displayed on future principal disbursements. |
| Bank to Bank Info | Provides instruction or additional information from sending bank for the receiver or intermediary account with institution or beneficiary institution. It corresponds to the 72 fields on SWIFT messages, and cannot be used for information for which another field is intended, or instructions are not required in a message. If a user inputs any details, it is sent to the Receiver. Even after authorisation, this field can be amended. The input is used for future confirmations and payments. If the amount is sent to re-generated, it does not perform any payments. |
| Send Payment Message | Controls whether to send or suppress the Swift messages (MT202 and MT210), after authorisation of the deal. |
| Principal Liquidation Account | Identifies the account number to which the entries are made for the reimbursement of the principal at liquidation or maturity date. |
| Interest Liquidation Account | Identifies the account number to which the entries are made for the reimbursement of the interest of deposit type contracts. The input is necessary when the disposal of the interest account is different from the disposal of the principal account. |

**Deal Capture**

| Field | Description |
|---|---|
| Debit Account | Account number to which the debits are passed, to collect charges at drawdown date. It needs to be expressed in the currency of the contract. Thus, the liquidation account for the interest can also be expressed in the currency of the contract. |
| Code | Specifies the Profit and Loss category code (available as a record within Temenos Transact FT.CHARGE.TYPE or FT.COMMISSION.TYPE tables) where the amount of the charges, collected at drawdown, is credited. The charges can be handling fees, documentary tax stamps, drawdown fees, legal fees, and so on which are collected from the client directly on the drawdown date. |
| Amount | Identifies the flat amount of charges that need to be debited to the counterparty at the drawdown of the contract or when the principal is increased. The charges amount is defined in the currency of the contract. |

**Deal Capture**

| Field | Description |
|---|---|
| Product Category | Allows the user to amend the product category code according to the requirement. |
| Mature at Start of the Day | Specifies whether the deal matures at the Start of Day (SOD). |
| RFR Calc Method | Calculation method for RFR averaging: Compound Simple |
| RFR Spread Treatment | Spread treatment method during RFR averaging: Spread-Inclusive - Uses the spread within the averaging calculation along with daily rates. Spread-Exclusive - Adds the spread separately after RFR averaging is done. |

**Deal Capture**

| Field | Description |
|---|---|
| Currency | To know more, refer to Currency. |
| Amount | To know more, refer to Amount. |
| Counterparty | To know more, refer to Counterparty. |
| Interest Rate and Margin | To know more, refer to Interest Rate and Margin. |
| Interest Accrual and Maturity | On Fixed Maturity deals, the From field has the value date of the contract from which the system starts to accrue the interest. To know more information, refer to the Start Date user guide in Temenos Transact . The To field has the maturity date of the deal. |
| Interest Schedule | To know more, refer to Interest Schedule. |
| Interest Start Date | To know more, refer to Interest Start Date. |
| Negative Interest | To know more, refer to Negative Interest. |
| Capitalise Interest | This is part of Others tab as shown below: This indicates the requirement for automatic capitalisation of interest on interest due dates. If the value is selected as Yes, the system updates the principal amount automatically with the full amount of interest, and capitalisation continues until the final maturity date is reached. If the value is No, the capitalisation of interest is not allowed. |
| Interest Basis | To know more, refer to Interest Basis. |
| Total Interest | To know more, refer to Total Interest. |
| Method | To know more, refer to Method. |
| Broker Fee | To know more, refer to Broker Fee. |
| Dealer | To know more, refer to Dealer. |
| Contract Date | To know more, refer to Contract Date. |
| Limits | To know more, refer to Limits. |
| Settlement | To know more, refer to Settlement. |
| Charge | To know more, refer to Charge. |
| Other | To know more, refer to Other. |
| Audit | To know more, refer to Audit. |

**Deal Capture**

| Field | Description |
|---|---|
| Currency | To know more, refer to Currency. |
| Amount | To know more, refer to Amount. |
| Counterparty | To know more, refer to Counterparty. |
| Interest Rate and Margin | To know more, refer to Interest Rate and Margin. |
| Interest Accrual and Maturity | In Call or Notice deals: The From field has the value date of the contract from which the system starts to accrue the interest. To know more information, refer to Start Date in the Temenos Transact user guide. The To field on call or notice deals has the maturity date of the deal. However, the user is specifically provided with an option to drill-down by Call or Notice type based on the deal type. On selecting a Call, the user cannot input a maturity date, whereas if it is a Notice deal, the user can input between 1 - 999 days. |

**Deal Capture**

| Field | Description |
|---|---|
| Interest Schedule | To know more, refer to Interest Schedule. |
| Interest Start Date | To know more, refer to Interest Start Date. |
| Negative Interest | To know more, refer to Negative Interest. |
| Capitalise Interest | This is applicable for all the call or notice deals on the main Deal Details screen. The capitalisation of interest is not allowed when the negative interest rate is selected for the contract. |
| Liquidate Interest | The system requirement is that interest due date is specified for all call or notice contracts and Liquidate Interest field is applicable for all call or notice deals. This states whether interest is liquidated or deferred at the interest due date.\| The Interest fields control when the interest is due and whether the interest accrued is paid, received or not paid on this date. If the field is set to No, the system does not liquidate the interest on the due date but creates a new interest due date according to the input on Interest Schedule field. If set to Yes, the amount of interest is retained within the contract and liquidated on the next interest due date. |
| Interest Basis | To know more, refer to Interest Basis. |
| Total Interest | To know more, refer to Total Interest. |
| Method | To know more, refer to Method. |
| Broker Fee | To know more, refer to Broker Fee. |
| Dealer | To know more, refer to Dealer. |
| Contract Date | To know more, refer to Contract Date. |

**Deal Capture**

| Field | Description |
|---|---|
| Auto Rollover | The contract is rolled automatically on its maturity date. A rollover happens indefinitely unless the rollover details are cleared to allow the contract to mature on the defined date or date entered in the Final Maturity Date field (which holds the last rollover period). |
| Auto Capitalise Interest | The contract is rolled to capitalise (add to the Principal) the interest. |
| Auto Rollover Term | The period for which the contract can be rolled over. The term can be expressed as a number of days, weeks or months, and system validation is applicable to check whether the date returned is a working day. |
| Rollover Interest Rate | The new interest rate applicable when the contract is rolled over on the auto-rollover term. If the field is left blank, it defaults the interest rate from the existing contract. |
| Final Maturity Date | The final maturity date for a fixed-term contract subject to Auto Rollover Term. If the contract is set for Auto Rollover, the date needs to be greater than the maturity date. On reaching the final maturity date, the contract stops automatically roll over and matures. The rollover advice is inhibited for each maturity subject to Auto Rollover Term , and the Final Maturity can be further extended (if required). |
| Charge | To know more, refer to Charge. |
| Other | To know more, refer to Other. |
| Audit | To know more, refer to Audit. |

**Deal Capture**

| Field | Description |
|---|---|
| FRA Type | Specifies the underlying strategy of the FRA transaction. The two main types, that is Hedge and Trade, are decided based on the respective accounting treatment, exposure to interest rate risk and revaluation of positions. The field value is selected as Trade, by default. |
| Buy Sell | Specifies whether it is a Buy or Sell FRA. The field value is selected as Buy, by default. |
| FRA Currency | Currency code in which the FRA deal is booked. ISO codes are used to standardise the structure of these records (that is, GBP, USD, AUD and so on). The user can choose from the existing records in CURRENCY by clicking the records in the list. |
| FRA Amount | FRA amount of the contract. |
| Counterparty | Counterparty of the deal. The counterparty is an opposite party in a contract or financial transaction and a record needs to be available in the Temenos Transact customer file. The customer record can be entered as a number or mnemonic. The liability number assigned to this counterparty in the customer file is used for checking the limits. The dealer can search for a counterparty by prefixing 'sn' (short name) or 'mn' (Mnemonic) with the search text which instantaneously performs a quick search for Counterparty Name, Short Name, or Mnemonic. The dealer can also search for counterparty based on Counterparty ID. The below screenshots show the result of counterparty search with ‘mn’ and ‘sn’ as prefix followed by four letters. |
| FRA Rate | Future fixed the interest rate on the notional FRA Principal. It is set at the time of the FRA transaction. |
| Agreement Type | Defines the FRA deal. This is a mandatory field. |
| Marketing Exchange | Specifies whether the customer is a treasury customer or not. Selecting this field states that the customer is a non-treasury customer. It also displays Treasury Rate and Exchange Profit fields in the FRA Deal Capture screen for user input. |
| FRA Period, Start Date and Maturity Date | Two drop-down fields with the start and maturity periods of the FRA contract. The value in the Start Date field can be 0 to 98 months and Maturity Date field is 1 to 99 months. The Start Date field updates the value based on the selection in the first box, similarly, the Maturity Date updates the contract’s maturity date based on the selection on the second box. The field when updated calculates the spot date and adds up the period specified to get both Start and Maturity Dates. |
| Reference Rate | The variance allowed is selected in the PERIODIC.INTEREST table. This reference rate needs to be a valid record in the table for the currency selected. |
| Fixing Date | Specifies the date on which the prevailing interest rate is determined. Transactions happen for: Foreign currency two days prior to the start date The local currency on the same day |
| No. of Days | Indicates the number of days between Start Date and Maturity Date. This is a no-input field. |
| Reference Price | Represents the interest rate on the cash market applicable to the longest period of the FRA. It is applicable only for hedge type of contracts and the rate input is selected in PERIODIC.INTEREST table. |
| Treasury Rate | Applicable only when the Marketing Exchange field is selected. The text box field specifies the rate in case the customer is not a treasury customer. |
| Exchange Profit | Marketing exchange profit or loss amount is calculated on the contract date for a non-treasury customer. This field is displayed only when the Marketing Exchange field is selected in the contract. This is a no input field. |
| Method | Methods using which a deal can be booked. The deal can have a valid broker code (records available on the BROKER table of Temenos Transact ) or other methods available in FX.DEAL.METHOD table of Temenos Transact , such as Telex, Reuters, Telephone and so on. |
| Broker Currency and Broker Fees | These fields are updated when the Method is selected as Brokerage. Broker Currency is a drop-down field whereas Broker Fees is a text box for manual input. |
| Dealer | This identifies the dealer desk associated with the contract. |
| Contract Date | This specifies the deal or trade date of the contract. |

**Deal Capture**

| Field | Description |
|---|---|
| Receive To A/C | Account from which the settlement profit amount is received. The settlement account needs to match the currency of the contract. |
| Pay from A/C | Account from which the settlement loss amount is paid. The settlement account needs to match the currency of the contract. |
| Cpty Bank 1 | Counterparty bank where the payment of the settlement amount is made. Additionally, the customer requests for external delivery of funds and does not require it to be credited to the current account. |
| Cpty Bank 2 | Counterparty reference of the second beneficiary bank for the settlement amount. It is used where contracts involve four-party transfers of funds. |
| Beneficiary Address | Full name and address of a beneficiary bank along with the settlement amount, where no settlement details are maintained for the beneficiary account. |

**Deal Capture**

| Field | Description |
|---|---|
| Portfolio | Portfolio number to which the FRA contract is linked. It links the deal to the customer portfolios for overall management. |
| Business Centre | Business centres of the contract. |
| Position | Applicable for all trade buy and sell contracts, and not for hedge contracts. It specifies whether the contract is entered to open (create) a new FRA position or close an existing open FRA position. |
| Limit Reference | Limit reference applicable to the FRA transaction. |
| Mature at Start of the Day | Specifies whether the deal matures at the Start of the Day. |

**Deal Capture**

| Field | Description |
|---|---|
| Swap Type | Type of swap Two main type includes Interest Rate Swap and Currency Interest Rate Swap, which decide the nature of the principal used, interest repayment obligation and so on. |
| Trade Type | Essential strategy of the swap transaction Two main types include Hedge and Trade, which decide the respective accounting treatment, exposure to interest rate risk and revaluation of positions. If the Swap Type is selected as Cirson, the Trade Type field automatically defaults to Hedge. |
| Marketing Exchange | Specifies whether the customer is a treasury customer Click the treasury rate fields to select both the legs of the Swap Deal Capture screen for user input. This is a non-mandatory field. |
| Start Date | Starting date of the swap contract Value date from which the system starts to accrue interest. Therefore, the date entered needs to be prior to the maturity date of the contract. |
| Maturity Date | Termination date of the swap contract and the date when the deal is liquidated During liquidation, all the corresponding amounts of principal (if appropriate) and interest passes to the appropriate accounts as designated within the transaction. |
| Agreement Type | Swap deal agreement type |
| Principal Exchange | Specifies if the deal involves principal exchange and triggers the Principal Exchange (PX) and Principal Re-Exchange (RX) schedules within the swap contract. |
| Portfolio | Portfolio number to which the swap contract is linked |
| Dealer | Dealer desk associated with the contract |
| Contract Date | Deal or trade date of the contract |

**Deal Capture**

| Field | Description |
|---|---|
| Counterparty/Broker | Indicates trade is done with a counterparty or broker. This field filters the list of counterparties or only brokers based on the selection The dealer has an option to search for a counterparty by prefixing ‘sn’ (short name) or ‘mn’ (Mnemonic) with the search text which instantaneously performs a quick search for Counterparty Name, Short Name or Mnemonic. The dealer can also search for a counterparty based on the Counterparty ID. The below screenshots are an example of a counterparty search with ‘mn’ and ‘sn’ as prefix followed by four letters. |
| Counterparty/Broker Selection | Represents the Counterparty or Broker of the trade. Counterparty is a customer with whom the bank makes the contract. A valid record is on the Temenos Transact CUSTOMER.SECURITY file with the classification of the customer as Counterparty, Broker or Both. The dealer can search for a Counterparty or Broker by typing the Short Name and it does a text-based search for Counterparty/Broker Name, Short Name, Country Name or Counterparty/Broker Number. |
| Portfolio | The portfolio number or security account to which the security trade is linked. A valid record is available on the Temenos Transact SEC.ACC.MASTER application. The dealer can directly search for a portfolio by entering the Short Name or Portfolio Number. The dealer is directed to the portfolio inventory screen to view the portfolio holdings and valuation of the selected portfolios, on clicking the ellipsis icon (marked in brown) available next to the drop-down. |
| Side | This indicates whether the dealer buys or sells the security. |
| Security | Drop-down for bond selection to which the dealer has traded. A valid record is available on the Temenos Transact SECURITY.MASTER application with the classification as Bond. The dealer can search for a security by entering the Short Name or Security Number, ISIN, Sub Asset Type, Stock Exchange, cusipNumber and sedolNumber. The search is prefixed by ISIN, ST, EX, CUSIP or SEDOL. For example, to search for security using ISIN, the dealer must enter ISIN US0378331005. Dealer can view details of the security in the same deal capture window, click the first ellipsis icon (marked in brown) available next to the drop-down. Dealer is directed to the security inventory screen to view the security holdings and valuation across all the own book portfolios, click the second ellipsis icon (marked in brown). |
| Stock Exchange | Value defaults on selecting the security from the SECURITY.MASTER application. The value date and the charges and commissions for the trade are calculated based on the setup done in STOCK.EXCHANGE application. Dealer can change defaulted stock exchange at the trade level. |
| Trade Currency | The currency in which the transaction is dealt with the Broker or Counterparty concerned or the trade is settled. After security selection, the value defaults as the security currency from the SECURITY.MASTER application. |
| Nominal | Nominal amount (that is, the face value) of the security traded. |
| Price | The price at which the nominal is bought or sold. After security selection, the value defaults from the SECURITY.MASTER application. Dealer can change the defaulted price at the trade level. |
| Trade Date | This records the trade date. |
| Settlement Date | This records the date on which the settlement of the trade executed. Value defaults based on the setup available in STOCK.EXCHANGE application. |
| Interest Days | Number of days for which interest is accrued (from last payment date to settlement date) |
| Accrued Interest | Amount of interest accrued on the securities up to the settlement date. |
| Gross Amount | The gross value of the trade in trade currency terms. After entering the nominal and price, the system calculates the gross amount. To know more information on the calculation of the gross amount, refer to the Temenos Transact user guide. |
| Net Amount | The net value of the trade in trade currency terms. After entering the nominal and price, the system calculates the net amount. To know more information on the calculation of the gross amount, refer to the Temenos Transact user guide. |

**Deal Capture**

| Field | Description |
|---|---|
| Counterparty or Broker | Indicates trade is done with a counterparty or broker. This field filters the list of counterparties or only brokers based on the selection. The dealer has an option to search for a counterparty by prefixing ‘sn’ (short name) or ‘mn’ (Mnemonic) with the search text which instantaneously performs a quick search for Counterparty Name, Short Name or Mnemonic. The dealer can also search for a counterparty based on the Counterparty ID. The below screenshots are an example of a counterparty search with ‘mn’ and ‘sn’ as prefix followed by four letters. |
| Counterparty or Broker Selection | Counterparty or broker of the trade. Counterparty is a customer with whom the bank makes the contract. A valid record is available on the Temenos Transact CUSTOMER.SECURITY file with the classification of the customer as Counterparty or Broker or Both. Dealer can search for a Counterparty or Broker by typing Short Name and it does a text-based search for Counterparty or Broker Name, Short Name, Country Name or Counterparty or Broker Number. |
| Portfolio | Portfolio number or security account to which the security trade is linked. A valid record is available on the Temenos Transact SEC.ACC.MASTER application. Dealer can directly search for a portfolio by entering the Short Name or Portfolio Number. Dealer is directed to the Portfolio Inventory screen to view the portfolio holdings and valuation of the selected portfolio, when clicking the ellipsis icon (marked in brown) available next to the drop-down. |
| Side | The dealer buys or sells the security. |
| Security | This helps to select the equity, which the Dealer has traded. A valid record is available on the Temenos Transact SECURITY.MASTER application with the classification as Share. The dealer can search for a security by entering the Short Name or Security Number, ISIN, Sub Asset Type, Stock Exchange, cusipNumber and sedolNumber. The search is prefixed using ISIN, ST, EX, CUSIP or SEDOL. For example, to search for security using ISIN, the dealer must enter ISIN US0378331005. Dealer can view details of the security in the same deal capture by clicking the first ellipsis icon available next to the drop-down. Dealer can view the security holdings and valuation across all the own book portfolios by clicking the second ellipsis icon. |
| Stock Exchange | Defaults on selecting the security from the SECURITY.MASTER application. The value date and the charges and commissions for the trade are calculated based on the setup in STOCK.EXCHANGE application. Dealer can change defaulted stock exchange at the trade level. |
| Trade Currency | Currency in which the transaction is dealt with the Broker or Counterparty concerned and trade is settled. After security selection, the value defaults as the security currency from the SECURITY.MASTER application. |
| Nominal | Nominal amount (that is the face value) of the security traded. |
| Price | Price at which the nominal is bought or sold. After security selection, the value defaults from the SECURITY.MASTER application. Dealer can change the defaulted price at the trade level. |
| Trade Date | Records the trade date. |
| Settlement Date | The date on which the settlement of the trade is executed. Value defaults based on the setup available in STOCK.EXCHANGE application. |
| Gross Amount | The gross value of the trade in trade currency terms. After entering the nominal and price, the system calculates the gross amount. To know more information on the calculation of the gross amount, refer to the Temenos Transact user guide. |
| Net Amount | The net value of the trade in trade currency terms. After entering the nominal and price, the system calculates the net amount. To know more information on the calculation of the net amount, refer to the Temenos Transact user guide |

**Deal Capture**

| Field | Description |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| Deal Type | Characteristics of a REPO contract. The value entered determines whether the contract is REPO or reverse REPO. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Counterparty | Counterparty with whom the deal is made. A valid record needs to exist in the Temenos Transact customer file. The customer record can be entered as a number or mnemonic. The liability number assigned to this counterparty in the customer file is used for the limit checking. The Dealer has the option to search for a counterparty by prefixing 'sn' (short name) or 'mn' (Mnemonic) with the search text which instantaneously performs a quick search for Counterparty Name, Short Name or Mnemonic. The dealer can also search for the counterparty based on the Counterparty ID. The below screenshots show the result of the counterparty search with ‘mn’ and ‘sn’ as prefixes followed by four letters. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Own Book | Portfolio number to which the REPO trade is linked. A valid record needs to exist in the Temenos Transact SEC.ACC.MASTER application. The Dealer can perform the following: Search for a portfolio by entering the short name or portfolio number. Click the ellipsis icon next to the drop-down, to view the portfolio holdings and valuation of the selected portfolio in the Portfolio Inventory screen. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Trade Date | The date on which the trade is made. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Txn Type | Specifies whether the deal is cash or security-driven. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Currency | Currency in which the REPO deal is booked. The user can choose from the existing records in CURRENCY by clicking the records in the list. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Interest Basis | Basis considered for total interest computation. The basis can be given as follows: Fixed Term Call - Notice 360/360 360/360 366/360 366/360 366/365 366/365 365/365 365/365 252/252 252/252 21/252 21/252 360/365 360/365 SPECIAL - Special Interest Basis is available only for fixed interest rate contracts. To create a new or assign an Interest Basis for the Special category, refer to Temenos Transact user guide. | Fixed Term | Call - Notice | 360/360 | 360/360 | 366/360 | 366/360 | 366/365 | 366/365 | 365/365 | 365/365 | 252/252 | 252/252 | 21/252 | 21/252 | 360/365 | 360/365 | SPECIAL | - |
| Fixed Term | Call - Notice |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 360/360 | 360/360 |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 366/360 | 366/360 |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 366/365 | 366/365 |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 365/365 | 365/365 |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 252/252 | 252/252 |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 21/252 | 21/252 |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 360/365 | 360/365 |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| SPECIAL | - |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Agreement | Agreement type for the contract. This is applicable for both legs of Repo or Reverse Repo. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Issue Date | The date on which the trade is to be effected. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Issue Amount | Price for the first leg of the REPO contract, specified in the Currency field. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Repurchase Date | The date on which the Repo contract matures. The securities return to the Seller and Buyer receives the repurchase amount specified in the contract on this date. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Repurchase Amount | Price for the second leg of repo contract. If the value is not entered, it populates from Temenos Transact after validation. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Rate Type | Specifies whether the contract is a fixed or floating rate contract. The other related fields are no input field as shown in the below screenshots based on the Rate Type field. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Repo Rate | Rate of interest for the REPO contract. Applicable for fixed REPO contracts. In the case of floating rate REPOs, the total interest is displayed after validation and the same is made as no input field. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Rate Key Floating | Rate of interest for the REPO contract. Applicable for floating rate REPO contract. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Interest Term | Period or frequency to re-fix the REPO contract. Available as the number of days, weeks or months. Applicable for floating rate REPO contract. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Interest Spread | Spread associated to calculate the overall interest rate of the REPO contract. Applicable for floating rate REPO contract. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Rate Selection | Determines whether the rate is BID or OFFER from the Temenos Transact PERIODIC.INTEREST table. Applicable for floating rate REPO contract. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| Next Fixing Date | The date on which the next rate change is applicable to the contract. Applicable for floating rate REPO contract. |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |

**Misc**

| Field | Description |
|---|---|
| Language | Set the language for the system. The user has the option to switch between multiple languages. (Currently, it supports English and French ) |
| Auto Refresh FX Rates | Refresh system-wide FX rates automatically (set to Yes) or manually (set to No). |
| FX Rates Refresh Interval (S) | Set the FX rates to refresh interval in seconds. |
| Auto Refresh Blotter | Refresh the trade blotters automatically (set to Yes) or manually (set to No) to update the blotters with new trades. |
| Auto Refresh Positions | The option to refresh FX Positions to automatic (set to Yes) or manual (set to No). |
| Positions in Thousands | Show the amounts in thousands (set to Yes) or the full figures (set to No) on the Position screens in the system. |
| Auto Show Reuters Widget | Control the auto display of the Reuters widget on the upper-right of the Deal capture screen, when a user selects a Currency Pair. |
| Open Dashboard after Login | If set to Yes, the Dashboard is set on the homepage and appears after the user logs on to the system. |
| Fit Dashboard to Screen | If set to Yes, the Dashboard is auto-adjusted to fit the width of the browser. |
| Save | Save user settings. |

**Positions**

| Option | Description |
|---|---|
| None | Does not show any value |
| Total | Adds or subtracts all the values present in the selected column to provide the total amount |
| Average | Displays the calculated mathematical average of all the values present in the selected column |
| Weighted Average | Displays the value calculated according to predefined parameters |
| Count | Counts the values present in the selected column |

**Positions**

| Field | Description |
|---|---|
| New Column Name | Inputs any alphanumerical character |
| Width | Defines the width of the column |
| Right Align | Displays data to the right of the column |
| Place Column | Decides if the column shows at the end or before another column. The default setup cannot be modified. Therefore, the first created column always shows in the end. Dealer can modify the position of the added columns but not the default columns. |
| Default Formula | Creates a default formula, which is used for all the lines. Enters any numerical characters and inserts the column name Default formula is (Cost – Market Rate) * 100. Dealer can override this formula in the individual field, by right-clicking and inserting a new formula. |
| Decimal Places | Decides on the number of decimal places displayed |
| Commas | Decides whether the commas are shown or not. For example, 1000 or 1,000 |
| If Result is | Decides the formatting of the result. It allows the following values: less than , greater than and equals to Dealer can assign a format for each of these values |

**Positions**

| Field | Description |
|---|---|
| New Column Name | Inputs any alphanumerical character |
| Width | Defines the width of the column |
| Right Align | Displays data to the right of the column |
| Place Column | Decides if the column shows at the end or before another column The default setup cannot be modified. Therefore, the first created column always shows in the end. Dealer can modify the position of the added columns but not the default columns. |
| Default Formula | Creates a default formula, which is used for all the lines Enters any numerical characters and inserts the column name Default formula is (Cost – Market Rate) * 100. Dealer can override this formula in the individual field, by right-clicking and inserting a new formula. |
| Decimal Places | Decides on the number of decimal places displayed |
| Commas | Decides whether the commas are shown or not. For example, 1000 or 1,000 |
| If Result is | Decides the formatting of the result It allows the following values: Less than Greater than and equals Dealer can assign a format for each of these values The colours of the new columns are not implemented. However, the system can display the colours according to the Dealer’s inputs. |

**Positions**

| Position | Description |
|---|---|
| AL | Related to matured deals |
| Spot | Deals that are due to mature in the spot period |
| Forward | Deals that are due to mature beyond the spot period |
| Net | Net of AL, Spot and Forward Positions |

**Positions**

| Field | Description |
|---|---|
| Adding Favourite Currency | To know more, refer to Adding Favourite Currency |
| Sorting | To know more, refer to Sorting |
| Search | To know more, refer to Search |
| Adding/Editing Columns | To know more, refer to Adding or Editing Columns |
| Default Button | To know more, Refer to Default button |
| Common Functionalities | To know more, refer to Common Functionalities |
| Editing the Layout | To know more, refer to Editing the Blotter Layout |
| Downloading and Printing Position Views | To know more, refer to Downloading and Printing Position Views |

**Positions**

| Field | Description |
|---|---|
| Adding Favourite Currency | To know more, refer to Adding Favourite Currency |
| Search | To know more, refer to Search |
| Adding/Editing Columns | To know more, refer to Adding or Editing Columns |
| Default Button | To know more, refer to the Default button |
| Common Functionalities | To know more, refer to Common Functionalities |
| Display Graph | This allows the user to display or hide the graph when not required. To perform this, click . |
| Editing the Layout | To know more, refer to Editing the Blotter Layout |
| Downloading and Printing Position Views | To know more, refer to Downloading and Printing Position Views |

**Positions**

| Field | Description |
|---|---|
| Search | To know more, refer to Search |
| Adding/Editing Columns | To know more, refer to Adding or Editing Columns |
| Default Button | To know more, refer to Default button |
| Common Functionalities | To know more, refer to Common Functionalities |
| Editing the Layout | To know more, refer to Editing the Blotter Layout |
| Downloading and Printing Position Views | To know more, refer to Downloading and Printing Position Views |

**Positions**

| Feature | Description |
|---|---|
| Search | To know more, refer to Search |
| Adding or Editing Columns | To know more, refer to Adding or Editing Columns |
| Default Button | To know more, refer to the Default button |
| Common Functionalities | To know more, refer to Common Functionalities |
| Editing the Layout | To know more, refer to Editing the Blotter Layout |

**Positions**

| Field | Description |
|---|---|
| Search | To know more, refer to Search |
| Adding or Editing Columns | To know more, refer to Adding or Editing Columns |
| Default Button | To know more, refer to the Default button |
| Common Functionalities | To know more, refer to Common Functionalities |
| Editing the Layout | To know more, refer to Editing the Blotter Layout |


---
