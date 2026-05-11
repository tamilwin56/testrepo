
# Temenos Transact — Staff_Channel Module Documentation


> **Comprehensive User Guide**
> Generated: 13 April 2026
> Content: Configuration | Reference | Field Descriptions | Glossary


## Table of Contents

  - [Staff_Channel Module Overview](#staff_channel-module-overview)
    - [Sub-Module Summary](#sub-module-summary)
    - [How to Use This Guide](#how-to-use-this-guide)
  - [Chapter 1: Staff_Channel - TT](#chapter-1-staff_channel---tt)
    - [Features in Staff_Channel - TT](#features-in-staff_channel---tt)
    - [1.1  Cheque Issue Management](#11-cheque-issue-management)
    - [1.2  Draft Management](#12-draft-management)
    - [1.3  Duplicate Check for Teller Transactions](#13-duplicate-check-for-teller-transactions)
    - [1.4  Managing Tills](#14-managing-tills)
    - [1.5  Misc](#15-misc)
    - [1.6  Multi Line Teller](#16-multi-line-teller)
    - [1.7  Multi Tills](#17-multi-tills)
    - [1.8  Multi Valued Teller](#18-multi-valued-teller)
    - [1.9  Passbook Printing](#19-passbook-printing)
    - [1.10  Preferential Pricing for FCY transactions](#110-preferential-pricing-for-fcy-transactions)
    - [1.11  Stock Control](#111-stock-control)
    - [1.12  Teller Default](#112-teller-default)
    - [1.13  Teller Financial Services](#113-teller-financial-services)
  - [Appendix A: Glossary of T24 Applications & Fields](#appendix-a-glossary-of-t24-applications-fields)
    - [Applications](#applications)
    - [Fields Referenced](#fields-referenced)
  - [Appendix B: Consolidated Field Reference](#appendix-b-consolidated-field-reference)
    - [Staff_Channel - TT (TT)](#staff_channel---tt-tt)

---


## Staff_Channel Module Overview


This document provides comprehensive documentation for the **Staff_Channel** module of Temenos Transact. It covers **1 sub-modules** with a total of **13 feature areas**.


### Sub-Module Summary


| # | Sub-Module | Code | Features | Description |
|---|-----------|------|----------|-------------|
| 1 | **Staff_Channel - TT** | `TT` | 13 | Staff_Channel - TT module of Temenos Transact |


### How to Use This Guide


Each feature in this document is organized into the following sections:

- 📖 **Introduction** — Overview and purpose of the feature
- ⚙️ **Configuration** — How to set up and configure the feature
- 🔧 **Working With** — Operational usage and field descriptions
- 📋 **Tasks** — Step-by-step procedures
- 📊 **Outputs** — Reports, enquiries, and generated outputs

Each feature includes a **Quick Reference Card** at the top with application names, key fields, prerequisites, and a summary. Appendices provide a full glossary, consolidated field tables, and end-to-end use-case scenarios.

---


## Chapter 1: Staff_Channel - TT


Staff_Channel - TT module of Temenos Transact


### Features in Staff_Channel - TT


| # | Feature | Sections |
|---|---------|----------|
| 1.1 | Cheque Issue Management | Confi |
| 1.2 | Draft Management | Intro, Confi, Worki, Tasks, Outpu |
| 1.3 | Duplicate Check for Teller Transactions | Intro, Confi, Worki, Tasks, Outpu |
| 1.4 | Managing Tills | Intro, Confi, Worki, Tasks, Outpu |
| 1.5 | Misc | Intro |
| 1.6 | Multi Line Teller | Intro, Confi, Worki, Tasks, Outpu |
| 1.7 | Multi Tills | Intro, Confi, Worki, Tasks, Outpu |
| 1.8 | Multi Valued Teller | Intro, Confi, Worki, Tasks, Outpu |
| 1.9 | Passbook Printing | Intro, Confi, Worki, Tasks, Outpu |
| 1.10 | Preferential Pricing for FCY transactions | Intro, Confi, Worki, Tasks, Outpu |
| 1.11 | Stock Control | Intro, Confi, Worki, Tasks, Outpu |
| 1.12 | Teller Default | Intro, Confi, Worki, Tasks, Outpu |
| 1.13 | Teller Financial Services | Intro, Confi, Worki, Tasks, Outpu |


### 1.1  Cheque Issue Management


> **📇 Quick Reference Card**
> 
> **Sections:** ⚙️ Configuration


#### ⚙️ Configuration

This section covers the applications used to configure Cheque Issue and Management.


##### ConfiguringSTOCK.PARAMETER

The STOCK.PARAMETER is the top-level parameter for creating and maintaining different types of stock of:

- Cheques
- Bankers cheques
- Drafts
- Fixed Deposit receipts
- Credit cards

The following screenshot shows the STOCK.PARAMETER for cheque.

The accepted IDs for this application are:

- CHQ for Cheque
- BCHQ for Bankers Cheque
- DRAFT for Demand Drafts
- FDR for Fixed Deposit Receipts
- CARD for Credit / Debit cards

The Stock Reg Id field in the STOCK.PARAMETER application can be used to define a combination of values using which the stock is updated in STOCK.REGISTER . This field can contain the following values:

- Company Code
- Department Code
- Local Table
- Co Code-dept Code
- Dept Code-local Tab
- Co Code-local Tab.

This provides the convenience of maintaining stock at different levels within the organization.

The Stock No Mask field identifies the mask the user wants to apply to the instrument numbers for the instruments (Cheque, Bankers cheque, Drafts, Fixed Deposit Receipts (FDR) or Credit cards). Input in this field must contain '#' characters. Number of '#' characters defines the maximum length of the instrument. First character can be R, which means that the account number is right justified and it can contain leading zeros.

- If the Cheque Number is 1234 and the Mask is #####, the display is 1234.
- If the Cheque Number is 1234 and the Mask is R#####, the Cheque Number is displayed as 01234.


##### ConfiguringCHEQUE.TYPE

This application holds the details of each type of cheque supported by the Cheque Control System.

The following screenshot shows the CHEQUE.TYPE record CURR (for Category 1001).

A Cheque Type is defined as a four-letter code.

- CURR – Current Account Cheque
- EURO – Euro Cheque

Each cheque type can be assigned a maximum and minimum holding, a default issue quantity (number of cheques in a book) and a notice period to allow reports to be produced for accounts requiring automatic reissue.

A list of account categories to which cheque can be issued is also recorded for each cheque type. Auto Reorder Type is defined if the reorder has to be based on a cheque number of the cheques held by the account holder. The Max Represent Number field in CHEQUE.TYPE defines how many times a cheque can be represented following a return.


##### ConfiguringSTOCK.ENTRY

The STOCK.ENTRY application is used to record inward or outward printed stock of stationery like cheque and Fixed Deposit Receipts (FDR). Any successful entry updates the STOCK.REGISTER table. Through this application, the stock details like Cheque Type , Stock Series , Stock Start Number , Stock Quantity and Stock Account Number are captured.

Given below is an example of STOCK.ENTRY for a corporate account.

Movement from one stock register to another can also be entered. It also forms the Stock Series based on CHEQUE.TYPE*STOCK.SERIES*STOCK.ACCT.NO, if the account number for which the stock has been received is noted in the STOCK.ENTRY . An example for inclusion of account number at the STOCK.ENTRY level would be interest or dividend warrants to be issued by a corporate.


##### ConfiguringSTOCK.REGISTER

The following screenshot shows the STOCK.REGISTER updated as CHEQUE.TYPE*SERIES*ACCOUNT.NO.

---


### 1.2  Draft Management


> **📇 Quick Reference Card**
> 
> **Purpose:** *Demand drafts issue is handled via the FUNDS.TRANSFER and TELLER applications in Temenos Transact . Retails banks that issue demand drafts maintain an inventory of the same. The need for maintenance of the inventory is to maintain an audit considering they are written orders issued by the bank to it...*
> 
> **Applications:** `CHEQUE.REGISTER.SUPPLEMENT`, `CHEQUE.TYPE`, `STOCK.ENTRY`, `STOCK.PARAMETER`, `TELLER`
> 
> **Key Fields:** *Assigned Category*, *Cheque Type*, *Internal*, *Issue Cheque Type*, *Payee Name*, *Stock Number*, *Stock Reg Id*, *Validate Payee Name* ... +1 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Demand drafts issue is handled via the FUNDS.TRANSFER and TELLER applications in Temenos Transact . Retails banks that issue demand drafts maintain an inventory of the same. The need for maintenance of the inventory is to maintain an audit considering they are written orders issued by the bank to its correspondents and the details need to be cross checked at the time of payment of these drafts. The bank and its agents will pay the beneficiary when the demand draft is deposited and cleared by the beneficiary’s bank.

CHEQUE.REGISTER.SUPPLEMENT table holds various statuses like issued presented, cleared, exception, unknown, cancelled, stopped, and returned. Hence the current status of a draft can be known by referring this application.

Cheque Type field and TELLER application aids in classifying an instrument as cheque or drafts. Additional validations like validating the payee name, validating the draft number can also be handled in this table.

The Draft Issue Management section contains detailed setup information and other information for functions like receipt of stock, issue, charges and stop payment instructions for drafts. The setup for receipt and update of stock into Temenos Transact is similar to Cheque issue with slight differences.


#### ⚙️ Configuration

The following section describes the draft management configuration parameters.


##### STOCK.PARAMETER

This table allows defining of top level parameters for different types of Drafts.

The Stock Reg Id field in the STOCK.PARAMETER application can be used to define a combination of values using which the stock is updated in the STOCK.REGISTER . This field can contain values COMPANY.CODE, DEPARTMENT.CODE, LOCAL.TABLE, CO.CODE-DEPT.CODE, DEPT.CODE-LOCAL.TAB or CO.CODE-LOCAL.TAB. This provides the convenience of maintaining stock at different levels within the organization.


##### CHEQUE.TYPE

There are certain fields that are needed to be updated for draft issue functionality. A unique CHEQUE.TYPE for drafts needs to be created.

Since the credit is to an internal suspense account, the Assigned Category field is populated with the related category and Internal field is set to Yes.

The format of the Internal Category code is : CCYCCCCCSSSS

- CCY stands for Currency
- CCCCC stands for Category and
- SSSS stands for Subdivision code from the Company.

Generally any demand draft issued by a bank has a limited period of validity. This information is provided in the Validity field to enable the system to track expired drafts. Any buyer of a draft is expected to either cancel or renew the draft which is past its validity period.

The payee name of an incoming draft (issued by the same bank) can be validated when the same is presented, say, through local clearing. For this the Validate Payee Name field has to be set a Yes. This serves as a basic security feature against forged drafts.


##### STOCK.ENTRY

Stock of draft can be maintained at various levels within the bank. This functionality is similar to STOCK.ENTRY for Cheque. Read Stock Entry section under Cheque issue management for more information.


#### 🔧 Working With

The following sections describe operations that can be done on drafts.


##### Draft Issue throughTELLER

The Cheque number is input in Stock Number field along with the Cheque Type and Payee Name in Issue Cheque Type and Payee Name fields of the TELLER application, respectively.

Teller transaction record showing the credit going into an internal account, as defined in the CHEQUE.TYPE .

Below is a CHEQUE.REGISTER.SUPPLEMENT record for a draft issued through TELLER .


##### CHEQUE.REGISTER.SUPPLEMENT

The drafts are issued on a bank internal account and it is possible to record the drawer account information in CHEQUE.REGISTER.SUPPLEMENT application along with the main details of the drafts issued by the bank.

In addition, every time a cheque or draft is returned or rejected, a return counter is incremented to track the number of times the instrument been returned or rejected.


##### Payment of Draft

Drafts are handled for payment through FUNDS.TRANSFER or TELLER. Duly presented and paid drafts are recorded in CHEQUE.REGISTER.SUPPLEMENT by the system.

The same is handed over by a customer for payment across the counter and paid through TELLER application as below:

The status change is shown below.

If payment has been stopped for a draft, when presented, override is produced when draft number is entered and committed in FT (Funds Transfer) or DC (Data Capture) or TT (Teller Transaction) applications. If a draft is returned for other reasons, draft number can be recorded in CHEQUE.REGISTER.SUPPLEMENT . It is automatically updated by the cheque control system and only restricted functions are allowed to update the usage of cheques held.

The payee name of an incoming draft (issued by the same bank) can be validated when the same is presented, say, through local clearing. For this the Validate Payee Name field in the relevant CHEQUE.TYPE record has to be set to Yes. This serves as a basic security feature against forged drafts.


##### Cancellation of a Draft

There are many instances that may require cancellation of the Draft purchased by the Customer. In such cases the Draft is cancelled by reversing the original transaction, subject to the STATUS of the related CHEQUE.REGISTER.SUPPLEMENT record being ISSUED. The demand draft is also physically returned to the bank, in such cases.


#### 📋 Tasks

Related topics:

- Execute Travellers Cheque Encashment
- Transfer Travellers Cheque Stock from Vault To Till
- Teller Processes

There are no specific tasks for the Draft Management feature.


#### 📊 Outputs

The Draft Issue Management section contains detailed setup information and other information for functions like receipt of TC stock, buy or sell TC against cash and so on.


##### Enquiries and Reports

In Draft Management, the user can view the below enquiries and reports:

TC Buy Today

This enquiry displays the Traveller's Cheques purchased today.

TC Position

This enquiry displays the Traveller's Cheque Position of the Teller. The Teller can perform the following activities:

- Transfer of TC Stock to Other Branch
- Transfer of TC from Vault to Till
- Transfer of TC from Till to Vault

TC Sell Today

This enquiry displays the list of Traveler's Cheque issued today.

TC Stock Balance

This enquiry displays the Traveller's Cheque stock by Teller or Branch.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA


> **Related Applications:** `CHEQUE.REGISTER.SUPPLEMENT`, `CHEQUE.TYPE`, `STOCK.ENTRY`, `STOCK.PARAMETER`, `TELLER`

---


### 1.3  Duplicate Check for Teller Transactions


> **📇 Quick Reference Card**
> 
> **Purpose:** *A user-defined framework is available for setting up a Duplicate Check functionality for transactions input through the TELLER module.*
> 
> **Key Fields:** *Arrangement*, *Cheque Bank Cde*, *Cheque No*, *Cheque Number*, *Debit Account*, *Withdrawal Amount*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

A user-defined framework is available for setting up a Duplicate Check functionality for transactions input through the TELLER module.

A wide variety of transactions can be configured easily in Temenos Transact by the menu system or by using role based home pages and can be customised for each user or bank. Also, various risk mitigation functions such as Teller limits, maker checker concept, stock control, duplicate checks and so on are also incorporated for better transaction and operation control.


#### ⚙️ Configuration

Duplicate teller transactions can be identified using the standard EB.DUPLICATE.TYPE framework. This table allows the user to define the field(s) to be evaluated to confirm if it’s a duplicate or not. EB.DUPLICATE.TYPE is linked using the TELLER.TRANSACTION application, as it is a mandatory input.

The TELLER.TRANSACTION application supports the definition of multiple EB.DUPLICATE.TYPE records.

A TT.CHEQUE.DEPOSIT duplicate check record is created in EB.DUPLICATE.TYPE application, for the TELLER application to check duplicates based on two fields in the TELLER application namely Cheque Number and Cheque Bank Cde . These fields represent the cheque number and bank code against which the cheque is drawn.

Next, the TT.CHEQUE.DEPOSIT EB.DUPLICATE.TYPE record is added to the appropriate TELLER.TRANSACTION record through the Duplicate Check field.


#### 🔧 Working With

When the bank user triggers the transaction with a Teller Transaction code which contains Teller Cheque Deposit duplicate check code, an override is raised to indicate a possible duplicate transaction.

Teller triggers a transaction for cheque deposit into a customer’s account with a Cheque Number and Cheque Bank Cde . The transaction is successfully processed.

The Duplicate Check functionality is setup based on the above two fields.

Transaction Code- 41, Cheque Number-045698 and Bank Code-23456

Consider a scenario in which the same cheque is picked for processing for the 2nd instance by the teller in the bank, when user triggers the cheque deposit transaction with the same Cheque Number and Bank Code, an override is raised.

Transaction Code- 41, Cheque Number-045698 and Bank Code-23456

The override message carries the teller transaction reference number.

Other Considerations:

- Multiple duplicate check records can be attached to Teller Transaction type.
- The duplicate check is run only against the Teller fields chosen by the user based on the EB Duplicate Type record defined.
- The system allows a flexible framework through which the user can define any field(s) from Teller as part of the duplicate check record to trigger the check when Teller entries are input.


#### 📋 Tasks

Duplicate teller transactions can be identified using the standard EB.DUPLICATE.TYPE framework. This table allows the user to define the fields to evaluate and confirm if the transaction is duplicate or not. EB.DUPLICATE.TYPE is linked using the TELLER.TRANSACTION application, as it is a mandatory entery.


##### Workflow

This section allows the user to perform the below activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Cash Withdrawal Local . |
| Cash Deposit Local | Enter an account arrangement ID in the Arrangement field and then click the FIND button. Enter values in the following fields: Withdrawal Amount Debit Account Cheque No Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

There are no Outputs available for Duplicate Check for Teller Transactions feature.

---


### 1.4  Managing Tills


> **📇 Quick Reference Card**
> 
> **Purpose:** *This section explains different operations that can be performed in a till by the user.*
> 
> **Key Fields:** *Amount Foreign*, *Amount Local*, *Central Bank Acct*, *Comments*, *Currency*, *Denomination details*, *Deposit Amount*, *Enter Balance* ... +17 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

This section explains different operations that can be performed in a till by the user.


#### ⚙️ Configuration

There are no configuration details available for this section.


#### 🔧 Working With

This section deals with the opening and closing of tills, along with the associated enquiries.


##### Opening Tills

To use a till ( TELLER.ID ), it must be opened and assigned to a specific user. The system ensures that only that user can input transactions to that till. It is possible to change the current teller or user without closing the till by assigning a different user. Normally, each morning it is a common practice for the teller to visually check the cash in their till prior to beginning the day’s work. In Temenos Transact the teller opens the till.


##### Closing Tills

Closing of the till can comprise of several operations:

- Balancing the till by the amount of currencies
- Balancing the till by entering the denominations (thereby calculating the amount)
- Compensating where the till is short in a currency
- Compensating where the till is over in a currency
- Authorising the till closure

The closing of a till allows the teller to balance the actual contents of the till against the balance held by the system. On closure, the teller is prompted for the till balance (in each currency) and this is compared to the current system balance.

Alternatively, if the teller has been set to use denominations, the entering of the number of units in each denomination (that is, 150 USD100 bills is USD15000.00) forces the physical count to agree the till balance to the cash account.

If a difference is found, then an override is required. Clicking yes to the override automatically adjusts the system balance to the till balance and posts the balancing entries to the over account and short account records defined in the TELLER.PARAMETER file.

When forcing the till closing by denominations, it is preferable to set-up a special version that requires the input of each number of units of the held currencies. The next screenshot gives an indication of this but shows the balance as well for information.

> **⚠️ Note:** When re opening the till, the system checks if the system balance has not moved since the last closure. If this is the case, then the till cannot be opened until the system balance is adjusted (via DATA.CAPTURE ) to match the till closing balance.


##### Enquiries

TELLER.POSITION enquiry shown below displays the balances of a specific Tellers tills

The TELLER.OVERALL enquiry shows the teller positions of all the tills in each currency.


#### 📋 Tasks

Related topics:

- Receive Cash from Central Bank
- Transfer Cash from Till to Vault
- Transfer Cash from Vault to Till
- Transferring Cash Between Tills
- Create New Till
- Transfer Travellers Cheque Stock to Other Branches
- Transfer Travellers Cheque Stock from Vault To Till
- Teller Processes

Teller application is meant to service the retail cash operations of the bank, which includes cash deposit and withdrawals, buying and selling foreign currencies and account to account transfers. It also undertakes traveller’s cheques, cheques sent for collection, transfers from till to till and also from and to the vault.

The Home screen is designed to assist the Head Teller in authorising transactions, to know cash balances of all the Tellers and Vault, Vault Cash Position, TC Stock Positions and Provision to enter necessary transactions of a Head Teller.


##### Workflow

Managing Tills related activities are listed below:

This option allows the user to open the Closed Till before starting Teller operations for the day. Till can be opened either by Head Teller or Teller by assigning to a specific user. On every business day, the Till is opened to carry out the cash transactions. On opening the Till, the required cash balance is transferred from vault.

To open a Till, perform the following steps:

1. Cash Position .
2. Select the Open Till option from the drop-down, corresponding to a record.
3. Click the Launch icon.
4. In the New Till Creation screen, in the Teller ID tab, enter values in the following fields: Till Status Teller Update Stock Passbook Device Comments
5. Click the Validate icon to check for errors and overrides.
6. Click the Commit icon to submit the record.

This option allows the vault user to transfer the cash from the Vault to the Till for the Till user to make the cash payments. The available balance with the Till user is transferred to the vault at the close of the business.

To transfer cash from the Vault to the Till, perform the following steps:

1. Transfer Cash from Vault to Till .
2. Click the New Deal icon.
3. Enter values in the following fields: To Teller Currency Amount Local Amount Foreign Narrative Denomination details
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon to submit the record.

This option allows the Teller or Head Teller to receive cash from Central bank. When the Branch is in need of cash and the branch Vault Position shows a deficit balance, then the Teller or Head Teller can request for Cash transfer from Central Bank.

To transfer cash from Central Bank, perform the following steps:

1. Cash from Central Bank .
2. Click the New Deal icon.
3. Enter values in the following fields: Deposit Amount Central Bank Acct Narrative Denomination details
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon to submit the record.

This option allows the Teller to transfer the surplus cash with the Branch to the Central Bank. When the Vault Position of the Branch exceeds the limits of holding cash in the vault, then the teller has to transfer the surplus cash to the Central Bank.

To transfer cash to Central Bank, perform the following steps:

1. Cash to Central Bank .
2. Click the New Deal icon.
3. Enter values in the following fields: LCY Amount Central Bank Acct Narrative Denomination details
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon to submit the record.

This option allows the Till user to transfer the cash from the Till to the Vault, to account for the transactions completed by the Till user for the day.

To transfer cash to Till to Vault, perform the following steps:

1. Transfer Cash from Till to Vault .
2. Click the New Deal icon.
3. Enter values in the following fields: From Teller Amount Local Narrative Denomination details
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon to submit the record.

This option allows the user to close the open Till to end the Teller operations for the day. Till can be closed either by Head Teller or Teller by assigning to a specific user. On every business day, the till is closed to carry out close of business for the day. While closing the till, the available cash balance is either transferred to the Vault or kept in a separate till or box of the Teller (in such case, there is no need to transfer the cash to the vault).

To close a Till, perform the following steps:

1. Close Till .
2. Select the Close Till option from the drop-down.
3. Click the Launch icon.
4. Enter values in the following fields: Till Status Enter Balance Comments
5. Click the Validate icon to check for errors and overrides.
6. Click the Commit icon to submit the record.

Using this option, Head Teller can assign the Till to another user when the already assigned user is on leave.

To change the Till user, perform the following steps:

1. Change Till User .
2. Click the Reassign Till icon.
3. Enter values in the following fields: Teller Comments
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon to submit the record.

This option allows the user to reopen the closed Till before starting Teller operations for the day. Till can be opened either by Head Teller or Teller by assigning to a specific user. On every business day, the till is opened to carry out the cash transactions and closed at the close of business for the day. On opening the till, the required cash balance is transferred from Vault and on closing the current Till, balance is transferred back to Vault.

To reopen a Till, perform the following steps:

1. Reopen Till .
2. Click the Reopen Till icon.
3. Enter values in the following fields: Till Status Notes
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon to submit the record.

This option allows the Teller to transfer cash from one Teller to another Teller.

To transfer a Till - Local Currency, follow the below steps:

1. Till Transfer – Local .
2. Select the Till Transfer – Local option from the drop-down.
3. Click the Launch icon.
4. Enter values in the following fields: Teller Amount Local Narrative
5. Click the Validate icon to check for errors and overrides.
6. Click the Commit icon to submit the record.

This option allows the Teller to transfer foreign currency from one teller to another teller.

To transfer a Till - Foreign Currency, follow the below steps:

1. Till Transfer – Foreign .
2. Select the Till Transfer – Foreign option from the drop-down.
3. Click the Launch icon.
4. Enter values in the following fields: To Teller Currency Foreign Currency Amount Narrative
5. Click the Validate icon to check for errors and overrides.
6. Click the Commit icon to submit the record.

This option allows the Teller or Head Teller to transfer the TC stock from one branch to another branch. The branch can transfer the surplus TC stock held with the branch or on request of other branch, the transfer can be initiated.

To transfer TC to other branches, follow the below steps:

1. TC Position .
2. Click the Trans of Stock-Oth Branch icon.
3. Enter values in the following fields: TC Amount TC Account TC Contra Account TC Currency
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon to submit the record.

This option allows the Teller to transfer the TC stock from Vault to individual Till in the same branch. Once the TC stock is updated to the Tills, the Teller can carry out Buying and Selling of TC Stock.

To Transfer TC from Vault to Till, follow the below steps:

1. TC Position .
2. Click the TC Vault to Till icon.
3. Enter values in the following fields: TC Amount Vault Account Till Account TC Currency Till Id
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon to submit the record.


#### 📊 Outputs

There are no Outputs available for Managing Tills feature.

---


### 1.5  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *The TELLER module in Temenos Transact processes a variety of retail transactions. It is an account based application for moving funds. It incorporates the administration of tills, processing of local and foreign currency transactions, travelers’ cheques, currency transfers, denomination control, pas...*
> 
> **Applications:** `ACCOUNT.STATEMENT`, `BC.SORT.CODE`, `CARD.ISSUE`, `DEAL.SLIP.FORMAT`, `DENOM.TYPE`, `FUNDS.TRANSFER`, `TELLER`, `TELLER. TRANSACTION` ... +12 more
> 
> **Key Fields:** *Charge Account*, *Chg Type*, *Exp Split Amt*, *Exp Split Date*, *Tran category*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- Temenos Transact Services

The TELLER module in Temenos Transact processes a variety of retail transactions. It is an account based application for moving funds. It incorporates the administration of tills, processing of local and foreign currency transactions, travelers’ cheques, currency transfers, denomination control, passbook updates, advice production, automatic charges defaulting, and rate defaulting.

The variety of transactions can be configured easily in Temenos Transact by the menu system or by using role based home pages and can be customised for each user or bank. Also, various risk mitigation functions such as teller limits, maker checker concept, stock control and so on are also incorporated for better transaction and operation control.


##### Configuring Teller

Although the system processes many types of transactions, the basic mechanism for balancing entries, defaulting rates and charges remains the same. Hence all transactions are processed by the one application ( TELLER ), but the screen prompts can be varied by tailored VERSION with specific defaults being controlled by a TELLER.TRANSACTION .

Each transaction prepares two balancing accounting entries (more when charges are present). Invariably, one side is the client (side 1) and the balancing entry is the teller cash account (side 2), that is, a simple cash deposit entails a credit to the customer account and a debit to the teller cash account.

In the Teller system, the cash that is held at a teller's position is recorded in an internal account defined as:

For Example : USD-10000-0012

The Cash Category is specified in the TELLER.PARAMETER file. It is the balance of these account records, it can be reconciled with the actual cash when the till is closed.

Cheques have to be posted directly to the collection accounts and not held by the teller (defined in TELLER.TRANSACTION ). This allows for easy reconciliation of funds as each cheque is recorded as a separate entry to this account.

It is possible to specify an exposure date on the teller contract, which is used to decide when the funds credited gets updated to the cleared balance on the account record. It is also possible to clear funds on a single teller transaction on multiple dates. This information is entered in the exposure date ladder fields ( Exp Split Date and Exp Split Amt ). Although the splitting information can be entered manually, they may also be made to default using either the TRANSACTION record or the BC.SORT.CODE record. Read Local Clearing and System Table for further information on setting up exposure date splitting defaults.

It is also possible to default the value date on the credit side by specifying a sort code that points to a BC.SORT.CODE record set up with a default value date period.

The Till Limits functionality helps currency wise till level limits to be maintained in each till based on the setup in TELLER.ID . The limits, whenever breached by a teller transaction, raises necessary overrides. Also, overrides are raised (whenever a till is opened or closed) when limit definitions are not made for currencies found in the stock, but the limit field is set in TELLER.ID .

Charges for customers’ account to account transfer transaction can be collected from any account. This allows flexibility to collect charges either from the remitter, beneficiary or a third party account.

Chg Type field in TELLER.TRANSACTION and TELLER applications and Charge Account field at TELLER level allow the user to specify the charge account .The charge account can be in any currency.

- It is possible to capture the card number attached to the debit account in the transaction.
- The card number has to be entered in the Card Number field at the time of transaction.
- There are validations are to check that the card number input has been issued to the debit account number.
- If a different card number is entered, the system gives an override message.
- If the card number does not exist, the system gives an error message.
- It is also possible to capture the details of the card transaction in a text field.

The following two functions are performed at the COB for TT.END.OF.DAY Teller transactions.

- Remove any unauthorized transactions and place on hold.
- Transfer all authorized transactions to history. This means that under normal circumstances, the transaction file is empty at the start of each day.
- If passbook processing is active, then the TELLER.PASSBOOK.STMT COB process updates the ACCOUNT.STATEMENT and the associated files with the details of passbooks updated on that day (see TELLER.PBOOK.PRINTED ).
- This process emulates the updates that take place if a statement had been produced.
- A passbook update is viewed as a statement by the system.

Profit and Loss (P and L) entries in Foreign Currency (FCY) can be entered in TELLER . The functionality is similar to the FUNDS.TRANSFER application. The other leg of the teller transaction must also be of the same FCY, otherwise the system produces the error message as shown in the image below.

Advices can be printed from any teller transaction. The format and content is user definable through the DEAL.SLIP.FORMAT application.

To define an advice, the details have to be entered into the DEAL.SLIP.FORMAT application. This file describes the data that has to be extracted from the deal and where, on an advice, it has to be printed. It also allows free format text, totaling and data to be extracted from associated files.

This advice can now be linked to an individual transaction, by entering the DEAL.SLIP.FORMAT key into the Advice Version field of the TELLER.TRANSACTION record. If the advice has to be printed by default, then the Print Advice field in the TELLER.TRANSACTION record has to be set to Y. An override can be requested if the teller does not produce the advice. The below image shows how a specific DEAL.SLIP.FORMAT record is assigned to TELLER. TRANSACTION

The advice is printed whenever the Prt Hotkey is depressed (defined on the TERMINAL record) or if the DEAL SLIP button is clicked when using the browser. The advice can be printed at any stage during the transaction, which means that the customer prior to committing the transaction can sign the advice.


##### Illustrating Model Parameters

The following are the model parameters related to Teller.

It defines the category and transaction codes to be used for balancing tills, Tran category to be used for cash, rounding details for local currency and the vault ID.

This defines the defaults and validation to be used for teller transactions. It also defines the accounts for both sides of the transaction, the charges (if any), the transaction codes, Curr Mkt and duplicate check to check for the occurrence of any duplicate contracts.

This parameter defines the description and value of the denominations in use for each currency. It also defines the units, coins and notes in use for each currency. A prerequisite to setting up this parameter, is to set up the appropriate DENOM.TYPE like Cash, Travellers Cheque, and so on.

This parameter allows the user to define the format of the data output on a savings account passbook. The SYSTEM record is the only one allowed in this parameter.

This parameter for authorisation is used to pick up the appropriate versions while amending or deleting or authorising the teller transactions through the menu and home Pages. If the input version is not specified in this parameter file, then while amending, authorising or deleting the teller transaction, the TELLER application is launched instead of the version that is used to input the transaction.

This parameter is used to define the various denomination types like Cash, Gift vouchers, Travellers cheque, and so on that can be attached to the TELLER.DENOMINATION , so that denominations in teller transaction can be filtered based on the denom types.

The Teller Financial Services (TFS) applications allow the user to enter multiple financial transactions on the same screen and commit all of them as one transaction. This application is the main transaction at front end. It captures the user input data and creates a TELLER or FT or a DC batch in the backend.


##### Illustrating Model Products

Model Products are not applicable for this module.


> **Related Applications:** `ACCOUNT.STATEMENT`, `BC.SORT.CODE`, `CARD.ISSUE`, `DEAL.SLIP.FORMAT`, `DENOM.TYPE`, `FUNDS.TRANSFER`, `TELLER`, `TELLER. TRANSACTION`, `TELLER.DENOMINATION`, `TELLER.ID`, `TELLER.PARAMETER`, `TELLER.PASSBOOK`, `TELLER.PASSBOOK.STMT`, `TELLER.PBOOK.PRINTED`, `TELLER.TRANSACTION`, `TERMINAL`, `TFS.PARAMETER`, `TRANSACTION`, `TT.END.OF.DAY`, `TT.TELLER.HP.VERSIONS`

---


### 1.6  Multi Line Teller


> **📇 Quick Reference Card**
> 
> **Purpose:** *Multi-line Teller (MLT)deals are unique to users operating with the Desktop interface.*
> 
> **Applications:** `TT.GROUP.CONDITION`
> 
> **Key Fields:** *Chg Discount Amt*, *Chg Maximum Amt*, *Chg Minimum Amt*, *Chg Premium Amt*, *Maximum Amt*, *Minimum Amt*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Multi-line Teller (MLT)deals are unique to users operating with the Desktop interface.

A multi-line deal is comprised of a master transaction containing links to each child or leg and controls the overall charges and accounting of the set. The words leg and child have the same meaning within the context of multi-leg transactions.

The purpose of multi-line deals is to progress from the original design of teller, which was essentially a two entry transaction (a credit and a debit). For example, the sale of one foreign currency against local; with default charging this could mean that a customer with three transactions is charged more commission overall; or the teller has to adjust the charges manually.

Multi-line deals allow the user to process multiple sale transactions whilst building a running total for charge or commissions. The total of sales is taken into consideration before applying defaults such as minimum commissions.

To invoke a multi-line deal instead of using F3 to get the next ID, enter the character ‘-‘ in place of the ID. Then, the system uses multi-line transaction IDs.

There are a few considerations to take into account when using multi-line transactions:

1. There has to be only one client in the set of legs comprising the multi-line deal.
2. Charges are calculated taking the multi-line as a complete unit.
3. Charges can be standard or modified when entering the details.
4. Deal Slips for Multi-line deals are produced via Enquiries.
5. Only Multi-line deals can use the Copy function.
6. Authorization, Reversal and Copy are done via the Master Deal only.


##### Multi – Line Teller andTT.GROUP.CONDITION

In the case of MLT, all the legs belong to the same customer and charges are consolidated and applied based on the type. So if the contract group is constructed based on a field of the CUSTOMER , all legs has the same contract group, and the relevant charge concessions defined in TT.GROUP.CONDITION is applied. If contract groups are based on some other criteria, and if the contract groups are not the same across the legs of the MLT, then TT.GROUP.CONDITION is not supported.

It is also possible to define maximum and minimum amounts of charges, together with a discount or premium, at an individual customer level or for a group of customers. This action overrules the Maximum Amt and Minimum Amt fields specified in the generic charge record.

The following fields of TT.GROUP.CONDITION define the special conditions applicable to specific groups of customers or individual customers:

- Chg Maximum Amt defines the maximum amount to be charged for which the Charge Type applies.
- Chg Minimum Amt defines the minimum amount to be charged for which the Charge Type applies.
- Chg Discount Amt specifies the amount to be deducted from the Charge amount calculated.
- Chg Premium Amt specifies the amount to be added to the Charge amount calculated.


##### Multi-line Charging

Charging on Multi-line deals differs from single line deals. Each charge type is taken from each separate TELLER.TRANSACTION used on the legs of the deal. Each charge type is then applied across the total balance across all the legs of the deal. The amount of each charge is stored on the header record for the multi-line deal. The charges are all calculated at the Local currency and converted to the currency of the first leg and posted to the corresponding account.


##### Special Function handling

The standard Temenos Transact functions operate slightly differently on MLT. The following features are specific to multi-line.

Copy on a MLT only works if performed on a header portion of a multi-line deal. It serves to copy the entire multi-line deal to a new set of ID’s. The copy is done leg by leg and the header is rebuilt after each individual copy (this means that if between original input and copy the charges on the TELLER.TRANSACTIONS used change, the copied deal have different amounts to the original). All unique data (Cheque serial numbers and so on) is deleted and the Teller ID is replaced with the ID of the currently signed on teller. Once the copy function has been run and the system has the ID of the new deal, pressing F3 or entering ‘-‘ brings up the next available ID. There is no way of zero authorizing a MLT copy. If any of the legs of a multi-line deal are in hold status then the deal does not copy.

Delete works the same as in other applications. The only difference being if a leg is deleted from a multi-line deal it rebuilds the header. If the line header is deleted, then it deletes in turn each leg. To maintain the integrity of the deal, it rebuilds the header after each leg it deletes.

It is now possible to reverse any one of the child records. The master deal gets rebuilt with the remaining child records.

Authorise can only be performed on header records. It then goes through each leg and authorizes them individually. If any legs are in hold status then the authorisation is not allowed.


#### ⚙️ Configuration

There are no configuration details available for this section.


#### 🔧 Working With

The following section describes the Multi-Line Teller operations available.


##### Multi-Line Usage

Consider an example where selling two currencies to a client, and receiving payment and commissions in local currency. The menu item can be chosen for this TELLER, SELLFM and system selects input mode for user.

It is convenient to allow the system to generate the next ID. This is done by entering the character ‘-‘ in the ID and committing the record.

It then transposed into the correct ID format as:

The user has provided the data. It is done only when the user completes the deal and presses F5 or the Commit Data toolbar icon that the special processing starts to become apparent.

Note: The transaction ID is TT/00084/00044-01, which indicates the user is in multi-line mode and this is the first leg of the deal.

Depending on whether the VERSION is set for Zero, authoriser input or requires a separate authoriser. The next dialog box may appear different.

With a zero authoriser, the deal can be completed (Finish). This button does not appear at this stage if the deal needs an independent authoriser.


##### Multi-Line Choices

This option allows the user prefers to add further deals to the multi-line set. A fresh input screen opens and the ID is incremented. In the example earlier, it is started with TT/00084/00044-01 and the next number is TT/00084/00044-02.

This option allows the user to modify the charges across a multi-line deal. It is covered in the modifying multi-line charging section of this guide.

This simply exits the user from the current deal. Similar to finishing a normal deal

For Zero Authoriser VERSION only user also has:

It triggers the authorisation of all the legs of the deal. If any of the legs are on hold, the authorisation process stops. If an override message is generated on any leg that requires an independent authoriser, the deal remains as unauthorised (usually status INAO) until such authorisation is provided.

Click the Next button and do the second leg of the deal:

On committing the data, the system allows the user to choose:

- FINISH - The deal and all the legs are authorised. Accounting, especially the charges are finalised.
- NEXT - A new input screen opens with the incremented ID.
- EXIT - There is an opportunity to come back and do further deals (defer the FINISH).
- MODIFY - There are more options as discussed later.

* The accounting updates are processed real-time for each leg, the charges are calculated but may change with further input.


##### Master and Child Deals

The master deal raised from the above example is shown in the following screenshot:

The user can view the individual IDs of the multi-line legs, the accounting information, and in this case the IDs of the accounting items (including the charges). There is no need of a version for this information.

The child deals are where the majority of the transaction data is held as shown below.


##### Modifying Multi-Line Charging

At the end of each leg, the user has the opportunity to modify the charge over the entire multi line deal. This is done by clicking the Modify button. This then gives the user three options. Waive, Modify and Standard.

- WAIVE -This option waives the charge completely from the entire multi line deal.
- MODIFY - This option takes the user to a new dialog box that asks them the account to post the charges to. The accounts appear as buttons with the account’s mnemonic or account number, if there is no mnemonic. Once the user has chosen the account to post to, they are prompted to choose the amount in the account currency to post as a charge. This process is shown below where the user chooses to post 200 Australian dollars to the account with the FREDAUD mnemonic.
- STANDARD - This option reverts the charges of the multi-line deal to the default charges that would have normally been levied across it.


#### 📋 Tasks

There are no Tasks available for Multi Line Teller feature.


#### 📊 Outputs

There are no Outputs available for Multi Line Teller feature.


> **Related Applications:** `TT.GROUP.CONDITION`

---


### 1.7  Multi Tills


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Multi-Tills (or Cash Bag) feature enables a single user to have more than one TELLER.ID depending on the set-up enunciated in the TELLER.PARAMETER application. Further, Multi-Tills contain a limited amount of cash transferred from the safe. Whenever there is a shortage of cash, instead of drawin...*
> 
> **Key Fields:** *Linked Tills*, *Max Tills*, *Multi Tills*, *Till Trf Only*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The Multi-Tills (or Cash Bag) feature enables a single user to have more than one TELLER.ID depending on the set-up enunciated in the TELLER.PARAMETER application. Further, Multi-Tills contain a limited amount of cash transferred from the safe. Whenever there is a shortage of cash, instead of drawing from the safe ,cash is transferred from the Multi-Tills. On the contrary if the till cash balance exceeds the permissible limits, then it is transferred to Multi-Tills. In short, it is possible to call the Multi-Tills as an intermediary between the safe and the till. The set-up, features of Multi-Tills are detailed in the following section.


#### ⚙️ Configuration

The basic set-up required for the functioning of Multi -Tills has to be made in the TELLER.PARAMETER application.

The trigger to Multi-Tills functionality is based on inputs in two fields in the TELLER.PARAMETER application.

- Multi Tills Permitted values are Yes and Null. If yes, the Max Tills field is a mandatory input. Multi-Tills functionality (that is, two or more tills for a user) is made available.
- Max Tills Any numeric, between 1-99 can be input. When input , it represents the number of tills a user can keep open at any given time when dealing with Multi-Tills . The input in this field can be changed at any time. Once changed , the new input is effective and earlier validations becomes null and void. For example, if Max Tills is input as three and then changed to two, any attempt to input more than two tills subsequently results in the Other tills must be closed error message.

For Multi Tills , once this set-up is made, the attaching of more than one teller ID is done through the TELLER.ID application. More than one teller ID (for a user) is permitted, only if the Multi Tills field is set to YES else an error is raised in case this field is set to null.

In TELLER.PARAMETER the Max Tills is set to two. That means a user can have a maximum of two tills and any attempt to input more than two, results in system raising an error as shown in the below screenshot.


#### 🔧 Working With


##### Linked Tills

This is set up using two fields in TELLER.ID application. They are:

Linked Tills

- This field can be input with any valid TELLER.ID
- The ID that is input has to belong to the same user, else the system raises an error.

Till Trf Only

- This field can take either YES or null.
- If input as YES , the TELLER.ID can do only till-to-till transfer.
- If a transaction representing other than till-to-till transfer is input, the system raises an error. The input in the field can be changed by the user at any time.

The above screen shot indicates how the TELLER.ID 0003 (for the same user) is linked to the TELLER.ID 0002 using the Linked Tills field.

In the above screenshot,

- The Linked Tills is a multi-value field. So for a user, if there are more than two tills, it can be linked by multi-valuing the field.
- TELLER.ID 0002 is main till and 0003 is linked till since in TELLER.ID 0002, the 0003 ID is provided in the Linked Tills field.

The Linked Tills functionality in Multi-Tills facilitates the following:

- Able to link two or more tills belonging to a particular user.
- Able to open the linked tills automatically when the master till is opened.

Illustration- In the above screenshot:

- User LISA2 has two tills - Till 0002 and Till 0003.
- Till 0002 is the master till and Till 0003 is called the linked or child till.
- Therefore, when Till 0002 is opened, then Till 0003 should also be opened automatically.

- This is applicable to only opening of tills. Closure of tills has to be done individually following traditional teller concepts.
- In the above case, if the user also had one more till, for example 0005, and consider it has not been linked to till 0002, then opening of till 0002 does not result in opening of till 0005,since it has not been linked.

Instead of TELLER.ID 0002, if TELLER.ID 0006 is linked (user is LISA2), the system raises a Till does not exist for Current User error at check fields( as shown in the screen shot below)

If the user has only one teller ID, the teller ID is defaulted at the transaction level. However, with the evolution of multi-tills, the till used to log into the teller application is the one that is automatically defaulted, unless it is changed at the application level.


#### 📋 Tasks

Related topics:

- Reopen Till

There are no Tasks available for Multi-Tills feature.


#### 📊 Outputs

There are no Outputs available for Multi-Tills feature.

---


### 1.8  Multi Valued Teller


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Teller module in Temenos Transact facilitates the management of tills, processing of local and foreign currency transactions, travelers cheques, denomination control, passbook printing, and so on.*
> 
> **Key Fields:** *Account*, *Account Number*, *Amount*, *Charge Account*, *Credit Account Number*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The Teller module in Temenos Transact facilitates the management of tills, processing of local and foreign currency transactions, travelers cheques, denomination control, passbook printing, and so on.

Additionaly, multi-value of certain fields is allowed to facilitate credit or debit to more than one account. This facility can also be used for passing on credit directly to various accounts of a customer out of a single cheque proceeds without routing the same through suspense accounts. This helps in updating the passbook online, but the actual availability of the amount is only after the clearance of the cheque.

For example, a single cheque can be deposited for credit to three accounts by multi-valuing the Credit Account Number and Amount fields.


#### ⚙️ Configuration

There are no configuration details available for this section.


#### 🔧 Working With

The procedure of creating a multi-value transaction is as follows:

A TELLER.TRANSACTION has to be defined for each type of transaction. Since multi-valuing is permitted only on side -1, new TELLER.TRANSACTIONS have to be defined with the transaction codes, currency and type of accounts that have to be multi-valued. The values input on side -1 are automatically defaulted on side – 2.

For example, if a cheque of USD 10,000 is deposited and has to be credited to three accounts AC1, AC2 and AC3, then while processing the teller transaction, credit fields can be multi-valued if the same are defined on side –1, of the TELLER.TRANSACTION .

The currency must be the same and all the three accounts should belong to the same customer. No cross currency is allowed. The multi-valued accounts can also include internal accounts.

In the above transaction, if two accounts of the same customer are used, a single CHEQUE.COLLECTION is created showing credit to both the accounts.

In the CHEQUE.COLLECTION application, the Account and the Amount fields can be multi-valued on side -1 only. These fields are defaulted from the credit side of the TELLER record.

Charge levied on any of the teller transaction (wherein either the credit or the debit side is multi-valued) is collected from the first account and the account is defaulted in Charge Account . Any further change in the charges, either during the teller transaction or during CHEQUE.COLLECTION , affects the first account only.

- The validations for using the above facility are as follows:
- The currency of the accounts have to be the same.
- Accounts must belong to the same customer.
- The multi-valued side can include internal accounts also.

In the case of multi-line teller transactions, in each leg of transaction, the Account Number can be multi-valued as per the details defined on side -1, of the TELLER.TRANSACTION .


#### 📋 Tasks

Related topics:

- Execute LCY Cash Deposit
- Execute FCY Cash Deposit

There are no Tasks available for Multi Valued Teller feature.


#### 📊 Outputs

There are no Outputs available for Multi Valued Teller feature.

---


### 1.9  Passbook Printing


> **📇 Quick Reference Card**
> 
> **Purpose:** *Passbooks can be issued to savings accounts (see ACCOUNT.CLASS and ACCOUNT ). When an entry is passed across a passbook account from any application, the details are recorded and the TELLER system updates the passbook when it is presented.*
> 
> **Key Fields:** *Arrangement*, *Attribute*, *Currency*, *End Date*, *Fixed Amount*, *GB Narrative*, *Line No*, *Line, Page No* ... +9 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Passbooks can be issued to savings accounts (see ACCOUNT.CLASS and ACCOUNT ). When an entry is passed across a passbook account from any application, the details are recorded and the TELLER system updates the passbook when it is presented.

The layout of the passbook has to be defined in the TELLER.PASSBOOK application. This describes the physical dimensions of the book in addition to header type information. For example, customer name and address, and positions of the debit or credit columns. The entire content of the passbook is user definable. Read TELLER.PASSBOOK for more details.


#### ⚙️ Configuration

To set up the system for passbook printing, do the following:

1. Define the TELLER.PASSBOOK format.
2. Define the device on the appropriate TELLER.ID .
3. Ensure that the TERMINAL can support a local print function.
4. Sets up any printer attributes see TELLER.ID and PRINTER.ATTRIBUTES .

This definition has the client details printed when

- A new book is issued (NEW),
- The balance carried forward as the first line of each page (FIRST) and
- The entries themselves on each detail line (LINE).

It also defines the dimensions of the passbook and any printer attributes that have to be downloaded when the device is initiated.

To inform the system that the teller has access to a passbook device, the user has to enter the device name in the TELLER.ID record. The device name is used to form the key to the PRINTER.ATTRIBUTES application, which is made up from PASSBOOK.DEVICE and the attributes, defined in the Attribute field on the TELLER.PASSBOOK record. In this example, the key to the PRINTER.ATTRIBUTES file is therefore HP8000L.INIT.

> **⚠️ Note:** There is an option to set the language used if the Prt Lang field is used. This ensures the language descriptions from any records are consistent and not affected by the language on the teller’s USER record.


#### 🔧 Working With

The following section describes different options available in passbook printing.


##### Updating Passbooks (Processing)

Once the teller transaction is committed, the user can launch the TT.PASSBOOK.PRINT application .

The ID of the record is the account number that needs to be printed for. This application displays the page and line of the passbook and the outstanding entries to print. The above screen shows there are two entries to print as there is one outstanding entry to print from before this teller transaction.

The user can modify the page and line number and instruct that a new passbook be printed by using the fields on this application.

If the teller does not wish to print the passbook at this time, then set the Print Passbook field to NO and commit. Print logic is not invoked this time.

Once the teller agrees with the Page No , Line No and New Passbook fields, the record can be committed.

Also, note if deal slip printing is configured, then this can also be launched in a separate window:

Once this is committed,

- A new window containing the Passbook Print data appears.
- The TT.PASSBOOK.PRINT application displays a confirmation message.

To print this, right click this window and select print, then the passbook printer has to be selected.

The system requests confirmation if the passbook is printed correctly. The user has to choose one of the following options.

- NO- The initial TT.PASSBOOK.PRINT screen appears.
- YES- The print confirmation screen appears.

If there are no entries to print for an account or passbook, the system displays the following message.

Account does not have outstanding entries to print.

The TELLER.PASSBOOK.REPRINT application is used to request a reprint.

- Input by specifying the required date range and commit the record.

- Go back into the TELLER.PASSBOOK.REPRINT record for the account and verify the record. The TT.PASSBOOK.PRINT application is launched.

- This now shows all entries between dates previously specified on TELLER.PASSBOOK.REPRINT . this can be checked by viewing the Start Date and End Date no-input fields.
- This application also shows the total number of pages to print and it is possible to identify what page is going to be printed by looking at the Process Page no-input field.

- The teller can update the Line, Page No and New Passbook fields, and commit the record. The 1st page of entries appears: Since this is a multi-page print job, TT.PASSBOOK.PRINT displays confirmation for the 2nd page: The entries to print has decreased accordingly and the page is now 2 of 2.
- Commit the record. Page 2 of Passbook Entries appears. TT.PASSBOOK.PRINT shows the confirmation stage. The user cannot modify Page, Line and New Passbook as these fields are now no-input.

The warnings section has two options:

Select NO and commit the record. The initial screen appears.

Select YES. The transaction has finished.

If the print job spans across passbooks during a multi-page transaction, that is, the 1st passbook is full and a new passbook must be inserted, then TT.PASSBOOK.PRINT appears:

The user has to insert new passbook A/C XXXXXX.


##### Different Pass Book Layout

For general accounts, the passbook layout is System by default. However it is possible to define and attach a different passbook layout using the Passbook ID field in the ACCOUNT.STATEMENT application.

> **⚠️ Note:** Unless this field is input for an account, which has the value Yes in the Passbook field, the default passbook layout is system.


##### TELLER.PASSBOOK.REPRINT

The TELLER.PASSBOOK.REPRINT application can be used to print entries at any time for an account. Besides the account number, the user should specify the period for which the passbook to be printed in the Start Date and End Date fields as shown below.


#### 📋 Tasks

Related topics:

- Update Passbook
- Update Passbook

Passbooks can be issued to savings accounts. When an entry is passed across a passbook account from any application, the details are recorded and the TELLER system updates the passbook when it is presented.


##### Workflow

This section allows the user to perform the below activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Authorised . |
| Find Account Arrangements | Enter an account arrangement ID in the Arrangement field and then click the FIND button. Click the Overview icon corresponding to a record. |
| Arrangement Overview (Account) | Click the New Activity icon. |
| New Activity | Click the Do Activity Today icon corresponding to Update Account Details activity. |
| Arrangement Activity | Enter a value in the GB Narrative field. Click the Validate icon. Select the Mortgage Insurance option and then click the Default Values(Calculation) icon. Enter values in the following fields: Type Currency Fixed Amount Select the Account option and then click the Static icon. Enter the value as 'Yes' in the Passbook field. Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

There are no Outputs available for Passbook Printing feature.

---


### 1.10  Preferential Pricing for FCY transactions


> **📇 Quick Reference Card**
> 
> **Purpose:** *In the FUNDS.TRANSFER application, FT.GROUP.CONDITION takes care of providing preferential treatment to a group of customers based on certain criteria like category and sector. A similar feature is provided in TELLER by way of TT.GROUP.CONDITION .*
> 
> **Key Fields:** *Charge Type*, *Chg Percent*, *Contract Group*, *Customer.2*, *Decis*, *Rate Spread*, *Sector*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

In the FUNDS.TRANSFER application, FT.GROUP.CONDITION takes care of providing preferential treatment to a group of customers based on certain criteria like category and sector. A similar feature is provided in TELLER by way of TT.GROUP.CONDITION .


#### ⚙️ Configuration

The following section describes the configuration settings for Preferential Pricing for FCY transactions.


##### TT.GROUP.CONDITION

The group of customers who need preferential treatment for Charges, Commission and Exchange rate spread should be classified under a particular contract group for identification. The procedure for defining a contract group for teller related preferential treatment is as given below:

- In APPL.GEN.CONDITION , create a record with TELLER as ID.
- The Contract Group field of APPL.GEN.CONDITION can be used to create groups like staff and so on (this is a multi-value field that enables creation of many number of groups based on different decisions).
- The Decis field is used to link any field of any application like Sector of CUSTOMER to one of the fields in TELLER , so that any transaction made for this contract group refers to the related TT.GROUP.CONDITION and applies the preferential rates. The linking is done through J descriptors. For example in the Standard Selection record of TELLER , the Customer.2 field can be linked through J descriptor to the Sector field in CUSTOMER . This has to be done under a unique field name. Afterwards in APPL.GEN.CONDITION , under the Contract Group (say Staff), set the Decis Field to the unique field name and equate it to a sector number relevant for staff (say 9900)
- The contract groups created through the APPL.GEN.CONDITION are linked to TT.GROUP.CONDITION .
- TT.GROUP.CONDITION enables to define preferential exchange rate spread, commission and charges for a contract group created through APPL.GEN.CONDITION . The data defined here for rates spread, charges and commission overrides the default conditions otherwise used by the TELLER application.

The ID of TT.GROUP.CONDITION is the same as the contract group defined under APPL.GEN.CONDITION (for example, Staff).

The following fields of TT.GROUP.CONDITION define the settings relating to the preferential treatment for a contract group:

- Rate Spread defines the preferential rate that can be applied on the exchange spread (CUST.MED.SPREAD, CUST.SMALL.SPRD of the corresponding CURRENCY record based on the transaction value)
- Chg Percent defines the concession percentage of charge or commission for the charge or commission type specified.

Instead of a concession percentage of charge or commission, a fixed amount also can be defined according to the currency.

It is also possible to define the attributes for a particular customer alone by giving the ID as C-Customer number (example: C-100001) in TT.GROUP.CONDITION .


#### 🔧 Working With

Whenever a teller transaction is made for a customer, the contract group is identified from APPL.GEN.CONDITION and the preferential percentage of rates, commission and charges pertaining to this group are applied based on the data specified in the TT.GROUP.CONDITION of that group. A no-input field called Contract Group in TELLER stores and displays the name of the contract group to which the customer belongs to for future reference.

Below are the examples for preferential pricing using FCY transactions.

Consider if the bank wants to pass on a concession of 30% on the exchange rate spread to its staff and wants to charge only 70% of the spread. The following steps are followed:

1. Create a record for TELLER in APPL.GEN.CONDITION .
2. Under Contract Group define STAFF.
3. Link the decision field to Sector of customer record, as STAFF as described above using j descriptor.
4. In TT.GROUP.CONDITION , give the @ID as STAFF.
5. In Rate Spread of TT.GROUP.CONDITION , enter 70

After these settings are over, whenever a teller transaction involving foreign exchange happens for Staff, then the system finds out the customer spread from the CURRENCY, based on the transaction amount, for example 0.05 and calculate 70% of it, which works out to 0.035. This spread of 0.035 is added to the rate for Staff, whereas for others the normal spread of 0.05 is added.

Similar to Concession on rate for staff, the Contract Group also has to be set for STAFF.

Consider the charges for Draft as defined in FT.CHARGE.TYPE , is USD30. In TT.GROUP.CONDITION of STAFF; 60 is defined under the Charge Percent field. Then in all the teller transactions of the customers who are identified as STAFF (Contract Group), if the Charge Type field is Draft, instead of charging USD30, only USD18 is going to be charged.


#### 📋 Tasks

There are no Tasks available for Preferential Pricing for FCY transactions feature.


#### 📊 Outputs

There are no Outputs available for Preferential Pricing for FCY transactions feature.

---


### 1.11  Stock Control


> **📇 Quick Reference Card**
> 
> **Purpose:** *In Temenos Transact , it is possible in to keep a track of the currency notes, bills and/or travelers’ cheques by currency and denominations. In the case of currency, it is useful or sometimes a mandatory banking requirement to track the amount of currency held by denomination.*
> 
> **Key Fields:** *Auto Denominate*, *Check Stock Amt*, *Cr Denom Type*, *Credit Account*, *Credit Currency/Amt*, *Credit Stock*, *Debit Stock*, *Denom Filter* ... +16 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

In Temenos Transact , it is possible in to keep a track of the currency notes, bills and/or travelers’ cheques by currency and denominations. In the case of currency, it is useful or sometimes a mandatory banking requirement to track the amount of currency held by denomination.


##### Teller Denominations

TELLER.DENOMINATION records identify the units, coins and notes that are available. When a transaction requiring the use of denomination is entered these can be used to identify the stock levels of each currency at note or coin level.

| Column 1 | Column 2 | Column 3 |
|---|---|---|
| USD1000 | One thousand US Dollar Bill/TC | 1000.000 |
| USD500 | Five Hundred US Dollar Bill/TC | 500.000 |
| USD5CENT | Five Cent Coin | 0.050 |


#### ⚙️ Configuration

The following section deals with the related attributes


##### Stock Control

Stock Upd field is introduced in TELLER.PARAMETER and TELLER.ID . If this field is set to Yes, the denomination units input in TELLER.ID during till closure is treated as the final stock with the teller. Also this overwrites the TT.STOCK.CONTROL with the denomination units entered in TELLER.ID , for each currency denomination( except travelers’ cheques denominations)

This functionality is catered only for cash transactions.

Travelers’ Cheques are more closely controlled by serial number as well as the denominations held.


##### Denomination Control

The denomination control for Side-1 of the teller transaction can be changed by the use of Check Stock Amt field. If this is set to Yes and more than one internal account is used on Side-1, then only the accounts with stock control set to DENOM can be used to check for denominations to the deal amount. If set to No, then all the accounts are used in the denomination control totals.


##### Denomination filtering

The DENOM.TYPES file is used to define various denomination types such as Cash, Gift Cheque, Traveller’s Cheques and so on.


#### 🔧 Working With

The TC.STOCK.IN.BANK enquiry shows the stock held by currency, denomination and serial number ranges.

The other three enquiries are:

- TC.STOCK.IN.TRUST - shows the stock allocated to trusted clients
- TC.RETAILER.STOCK - shows the stock held at a specific site
- TC.STOCK - displays the stock by Category, Currency and/or TELLER.ID , which can be used to verify the sales made that day.


##### Denomination filtering

This Denom Type is attached to TELLER.DENOMINATION.

TELLER DENOMINATIONS list with Denom Type as CASH is shown below.

Based on the Denom Filter (Yes), Cr Denom Type and Dr Denom Type set at the TELLER.TRANSACTION level, the filtering functionality is enabled, else the default functionality is available.

TELLER record being input with a Transaction Code as 10 is shown below.

As only Cr Denom Type is set in this particular TELLER.TRANSACTION , TELLER.DENOMINATION having CASH Denom Type are available in the UNIT side of the TELLER transaction. The DR.UNIT side has all the available denominations since Dr Denom Type is NULL. It is also possible to have filtering enabled in both sides of the TELLER.TRANSACTION .


##### Auto Denomination

The Auto Denominate field in TELLER.TRANSACTION offers the user an option to determin whether the denominations should be user-defined for each teller transaction or automatically pre-filled. Allowable values are YES or NO. When this field is set to YES, then the system supports the default pre-filling of the denominations, when this field is set to NO, the system does not default any denominations. The user can input the denomination.

If Auto Denominate is set to NO and the user does not input the correct denomination which equals the transaction amount, the system throws an appropriate error message and does not pre-fill or default the denomination and hence the transaction cannot be committed.

In other words, if the user is not inputting the correct denomination, then the system does not commit the transaction by pre-filling a denomination.


##### Serial Numbers

It is recommended to create TELLER.TRANSACTION records and customised version, for the receipt or sale of travelers’ checks, for dealing with clients to whom you provide travelers’ checks on a trust basis.


##### Teller – Enquiries

The Teller enquiry records provided with the system allows the teller to view the following

- Teller’s current cash position by till, currency and denomination ( TELLER.POSITION )
- The cash held by all other tellers and the vault ( TELLER.OVERALL )
- The entries, in chronological order, passed across the teller cash account(s) ( STMT.ENT.TODAY ) and reversed teller transactions.

There are other enquiries associated with travelers’ checks, detailed previously in this chapter.

This is in addition to the standard List option, that enables the user to list all teller transactions based on any selection criteria and any sort order.

For the STMT.ENT.TODAY enquiry, the account to be entered for the selection criteria should be the teller's cash account (CURRENCY: CATEGORY CODE: TELLER.ID).

For client account enquiries, STMT.ENT.TODAY gives the current account balance including all entries made on that day. The account balance can also be obtained from the main account record.


#### 📋 Tasks

Related topics:

- Teller Processes

In Temenos Transact , it is possible in to keep a track of the currency notes, bills and/or travellers’ cheques by currency and denominations. In the case of currency, it is useful or sometimes a mandatory banking requirement to track the amount of currency held by denomination.


##### Workflow

Stock Controls related activities are listed below:

Traveller’s cheques are preprinted and fixed amount cheques and issued on payment to buyers either directly by issuing bank or through agents of issuing bank. Teller module handles Travellers Cheque (TC) processing, that is, both issue and purchase. This option is used to record receipt of TC Stock.

To record the receipt of TC Stock activity, follow below steps:

1. Receipt of TC Stock .
2. Select the TC Stock Receipt tab.
3. Enter values for the following fields: TC Currency TC Amount TC Account Narrative TC Contra Account Narrative
4. Click the Validate icon to check for errors, if any.
5. Click the Commit icon.

Draft Management related activities are listed below:

This option allows the user to buy Traveller's Cheques against cash. The exchange rate is auto-populated from the CURRENCY application and can be changed by the user, if required.

To buy a TC against cash, perform the following steps:

1. Buy TC's against cash .
2. In the Buy TCs against Cash screen, enter values in the following fields: TC Currency TC Amount TC Debit Account Narrative

1. Click the Validate icon to check for errors and overrides.
2. Click the Commit icon.

This option allows the user to sell Traveller's Cheques against cash. The exchange rate is auto-populated from the CURRENCY application and can be changed by the user, if required.

To sell a TC against cash, perform the following steps:

1. Sell TC's against cash .
2. In the Sell TCs against Cash screen, enter values in the following fields: TC Currency TC Amount TC Account Narrative Waive Charge

1. In TC Denomination tab, enter values in the required fields.
2. Click the Validate icon to check for errors and overrides.
3. Click the Commit icon.

This option allows the user to buy Traveller's Cheques against account transfer of funds. The exchange rate is auto-populated from the CURRENCY application and can be changed by the user, if required. The charge amount auto-populated in the transaction can be overridden or waived by the user.

To buy a TC against account, perform the following steps:

1. Buy TC's against Account .
2. In the Buy TCs against Account screen, enter values in the following fields: TC Currency TC Amount TC Account Credit Currency/Amt Credit Account Narrative

1. Click the Validate icon to check for errors and overrides.
2. Click the Commit icon.

This option allows user to sell Traveller's Cheque against account transfer of funds. The exchange rate is auto-populated from the CURRENCY application and can be changed by the user, if required. The charge amount auto-populated in the transaction can be overridden or waived by the user.

To a sell TC against account, perform the following steps:

1. Sell TC's against Account .
2. In the Sell TCs against Account screen, enter values in the following fields: TC Currency TC Amount TC Account Narrative Payment Currency Payment Account

1. In the TC Denom tab, enter values in the required fields.
2. Click the Validate icon to check for errors and overrides.
3. Click the Commit icon to submit the record.

Traveller’s Cheques are preprinted cheques with fixed amount and issued on payment to buyers either directly by issuing bank or through agents of issuing bank. Teller module handles Travellers Cheque (TC) processing, that is both issue and purchase. This option is used to record receipt of TC Stock.

To receive the TC stock, perform the following steps:

1. Receipt of TC Stock .
2. Enter values in the following fields: TC Currency TC Amount TC Account Narrative TC Contra Account Narrative.1
3. Click the Validate icon to check for errors, if any.
4. Click the Commit icon.

This option allows the Teller or Head Teller to transfer the TC stock from one branch to another branch. The branch can transfer the Surplus TC stock held with the Branch or on request of other branch, the transfer can be initiated.

To transfer TC stock to other branches, follow the below steps:

1. TC Position .
2. Click the Trans of Stock-Oth Branch icon.
3. Enter values in the following fields: TC Currency TC Amount.1 TC Account.1 Narrative.1 TC Contra Account Narrative.1
4. Click the Validate icon to check for errors, if any.
5. Click the Commit icon.

This option allows the Teller to transfer the Traveller's Cheque stock from Vault to individual Till in the same branch. After the TC stock is updated to the Tills, the Teller can carry out buying and selling of TC stock.

To transfer TC from Vault to individual Till, follow the below steps:

1. TC Position .
2. Click the TC Vault to Till icon.
3. Enter values in the following fields: TC Currency TC Amount.1 Debit Stock Credit Stock
4. Click the Validate icon to check for errors, if any.
5. Click the Commit icon.


#### 📊 Outputs

There are no Outputs available for Stock Control feature.

---


### 1.12  Teller Default


> **📇 Quick Reference Card**
> 
> **Purpose:** *The TELLER system provides an interface to other modules within Temenos Transact through the TELLER.DEFAULT application.*
> 
> **Key Fields:** *Account*, *Amount*, *Amount Deposited*, *Benef Customer*, *Cheque No*, *Consolidate Now*, *Credit Account*, *Credit Currency* ... +13 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The TELLER system provides an interface to other modules within Temenos Transact through the TELLER.DEFAULT application.

It provides another module the ability to create a teller transaction automatically. It contains all necessary information such as accounts, amounts, rates, charges and so on, which can then be accessed by the teller by entering a reference number.

Once the TELLER.DEFAULT record has been processed, it cannot be reprocessed. The layout of TELLER.DEFAULT is exactly the same as TELLER but includes ten additional fields that can include free format data and two fields to record information that the record has been processed, the process date and the transaction reference number.

The link to TELLER.DEFAULT is through the Our Reference field in TELLER . If this is entered prior to any other data, then the associated TELLER.DEFAULT record gets loaded.


#### ⚙️ Configuration

There are no configuration details available for this section.


#### 🔧 Working With

This section includes the following:


##### Account Closure

If a client prefers to close his account, the teller must perform two transactions within Temenos Transact .

1. The account record must be closed. This informs the teller of all outstanding credit or debit interest, charges, tax and so on.
2. The teller must pay the client the amount due. However, in order to perform the latter client has to enter the details from the ACCOUNT.CLOSURE screen into TELLER .

The account closure procedure records the details in TELLER.DEFAULT (ID of account number) and the teller pulls the details automatically into a teller transaction by entering the account number into the Our Reference field.


#### 📋 Tasks

Related topics:

- Perform End of Day Activities - Nostro Funding For Travellers Cheques Issued
- Execute LCY Cash Deposit
- Execute Buy FCY Against LCY Cash
- Teller Processes

The Teller home page has a custom set of menus and enquiries, which are required by a Teller on a day-to-day basis. The Home Page handles different types of teller related transactions and also helps the Teller in viewing the Cash Positions, TC Stock, Unauthorised Transactions, Forward Movements for the Account and the Mandate (signature) of the account.

The Dashboard of the Teller Home Page is designed to view the Appointments and the Future Appointments of the Teller and also the provision of viewing the internal messages sent by different roles in the Branch.


##### Workflow

Teller Default related activities are listed below:

This enquiry is used to fund the Nostro account.

To fund a Nostro account, follow the below steps:

1. Fund Nostro for TC Issuance .
2. Enter values in the following fields: Debit Account Debit Value Date Credit Currency Credit Account Benef Customer MT103 Receiver Bank
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon.

This function allows the user to authorise all the transactions which are in unauthorised status. This enquiry lists all the unauthorised transactions of above nature and by selecting the appropriate drill down, the user can either authorise or delete the record.

The user can also authorise the pending Transactions of Drafts/Transfers, Arrangements Transfers, Cheques, Debit Cards, Currency Exchanges and STO/DD/Sweeps.

To authorise a transaction, follow the below steps:

1. Transactions .
2. In the Unauthorised TFS Transactions screen, click the Authorise icon.
3. In the Transaction section, verify the details and then click the Authorise icon.

This option allows the user to reverse Teller transactions such as, Cash Deposit, Cash Withdrawals and so on, after authorisation of the transactions.

To reverse a Teller transaction, follow the below steps:

1. Reverse Transactions .
2. Click the Reverse icon.
3. Enter values in the following fields: Reverse Consolidate Now
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon to submit the record.

This option allows the Teller to enter local currency cash deposit transaction into a local currency account. A transaction reference number is generated after the transaction is committed. After the transaction is complete, it is available for authorisation by the Head Teller or Supervisor, if the deposited amount exceeds the teller limit.

To deposit the cash in local currency, follow the below steps:

1. Cash deposit Local .
2. Enter values in the following fields: Deposit Amount Credit Account Narrative Denomination
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon to submit the record.

This option allows the user to enter a foreign currency cash deposit into an account which could be in a local currency or foreign currency. In this transaction, the currency in which the deposit is done must be entered. The exchange rate is defaulted from the Currency file and it can be changed by user, if required. A charge can be applied on the transaction by setting it up at the Teller Transaction level. The charge amount defaulted in the transaction can be overridden or waived.

To deposit the cash in foreign currency, follow the below steps:

1. Cash deposit Foreign .
2. Enter values in the following fields: Currency Deposited Amount Deposited Account Narrative Waive Charges Denomination
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon to submit the record.

This option allows the user to withdraw cash in local currency account of the customer.

To withdraw the cash in local currency, follow the below steps:

1. Cash withdrawal Local .
2. Enter values in the following fields: Withdrawal Amount Debit Account Narrative Cheque No Denomination
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon to submit the record.

This option allows the user to withdraw foreign currency from an account. The exchange rate is defaulted from the CURRENCY application and if required it can be changed by user. The charge amount defaulted in the transaction can be overridden or waived by user. An exception will be thrown when the cheque number entered is not attached with the customer account.

To withdraw the cash in foreign currency, follow the below steps:

1. Cash withdrawal Foreign .
2. Enter values in the following fields: Withdrawal Amount Withdrawal Currency Exchange rate Narrative Cheque No
3. In the Cash Denom tab, enter values in the required fields.
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon to submit the record.

This option allows the user to change denominations in the same currency.

To change the denomination, follow the below steps:

1. Change Denomination .
2. Enter values in the following fields: Amount Credit Narrative Denomination
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon to submit the record.

This option can be used to enter a transaction to buy foreign currency against local currency.

To buy the foreign currency, follow the below steps:

1. Buy Foreign Ccy against Local Ccy .
2. Enter values in the below fields: Amount Waive Charges Narrative Denomination
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon to submit the record.

This option is used to enter a transaction to sell foreign currency against local currency.

To sell foreign currency, follow the below steps:

1. Sell Foreign Ccy against Local Ccy .
2. Enter values in the following fields: Amount Waive Charges Narrative Denomination details for Cash Paid and Received
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon to submit the record.


#### 📊 Outputs

The Teller module in Temenos Transact processes a wide variety of retail transactions. Teller is a account based application for moving funds. It incorporates the Cash entries today, cash position by currency, exchange rate and so on.


##### Enquiries and Reports

The user can view the below list of enquiries and reports pertaining to Teller Default in the core banking system.

TC Stock Balances

This enquiry displays the Traveller’s Cheque Stock by Teller or Branch.

Cash Entries Today

This enquiry displays the list of transactions completed by a Teller.

Cash Position - Currency

This enquiry displays the cash position of the Teller by currency.

Cash Position - Denom

This enquiry displays the cash position of the Teller by denomination.

Cash Position - Teller

This enquiry displays the cash position of the Teller by denomination and by currency.

Exchange Rate

This enquiry displays the exchange rate of various currencies.


##### SWIFT Messages

NA


##### Advices

The user can view the below list of advices.

This advice is used to enter a foreign currency cash deposit into a different currency account. In this transaction, the currency in which the deposit is done must be entered.

This advice allows cash deposit in local currency into a foreign currency account.

This advice allows cash deposit transaction in local currency into a local currency account.

This advice allows the user to enter a cash withdrawal in foreign currency from an account held in any currency.

This advice allows cash withdrawal in local currency from a foreign currency account.

This advice allows withdrawal of cash without cheques (using withdrawal slips) in local currency.

This advice allows withdrawal of cash in local currency.


##### Alerts

NA

---


### 1.13  Teller Financial Services


> **📇 Quick Reference Card**
> 
> **Purpose:** *The TELLER.FINANCIAL.SERVICES suite supports:*
> 
> **Key Fields:** *Account*, *Account Cr*, *Account Dr*, *Allow His Reversal*, *Allowed Categ*, *Allowed Categ.1*, *Allowed Categ.2*, *Aml Details* ... +74 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The TELLER.FINANCIAL.SERVICES suite supports:

- A companywide parameter table that allows configuration of how consolidation has to happen, user friendliness, security parameters among others.
- A simple transaction type table that holds the mapping to the underlying Transaction type ( FT.TXN.TYPE.CONDITION or TELLER.TRANSACTION or TRANSACTION ) eliminating redundant configuration for this suite.
- Capture of multiple transactions (any different combination of transactions) on the same screen Even if they belong to different accounts of the customer. Optional primary account to avoid having to re-enter the same account number in each Leg Optional surrogate account to override the default primary account for a specific Leg
- Local and Foreign Currency Transactions It is even possible to capture the information in a 3rd currency for the system to automatically calculate the exchange rates of debit and credit accounts. Example, Transfer USD 100 from my GBP Account into my EUR Account
- Charges for each TFS Leg or a Consolidated Charge
- Consolidated Transaction Advice
- A Consolidated entry on the Customer account per configuration
- Consolidation can happen as either All Debits and Credits Separately or All Debits and Credits together resulting in 2 or 1 entries on the customer account respectively
- All transactions supported by the underlying modules (FT, TT or DC) with the exception of wire transfers through FT
- Example, SWIFT
- Reversal of FT or TT transactions in history by creating offsetting DC Transaction.
- A sub-set of transactions supported by TFS on a single screen are (all of these allow both local & foreign currencies) Cash deposit Cash Withdrawal Cash back Bill Payment Loan Repayment Term deposit partial withdrawal Deposit Pre-closure Multi-Deposit Open Account to Account transfer Cheque Encashment ON-US Cheque Deposit Cheque Deposit for Local Clearing Cheque Deposit for Collection Currency Exchange Units Exchange
- Transactions on Customer, Internal & PL account.
- Easy keyboard navigation thereby improving user efficiency.
- Massive defaulting features facilitating minimal user input
- Easy trace back from Accounting Entry.
- Supports inter-branch transactions and multi-book
- Complete control on the status of the child transactions – supports all Temenos Transact functions. If TFS is in unauthorised status, all its child transactions go to unauthorised status. Authorising TFS automatically authorises the child transactions.
- One click to reverse or delete unauthorised legs.
- Capture of AML information and basic validation on the validity of the Transaction Limits legal identification document


#### ⚙️ Configuration

The setup for TELLER and FUNDS.TRANSFER must be complete before setting up TFS. Refer to the respective user guides on how to set them up.

Similar to Funds Transfer( FT )or Teller Transaction (TT) modules, TFS suite consists of TFS.PARAMETER , a Temenos Transact company-wide parameter table and TFS.TRANSACTION , a Transaction type definition table.

Some of the settings of TFS.PARAMETER (such as Currency conversion, OFS Version for the child transaction, Transaction Limit specifications) are also repeated at TFS.TRANSACTION level, giving the flexibility to override the Temenos Transact company-wide settings for a given transaction type.

There are yet other settings of TFS.PARAMETER (such as Consolidation Method, Add-on Factors for Consolidation Level) that are repeated at TELLER.FINANCIAL.SERVICES level, giving the user a choice in how they want the entries to be generated in a given TFS Transaction.


##### Pre-requisites before Setting UpTFS.PARAMETER

This is the parameter table for TELLER.FINANCIAL.SERVICES . This is an INT type file and can be maintained for each company in Temenos Transact . If a record does not exist for the current company, then the system tries to apply the parameterisation of the master company.

TFS allows consolidation of two or more user input transactions and gives a single credit or debit to the customer’s account.

If this consolidation feature needs to be enabled, then an exclusive category needs to be identified as the Consolidation Washthru Category. The range of this category has to be in the ,Internal Account range 10000 to 19999 (this category is specified in TFS.PARAMETER ).

Accounts in this category are used by TFS to temporarily place the amounts of the user input legs so that it can consolidate them and give a single credit or debit per TFS Transaction, to the customer’s primary account.

At the end of a given TFS Transaction, the sum of all entries to the Washthru account is zero.

The user can create a default account for the Consolidation Washthru Category in local currency. Once this default account is created, during transaction processing, the washthru accounts for the respective currencies and teller IDs are automatically created by the system (Teller). The washthru accounts are created by Temenos Transact TELLER module in a manner similar to how the till accounts are created.

That is, CCY : Category : Teller ID.

TFS uses BC.SORT.CODE to arrive at the exposure date for cheques being deposited for local clearing or collection.

When consolidating a cheque deposit and cash (or any other credit that requires same day availability) deposit, it needs to apply a default, same day availability for that portion of the consolidated amount. For this purpose a default record in BC.SORT.CODE needs to be created with the Value Date Prd and Exp Date Prd fields left blank.

This value is specified in the Consol Sort Code field in TFS.PARAMETER

Temenos Transact TELLER, FT and data capture (DC) modules currently support application of forward exposures by way of Exposure Date (single availability date for the funds deposited). In addition to this, Teller also supports Exposure Split Dates (multiple availability dates for the funds deposited).

- The online cleared and working balances on the account can be updated only in the Start of Day of the Exposure date.

However, none of these transactions can be reversed once they are moved into history at Close of Business. So, revising a float input on a day in the past is not possible.

An alternative method to hold the funds till the cheque is cleared is using the AC LOCKED EVENTS feature which allows to lock the funds deposited.

- The online cleared and working balances on the account can be updated immediately but the amount is really Locked(Locked Amount field in ACCOUNT updated from AC.LOCKED.EVENTS ).

The advantage of using the lock approach is that the hold can be revised at any time by simply reversing the AC LOCKED EVENTS record.

The net result of both approaches is the same as far as the customer is concerned – The amount available for withdrawal is the same.

The only difference lies in any internal reports run based on the cleared balance of all accounts because when the lock approach is taken, the report might also show cheque deposits which have updated the cleared balance although they really haven’t been cleared.

When multiple financial operations are done in one transaction, it is not uncommon for a financial institution to want to apply one charge to the customer – one charge for the whole consolidated transaction instead of applying one for each of the activities. For example, if a customer made cash deposit and a cheque deposit, each of which could otherwise carry a charge, it might be more sensible to apply one charge based on the consolidated amount.

A decision needs to be taken by the financial institution on whether it really wants to apply a consolidated charge or charge for each of the TFS Legs as if they were done independent of each other.

It is important to note that TFS does not calculate consolidated charge by itself. It only facilitates application of a consolidated charge through custom developed API. Refer to description of the Consol Chg Api field later in this document for more details.

All the parameters that have a combo-box in this application can be left blank in case the user is not sure of the value to input. The system automatically defaults these values.

- When set to Float, TFS uses the TELLER or FT or DC’s Exposure Date or Exp Split Dat feature to apply a float on the funds deposited.
- When set to Lock, TFS creates AC.LOCKED.EVENTS for each of the split exposures.

TFS facilitates capture of customer information (especially in the case of walk-in customers who do not have an account in Temenos Transact ). Such information can be used in any local extraction process to pass on to an AML solution for further analysis at the close of business.

As a minimum, it is possible to validate if legal ID information has been input on the transaction screen and if yes, if it is is still valid. This validation also applies for a customer who has an account in Temenos Transact . TFS automatically checks the Temenos Transact CIF (Customer Information File) and applies the validations mentioned above.

This Aml Details field is to indicate if TFS has to do this minimum validation at all or just treat whatever is captured on the screen as just information. If this field is set to Information, then validation does not happen on the AML or KYC data.

TFS uses the same set of fields in CUSTOMER that is currently used to capture KYC information when creating a new customer. Some of those fields use virtual lookup tables ( EB.LOOKUP ). This Aml Lookup field indicates whether TFS has to use the same virtual tables or if the financial institution wishes to create exclusive lookup tables to be used by TFS.

- If this field is set to Customer, then TFS expects the following look up tables CUS.LEGAL.DOC.NAME for Legal Doc Name field CUS.COMM.TYPE for Comm Type field CUS.LEGAL.ISS.AUTH for Legal Iss Auth field
- If this field is set to Native, then TFS expects the following look up tables TFS.LEGAL.DOC.NAME for Legal Doc Name field TFS.COMM.TYPE for Comm Type field TFS.LEGAL.ISS.AUTH for Legal Iss Auth field

This field indicates if consolidation is enabled for this Temenos Transact company of this implementation.

When consolidation is enabled, it is possible to consolidate the user input legs as

- Gross – All Debits together and All Credits together resulting in two entries on the customer account
- Net – All Debits and Credits together resulting in one entry on the customer account.

When the user input legs are consolidated, the default consolidation level is by value date of the leg. Also, it is possible for a financial institution to specify additional filters by which consolidation has to happen.

The additional levels are

- By Currency
- By TFS Transaction Type
- By Currency & TFS Transaction Type

It is important to note that these levels are only on top of the consolidation by value date. In other words, two user input legs on a single TFS Transaction cannot be consolidated if they don’t have the same value date.

This is the category of the washthru account to be used by TFS when consolidation is enabled.

This is the key to BC.SORT.CODE that contains the default Same Day Availability definition.

When the user input legs are consolidated, the resultant transaction is defaulted as another TFS leg automatically. There is a corresponding child transaction (in TELLER ) created for this leg.

This Consol Tfs Txn field is used to define the TFS.TRANSACTION ID that should be used in the consolidated TFS leg.

If the Consolidation Method is set to be NET, TFS consolidates all debits and credits to the customer’s account (held in the Primary Account field in TELLER.FINANCIAL.SERVICES ). If the resultant amount is zero, then there are a few alternatives that can be automatically applied.

This Consol Amt Zero field helps a financial institution specify their preference in such a situation. It accepts one of the following three values:

- Force.Gross: The system forces the consolidation to be done as Gross. All debits are consolidated as one entry and all credits consolidated as one entry
- Ignore.Consol.Leg: The system does not generates any consolidated leg , in other words, no entry exists on the customer’s account at all.
- Undo.Consolidation: The system does the undo consolidation , this results in each of the user input legs directly hitting the customer’s account.

If a consolidated charge needs to be applied, then that charge is defaulted as another TFS leg automatically. There is a corresponding child transaction created for this leg.

This Consol Chg Tfs Txn field is used to define the TFS.TRANSACTION ID that should be used in the consolidated charge TFS leg.

TFS does not calculate a consolidated charge by itself. It only facilitates application of a consolidated charge by way of allowing a local API to be attached here.

During consolidation, TFS invokes this API and expects this API to return the Charge Code, Charge PL and the Charge Amount among others.

The syntax for this API is:

1. PL Category (Optional if charge code is returned)
2. Charge Code (Key to FT.CHARGE.TYPE ; Optional if PL category is returned)
3. Charge Account (Account to be charged)
4. Charge Currency (Currency of the charge amount. Could be different from the Currency of the charge account. Optional. If not provided, then it can be assumed to be the same as that of the charge account)
5. Charge Amount

This information is then used to build a separate TFS Transaction leg.

TFS builds up a statement narrative for the consolidated leg, based on a native logic.

If a financial institution wants to customise this narrative, then it can be accomplished by developing a custom API and attached in this field.

During consolidation, TFS invokes this API and expects this API to return the text that should be populated on the narrative field for the consolidated Leg.


##### Usability Parameters

Hot Field is a concept in Temenos Transact browser, which allows the user to define a field as Hot, that is, validate the field immediately upon input.

A number of fields on TFS can be made as hot fields, depending on the work-flow, user preferences in the implementation.

It is recommended to make the Beneficiary ID field as Hot Field always. And making the Consolidate Now field as Hot Field helps to reduce number of mouse clicks at the end of user input legs.

In Temenos Transact, it is possible to provide lists of values in two ways either as a combo-box or as a drop down. Read Usability section for more information on the advantages of combo-box. TFS allows either way of listing the values for the Transaction field.

When opening a new deal in TFS, it is normally required for the user to expand the multi-value set to input multiple legs (or transactions).

By setting this field to a desired number, when opening a new deal, TFS has automatically expanded the TFS Legs multi-value set to the number specified here facilitating faster input of transactions.

While atleast one TFS Leg needs to be supplied for transaction information in order to successfully commit a TFS Transaction, any other legs that are left blank are deleted by TFS.

Using either AUTO.NEW.CONTENT version functionality or using the AUTO.EXPAND feature in TFS.PARAMETER , it is possible to launch a new deal in TFS with multiple blank TFS Legs so the user doesn’t have to manually insert new legs (by expanding the multi-value set). At the end of capturing the information, only valid TFS legs are validated and processed. The rest are cleaned up (deleted) by TFS during validation stage.

A valid TFS leg by definition is one that is supplied with value(s) in one of these fields:

- Account Dr
- Account Cr
- Amount
- Beneficiary ID

When using the Transaction field as a combo-box, it normally displays all the transaction types as specified in TFS.TRANSACTION .

This Version field and the associated Include Txn allow us to filter the transaction types to be displayed on the screen, based on the version of TFS being used.

If no value is specified in these fields and if Txn Lookup field is set to combo-box, then TFS.PARAMETER raises an override to that effect stating that transaction filtering is not setup for combo-box.


##### Currency Conversion Parameters

In TFS, it is even possible to do a transaction in a 3rd currency . For example, transfer USD 100 from my GBP account to my EUR account where USD is neither the debit currency nor the credit currency. TFS automatically calculates the debit and credit currency equivalents from the transaction currency (which is USD in this case).

In such situation, using the Txn Ccy To Dr Ccy field, the rate preferences can be set that can be applied when calculating the debit currency equivalent (GBP in this example).

Preference set in Txn Ccy To Cr Ccy is used when calculating the credit currency equivalent (EUR in this example).

In any transaction, from the financial institution’s perspective, the debit side can be treated as the Buy side and the credit side can be treated as the Sell side.

These set of fields can be used to specify the financial institution’s rate preferences for each of the possible scenarios

- Buy Fcy Sell Lcy – when the debit side is foreign currency and credit side is local currency
- Buy Lcy Sell Fcy – when the debit side is local currency and credit side is foreign currency
- Buy Fcy Sell Fcy – when the debit and credit sides are both foreign currency

When foreign currency is involved in a transaction, the TELLER module normally calculates market exchange profit (if Mkt Exch Method in TELLER.PARAMETER is set to Middle). It calculates the difference between local currency equivalent arrived at using mid-reval rate and local currency equivalent arrived at using buy-sell rate and booking this difference as profit.

This Mkt Exch Profit field in TFS.PARAMETER is to indicate if TFS should allow TELLER to calculate market exchange profit or not.

It may not be common to apply market exchange profit for an account to account transfer or cash deposit or cash withdrawal (even if foreign currency is involved) but simply apply a charge for it.

A real forex transaction where the customer wants to buy a foreign or local currency against local or foreign currency is something where a market exchange profit can be applied.

It is advisable to set this field as NO in TFS.PARAMETER and enable it in the corresponding field in TFS.TRANSACTION level only for those transaction types for which market exchange profit is to be calculated.


##### Interface Parameters

TFS uses Temenos Transact Open Financial Services to create transactions for each TFS leg, in FT or TT or DC module.

This is the key to OFS.SOURCE table. This is common for all modules and is used by TFS when creating the child transactions.

Starting from this field to OFS Version is an associated multi-value set to give child module specific definitions.

This field specifies the child transaction’s module.

In an implementation, if there are any local reference fields captured in TFS that need to be passed along to the child transaction, then a routine can be developed and attached here for the respective module. TFS invokes this API before creating the child transaction and expects this API to return any field name and values it needs to be passed along, in a standard OFS format (Vanilla OFS).

When creating child transactions via TFS, it is possible to apply custom validations on the child transactions via versions. This OFS Version holds the default version for the associated child transaction module that TFS uses when creating the child transaction (this is done for each leg at a time). The same field is also available at TFS.TRANSACTION level which when specified takes precedence.


##### DC Related Parameters

When a TELLER or FT child transaction created by TFS needs to be reversed, as long as it is in live, TFS simply reverses them.

However, if it is in history, then TFS tries to create offsetting DC legs for each of the accounting and PL entries raised by the child transaction (This does not include the position accounting entries). In such situations, it uses the details (like transaction code, amount, currency and so on) as available in the accounting entry. But if the transaction code used by the child transaction is not enabled for use in DC (the Data Capture field not set to Y in TRANSACTION table), then TFS uses the default transaction code specified in these two fields.

Note that if history reversal is enabled in FT.TXN.TYPE.CONDITION for an FT child transaction, TFS simply reverses the FT from history.

In cases where DC is used to reverse or create offsetting entries to undo another child transaction (either by user input DC TFS Leg or by trying to reverse a child TELLER or FT transaction in history), the DC legs are created with reversal marker which gets passed onto accounting entry (stmt entry).

Now if this reversal DC needs to be undone, it can be done in one of two ways. Retain the reversal marker but apply the appropriate credit or debit sign, and credit or debit transaction codes or take out the reversal marker and simply swap the transaction codes.

These scenarios are typically a result of user error. The decision is simply based on how the financial institution wants the entries to be reflected on the customer’s account statement. Left blank, it defaults to Retain Marker.


##### Transaction Limit Parameters

It is not uncommon for financial institutions to apply a control on the transactions done by end users. One such control is on the transaction amount itself. TFS supports validation of transaction amounts and to raise an alert (Override) to the user if a particular transaction breaches the limit specified.

The limits can be set for each currency as applicable and also a global limit definition in LCY equivalent. During transaction processing, if TFS cannot find the transaction currency in the Limit definition, then it calculates the LCY equivalent of the transaction amount and validate against the LCY Limit.

These same fields are available at TFS.TRANSACTION level, which take precedence over these settings, when that transaction type is used on a TFS Leg.

This field allows the user to enable or disable transaction limit validations. By setting it No, this feature can be disabled altogether.

Enabling it can be done in one of two ways.

- Consolidated Legs – the amount of the TFS legs which were a result of consolidation are validated against the limit.
- User Input Legs – the amount of the TFS legs that were input by the user is validated against the limit.

When set to No, the system treats it as being disabled and no validation takes place.

From a business perspective, this can be looked upon as validating either the individual transactions (user input leg) or the total transaction amount (consolidated leg) , for example, a customer can come in with GBP 10,000.00 cash, EUR 5,000.00 cash, a couple of cheques worth USD 20,000. If the Limit for GBP, EUR and USD are 15,000.00, 10,000 and 25,000 respectively, then validating against individual user input legs does not violate or breach the limit. However validating against the consolidated leg obviously breaches the limit.

Depending on the purpose of applying this Transaction Limit control, the financial institution can decide which type of validation needs to be done.

This is the global LCY limit that can be applied when no limit is specified for the transaction currency. In such cases, TFS calculates the local currency equivalent (using mid-reval rate) of the transaction amount and validate against the limit specified in this field.

When LCY equivalent is used, it raises an override to the effect that Transaction Limit not defined for the Currency XXX

Besides, if the transaction amount breaches the limit, then it raises an override to that effect.

For normal local currency transactions, this field is taken as the Local Currency transaction limit.

This is the same as in TFS.PARAMETER . If this field is set at the TFS.TRANSACTION level, then it takes precedence over the setup in TFS.PARAMETER , but only when this TFS Transaction type is used.


##### Miscellaneous Parameters

In TFS all transactions are entered on the same screen using a set of associated multi-value fields. Especially when the transaction field is displayed as a combo-box, it is quite possible for the user to have chosen the wrong transaction type (because more than one transaction types might start with the same letter – say, CASHDEP and CASH.BACK both start with C). When the user realises the mistake, and changes the transaction type to be the correct one, a number of re-calculations need to be done including the appropriate account defaulting. However, the currency and amount might still need to be retained.

This Reset Fields field allows us to define which of the fields in a TFS leg need to be changed or reset for re-calculation when the user changes the transaction type.


##### Setting upTFS.TRANSACTION

TFS.TRANSACTION is the transaction type definition table for the TFS Suite. This is a FIN type table and needs to be maintained for each Temenos Transact Lead Company.

It allows definition of mapping to the underlying Temenos Transact Module and its respective Transaction type ( FT.TXN.TYPE.CONDITION or TELLER.TRANSACTION or TRANSACTION as appropriate)

While the Description field is used for enrichment purposes and general description of this transaction type, the value in the Consol Narr field is used when TFS builds the statement narrative for the consolidated transaction. On the customer’s account statement, the narrative appears as below.

(The rest of the information in the narrative is dynamically built by TFS)

Even if consolidation is enabled, it is possible to exclude a specific transaction type from consolidation. If this field is set to Yes, then any user input legs using this transaction type cannot be included in consolidation.

It is important to note that if an implementation uses Temenos Transact cheque collection process to manage the life of the cheque (configured via CQ.PARAMETER ), then this field needs to be set to Yes for those TFS Transaction types used for recording collection or clearing cheques. This is because the CHEQUE.COLLECTION record is needed to have the primary account and not the washthru account.

These two fields hold the mapping to the underlying child transaction module and its respective transaction type tables.

- If Interface To is set to TT, then Interface As must hold a valid record in TELLER.TRANSACTION .
- If Interface To is set to FT, then Interface As must hold a valid record in FT.TXN.TYPE.CONDITION .
- If Interface To is set to DC, then Interface As must be left blank and the appropriate TRANSACTION codes must be specified in Dr Txn Code and Cr Txn Code fields.

This field holds the version to be used to create the child transaction when this particular TFS Transaction type is used.

If this field is set, then it takes precedence over the default version specified in TFS.PARAMETER

TELLER.FINANCIAL.SERVICES has a field called Surrogate Ac which can be used as a surrogate to the debit or credit accounts on each leg. This is primarily to avoid displaying both Dr and Cr accounts on the screen so as to make the screen user friendly.

- If this field in TFS.TRANSACTION is set to ACCOUNT.DR then, any account keyed in Surrogate Ac in TELLER.FINANCIAL.SERVICES is set as default debit account of the associated TFS Leg.
- If this field in TFS.TRANSACTION is set to ACCOUNT.CR the, any account keyed in Surrogate Ac in TELLER.FINANCIAL.SERVICES is set as default credit account of the associated TFS Leg.

For more information, read section on Account Defaulting .

In cases where the transaction type points to TELLER or FT, it is possible to use TFS to reverse that transaction even if it has been moved to history. TFS accomplishes this by creating offsetting DC legs for the accounting entries raised by the original child transaction.

When doing so, TFS uses the transaction codes as they are in the Stmt Entry or Categ Entry. However if those transaction codes are not enabled for use in DC then values specified in these two fields can be used for creating the DC legs.

This is the same as in TFS.PARAMETER . If this field is set at the TFS.TRANSACTION level, then it takes precedence over the setup in TFS.PARAMETER , but only when this TFS Transaction type is used.

This is the same as in TFS.PARAMETER . If this field is set at the TFS.TRANSACTION level, then it takes precedence over the setup in TFS.PARAMETER , but only when this TFS Transaction type is used.

This is the same as in TFS.PARAMETER . If this field is set at the TFS.TRANSACTION level, then it takes precedence over the setup in TFS.PARAMETER , but only when this TFS Transaction type is used.

This is the same as in TFS.PARAMETER . If this field is set at the TFS.TRANSACTION level, then it takes precedence over the setup in TFS.PARAMETER , but only when this TFS Transaction type is used.

This is the same as in TFS.PARAMETER . If this field is set at the TFS.TRANSACTION level, then it takes precedence over the setup in TFS.PARAMETER , but only when this TFS Transaction type is used.

This is the same as in TFS.PARAMETER . If this field is set at the TFS.TRANSACTION level, then it takes precedence over the setup in TFS.PARAMETER , but only when this TFS Transaction type is used.

It is recommended that this field is set to No in TFS.PARAMETER and set to Yes at TFS.TRANSACTION level only for those transaction types for which the financial institution really wants to book market exchange profit (For example, Currency Exchange transaction).

Transaction limits can be set at TFS.TRANSACTION level to override the Temenos Transact Company-wide settings in TFS.PARAMETER .

Shown below are three examples with three different variations on these definitions.

- Clearing and Collection Transactions are being exempt from Transaction limit validation
- For Local Currency Cash Deposits, the limit is specified in LCY
- For Foreign Currency Cash Deposits, the limit is specified for each currency

At TFS.PARAMETER level, it is possible to enable transaction limit validations (where the system validates the transaction amount against a pre-set limit and raise an override if the transaction breaches the limit). If there is such a situation that a particular transaction type needs to be excluded from such validation, this field can be set to YES.

This is the same as in TFS.PARAMETER . If this field is set at the TFS.TRANSACTION level, then it takes precedence over the setup in TFS.PARAMETER , but only when this TFS Transaction type is used.

This is the same as in TFS.PARAMETER . If this field is set at the TFS.TRANSACTION level, then it takes precedence over the setup in TFS.PARAMETER , but only when this TFS Transaction type is used.

This is the same as in TFS.PARAMETER . If this field is set at the TFS.TRANSACTION level, then it takes precedence over the setup in TFS.PARAMETER , but only when this TFS Transaction type is used.


#### 🔧 Working With

Below is an overview on usability and workflow aspects of TFS. It is an illustration of an initial input screen of TFS. Each row is referred to as a TFS Leg.


##### Illustration

| Callout Numbers | Description |
|---|---|
|  | Transaction Reference |
|  | Field to indicate at TFS level if consolidation has to be enabled for this TFS transaction or not. Defaulted to the setting in TFS.PARAMETER but can be changed by user. The same applies to Consol Method and C onsol Level Addon fields. |
|  | Primary account to be used in this TFS Transaction –this is the transaction account of the Customer – Current Account or Checking Account and so on. But it could be any type of account , it even accepts internal accounts. |
|  | Customer number of the primary account holder (Populated when launching the deal from an enquiry drill down or when Consolidate Now is set to Yes. |
|  | TFS Transaction type displayed as a combo-box. |
|  | Surrogate Account – no input required in this field except for account-account transfer type of transactions (including Bill payments).When input, this is used as one side of that TFS leg, with the primary account being on the other side. |
|  | Currency of the Transaction (need not be either the debit currency or the credit currency). If left blank, it is assumed to be local currency. TFS defaults LCY but still validates if LCY is allowed for this transaction type. |
|  | Amount of the transaction in the currency specified in the previous field. |
|  | Deal Rate – when foreign currency is involved, TFS automatically calculates the exchange rate between the debit and credit currencies and defaults in this field. User can override the default value. |
|  | Sort Code – used for cheque collection or clearing type transactions to apply a float or hold on the funds deposited. Value in this field is ID to BC.SORT.CODE . |
|  | Consolidate Now – the user uses this to indicate that data capture of all legs have been complete and asks the system to do the consolidation. |
|  | Associated tabs to record related information like denominations, cheque or Bill payment details. All other tabs are for reference only and information in those tabs are automatically defaulted by the system. |


##### Usability

- Traversing through each field and through each leg can be done by Tab key on the keyboard and there is minimal or no need to switch frequently between mouse and keyboard.
- When the transactions (the first column) are listed in a Combo-box, typing the first letter automatically takes the user to the value – the user does not have to input the full text (For example: for FCASHDEP, the user just needs to type F and it automatically brings the focus on to the first value that starts with F.
- Following that, if the first value that starts with F is not the desired value, then the user can just use the cursor keys to scroll up and down to choose the value and press Tab or just keep pressing F until the focus comes on desired value.
- A drop-down means that the user has to click on the icon to display the list. A combo-box can display the full list by simply pressing the Alt + Down Arrow on the keyboard. It also facilitates faster input by automatically taking the focus to the value when the first letter of that value is typed.
- Note that the transaction type names in this screenshot are alpha. It is also possible to create transaction types as purely numerical value , based on how the financial institution prefers.
- The user inputs these legs and chooses Consolidate Now which results in defaulting of accounts, exchange rate conversions, validations on denominations, exposure and so on, and also creation of a consolidated transaction as yet another TFS Leg and a consolidated charge transaction as yet another TFS Leg.
- What comes back on the screen is something like shown in the next page, following which the user could address the exceptions and simply commit. The advantage of showing the denominations input as an exception is to facilitate easier navigation. Clicking on the link automatically takes the user to the denomination field instead of the user having to change tabs from the Transaction Details tab.
- TFS in-turn converts each of the TFS Legs into a child transaction under either TT or FT or DC module.
- Apart from other ways of listing the accounting entries, the search on STMT.ENTRY based on Their Reference can also be done.


###### Illustration

- A Consolidated Credit with the narrative detailing what makes up that Consolidated Credit
- A Consolidated Debit with the narrative detailing what makes up that Consolidated Debit
- In this case, just the Cash Back which is the only Debit transaction – because of the presence of a Collection cheque which had a forward exposure, credits and debits were consolidated separately
- A Consolidated Debit with the narrative detailing that it is for the Consolidated Charge.

Because in this illustration the Exposure Method is set to Lock and when Temenos Transact cheque collection is not used, TFS automatically creates an AC.LOCKED.EVENTS record to lock the funds from the collection cheque which had a forward exposure of +7 working days.

Apart from other ways of tracking the lock on funds deposited, a quick search on AC.LOCKED.EVENTS using the TFS reference number gives this.


##### Workflow

TELLER.FINANCIAL.SERVICES can be launched by one of the following workflows.

- As a drill-down from an ACCOUNT LIST enquiry The user runs an enquiry to search for the customer standing at the counter, using one of the ID information provided by the customer
- Or directly from the Menu item (as for a Walk-In Customer) This is only an illustration. Integration with a peripheral device is not within the purview of TFS.

The following section describes processing transactions via TFS

- TFS supports all the standard Temenos Transact functions. It also controls the function, authoriser requirements and status of the child transactions.
- If a TFS is input in a self authorising version, then the child transactions can also be self authorised. If TFS is input in a single authoriser version, then the child transactions can also be created in unauthorised status. When TFS is authorised, it automatically authorises the child transactions.
- Apart from native defaulting and validations performed by TFS, it presents the errors and overrides raised by the child transactions, on the screen to the user.
- If the user doesn’t have rights to approve of one or more overrides, as with any other Temenos Transact application, TFS goes to INAO status (Input Authorised but Not All Overrides Approved).
- If TFS goes to INAO, it forces the child transactions to be in INAU. Authorising (approving the overrides) TFS is in turn authorising all the child transactions.
- TFS stores the child transaction’s reference, references to the accounting entries raised and the child transaction’s record status for each TFS leg.
- Reversal of TFS legs is done by opening TFS in Input mode, setting a Reversal Mark field to R for each TFS leg that needs to be reversed.
- If consolidation is not enabled, then any individual TFS leg can be reversed independent of the other legs. If consolidation is enabled, then all TFS legs need to be reversed.
- The same concept applies for deletion of unauthorised child transactions. If the Reversal Mark field is set to R and if the child transaction is still in unauthorised status, then TFS automatically deletes the child transaction.
- As long as it has not been authorised yet, TFS allows amendments to data any number of times and automatically updates the child transactions (which is also in unauthorised status) with the changes.
- This behaviour remains the same regardless of the various combinations of functional parameters (like Consolidation, Currency conversion parameters and so on) discussed in the coming sections.
- As with TELLER or FT or DC, TFS also supports intercompany transactions – transactions on accounts that do not belong to the current Temenos Transact Company. Inter-company entries is generated.

- TFS creates the underlying child transactions even when it is in Unauthorised status (input via 1 authoriser version). Any amendment to an Unauthorised TFS leg overwrites the child transactions (although the reference remains the same).
- Once authorised, TFS does not allow any amendment to any of the transaction details( although it allows opening an authorised record in Input mode).

- It is possible to reverse just one TFS leg of a TFS transaction. However, if consolidation has been done for that TFS transaction, then all TFS legs need to be reversed. This can be done by setting the Consolidate Now field to Reverse and TFS marks each TFS leg for reversal. The system validates if all legs have been marked for reversal and throws an error if otherwise.
- Committing or authorising TFS, leads to reversal of the underlying child transactions.
- Note that when a child transaction is in history (TELLER and FT are moved to history during Temenos Transact COB), TFS creates offsetting DATA.CAPTURE legs for each of the accounting entries raised by the child transaction. The relevant parameters to this feature are Txn Rev Dc Cr and Txn Rev Dc Dr in TFS.PARAMETER and TFS.TRANSACTION and the Dc Rev On Rev field in TFS.PARAMETER .
- FT allows reversal of a transaction in history as controlled by the settings in Allow His Reversal field in FT.TXN.TYPE.CONDITION . If the FT.TXN.TYPE.CONDITION specified in TFS.TRANSACTION has this setting, TFS reverses the FT from history instead of creating DATA CAPTURE .

- If the TFS legs are in unauthorised status and if they need to be deleted while information captured on TFS needs to be retained, then the user can follow the same procedure using the Reversal Marker (explained above for Reversal of authorised TFS Legs).
- TFS recognises that the underlying child transactions are in NAU status , deletes them and clears the references stored within.
- There are a set of fields that store information about the underlying child transactions for each TFS leg. Underlying field holds the reference to the underlying child transaction. Ul Status field holds the status of the child transaction whose reference is stored in the Underyling field. R Underlying field holds the reference to the reversal of the child transaction (this is normally the same as the Underlying field unless the Reversal was done on a child in History resulting in creation of offsetting DC batches) R Ul Status field holds the status of the reversal of the child transaction whose reference is stored in R.Underlying field. Ul Stmt Nos field holds the reference to the accounting/PL entries raised by the underlying child transaction. R Ul Stmt Nos field holds the reference to the accounting/PL entries raised by the Reversal of the child transaction (either by reversing the original child transaction or by doing offsetting DC batches).

The Lock Ref field holds the references to AC.LOCKED.EVENTS records created to withhold funds availability.

Given below is a matrix of Temenos Transact Functions, value in the Reversal Mark fields and what happens to the Ul Status and R Ul Status fields

The following three sub-sections highlight the mapping between TFS fields and the fields in the child transactions.

The debit and credit accounts are populated in TELLER Side-1 or Side-2 depending on the specifications in TELLER.TRANSACTION .


##### Account Defaulting – Bank Side

This applies tp transactions where one or both sides of the transaction is the financial institution itself – For example: Cash Till, Checks Receivable, Currency Exchange, Notes Exchange and so on.

For TT Transactions, based on the underlying transaction type ( TELLER.TRANSACTION ), the system picks up the Allowed Categ.1 and Allowed Categ.2 fields and attempts to default the Cr and Dr account numbers based on the transaction currency of the TFS leg.

Such defaulting based on Allowed Categ in TELLER.TRANSACTION is not affected by any of the defaulting based on Primary Account or Surrogate Account explained below.

Such defaulting is not possible if the child transaction is on FT or DC.


##### Account Defaulting – Customer Side

There is an optional feature in TFS to key in a Primary Transaction Account of the customer so as to not repeat the same account over and again in each of the TFS legs. If this field is keyed in, TFS assumes that this account is part of each TFS leg (either debit or credit side depending on the transaction type) and automatically defaults it.

If the primary customer is keyed in, TFS defaults the first account of the customer (as stored in CUSTOMER.ACCOUNT ) in Primary Account field.

Primary Account (if supplied) is defaulted in the user input legs.

The consolidation washthru account is defaulted in the user input legs and the primary account is only used in the consolidated leg against the consolidation washthru account, there by resulting in just one entry on the primary account.

When consolidation is enabled, primary account becomes a mandatory input.

While using this primary account in the individual TFS legs:

- In simpler cases like a cash deposit ,cash withdrawal , cheque collection or a clearing type transaction, it is easy to determine the other side of the leg , which is a till account or cheques receivable account and so on.
- It gets complex when it is a transfer type of transaction – examples of this are simple account to account transfers or bill payments, loan or deposit related transactions against the primary account.

While the primary account is sufficient to default one side of the leg, there needs to be a way to default the other side of the leg without having to show both the Credit and Debit account fields on the screen which makes user input clumsy.

- In order to facilitate easy user input and defaulting, TFS has what is called as a Surrogate Account, associated with each TFS leg. This field as the name stands for, is a surrogate to either the debit or credit side of the leg. The user has to just key-in this field with whatever the other side of the leg should be – there is no need to think/decide whether it is the debit or the credit side.
- This can be used either as one side of the TFS leg with the primary account being on the other side of that TFS leg or instead of the primary account but just for that TFS leg. Both scenarios are explained below.

TFS automatically defaults the primary account on one side and the surrogate account as the other side of the TFS leg. To know if the surrogate account for a given TFS leg corresponds to the debit or the credit side, is determined by the setting in the Surrogate Ac field in TFS.TRANSACTION to either ACCOUNT.CR or ACCOUNT.DR (indicating clearly that the value in surrogate account has to be defaulted as the credit account or debit account on that TFS leg. Instead of having just one transaction type as Account to Account Transfer, there are two TFS transaction types – From And To.

Given below is an illustration of how TFS TRANSACTION is setup for account to account transfers FROM and TO.

The user keys in the following values.

- The first leg means, Transfer GBP 150.00 FROM A/C 22594 (Surrogate Account) to A/C 22462 (Primary Account).
- The second leg means, Transfer EUR 135.00 TO A/C 22586 (Surrogate Account) from A/C 22462 (Primary Account).

The TFS defaults the following values.

- Surrogate account in the 1st leg becomes the debit account and the primary account becomes the credit account.
- Surrogate account in the 2nd leg becomes the credit account and the primary account becomes the debit account.

This same concept can be applied to other transaction types like,

- Bill Payment (where the surrogate account which is keyed in with the payee account number, is set to default the credit account).
- Cheque Encashment (where the surrogate account which is keyed in with the account number on the cheque, is set to default the debit account).
- Loan Repayment (where the surrogate account which is keyed in with the loan account number, is set to default the credit account).

If there is a specific setting in TFS.TRANSACTION on what the surrogate account should stand for, the Surrogate Ac field in TELLER.FINANCIAL.SERVICES becomes a mandatory input for the associated TFS leg. If the user does not input any value, TFS raises an error.

When there is no specific setting in TFS.TRANSACTION on what the surrogate account should stand for, it is used to simply take precedence over the primary account, for the associated TFS leg.

Consider that one of the five TFS legs in a TFS transaction is a cash deposit and the customer wants to make the deposit to a savings account just for this TFS leg.

One side of this TFS leg is the till account. In a normal course of operation, TFS uses the primary account to be the other side. To honour the customer’s request, the user can just key in the savings account in the Surrogate Ac field on that TFS leg.

In this case, the surrogate account takes precedence over the primary account and TFS defaults this surrogate account as the credit account for that TFS leg alone.

This leg is ignored during consolidation.


##### Inter-Company Transactions

TFS supports transactions on accounts that do not belong to the current logged in Temenos Transact Company. However this is applicable only if the customer is shared between the Temenos Transact Company where the customer of the financial institution belongs to and the Temenos Transact Company that the user is currently logged onto.

Consider an account 4000000251 which belongs to the Temenos Transact Company GB-001-0002.

The following TFS transaction is done in Temenos Transact Company GB-001-0001


##### Market Exchange Profit

When enabled in TELLER.PARAMETER in the Mkt Exch Method field as MIDDLE, TELLER calculates market exchange profit as the difference in LCY equivalents of debit and credit sides of a transaction, arrived at using buy-sell rate and mid-reval rate.

From TFS, there is a flexibility to define if TELLER has to calculate this for all transactions (specified at TFS.PARAMETER level) or only specific transactions (specified at TFS.TRANSACTION level).

The following two examples use FCASHDEP which is set not to calculate market exchange profit and XCHANGE transaction which is set to calculate market exchange profit. It can be observed that TFS forces TELLER not to calculate the market exchange profit for FCASHDEP.

In this transaction, the customer makes a GBP cash deposit into a USD Account

It can be observed that the Market Exch Profit is calculated neither by TFS nor by TELLER.

In this transaction the financial institution buys GBP and sells USD.

It can be observed that there is a market exchange profit of USD 2 calculated by TFS. In this case, USD 192.00 is arrived based on the user supplied rate (or when defaulted by the system based on buy or sell rate) and USD 194.00 is based on mid reval rate between GBP and USD.


##### Consolidation

- Consolidation of user input legs in a TFS transaction is controlled by Consolidation field in TFS.PARAMETER and Consol Instruction field in TFS.
- If consolidation is enabled at TFS.PARAMETER level, it is possible to disable at the TFS level. However if consolidation is disabled at TFS.PARAMETER level, it is not possible to enable it at TFS level.
- The Consol Method consolidation parameter is also available at TFS level so the user has the choice to override Temenos Transact company-wide settings for a given TFS transaction.
- This implies that, though the Temenos Transact company-wide parameter may be set to consolidate as NET (debits and credits together), it is possible to consolidate as GROSS (debits separately and credits separately) at an individual TFS level.
- Similarly, even though the Temenos Transact company-wide parameter for add-on consolidation factors ( Consol Level Addon ) may be set to NO, it is possible to use Currency or Currency + Transaction type or Transaction type as add-on consolidation factors at an individual TFS level.
- If the financial institution doesn’t want the user to have this choice, then these fields can be hidden from the TFS version and restrict the user to Temenos Transact company-wide parameter definition (which TFS automatically inherits from the parameter).

Consol Instruction=YES), for each of the user input legs, instead of defaulting the primary account on one side of the leg, TFS uses an internal washthru account belonging to the category specified in TFS.PARAMETER .

Example:

In the example of a foreign cash deposit (GBP 100) and a local currency cash deposit (USD 100), the user can provide the below details.

When the user indicates completion of the user input legs by setting Consolidate Now to Yes, the below screen appears.

In the two user input legs, the credit side is defaulted with the consolidation washthru account.

The main transaction details with all the legs are shown in the below screen.

The accounting entries for this TFS Transaction are shown below. The TFS transaction reference is available in the Their Reference field in all entries, for easy trace-back.

In the following sections, it can seen how the consolidation behaviour changes based on different combinations of parameters.

Consider an example where the customer who has GBP 100, USD 100 (local currency) requires cash back of USD 10 and transfers USD 15 to one of his other accounts 22578.

The Enable Consolidation , Consol Method and Consol Level Addon fields are automatically defaulted by TFS based on settings in TFS.PARAMETER .

In both scenarios below, Consolidation is enabled and Consol Level Addon is set to NO.

When Consol Method is set to Net, all credits and debits are consolidated together to produce just one entry (of course there are exceptions to this scenario but this is the typical result)

One entry is raised on the primary account (apart from the consolidated charge).

The same narrative is available on the TFS screen under the Statement Narrative tab.

When Consol Method is set to Gross, credits and debits are consolidated separately to produce two entries on the customer account.

There are two entries on the primary account (apart from the consolidated charge).

The same narrative is available on the TFS screen under the Statement Narrative tab.

In the below scenarios, Consolidation is enabled and Consol Method is set to Net.

An illustration of consolidation by currency is shown below. The same applies for other factors like Transaction Type ( TFS.TRANSACTION ) and Currency + Transaction Type.

When Consol Level Addon is set to CCY, then even though currency conversion takes place in the user input leg, they are consolidated by the currency of the Leg during consolidation.

There are two entries on the primary account (apart from the consolidated charge).

The same narrative is available on the TFS screen in the Statement Narrative tab.

This happens only when Consol Method is set to NET. To mitigate, there are three options.

- Force Gross – Undo NET consolidation and re-do Consolidation as GROSS , one credit and one debit entry are raised on the customer account.
- Ignore the consolidated leg – which results in no entry being raised on the customer account.
- Undo Consolidation – Undo all consolidation and each user input TFS leg hits the customer account directly.

Example:

Consider a cash deposit of USD 100, an account transfer into the primary account for USD 50 and an account transfer out of the primary account for USD 150.00 making the net total to 0.

Based on TFS.PARAMETER which is set to Force Gross, TFS has created two consolidated legs.

For the same example, when Consol Amt Zero is set to Undo Consolidation, the system automatically sets Consol Instruction to NO and forces each user input leg to hit the primary account directly. Consolidated charge is not applicable in this case since consolidation does not happen and individual leg level charging can be applied.

For the same example, when Consol Amt Zero is set to Ignore Consol Leg , then the 0 amount consolidated leg is ignored and the result is no entry hitting the customer account at all – except for the consolidated charge.

The reason why the consolidated charge is still applied here is because it is after all a composite transaction.

- In the normal course of operation, the user inputs all the legs per customer’s instructions and instructs TFS to consolidate the legs by setting the Consolidate Now field to YES.
- After TFS inserts the consolidated leg(s), but before committing the transaction, if the user amends any transaction details (currency, amount, deal rate and so on) on the original user input legs, then the user must instruct TFS again, explicitly, to consolidate the legs again by setting the Consolidate Now field to YES again. This is the reason TFS automatically sets this field back to “” every time.
- If the user does not Consolidate again, there is a balance left behind in the washthru account due to change in the transaction information. If the running total in any of the washthru accounts is not 0, then TFS does not allow the user to commit the transaction.
- In the illustration below, the user inputs cash deposit and a transfer from another account and instructed TFS to consolidate. TFS generates a consolidated leg and a consolidated charge.

- Now the user changes the cash deposit amount from 100 to 150 and tries to commit the transaction. Because of the change, the amount credited to the washthru account in the user input leg is different from what was debited from the washthru account in the consolidated leg and results in a balance in the running total.
- The sum of user input legs (300.00) is not the same as the consolidated leg (250.00) leaving the difference (50.00) in the washthru account which is what it returns as error. Ignore the denomination error as it is irrelevant in this context.
- Regardless of whether it is local currency or foreign currency leg, any change to any transaction detail (currency, amount, deal rate and so on) results in the same error if the user didn’t instruct TFS to consolidate again.
- However this doesn’t include any non-transactional change on the user input TFS legs. For example, if the user changed the Sort code after consolidating, it does not reflects on the consolidated leg if the user didn’t set Consolidate Now to YES before committing. In this case, the system does not raise an error and the transaction goes through.
- Now the user can set Consolidate Now to YES again and commit. TFS now completely refreshes the consolidated leg and the consolidated charge.

This section lists the scenarios as exceptions in consolidation, even if enabled.

When a TFS transaction consists of credit and debit TFS legs and if the credit TFS leg contains a forward exposure, consolidation gets forced to be on GROSS basis. This applies even if that credit with the forward exposure carries a different value date from the debit transaction.

If for a TFS leg, the Consol Exclude field in the respective TFS.TRANSACTION is set to YES, then that TFS leg is excluded from consolidation.

Example: For collection or a clearing cheque for which CHEQUE.COLLECTION record needs to be created.

When consolidated amount is 0 and Consol Amt Zero in TFS.PARAMETER is set to either Ignore Consol Leg or Undo Consolidation.


##### Forward Exposure

Any deposit transaction type can use this Collection or Clearing Cheques feature to withhold funds availability.

For collection cheques or clearing cheques, normally Temenos Transact Cheque Collection is used to control the life of the cheque and there by the availability of funds for the Customer.

If a financial institution does not want to use cheque collection but still wants to be able to apply a hold on the funds deposited, they can do so using Temenos Transact Exposure date feature.

TFS allows application of a hold either by means of a forward exposure date or by locking the funds using AC.LOCKED.EVENTS . This is controlled by the Exposure Method field in TFS.PARAMETER .

Consider a customer comes in with a cheque to be sent for collection USD 150.00 and another cheque for local clearing USD 250.00 and a cash deposit of USD 100. Assume that the Value Date for all these legs is the same.

In both approaches, the user does not have to key in the hold date. TFS uses the Sort Code field (where the user typically keys in the sort code on the cheque – this corresponds to BC.SORT.CODE in Temenos Transact where the hold period is specified) to calculate the hold date. In both approaches, capture of information is the same and the difference is the background process.

In the illustration, there are two demo BC.SORT.CODE records uses – COLL (which carries +7W hold) and LCLG (which carries +1W hold) which the user keys in the Sort Code field.

TFS uses the multi exposure split date feature to apply different exposures for portions of the consolidated amount, based on the original transaction.

In the below screenshot, the collection cheque USD 150.00 carries +7W (15 JUL 2009) and Clearing Cheque USD 250.00 carries +01W (08 JUL 2009) while the cash deposit USD 100.00 has Same Day Availability(06 JUL 2009).

When Exposure Method in TFS.PARAMETER is set to Float, for the example above, the Exposure split dates and amounts have been passed onto TELLER which in turn is passed it on to STMT.ENTRY .

The respective portions of the funds are made available for withdrawal on the start of day of their corresponding Exposure dates.

When Exposure Method in TFS.PARAMETER is set to Lock, for the example above, there are two AC.LOCKED.EVENTS records created with TO.DATE as the Split Date shown in screen shot above. To revise the hold, the AC.LOCKED.EVENTS record can be directly reversed and re-booked.

Reversing TFS Legs also automatically reverses all AC LOCKED EVENTS records created by that TFS Transaction.

The respective portions of the funds are made available for withdrawal on the start of day of their corresponding To Dates.

The below screenshot shows the clearing cheque with lock period until 08 JUL 2009.

The below screenshot shows the collection cheque with lock period until 15 JUL 2009


##### Transaction Limit Validations

There are three different overrides that might be raised based on what is defined and what is not.

- When Limit is specified for the transaction currency
- When Limit is not specified for the transaction currency but global LCY limit is specified. TFS still raises limit not defined override in this case too
- When Limit is not specified for the transaction currency and global LCY limit is also not specified

All these three overrides are illustrated in the screenshot below.

This is the setup.

- Even though the GBP limit at TFS.PARAMETER level is set to 5,000.00, the settings in TFS.TRANSACTION (2,500.00) takes precedence and hence the warning that the transaction breaches the Limit
- There is no limit specified for the CAD currency. So TFS raises an override to that effect.
- Since there is a Global LCY limit specified in TFS.PARAMETER level, TFS calculates the LCY equivalent of the CAD amount and compares it against the LCY limit. Since CAD 12,000.00 is above the LCY limit of 7,500.00, it raises an override to that effect.


##### AML or KYC Validations

TFS allows capture of customer information (even for walk-in Customers) for both KYC and AML purposes.

- This information is similar to the information captured when creating a new customer.
- The user has the choice to indicate which customer number to be used for AML purposes. If left blank, then system automatically defaults the PRIMARY.CUSTOMER .
- When it defaults, it also raises an override to that effect.
- For walk-in customers, the user can input the rest of the fields. If the Aml Details field in TFS.PARAMETER is set to Validation, then TFS validates the expiry date of the legal document.
- For existing customers, based on the CUSTOMER table, the system raises an override. If the document has expired. If no AML information had been captured in CUSTOMER .

For walk-in customers, based on the transaction details, and the system raises an override.

- If the document has expired
- If no AML information has been captured in TFS


##### Bill Payment

For bill payment, it is possible to directly enter the payee account number in the Surrogate Ac field or use the Beneficiary Feature to default the Payee account number.

A customer is most likely to use the Payee from the list of Payees created via ARC IB, even when he or she comes to a branch to do a bill payment. In such cases, the list of Payees are in BENEFICIARY table in Temenos Transact .

Example:

The below example explains the process of bill payments using TFS (TFS does not support wire or telex transfers or SWIFT generation)

Once the transaction type and amount details are entered as shown above, the user needs to go to the Bill Payment tab and choose a beneficiary from the drop down. The user can also enter custom payment details which are passed onto the child transaction in FT.

Upon choosing the beneficiary, since this is a hot field, the system immediately validates and defaults the payee account number in the Surrogate Ac field.

Since in TFS.TRANSACTION of BILLPAY, the Surrogate Ac is set to ACCOUNT.CR, this surrogate account is later defaulted as the credit account.

This diagram represents the process flow for TELLER.FINANCIAL.SERVICES .


#### 📋 Tasks

Related topics:

- Receive or Execute Teller Financial Services

Teller Financial Services facilitates capture of information for many transactions in one screen and with one click it creates a consolidated entry (which can be parameterised) on the customer account, a consolidated charge and transaction advice.


##### Workflow

The user can perform the following activities:

Teller Financial Services captures all the information in one screen of Teller Financial Services, but creates separate entries on the customer account for each of them.

To initiate a Teller transaction, follow the below steps:

1. Teller Operations .
2. In the Transaction screen, enter values in the following fields: Primary Account Transaction Account CCY Amount Deal Rate
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon to submit the record.


#### 📊 Outputs

Teller Financial Services is a companywide parameter table that allows configuration of how consolidation has to happen, user friendliness, security parameters among others.


##### Enquiries and Reports

NA


##### SWIFT Messages

NA


##### Advices

The user can view the below list of advices:

This advice helps the user to capture the information of many transactions in one screen and displays the consolidated charge and consolidated transaction.


##### Alerts

NA

---


---


## Appendix A: Glossary of T24 Applications & Fields


This glossary lists all T24/Transact application names and field names referenced throughout this document, with descriptions where available.


### Applications


| Application | Description |
|------------|-------------|
| `ACCOUNT.STATEMENT` | T24 application: ACCOUNT.STATEMENT |
| `BC.SORT.CODE` | T24 application: BC.SORT.CODE |
| `CARD.ISSUE` | T24 application: CARD.ISSUE |
| `CHEQUE.REGISTER.SUPPLEMENT` | T24 application: CHEQUE.REGISTER.SUPPLEMENT |
| `CHEQUE.TYPE` | T24 application: CHEQUE.TYPE |
| `DEAL.SLIP.FORMAT` | T24 application: DEAL.SLIP.FORMAT |
| `DENOM.TYPE` | T24 application: DENOM.TYPE |
| `FUNDS.TRANSFER` | T24 application: FUNDS.TRANSFER |
| `STOCK.ENTRY` | T24 application: STOCK.ENTRY |
| `STOCK.PARAMETER` | T24 application: STOCK.PARAMETER |
| `TELLER` | T24 application: TELLER |
| `TELLER. TRANSACTION` | T24 application: TELLER. TRANSACTION |
| `TELLER.DENOMINATION` | T24 application: TELLER.DENOMINATION |
| `TELLER.ID` | T24 application: TELLER.ID |
| `TELLER.PARAMETER` | T24 application: TELLER.PARAMETER |
| `TELLER.PASSBOOK` | T24 application: TELLER.PASSBOOK |
| `TELLER.PASSBOOK.STMT` | T24 application: TELLER.PASSBOOK.STMT |
| `TELLER.PBOOK.PRINTED` | T24 application: TELLER.PBOOK.PRINTED |
| `TELLER.TRANSACTION` | T24 application: TELLER.TRANSACTION |
| `TERMINAL` | T24 application: TERMINAL |
| `TFS.PARAMETER` | T24 application: TFS.PARAMETER |
| `TRANSACTION` | T24 application: TRANSACTION |
| `TT.END.OF.DAY` | T24 application: TT.END.OF.DAY |
| `TT.GROUP.CONDITION` | T24 application: TT.GROUP.CONDITION |
| `TT.TELLER.HP.VERSIONS` | T24 application: TT.TELLER.HP.VERSIONS |


### Fields Referenced


| Field | Field | Field |
|-------|-------|-------|
| `Account` | `Account Cr` | `Account Dr` |
| `Account Number` | `Allow His Reversal` | `Allowed Categ` |
| `Allowed Categ.1` | `Allowed Categ.2` | `Aml Details` |
| `Aml Lookup` | `Amount` | `Amount Deposited` |
| `Amount Foreign` | `Amount Local` | `Arrangement` |
| `Assigned Category` | `Attribute` | `Auto Denominate` |
| `Benef Customer` | `Beneficiary ID` | `Buy Fcy Sell Fcy` |
| `Buy Fcy Sell Lcy` | `Buy Fcy Sell Lcy, Buy Lcy Sell Fcy, Buy Fcy Sell Fcy` | `Buy Lcy Sell Fcy` |
| `By Currency` | `CCY` | `Ccy Limit` |
| `Central Bank Acct` | `Charge Account` | `Charge Type` |
| `Check Stock Amt` | `Cheque Bank Cde` | `Cheque No` |
| `Cheque Number` | `Cheque Type` | `Chg Discount Amt` |
| `Chg Maximum Amt` | `Chg Minimum Amt` | `Chg Percent` |
| `Chg Premium Amt` | `Chg Type` | `Comm Type` |
| `Comments` | `Consol Amt Zero` | `Consol Chg Api` |
| `Consol Chg Tfs` | `Consol Chg Tfs Txn` | `Consol Exclude` |
| `Consol Instruction` | `Consol Level Addon` | `Consol Method` |
| `Consol Narr` | `Consol Narr Api` | `Consol Sort Code` |
| `Consol Tfs Txn` | `Consol Washthru` | `Consolidate Now` |
| `Consolidation` | `Contract Group` | `Cr Denom Type` |
| `Cr Txn Code` | `Credit Account` | `Credit Account Number` |
| `Credit Currency` | `Credit Currency/Amt` | `Credit Narrative` |
| `Credit Stock` | `Currency` | `Currency Deposited` |
| `Customer.2` | `Dc Rev On Rev` | `Deal Rate` |
| `Debit Account` | `Debit Stock` | `Debit Value Date` |
| `Decis` | `Denom Filter` | `Denom Type` |
| `Denomination` | `Denomination details` | `Deposit Amount` |
| `Description` | `Dr Denom Type` | `Dr Txn Code` |
| `Enable Consolidation` | `End Date` | `Enter Balance` |
| `Exc From Txn Limit` | `Exchange rate` | `Exp Date Prd` |
| `Exp Split Amt` | `Exp Split Dat` | `Exp Split Date` |
| `Exposure Date` | `Exposure Method` | `Fixed Amount` |
| `Foreign Currency Amount` | `From Teller` | `GB Narrative` |
| `Hot Field` | `Hot Fields` | `Ignore Consol Leg` |
| `Interface Api` | `Interface As` | `Interface To` |
| `Internal` | `Issue Cheque Type` | `LCY Amount` |
| `Lcy Limit` | `Legal Doc Name` | `Legal Iss Auth` |
| `Limit Ccy` | `Line No` | `Line, Page No` |
| `Linked Tills` | `Lock Ref` | `MT103 Receiver Bank` |
| `Max Tills` | `Maximum Amt` | `Minimum Amt` |
| `Mkt Exch Method` | `Mkt Exch Profit` | `Multi Tills` |
| `Narrative` | `Narrative.1` | `New Passbook` |
| `Notes` | `OFS Version` | `Ofs Source` |
| `Ofs Version` | `Our Reference` | `Page No` |
| `Page, Line` | `Passbook` | `Passbook Device` |
| `Passbook ID` | `Payee Name` | `Payment Account` |
| `Payment Currency` | `Primary Account` | `Print Passbook` |
| `Prt Lang` | `R Ul Status` | `R Ul Stmt Nos` |
| `R Underlying` | `Rate Spread` | `Reset Fields` |
| `Reversal Mark` | `Reverse` | `Sector` |
| `Sort Code` | `Start Date` | `Stock Number` |
| `Stock Reg Id` | `Stock Upd` | `Surrogate Ac` |
| `Surrogate Account` | `TC Account` | `TC Account.1` |
| `TC Amount` | `TC Amount.1` | `TC Contra Account` |
| `TC Currency` | `TC Debit Account` | `Teller` |
| `Their Reference` | `Till Account` | `Till Id` |
| `Till Status` | `Till Trf Only` | `To Teller` |
| `Tran category` | `Transaction` | `Transaction Code` |
| `Txn Ccy To Cr Ccy` | `Txn Ccy To Dr Ccy` | `Txn Lookup` |
| `Txn Rev Dc Cr` | `Txn Rev Dc Dr` | `Type` |
| `Ul Status` | `Ul Stmt Nos` | `Underlying` |
| `Update Stock` | `Validate Payee Name` | `Validity` |
| `Value Date Prd` | `Vault Account` | `Waive Charge` |
| `Waive Charges` | `Withdrawal Amount` | `Withdrawal Currency` |
| `onsol Level Addon` |  |  |


---


## Appendix B: Consolidated Field Reference


This appendix consolidates all field description tables from across the documentation, grouped by sub-module. This provides a single reference for all field definitions.


### Staff_Channel - TT (TT)


**Teller Financial Services**

| Callout Numbers | Description |
|---|---|
|  | Transaction Reference |
|  | Field to indicate at TFS level if consolidation has to be enabled for this TFS transaction or not. Defaulted to the setting in TFS.PARAMETER but can be changed by user. The same applies to Consol Method and C onsol Level Addon fields. |
|  | Primary account to be used in this TFS Transaction –this is the transaction account of the Customer – Current Account or Checking Account and so on. But it could be any type of account , it even accepts internal accounts. |
|  | Customer number of the primary account holder (Populated when launching the deal from an enquiry drill down or when Consolidate Now is set to Yes. |
|  | TFS Transaction type displayed as a combo-box. |
|  | Surrogate Account – no input required in this field except for account-account transfer type of transactions (including Bill payments).When input, this is used as one side of that TFS leg, with the primary account being on the other side. |
|  | Currency of the Transaction (need not be either the debit currency or the credit currency). If left blank, it is assumed to be local currency. TFS defaults LCY but still validates if LCY is allowed for this transaction type. |
|  | Amount of the transaction in the currency specified in the previous field. |
|  | Deal Rate – when foreign currency is involved, TFS automatically calculates the exchange rate between the debit and credit currencies and defaults in this field. User can override the default value. |
|  | Sort Code – used for cheque collection or clearing type transactions to apply a float or hold on the funds deposited. Value in this field is ID to BC.SORT.CODE . |
|  | Consolidate Now – the user uses this to indicate that data capture of all legs have been complete and asks the system to do the consolidation. |
|  | Associated tabs to record related information like denominations, cheque or Bill payment details. All other tabs are for reference only and information in those tabs are automatically defaulted by the system. |


---
