
# Temenos Transact — Trade_Banking Module Documentation


> **Comprehensive User Guide**
> Generated: 13 April 2026
> Content: Configuration | Reference | Field Descriptions | Glossary


## Table of Contents

  - [Trade_Banking Module Overview](#trade_banking-module-overview)
    - [Sub-Module Summary](#sub-module-summary)
    - [How to Use This Guide](#how-to-use-this-guide)
  - [Chapter 1: Trade_Banking - FF](#chapter-1-trade_banking---ff)
    - [Features in Trade_Banking - FF](#features-in-trade_banking---ff)
    - [1.1  Automatic Upload and Batching](#11-automatic-upload-and-batching)
    - [1.2  Charges](#12-charges)
    - [1.3  Disbursement and Settlement](#13-disbursement-and-settlement)
    - [1.4  Manual Upload and Batching](#14-manual-upload-and-batching)
    - [1.5  Misc](#15-misc)
    - [1.6  Product Type](#16-product-type)
    - [1.7  Products](#17-products)
  - [Chapter 2: Trade_Banking - LC](#chapter-2-trade_banking---lc)
    - [Features in Trade_Banking - LC](#features-in-trade_banking---lc)
    - [2.1  Amendment](#21-amendment)
    - [2.2  Assignment of proceeds](#22-assignment-of-proceeds)
    - [2.3  Avalisation under Collection](#23-avalisation-under-collection)
    - [2.4  Brokerage](#24-brokerage)
    - [2.5  Charges and Commission](#25-charges-and-commission)
    - [2.6  Collection](#26-collection)
    - [2.7  Collection Amendment](#27-collection-amendment)
    - [2.8  Drawings](#28-drawings)
    - [2.9  Islamic LoC](#29-islamic-loc)
    - [2.10  Issuance or Register of a LC](#210-issuance-or-register-of-a-lc)
    - [2.11  Managing External Requests](#211-managing-external-requests)
    - [2.12  Margin or Provisions](#212-margin-or-provisions)
    - [2.13  Merchanting Trade](#213-merchanting-trade)
    - [2.14  Misc](#214-misc)
    - [2.15  Open Account Trade](#215-open-account-trade)
    - [2.16  Post Shipment Finance](#216-post-shipment-finance)
    - [2.17  Pre-shipment Finance](#217-pre-shipment-finance)
    - [2.18  Pre advice of a LC](#218-pre-advice-of-a-lc)
    - [2.19  Reversal or Cancellation](#219-reversal-or-cancellation)
    - [2.20  RMA Verification](#220-rma-verification)
    - [2.21  Shipping Guarantee](#221-shipping-guarantee)
    - [2.22  Shipping Guarantee against Import Collection](#222-shipping-guarantee-against-import-collection)
    - [2.23  Syndicated Letter of Credit](#223-syndicated-letter-of-credit)
    - [2.24  TBML Check for Letter of Credit](#224-tbml-check-for-letter-of-credit)
    - [2.25  Tickler and Tracers](#225-tickler-and-tracers)
    - [2.26  Trade Based Lending](#226-trade-based-lending)
    - [2.27  Trade Evidence For Advance Payment](#227-trade-evidence-for-advance-payment)
  - [Chapter 3: Trade_Banking - MD](#chapter-3-trade_banking---md)
    - [Features in Trade_Banking - MD](#features-in-trade_banking---md)
    - [3.1  Amendment of Issued or Registered Guarantees](#31-amendment-of-issued-or-registered-guarantees)
    - [3.2  Cancel Reinstate Guarantee](#32-cancel-reinstate-guarantee)
    - [3.3  Collateral](#33-collateral)
    - [3.4  Commission and Charges](#34-commission-and-charges)
    - [3.5  Expiry or Reinstate Expired Guarantee](#35-expiry-or-reinstate-expired-guarantee)
    - [3.6  Issue Register Guarantee](#36-issue-register-guarantee)
    - [3.7  Managing External Requests](#37-managing-external-requests)
    - [3.8  Margin or Provision](#38-margin-or-provision)
    - [3.9  Misc](#39-misc)
    - [3.10  Multi Party Guarantee](#310-multi-party-guarantee)
    - [3.11  Non Extension Guarantee](#311-non-extension-guarantee)
    - [3.12  Pay Reject Claim under Guarantee](#312-pay-reject-claim-under-guarantee)
    - [3.13  Presentation under SBLC](#313-presentation-under-sblc)
    - [3.14  Register Claim under Guarantee](#314-register-claim-under-guarantee)
    - [3.15  Reimbursement Processing SBLC](#315-reimbursement-processing-sblc)
    - [3.16  RMA Verification](#316-rma-verification)
    - [3.17  Standby Letterr of Credit](#317-standby-letterr-of-credit)
    - [3.18  Syndicate Guarantee](#318-syndicate-guarantee)
    - [3.19  TBML Check for Guarantee and SBLC](#319-tbml-check-for-guarantee-and-sblc)
  - [Chapter 4: Trade_Banking - SU](#chapter-4-trade_banking---su)
    - [Features in Trade_Banking - SU](#features-in-trade_banking---su)
    - [4.1  Facility Agreement](#41-facility-agreement)
    - [4.2  Finance Request](#42-finance-request)
    - [4.3  Invoice Batching](#43-invoice-batching)
    - [4.4  Invoice Capture](#44-invoice-capture)
    - [4.5  Misc](#45-misc)
  - [Chapter 5: Trade_Banking - TCIB](#chapter-5-trade_banking---tcib)
    - [Features in Trade_Banking - TCIB](#features-in-trade_banking---tcib)
    - [5.1  Collection](#51-collection)
    - [5.2  Export Drawings](#52-export-drawings)
    - [5.3  Export LC Advising](#53-export-lc-advising)
    - [5.4  Export LC Amendemnt Advising](#54-export-lc-amendemnt-advising)
    - [5.5  Guarantee Amendment](#55-guarantee-amendment)
    - [5.6  Guarantee Claims](#56-guarantee-claims)
    - [5.7  Guarantee Issuance](#57-guarantee-issuance)
    - [5.8  Guarantees Received](#58-guarantees-received)
    - [5.9  Import Drawings](#59-import-drawings)
    - [5.10  Import LC Amendment](#510-import-lc-amendment)
    - [5.11  Import LC Issuance](#511-import-lc-issuance)
    - [5.12  Misc](#512-misc)
    - [5.13  TCIB Dashboard](#513-tcib-dashboard)
  - [Appendix A: Glossary of T24 Applications & Fields](#appendix-a-glossary-of-t24-applications-fields)
    - [Applications](#applications)
    - [Fields Referenced](#fields-referenced)
  - [Appendix B: Consolidated Field Reference](#appendix-b-consolidated-field-reference)
    - [Trade_Banking - FF (FF)](#trade_banking---ff-ff)
    - [Trade_Banking - LC (LC)](#trade_banking---lc-lc)
    - [Trade_Banking - MD (MD)](#trade_banking---md-md)
    - [Trade_Banking - SU (SU)](#trade_banking---su-su)
    - [Trade_Banking - TCIB (TCIB)](#trade_banking---tcib-tcib)

---


## Trade_Banking Module Overview


This document provides comprehensive documentation for the **Trade_Banking** module of Temenos Transact. It covers **5 sub-modules** with a total of **71 feature areas**.


### Sub-Module Summary


| # | Sub-Module | Code | Features | Description |
|---|-----------|------|----------|-------------|
| 1 | **Trade_Banking - FF** | `FF` | 7 | Trade_Banking - FF module of Temenos Transact |
| 2 | **Trade_Banking - LC** | `LC` | 27 | Trade_Banking - LC module of Temenos Transact |
| 3 | **Trade_Banking - MD** | `MD` | 19 | Trade_Banking - MD module of Temenos Transact |
| 4 | **Trade_Banking - SU** | `SU` | 5 | Trade_Banking - SU module of Temenos Transact |
| 5 | **Trade_Banking - TCIB** | `TCIB` | 13 | Trade_Banking - TCIB module of Temenos Transact |


### How to Use This Guide


Each feature in this document is organized into the following sections:

- 📖 **Introduction** — Overview and purpose of the feature
- ⚙️ **Configuration** — How to set up and configure the feature
- 🔧 **Working With** — Operational usage and field descriptions
- 📋 **Tasks** — Step-by-step procedures
- 📊 **Outputs** — Reports, enquiries, and generated outputs

Each feature includes a **Quick Reference Card** at the top with application names, key fields, prerequisites, and a summary. Appendices provide a full glossary, consolidated field tables, and end-to-end use-case scenarios.

---


## Chapter 1: Trade_Banking - FF


Trade_Banking - FF module of Temenos Transact


### Features in Trade_Banking - FF


| # | Feature | Sections |
|---|---------|----------|
| 1.1 | Automatic Upload and Batching | Intro, Confi, Tasks, Outpu |
| 1.2 | Charges | Intro, Confi, Tasks, Outpu |
| 1.3 | Disbursement and Settlement | Intro, Confi, Tasks, Outpu |
| 1.4 | Manual Upload and Batching | Intro, Confi, Tasks, Outpu |
| 1.5 | Misc | Intro |
| 1.6 | Product Type | Intro, Confi, Tasks, Outpu |
| 1.7 | Products | Intro, Confi, Tasks, Outpu |


### 1.1  Automatic Upload and Batching


> **📇 Quick Reference Card**
> 
> **Purpose:** *Corporates and SMEs are embracing digital working models. The Enterprise Resource Planning (ERP) systems at the corporate have the potential to generate a list of invoices in soft copies. Temenos Transact is aligned to receive and upload invoice details received in soft copies, which has several ben...*
> 
> **Key Fields:** *Decision*, *Doc Back Val Days*, *Duplicate Check*, *Upload Reference*, *Upload Type*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Corporates and SMEs are embracing digital working models. The Enterprise Resource Planning (ERP) systems at the corporate have the potential to generate a list of invoices in soft copies. Temenos Transact is aligned to receive and upload invoice details received in soft copies, which has several benefits, such as,

- Reduce human errors
- Increase in productivity and efficiency
- Fast reconciliation

Temenos Transact accepts files with extension .CSV. It creates individual bill records for each of the invoices from the list of successfully uploaded file. Errors are marked as exceptions for correction. The number of records in the upload file can be easily reconciled.

At the time of upload, certain checks are configured. Fields are defined to check for duplicate values in the EB.DUPLICATE.TYPE application. It is attached to the Duplicate Check field in BL.PARAMETER application. The product type is automatically assigned to each bills ( BL.REGISTER ) based on the user defined conditions. Factoring requires grouping of bills into batches on common parameters.

Bills are generated in USD for a corporate customer.

The field values for grouping logic is defined in the BL.BATCH.CONDITIONS table. The date of the uploaded invoices are backdated up to the number of days defined in Doc Back Val Days field. Otherwise, the system generates an override.


#### ⚙️ Configuration

The following configurations are setup at the parameter level.


##### Default Conditions for Updating the Product Type

Conditions for updating the product type in the BL registers, based on the default or customer level conditions are defined in the BL.BATCH.CONDITIONS table.

> **⚠️ Note:** The record ID can be Company ID – PRODUCT or Customer ID – PRODUCT

The below screenshot shows company level product conditions.

The below screenshot shows customer level product conditions.


##### Default Conditions for Batching

The BL registers created from the same upload reference is batched based on the conditions defined in the BL.BATCH.CONDITIONS . The default (mandatory) conditions are currency, liability customer and product type ID.

> **⚠️ Note:** Product type ID can be company ID – BATCH or customer ID – BATCH.

The below screenshot shows customer level batch conditions.


##### File Upload Type

The user creates a record in the EB.FILE.UPLOAD.TYPE defining the file name, type and version of BL.REGISTER .

> **⚠️ Note:** Currently, .CSV file type is supported.


#### 📋 Tasks

Related topics:

- Process Settlement of Receivables
- Batch Receivables Registers
- Factoring and Forfaiting Processes

Automatic Upload and Batching provides the users with the options to Register, Batch and Rebatch the receivables with zero authorisation.


##### Workflow

The user can register, authorise and delete the receivables by using the below workflow:

This menu allows the user to upload the receivables with zero authorisation through EB.FILE.UPLOAD application.

To upload the receivables, follow the below steps:

1. Upload Receivables .
2. Enter or select a value in the Upload Type field.
3. Choose a file to upload.
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon to submit the record.

This menu displays the list of BL.REGISTER application records, which are in On Hold (IHLD) status, where the user can amend or delete the individual records with zero authorisation version.

To amend or delete the upload errors, follow the below steps:

1. Amend/Delete Upload Errors .
2. Enter a value in the Upload Reference field and click the FIND button.
3. In Upload Record Line Number screen, click the Amend icon to amend the field values as required.
4. Click the Validate icon to check for errors and overrides
5. Click the Commit icon to submit the record.

To delete the upload errors, follow the below steps:

1. Amend/Delete Upload Errors .
2. Enter a value in the Upload Reference field and click the FIND icon.
3. In Upload Record Line Number screen, click the Delete icon.
4. Click the Commit icon to delete upload errors.

This menu allows the user to delete the list of exception records created after the upload.

To amend or delete the uploaded registers, follow the below steps:

1. Delete All Uploaded registers .
2. Enter a value in the Upload Reference field and click the FIND button.
3. Select the list of uploaded registers to be deleted.
4. Click the Apply the chosen operation to the selected row(s) icon to delete the chosen records

This menu allows the user to delete the retrieved error records in the register after the upload.

To delete the retrieve Upload Error records, follow the below steps:

1. Delete Upload Error Register .
2. Enter a value in the Upload Reference field and click the FIND button.
3. Select the retrieve error records from the list.
4. Click the Apply the chosen operation to the selected row(s) icon to delete the chosen records.

This menu allows the user to amend the failed registers while updating the product type.

To rectify the failed register records, follow the below steps:

1. Rectify Product Update Errors .
2. Enter a value in the Upload Reference field and click the FIND button.
3. Click the Edit icon corresponding to a record to rectify the product update errros.
4. Click the Validate icon to check for errors.
5. Click the Commit icon to submit the record.

| SCREENS | WORKFLOW |
|---|---|
|  | Auto Batching/Change Product . |
| Mapping of upload reference to a Batch | Enter the upload reference value and select the action as Batch. Click the Commit icon. |
| Defining Batching conditions | The Bill Registers created out of the same upload reference can be batched by defining the conditions in BL.BATCH.CONDITIONS application. Enter the default mandatory conditions, such as, Currency, Liability, Customer and Product Type. Add the necessary conditions through the Decision fields. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

This menu displays the list of unauthorised auto-created registers in case zero authorisation version of EB.FILE.UPLOAD is not used in 'Upload Receivables' option.

To authorise an auto-created register, follow the below steps:

1. Authorise/Delete All Uploaded registers .
2. Enter a reference value in the Upload Reference field and click the FIND button.
3. Select the list of uploaded registers to be authorised.
4. Select the Authorise option and then click the Apply the chosen operation to the selected row(s) icon to authorise the chosen records.

To delete an auto-created register, follow the below steps:

1. Authorise/Delete All Uploaded registers .
2. Enter a reference value in the Upload Reference field and click the FIND button.
3. Select the list of uploaded registers to be deleted.
4. Select the Delete option and then click the Apply the chosen operation to the selected row(s) icon to delete the chosen records.


#### 📊 Outputs

After the Automatic Upload and Batching is complete, the user can view the below enquiries and reports.


##### Enquiries and Reports

This section helps the user to view the details of automatic batches, uploads and registers.

Auto Batch Details

This enquiry displays the details of BL.BATCH application records for a given upload reference number.

Auto Upload Details

This enquiry displays the statistical details of the uploaded invoices.

Auto Register Details

This enquiry displays the details of BL.REGISTER application records for a given upload reference number.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


### 1.2  Charges


> **📇 Quick Reference Card**
> 
> **Purpose:** *Banks charge for the services they provide to make a profit and pay operating expenses.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Banks charge for the services they provide to make a profit and pay operating expenses.


#### ⚙️ Configuration

Charges feature has no specific configuration to be setup. The parameter tables are setup at the implementation stage.


#### 📋 Tasks

There are no Tasks available for Charges feature.


#### 📊 Outputs

There are no Outputs available for Charges feature.

---


### 1.3  Disbursement and Settlement


> **📇 Quick Reference Card**
> 
> **Purpose:** *Disbursement is the act of paying out or disbursing money. It is a cash outflow.*
> 
> **Key Fields:** *BL Type*, *Bill Register*, *Currency*, *Customer*, *Drawer*, *Operation*, *Principal Amt*, *Waive Charge (Y/N)*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Disbursement is the act of paying out or disbursing money. It is a cash outflow.

Money paid for expenses, cash expenditures or dividend payments.


#### ⚙️ Configuration

Disbursement and settlement has no specific configuration to be setup. The parameter tables are setup at the implementation stage.


#### 📋 Tasks

Related topics:

- Batch Receivables Registers
- Perform Disbursement Under Batched Receivables
- Factoring and Forfaiting Processes

Disbursement and Settlement helps the users to enter, amend, reverse and delete the disbursed and settled records.


##### Workflow

This section helps the user to perform the below tasks:

| SCREENS | WORKFLOW |
|---|---|
|  | Input Disbursement-Register . |
| BL.BLR.DISBURSE | Enter values in the Drawer , BL Type , Currency fields and then click the FIND button. |
| Disbursement | Enter the disbursement amount. Click the Commit icon. The system authorises the records in the BL.REGISTER application through the fast path enquiry. Upon successful authorisation, a green flag is displayed adjacent to the respective record. |
| Registering the Disbursement | Click the Disbursement icon in the tool bar. The Disbursement screen launches and displays the values in the Customer , Currency , Principal Amt and Bill Register fields. Enter values in the other required fields. Click the Commit icon to submit the record. |

| SCREENS | WORKFLOW |
|---|---|
|  | Input Disbursement-Batch . |
| BL.BATCH.DISBURSE | Enter values in the Drawer , BL Type , Currency fields and click the FIND button. |
| Disbursement | Enter the disbursement amount. Click the Commit icon. The system authorises the records in the BL.REGISTER application through the fast path enquiry. Upon successful authorisation, a green flag is displayed adjacent to the respective record. |
| Batching the Disbursement | Click the Disbursement icon in the tool bar. The Disbursement screen launches and displays the values in the Customer , Currency , Principal Amt and Bill Register fields. Enter values in the other required fields. Click the Commit icon to submit the record. |

| SCREENS | WORKFLOW |
|---|---|
|  | Input Settlement . |
| BL.BLR.SETTLE | Enter values in the required fields and click the FIND button. |
| Settlement | Enter the amount to settle with settlement type and then click the Commit icon. The system authorises the records in the BL.REGISTER application through the fast path enquiry. Upon successful authorisation, a green flag is displayed adjacent to the respective record. |
| Registering the Disbursement | Click the Settlement icon in the tool bar. The Settlement screen launches and displays the values in the Customer , Currency , Principal Amt and Bill Register fields. Enter values in the other required fields. Click the Commit icon to submit the record. |

This menu allows the user to attach an individual Bill Register or Bill Batches to a Bill Contract.

1. Input Receivable Contract .
2. Enter values in the mandatory fields such as, Operation , Customer , Currency and Waive Charge (Y/N) .
3. Select a option from the Operation field.
4. Enter a value in the Bill Register field.
5. Click the Validate icon to check for errors.
6. Click the Commit icon to submit the record.

This menu allows the user to track the bill registers which are disbursed and not attach to a Bill Contract.

1. Unsuccessful Disbursement – Register .
2. The system displays the list of records by clicking the FIND button. The user can delete the disbursement by choosing and amending the Bill Registers from the list.
3. The system deletes the selected records through fast path enquiry by clicking the Commit icon to submit the record.

This menu allows the user to track the Bill Batches, which are disbursed and not attached to a Bill Contract.

1. Unsuccessful Disbursement – Batch .
2. The system displays the list of records by clicking the FIND button. The user can delete the disbursement by choosing and amending the Bill Registers from the list.
3. The system deletes the selected records through fast path enquiry by clicking the Commit icon to submit the record.

This menu allows the user to amend or reverse a Bill Contract.

To amend a Bill Contract, follow the below steps:

1. Amend/Reverse Receivable Contract .
2. In the Outstanding Receivable Contracts screen, click the Amend icon to amend an unauthorised receivable contract.
3. In the Amend Receivable Contract screen, enter or modify the values in the required fields.
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon to submit the record.

To reverse a Bill Contract, follow the below steps:

1. Amend/Reverse Receivable Contract .
2. In the Outstanding Receivable Contracts screen, click the Reverse icon to reverse an unauthorised receivable contract.
3. In the Bill Contract Input screen, click the Reverse icon to reverse the record.

This menu allows the user to delete an unauthorised disbursement contract.

To delete a Disbursement Contract, follow the below steps:

1. Delete Receivable Disbursement .
2. Click the Delete icon to delete the unauthorised disbursement contract from the list.
3. Click the Delete icon to delete the record.

This menu allows the user to delete an unauthorised settlement contract.

To delete a Settlement Contract, follow the below steps:

1. Delete Receivable Settlement .
2. Click the Delete icon to delete the unauthorised settlement contract from the list.
3. Click the Delete icon to delete the record.

This menu allows the user to delete an unauthorised Bill Contract.

To delete a Settlement Contract, follow the below steps:

1. Delete Receivable Contract .
2. In the Unauthorised Receivable Contracts screen, click the Delete icon to delete the unauthorised bill contract from the list.
3. In the Bill Contract Input screen, click the Delete icon to delete the record.

This menu displays the list of unauthorised Bill Contracts that can be authorised or deleted by the user.

To authorise a Receivable Contract perform the following steps:

1. Authorise/Delete Receivable Contract
2. Click the Authorise icon corresponding to a Bill Contract.
3. Click the Authorise icon to authorise the record.

To delete a Receivable Contract perform the following steps:

1. Authorise/Delete Receivable Contract
2. Click the Delete icon corresponding to a Bill Contract.
3. Click the Delete icon to delete the record.
4. Click the OK button in the message box that appears.

This menu displays the list of unauthorised Bill Disbursement records.

To authorise a Bill Disbursement, follow the below steps:

1. Authorise/Delete Disbursement .
2. In the Unauthorised Receivable Disbursement screen, click the Authorise icon corresponding to a record.
3. Verify the transaction details and then click the Authorise icon to commit the authorisation.

To delete a Bill Disbursement, follow the below steps:

1. Authorise/Delete Disbursement .
2. In the Unauthorised Receivable Disbursement screen, click the Delete icon corresponding to a record.
3. Click the Delete icon to commit the deletion.

This menu displays the list of unauthorised Bill Settlements.

To authorise a Bill Settlement, follow the below steps:

1. Authorise/Delete Settlement .
2. In the Unauthorised Receivable Settlement screen, click the Authorise icon corresponding to a record.
3. Verify the transaction details and then click the Authorise icon to commit the authorisation.

To delete a Bill Settlement, follow the below steps:

1. Authorise/Delete Settlement .
2. In the Unauthorised Receivable Settlement screen, click the Delete icon corresponding to a record.
3. Click the Delete icon to commit the deletion.


#### 📊 Outputs

This section helps the user to understand the various enquiries and reports in Disbursement and Settlement.


##### Enquiries and Reports

This topic helps the user to view the status of the disbursements, pending disbursements, overdue details, list of receivables and so on.

List of Discounted Receivables

This enquiry displays the list of discounted bills.

List of Receivables by Type

This enquiry displays the list of bill contracts based on the bill type.

List of Receivables maturing next 7 days

This enquiry displays the list of Bill Registers that matures in the next seven days. The user can view the Bill Register record by clicking the View icon.

Receivable Status

This enquiry displays the status of the Bill Registers. The user can view the Bill Register record by clicking the View icon.

Pending Disbursements

This enquiry displays the list of pending disbursements. The user can view the individual Bill Registers by clicking the View icon.

Enquiries Overdue Registers

This enquiry displays the list of unsettled Bill Registers beyond the due date.

Buyer Seller Limit Details

This enquiry displays the buyer and seller limit details.

View Receivable Advices/Messages

This enquiry displays List of Bill (BL) Delivery Messages and the drilldown gives the options to view the BL Delivery Messages for each record.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


### 1.4  Manual Upload and Batching


> **📇 Quick Reference Card**
> 
> **Purpose:** *Creation of a contract in Temenos Transact is called loading of bill. Bill contract involves three stages, such as*
> 
> **Applications:** `BL.REGISTER`
> 
> **Key Fields:** *Amount*, *Batching/Rebatching*, *Bill Type*, *CHANGE.PRODUCT*, *Charge Codes*, *Currency*, *Drawee*, *Drawer* ... +4 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Creation of a contract in Temenos Transact is called loading of bill. Bill contract involves three stages, such as

- BL.REGISTER (BR)
- BL.BATCH (BB) – Required for factoring or simple aggregation
- BL.BILL (BL)


#### ⚙️ Configuration

Manual upload and batching feature has no specific configuration to be setup. The parameter tables are setup at the implementation stage.


#### 📋 Tasks

Related topics:

- Process Settlement of Receivables
- Batch Receivables Registers
- Factoring and Forfaiting Processes

The Manual Upload and Batching helps the users to Register, Batch and Rebatch the receivables with authorisation.


##### Workflow

The user can register, authorise, delete the receivables using the below workflow:

This menu allows the user to register the details of a Bill.

To register the bill details, follow the below steps:

1. Register Receivables .
2. Enter the bill details such as, Drawer , Drawee , Start Date , End Date , Currency , Amount , Bill Type and Charge Codes .
3. Click the Validate icon to check for errors.
4. Click the Commit icon to submit the record.

This menu allows the user to change the product type of a Bill Register.

To change the product type, follow the below steps:

1. Change Product Type .
2. Select the list of registers to change the product type and enter a value in the New Bill Type field.
3. Click the Apply the chosen operation to the selected row(s) icon to change the product type.

This menu allows the user to amend or reverse a Bill Register.

To amend a Bill Register, follow the below steps:

1. Amend/Reverse Receivables .
2. In the Outstanding Receivables screen, click the Amend icon corresponding to a record.
3. Amend the required field values.
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon to submit the record.

To reverse a Bill Register, follow the below steps:

1. Amend/Reverse Receivables .
2. In the Outstanding Receivables screen, clcik the Reverse icon corresponding to a record.
3. Click the Reverse icon to reverse the record.

This menu allows the user to delete the unauthorised Bill Registers. The user can delete only if the registered bill is not attached to a Bill Batch or a Bill Contract.

To authorise or delete a Bill Register, follow the below steps:

1. Delete Receivables .
2. In the Unauthorised Receivable Register screen, select the Bill Registers to be deleted.
3. Click the Apply the chosen operation to the selected row(s) icon to delete an unauthorised Bill Register.

This menu allows the user to batch a group of bills entered using the Bill Register.

To batch the bill records, follow the below steps:

1. Receivable Batch .
2. Enter the Register Id to be batched.
3. Click the Validate icon to check for errors.
4. Click the Commit icon to submit the record.

This menu allows the user to amend or reverse a Bill Batch.

To amend a Bill Batch, follow the below steps:

1. Amend/Reverse Receivable .
2. In the Batched Receivables Records screen, click the Amend icon corresponding to a record to amend the field values as required.
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon to submit the record.

To reverse a Bill Batch, follow the below steps:

1. Amend/Reverse Receivable .
2. Click the Reverse icon to reverse a Bill Batch.
3. Click the Reverse icon to reverse the record.

This menu allows the user to delete the unauthorised Bill Batches. The user can delete a Bill Batch when it is not attached to a Bill Contract.

To delete a Bill Batch, follow the below steps:

1. Delete Receivables Batch .
2. In the Unauthorised Batch Contracts screen, click the Delete icon to delete an unauthorised Bill Batch.
3. In the Authorise/Delete Batch screen, click the Delete icon to delete the record.

This menu allows the user to batch the Bill Registers that are updated by new BL.TYPE based on the batching conditions defined in BL.BATCH.CONDITIONS application.

To rebatch a Bill Register, follow the below steps:

1. Rebatch .
2. Enter values in the SELLER.REFERENCE , CHANGE.PRODUCT fields.
3. Select the Rebatch option in the Batching/Rebatching field.
4. Click the Validate icon to check for errors.
5. Click the Commit icon to submit the record.
6. Run the BL.CREATE.BATCH service.

This menu displays the list of unauthorised Registered Receivables.

To authorise a registered receivable, follow the below steps:

1. Authorise/Delete Receivable Register .
2. In the Unauthorised Registered Receivables screen, click the Authorise icon corresponding to a record.
3. Verify the transaction details and then click the Authorise icon to commit the authorisation.

To delete a registered receivable, follow the below steps:

1. Authorise/Delete Receivable Register .
2. In the Unauthorised Registered Receivables screen, click the Delete icon corresponding to a record.
3. Click the Delete icon to commit the deletion.

This menu displays the list of unauthorised Receivable Batch contracts.

To authorise a Receivable Batch contract, follow the below steps:

1. Authorise/Delete Receivable Batch .
2. In the Unauthorised Batch Contracts screen, click the Authorise icon corresponding to a contract.
3. Verify the transaction details and then click the Authorise icon to commit the authorisation.

To delete a Receivables Batch contract, follow the below steps:

1. Authorise/Delete Receivable Batch .
2. In the Unauthorised Registered Receivables screen, click the Delete icon corresponding to a contract.
3. Click the Delete icon to commit the deletion.


#### 📊 Outputs

After the Manual Upload and Batching is complete, the user can view the below enquiries, advices and reports.


##### Enquiries and Reports

This section helps the user to view the details, such as, lodged receivables, advices for discounted bills, product update and upload summary.

List of Lodged Receivables

This enquiry displays the list of authorised Bill Registers. Using this enquiry, the user can view the Bill Register record by clicking the Receivable Register icon.

Receivables Lodged for Colln/Discounting

This enquiry displays the list of Bill Registers to be attached to a Bill Contract. Using this enquiry, the user can view the Bill Register record by clicking the Receivable Register icon.

List of Batched Receivables

This enquiry displays the list of Bill Batches.

Invoice Upload Summary

This enquiry displays the status of the invoice details based on the currency and amount category. The user can view the Invoice details only after the Invoice file is uploaded.

Update Product Summary

This enquiry displays the invoice details based on the currency and amount category after the product is update. The user has to enter the Upload Reference to view the enquiry details.

List of Receivables sent for Collection

This enquiry displays the details of List of Receivables sent for Collection and the drilldown provides the options to view the details of Receivables sent for Collection.

List of Collateralised Receivables

This enquiry displays the details of List of Collateralised Receivables and the drilldown provides the options to view the details of Collateralised Receivables.

List of Receivables with Suspended Int

This enquiry displays the details of List of Receivables with Suspended Interest and the drilldown provides the options to view the details of Receivables with Suspended Interest.


##### SWIFT Messages

NA


##### Advices

The below list of advices are generated by the core banking system pertaining to Manual Upload and Batching.

This enquiry displays the list of bill delivery messages. The user has to further drilldown to view the bill delivery messages.


##### Alerts

NA


> **Related Applications:** `BL.REGISTER`

---


### 1.5  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *Bills are receivables represented by invoices or bills of exchange. A business corporate (startups or SMEs or multinational corporates) can sell its bills to a Temenos Transact bank at a discount for a fee. The bank then collects the payments from the corporates customers, which is referred as facto...*
> 
> **Key Fields:** *Bill Type*, *Cat Ira*, *Category*, *Chg Discount Amt*, *Chg Maximum Amt*, *Chg Minimum Amt*, *Chg Premium Amt*, *Collateral* ... +17 more
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- Temenos Transact Services
- System Maintained Files
- Create Receivables Register
- Perform Disbursement Under Receivables

Bills are receivables represented by invoices or bills of exchange. A business corporate (startups or SMEs or multinational corporates) can sell its bills to a Temenos Transact bank at a discount for a fee. The bank then collects the payments from the corporates customers, which is referred as factoring or receivables financing.

The risk department in a bank may not approve financing of all bills. Such bills are sent for collection with the bank acting as an agent. Occasionally, banks consider accepting a bill as a collateral for extending a line of credit. A bank can extend their services to a corporate customer on the strength of bills. For example, factoring, collections and bill discounting.


##### Classifying Bills

The bill business from a bank's perspective are classified as follows:

The below are the various types of bills:

- Trade Bills are a consequence of trade finance business by a corporate that can further be classified into: Demand Bills – Payable on demand Usance Bills – Paid after a specified number of days (For example, the days count starts from the date of transport document)
- Direct Bills refer to a payment method where the seller sends the invoice directly to the buyer, bypassing intermediaries, and relying on mutual trust for payment upon receipt or within agreed terms.
- Clean Bills are bills of exchange presented for payment without any accompanying documents, relying solely on the buyer’s trust for payment.

After lodgment, the following operations can be performed on bills for a customer of a bank:

- Collecting invoice amount in part or full and crediting the operative account
- Discounting or purchase
- For factoring, individual bills are grouped together and collectively discounted or purchased
- Using bills as collateral to secure limits

Additionally, the bills module also supports:

- Retention of margin during advance disbursement
- Partial disbursement
- Partial or rebate type of settlement
- Cross currency disbursement or settlement


##### Configuring Factoring and Forfaiting

The individual bill types and their nomenclature differs from country to country. The parameters tables (also known as applications in Temenos Transact ) are the building blocks for designing the business process flow. It defaults common values to improve accuracy and efficiency.


###### Setting up Parameter Tables

The parameter tables in the bills module for transaction processing are listed below:

| Table Name | Short Name | Description |
|---|---|---|
| BL.PARAMETER | BP | Company level parameter |
| BL.TYPE | BT | Bill type definitions |
| BL.TXN.TYPE.CONDITION | BTTC | Bill types and transactions |
| APPL.GEN.CONDITION | AGC | Bill contract group definition |
| BL.GROUP.CONDITION | BGC | Defining customer or group conditions |

> **⚠️ Note:** Tables are configured in the above sequence, when setting up the parameters.

The explanation on each of the parameter files and its content is given below:

| Field | Description |
|---|---|
| Int Amort Freq | Determines the frequency for interest amortisation when a bill is discounted or purchased. Indicates he start period for amortisation. Accepts values, such as Daily, Monthly or Weekly. Updates dynamically when the Close of Business (COB) process is run in the system. |
| Days Post Maturity | Defines the number of days post maturity of the contract after which the records are moved to the history file. |
| Max Int Rate | The value mentioned in this field is used to check if the calculated effective rate of interest is within the permissible limits. The maximum interest rate should not exceed the rate specified in this field. When the effective rate comes below the rate mentioned in this field, an override message is generated. This is an optional field. |
| Minimum Interest Rate | The values specified in this field is used to check if the calculated effective rate of interest is within the the permissible limits. The minimum interest rate should not go below the rate specified in this field. When the effective rate goes below the rate mentioned in this field, an override message is generated. |
| Grace Days | Determines the number of days within which a bank’s customer has to settle a bill repayment. At the end of this period, a penalty is charged based on the outstanding debit balance on the bill account. |

| BL.TYPE | Description |
|---|---|
| 1 | Discounted bill with recourse |
| 2 | Discounted bill without recourse |
| 3 | Collection bills |
| 8 | Factoring transaction with recourse |
| 9 | Factoring transaction non-recourse |

| Field | Description |
|---|---|
| Grace Days | Determines the number for calculation of grace days. For example, 2C – 2 calendar days and 2W – 2 working days. This is an optional field. |
| Currency | Indicates the currency in which the charges are defined. The other associated fields are Interest Key , Interest Spread and Interest Rate . |
| Interest Rate | Determines the interest rate that is used at the transaction processing level. This is an optional field associated with Currency , Interest Key and Interest Spread . |
| Max Int Rate | Checks if the calculated effective rate of interest is within the permissible limits. When the interest rate is defined, the maximum interest rate should not breach the rate specified in this field. An override message is generated when the effective rate is breached. This is an optional field. |
| Minimum Interest Rate | Checks if the calculated effective rate of interest is within the permissible limits. When the interest rate is defined, the minimum interest rate should not breach the rate specified in this field. An override message is generated when the effective rate is breached. |

| Field | Description |
|---|---|
| Chg Maximum Amt | Defines the maximum amount charged for the applicable charge type. |
| Chg Minimum Amt | Defines the minimum amount charged for the applicable charge type. |
| Chg Discount Amt | Specifies the amount deducted from the charge amount calculated. |
| Chg Premium Amt | Specifies the amount added to the charge amount calculated. |

Allocates group codes, based on a number of defined conditions and/or local routines for any Temenos Transact application with a STANDARD.SELECTION .

A contract group is defined in this application, and created based on the category. For example, DISCBILL and COLLBILL is in the category range code from 30000 to 30001 and 30100 to 30120, respectively. The APPL.GEN.CONDITION requires a record with an ID of BL.BILL .

Defines the status of a process step in the life cycle of a bill. This status is entered at BILL.REGISTER or BL.BILL level. The status of a bill is monitored on a daily basis, when a report is generated from this application. Once the status is defined, the same is used in BL.REGISTER or BL.BATCH application.

The other setups done at the parameter level are:

This is a percentage of invoice or bill amount retained by the bank at the time of making advance disbursement to the seller. The value in the Retention Margin field defaults in BL.REGISTER when the Bill Type is attached, and the Retention Margin field is set to Allowed in the BL.TYPE application.

The system calculates and updates the maximum available amount for disbursement based on the retention margin. The retention margin is defined for:

- Product type in BL.TXN.TYPE.CONDITION
- Customer level in BL.GROUP.CONDITION
- Buyer in BL.BUYER.SELLER.LIMIT

The order in which the Retention Margin field is defaulted in BL.REGISTER are as follows:

1. BL.BUYER.SELLER.LIMIT
2. BL.GROUP.CONDITION – Customer specific
3. BL.GROUP.CONDITION – Group
4. BL.TXN.TYPE.CONDITION

The Cat Ira defines the profit and loss category code in BL.PARAMETER application to which the interest received in advance is posted. On authorisation, this field cannot be modified. However, the change in the existing profit and loss category can be specified in the New Cat Ira field. During COB, the category code is updated as the new category code. Henceforth, the new profit and loss category is used for reporting.

Similarly, the category of the bill in which it is reported is entered in the Category field of BL.TYPE application. On authorisation, this field cannot be modified. However, to change the existing category code the New Category field is used. At COB, the category code in this field is updated as the new category code Henceforth, all transactions are reported in this category code.

The E.UPLOAD.BL.REG.ERR.DTLS enquiry displays all the BL.REGISTER records in IHLD status, which can be amended or deleted.

The following setup is done in the system for the enquiry to display the error text and upload record line number.

The Log Level field in the record Temenos Transact .GENERIC.UPLOAD of EB.LOGGING.PARAMETER is set to Trace.

The Int Log File field in SPF is set to Yes.


##### Illustrating Model Parameters

Model parameters consists of the below tables:

| Table Name | Description |
|---|---|
| BILL.PARAMETER | This is a module level parameter file for bills. It is set before entering any bills contract along with the other parameter files. The disbursement, repayment and amortisation transaction code along with the interest rate caps, Profit and loss category for IRA Interest Received in Advance (IRA) are defined. The user can amend these pre-defined and fixed files. |
| BILL.TXN.TYPE.CONDITION | This parameter table defines the defaulting values for different combination of bill type and bill operation. ID of the table is DISCOUNT, COLLATERAL and COLLECTION, which are the supported bill operations. |
| APPLICATION.CONDITION ; | Contract groups are defined in this application based on category (product) code. This grouping is used to set default charge, commission and interest using the BILL.GROUP.CONDITION . The record ID to this table is BL.BILL to define bill groups. |
| BILL.GROUP.CONDITION | This parameter table is used to modify or override the values defaulted from a BL.TXN.TYPE.CONDITION record. Default charge, commission and interest can be defined for an individual customer or a group defined in APPL.GEN.CONDITION . |
| BILL.TYPE | Parameter settings for various types of bills (such as, discounted, collection), which are defaulted while entering a bill register record. It defines the contract category for various bill types and determines the liability customer in case of dishonour of a bill for each defined bill type. |
| BILL.STATUS | This application defines the status on the movement of bills. This status is given at bill register or bill batch level. |
| EB.DUPLICATE.TYPE | This application determines the duplicate records created in BL.REGISTER application. The system generates an override when the fields defined in the EB.DUPLICATE.TYPE and BL.REGISTER are same. |
| FILE.UPLOAD.TYPE | File upload type application allows the user to pre configure the upload directory, application and version details to process the header or item record in the uploaded file. This application displays all the records with value BILL.REGISTER in the Items Upd Appl field. |
| PRODUCT.CONDITIONS | BL.BATCH.CONDITIONS table defines the conditions for updating the product type in the BL registers based on the default conditions or customer specific conditions. Record ID format is . |
| CHANGE.PRODUCT.CONDITIONS | BL.BATCH.CONDITIONS table defines the conditions for updating the product type in the BL registers based on the default conditions or customer specific conditions. Record ID format is . |
| BATCH.CONDITIONS | This application defines the soft conditions for determining product types, batching and change product conditions for the bulk upload of invoices. |
| BUYER.SELLER. LIMIT | This application records the buyer-seller limit for information purpose. This holds buyer's maximum exposure for which the record is setup. |


##### Illustrating Model Products

Factoring and Forfaiting (FF) involves the sale of the receivables by the seller to meet their immediate cash needs. FF module supports the below products:

| Product Name | Features |
|---|---|
| Bills for collection | Collection bills that can neither be discounted (purchased) nor taken as collateral. The invoice or bill of exchange amount is credited to a customer’s account only after the credit is made to Nostro account. |
| Bills for discounting | Collection bill that is discounted (purchased) by the bank for value and the invoice or bill of exchange amount is credited to the customer even before it is realised This loan is extended to the customer (drawee) The loan is settled when the bill is realized or returned without payment |
| Bills for collateral | Bill collateral product is a trade bill that is taken as a collateral for establishing an account limit for lending. |
| Creation of bills contract | Lodging a bill in transact system Bill contract involves 3 steps |
| Manual upload and batching | Manual upload and batching provides the users with the options to register, batch and rebatch the receivables with authorisation. Creation of BILL.REGISTER Creation of BL.BATCH Creation of BL.BILL |
| Automatic upload and batching | Automatic upload and batching provides the users with the options to register, batch and rebatch the receivables with zero authorisation. |
| Disbursement and settlement | Disbursement and settlement provides the users with the options to input, amend, reverse and delete the disbursed and settled records. |

---


### 1.6  Product Type


> **📇 Quick Reference Card**
> 
> **Purpose:** *The type of the bill defined determines the operation selected for the product.*
> 
> **Key Fields:** *Info Liability*, *Liability Pty*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The type of the bill defined determines the operation selected for the product.


#### ⚙️ Configuration

When different products are defined in BL.TYPE , it is,

- Mandatory to specify the party whose liability limit needs to be updated.
- Optional to update the information limit of the party.

The Liability Pty and Info Liability are multi-value fields. The liability party can be established and tracked for a factoring transaction.


#### 📋 Tasks

There are no Tasks for Product Type.


#### 📊 Outputs

There are no outputs for Product Type.

---


### 1.7  Products


> **📇 Quick Reference Card**
> 
> **Purpose:** *The characteristics of a product helps to distinguish it from one another. Operations on a bill is classified as follows:*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The characteristics of a product helps to distinguish it from one another. Operations on a bill is classified as follows:

- Bills for collection
- Bills for discounting
- Bills as collateral


#### ⚙️ Configuration

Products feature has no specific configuration to be setup. The parameter tables are setup at the implementation stage.


#### 📋 Tasks

There are no Tasks available for Products feature.


#### 📊 Outputs

There are no Outputs available for Products feature.

---


---


## Chapter 2: Trade_Banking - LC


Trade_Banking - LC module of Temenos Transact


### Features in Trade_Banking - LC


| # | Feature | Sections |
|---|---------|----------|
| 2.1 | Amendment | Intro, Confi, Tasks, Outpu |
| 2.2 | Assignment of proceeds | Intro, Confi, Tasks, Outpu |
| 2.3 | Avalisation under Collection | Intro, Confi, Tasks, Outpu |
| 2.4 | Brokerage | Intro, Confi, Tasks, Outpu |
| 2.5 | Charges and Commission | Intro, Confi, Tasks, Outpu |
| 2.6 | Collection | Intro, Confi, Tasks, Outpu |
| 2.7 | Collection Amendment | Intro, Confi, Tasks, Outpu |
| 2.8 | Drawings | Intro, Confi, Tasks, Outpu |
| 2.9 | Islamic LoC | Intro, Confi, Worki, Tasks, Outpu |
| 2.10 | Issuance or Register of a LC | Intro, Confi, Tasks, Outpu |
| 2.11 | Managing External Requests | Intro, Confi, Tasks, Outpu |
| 2.12 | Margin or Provisions | Intro, Confi, Tasks, Outpu |
| 2.13 | Merchanting Trade | Intro, Confi, Worki, Tasks, Outpu |
| 2.14 | Misc | Intro |
| 2.15 | Open Account Trade | Intro, Confi, Worki, Tasks, Outpu |
| 2.16 | Post Shipment Finance | Intro, Confi, Tasks, Outpu |
| 2.17 | Pre-shipment Finance | Intro, Confi, Tasks, Outpu |
| 2.18 | Pre advice of a LC | Intro, Tasks, Outpu |
| 2.19 | Reversal or Cancellation | Intro, Confi, Tasks, Outpu |
| 2.20 | RMA Verification | Intro, Confi, Tasks, Outpu |
| 2.21 | Shipping Guarantee | Intro, Confi, Tasks, Outpu |
| 2.22 | Shipping Guarantee against Import Collection | Intro, Confi, Tasks, Outpu |
| 2.23 | Syndicated Letter of Credit | Intro, Confi, Tasks, Outpu |
| 2.24 | TBML Check for Letter of Credit | Intro, Confi, Worki, Tasks, Outpu |
| 2.25 | Tickler and Tracers | Intro, Confi, Tasks, Outpu |
| 2.26 | Trade Based Lending | Intro, Confi, Worki, Tasks, Outpu |
| 2.27 | Trade Evidence For Advance Payment | Intro, Confi, Worki, Tasks, Outpu |


### 2.1  Amendment


> **📇 Quick Reference Card**
> 
> **Purpose:** *The amendment of a Letter of Credit (LC) allows the user to insert changes, which generates an amendment to the original terms and conditions of an LC. In an irrevocable LC, as the contract is binding on the issuing bank, amendments are effected only with the concurrence or at the request of the ben...*
> 
> **Key Fields:** *Amendment No*, *External Ref*, *Send Message?.1*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The amendment of a Letter of Credit (LC) allows the user to insert changes, which generates an amendment to the original terms and conditions of an LC. In an irrevocable LC, as the contract is binding on the issuing bank, amendments are effected only with the concurrence or at the request of the beneficiary and applicant.

These amendments are effected by quoting the suitable references (correspondence details). Amendment advices are delivered to the beneficiary through the advising bank.

The system auto generates the following:

- All relevant accounting entries for commissions
- Increase or decrease of the principal amounts
- Advices and documents to the electronic delivery system related to amendments


##### SWIFT 2023 Changes for MT707

As a part of SWIFT R 2023 changes, the length of the below mentioned tags is increased from 65x to 140z for MT707.

| Tag | Field Name |
|---|---|
| 44A | Place of Taking in Charge/Dispatch from .../Place of Receipt |
| 44E | Port of Loading/Airport of Departure |
| 44F | Port of Discharge/Airport of Destination |
| 44B | Place of Final Destination/For Transportation to.../Place of Delivery |


#### ⚙️ Configuration

Amendment has no specific configuration to be setup. The parameter tables are setup at the implementation stage.


#### 📋 Tasks

Related topics:

- Issue Import LC
- Amend Import LC
- Trade Finance and Guarantees Processes
- Corporate Amend Import LC

An amendment to a Letter of Credit (LC) signifies any change made to the terms of an LC after it has been authorised. Amendment can be made at any time after the LC authorisation and before expiry date.


##### Workflow

The user can amend, import and export LCs by using the below workflow:

This section allows the user to perform the below activities:

This menu allows the user to amend the issued Import LC for any internal requirement which is not communicated to third parties nor generate an advice of amendment.

To amend an Internal Amendment, follow the below steps:

1. Internal Amendment .
2. In the Import LC screen, click Amend icon corresponding to a record.
3. In the Internal Amendment Import LC screen, enter values in the mandatory fields and amend the required changes in the corresponding fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.

This menu allows the user to amend the issued Import LC.

To process an External Amendment, follow the below steps:

1. External Amendment .
2. In the Import LCs screen, click Amend icon corresponding to a record.
3. In the External Amendment Import LC screen, enter values in the mandatory fields and amend the required changes in the corresponding fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to issue an Amendment Seeking Beneficiary’s Consent.

To process an Amendment Seeking Beneficiary’s Consent, follow the below steps:

1. Amendment Seeking Benef’s Consent .
2. In the Import LCs screen, click Amend icon corresponding to a record.
3. In the Import LC Amendment (Ben Consent sought) screen, enter values in the mandatory fields and amend the required changes in the respective fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to record the beneficiary’s consent (amendment seeking the beneficiary’s consent) on the amendment of an import LC.

To approve the amendment of an import LC, follow the below steps:

1. Approve/Reject Amendment of Import LC .
2. In the List of Amended Import LCs screen, click the Approve/Reject icon corresponding to a record.
3. In the Approve/Reject Amendment (Import LC) screen, enter a value in the Amendment No field.
4. Select the Approved button to approve the amendment by which the system raises accounting entries and limit updates, if any.
5. Click the Validate icon to check for the errors and overrides.
6. Click the Delivery Preview icon to view the delivery messages
7. Click the Commit icon to submit the record.

To reject the amendment of an import LC, follow the below steps:

1. Approve/Reject Amendment of Import LC .
2. In the List of Amended Import LCs screen, click the Approve/Reject icon corresponding to a record.
3. In the Approve/Reject Amendment (Import LC) screen, enter a value in the Amendment No field.
4. Select the Rejected button to reject the amendment and there is no change made to the LC record.
5. Click the Validate icon to check for the errors and overrides.
6. Click the Delivery Preview icon to view the delivery messages.
7. Click the Commit icon to submit the record.

This menu lists the LC amendment records, which are under the bank user queue for processing.

To amend an LC that are in Pending with Bank, follow the below steps:

1. Pending with Bank .
2. In the Amendment Request Pending With Bank screen, click the Modify Request icon to amend a record.
3. Click the Validate icon to check for the errors and overrides
4. Click the Commit icon to submit the record.

To view the records that are in Pending with Bank, follow the below steps:

1. Pending with Bank .
2. In the Amendment Request Pending with Bank screen, click the View Full Details icon to view a record.

To amend an LC that are in Pending with Customer, follow the below steps:

1. Pending with Customer .
2. In the Amendment Request Pending with Customer screen, click the Modify Request icon to amend a record.
3. Click the Validate icon to check for the errors and overrides
4. Click the Commit icon to submit the record.

To view the records that are in Pending with Customer, follow the below steps:

1. Pending with Customer .
2. In the Amendment Request Pending with Bank screen, click the View Full Details icon to view a record.

This menu allows the user to authorise or delete the import LC amendments.

To authorise the import LC amendments, follow the below steps:

1. Import LCs/Amendments .
2. In the Unauthorised Import LCs screen, click the Authorise icon to authorise a transaction.
3. In the Import LCs screen, verify the transaction details and then click the Authorise icon to commit the authorisation.

To delete the import LC amendments, follow the below steps:

1. Import LCs/Amendments .
2. In the Unauthorised Import LCs screen, click the Delete icon to delete a transaction.
3. In the Import LCs screen, verify the transaction details and then click the Delete icon to commit the deletion.

This section allows the user to perform the below activities:

This menu lists the inward letter of credits amendment messages that are created from the incoming SWIFT messages and are on On hold status by Temenos Transact .

To process the inward amendment SWIFT messages, follow the below steps:

1. Bene Consent Amendment’s .
2. In the List of Export LC Amendments on Hold screen, click the Modify icon corresponding to a record.
3. In the Export LC Amendment screen, enter values in the mandatory fields based on the message types.
4. Click the Validate icon to check for the errors overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to do a simple correction to an export LC, such as, amending liability reversal date, limit reference and so on. These corrections are neither communicated to third parties nor generates an advice of amendment.

To make an internal amendment of a LC, follow the below steps:

1. Internal Amendment .
2. In the Export LCs screen, click the Amend icon corresponding to a record.
3. In the Internal Amendment of Export LC screen, enter a value in the External Ref field and do the necessary internal corrections.
4. Click the Messages tab and select the No option in the Send Message?.1 field.
5. Click the Validate icon to check for errors and overrides.
6. Click the Delivery preview icon to ensure that there is no delivery messages are generated and then click the Commit icon.

This menu allows the user to amend the registered Export LC.

To process an external amendment, follow the below steps:

1. External Amendment .
2. In the Export LCs screen, click the Amend icon corresponding to a record to proceed with the transaction.
3. In the External Amendment of Export LC screen, enter values in the mandatory fields and amend values in the required fields.
4. Click the Validate icon to check for errors and overrides.
5. Click the Delivery Preview icon to preview the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to record the beneficiary’s consent (amendment seeking the beneficiary’s consent) on the amendment of an export LC.

To approve the amendment of an export LC, follow the below steps:

1. Approve/Reject Amendment of Export LC .
2. In the List of Amended Export LCs screen, click the Approve/Reject icon corresponding to a record.
3. In the Accept/Reject Amendment (Export LC) screen, enter a value in the Amendment No field.
4. Select the Approved button to approve the amendment by which the system raises accounting entries and limit updates, if any.
5. Click the Validate icon to check for the errors and overrides.
6. Click the Delivery preview icon to view the delivery messages.
7. Click the Commit icon to submit the record.

To reject the amendment of an export LC, follow the below steps:

1. Approve/Reject Amendment of Export LC .
2. In the List of Amended Export LCs screen, click the Approve/Reject icon corresponding to a record.
3. In the Accept/Reject Amendment (Export LC) screen, enter a value in the Amendment No field.
4. Select the Rejected button to reject the amendment and there is no change made to the LC record.
5. Click the Validate icon to check for the errors and overrides.
6. Click the Delivery preview icon to view the delivery messages.
7. Click the Commit icon to submit the record.

This menu allows the user to process Beneficiary’s Consent for which beneficiary consent received.

To process an Amendment Seeking Beneficiary’s Consent, follow the below steps:

1. Amendment Seeking Benef’s Consent .
2. In the Export LCs screen, click the Amend icon for corresponding record to proceed with the transaction.
3. In the Export LC Amendment (Ben Consent sought) screen, enter values in the mandatory and other required field.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.

This menu allows the user to authorise or delete the export LC amendments.

To authorise the export LC amendments, follow the below steps:

1. Export LCs/Amendments .
2. In the Unauthorised Export LCs screen, click the Authorise icon to authorise a transaction.
3. In the Export Negotiation LCs screen, verify the transaction details and then click the Authorise icon to commit the authorisation.

To delete the export LC amendments, follow the below steps:

1. Export LCs/Amendments .
2. In the Unauthorised Export LCs screen, click the Delete icon to delete a transaction.
3. In the Export Negotiation LCs screen, verify the transaction details and then click the Delete icon to commit the deletion.

This menu allows the user to authorise or delete the LC amendments which require the beneficiary consent.

To authorise the LC amendments which require bene’s consent, follow the below steps:

1. Bene Consent Amendments .
2. In the Unauthorised LC Amendments screen, click the Authorise icon to authorise a transaction.
3. In the LC Amendment (Ben Consent sought) screen, verify the transaction details and click the Authorise icon to commit the authorisation.

To delete the LC amendments which require bene’s consent, follow the below steps:

1. Bene Consent Amendments .
2. In the Unauthorised LC Amendments screen, click the Delete icon to delete a transaction.
3. In the LC Amendment (Ben Consent sought) screen, verify the transaction details and click the Delete icon to commit the deletion.


#### 📊 Outputs

The user can view the below swift messages, enquiries and reports while processing the LC amendments.


##### Enquiries and Reports

This section helps the user to view the approved and rejected LC amendments, which are initiated from Temenos Connect Internet Banking.

Accepted

This enquiry displays the details of the approved amendment requests which are initiated from Temenos Connect Internet Banking.

Accepted

This enquiry displays the details of the rejected amendment requests which are initiated from Temenos Connect Internet Banking.


##### SWIFT Messages

This section helps the user to view the below listed SWIFT Messages.

This message is sent to the collecting bank while making an amendment to an outward documentary collection.

This message is sent by the issuing bank to the advising bank and generates while making an external amendment to an import LC.

This message is sent by the LC issuing bank to the reimbursing bank and generates while making an external amendments to an import LC, if the original LC includes a reimbursement authority.


##### Advices

NA


##### Alerts

NA

---


### 2.2  Assignment of proceeds


> **📇 Quick Reference Card**
> 
> **Purpose:** *Assignment of proceeds is an instruction (which is irrevocable) given by the beneficiary of a documentary credit or standby letter of credit authorising the payment (all or part of the proceeds due to it) to a third party. As stated in Uniform Customs and Practice for Documentary Credits (UCP 600) A...*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Assignment of proceeds is an instruction (which is irrevocable) given by the beneficiary of a documentary credit or standby letter of credit authorising the payment (all or part of the proceeds due to it) to a third party. As stated in Uniform Customs and Practice for Documentary Credits (UCP 600) Article 39, proceeds can only be assigned and does not provide the assignee the right to perform the credit.

In UCP 600, only limited information is given on how a notice of assignment needs to be handled.

> **⚠️ Note:** An assignment of proceeds is subject to the provisions of the applicable law. This law can be for assignor and the bank that is being asked to accept, acknowledge, and act on the instructions.

An assignment of proceeds can occur in a number of circumstances, such as when a beneficiary of a documentary credit is:

- Not the supplier of (some or all) the goods being shipped but funds are to be paid to the supplier and cannot be transferred or appropriate for the supplier.
- Unable to pay for the freight cost to a carrier or owner (for example, charter party transactions) in advance, and assigns part of the proceeds to cover those costs.


#### ⚙️ Configuration

There are no specific configuration to be setup at feature level. The parameter tables are setup at the implementation stage.


#### 📋 Tasks

There are no Tasks available for Assignment of Proceeds feature.


#### 📊 Outputs

There are no Outputs available for Assignment of Proceeds feature.

---


### 2.3  Avalisation under Collection


> **📇 Quick Reference Card**
> 
> **Purpose:** *Exporters can require a third party (bank), to guarantee payment of a Bill of Exchange (BOE) drawn on an importer under a trade contract. This action, known as avalisation, is provided by a bank on behalf of the exporter on request. The bank commits itself unconditionally to pay if the drawee defaul...*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Exporters can require a third party (bank), to guarantee payment of a Bill of Exchange (BOE) drawn on an importer under a trade contract. This action, known as avalisation, is provided by a bank on behalf of the exporter on request. The bank commits itself unconditionally to pay if the drawee defaults, by endorsing the bill on the back.

An avalised bill substitutes the bank's risk for the importers risk thus providing the exporter with assurance that payment will be met. This bill is subsequently discounted or negotiated for better credit terms, thus enhancing the trade relationship with the importer.

Hence, avalisation is an endorsement on a BOE or draft by a bank, which guarantees payment if the drawee (importer) defaults payment of the bill at maturity.


#### ⚙️ Configuration

Avalisation has no specific configuration to be set up at feature level. The parameter tables are set up at the implementation stage.


#### 📋 Tasks

Related topics:

- Accept Import Collection
- Lending Processes (Corporate)

Exporters can require a third party (bank) to guarantee payment of a Bill of Exchange (BOE) drawn on an importer under a trade contract. This action is known as avalisation, is provided by a bank on behalf of the exporter on request. The bank commits itself unconditionally to pay if the drawee defaults, by endorsing the bill on the back.

An avalised bill substitutes the bank's risk for the importers risk thus providing the exporter with assurance that payment is met. This bill is subsequently discounted or negotiated for better credit terms, thus enhancing the trade relationship with the importer.

Hence, avalisation is an endorsement on a BOE or draft by a bank, which guarantees payment if the drawee (importer) defaults payment of the bill at maturity.


##### Workflow

The user can perform Avalisation related tasks using the below workflow:

This menu allows the user to accept or avalise the Inward Collections.

To accept or avalise an Inward Collection, follow the below steps:

1. Acceptance/Avalisation of Inward Collection .
2. In the Unaccepted Inward Collection screen, click the Record the Due Date icon to proceed with the transaction.
3. In the Acceptance of Inward Collection (Tenor) screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to initiate a payment of accepted and avalised collection.

To Initiate a payment of accepted or avalised collection, follow the below steps:

1. Initiate Payment of Accepted/Avalised Collection .
2. In the List of Accepted Inward Collections screen, click the Initiate Settlement icon to proceed with the transaction.
3. In the Initiated Settlement of Inward Collns screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to settle the accepted and avalised collection.

To settle the accepted or avalised collection, follow the below steps:

1. Settle Accepted/Avalised Collection .
2. In the Settlement Initiated Inward Collections screen, click the Online Settlement icon to proceed with the transaction.
3. In the Settlement of Inward Collections screen, enter values in the required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to purchase the outward avalised collections.

To purchase an outward avalised collection, follow the below steps:

1. Purchase of Avalised Collection .
2. Click the Discount icon to discount a record.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to amend an already discounted collection bill.

To amend an already discounted collection bill, follow the below steps:

1. Amendment to Avalised Collection Purchased .
2. Click the Discounting icon to amend a record.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to initiate a payment of accepted or avalised collection.

To initiate a payment of accepted or avalised collection, follow the below steps:

1. Initiate Payment of Accepted/Avalised Collection .
2. In the List of Accepted Inward Collections screen, click the Initiate Settlement icon corresponding to a record to proceed with the transaction.
3. In the Initiated Settlement of Inward Collns screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to preview the delivery messages.
6. Click the Commit icon to submit the record.

To view the accepted or avalised collection, follow the below steps:

1. Initiate Payment of Accepted/Avalised Collection .
2. In the List of Accepted Inward Collections screen, click the View icon corresponding to a record to view the record.

This menu allows the user to purchase the outward avalised collections.

To purchase an avalised collection, follow the below steps:

1. Purchase of Avalised Collection .
2. In the Avalised Collections pending for Payment screen, click the Discount icon corresponding to a record to discount a record.
3. In the Discount of Outward Avalized Collection screen, enter the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to preview the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to amend an already discounted collection bill.

To amend an already discounted collection bill, follow the below steps:

1. Amendment to Avalised Collection Purchased .
2. In the List of Avalised Discounted Bills under Exp LC screen, click the Discounting icon corresponding to a record to proceed with the transaction.
3. In the Amendment to Usance Bills Discounted screen, enter values in required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to preview the delivery messages.
6. Click the Commit icon to submit the record.

To view already discounted collection bill, follow the below steps:

1. Amendment to Avalised Collection Purchased .
2. In the List of Accepted Inward Collections screen, click the View icon corresponding to a record to view the record.


#### 📊 Outputs

There are no Outputs available for Avalisation under Collection feature.

---


### 2.4  Brokerage


> **📇 Quick Reference Card**
> 
> **Purpose:** *An agent is a broker or middleman between importer and exporter. They obtain their fee or commission from the drawing amount (percentage or flat amount).*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

An agent is a broker or middleman between importer and exporter. They obtain their fee or commission from the drawing amount (percentage or flat amount).


#### ⚙️ Configuration

Brokerage should be a valid entry in the BROKER table. Brokerage has no specific configuration to be setup. The parameter tables are setup at the implementation stage.


#### 📋 Tasks

There are no Tasks available for Brokerage feature.


#### 📊 Outputs

There are no Outputs available for Brokerage feature.

---


### 2.5  Charges and Commission


> **📇 Quick Reference Card**
> 
> **Purpose:** *Trade finance transactions can be issued in any currency as specified in the LC Currency field in the LETTER.OF.CREDIT application. By default, the commission is calculated in LC currency. However, if a valid CSN currency is specified in the CSN Currency field available in the CURRENCY application (...*
> 
> **Key Fields:** *CSN Currency*, *Charge Code*, *Charge Currency*, *Charge Routine*, *Charge Settled   From*, *Charge Status*, *Currency*, *LC Currency* ... +2 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Trade finance transactions can be issued in any currency as specified in the LC Currency field in the LETTER.OF.CREDIT application. By default, the commission is calculated in LC currency. However, if a valid CSN currency is specified in the CSN Currency field available in the CURRENCY application (this field accepts value from the same record as LC currency or the equivalent local base currency as specified from the COMPANY application), the commission is calculated and credited to the Profit and Loss (P&L) of this currency instead of the transaction currency. Amortisation and accruals for commission are calculated accordingly. Commission can be debited from an account of any currency. The conversion happens accordingly and positional entries are raised upon conversion.

Charges when defined are accepted in equivalent currency as specified in the Charge Currency field. If the applicable charges that are defined for respective Charge Code field in the FT.COMMISSION.TYPE table and the same codes are specified in the Charge Code field in LETTER.OF.CREDIT , then the charges are calculated or defaulted for the corresponding currency specified in the Currency field in FT.COMMISSION.TYPE as the LC currency. The charges are then converted into equivalent currency specified in the Charge Currency field. Completed drawings and charges collected can be denominated in another currency different from LC currency. Charges can be collected immediately or later.


#### ⚙️ Configuration

A list of charge codes are created in the FT.CHARGE.TYPE and/or FT.COMMISSION.TYPE applications to activate the charges functionality. These configuration tables has the details of each type of charge or commission. (To know more on configuration and usage, and charges and commission, refer to SYSTEM and FT.COMMISSION.TYPE tables, respectively). The types of charges or commission are defined in FT.COMMISSION.TYPE application. LC.TXN.TYPE.CONDITION table is used to define default charges for trade finance products.

The bank can guarantee a minimum commission receipt irrespective of the percentages set and transaction value. The Overall Min Amt and Overall Max Amt fields are used to set the minimum and maximum commission to be collected, respectively. Charges and commissions can be accrued or amortised over a period by defining it in the FT.COMMISSION.TYPE . There is no standard rule or order for defaulting settlement accounts in LC application. If account numbers are entered for opener, beneficiary and advising bank, they are defaulted while collecting charges. They are also defaulted in DRAWINGS application.

If payment method is indicated as Nostro in DRAWINGS , the payment account is defaulted by using NOSTRO.ACCOUNT for the payment currency. Transaction codes defined in LC.PARAMETERS are used in STMT.ENTRY Default List (STMT.ENTRY) and CATEG.ENTRY Default List (CATEG.ENTRY) enquiries for narrating underlying transactions affecting accounts and PL heads. Profit and Loss (P and L) category code related fields are defined in LC.PARAMETERS .


##### Periodic Commission

The user defines the period based banded structure of commission rates in the following steps:

1. Define FT.COMMISSION.TYPE records for amount band (for each period). Ensure not to define maximum and/or minimum amounts.
2. Define the period bands in PERIODIC.COMMISSION table (new table) attaching the FT.COMMISSION.TYPE record IDs for the respective bands.
3. Create another FT.COMMISSION.TYPE record with the same ID of PERIODIC.COMMISSION . Attach transaction codes, category, minimum and maximum commission amount, and tax code.
4. Define the routine as @PERIODIC.COMMISSION in the Charge Routine field.


#### 📋 Tasks

Related topics:

- Pre-Advise Import LC
- Define Fees and Commissions Parameters
- Core Parameter Maintenance Processes

The trade finance application allows the user to set up charges at the time of Letter of Credit (LC) issuance or advising, at any time afterwards, or at the time of LC payment or negotiation.


##### Workflow

The user can perform the following tasks:

| SCREENS | WORKFLOW |
|---|---|
|  | Direct Charge Collection . |
| LC Charges | Enter value for any one of the selection criteria and click the FIND button. |
| LC Charges | Click the View LC Record icon corresponding to the record. Click the Delivery Preview icon to view the delivery messages. |

| SCREENS | WORKFLOW |
|---|---|
|  | Settle/Writeoff Claimed Charges . |
| LCs with Chgs Claimed/Debited to CRF | Enter a value in any one of the selection criteria and click the FIND button. |
| LCs Charges Claimed but not Received | Click the Settle Claimed Charge icon corresponding to the record. |
| Settlement of Claimed Charges | Enter values in the Charge Status and Charge Settled From fields. Click the Validate icon to check for errors and overrides. Click the Delivery Preview icon to view the delivery messages. Click the Commit icon to submit the record. |


#### 📊 Outputs

The trade finance application allows the user to set up charges at the time of Letter of Credit (LC) issuance or advising, at any time afterwards, or at the time of LC payment or negotiation.


##### Enquiries and Reports

NA


##### Swift Messages

NA


##### Advices

Users can view the following Advices:

The below advice is generated, when the user performs drawings under export LC.

After releasing the margin for an import LC, the user can view the below delivery message.

The below delivery message ia generates, when the user amend or opens an import letter of credit.

The below delivery message is generated, when the user opens an import letter of credit.

The below delivery message is generated, when the user performs the import letter of credit drawings.

The below delivery message is generated, when the user collects the charges under drawings in import letter of credit.

The below delivery message is generated, when the user performs the acceptance of inward collections.

The below delivery message is generated, when the user performs drawings under import letter of credit.


##### Alerts

NA

---


### 2.6  Collection


> **📇 Quick Reference Card**
> 
> **Purpose:** *As stated in article 2 of Uniform Rules for Collection (URC) 522, collection means the handling of documents by banks, in order to;*
> 
> **Key Fields:** *Clean Colln Type*, *Document Amount*, *Document Currency*, *Drawee ID*, *Drawer ID or Drawer Name & Address*, *End Range.1.*, *Expiry/Reversal Date*, *Remitting Bank ID or Remitting Bank Name and Drawee ID (Our Customer)* ... +2 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

As stated in article 2 of Uniform Rules for Collection (URC) 522, collection means the handling of documents by banks, in order to;

- Obtain payment and/or acceptance, or
- Deliver documents against payment and/or acceptance, or
- Deliver documents on other terms and conditions.

The liability of the banks are restricted to forwarding and releasing documents against payment or acceptance. When there are major discrepancies in a Letter of Credit (LC), the bank may choose to send it for collection without any risk or responsibility on its part. The four parties involved in a documentary collection are:

| Party | Role |
|---|---|
| Principal/remitter/seller/drawer | Hands over the documents to his bank with a collection order |
| Remitting bank | Seller’s bank |
| Collecting/presenting/issuing bank | Takes care of the actual collection by presenting to the buyer the documents as per terms of collection |
| Drawee/buyer/beneficiary/importer | To whom the collection documents are presented |


#### ⚙️ Configuration

LC.TYPES application predefines all types of collections.

- This application is used to set the type of collection and the way Temenos Transact treats the transaction through its various phases (opening, drawing and maturity).
- It defines and describes the collection types required in the system, and also used to setup the default category code for each type.
- The characteristics of each LC and collection type are recorded in this application.


#### 📋 Tasks

Related topics:

- Register Export Collection
- Amend Import Collection
- Trade Finance and Guarantees Processes
- Corporate Accept Import Collection
- Corporate Settle Exp Collection
- Corporate Register Import Collection
- Corporate Reg Export Collection
- Corporate Amend Exp Collection

A documentary collection is a process by which an exporter’s bank collects funds from the importer’s bank in exchange for documents detailing shipped merchandise.

Inward Collection

Inward Collection is a mode of payment for foreign trade in which the commercial documents are released to the buyer through their bank, against payment or acceptance of bill of exchange.

Outward Collection

The outward collection is initiated by the drawer. The drawer ships the goods to the drawee and submits the supporting documents to the remitting bank under collection. The remitting bank lodges the collection received from the drawer in the system, generates a collection schedule and forwards the documents to the collecting bank.


##### Workflow

The user can amend the outward collections using the below workflow:

The user can amend the inward collections and take or reduce margin using the below workflow:

This enquiry explains,

This menu allows the user to view the queries that are pending with the bank user and the customer.

To send an enquiry or accept, follow the below steps:

1. Pending with Bank .
2. In the List Of Inward Collections Pending With Bank screen, click the Query/Accept icon corresponding to a record.
3. In the Internet Pending Inward Collections screen, enter values in the required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.

To settle the transaction, follow the below steps:

1. Pending with Bank .
2. In the List Of Inward Collections Pending With Bank screen, click the Settle icon corresponding to a record.
3. In the Payment Of Inward Collections screen, enter values in the required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.

To amend the inward collections pending with IB customer:

1. Pending with IB Customer .
2. In the List Of Inward Collections pending with Customer screen, click the Amend icon corresponding to a record.
3. In the Internet Pending Inward Collections screen, enter values in the required fields.
4. Click the Validate icon to check for the errors and overrides
5. Click the Commit icon to submit the record.

This menu allows the user to take or reduce the margins for inward collections.

To take or reduce the margin for an inward collection, follow the below steps:

1. Take/Reduce Margin .
2. In the Take/Reduce Margin under Inward Collections screen, click the Take/Release Margin icon to take or reduce the margin for a transaction.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to authorise or delete the direct collection, inward collection amendment and outward collection amendment.

This menu allows the user to authorise or delete the pending inward collection amendment records.

To authorise the inward collection amendments, follow the below steps:

1. Inward Colln/Amendments .
2. In the Unauthorised Inward Collections screen, click the Authorise icon to authorise a transaction.
3. In the Inward Colln Doc Details screen, click the Authorise icon further to commit the authorisation.

To delete the inward collection amendments, follow the below steps:

1. Inward Colln/Amendments .
2. In the Unauthorised Inward Collections screen, click the Delete icon to delete a transaction.
3. In the Inward Colln Doc Details screen, click the Delete icon further to commit the deletion.

This menu allows the user to authorise or delete the pending outward collection amendment records.

To authorise or delete the outward collection amendments, follow the below steps:

1. Outward Colln/Amendments .
2. In the Unauthorised Outward Collections screen, click the Authorise icon to authorise a transaction.
3. In the Amend Outward Collection screen, click the Authorise icon further to commit the authorisation.

To delete the outward collection amendments, follow the below steps:

1. Outward Colln/Amendments .
2. In the Unauthorised Outward Collections screen, click the Delete icon to delete a transaction.
3. In the Amend Outward Collection screen, click the Delete icon further to commit the deletion.

This menu allows the user to authorise or delete the direct collection records.

To authorise the direct collections, follow the below steps:

1. Direct Colln Allotment .
2. In the List Of Unauthorised Direct Collection screen, click the Authorise icon corresponding to a record to authorise a transaction. .
3. Click the Authorise icon further to commit the authorisation.

To delete the direct collections, follow the below steps:

1. Direct Colln Allotment .
2. In the List Of Unauthorised Direct Collection screen, click the Delete icon corresponding to a record to delete a transaction.
3. Click the Delete icon further to commit the deletion.

This menu allows the user to register a Sight Documentary Collection.

To register a Sight Documentary Collection, follow the below steps:

1. Lodge Sight Docy Collection .
2. Enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to register a Usance Documentary Collection.

To register a Usance Documentary Collection, follow the below steps:

1. Lodge Usance(Tenor) Documentary Collection .
2. Enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to close the Inward collections which are to be returned to remitting bank due to unpaid reason.

To close an inward collection, follow the below steps:

1. Closure of Inward Collection .
2. In the Inward Collections available for closure screen, click the Closure icon corresponding to a record.
3. In the Closure of Inward Docy Collection screen, enter values in the required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to register a clean inward collection on presentation of draft by the remitting bank.

To register a clean inward collection, perform the below task:

1. Lodge Clean Collection .
2. In the Clean Collections screen, enter values in the mandatory and other required fields: Clean Colln Type Document Currency Document Amount Expiry/Reversal Date Remitting Bank Ref Drawer ID or Drawer Name & Address Remitting Bank ID or Remitting Bank Name and Drawee ID (Our Customer)
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the SWIFT messages.
5. Click the Commit icon to submit the record.

The user can lodge and amend the outward collections using the below workflow:

This menu allows the user to register the outward clean collection on presentation of financial documents by the drawer.

To register the outward clean collection, follow the below steps:

1. Lodge Clean Collections .
2. Enter values in the mandatory fields and in the Drawee ID field.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the swift messages.
5. Click the Commit icon to submit the record.

This enquiry displays the inward MT4XX series messages that are auto-processed and placed under the respective outward collections menu. The user can access the record for further processing and also to view the received inward messages.

To access and view the inward messages, follow the below steps:

1. Messages Processed .
2. In the Messages Processed under Inward SWIFT Messages screen, click the View icon to view the received inward messages.

To access and view the inward messages, follow the below steps

1. Messages Processed .
2. In the Processing of Outward Collection Swift Messages screen, click the Edit icon to process the inward messages.
3. In the Payment of Outward Collection screen, click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to send and receive the queries from Temenos Connect Internet Banking customer. Initiation of outward collection from Temenos Connect Internet Banking, once approved by Temenos Connect Internet Banking manager is available for further processing in the Pending with Bank tab.

To send a query or action, follow the below steps:

1. Pending with Bank .
2. In the List Of Outward Collections Pending With Bank screen, click the Query/Action icon corresponding to a record.
3. In the Internet Pending Outward Collections screen, enter values in the required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.

To view the transaction, follow the below steps:

1. Internet Pending Outward Collections .
2. In the List Of Outward Collections Pending With Bank screen, click the View icon corresponding to a record.

To view the transaction, follow the below steps:

1. Pending With IB Customer .
2. In the List Of Outward Collections pending with Customer screen, click the View icon corresponding to a record.

To do an action to the transaction, follow the below steps:

1. Pending With IB Customer .
2. In the List Of Outward Collections pending with Customer screen, click the Action icon corresponding to a record.
3. In the Internet Pending Inward Collections screen, enter values in the required fields.
4. Click Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.

This menu allows the user to register the acknowledgement received for outward collections.

To view the MT410 message, follow the below steps:

1. Messages Processed .
2. In Processing of Outward Collection Swift Messages screen, click the View icon corresponding to a MT410 message.

To process the MT410 message, follow the below steps:

1. Messages Processed .
2. In Processing of Outward Collection Swift Messages screen, click the Edit icon corresponding to a MT410 message.
3. In Payment of Outward Collection screen, enter values in the required fields.
4. Click Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.

This menu allows the user to give a series of pre-allotted reference numbers or pre-printed collection schedules to the seller or exporter or customer for sending directly to the buyers.

The Temenos Transact reference number is known only when the user enters the transaction details. While lodging the outward collection, the user must give the allotted direct collection reference number used by the customer.

To define the direct collection range for customers, follow the below steps:

1. Define Direct Collection Range for Customers .
2. In Direct Collection Allotment screen, enter the customer no to set the range of reference numbers.
3. Enter values in the below fields: Start Range.1 End Range.1.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to authorise the inward SWIFT messages.

This menu explains,

This menu allows the user to authorise the unauthorised inward SWIFT messages that are related to LCs.

1. Unauthorised Inward LC’s .
2. In the List of Unauthorised Export LCs screen, click the Authorise icon corresponding to a record.
3. Click the Authorise icon further to commit the authorisation.

This menu allows the user to authorise the unauthorised inward amendment SWIFT messages that are of bene’s consents.

1. Unauthorised Bene Consents Amendments .
2. In the List of Unauthorised Export LC Amendments screen, click the Authorise icon corresponding to a record.
3. Click the Authorise icon further to commit the authorisation

This menu explains,

This menu allows the user to authorise or delete the inward SWIFT messages that are related to inward collections.

To authorise the Inward Collections SWIFT messages:

1. Authorise/Delete Inward Collections .
2. In the unauthorised inward Collection Swift Messages screen, click Authorise icon corresponding to a record.
3. In the Amend Inward Docy Collection screen, check for the required field values.
4. Click the Authorise icon further to commit the authorisation.

To delete the Inward Collections SWIFT messages:

1. Authorise/Delete Inward Collections .
2. In the unauthorised inward Collection Swift Messages screen, click Delete icon corresponding to a record.
3. Click the Delete icon further to commit the deletion.

This menu explains,

This menu allows the user to view the inward SWIFT messages that are related to trade finance.

To view the SWIFT messages:

1. Inward Trade Swift Messages .
2. In the Inward Trade Finance Swift Messages screen, click the View Swift Message icon corresponding to a record.

To view a contract:

1. Inward Trade Swift Messages .
2. In the Inward Trade Finance Swift Messages screen, click the View Contract icon corresponding to a record.

This menu allows the user to view and process the inward SWIFT repaired messages.

To view the SWIFT messages in repaired queue:

1. Processing Of Repaired Messages .
2. In the Inward Trade Finance Swift Messages screen, click the View Swift Messages icon corresponding to a record.

To send MT799 or MT499 for an inward SWIFT message :

1. Processing Of Repaired Messages .
2. In the Inward Trade Finance Swift Messages screen, click the Send MT799/MT499 icon corresponding to a record.
3. In the Free Format Message screen, enter values in the required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to preview the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to register a Sight Document received from Drawer.

To register a Sight Documentary Collection, follow the below steps:

1. Lodge Sight Docy Collection .
2. In the Outward Docy Collection(Sight) screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to register a Usance Document received from Drawer.

To register a Usance Documentary Collection, follow the below steps:

1. Lodge Usance(Tenor) Documentary Collection .
2. In the Outward Docy Collection (Tenor) screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to purchase an outward collection.

To purchase outward collection, follow the below steps:

1. Purchase of Collection .
2. In the List of Collection pending for Purchase/Discount screen, click the Discount icon to proceed with the transaction.
3. In the Purchase/Discount of Outward Collection screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to do the Payment for an Outward Collection.

To initiate a payment for outward collection, follow the below steps:

1. Payment of Outward Collection .
2. In the Outward Collection pending for Payment screen, click Record the Due Date icon to proceed with the transaction.
3. In the Payment of Outward Collection screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to send tracer to unpaid Outward Collection.

Follow the below steps to send Tracer:

1. Trace the Collection .
2. In the List of outward Collections screen, click Trace icon to proceed with the transaction.
3. In the Purchase/Discount of Outward Collection screen, enter values in the required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to accept an outward collection.

To accept an outward collection, follow the below steps:

1. Acceptance of Outward Collection .
2. In the Outward Tenor Collection pending for Acceptance screen, click Accept icon to proceed with the transaction.
3. In the Acceptance of Outward Collection (Tenor) screen, enter values in the mandatory and required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to perform the payment for an inward collection.

To process a payment of inward collection, follow the below steps:

1. Payment of Inward Collection .
2. In the Inward Collections pending for Payment screen, click the Payment icon corresponding to a record to proceed with the transaction.
3. In the Payment of Inward Collection screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to preview the delivery messages.
6. Click the Commit icon to submit the record

This menu allows the user to view and pay the accepted outward collections.

To view the accepted outward collections, follow the below steps:

1. Online Maturity of Accepted Collections .
2. In the List of Accepted Collections - Export LC screen, click the View icon corresponding to a record to view the accepted outward collections.

To take action on the accepted collections, follow the below steps:

1. Online Maturity of Accepted Collections .
2. In the List of Accepted Collections - Export LC screen, click the MAT icon corresponding to a record to proceed with the transactions.
3. In the Online Maturity of Accepted Collection screen, enter the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to preview the delivery messages.
6. Click the Commit icon to submit the record.


#### 📊 Outputs

A documentary collection is a process by which an exporter’s bank collects funds from the importer’s bank in exchange for documents detailing shipped merchandise.

The user can view the below swift messages, enquiries and reports while processing and after processing the inward collections.


##### Enquiries and Reports

This section allows the user to view the below enquiries and reports:

This section helps the user to view the details of outstanding inward collections, overdue inward collections, inward collections that are of pending responses, etc.

Lodged Documents

This enquiry displays the list of import LC bills received under collection that are yet to be paid or accepted or rejected.

Import LCs with FX Cover

This enquiry displays the list of import LCs that are covered by the FX contract.

Clean Collection Outstanding

This enquiry displays the list of inward clean collections outstanding that are yet to be paid. Users can view the collection record by clicking the View Record icon.

Collections Avalised

This enquiry displays the list of inward collection avalised bill.

Collections Overdue

This enquiry displays the list of all unpaid inward collections that crossed the due date.

Collections Pending Response

This enquiry displays the list of all inward collections that are awaiting response from internet banking customers, beyond the days specified in LC.PARAMETERS application along with the number of exceeding days.

Collections Outstanding

This enquiry displays the details of the outstanding inward documentary collections. Users can view the collection record by clicking the View Record icon.

Collection Released Under Trust

This enquiry displays the outstanding inward documentary collections for which the related documents have been released under Trust. Users can view the collection record by clicking the View Record icon.

This section helps the user to view the details of outstanding outward collections, list of export bills that are sent for collections, outward discounted collections, and so on.

Bills sent for Collection

This enquiry displays the details of export LCs that are expired but the liability of them are yet to be reversed in the bank’s books.

Bills Paid Under Reserve

This enquiry list the details of export bills paid under reserve that are outstanding in the books of the bank. Users can view the drawing record by clicking the View Record icon.

Export LCs with FX Cover

This enquiry displays the list of export LCs that are covered by FX contract.

Bills Negotiated

This enquiry displays the list of all outstanding bills negotiated or discounted under export LC. Users can view the drawing record by clicking the View Drawing icon.

LC Expired

This enquiry displays the list of outstanding export LCs. Users can further drill down to the LC from this enquiry.

Usance Bills Due

This enquiry displays the list of usance bills under export LC that are due for settlement.

Clean Collections Outstanding

This enquiry displays the list of outstanding outward clean collections. Users can view the drawing record by clicking the View Record icon.

Discounted Outward Collection

This enquiry displays the list of outward discounted collections.

Doc Collections Outstanding

This enquiry displays the list of outward documentary collections outstanding. Users can view the drawing record by clicking the View Record icon.

Rejected Internet Requests

This enquiry lists all the rejected Temenos Connect Internet Banking initiated outward collection requests,


##### SWIFT Messages

This section allows the user to view the below SWIFT Messages:

Below are the list of SWIFT Messages:

This message generates as an acknowledgement while registering an inward collection document.

This message generates as an acceptance while making an acceptance of inward collection.

This message is sent by the collecting bank to the remitting bank to advice non-payment or non-acceptance against individual collection bill or part thereof.

This message is used to advise the receiver about the status of collection documents received by the collecting bank.

This message is sent by the issuing bank to the paying or negotiating or accepting bank to advise the receiver that the documents received with discrepancies have been taken up.

This message is used to advise the receiver bank that the documents received are not in accordance with the terms and conditions of the credit. It generated while rejecting the documents under import LCs or export LCs.

This message is sent by the issuing bank from which it has received documents. It is used to advise the receiver about reimbursement or payment for a drawing under a documentary credit.


##### Advices

The below list of advices are generated by the core banking system pertaining to Collections.

Below are the list of advices:

The below delivery messages generates when the user accepts the collection document.

The below delivery message generates when the user acknowledges the collection document.

The below advice generates and sent to the presenting bank when the user accepts the collection document.

The below message generates when the user collects the charges on collection document.

This advice is sent to drawee to inform about the documents received for collection.

Below are the list of advices:

This advice is sent to the collecting bank with the details of the documents sent for collection.

This advice is sent to drawee as an acknowledgement after sending the documents for collection.


##### Alerts

NA

---


### 2.7  Collection Amendment


> **📇 Quick Reference Card**
> 
> **Purpose:** *Collection remittance contains instructions for the collecting bank. These can modified by the remitting bank or case of need. The field 74 of MT430 list some instructions, but principal can give new instructions regarding the collection. For example, amendments such as, extension of maturity, accep...*
> 
> **Key Fields:** *Description*, *Short Description*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Collection remittance contains instructions for the collecting bank. These can modified by the remitting bank or case of need. The field 74 of MT430 list some instructions, but principal can give new instructions regarding the collection. For example, amendments such as, extension of maturity, acceptance of partial payment, waiver of charges, or to protest against non-acceptance or non-payment.


#### ⚙️ Configuration

There is no specific configuration for collection amendment. The parameter tables are setup at the implementation stage.


#### 📋 Tasks

Related topics:

- Accept Import Collection
- Amend Import Collection
- Trade Finance and Guarantees Processes

A documentary collection is a process by which an exporter’s bank collects funds from the importer’s bank in exchange for documents detailing shipped merchandise.

Inward Collection

Inward Collection is a mode of payment for foreign trade in which the commercial documents are released to the buyer through their bank, against payment or acceptance of bill of exchange.

Outward Collection

The outward collection is initiated by the drawer. The drawer ships the goods to the drawee and submits the supporting documents to the remitting bank under collection. The remitting bank lodges the collection received from the drawer in the system, generates a collection schedule and forwards the documents to the collecting bank.


##### Workflow

The user can amend the outward collections using the below workflow:

This menu allows the user to amend the outward collections.

To amend an outward collection, follow the below steps:

1. Amend/Upload (Docs) Outward Collection .
2. In the List of outward Collections screen, click Amend icon corresponding to a record.
3. In the Amend Outward Collection screen, enter values in the required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to perform changes to the inward collections, if any.

To amend an inward collection, follow the below steps:

1. Amendment of Inward/Avalised Collection .
2. In the List Of Inward Collection screen, click the Amend icon to amend a transaction.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

To amend an inward collection, follow the below steps:

1. Amendment of Inward/Avalised Collection .
2. In the List Of Inward Collection screen, click the Upload icon to upload a document to a transaction.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to amend a sight collection that are already purchased or discounted.

To amend a purchased collection, follow the below steps:

1. Amendment to Collection Purchased .
2. Click the Discounting icon to amend a record.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to perform changes and upload document to the inward collections.

To amend an inward or avalised collection, follow the below steps:

1. Amendment of Inward/Avalised Collection .
2. In the List of Inward Collections screen, click the Amend icon to amend a transaction.
3. In the Amend Inward Docy Collection screen, amend values in the required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to preview the delivery messages.
6. Click the Commit icon to submit the record.

To upload a document for an inward or avalised collection, follow the below steps:

1. Amendment of Inward/Avalised Collection .
2. In the List of Inward Collections screen, click the Upload icon to upload the documents.
3. In the Document Capture screen, enter values in the below mandatory fields and then click the Commit icon: Short Description Description
4. In the IM Image Upload screen, click the Choose File button from the Upload Image field.
5. Browse and select the required document and then click the Open button.
6. Click the Validate icon to check for the errors and overrides.
7. Click the Commit icon to submit the record.

This menu allows the user to perform changes and upload document to the Outward collections:

To amend an outward collection, follow the below steps:

1. Amend/Upload(Docs) Outward Collection .
2. In the List of Outward Collections screen, click the Amend icon to amend a transaction.
3. In the Amend Outward Collection screen, amend values in the required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to preview the delivery messages.
6. Click the Commit icon to submit the record.

To upload a document for an inward collection, follow the below steps:

1. Amend/Upload(Docs) Outward Collection .
2. In the List of Outward Collections screen, click the Upload icon to upload the documents.
3. In the Document Capture screen, enter values in the below mandatory fields and then click the Commit icon: Short Description Description
4. In the IM Image Upload screen, click the Choose File button from the Upload Image field.
5. Browse and select the required document and then click the Open button.
6. Click the Validate icon to check for the errors and overrides.
7. Click the Commit icon to submit the record.


#### 📊 Outputs

After the collection and amendment process, the user can view the below advices.


##### Enquiries and Reports

NA


##### SWIFT Messages

NA


##### Advices

The below list of advices are generated by the core banking system pertaining Collection Amendments:

This advice is sent to Letter Of Credit (LC) issuing bank with the export documents under the letter of credit for payment by collecting or negotiating bank.

This advice is sent to the remitting bank as an acknowledgement to the collection documents.

This advice is sent to drawee as a confirmation for amendment of outward collection document.

This advice is sent to the collecting bank to enquire the status of the collection documents.


##### Alerts

NA

---


### 2.8  Drawings


> **📇 Quick Reference Card**
> 
> **Purpose:** *The beneficiary can draw under the Letter of Credit (LC) by presenting a draft and copies of invoices. The issuing bank is obligated to make the payment if the documents presented comply with the terms of the LC.*
> 
> **Key Fields:** *Authority Amount*, *Authority Currency*, *Bill Paid UnderReserve Returned Unpaid*, *Claim amount*, *Discrepancies.1*, *Discrepancy Type*, *Disposal of Docs*, *Doc Amount* ... +19 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The beneficiary can draw under the Letter of Credit (LC) by presenting a draft and copies of invoices. The issuing bank is obligated to make the payment if the documents presented comply with the terms of the LC.


#### ⚙️ Configuration

This feature has no specific configuration to be setup. The parameter applications are setup at the implementation stage.


#### 📋 Tasks

Related topics:

- Amend Import LC
- Register Documents Against Export LC (Sight or Mixed)
- Trade Finance and Guarantees Processes

DRAWINGS application in Temenos Transact has the flexible payment and reimbursement mechanism, whereby funds are collected or paid through a number of intermediaries. The funds are also paid to third parties or agents who are not involved in the Letter Of Credit (LC).


##### Workflow

The user can draw down the export and import LCs by using the below workflow:

| SCREENS | WORKFLOW |
|---|---|
|  | Register/Upload Documents . |
| Import LC Doc Registration/Upload | Enter the transaction reference number in the search criteria and then click the FIND button. |
| Import LC's Pending Document Registration/Upload | Click the Register/Upload icon to register and upload a document. |
| Drawings for Document Upload | Click the Upload icon further to upload a document. |
| Details of Document Upload | Enter or select values in the required fields. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

This section allows the user to perform the below activities:

This menu allows the user to record the document details before the receipt of the negotiated documents and after the receipt of the payment from the issuing bank.

The user records the document details on the basis of a SWIFT confirmation from the negotiating bank stating that the documents negotiated are in strict compliance of the LC terms.

To record the document details after SWIFT confirmation, follow the below steps:

1. Amendment to Paid Drawings .
2. In the Paid Drawings for Amendment screen, click the Amendment icon of a paid drawing.
3. In the Documents Received after Payment screen, select a value from the Document Code.1 field.
4. Click the Validate icon to check for errors and overrides.
5. Click the Delivery Preview (opens in new window) icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to amend or edit a mixed type of drawings under an import LC.

To amend or edit a mixed type of drawing, follow the below steps:

1. Drawings Under Mixed Payment .
2. In the Import LC's pending for Payment & Acceptances under Mixed Drawings screen, click the Accept icon to amend or edit a record.
3. In the Drawings under Mixed Payment Import LC screen, enter or modify the required field values.
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon.

This menu allows the user to amend or settle a mixed payment by online.

To amend a mixed payment by online, follow the below steps:

1. Amendment/Online Settlement of Mixed Payments .
2. In the Manual Maturity of Acceptance under Mixed Drawing screen, click the Amend Mixed Drawings icon to amend the values of a record.
3. In the Amendment on Mixed Drawings screen, enter or modify the values in the required fields.
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon.

To settle a mixed payment by online, follow the below steps:

1. Amendment/Online Settlement of Mixed Payments .
2. In the Manual Maturity of Acceptance under Mixed Drawing screen, click the Online Maturity icon to proceed with the transaction.
3. In the Online Maturity of Mixed Payment Drawings (Imports) screen, verify the field values.
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon.

This menu allows the user to amend:

- Discounted usance drawing
- Extension of maturity date or early maturity or online maturity and so on

To amend a discounted usance drawing, follow the below steps:

1. Amendment to Usance Discounting .
2. In the Discounted Import Usance Bills screen, click the Amendment icon.
3. In the Amendment to Usance Bills Discounted screen, enter a value in the New Maturity Date field.
4. Click the Delivery preview (opens in new window) icon to view the delivery messages.
5. Click the Validate icon to check for errors and overrides.
6. Click the Commit icon.

This menu allows the user to amend a discounted mixed type of drawings.

To amend a discounted mixed type of drawings, follow the below steps:

1. Amendment for Mixed Payment Discounting .
2. In the Discounted Mixed Payment Bills(Import) screen, click the Amendment icon to amend a record.
3. In the Amendment to Mixed Payment Discounting screen, enter values in the required fields.
4. Click the Delivery preview (opens in new window) icon to view the delivery messages.
5. Click the Validate icon to check for errors and overrides.
6. Click the Commit icon.

This menu allows the user to edit a mixed type of drawings under an Export LC.

To edit a mixed type of drawings, follow the below steps:

1. Drawings Under Mixed Payment .
2. In the Export LC's pending for Payment & Acceptances under Mixed Drawings screen, click the Accept icon corresponding to a record.
3. In the Drawings Under Mixed Payment (Exports) screen, enter values in the mandatory and other required fields.
4. Click the Delivery preview (opens in new window) icon to view the delivery messages.
5. Click the Validate icon to check for errors and overrides.ny.
6. Click the Commit icon.

This menu allows the user to register the pending export LC documents and to amend the registered export LC documents.

To amend the captured or registered documents, follow the below steps:

1. Capture/Check Documents .
2. In the List of Registered/Captured Drawings screen, click the Amend icon corresponding to a record.
3. In the Capture/Check documents screen, amend the field values as required.
4. Click the Delivery preview (opens in new window) icon to view the delivery messages.
5. Click the Validate icon to check for the errors and overrides.
6. Click the Commit icon to submit the record.

This menu allows the user to amend and settle the mixed payment values by online.

To amend the mixed payment values by online, follow the below steps:

1. Amendment/Online Settlement of Mixed Payments .
2. In the Manual Maturity of Acceptance under Mixed Drawing (Exports) screen, click the Amend icon to amend a record.
3. In the Amendment to Mixed Drawings screen, enter or modify the required field values.
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon.

To settle the mixed payment values by online, follow the below steps:

1. Amendment/Online Settlement of Mixed Payments .
2. In the Manual Maturity of Acceptance under Mixed Drawing (Exports) screen, click the Online Maturity icon for a record to settle the mixed payment by online.
3. In the Online Maturity of Mixed Payment Drawings(Exports) screen, verify the field values.
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon.

This section allows the user to perform the below activities:

This menu allows the user to perform operations pertaining to internet banking customer.

To send the queries to the customer, follow the below steps:

1. Pending with Bank .
2. Click the Queries to Customer icon to send the queries to the customer.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Commit icon.

To view the queries that are pending with customer, follow the below steps:

1. Pending with IB Customer .
2. Click the Edit icon to edit the drawings in case of long pending queries.

This menu allow the user to discount the import usance bills, where the issuing bank makes payment to beneficiary or negotiating bank before the maturity of the bill and later recovers the payment amount from the applicant on the accepted maturity date.

1. Discounting of Usance Bills (Imports) .
2. In the Accepted Documents Under Import LC screen, click Discounting icon corresponding to a record.
3. In the Discounting of Usance Bills (Import LC) screen, change the Drawing Type field values as ‘Ma’ (Matured Acceptance) and enter values in the required fields.
4. Click the Delivery preview (opens in new window) icon to view the delivery messages.
5. Click the Validate icon to check for errors and overrides.
6. Click the Commit icon to submit the record.

This menu allows the user to create a loan for import payments.

To create a loan for import payment, follow the below steps:

1. Create Loan for Import Payment .
2. Enter the drawing reference number in the TF Drawing Ref field.
3. Enter values in the mandatory fields, such as, Loan Maturity Date and Interest Rate (Fixed).1 .
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon.

This menu allows the user to discount an accepted mixed payment.

To discount an accepted mixed payment, follow the below steps:

1. Discounting for Mixed Payments(Imports) .
2. In the Documents pending for discounting screen, click the Accept icon to accept a record.
3. In the Discounting for Mixed Drawings screen, verify the record details.
4. Click the Delivery preview (opens in new window) icon to view the delivery messages.
5. Click the Validate icon to check for errors and overrides.
6. Click the Commit icon.

This menu displays the list of unauthorised drawings, where the supervisor can authorise or delete the drawings.

To authorise a drawing, follow the below steps:

1. Drawings .
2. In the Unauthorised Drawings screen, click the Authorise icon from the list of unauthorised drawings.
3. In the Accept Documents (Import LC) screen, click the Authorise icon to authorise the drawings.

To delete a drawing, follow the below steps:

1. Drawings .
2. In the Unauthorised Drawings screen, click the Delete icon from the list of unauthorised drawings.
3. In the Accept Documents (Import LC) screen, click the Delete icon to delete the drawings.

This menu allows the user to perform operations pertaining to internet banking customer.

To send the queries that are pending with Bank, follow the below steps:

1. Pending with Bank .
2. Click the Queries to Customer icon to send the queries to the customer.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Commit icon to submit the record.

To edit the queries that are pending with customer, follow the below steps:

1. Pending with IB Customer .
2. Click the Queries to Customer icon to send the queries to the customer.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Commit icon to submit the record.

This menu allow the user to make a payment for accepted drawings on any day, on or before the specified maturity date and amend the accepted drawings.

To accept the online matured contracts, follow the blow steps:

1. Online Maturity of Acceptance .
2. In the Accepted Documents Under Export LC screen, click the Online Maturity icon to proceed with the transaction
3. In the online Maturity of Acceptance(Export) screen, enter values in the required fields, if any.
4. Click the Validate icon to check for errors and overrides.
5. Click the Delivery Preview icon to preview the delivery messages.
6. Click the Commit icon to submit the record.

To amend the accepted drawings, follow the blow steps:

1. Online Maturity of Acceptance .
2. In the Accepted Documents Under Export LC screen, click the Amend Accepted Drawings icon to amend the accepted drawings.
3. In Amendment on Accepted Drawings screen, amend values in the required fields.
4. Click the Validate icon to check for errors and overrides.
5. Click the Delivery Preview icon to preview the delivery messages.
6. Click the Commit icon to submit the record.

| SCREENS | WORKFLOW |
|---|---|
|  | Bill (Paid Under Reserve) Returned Unpaid . |
| Contract Screen | Select a value in the Bill Paid UnderReserve Returned Unpaid field and then click the Edit icon. |
| Bill Paid UnderReserve Returned Unpaid | Enter values in the mandatory and other required fields. Click the Delivery preview (opens in new window) icon to view the delivery messages. Click the Validate icon to check for the errors and overrides. Click the Commit icon to submit the record. |

This section allows the user to perform the below activities:

This tab allows the user to record the reimbursement authorisation received from the issuing bank by SWIFT MT740.

To create a new authority, follow the below steps:

1. Input Authority .
2. In the Input and Modify Unauthorised Authorities screen, click the New Authority icon to enter a new authority for a record.
3. In the Reimbursement Authority screen, enter values in the below mandatory fields based on the MT740 SWIFT message: Documentary Credit No Issuing Bank id Authority Currency Authority Amount
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon.

To amend an existing authority, follow the below steps:

1. Input Authority .
2. In the Input and Modify Unauthorised Authorities screen, click the Modify icon to modify the existing authority from the list.
3. In the Reimbursement Authority screen, enter or modify the required field values.
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon.

This tab allows the user to record the amendments received (MT747) from the issuing bank for the existing reimbursement authorisation.

To record the amendments on reimbursement authorisation, follow the below steps:

1. Amend Authority .
2. In the List of Reimbursement Authorities tab, click the Amend icon of a record.
3. In the Reimbursement Amendment screen, enter the amendment field values by referring to MT740 SWIFT message.
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon.

This tab allows the user to register a reimbursement claim for which the user not holding a reimbursement authority. Therefore, a dummy authority is created to follow up with the issuing bank.

To register a claim with the dummy authority, follow the below steps:

1. Awaiting Authority .
2. In the Authorities created without MT740 based on Claim screen, click the Results Toolbar icon and select New Task from the drop-down at the foremost in position to register a dummy reimbursement authority.
3. In the Reimbursement Authority screen, enter values in the below mandatory fields: Documentary Credit No Issuing Bank id Authority Currency Authority Amount
4. Click the View Record icon to view the existing authority from the list.
5. Click the Authority Recd icon to edit the existing authority.
6. Click the Register Claim icon to register a reimbursement claim.
7. Click the Validate icon to check for errors and overrides.
8. Click the Commit icon.

This tab allows the user to register a reimbursement claim received from the claiming bank through SWIFT MT742.

To register a claim received from the claiming bank, follow the below steps:

1. Register Claims .
2. In the Register Reimbursement Claims tab, click the Register Claim icon to register a claim for a record.
3. In the Register Reimbursement Claim screen, verify the record details.
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon.

This tab allows the user to modify, cancel, reject the claims before authorisation.

To modify an existing claim, follow the below steps:

1. Modify/Cancel/Reject Claims .
2. In the List of Claims to be Modified screen, click the Modify icon to modify an existing claim.
3. In the Register Reimbursement Claim screen, enter or modify the required field values.
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon.

To cancel or reject a claim, follow the below steps:

1. Modify/Cancel/Reject Claims .
2. In the List of Claims to be Modified screen, click the Cancel/Reject icon to cancel or reject the claim.
3. In the Reject Claims under Export LC screen, verify the field values, if required.
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon.

To send the MT799 message, follow the below steps:

1. Modify/Cancel/Reject Claims .
2. In the List of Claims to be Modified screen, click the Send MT799 icon to send the MT799 message.
3. In the Free Format Messages MT799 screen, enter values in the required fields.
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon.

This tab allows the user to send a notice to the claiming bank on non-confirming the reimbursement claim.

To send a notice to the claiming bank on non-confirming a claim, follow the below steps:

1. Register Claims .
2. In the Register Reimbursement Claims screen, click the Register Claim icon to register a claim for a record.
3. In the Register Reimbursement Claim screen, click the MT744 tab.
4. Enter a value in the Claim amount field and other required field values.
5. Click the Delivery preview icon to view the MT744 message.
6. Click the Validate icon to check for errors and overrides.
7. Click the Commit icon.

This tab displays the list of unauthorised records that are created through inward messages and consists of the following sub-tabs:

This tab displays the list of unauthorised records of LETTER.OF.CREDIT application that are created through the MT740 inward messages.

To amend and view the inward messages, follow the below steps.

1. Inward Authority .
2. Click the Modify icon to enter or modify the values in the required fields.
3. Click the View Inward Message icon to view the messages.
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon.

This tab displays the list of records with the status as either created or not created based on the inward messages MT747 in the LC.AMENDMENTS application.

1. Inward Authority Amendment .
2. Click the Modify icon to enter or modify the values in required fields.
3. Click the View Inward Message icon to view the messages.
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon.

This tab displays the list of records with the status as either created or not created based on the inward messages MT742 in the DRAWINGS application.

1. Inward Claims .
2. Click the Process the Message icon to process the inward messages.
3. Click the View Inward Message icon to view the messages.
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon.

This tab displays the list of inward messages with the status 'Record not created'. These messages are not mapped with the respective applications due to the error messages.

1. Click the View SWIFT Message icon to view the inward messages.
2. Click the Send MT799/MT499 icon to send the SWIFT messages for clarification.
3. Click the Validate icon to check for errors and overrides.
4. Click the Commit icon.

This menu allows the supervisor to:

- Authorise or amend the reimbursement authority
- Authorise claims
- View the summary of the LC

This menu consists of the following tabs:

This tab is used to authorise an unauthorised reimbursement authority record.

To authorise an unauthorised reimbursement authority record, follow the below steps:

1. Authorise Reimbursement Authority .
2. In the Unauthorised Reimbursement Authorities screen, click the Authorise icon from the list of reimbursement authority records.
3. In the Reimbursement Authority screen, click the Authorise icon to authorise an unauthorised reimbursement authority record.

To delete an unauthorised reimbursement authority record, follow the below steps:

1. Authorise Reimbursement Authority .
2. In the Unauthorised Reimbursement Authorities screen, click the Delete icon from the list of reimbursement authority records.
3. In the Reimbursement Authority screen, click the Delete icon to delete an unauthorised reimbursement authority record.

This tab is used to authorise an unauthorised reimbursement amendment authority record.

To authorise an unauthorised reimbursement amendment authority record, follow the below steps:

1. Authorise Authority Amendment .
2. In the Unauthorised LC Amendments screen, click the Authorise icon from the list of unauthorised reimbursement amendment authority records.
3. In the LC Amendment(Ben Consent sought) screen, click the Authorise icon to authorise an unauthorised reimbursement amendment authority record.

To delete an unauthorised reimbursement amendment authority record, follow the below steps:

1. Authorise Authority Amendment .
2. In the Unauthorised LC Amendments screen, click the Delete icon from the list of unauthorised reimbursement amendment authority record.
3. In the LC Amendment(Ben Consent sought) screen, click the Delete icon to delete an unauthorised reimbursement amendment authority record.

This tab is used to authorise an unauthorised reimbursement claim.

To authorise an unauthorised reimbursement claim, follow the below steps:

1. Authorisation of Claim .
2. In the Unauthorised Reimbursment Claims screen, click the Authorise icon from the list of unauthorised reimbursement claim.
3. In the Register Reimbursement Claim screen, click the Authorise icon to authorise an unauthorised reimbursement claim.

To delete an unauthorised reimbursement claim, follow the below steps:

1. Authorisation of Claim .
2. In the Unauthorised Reimbursment Claims screen, click the Delete icon from the list of unauthorised reimbursement claim.
3. In the Register Reimbursement Claim screen, click the Delete icon to delete an unauthorised reimbursement claim.

This tab is used to view the list of claims that are maturing today. Follow the below steps to view the reimbursement claim details.

- In the Reimbursement Claims MaturingToday screen, click the View Drawing icon to view the reimbursement claim details.

This tab is used to view the summary of a LC.

1. In the Reimbursement Summary screen, enter the LC reference number.
2. Click the FIND button to view the LC summary.


#### 📊 Outputs

After the drawings completion, the user can view the below enquiries, advices and swift messages.


##### Enquiries and Reports

This section allows the user to view the details such as, import LCs pending documents, usance bill discounting, import LCs that are expired but outstanding, import LCs that are linked to shipping guarantees.

Trust Release

This enquiry displays the details of the documents under import LC, which are released under Trust. The user can view the drawing record by clicking the View Record icon.

Expired

This enquiry displays the list of import LCs, which are expired but the liability of these are yet to reverse or nullify in the bank’s book. The user can view the LC by clicking the View Record icon.

Linked to SG

This enquiry displays the list of import LCs, which are issued against a shipping guarantee. The user can view the LC and Guarantee transaction record by clicking View LC and View Guarantee icons respectively.

Bills Discounted

This enquiry displays the list of outstanding usance bills that are discounted under import LC. The user can view the drawing record by clicking the View Record icon.

Paid Drawings pending docs

This enquiry displays the list of paid drawings that are pending with documents.

Summary

This enquiry displays the reimbursement summary details for a given transaction reference number.

Today Claims

This enquiry displays the list of reimbursement claims that are maturing today.


##### SWIFT Messages

This section allows the user to view the below list of SWIFT messages.

This message type is an advice of payment for a collection document.

This message is sent by an issuing bank to the reimbursing bank requesting to honour reimbursement claims of payments under letter of credit.

This message is sent by the paying bank or negotiating bank to the authorised bank to reimburse the sender for their payment or negotiations.

This message is generated to notify the receiver that the sender is considering the claim as not in accordance with the instructions in the reimbursement authorisation.


##### Advices

This section allows the user to view the below list of Advices.

This advice is sent to the presenter to inform that the documents received under import LCs consists of discrepancies.

This advice is sent to the applicant as a confirmation for acceptance of documents under letter of credit.

This advice is sent to presenter as an acknowledgement for receiving documents under export letter of credit.

This advice is sent to presenter on receiving payment from LC issuing bank.

This advice is sent to presenter as a confirmation of payment received under letter of credit.

The below schedule is sent to the beneficiary once the payment under documentary credit is credited to their account.


##### Alerts

NA

---


### 2.9  Islamic LoC


> **📇 Quick Reference Card**
> 
> **Purpose:** *The introduction of Islamic principles into the structure of letters of credit, along with modifications to meet the requirements of Islamic trade and finance in the Middle East, is essential given the central role letters of credit play in international trade. It is imperative that these instrument...*
> 
> **Applications:** `LC.PARAMETERS`, `LC.TYPES`
> 
> **Key Fields:** *Applicant*, *Classification*, *Is Payment Category*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The introduction of Islamic principles into the structure of letters of credit, along with modifications to meet the requirements of Islamic trade and finance in the Middle East, is essential given the central role letters of credit play in international trade. It is imperative that these instruments align both conceptually and operationally with Shariah principles. Historically, letters of credit have evolved through trade practices that, over time, gained legal force, but no efforts were made in their early stages to integrate Shariah values into their content and implementation.

Islamic letter of Credit clearly defines the underlying principles and practices of letters of credit, evaluate them from a Shariah perspective, and propose necessary changes to current practices in order to bring letters of credit into compliance with Shariah law and align them with the Islamic value system.

An Islamic Letter of Credit (ILC) is a financial instrument used in international trade that complies with Islamic law (Shariah). It acts as a guarantee from a bank to a seller (beneficiary) that payment is made upon the fulfillment of specific conditions. This mechanism is vital for facilitating trade while ensuring adherence to Islamic principles, particularly those prohibiting interest (riba) and excessive uncertainty (gharar).

In the case of a Letter of Credit using Murabaha, the procedures of Murabaha are applied, with the exception that payment to the bank is not deferred. The Islamic bank opens the LC and, after the shipment of goods and submission of the required documents, makes payment to the exporter using the bank’s own funds. Upon the arrival of the goods, the bank takes delivery and sells the goods to the client. The bank recovers its cost and earns a small commission for services rendered as an agent, while the client repays the bank on a deferred basis, as agreed.


#### ⚙️ Configuration

The user can define the configuration to trigger the Islamic LC process in the LC.TYPES table, where the Classification field is used to initiate the Islamic configurations. The transaction bank can configure a separate LC type for Islamic transactions and, in the Classification field, use a prefix of ‘IS’ followed by the specific nature of the Islamic LC.


#### 🔧 Working With

Once the configurations for the Islamic Letter of Credit (LC) are completed, the process largely follows the same flow as a conventional LC. The first step involves the issuance of the Pre-Advice for the LC, which triggers the MT705 SWIFT message.

The following example illustrates how the Pre-Advice flows within this process.

Upon configuring the LC type for the Islamic Letter of Credit, the system utilizes the same configuration for subsequent transactions. The user enters the basic details, including the parties involved in the LC into the system.

After validating and committing the contract, the system updates the relevant MT705 fields which generates the Pre-Advice of the LC. This Pre-Advice is a SWIFT MT705 message where the Issuing Bank is populated in the Applicant field of the message, signifying the party initiating the LC.

This same process continues in the LC issuance phase. When the LC is issued, the MT700 message is generated. In this message, the Issuing Bank is once again listed in the Applicant field, just as it appeared in the MT705 message, confirming the bank's role in initiating the letter of credit.

> **⚠️ Note:** When the applicant's address is updated, the system does not populate tag 50 in 707 unless there is a change in the issuing bank name in the Transact.

During the document presentation phase, the regular procedures followed in conventional LCs are applied. This includes the registration of the documents, handling any discrepancies, and processing the negotiation flow as per standard procedures. The system ensures that all document-related processes align with the usual trade finance practices, ensuring that the documents are reviewed, discrepancies are handled, and payments are negotiated efficiently.

However, a key difference occurs in the payment process for the drawings. The transaction bank defines the intermediary configuration for the Islamic LC, which specifies how the payment is processed. Based on this configuration, the system defaults the payment mechanism based on the currency of the drawing. This ensures that the payment process adheres to the rules and regulations specific to Islamic finance, while also allowing for the efficient processing of payments in the correct currency. Once the currency is determined, the payment is processed accordingly and can be used for settling the drawing in compliance with the established terms of the Islamic LC.

> **⚠️ Note:** The category is derived from the Is Payment Category field in LC.PARAMETERS .


#### 📋 Tasks

There are no Tasks available for Islamic Letter of Credit feature.


#### 📊 Outputs

There are no Outputs available for Islamic Letter of Credit feature.


> **Related Applications:** `LC.PARAMETERS`, `LC.TYPES`

---


### 2.10  Issuance or Register of a LC


> **📇 Quick Reference Card**
> 
> **Purpose:** *This enables the user to understand the issuance/register of LC and the roles of an issuing bank.*
> 
> **Key Fields:** *Back-to- Back*, *Back-to-Back LC*, *Disposal of Docs*, *Instructions from Intermediary Bank*, *Record Type*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

This enables the user to understand the issuance/register of LC and the roles of an issuing bank.


##### Issuance of Import LC

An import Letter of Credit (LC) is an unconditional undertaking, given by a bank (issuing bank) at the request of their customer (applicant or importer) to pay the beneficiary (or supplier) against stipulated documents, provided all the terms and conditions in the LC are complied with.

The issuing bank of the LC can:

- Undertake to make payment to the order of a third party (beneficiary) or accept and pay bills of exchange (or drafts) drawn by the beneficiary at sight or on a fixed future date.
- Authorise another bank (normally the bank in the exporters’ country) to effect payment, or to accept and pay bill of exchange on a fixed future date.
- Authorise another bank to negotiate against credit compliant documents.

The issuing bank does the following during the of issuance of LC:

- LC application request related checks (manual check by the user)
- Credit-related checks (manual check by the user)
- Legal and regulatory checks (manual check by the user)
- Captures the LC details in the system (user enters the LC data in the system)
- Transmission of the LC messages (generate delivery message as the preview)
- Provide reimbursement authorisation (generate delivery message as the preview)


##### SWIFT 2023 Changes for Documentary Credit

As a part of SWIFT Regulations 2023 the length of the below mentioned tags is increased from 65x to 140z ,in MT700/710/720.

| Tag | SWIFT Field Name |
|---|---|
| 44A | Place of Taking in Charge/Dispatch from .../Place of Receipt |
| 44E | Port of Loading/Airport of Departure |
| 44F | Port of Discharge/Airport of Destination |
| 44B | Place of Final Destination/For Transportation to.../Place of Delivery |

In MT710/720, the newly introduced Instructions from Intermediary Bank field is of length 12*65x, Tag 78D and Status=O.


#### ⚙️ Configuration

This section explains the configuration for a non-bank issuer of LC.

For a non-bank issuer of the credit, the Record Type field has to be set as Class in ACCOUNT.CLASS .

The sector has to be defined separately for non-bank issuer in the SECTOR table.

The Customer ID has to be created with sector pertaining to non-bank issuer accordingly.


#### 📋 Tasks

Related topics:

- Amend Import LC
- Issue Back To Back LC
- Trade Finance and Guarantees Processes
- Corporate Issue Import LC

The Temenos Transact trade finance application supports the recording and administration of Letter of Credits (LCs) and documentary collections. The application is fully integrated with the rest of the Temenos Transact system, taking advantage of the Temenos Transact limits processing, accounting, position management and customer portfolio and security features.

The user can create many different types of LCs by using the LC.TYPES application, where combinations of the major features of a LC is set up. For example, import or export, sight or usance, payment or acceptance, confirmed or unconfirmed.


##### Workflow

The Trade Finance Officer can issue various LCs using the below workflow:

This section consists of:

This menu allows the user to issue Import Sight Payment Letter of Credit.

To issue an Import Sight Payment LC, follow the below steps:

1. Issue of Sight Payment LCs .
2. In the Import Sight LCs screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to issue an Import Usance Letter of Credit.

To issue an Import Usance LC, follow the below steps:

1. Issue of Usance LCs .
2. In the Import Usance LCs screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to issue an Import Negotiation LC.

To issue an Import Negotiation LC, follow the below steps:

1. Issue of Negotiation LCs .
2. In the Import Negotiation LCs screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to issue Mixed Payment Letter of Credit.

To issue a Mixed Payment LC, follow the below steps:

1. Issue of Mixed Payment LCs .
2. In the Import Mixed Payment LCs screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to issue a standby LC.

To issue a standby LC, follow the below steps:

1. Issue of Stand By LCs .
2. In the Import Stand By LC screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for errors and overrides.
4. Click the Delivery Preview icon to view the swift messages.
5. Click the Commit icon to submit the record.

This menu allows the user to issue a Back to Back Import Letter of Credit.

To issue a Back to Back Import LC, follow the below steps:

1. Back to Back Import LC .
2. In the Back to Back Import LCs Screen, Click the Modify Import LC icon for corresponding record to issue a Back to Back LC.
3. In the Back to Back import LC screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This section consists of:

This menu allows the user to register an export LCs that are of back to back LC type.

To register an export LC, which are of back to back type, follow the below steps:

1. Export LC for Back to Back LC .
2. In the Export LCs screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to advise or register the standby LCs.

To advise or register a standby LC, follow the below steps:

1. Advise/Register Stand By LCs .
2. In the Export Stand By LC screen, enter values in the mandatory and other fields.
3. Click the Validate icon to check for errors and overrides.
4. Click the Delivery Preview icon to view the swift messages.
5. Click the Commit icon to submit the record.

This menu allows the user to advise or register the Sight Payment LC.

To advise or register a Sight Payment LC, follow the below steps:

1. Advice/Register Sight payment LCs .
2. In the Export Sight Payment LCs screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to advise or register Usance LC.

To advise or register an Usance LC, follow the below steps:

1. Advice/Register Usance LCs .
2. In the Export Usance LCs screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to advise or register a Negotiation LC.

To advise or register a Negotiation LC, follow the below steps:

1. Advice/Register Negotiation LCs .
2. In the Export Negotiation LCs screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to advise or register a Mixed Payment LC.

To advise or register a Mixed Payment LC, follow the below steps:

1. Advice/Register Mixed Payment LCs .
2. In the Export Mixed Payment LCs screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to transfer the Export LC to one or more second beneficiary.

To transfer an Export LC, follow the below steps:

1. Transfer of Export LC .
2. In the Transfer of Export LC screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the Trade Finance Officer to issue the Letter of Credits that are requested from the Corporate Internet Banking.

For the issuance of internet LCs, follow the below steps:

1. Internet Requests .
2. Click the Pending with Bank tab to view the list of pending requests.
3. Select the operation to O and IB Status to Approved.
4. Enter the Temenos Transact banks instruction, charges or margin details.
5. Click the Commit icon to submit the record.

This section consists of:

This menu lists the inward letter of credit messages that are created from the incoming SWIFT messages and are on On hold status by Temenos Transact .

Follow the below steps to process the inward SWIFT messages:

1. Inward LC’s .
2. In the Inward LC’s under Inward SWIFT Messages (LC) screen, click the Modify icon to process the inward swift messages.
3. Enter values in the mandatory fields based on the message types.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu displays the processed inwards of MT752 and MT756 message types.

To process the inward amendment SWIFT messages, follow the below steps:

1. Other Inward Messages .
2. In the Bene Consent Amendment’s under Inward SWIFT Messages (LC) screen, click the Modify icon to process the inward swift messages.
3. Enter values in the mandatory fields based on the message types.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This section consists of:

This menu,

- Displays MT750 and MT754 messages which creates the drawing type as 'CO' and 'SP' under an existing Import Letter of Credit
- Allows the user to view and process the SWIFT message according to their message type.

To view the inward SWIFT messages, follow the below steps:

1. Import Inward Swift Messages .
2. In the Inward Swift Messages – Import screen, click the View icon corresponding to a record to view the inward SWIFT messages.
3. In the Incoming Message’s Tag Details screen, view the SWIFT message.

To process the documents, follow the below steps:

1. Import Inward Swift Messages .
2. In the Inward Swift Messages – Import screen, click the Process the Message icon corresponding to a record to process the inward SWIFT messages.
3. In Capture/Check documents screen, enter values in the mandatory fields based on the message types.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to preview the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to view and reply to the acknowledgement message received.

To view an Acknowledgement message, follow the below steps:

1. Acknowledgement Messages .
2. In the Acknowledgement Messages screen, click the View icon corresponding to a record to view an Acknowledgement Message.
3. In the Incoming Message’s Tag Details screen, view the SWIFT message.

To process the inward SWIFT messages, follow the below steps:

1. Acknowledgement Messages .
2. In the Acknowledgement Messages screen, click the Edit icon corresponding to a record to reply to the Acknowledgement Messages.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to preview the delivery messages.
5. Click the Commit icon to submit the record.

This menu lists the inward letter of credit messages that are created from the incoming swift messages and are on ‘On hold’ status by Temenos Transact.

To process the inward SWIFT messages, follow the below steps:

1. Inward LC’s .
2. In the List of Inward Export LCs on HOLD screen, click the Modify icon corresponding to a record to process the inward SWIFT messages.
3. Enter values in the mandatory fields based on the message types.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to preview the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to view the received MT734 SWIFT messages and process the documents for rejection to beneficiary.

To view SWIFT messages, follow the below steps:

1. Rejection through MT734 .
2. In the Inward Swift Messages - Export screen, click the View SWIFT Message icon corresponding to a record to view the SWIFT message.
3. In the Incoming Message’s Tag Details screen, view the SWIFT messages.

To process the documents for rejection to beneficiary, follow the below steps:

1. Rejection through MT734 .
2. In the Inward Swift Messages - Export screen, click the Process the Message icon corresponding to a record to view the SWIFT message.
3. In Reject Documents under Export LC screen, enter a value in the Disposal of Docs field and in other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to preview the delivery messages.
6. Click the Commit icon to submit the record

This menu shows list of Unauthorised (INAU) records in DRAWINGS which have been created through the inward messages MT744 with options to view, edit and also to send a MT799 message.

To view the SWIFT messages, follow the below steps:

1. Non-Conforming Reimbursements .
2. In the Notice of Non-Confirming Reimbursements screen, click the View SWIFT Message icon to view the swift message.
3. In the Incoming Message’s Tag Details screen, view the SWIFT messages.

To edit a contract, follow the below steps:

1. Non-Conforming Reimbursements .
2. In the Notice of Non-Confirming Reimbursements screen, click the Edit icon to process the transaction.
3. In the Notice of Non-Confirming Claim screen, modify the required details.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to preview the delivery messages.
6. Click the Commit icon to submit the record

To send a MT799, follow the below steps:

1. Non-Conforming Reimbursements .
2. In the Notice of Non-Confirming Reimbursements screen, click the Send MT799 icon to send a MT799 message.
3. In the Free Format Messages MT799 screen, enter values in the mandatory and in other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to preview the delivery messages.
6. Click the Commit icon to submit the record

This menu lists all the inward SWIFT messages which does not create any transaction in Temenos Transact due to the invalid transaction reference provided in tag 21.

To view the SWIFT messages, follow the below steps:

1. Processing Of Repaired Messages .
2. In the Inward Trade Finance Swift Messages screen, click the View SWIFT Message icon corresponding to a record to view the SWIFT message.
3. In the Incoming Message’s Tag Details screen, view the SWIFT messages.

To send a MT799 or MT499, follow the below steps:

1. Processing Of Repaired Messages .
2. In the Inward Trade Finance Swift Messages screen, click the Send MT799/MT499 icon corresponding to a record to view the SWIFT message.
3. In Free Format Messages screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to preview the delivery messages.
6. Click the Commit icon to submit the record

This menu displays the processed inwards of MT752, MT756, MT732 message types.

To view the SWIFT messages, follow the below steps:

1. Other Inward Messages .
2. In the Inward Swift Messages - Export screen, click the View SWIFT Message icon corresponding to a record to view the SWIFT message.
3. In the Incoming Message’s Tag Details screen, view the SWIFT message.

To process the inward messages, follow the below steps:

1. Other Inward Messages .
2. 2. In the Inward Swift Messages - Export screen, click the Process the Message icon corresponding to a record to process the transaction.
3. Enter values in the mandatory fields based on the message types.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to preview the delivery messages.
6. Click the Commit icon to submit the record.


#### 📊 Outputs

The Temenos Transact trade finance application supports the recording and administration of Letter of Credits (LCs) and documentary collections. The application is fully integrated with the rest of the Temenos Transact system, taking advantage of the Temenos Transact limits processing, accounting, position management, and customer portfolio and security features.

The user can create many different types of LCs by using the LC.TYPES application, where combinations of the major features of a LC is set up. For example, import or export, sight or usance, payment or acceptance, confirmed or unconfirmed.


##### Enquiries and Reports

This section helps the user to view the details such as, LC expiry date, outstanding LCs, bills due for settlement, and so on.

Outstanding

This enquiry displays the list of outstanding import LCs. The user can view the LC record and document by clicking the View Record and View Document icons respectively.

Usance Bills Due

This enquiry displays the list of usance bills that are accepted under import LCs and are yet to be settled or paid (that is the maturity date is less than today). The user can view the drawing record by clicking the View Record icon.

LC Expired

This enquiry displays the list of export LCs that are expired but the liability of which are yet to be reversed in the bank’s books.

LC Summary – Import

This enquiry displays the detailed summary of all import LC transactions and also provides the summary details of various actions such as, issue, amendment and drawing completed in a selected import letter of credit.

LC Summary – Export

This enquiry displays the detailed summary of all export LC transactions and also provides the summary details of various actions such as, issue, amendment and drawing completed in a selected export letter of credit.


##### SWIFT Messages

This section helps the user to view the below listed SWIFT messages:

This message is sent to the issuing bank as an acknowledgement to the receipt of the documentary credit message.

This message is sent by a bank, which has received details of a letter of credit from the issuing bank, to be advised through another bank to the beneficiary.

This message is sent by the issuing bank to the advising bank.

MT103 is the direct payment order to the beneficiary’s bank, which results in the beneficiary’s account being credited.

MT202 denotes the movement of funds between financial institutions.

This message requests for the transfer of funds between financial institutions, related to an underlying customer credit transfer that was sent with the cover message.

This message is an advance notice to the account servicing institution stating that the institution receives funds. These funds are to be credited to the sender’s account.

This message is used to enquire about the status of the documents sent for collection.

This message contains information for which no other message type has been defined.

This message is sent when an export LC is transferred by the first beneficiary to a second beneficiary.

This message is sent by the bank to the issuing bank for the documents that are submitted. It is used to advise the receiver that the documents submitted are not in accordance with the terms and conditions of the credit.

This message is sent by paying or accepting bank to the issuing bank. It is used to advise the receiver that the documents submitted are in accordance with the credit terms and are forwarded as instructed.

This message is sent by issuing bank to a paying or negotiating or accepting bank in response to an MT750. It is used to advise the receiver that the documents can be picked up and they are in order in spite of discrepancies.

This message contains information for which no other message type has been defined.


##### Advices

The section helps the user to view the list of advices:

This advice is sent to the applicant as a confirmation of receiving the documents under import LC.

This advice is sent to the applicant as a confirmation of letter of credit upon opening of import LC.

This advice is sent to the applicant with the LC copy and swift copy upon opening of import letter of credit.

This advice generates when the user advise or register the Export LC.


##### Alerts

NA

---


### 2.11  Managing External Requests


> **📇 Quick Reference Card**
> 
> **Purpose:** *Transact and its associated APIs capture external requests for Trade Finance products such as Letters of Credit and Documentary Collections. External requests from sources such as corporate users, interbank banking, or other channels are now seamlessly integrated into the system. Once a request is i...*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Transact and its associated APIs capture external requests for Trade Finance products such as Letters of Credit and Documentary Collections. External requests from sources such as corporate users, interbank banking, or other channels are now seamlessly integrated into the system. Once a request is initiated, the system automatically notifies the Trade Finance bank user so they can perform the necessary action in Transact. This streamlines workflows, ensuring the efficient and secure management of trade finance requests across diverse channels.

Read Home to know more about the published APIs and read Trade Finance to know more about Temenos Digital.


#### ⚙️ Configuration

This feature has no specific configuration to be setup. The parameter applications are setup at the implementation stage.


#### 📋 Tasks

There are no Tasks available for Managing External Requests feature.


#### 📊 Outputs

There are no Outputs available for Managing External Requests feature.

---


### 2.12  Margin or Provisions


> **📇 Quick Reference Card**
> 
> **Purpose:** *Provision or margin (collateral) is collected from the customer at the time of issuing or confirming a Letter of Credit (LC). This can be up to or exceeding 100% of LC value. The provision collected can be parked in any account defined by the user or in a default internal account (when not defined).*
> 
> **Key Fields:** *Limit With Prov*, *Prov Calc Base*, *Prov Netting*, *Take Margin?*, *Take/Reduce Margin*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Provision or margin (collateral) is collected from the customer at the time of issuing or confirming a Letter of Credit (LC). This can be up to or exceeding 100% of LC value. The provision collected can be parked in any account defined by the user or in a default internal account (when not defined).


#### ⚙️ Configuration

The following parameter setup is done for margin or provision:

- Transaction codes related fields for provision or margin are defined in LC.PARAMETERS .
- The bank can define if the provision on LC is to be calculated on LC or liability amount. It is defined using Prov Calc Base field in LC.PARAMETERS . (The input in this field is superseded by inputs under Prov Calc Base in the Issuance of LC).
- Prov Netting field in LC.PARAMETERS is used to net the proportionate cash margin released along with the drawings amount and debit the balance amount from the drawdown account when drawings are initiated.
- Customer limit is optionally updated by taking into account the provision collected by defining Limit With Prov field in LC.PARAMETERS .
- LC.CUSTOMER.CONDITION is used to default provision percent and accounts.


#### 📋 Tasks

Related topics:

- Amend Import LC
- Take or Release Margins
- Trade Finance and Guarantees Processes

Trade Finance application allows margin or provision upto and above hundred percent of the Letter of Credit (LC) amount.

In few cases, where there is a tolerance or an additional amount specified for the LC or where a shipping guarantee against the LC has been issued a provision or margin is required in excess of hundred percent of LC.


##### Workflow

In this feature, the user can perform the below activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Take/Reduce Margin . |
| Contract Screen | Select a value in the Take/Reduce Margin field drop-down. Click the Edit icon. |
| Take/Reduce Margin | In the Import LC tab, select the Y option in the Take Margin? field. Enter values in the required fields. Click the Validate icon to check for errors and overrides. Click the Delivery Preview icon to view the delivery messages. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Release Margin . |
| Margin Outstanding in Import LCs | Click the Release Margin icon. |
| In the Release Margin on Import LC | Enter values in the mandatory and other required fields. Click the Validate icon to check for errors and overrides. Click the Delivery Preview icon to view the delivery messages. Click the Commit icon to submit the record. |


#### 📊 Outputs

The user can view the below delivery messages while releasing the margin for an import LC.


##### Enquiries and Reports

NA


##### SWIFT Messages

NA


##### Advices

The user can view the below advice related to import LC.

After releasing the margin for an import LC, the user can view the credit advice for provision release.


##### Alerts

NA

---


### 2.13  Merchanting Trade


> **📇 Quick Reference Card**
> 
> **Purpose:** *A trade contract is identified as a Merchanting Trade when:*
> 
> **Key Fields:** *Lc Types*, *Linked Merchant Trade Reference*, *Merchant Trade*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

A trade contract is identified as a Merchanting Trade when:

- The supplier of goods is resident in one foreign country
- The buyer of goods is resident in another foreign country
- The merchant or the intermediary is resident of another country (third country)

The merchant books a Buy order from the buyer, places a relevant order with a supplier, supervises and coordinates the shipment of goods from the supplier’s country and delivers the same in the buyer’s country.

The merchant receives the payment from the overseas buyer and makes the payment to the overseas supplier through the supplier’s banker, for the above said trade. The difference between inward remittances from the buyer and the outward remittance is the profit for the merchant from that merchanting trade cycle.

The TF modules support linking the two sides of a merchanting trade contract and the same is illustrated below.


#### ⚙️ Configuration

This feature has no specific configuration to be setup.


#### 🔧 Working With

The LETTER.OF.CREDIT and DRAWINGS applications support identifying if the underlying contract is a merchanting trade or not. These applications enable linking the two sides of the merchanting trade contracts, that is, linking the import and export side of the merchant trade cycle and vice versa.

- If the trade documents submitted are for the first leg under the merchant trade cycle, the contract can be marked as First Leg in the Merchant Trade field from the drop down list(as shown below).
- Marking the contract as First Leg helps to identity the said trade contract as a merchanting trade contract and it enables the system to link the second leg of the contract or linked contract, when the documents are submitted any time after the presentation of the first leg document.
- Subsequently, when the second leg document is received and marked as Yes from the drop down list, the contract reference or @ID of the first leg becomes mandatory and the same has to be updated in the Linked Merchant Trade Reference field.
- Upon authorization of the second leg contract (marked as Yes in the Merchant Trade field), the first leg contract reference is updated with this second leg contract / linked contract reference or @ID.
- The linking is now established between two contracts of the merchanting trade cycle.

- The linking is supported for one-to-one contracts (or transactions) only and not for one-to-many or many-to-one contracts.
- Linking is not possible between LC reference and Drawings reference. Two contracts of the Merchanting trade can be linked between Drawings reference to another drawings reference and LC reference to another LC reference only.
- The linking is established only when one contract is export and the other is import or vice versa. It is not possible to link two exports or two imports contracts.
- For contracts with Lc Types as Documentary Letter Of Credit, the merchanting trade link can be established in the DRAWINGS application only.
- For contracts with Lc Types as Documentary Collection or Open Account Trade or Trade Evidence Against Advance Payments, the merchanting trade link can be established in either LETTER.OF.CREDIT or DRAWINGS application.
- The linking is established as long as the trade products are lodged or settled within the TF modules, that is, within LETTER.OF.CREDIT and DRAWINGS applications.
- When one side of the contract under the merchanting trade cycle is Documentary Letter of Credit and the other side of the contract is Documentary Collection or Open Account Trade or Trade Evidence Against Advance Payments, then the linking should always be done in the DRAWINGS application only for both the sides of the contract.


#### 📋 Tasks

There are no Tasks available for Merchanting Trade feature.


#### 📊 Outputs

This enquiry allows the user to view the list of Merchant trade contracts based on various selection criteria.


##### Enquiries and Reports

The user can view the below list of enquiries and reports:

Merchant Trade Under LC

This enquiry displays the list of merchant trade contracts under Letter of Credit application. The user can further drilldown to the application by clicking the View Record icon.

Merchant Trade Under Drawings

This enquiry displays the list of merchant trade contracts under Drawings application. The user can further drilldown to the application by clicking the View Record icon.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


### 2.14  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *International trade is conducted between or among individuals or organisations not well known to each other and/or located in different countries. The seller requires the confidence that the buyer is credit worthy and pays on time; on the other hand, the buyer needs an assurance that the seller supp...*
> 
> **Applications:** `LC.TYPES`
> 
> **Key Fields:** *Amort Trans*, *Amortisation Cycle Foreign Currency*, *Amortisation Cycle Local Currency*, *Amortise Charges*, *Application*, *Backward Delivery*, *Category Code*, *Category code* ... +92 more
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- APIs
- Temenos Transact Services
- System Maintained Files

International trade is conducted between or among individuals or organisations not well known to each other and/or located in different countries. The seller requires the confidence that the buyer is credit worthy and pays on time; on the other hand, the buyer needs an assurance that the seller supplies goods as per contracted terms. The seller in such cases would prefer a well-known bank to provide a commitment for payment and the buyer likewise would like to include appropriate terms, conditions and documentation that would assure description, quality and quantity of goods.

A Letter of Credit (LC) is a widely used instrument in international trade that meets the requirements of both the buyers and sellers. It is an undertaking by the issuing bank to the beneficiary of the credit, made on behalf of the applicant to pay irrevocably, on fulfillment of terms and conditions mentioned. Additionally, the banks play different roles (issuing, advising, confirming, negotiating and reimbursing bank) in the LC cycle to fulfill the LC conditions along with the parties mentioned in the credit.

The International Chamber of Commerce (ICC) is the world’s largest business organisation working to promote international trade, responsible business conduct and a global approach to regulation to accelerate inclusive and sustainable growth to the benefit of all members. ICC governs documentary credits (also known as LCs) in form and content. The Uniform Customs and Practices for documentary Credits (UCPDC) publication is a set of rules on the issuance and use of LC.

The below topic describes the different payment methods used in trade finance, work flow, list functionalities supported in different modules and LC in Temenos Transact .

LC is a financial instrument that is widely used in the international trade. It is issued by the importer’s bank at the request of the importer (buyer or applicant) in favour of the exporter (seller or beneficiary). It is a commitment to make payments, provided the exporter submits the required documents and complies with the terms and conditions stated in the LC. It is customary for the LC to be advised to the beneficiary through a bank, called the advising bank. It is one of the most secure methods for a seller to receive payment and the buyer to receive goods as per contracted terms and conditions. LC from a risk management perspective mitigates trade and payment risks.

The LETTER.OF.CREDIT and DRAWINGS applications are closely coupled to provide a wide range of support for trade finance business. This ensures a seamless automated business process flow starting from issuing an LC and concluding with drawings.

The LETTER.OF.CREDIT application supports opening and amending LCs and documentary collections (import and export). It suits all the roles of a bank (issuing, advising, confirming and negotiating). The DRAWINGS application records the presentation of documents under the LC and makes the actual payments under the LC or collection, that is, negotiation of LCs and collections are handled through DRAWINGS application.

The following are the list of functionalities supported in the LETTER.OF.CREDIT , LC.AMENDMENTS and DRAWINGS module:

- Pre-advice of a LC
- Issue or Register and Advise of an LC Sight or Usance LC Payment or Acceptance Back to Back LC Confirmed LC Transfer LC Revolving or Reinstatement LC
- LC Amendments
- Drawings Mixed Payments (with limited functionality) Payment handled through Payment order Payment handled through LC module Brokerage
- Reversal or Cancellation of LC
- Charges
- Commission
- Margin or Provision
- Pre-shipment Finance
- Post-shipment Finance
- Assignment of Proceeds
- Shipping guarantee
- Ticklers and Tracers
- Syndicated Letter of Credit
- Swift Messages
- Collections Direct Export Collections Collection Amendments Shipping Guarantee against Import Collections Outward or Inward Collection Avalisation Clean Collection Open Account Trade Trade Evidence for Advance Payments

Trade finance module supports the recording and administration of LCs and documentary collections. It records the full details of the credit including amounts, dates, parties involved, charges, commission, margin and so on. Additionally, the trade finance module includes LETTER.OF.CREDIT , LC.AMENDMENTS , DRAWINGS and DRAW.NEGOTIATION that support the processing and management of both import and export LC cycle.

LETTER.OF.CREDIT application is used to send pre-advices, open LCs and make amendments. LC.AMENDMENTS application is used to send amendments. DRAWINGS and DRAW.NEGOTIATION applications are used for negotiations and payments.

The LC cycle starts from issuance of the LC and ends on payment realisation (including the principle features governing the LC). The flow and features differ between import and export type of LC. Not every LC needs to go through the entire cycle and this depends on the type and requirement of the LC. The LETTER.OF.CREDIT application records the initial liability of an LC (that is, the amount of the facility) or the request to make a collection. The DRAWINGS application makes the actual payments and drawings under the LC or collection.

Additionally, for high value transactions most banks participate in syndicated LC deals. Both LC and SL module support the processing and management of import and export LC under a syndicated facility. Large number of VERSION and ENQUIRY records are supplied with Temenos Transact Model Bank (MB) for trade finance products supporting flows in line with each features, and these are detailed within the Model Bank Reference Documentation .

- A LETTER.OF.CREDIT has to exist for the user to enter the details in the DRAWINGS application.
- An efficient delivery system is the backbone of the entire module. It is linked on-line with soft delivery, which means the user has the option to verify delivery messages before being transmitted.
- Trade finance transactions can be handled in any currency. Drawings made and/or charges collected can be denominated in a currency different from the LC currency. All foreign money entries automatically update foreign exchange positions if necessary.

Documentary credits are often a preferred method of payment in international trade. An LC, also referred to as a documentary credit, is a contractual agreement whereby the issuing bank (importer’s bank), acting on behalf of its customer (the importer or buyer), promises to make payment to the beneficiary or exporter against the receipt of complying stipulated documents. The issuing bank typically uses intermediary banks to facilitate the transaction and make payment to the exporter. In import LC, issuing bank take the main role of issuing the LC.

When

is the importers bank, who wants to finance a deal with an LC, then the user enters the LC details using the

application. This automatically checks and updates the customer’s credit limit, advises the various parties by SWIFT or printed advice, and takes any initial charges, etc. When

bank is requested to make a payment under the LC the details are entered in the

application, which makes any necessary accounting entries, send all required payment messages, advise the various parties and reduce the LC by the drawing amount.

> **⚠️ Note:** Documents are printed using the DELIVERY application. The outward messages for an LC can be previewed at the input stage.

The following are the roles of the issuing bank, the type of operation performed in Temenos Transact aligning with the business function.

The Issuing bank can perform the following through LETTER.OF.CREDIT or LC.AMENDMENTS applications:

- Issue a re-advice by SWIFT
- Issue the actual LC based on the pre-advice
- Amend the LC terms and conditions
- Authorise a reimbursement
- Amend a reimbursement
- Reverse or cancellation of LC

The Issuing bank can perform the following through DRAWINGS application:

- Receive and pay drawings
- Send advice and effect a payment
- Authorise reimbursement or payment

> **⚠️ Note:** The above stages are for illustration purposes and not every LC needs to go through all of these stages.

The issuing bank requests the exporter’s bank to advice (with or without adding confirmation) and in due course exporter’s bank may undertake to accept documents from the beneficiary under the terms of the credit.

Temenos Transact supports the creation of the LC manually or on a semi-automatic basis on the receipt of an incoming SWIFT message (MT700 or 710 or 720 or 705). The same processing is done as in the example used for import, but in this instance, it is in the opposite role. The same conditions applies for sight, acceptance or deferred payments and the scale of charges is related to the role of the exporter's bank. The exporter’s bank can perform the following using the LETTER.OF.CREDIT or LC.AMENDMENTS applications.

They can act as advising bank and/or confirming bank and/or negotiating bank. The basic role is listed below:

- Advise a pre-advice to beneficiary or by SWIFT to second advising bank
- Advise the LC to beneficiary or by SWIFT to second advising bank
- Advise the amend under the LC to beneficiary or by SWIFT to second advising bank
- Request reimbursement
- Send acceptance or rejection of amendment message
- Confirm or negotiate the LC
- Transfer of LC
- Issue back to back LC
- Handle the documents presented under LC or collections


##### Configuring Letter of Credit

To support the recording and administration of LC and documentary collections, various parameter files and system tables need to be set up. This section provides a brief overview of the system and parameter set-up for holding the static data that is standard for LC and drawings processing. This section explains the various parameters and system core table setup that need to be set for operation of the LC and related modules.

| Field | Description |
|---|---|
| Reimburse Days | Sends reimbursement message in case of usance drawing before maturity. It is also used to decide when to send a MT 742 and MT754 SWIFT messages. |
| Revol Advice Days | Sends a revolution advice before the next revolution. |
| Maturity Usance | Reports imminent maturity of usance drawings. |
| Collections Due | Reports imminent due date of collections. |

| Code | Description of Use |
|---|---|
| P | Pre-advises a LC. This function accepts a reduced amount of information regarding the LC and when authorised, generates appropriate advices for despatch to the various patties in the transaction. |
| O | Opens a new LC or documentary collection. Converts a pre-advised LC into a live LC. At this point the credit limits are checked and utilised, contingent accounting entries are raised and initial charges may be taken. |
| A | Amends an existing LC or documentary collection. Allows the details to be modified. When requested, the system automatically generates amendment advices to be despatched to the parties to the transaction. |
| C | Takes direct charges. This code applies a direct charge to the LC or documentary collection. Charge input is performed on this record but the charges are immediately transferred to the LC.ACCOUNT.BALANCES file where they can be viewed and, in a limited way, amended. |
| T | Traces a documentary collection. This function applies only to documentary collections. Generates tracer messages such as a SWIFT MT420. |

The core tables that are to be set for operation of the LC and related modules are explained below:

Delivery message to the customers for debit or credit of his account, broker for confirmation of trade and depository for completion of settlement of the trade are generated.

Accounting entries are generated on the authorised transactions.

The limit system is designed to monitor the availability and utilisation of limits. Customer limits are monitored in real-time. Back end reports are used to monitor limits for commodities, countries, country groups and currencies. The system caters to defining both simple and complex limits. LC can be issued after setting up of limits and collateral.

Transactions can be done without creating limits. Temenos Transact creates a limit record for the customer for the relevant limit product automatically on authorisation of the LC contract, in the absence of the limit reference with notification message.

The core static tables that need to be set for operation of the LC and related modules are explained below:

Separate category codes are used judiciously to indicate different types of LCs and collection instruments from reporting angle. Care should be taken when defining additional sub-classifications, that sufficient detail is not available to provide the required breakdown.

The banks should not define separate

codes for resident and non-resident customers or for local and foreign currency transactions, since this information is already available on an individual prime record.

LC and DRAWINGS applications use hard coded category range 23000-23999. Each type of LC (and collection) can be defined with a default category code. These codes are used to reflect various LC and collection type in line with the reporting requirement like LC import sight, LC export sight confirmed LC, etc. Further, P/L category code for collecting and writing off charges, commission and internal provision account, category codes used are indicated in LC.PARAMETERS . Default internal accounts in local currency can be opened using the category codes as defined. Category codes between 10000 and 19999 can be used.

ACCOUNT.CLASS records are required for automatic debit or credit by the system. Temenos Transact opens an account in the local currency in the internal category mentioned in ACCOUNT.CLASS . Even if present business does not warrant such setup, it is better to create them. They can be used only if needed. Duplications of category and sector code combined are not allowed within one entry on the ACCOUNT.CLASS table.

- LCAMORT record indicates the internal account for amortisation of charges and commissions if required by the user.
- LCDIFF record to post the differential amount of 0.01 or 0.02 on account of application of exchange rate for the currencies involved in the transaction.
- TFLC record is to default a suspense account in case there is no Nostro account for the credit currency, when bill proceeds are remitted within DRAWINGS application.
- CUSDEBIT record is an internal suspense account used when a customer account is not available for debit in case of sight bills.

There is no standard rule or order for defaulting settlement accounts in LC application. If account numbers are entered for opener, beneficiary and advising bank, then they are defaulted while collecting charges. They are also defaulted in DRAWINGS application.

> **⚠️ Note:** When payment method is indicated as Nostro in DRAWINGS , the payment account is defaulted using NOSTRO.ACCOUNT for the payment currency.

CURRENCY table contains all details of each individual currency. For example currency name, number of decimal places together with other information such as the buy and sell rates.

The markets defined in this table are used to identify the correct exchange and revaluation rates to be applied to each currency. Different rates are used in instances where specific currency markets exists. For example, financial and convertible markets or where pricing considerations require separate rates like normal market rates or notes or travellers cheque.

> **⚠️ Note:** Up to nine currency markets can be created for each currency but when only one market exists, this should be defined as 1, which is the default used by other applications. For example, DATA.CAPTURE and FUNDS.TRANSFER .

This table contains common elements of each currency. This table ensures that the same numeric codes and number of decimals are used for a currency across different companies in a multi-company environment.

HOLIDAY table is used to check whether the maturity or other schedule activity date is a working day at the time of entering a contract. It is possible to indicate the business day definition while entering the contract and Temenos Transact checks the scheduled activities and suitable overrides are generated.

HOLIDAY table is to indicate the public holidays for each country or region within the country. REGION and COUNTRY table must be defined before creating the HOLIDAY table.

The COUNTRY table contains static details of each country, the currency codes, etc.

The LETTER.OF.CREDIT module is dependent on many other applications or functionalities in Temenos Transact .

Customer records are necessary to have details of the underlying party to the LC transactions, counterparty, correspondent banks and broker.

The banks need accounts for payment and receipt into customer and brokerage settlement accounts.


##### Illustrating Model Parameters

Model parameters consists of the below tables:

| Table Name | Description |
|---|---|
| LC.TXN.TYPE.CONDITION | This parameter file is used to setup the default charges for all LC or documentary collections and drawing types. The system has a set of default charges setup in this file for each LC transaction entered. The defaulting mechanism works by defining a record in this file, corresponding to each type of LC ( LC.TYPE ), together with the operations that is performed. |
| LC.GROUP.CONDITION | Defines special rules for a group of customers or specific customers for, (charges, commissions, exchange rate spread and payment value dating). When the definition is for a group of customers, the LC.GEN.CONDITION record must exist before any associated group condition is specified. |
| LC.TYPES | The users can setup customised LC and documentary collections. Defines LC types allowed in the system with their narrative descriptions. Verifies the credit types and sets the default Category Code , during input and validation of LC. It is used for the maintenance of LC statistics in the form of a counter, which is updated when LC is pre-advised, opened, expired and closed. |
| LC.ADVICE.TEXT | Holds static narrative information that helps to map the construction of LC advices or documents that are generated by LC transactions, within the Temenos Transact delivery application. Creates document code and text message related to the documents required in LC. Additionally, provision is available to default the required documents based on customer ID-Inco Terms, and mode of shipment. The record ID is as follows: Customer ID-Inco Terms-Mode of Shipment Inco Terms-Mode of Shipment Customer ID Free Text When opening an import LC in Temenos Transact , the user can select document code against Documents Required field (Swift field 46-A) instead of typing text message. When the user wants to edit the text message, it can be done at contract level. |
| LC.CLAUSES | Holds static narrative information that helps in mapping the construction of LC advices or documents that are generated by LC transactions, within the Temenos Transact delivery application. By creating a record in this file, the user can select the record instead of typing additional conditions (Swift field 47-A) while opening LC. LC.CLAUSES details can also be defaulted at the transaction level based on the applicant's customer ID, inco terms and mode of shipment. The preferential order of the record ID is: Customer ID-Inco Terms-Mode of Shipment Inco Terms-Mode of Shipment Customer ID Free Text |
| DR.DISCREPANT.TYPE | Holds records of discrepant type, EB.ACTIVITY , tickler days, risk party and reduce liability. When discrepant LC export document is payable to beneficiary under payment under reserve, the system updates records based on the setup made in this application. The related activity codes triggers production of advices and swift messages. |
| LC.GEN.CONDITION | Identifies a specific group of customers who are cross-related to the LC.GROUP.CONDITION table to define LC conditions applicable to that group. The key to this table is also the key to the associated LC.GROUP.CONDITION record. LC groups are determined based on customer details such as, sector and target. The criteria used and their priority are specified in the Condition Priority file, in the record whose ID is LETTER.OF.CREDIT . |
| LC.PARAMETERS | Contains data and parameter fields required for LC processing, which are not available in any other file, (there is only one record). Holds static data that is standard for LC and drawings processing. It is used to: Input defaults (closure days, currency, market, position type) Entries generation (transaction codes and account numbers) End of day processing (pre-advise days, accrual or amortisation cycle) |


##### Illustrating Model Products

A LC is a document issued by financial institution on behalf of its customer, which provides a payment undertaking to beneficiary against complying presentation of the documents as stated in the credit.

LC Module supports the below products:

| Product Name | Features |
|---|---|
| Issuance of import LCs | The LC module within model bank ( Temenos Transact ) is used to record the contingent deals that are required to record LC type transactions in the banks’ books. A bank user opens a credit record in Temenos Transact based on the application received from the customer. The initiation to issue a LC can be directly from the corporate client through Corporate Internet Banking channel. The following types of import LCs are issued: Sight payment Usance Negotiation. Mixed payment Stand by The following types of export LCs are advised to the beneficiary: Sight payment Usance Negotiation Mixed payment. Stand by Transfer |
| Maintenance of import LCs | Any changes or cancellation of LC, which is communicated to third parties like advising bank or beneficiary through the generation of the message. Amendment can be either internal or external. Collection and reversal of provision can be done through maintenance of LC’s |
| Drawings under import LCs | Drawings under Import LCs has a flexible payment and reimbursement mechanism whereby funds are collected or paid through a number of intermediaries, and even be paid to parties not involved in the LC. Temenos Transact automatically produces the payment instructions necessary for these facilities. |
| Discounting of usance bills under LC | Issuing bank makes the payment to the beneficiary or negotiating bank before the accepted maturity of the said drawing or bill and then recovers the payment amount from the applicant on the accepted maturity date. |
| Collections | The LC module within model bank ( Temenos Transact ) also facilitate documentary collections (outward and inward). The following types of collections are processed: Documents against payment Documents against acceptance Clean collection |
| Open Account Trade | The LC module within model bank (Temenos Transact) also facilitates Open Account Trade (Import and Outward). The following types of contracts are processed: Lodge import trade documents Lodge export trade documents |
| Trade Evidence for Advance Payments | The LC module within model bank (Temenos Transact) also facilitates registering of trade evidence against the advance payments. |


> **Related Applications:** `LC.TYPES`

---


### 2.15  Open Account Trade


> **📇 Quick Reference Card**
> 
> **Purpose:** *Open Account Trade is the simplest form of trade finance product and services, where the goods are produced and shipped by the exporter and received by the importer even before payment for the transaction is made or becomes due. Also, the necessary trade documents are directly dispatched to the impo...*
> 
> **Key Fields:** *Amend Del*, *Drawing Type*, *Drawings Type*, *Duplicate Check*, *Import Export*, *Internal Amendment Ref*, *Invoice Amount*, *Invoice Number, Invoice Date* ... +4 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Open Account Trade is the simplest form of trade finance product and services, where the goods are produced and shipped by the exporter and received by the importer even before payment for the transaction is made or becomes due. Also, the necessary trade documents are directly dispatched to the importer without intervention of the banks. Banks intervene at the time of remittance against the trade contract, that is, trade document is booked and remittance is initiated.

The below flowchart explains an open account trade cycle.

- Contract agreement between importer and exporter.
- Exporter ships the goods and dispatches the original shipping and commercial documents to importer directly.
- Exporter submits copy the above said documents to their banker.
- Importer receives goods and documents, takes control of the goods and submits the copy of the trade documents to its banker along with payment instruction.
- Importer’s bank lodges the import bills and makes the payment.
- Exporter bank receives payment, credits the exporter and close the outstanding export bills.

Liability is not there on the banks, they just act on the instruction from the importer or exporter to book the trade documents and initiate or receive payment against the documents without any risk or responsibility on its part. The parties involved in an open account trade cycle are:

| Party | Role |
|---|---|
| Seller or drawer or beneficiary or exporter | One who receives the inward remittances against the trade documents for export of goods |
| Buyer or drawee or remitter or importer | One who initiates the outward remittances against the trade documents for import of goods |
| Remitting bank | Buyer’s bank who initiates the outward remittances against trade document |
| Beneficiary bank | Seller’s bank handles the inward remittances against the trade document |


#### ⚙️ Configuration

Configure a new record in LC.TYPES that are specific to open account trade by defining the below:

- Setup the default category code for each type of open account trade.
- Define if the record is export or import trade document, by updating the Import Export field as either I or E.
- Define the Payment Type as either P or A (P – Sight payment and A – Usance), other pay type is not supported for open account trade contract.
- Define the Duplicate Check field based on the Invoice Number, Invoice Date and Invoice Amount fields in LC application.
- The rest of the fields are left blank in LC.TYPES , So that it is understood that the record type does not pertain to documentary LC or documentary collection.


#### 🔧 Working With

The LETTER.OF.CREDIT application supports opening contracts using open account trade method of payments. These can be registered as import or export contracts by setting the Operation field to Ot.

The Drawings Type field is set to Oa or Os to indicate that that open account trade contracts is applied in LETTER.OF.CREDIT application. That is, when Payment Types in LC.TYPES is set to P or A, the Drawing Type is defaulted to OS (P for Payment) or OA (A for Acceptance).

> **⚠️ Note:** No other Drawing Type is allowed for Operation Type with OT.

Any changes to the contract booked in the LETTER.OF.CREDIT application, can be amended only when Operation field is set to A . The Amend Del field is not applicable for open account trading contracts, that is, only internal amendment is allowed for open account trade contracts. The basic details can only be modified.

During remittances or payment, the DRAWINGS version is used. For imports, outward remittance or payment message, MT103 is initiated by debiting the customer’s account and credit to Nostro account. For exports on receipt of inward remittance from the receiving bank, DRAWINGS version is used to debit Nostro account and credit customer (or own account).

> **⚠️ Note:** Banks act only on the instruction of the importer and exporter to initiate or receive payment against the trade documents and do not hold any risk or responsibility on the contract. Hence, contingent accounting is not raised or limits are not blocked.

The user can recover charges as defined in FT.COMMISSION.TYPE . Default charges are defined in LC.TXN.TYPE.CONDITIONS based on LC.TYPES . If charges are not recovered while booking the contract in LC application, the same can be recovered in DRAWINGS .

> **⚠️ Note:** Temenos Transact supports recovery of upfront flat or fixed charges for open account trade.


#### 📋 Tasks

Related topics:

- Amend Open Account Trade (Import)
- Lodge Documents Against Open Account Trade (Import)
- Lodge Documents Against Open Account Trade (Export)
- Amend Open Account Trade (Export)

An Open Account Trading is a sale, where the goods are shipped and delivered before payment. The goods along with the necessary documentation are shipped directly to the importer, who has agreed to pay the exporter at a specified date. The majority of risk in this product lies with the exporter, wherein the goods are dispatched first and then payment is received from the importer.


##### Workflow

The Trade Finance Officer and Trade Finance Supervisor can process the Open Account Transactions using the below workflows:

This menu allows the user to Lodge the Import documents.

To lodge the import documents, follow the below steps:

1. Lodge Import Documents .
2. In the Import Documents screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Commit icon to submit the record.

This menu allows the user to Lodge the export documents.

To lodge the export documents, follow the below steps:

1. Lodge Export Documents .
2. In the Export Documents screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Commit icon to submit the record.

This menu allows the user to amend the lodged Import documents for the internal requirements.

To amend the import documents, follow the below steps:

1. Amend Import Documents .
2. In the Lodged Import Documents screen, click the Amend icon corresponding to a record.
3. In the Internal Amendment of Import Docs screen, enter a value in the Internal Amendment Ref field and amend the required changes in the corresponding fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.

This menu allows the user to amend the lodged export documents for the internal requirements.

To amend the export documents, follow the below steps:

1. Amend Export Documents .
2. In the Lodged Export Documents screen, click the Amend icon corresponding to a record.
3. In the Internal Amendment of Export Docs screen, enter a value in the Internal Amendment Ref field and amend the required changes in the corresponding fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.

This menu allows the user to authorise or delete the lodged or amended import documents.

To authorise the lodged or amended import documents, follow the below steps:

1. Import Open Account/Amendments .
2. In the Unauthorised Open Account Lodgement/Amendment screen, click the Authorise icon corresponding to a record.
3. Verify the transaction details and then click the Authorise icon to commit the authorisation.

To delete the lodged or amended import documents, follow the below steps:

1. Import Open Account/Amendments .
2. In the Unauthorised Open Account Lodgement/Amendment screen, click the Delete icon corresponding to a record.
3. Click the Delete icon to commit the deletion.

This menu allows the user to authorise or delete the lodged or amended export documents.

To authorise the lodged or amended export documents, follow the below steps:

1. Export Open Account/Amendments.
2. In the Unauthorised Open Account Lodgement/Amendment screen, click the Authorise icon corresponding to a record.
3. Verify the transaction details and then click the Authorise icon to commit the authorisation.

To delete the lodged or amended export documents, follow the below steps:

1. Export Open Account/Amendments .
2. In the Unauthorised Open Account Lodgement/Amendment screen, click the Delete icon corresponding to a record.
3. Click the Delete icon to commit the deletion.

This menu allows the user to process the payment of lodged sight import documents.

To process the payment of sight import documents, follow the below steps:

1. Sight Payment of Import Docs .
2. In the Lodged Import Documents screen, click the Pay icon corresponding to a record.
3. In the Payment of Import Documents screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.

This menu allows the user to register the payment of lodged sight export documents.

To register the payment of sight export documents, follow the below steps:

1. Sight Payment of Export Docs .
2. In the Lodged Export Documents screen, click the Pay icon corresponding to a record.
3. In the Payment of Export Documents screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.

This menu allows the user to process the payment of lodged usance import documents.

To process the payment of usance import documents, follow the below steps:

1. Usance Payment .
2. In the Lodged Import Documents screen, click the Pay icon corresponding to a record.
3. In the Payment of Import Documents screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.

This menu allows the user to register the payment of lodged usance export documents.

To register the payment of usance export documents, follow the below steps:

1. Usance Payment .
2. In the Lodged Export Documents screen, click the Pay icon corresponding to a record.
3. In the Payment of Export Documents screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.

This menu allows the user to authorise or delete the sight and usance payments of import documents.

To authorise the sight and usance payment of import documents, follow the below steps:

1. Import Open Account Payment/Pendings .
2. In the Unauthorised Import Open Account Payment screen, click the Authorise icon corresponding to a record.
3. Verify the transaction details and then click the Authorise icon to commit the authorisation.

To delete the sight and usance payment of import documents, follow the below steps:

1. Import Open Account Payment/Pendings .
2. In the Unauthorised Import Open Account Payment screen, click the Delete icon corresponding to a record.
3. Click the Delete icon to commit the deletion.

This menu allows the user to authorise or delete the sight and usance payment of export documents.

To authorise the sight and usance payment of export documents, follow the below steps:

1. Export Open Account Payment/Pendings .
2. In the Unauthorised Export Open Account screen, click the Authorise icon corresponding to a record.
3. Verify the transaction details and then click the Authorise icon to commit the authorisation.

To delete the sight and usance payment of export documents, follow the below steps:

1. Export Open Account Payment/Pendings .
2. In the Unauthorised Export Open Account screen, click Delete icon corresponding to a record.
3. Click the Delete icon to commit the deletion.


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to Open Account Trading in the core banking system.


##### Enquiries and Reports

This section allows the user to view the list of lodged export and import bills based on various selection criteria.

Import Document Lodged

This enquiry displays the list of lodged import bills based on customer. The user can further drilldown to the application by clicking the View Record icon.

Export Document Lodged

This enquiry displays the list of lodged export bills based on customer. The user can further drilldown to the application by clicking the View Record icon.

Billwise Payment Import

This enquiry displays the Import bill wise utilisation. The user can further drilldown to the application by clicking the View Record icon.

Billwise Payment Export

This enquiry displays the Export bill wise utilisation. The user can further drilldown to the application by clicking the View Record icon.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


### 2.16  Post Shipment Finance


> **📇 Quick Reference Card**
> 
> **Purpose:** *Post-shipment finance is an advance payment requested by an exporter after the goods are shipped to the importer. It can be extended with or without recourse.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Post-shipment finance is an advance payment requested by an exporter after the goods are shipped to the importer. It can be extended with or without recourse.


#### ⚙️ Configuration

Post-shipment finance has no specific configuration to be setup. The parameter tables are setup at the implementation stage.


#### 📋 Tasks

Related topics:

- Perform Past Due Write-Off
- Negotiate or Discount Export LC (Sight or Usance or Mixed)
- Negotiate or Discount Export LC (Sight or Usance or Mixed)
- Lending Processes (Corporate)
- Lending Processes (Corporate)

Post-Shipment Finance is a kind of loan provided by a financial institution to an exporter or seller against a shipment that has already been made. This type of export finance is granted from the date of extending the credit, after shipment of the goods to the realisation date (the exact date on which the exporter receives the payment) of the exporter proceeds.


##### Workflow

The user can process the Post-shipment finance using the below workflows:

This menu allows the user to discount or negotiate sight drawings.

To discount a sight bill, follow the below steps:

1. Sight Bill Negotiation/Discounting .
2. In the List of Sight Bills under Export LC screen, click the Discounting icon corresponding to a record.
3. In the Negotiation/Discount Sight Bill (Export) screen, enter values in the mandatory and other required fields.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Validate icon to check for errors and overrides.
6. Click the Commit icon to submit the record.

This menu allows the user to discount or negotiate Usance drawings.

To discount a Usance bill, follow the below steps:

1. Usance Bill Negotiation/Discounting .
2. In the List of Usance Bills under Export LC screen, click the Discounting icon corresponding to a record.
3. In the Discounting of Usance Bills (Export LCs) screen, enter values in the mandatory and other required fields.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Validate icon to check for errors and overrides.
6. Click the Commit icon to submit the record.

This menu allows the user to discount the mixed type of drawings.

To discount the mixed type of drawings, follow the below steps:

1. Mixed Bills Negotiation/Discounting .
2. In the Negotiate/Discount Mixed payment (Export) screen, click the Amend icon.
3. In the Negotiate/Discount Mixed Bills (Export) screen, enter or modify values in the required fields.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Validate icon to check for errors and overrides.
6. Click the Commit icon to submit the record.

This menu allows the user to amend a sight drawing, which is discounted or negotiated. The amendment includes the extension of maturity date with (or without) a change in the discount rate from an effective date or doing an early maturity online.

To amend a discounted sight bill, follow the below steps:

1. Amendment to Sight Discounting .
2. In the List of Discounted Sight Bills under Export LC screen, click the Discounting icon corresponding to a record.
3. In the Amendment to Bill Purchased/Discounted screen, enter values in the mandatory and other required fields.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Validate icon to check for errors and overrides.
6. Click the Commit icon to submit the record.

This menu allows the user to amend a usance drawing, which is already discounted or negotiated. The amendment includes the extension of maturity date with (or without) a change in the discount rate from an effective date or doing an early maturity online.

To amend a discounted usance bill, follow the below steps:

1. Amendment to Usance Discounting .
2. In the Discounted Usance Bills under Export LC screen, click the Amendment icon corresponding to a record.
3. In the Amendment to Usance Bills Discounted screen, enter or modify values in the required fields.
4. Click the Delivery Preview icon corresponding to a record.
5. Click the Validate icon to check for errors and overrides.
6. Click the Commit icon to submit the record.

This menu allows the user to amend a mixed payment drawing, which is already discounted or negotiated. The amendment includes the extension of maturity date with (or without) a change in the discount rate from an effective date or doing an early maturity online.

To amend a discounted mixed payment bill, follow the below steps:

1. Amendment for Mixed Payment Discounting .
2. In the Discounted Mixed Payment Bills (Export) screen, click the Amendment icon corresponding to a record.
3. In the Amendment to Mixed Payment Discounting screen, enter or modify values in the required fields.
4. Click the Validate icon to check for errors and overrides.
5. Click the Delivery Preview icon to preview the delivery messages.
6. Click the Commit icon to submit the record.


#### 📊 Outputs

There are no Outputs available for Post-shipment Finance feature.

---


### 2.17  Pre-shipment Finance


> **📇 Quick Reference Card**
> 
> **Purpose:** *Temenos Transact facilitates the pre-shipment finance by granting the beneficiary an export loan or packing credit. The export loan or packing credit is extended to the exporter to handle manufacturing and packing cost of the goods meant for exports.*
> 
> **Key Fields:** *Category*, *Currency*, *Customer Id*, *Limit Reference*, *Negotiate/Discount Sight Bill (Export)*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Temenos Transact facilitates the pre-shipment finance by granting the beneficiary an export loan or packing credit. The export loan or packing credit is extended to the exporter to handle manufacturing and packing cost of the goods meant for exports.

These export loans are adjusted from the proceeds of the export bills covering the related shipment or consignment.


#### ⚙️ Configuration

LOANS.AND.DEPOSITS module is used to facilitate loan transaction.


#### 📋 Tasks

Related topics:

- Perform Past Due Write-Off
- Provide Export Financing
- Lending Processes (Corporate)

Pre-shipment finance also known as Packing Credit, refers to the credit extended to the small scale manufacturers or exporters, who do not possess sufficient financial resources to meet the expenditure involved in production of goods, prior to the shipment of goods for the execution of export order. It refers to any loan granted to an exporter for the purchase, processing and manufacturing or packing of goods.


##### Workflow

The user can provide pre-shipment financing using the below workflow:

| SCREENS | WORKFLOW |
|---|---|
|  | Create Export Packing Credit Account . |
| Contract Screen | Click the New icon. |
| Export Packing Credit Account | Enter values in the following mandatory fields: Limit Reference Customer Id Currency Category Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

| SCREENS | WORKFLOW |
|---|---|
|  | Create Export Packing Credit Limit . |
| Contract Screen | Click the New icon. |
| Export Packing Credit Limit | Enter values in the required fields. Click the Delivery Preview icon to view the delivery messages. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

| SCREENS | WORKFLOW |
|---|---|
|  | Create Export Packing Credit Loan . |
| Contract Screen | Click the New icon. |
| Input Export Packing Credit Loan | Enter values in the mandatory and other required fields. Click the Delivery Preview icon to view the delivery messages. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

| SCREENS | WORKFLOW |
|---|---|
|  | Sight Negotiation-Adjustment of EPC . |
| Contract Screen | Select a value in the Negotiate/Discount Sight Bill (Export) field drop-down. Click the Edit icon. |
| Negotiate/Discount Sight Bill (Export) | Enter values in the mandatory and other required fields. Click the Delivery Preview icon to view the delivery messages. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |

| SCREENS | WORKFLOW |
|---|---|
|  | Sight Negotiation-Adjustment of Loan . |
| Contract Screen | Select a value in the Negotiate/Discount Sight Bill (Export) field drop-down. Click the Edit icon. |
| Negotiate/Discount Sight Bill (Export) | Enter values in the mandatory and other required fields. Click the Delivery Preview icon to view the delivery messages. Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |


#### 📊 Outputs

There are no Outputs available for Pre-shipment Finance feature.

---


### 2.18  Pre advice of a LC


> **📇 Quick Reference Card**
> 
> **Purpose:** *The pre-advice is for information purposes and not a legally binding contract. The terms and conditions can be changed or amended later, when the actual Letter of Credit (LC) is opened. Only irrevocable LC becomes a binding contract on the issuing bank. The issuing bank sends a MT705 to the advising...*
> 
> **Sections:** 📖 Introduction | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The pre-advice is for information purposes and not a legally binding contract. The terms and conditions can be changed or amended later, when the actual Letter of Credit (LC) is opened. Only irrevocable LC becomes a binding contract on the issuing bank. The issuing bank sends a MT705 to the advising bank.


##### SWIFT 2023 Changes for MT705

As a part of the changes in SWIFT Regulation 2023, the length of the below mentioned fields is increased from 65x to 140z for MT705.

| Tag | SWIFT Tag Name |
|---|---|
| 44A | Place of Taking in Charge/Dispatch from.../Place of Receipt |
| 44B | Place of Final Destination/For Transportation to.../Place of Delivery |
| 44E | Port of Loading/Airport of Departure |
| 44F | Port of Discharge/Airport of Destination |


#### 📋 Tasks

Related topics:

- Issue Import LC
- Pre-Advice Import LC
- Trade Finance and Guarantees Processes
- Corporate Pre-Advise Import LC

A pre-advice is a brief advice of documentary credit sent by the Issuing Bank to the Advising Bank. It is for the information purpose and not a legally binding contract. At the request of an applicant, the issuing bank may give a pre-advice of issuance and/or amendment of the letter of credit. A Pre-advice is usually marked with a reference such as “full details to follow”.

The terms and conditions can be changed or amended later, when the actual Letter of Credit (LC) is opened. Only irrevocable LC becomes a binding contract on the issuing bank. The issuing bank sends MT705 to the advising bank for Pre-advice of Import LC.


##### Workflow

The user can create and register a Pre-advice of import and export LCs using the below workflow:

This menu allows the user to issue an import LC Pre Advice.

To issue an import LC Pre Advice, perform the below steps:

1. Pre Advice of Import LCs .
2. In the Import LC Pre Advice screen, enter values in the mandatory and other required fields.
3. Click the Delivery preview (opens in new window) icon to view the delivery messages.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.

This menu allows the user to issue a LC for a Pre Advised Import LC.

To issue a LC for Pre Advised Import LC, perform the below steps:

1. Pre Advice to Issue/List of Preadvised LCs .
2. In the List of Pre-Advised Import LCs screen, click the Pre Advice to Issu e icon corresponding to a record.
3. Enter values in the required fields.
4. Click the Delivery preview (opens in new window) icon to view the delivery messages.
5. Click the Validate icon to check for the errors and overrides.
6. Click the Commit icon to submit the record.

This menu allows the user to register an export LC Pre Advice.

To register an export LC Pre Advice, perform the below steps:

1. Pre Advice .
2. In the Export LC Pre Advice screen, enter values in the mandatory and other required fields.
3. Click the Delivery preview (opens in new window) icon to view the delivery messages.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.

This menu allows the user to register LC for a Pre Advised Export LC.

To register a LC for a Pre Advised Export LC, perform the below steps:

1. PreAdvice to Advice/List of Preadvised LCs .
2. In the List of Pre-Advised Export LCs screen, click the PreAdvice to Advice icon corresponding to a record.
3. Enter values in the required fields.
4. Click the Delivery preview (opens in new window) icon to view the delivery messages.
5. Click the Validate icon to check for the errors and overrides.
6. Click the Commit icon to submit the record.


#### 📊 Outputs

Once the Pre-advice of LC is authorised, the user can view the below delivery messages.


##### Enquiries and Reports

NA


##### SWIFT Messages

Below list of SWIFT Messages are triggered by the core banking system for Pre Advice of LC.

MT705 is a brief advice of a documentary credit where the full details of the message follows through the MT700.


##### Advices

The below list of advices are generated by the core banking system pertaining to Pre-advice of a LC..

After authorising the pre-advice LC, the below delivery message is sent to applicant.

Below delivery message generates after authorising the issuance of a LC from a pre-advice LC.

Banks receives the Pre-Advice of the LC before the receipt of the actual LC from the issuing bank. Below advice generates when the user register the received pre-advice LC.

Below advice generates when the user converts the pre-advice LC to advice of export LC.


##### Alerts

NA

---


### 2.19  Reversal or Cancellation


> **📇 Quick Reference Card**
> 
> **Purpose:** *The applicant can initiate a request for reversal or cancellation of import LC. It can be initiated by beneficiary or any other parties in the LC (provided there is an agreement to reverse or cancel the LC by all other parties).*
> 
> **Key Fields:** *Cancellation Request*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The applicant can initiate a request for reversal or cancellation of import LC. It can be initiated by beneficiary or any other parties in the LC (provided there is an agreement to reverse or cancel the LC by all other parties).


#### ⚙️ Configuration

Reversal or cancellation of LC feature has no specific configuration to be setup. The parameter tables are setup at the implementation stage.


#### 📋 Tasks

Related topics:

- Amend Import LC
- Cancel Import LC
- Trade Finance and Guarantees Processes

Cancellation of an import LC can be done on applicant’s request and the cancellation of the credit should be intimated to the beneficiary through the advising bank.


##### Workflow

In Reversal and Cancellation, the user can perform the below activity:

The user can cancel or reverse an import LC.

To cancel an import LC, perform the below steps:

1. Reversal/Cancellation of Import LC .
2. In the Import LC screen, click the Cancel icon corresponding to a record.
3. In the Reversal/Cancellation of Import LC screen, enter values in the required fields.
4. Click the Validate icon to check for errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages and then click the Commit icon to cancel the import LC.

To reverse an import LC, perform the below steps:

1. Reversal/Cancellation of Import LC .
2. In the Import LC screen, click the Reverse icon corresponding to a record.
3. In the Reversal/Cancellation of Import LC screen, click the Reverse icon.

This menu allows the user to cancel or reverse an Export LC.

To cancel an Export LC, follow the below steps:

1. Reversal/Cancellation of Export LC .
2. In the Export LC screen, click the Cancel icon corresponding to a record.
3. In the Reversal/Cancellation of Export LC screen, select the Cancel option in the Cancellation Request field and enter values in the other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to preview the delivery messages.
6. Click the Commit icon to cancel the Export LC.

To reverse an import LC, follow the below steps:

1. Reversal/Cancellation of Export LC .
2. In the Export LC screen, click the Reverse icon corresponding to a record.
3. In the Reversal/Cancellation of Export LC screen, click the Reverse icon.


#### 📊 Outputs

There are no Outputs available for Reversal/Cancellation feature.

---


### 2.20  RMA Verification


> **📇 Quick Reference Card**
> 
> **Purpose:** *This section explains about Relationship Management Application (RMA) verification in Transact.*
> 
> **Applications:** `DRAWINGS`, `LC`, `LC.AMENDMENTS`, `PP.RMA`
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

This section explains about Relationship Management Application (RMA) verification in Transact.

When a user initiates any MT7XX and MT4XX series SWIFT message for LC Deals, the Temenos system conducts an RMA verification. This check allows the user to determine if Temenos model bank has an RMA with the receiver of the SWIFT message for any LC Deal and if the messageis delivered.

The system performs this verification at field-level in any deal, that is, if the user generates multiple MT7XX SWIFT messages, the system checks for each recipient individually. If RMA is not available, it posts an override message for each check. This verification is conducted based on both Customer ID and SW-‘BIC’ entered by the user.

Once the user commits the LC (including LC , LC.AMENDMENTS , DRAWINGS ) and has any MT7XX or MT4XX SWIFT messages to send, the system consults PP.RMA using the existing DE.CHECK.RMA API (either from the entered customer ID or SW-‘BIC’). If RMA is available, the system proceeds without any override; otherwise, it raises a specific override on the mentioned fields.


#### ⚙️ Configuration

RMA Verification has no specific configuration to be setup. The parameter tables are setup at the implementation stage.


#### 📋 Tasks

There are no Tasks available for RMA Verification feature.


#### 📊 Outputs

There are no Outputs available for RMA Verification feature.


> **Related Applications:** `DRAWINGS`, `LC`, `LC.AMENDMENTS`, `PP.RMA`

---


### 2.21  Shipping Guarantee


> **📇 Quick Reference Card**
> 
> **Purpose:** *A guarantee is issued in favour of a shipping company where the goods have arrived at the destination port but the original documents of title (bill of lading) under the Letter of Credit (LC) has not been received. It is issued without reference to amount or expiry and is only cancelled upon the del...*
> 
> **Key Fields:** *Drawing Type*, *Reduce Lc Liab*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

A guarantee is issued in favour of a shipping company where the goods have arrived at the destination port but the original documents of title (bill of lading) under the Letter of Credit (LC) has not been received. It is issued without reference to amount or expiry and is only cancelled upon the delivery of the original bill of lading to the shipping company.

A Shipping Guarantee (SG) is issued by the bank for sea shipments, at the request of the importer customer to enable clearance of goods in circumstances, where the vessel or flight carrying the goods arrives prior to receipt of original title documents and the goods are consigned to the bank.

When issuing a SG, the bank incurs a liability in respect of loss of control over the goods. A Delivery Order (DO) is issued for air shipments.


#### ⚙️ Configuration

The below field in MD.PARAMETER is setup.

Reduce Lc Liab – Accepts values Yes or No. It shifts the liability from Letter of Credit (LC) to guarantee.


#### 📋 Tasks

Related topics:

- Issue Shipping Guarantee Against Import Collection

Under Letter of Credit transactions, when the goods arrive at the buyer's country before the receipt of documents, a shipping guarantee against the import Letter of Credit is issued at the request of the buyer to take possession of the goods to avoid demurrage and other charges.

In the Temenos Transact, when shipping guarantee is issued against import Letter of Credit, user options are available to shift the liability from Letter of Credit to Guarantee or update the guarantee liability in addition to Letter of Credit liability.


##### Workflow

The user can create a shipping guarantee using the below workflow:

This menu allows the user to create shipping guarantee under drawings.

To create a shipping guarantee under drawings, follow the below steps:

1. Drawings Under Shipping Guarantee .
2. In the Drawings Created but document not received under Shipping Guarantee Screen, click the Pay/Accept SG Drawings icon.
3. In the Acceptance under Import LC screen, select the SG option in the Drawing Type field and enter values in the other required fields.
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon to submit the record.


#### 📊 Outputs

There are no Outputs available for Shipping Guarantee feature.

---


### 2.22  Shipping Guarantee against Import Collection


> **📇 Quick Reference Card**
> 
> **Purpose:** *When the goods arrive at the buyer’s country before the receipt of import collection documents, banks issue Shipping Guarantee (SG) against import collection documents in Letter of Credit (LC) transactions. This is done at the request of the customer by collecting cash margin up to or more that 100%...*
> 
> **Key Fields:** *Reduce Lc Liab*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

When the goods arrive at the buyer’s country before the receipt of import collection documents, banks issue Shipping Guarantee (SG) against import collection documents in Letter of Credit (LC) transactions. This is done at the request of the customer by collecting cash margin up to or more that 100% of the document value.


#### ⚙️ Configuration

Reduce Lc Liab – This field in MD.PARAMETER enables the bank to shift the liability from LC to guarantee. Allowed values are Yes or No.

This feature has no other specific configuration to be set up at feature level. The parameter tables are set up at the implementation stage.


#### 📋 Tasks

Related topics:

- Issue Shipping Guarantee Against Import Collection

There are no Tasks available for Shipping Guarantee against Import Collection feature.


#### 📊 Outputs

There are no Outputs available for Shipping Guarantee against Import Collection feature.

---


### 2.23  Syndicated Letter of Credit


> **📇 Quick Reference Card**
> 
> **Purpose:** *One of the main instruments of payment used in international trade is the Letter of Credit (LC). It offers all parties to the transaction a much more secure transaction than clean payment or documentary collection. Corporates require finance (in the form of LC) running into many millions of dollars ...*
> 
> **Key Fields:** *Synd Chg Code*, *Syndicate Charge*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

One of the main instruments of payment used in international trade is the Letter of Credit (LC). It offers all parties to the transaction a much more secure transaction than clean payment or documentary collection. Corporates require finance (in the form of LC) running into many millions of dollars and in such case a bank approach other lenders with the aim of creating a syndicated transaction.

Hence, a syndicated facility is granted to the customer and the facility agreement states the products for which the facility is used. For example, loans, guarantees, standby LC or documentary LC. The customer can choose to draw a loan or to issue a guarantee or a standby LC or a documentary LC.

Syndicated LC agreements can be arranged for corporate customers. Also, a bank may have a facility agreed to syndicate Issuing bank risk under export LC where the agent bank (arranger) syndicates their confirmation liability.


#### ⚙️ Configuration

The bank collects charges that are common for bank and participant banks in a syndicated LC. In such cases, the commission collected is split between the agent bank and its participant.


##### Synd Chg Code

This field in LC.PARAMETER enables the splitting of commission between the agent bank and its participants.

- Defines the charges that needs to be split
- Syndicates only the charges defined in this field
- This is a multi-value field and the bank can define more than one type of charge or commission
- At the LC level, Syndicate Charge field is set to Yes, to syndicate the charges
- Allows the user to enter a valid FT.COMMISSION.TYPE or FT.CHARGE.TYPE ID and these specific charges work in conjunction with the Syndicate Charge field
- When Syndicate Charge in LC is set to Yes, the system checks if respective charge code is specified in Synd Chg Code of LC.PARAMETERS


#### 📋 Tasks

There are no Tasks available for Syndicated Letter of Credit feature.


#### 📊 Outputs

There are no Outputs available for Syndicated Letter of Credit feature.

---


### 2.24  TBML Check for Letter of Credit


> **📇 Quick Reference Card**
> 
> **Purpose:** *Trade finance encompasses the provision of financial services to facilitate trade activities, whether conducted domestically or internationally. These transactions typically involve both a seller, offering goods or services, and a buyer. Various intermediaries, including banks and other financial in...*
> 
> **Applications:** `DIPO.ITEMS`, `DISPO.ITEMS`
> 
> **Key Fields:** *Status*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Trade finance encompasses the provision of financial services to facilitate trade activities, whether conducted domestically or internationally. These transactions typically involve both a seller, offering goods or services, and a buyer. Various intermediaries, including banks and other financial institutions, play a crucial role in enabling these transactions by providing financial support.

Trade finance operations encompass a range of activities such as lending, issuing letters of credit, factoring, export credit, and insurance. Entities involved in trade finance include importers and exporters, financial institutions like banks and financiers, insurers, export credit agencies, and additional service providers such as tax agents, legal advisors, and trade mediators. Some forms of trade finance are tailored to complement traditional financing methods, offering additional support to facilitate smooth trade operations.

TBML, or Trade-Based Money Laundering, has gained widespread usage, encompassing a diverse range of services and products, among them those commonly known as Trade Finance.

Letter of Credit (LC) is a formal document in which the importer's bank extends credit to the importer and undertakes the responsibility of paying the exporter. Specifically, at the importer's request, the importer's bank disburses a specified sum to a named beneficiary upon the presentation of predetermined documents outlined in the terms and conditions of the LC.

This documentary credit arrangement provides a globally recognised method of obtaining a commercially acceptable commitment by facilitating payment when the documentation representing the goods is presented, thereby enabling the transfer of title to those goods. The true value of goods transferred between countries can be obscured through misrepresentation of price, quantity, and quality. Letters of Credit can be exploited to create a facade, as the documentation generated in the process creates a paper trail that money launderers can exploit to disguise illicit proceeds.

Regarding trends and developments in trade-based money laundering (TBML), criminals exploit sectors, products, or businesses susceptible to gaps or inconsistent application of customer due diligence and know-your-customer processes across jurisdictions. This section explores trends in economic sectors and products vulnerable to TBML activities. It highlights a wide range of sectors, including both high-value, low-volume products like precious metals, and low-value, high-volume products like second-hand textiles, which criminals exploit to launder illicit proceeds. Common themes conducive to TBML exploitation include goods with wide pricing margins, extended trade cycles involving multiple jurisdictions, and goods challenging for customs authorities to inspect. Supply chains moving lower-value goods are particularly susceptible to end-to-end ownership.


#### ⚙️ Configuration

The TRANSACT trade finance application communicates with the TRANSACT FCM through the utilisation of DISPO.ITEMS . Read FCM Architecture and Design for more information on the FCM architecture and design.

The fields and inquiries can be employed to configure and engage with any external TBML engines.


#### 🔧 Working With

This functionality allows the transmission of a trade finance transaction to TBML to be carried out by the bank user across various workflows associated with trade finance products.

The workflow enabled for TBML check involves conducting checks at various stages of trade finance transactions to mitigate risks associated with Trade-Based Money Laundering (TBML). The following workflows are specifically enabled for TBML checks:


##### Issuance of Import/Export LC

During the issuance of Import/Export Letters of Credit (LC), banks perform TBML checks to ensure compliance with regulations and prevent illicit activities. This includes verifying the legitimacy of the parties involved, scrutinising the documentation provided, and assessing the underlying trade transactions for any suspicious activities.


##### Amending (External) Letter of Credit

When amendments are made to existing Letters of Credit, TBML checks are conducted to verify the validity and necessity of the amendments. This involves reviewing the proposed changes, assessing their impact on the transaction, and ensuring compliance with regulatory requirements to prevent potential TBML activities.


##### Drawings or Presentation under Letter of Credit

TBML checks are carried out during the process of drawings or presentation under Letters of Credit. Banks verify the authenticity of presented documents, confirm adherence to LC terms and conditions, and scrutinise the underlying trade transactions for any indications of TBML. This includes examining invoices, bills of lading, certificates of origin, and other relevant documents to detect any discrepancies or anomalies that may raise concerns related to money laundering.

By incorporating TBML checks into these critical workflows, banks aim to enhance transparency, ensure regulatory compliance, and mitigate the risks associated with illicit financial activities in trade finance transactions. These checks contribute to safeguarding the integrity of the financial system and maintaining trust in trade finance.


##### Payload Sent to FCM During Different Events of FCM Contact Points

Payloads transmitted to FCM vary depending on the different events occurring at FCM contact points. These events, along with their corresponding payload and date type, are as follows:

| Payload | Data Type | Multi Value |
|---|---|---|
| DEAL REFERENCE | Text | N |
| APPLICATION NAME | LETTER.OF.CREDIT | N |
| LC.AMOUNT | Number | N |
| APPLICANT.BANK | Customer ID/Text | N |
| APPLICANT.CUSTNO | Customer ID/Text | N |
| APPLICANT | Text | N |
| BENEFICIARY.CUSTNO | Text | N |
| BENEFICIARY | Customer ID/Text | N |
| ADVISING.BK.CUSTNO | Customer ID/Text | N |
| ADVISING.BK | Customer ID/Text | N |
| ADVISE.THRU.CUSTNO | Customer ID/Text | N |
| ADVISE.THRU | Customer ID/Text | N |
| AVAIL.WITH.CUSTNO | Customer ID/Text | N |
| AVAILABLE.WITH | Customer ID/Text | N |
| THIRD.PARTY.CUSTNO | Customer ID/Text | N |
| THIRD.PARTY | Customer ID/Text | N |
| REQ.CONF.BNK | Customer ID/Text | N |
| REQ.CONF.BNK.NAME | Customer ID /Text | N |
| ASSN.CUSTNO | Customer ID /Text | Y |
| ASSN.ADD | Text | N |
| RISK.PARTY | Customer ID | Y |
| SHIP.DESPATCH | Text | N |
| OTHER.DESPATCH.DET | Text | N |
| TRANSPORTATION | Text | N |
| FINAL.DESTINATION | Text | N |
| LC.CURRENCY | Text | N |
| DRAWEE.CUST.NO | Customer ID/Text | N |
| DRAWEE | Customer ID/Text | N |
| ISSUING.BANK.NO | Customer/ Text | N |
| ISSUING.BANK | Text | N |
| NON.BANK.ISSUER.ID | Customer/ Text | N |
| NON.BANK.ISSUER | Text | N |
| NEG.WITH.BANK | Customer ID/Text | N |
| AVAIL.CUSTNO | Customer ID | N |
| AVAIL.CUST | Text | N |
| DATE.TIME (Audit) | Date/ Text | N |
| FCM Field | Text | N |

The payloads contain various information such as customer IDs, text data, and other relevant details, aiding in the communication and processing of trade finance transactions within the FCM system.

The following are examples of triggering a TBML for Issuance of Import LC.

To trigger a TBML for Issuance of Import LC,

- Input the Contract details for the Issuance of Import LC.
- Check the FCM Enable checkbox to trigger the transaction for TBML check.
- Once the transaction is committed, an override is displayed to show the contract is sent for FCM check.
- The transactions transmitted through FCM are monitored using a specialised inquiry to display the trade transactions for FCM, which can be accessed for viewing.
- Transactions are segregated based in the Status field in the DIPO.ITEMS application. The workflow is applied for all trade finance applications.
- Once a transaction undergoes an FCM check, the FCM engine typically responds with one of three outcomes: Approved Rejected Possible


#### 📋 Tasks

There are no Tasks available for the TBML Check for Letter of Credit feature.


#### 📊 Outputs

There are no Outputs available for the TBML Check for Letter of Credit feature.


> **Related Applications:** `DIPO.ITEMS`, `DISPO.ITEMS`

---


### 2.25  Tickler and Tracers


> **📇 Quick Reference Card**
> 
> **Purpose:** *Tracer is an inquiry message initiated from one bank to another to trace the documents, payments or its status. They are not part of LC cycle or collection process, but play an important role in the transaction life cycle of both LC and collections. In general, there is no specific message series fo...*
> 
> **Key Fields:** *Trace Date*, *Trace Date Req*, *Tracer Date*, *Tracer stat*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Tracer is an inquiry message initiated from one bank to another to trace the documents, payments or its status. They are not part of LC cycle or collection process, but play an important role in the transaction life cycle of both LC and collections. In general, there is no specific message series for tracers in LC, it is relayed through free format message type or the messages are covered under the existing 7xx series message type. Tracers are relayed through MT420 for collection transaction.

Tracers are sent to counter parties outside the bank. Ticklers are for internal maintenance. It is a diary event or a delegation tool. A user can schedule a tickler for, certain event(s), on certain date(s), to different receivers or the user or for any other person (assistants), setting the appropriate status for the said tasks. These tasks are broken into different applications. The supervisor monitors the progress of the tasks assigned by setting ticklers. The user extracts enquiries or reports to suit local requirements.


#### ⚙️ Configuration

- When a tracer is generated, the next tracer generation date is automatically decided using EB.FREE.PARAMETERS or COUNTRY tables.
- Tracer stat – Stops the schedules tracer anytime during the lifecycle, when this field in EB.FREE.MESSAGE is set to Stop.
- Tracer Date – Stops any scheduled tracer, when the date in this field is removed.
- EB.FREE.PARAMETERS has a company code as the ID. This field has to be set up mandatorily, if tracers are to be scheduled. A set of model routines are also released.

The below table details the Trace Date Req field:

| Field | Description |
|---|---|
| Trace Date Req | Tracer mechanism is mandatory for each discrepant type defined in DR.DISCREPANT.TYPE . When set to Yes, Trace Date field in DRAWINGS becomes mandatory and vice-versa. This field controls the Trace Date field in a DRAWINGS which uses this discrepant type. |


#### 📋 Tasks

There are no Tasks available for Ticklers and Tracers feature.


#### 📊 Outputs

There are no Outputs available for Ticklers and Tracers feature.

---


### 2.26  Trade Based Lending


> **📇 Quick Reference Card**
> 
> **Purpose:** *Trade based lending is fundamental to international trade, offering a range of financial instruments designed to streamline and secure cross-border transactions. Addressing the inherent risks associated with global commerce provides substantial benefits to both importers and exporters.*
> 
> **Applications:** `AA.ARRANGEMENT`, `DRAWINGS`
> 
> **Key Fields:** *Alternate Id*, *Transaction Reference*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Trade based lending is fundamental to international trade, offering a range of financial instruments designed to streamline and secure cross-border transactions. Addressing the inherent risks associated with global commerce provides substantial benefits to both importers and exporters.

Below are the advantages of trade based lending.

- Targeted financing: Trade based lending supplies essential working capital throughout the trade cycle, facilitating efficient procurement, production, and collection of receivables.
- Risk mitigation: It reduces risks such as non-payment, fraud, and shipment discrepancies by using instruments like letters of credit to ensure transaction security.
- Enhanced liquidity: By bridging the gap between payments and receipts, trade based lending significantly improves cash flow for businesses.

Unlike traditional loan structures, trade based lending focuses on the trade transaction and the creditworthiness of the goods involved.


#### ⚙️ Configuration

There is no specific configuration to be setup at feature level. The parameter tables are setup at implementation stage.


#### 🔧 Working With

This section explains the creation of trade loans, viewing loan arrangement and contract details.

Trade finance loans in AA framework enable the new loan products tailored for trade finance, rendering them negotiable for both import and export cycles.


##### Creating Trade Based AA Loan

The user can follow the below procedure to create a trade based AA loan.

1. Product Catalog .
2. Click and select New Arrangement to create a new arrangement as shown below.
3. Enter Alternate Id along with the mandatory fields required for the loan. Validate and commit the arrangement.


##### Viewing Loan Arrangement Details

The user can follow the below procedure to view the loan arrangement details.

1. Authorise/View Loan Details . This enquiry fetches outstanding loan arrangement details and the unauthorized loan details.
2. Enter the arrangement details in Transaction Reference or use the trade finance contract reference given in Alternate Id . The enquiry populates the loan arrangement that is linked to the transaction. In the below example, the enquiry populates two items as there are loans against LC and DRAWINGS .
3. Click to view the linked LC/ DRAWINGS record ( View Record ) or the loan arrangement ( View Arrangement ). Click View Record corresponding to LC record to view LC where the linked record ID is displayed. Click View Record corresponding to DRAWINGS record to view DRAWINGS where the linked record ID is displayed. Click View Arrangement to view AA.ARRANGEMENT where Alternate Id is displayed.


##### Viewing loan information for LC andDRAWINGScontracts

New contextual inquiries are available in LC and DRAWINGS to display the associated AA loan arrangement details, allowing the user to access loan information from the trade finance contracts when required.

View Loan Details as shown below.

View Loan Details as shown below.

> **⚠️ Note:** The LC reference is same as DRAWINGS but with extra integers. Hence the system displays, LC with LC and DRAWINGS records. DRAWINGS with DRAWINGS records.

A new overview screen created for Trade Finance Loans allows users to view the linked Alternate ID associated with the loan. This screen enables the execution of activities such as amending the principal, extending the due date, increasing the validity, processing prepayments, and more, as listed below.

> **⚠️ Note:** The Amendment Alternate ID is designed to support the capture of multiple Trade Finance Letters of Credit (LCs) and drawings during the tenure of the loan.


#### 📋 Tasks

There are no tasks available for Trade Based Lending feature.


#### 📊 Outputs

There are no outputs available for Trade Based Lending feature.


> **Related Applications:** `AA.ARRANGEMENT`, `DRAWINGS`

---


### 2.27  Trade Evidence For Advance Payment


> **📇 Quick Reference Card**
> 
> **Purpose:** *Advance payment method of trading is the popular method among both trade entities and the banks used for payment.*
> 
> **Key Fields:** *Amend Del*, *Drawings Type*, *Duplicate Check*, *Import Export*, *Operation Type*, *Pay type*, *Payment types*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Advance payment method of trading is the popular method among both trade entities and the banks used for payment.

- The parties to the contract choose an appropriate method of payment according to their needs.
- Importers pay the exporters (in full or partial) the value of the contract in advances before the goods are shipped to importers.
- Exporters thus avoid credit risk as the payment is received prior to the ownership of the goods.
- Banks intervene at the time of remittance and at the time of booking or registering the trade documents against the advanced payment as proof of shipment.

The advance payment cycle starts with the payments and ends with the documentary evidence submission against the payment reference. In Temenos Transact, the TF module supports booking of trade documents against the advance payments.

> **⚠️ Note:** Remittance is handled as part of Payments.


##### Advance Payment Cycle

The following section describes the steps involved in this payment method along with an illustration.

1. Firstly, a contract agreement is made between importers and exporters.
2. Outward remittances are made when the importer submits purchase order or pro-forma invoice to the importers’ bank for payment
3. The importer's bank sends MT103 to the exporter.
4. The exporter's bank receives the inward remittance and credits the beneficiary’s or exporter’s account.
5. The exporter dispatches all original shipping and commercial documents to the importer directly.
6. The exporter’s bank receives the copy of documents for booking and updates the inward remittances (advance payment) reference and closes the contract.
7. Similarly, the importer submits the copy of documents to the importer’s bank as evidence of import against the advance payment made and closes the contract.

There is no liability on the banks, they just act on the instruction from the importer or exporter to book the trade documents as proof of shipment with no risk or responsibility on its part.


#### ⚙️ Configuration

To configure a new LC.TYPES record that is specific to Advance Payments define the following fields:

1. Setup the default category code for each type of advance payment.
2. Set Import Export as I or E, to define if the record is export or import trade document
3. Set Pay type as P, for sight payment. No other Pay type is supported for advance payments.
4. Set Duplicate Check based on the Invoice number, Invoice date and Invoice amount fields in the LC module.
5. Set the rest of the fields as blank in LC.TYPES , implying that the record type does not pertain to Documentary LC or Documentary Collection.


#### 🔧 Working With

The LC application supports registering of contracts using advance payment method of payments. These contracts can be registered as import or export contracts with Operation Type set as AP.

Drawings Type OS is applied for registering the trade documents against the advance payment contracts in the LC application. That is, for P Payment types in LC.TYPES record, this defaults to OS (P for Payment).

> **⚠️ Note:** No other draw type is allowed for Operation Type with AP.

Any changes to the contract booked in the LC module, can be amended using A operation only. The Amend Del field is not applicable for advance payment contracts that is, only internal amendment is allowed implying only basic details can be changed.

- Banks act only on the instruction of the importer and exporter to register the trade documents against the advance remittances and do not hold any risk or responsibility on the contract. Hence no contingent accounting is raised or limits are not blocked.
- Advance remittances is handled out of the TF module.

The user is allowed to recover charges as defined in FT.COMMISSION.TYPE . Default charges can be defined in LC.TXN.TYPE.CONDITIONS based on LC.TYPES .

Temenos Transact supports recovery of upfront flat or fixed charges for handling advance payment trade documents.


#### 📋 Tasks

Related topics:

- Amend Advance Payment Trade (Import)
- Amend Advance Payment Trade (Export)
- Lodge Documents Against Advance Payment Trade (Export)
- Lodge Documents Against Advance Payment Trade (Import)

In Advance Payment method, importer pays the exporter in full or partial payment in advance based on the value of the contract before the goods are shipped to importers. Exporter avoids credit risk because payment received before the ownership of the goods are transferred.


##### Workflow

The Trade Finance Officer and Trade Finance Supervisor can process the Advance Payment Transactions using the below workflow:

This menu allows the user to lodge the import advance payment.

To process the lodging of import advance payment, follow the below steps:

1. Lodge Import Advance Payment .
2. In the Import Advance Payment screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Commit icon to submit the record.

This menu allows the user to lodge the export advance payment.

To process the lodging of export advance payment, follow the below steps:

1. Lodge Export Advance Payment .
2. In the Export Advance Payment screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Commit icon to submit the record.

This menu allows the user to amend the lodged import advance payment.

To process an amendment to import advance payment, follow the below steps:

1. Amend Import Advance Payment .
2. In the Advance payment screen, click the Amend icon for corresponding record to proceed with the transaction.
3. In the Amendment of Advance Payment screen, enter values in the mandatory fields and amend the required changes in the corresponding fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.

This menu allows the user to amend the lodged export advance payment.

To process an amendment to export advance payment:

1. Amend Export Advance Payment .
2. In the Advance payment screen, click the Amend icon for corresponding record to proceed with the transaction.
3. In the Amendment of Advance Payment screen, enter values in the mandatory fields and amend the required changes in the corresponding fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Commit icon to submit the record.

This menu allows the user to authorise or delete the lodged and amended import advance payment.

To authorise the lodged oramended import advance payment, follow the below steps:

1. Import Advance Payment Trading / Amendments .
2. In the Unauthorised Advance Payment Lodgement/Amendment screen, click the Authorise icon corresponding to a record.
3. Verify the transaction details and then click the Authorise icon to commit the authorisation.

To delete the lodged or amended import advance payment, follow the below steps:

1. Import Advance Payment Trading / Amendments .
2. In the Unauthorised Advance Payment Lodgement/Amendment screen, click the Delete icon corresponding to a record.
3. Click the Delete icon to commit the deletion.

This menu allows the user to authorise or delete the lodged or amended export advance payment.

To authorise the lodged or amended export advance payment, follow the below steps:

1. Export Advance Payment Trading / Amendments .
2. In the Unauthorised advance payment Lodgement/Amendment screen, click the Authorise icon corresponding to a record.
3. Verify the transaction details and then click the Authorise icon to commit the authorisation.

To delete the lodged or amended export advance payment, follow the below steps:

1. Export Advance Payment Trading / Amendments .
2. In the Unauthorised advance payment Lodgement/Amendment screen, click the Delete icon corresponding to a record.
3. Click the Delete icon to commit the deletion.


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to Trade Evidence for Advance Payments in the core banking system.


##### Enquiries and Reports

This section allows the user to view the list of enquiries and reports:

Import Document Lodged

This enquiry displays the list of lodged Import bills based on customer.

Export Document Lodged

This enquiry displays the list of lodged Export bills based on customer.

Billwise Payment Import

This enquiry displays the Import bill wise utilisation.

Billwise Payment Export

This enquiry displays the Export bill wise utilisation.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


---


## Chapter 3: Trade_Banking - MD


Trade_Banking - MD module of Temenos Transact


### Features in Trade_Banking - MD


| # | Feature | Sections |
|---|---------|----------|
| 3.1 | Amendment of Issued or Registered Guarantees | Intro, Tasks, Outpu |
| 3.2 | Cancel Reinstate Guarantee | Intro, Tasks, Outpu |
| 3.3 | Collateral | Intro, Confi, Tasks, Outpu |
| 3.4 | Commission and Charges | Intro, Tasks, Outpu |
| 3.5 | Expiry or Reinstate Expired Guarantee | Intro, Confi, Tasks, Outpu |
| 3.6 | Issue Register Guarantee | Intro, Tasks, Outpu |
| 3.7 | Managing External Requests | Intro, Confi, Tasks, Outpu |
| 3.8 | Margin or Provision | Intro, Confi, Tasks, Outpu |
| 3.9 | Misc | Intro, Outpu |
| 3.10 | Multi Party Guarantee | Intro, Tasks, Outpu |
| 3.11 | Non Extension Guarantee | Intro, Confi, Worki, Tasks, Outpu |
| 3.12 | Pay Reject Claim under Guarantee | Intro, Tasks, Outpu |
| 3.13 | Presentation under SBLC | Intro, Confi, Worki, Tasks, Outpu |
| 3.14 | Register Claim under Guarantee | Intro, Tasks, Outpu |
| 3.15 | Reimbursement Processing SBLC | Intro, Confi, Worki, Tasks, Outpu |
| 3.16 | RMA Verification | Intro, Confi, Tasks, Outpu |
| 3.17 | Standby Letterr of Credit | Intro, Confi, Worki, Tasks, Outpu |
| 3.18 | Syndicate Guarantee | Intro, Tasks, Outpu |
| 3.19 | TBML Check for Guarantee and SBLC | Intro, Confi, Worki, Tasks, Outpu |


### 3.1  Amendment of Issued or Registered Guarantees


> **📇 Quick Reference Card**
> 
> **Purpose:** *Underlying terms and conditions under a guarantee that has already been issued can be amended or varied, without variation in contract, discharging the guarantee and releasing the guarantor from its liability. A guarantee can be amended with or without the consent of the beneficiary. The guarantor, ...*
> 
> **Sections:** 📖 Introduction | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Underlying terms and conditions under a guarantee that has already been issued can be amended or varied, without variation in contract, discharging the guarantee and releasing the guarantor from its liability. A guarantee can be amended with or without the consent of the beneficiary. The guarantor, on behalf of the applicants requests, issues an amendment. If the role of the bank were to advise the amendment, then it would do without any delay to the beneficiary.


##### SWIFT 2021 Changes in Amendment Flow

As part of Swift Release 2021, SWIFT has also stipulated a new flow for Amendments, based on which the behavior for Issuance of Amendment has been modified. Unlike current functionality, wherein user modifies the existing value of relevant fields in deal directly, user to issue an amendment using a different set of fields to generate MT767 (and MT775 as applicable) from MD.DEAL . These values are stored in a dynamic system table known as MD.AMEND.HIST . User to wait until the Amendment Response MT787 is received from the Receiving Bank and then impact or overwrite the existing value in the deal. Based on this logic, the amendment cycle that has been revamped as part of SWIFT 2021 changes are depicted below.


##### SWIFT 2023 Changes in Amendment Flow

The following field for MT767 is available in Seq B to include the Advising Bank Reference.

| Status | Tag | Field Name | Content/Options |
|---|---|---|---|
| O | 23 | Advising Bank Reference | 16x |

The field length for 24G has been increased to 12*65z in both Seq B and C.


#### 📋 Tasks

Related topics:

- Issue Guarantee
- Amend Guarantee or Standby LC
- Trade Finance and Guarantees Processes

Amendment of guarantees allows the user to do changes in the issued or registered guarantees.

Amendment of guarantee can be internal amendment or external amendment. In case of an external amendment the changes are communicated to third parties, such as, advising bank or beneficiary through a generation of the message.


##### Workflow

The user can process the internet amend request using the below workflow:

This menu allows the user to amend a letter of guarantee that are raised by the corporate clients through Temenos Connect Internet Banking.

To approve the internet amendment request, follow the below steps:

1. Internet Amend Requests .
2. In the Pending with bank tab, click the Edit Record icon corresponding to a record.
3. Click the View Record icon to view the amendment request.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

To view the amendment request that are pending with the customer, follow the below steps:

1. Internet Amend Requests .
2. In the Pending with customer tab, click the View Record icon corresponding to an amendment request that is pending with the customer.

To edit the amendment request that are pending with the customer, follow the below steps:

1. Internet Amend Requests .
2. In the Pending with customer tab, click the Edit Record icon corresponding to a record.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

To process the internet amendment request, follow the below steps:

1. Internet Amend Requests .
2. In the Amendment under process tab, click the Edit Record icon to process the internet amendment request.
3. Click the View Record icon to view the internet amendment request.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to Amend or Reverse an issued guarantee.

To amend an issued guarantee, follow the below steps:

1. Amend/Reverse - Guarantee Issued .
2. In the Guarantees Issued screen, click the Amend icon corresponding to a record.
3. In the Amendment to Guarantee screen, enter the mandatory and other required field values.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

To reverse an issued guarantee, follow the below steps:

1. Amend/Reverse - Guarantee Issued .
2. In the Guarantees Issued screen, click the Reverse icon corresponding to a record.
3. Click the Reverse icon to reverse an issued guarantee record.

This menu allows the user to register the response of an issued guarantee amendment.

To respond to an amendment of an issued guarantee, follow the below steps:

1. Amendment Response To Guarantee Issued .
2. In the Amendment of Guarantees Issued screen, click the Amendment Response icon corresponding to a record.
3. In the Amendment Response to Guarantee screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon.

This menu allows the user to amend or reverse an amendment of guarantee received.

To process an amendment for the guarantee received, follow the below steps:

1. Amendment to Guarantee Received .
2. In the Guarantees Received screen, click the Amend icon for corresponding record to proceed with the transaction.
3. In the Amendment to Guarantee Received screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon.

To reverse an amendment for the guarantee received, follow the below steps:

1. Amendment to Guarantee Received .
2. In the Guarantees Received screen, click the Reverse icon corresponding to a record.
3. Click the Reverse icon to reverse a received guarantee record.

This menu allows the user to respond to an amendment of a received guarantee.

To respond to an amendment of a received guarantee, follow the below steps:

1. Amendment Response To Guarantee Received .
2. In the Amendment of Guarantees Received screen, click the Amendment Response icon corresponding to a record.
3. In the Amendment Response to Guarantee Received screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon.

This menu allows the user to respond to an amendment of an advised guarantee.

To respond to an amendment of an advised guarantee, follow the below steps:

1. Amendment Response To Guarantee Advised .
2. In the Amendment of a Guarantees Advised screen, click the Amendment Response icon corresponding to a record.
3. In the Amendment Response to Guarantee screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon.


#### 📊 Outputs

Amendment of guarantees allows the user to do any changes in issued or registered guarantees. Amendment of guarantee can be internal amendment or external amendment. In case of an external amendment the changes are communicated to third parties, such as, advising bank or beneficiary through a generation of the message.


##### Enquiries and Reports

NA


##### SWIFT Messages

The user can view the below SWIFT messages:

This message is sent by the guarantee issuing bank to the counter-party bank to advise an amendment to the guarantee. This message is generated while making an amendment to a guarantee.

This message is sent by a bank which has received the guarantee to the bank that had issued the guarantee. It may also be sent by a bank which has been requested to issue a guarantee to the bank that requested the issuance of the guarantee.

This is a free format message and it is sent when the existing message types or tags are inadequate or inappropriate for a particular situation.

This message is sent by the guarantee issuing bank to the counter-party bank as an extension of MT767.

This message is sent to the bank that issued the undertaking amendment, either directly or through one or more advising parties, to indicate acceptance or rejection by the beneficiary of the amendment.


##### Advices

The below list of advices are generated by the core banking system pertaining to amendment of issued or registered guarantees.

The below advice is sent to customer for releasing the provision related to the guarantee.

The below advice is sent to the customer for amending the bank guarantee on their request.

The below advice is sent to the customer while performing the guarantee invocation.

The below advice is sent to beneficiary to advice the cancellation of claim under inward guarantee.


##### Alerts

NA

---


### 3.2  Cancel Reinstate Guarantee


> **📇 Quick Reference Card**
> 
> **Purpose:** *Bank guarantees issued by banks may be cancelled for various reasons. A reverse function is used to cancel such guarantees issued. Also, when a contract is expired, the guarantee needs to be reinstated.*
> 
> **Sections:** 📖 Introduction | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Bank guarantees issued by banks may be cancelled for various reasons. A reverse function is used to cancel such guarantees issued. Also, when a contract is expired, the guarantee needs to be reinstated.


#### 📋 Tasks

Related topics:

- Issue Guarantee
- Reinstate Expired Guarantees
- Trade Finance and Guarantees Processes

Cancellation of a Guarantee can be done on applicant’s request and the cancellation of the credit should be intimated to the beneficiary through the advising bank. Reinstatement is the guarantee shall be continue to be effective.


##### Workflow

The Trade Finance Officer can reinstate the Guarantee transactions using the workflow below:

This menu allows the user to reinstate the guarantee which is not in effect.

To reinstate a guarantee, follow the below steps:

1. Reinstate Liquidated Guarantees .
2. In the Reinstate Liquidated Guarantees screen, click the Amend icon for corresponding record to proceed with the transaction.
3. In the Reinstate Guarantee screen, enter values in the mandatory fields and set the Reinstate Guarantee option.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to cancel a shipping guarantee.

To cancel a shipping guarantee, follow the below steps:

1. Cancellation of Shipping Guarantee .
2. In the Cancel Shipping Guarantee screen, enter values in the mandatory fields.
3. Click the Validate icon to check for errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.


#### 📊 Outputs

There are no Outputs available for Cancel or Reinstate Guarantees.

---


### 3.3  Collateral


> **📇 Quick Reference Card**
> 
> **Purpose:** *Guarantees received as personal and corporate guarantees can be used as collateral for assistance provided to customers.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Guarantees received as personal and corporate guarantees can be used as collateral for assistance provided to customers.


#### ⚙️ Configuration

The COLLATERAL.TYPE and COLLATERAL.CODE applications are set up during implementation to indicate different collateral types to be used by the bank. Suitable records are created to cover guarantees, by including the MD application in the COLLATERAL.TYPE .


#### 📋 Tasks

There are no Tasks available for Collateral feature.


#### 📊 Outputs

There are no Outputs available for Collateral feature.

---


### 3.4  Commission and Charges


> **📇 Quick Reference Card**
> 
> **Purpose:** *Banks collect guarantee fee based on the assumption of risk that carries the guarantee.*
> 
> **Key Fields:** *Transaction Ref*
> 
> **Sections:** 📖 Introduction | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Banks collect guarantee fee based on the assumption of risk that carries the guarantee.

Financial guarantee carries more risk and is charged at higher rate when compared to performance guarantee, which carries less risk.

Besides, banks also collect processing and handling charges.


#### 📋 Tasks

Related topics:

- Register Claims
- Amend Import LC
- Issue Import LC
- Trade Finance and Guarantees Processes

The Miscellaneous Deals application allows the user to take the commission and charges at the time of guarantee issuance or advising or at any time afterwards.

Guarantee fee is a sum paid to the issuer of a mortgage-backed security. It helps the issuer pay the administrative costs and other expenses. Guarantee fees is also charged by guarantors for the services rendered. It can be either a percentage of the asset value or a fixed amount.


##### Workflow

This section allows the user to view the below enquiries and reports:

| SCREENS | WORKFLOW |
|---|---|
|  | Guarantee Claimed Commission Settlement . |
| Guarantee Commission Claimed | Enter a value in the Transaction Ref field and click the FIND button. |
| Guarantee Commission Claimed but not Settled | Click the Settle Claim icon corresponding to a record. |
| Settlement of Guarantee claimed Commission screen | Enter values in the mandatory and applicable fields. |
| Settlement of Guarantee claimed Commission screen | Click the Validate icon to check for errors and overrides. Click the Delivery Preview icon to view the delivery messages. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Guarantee Commission Refund . |
| Guarantee Commission Claimed | Enter a value in the Transaction Ref field and click the FIND button. |
| Commission Collected on Guarantees | Click the Refund Commission icon corresponding to a record. |
| Refund of Commission | Enter values in the mandatory and applicable fields. Click the Validate icon to check for errors and overrides. Click the Delivery Preview icon to view the delivery messages. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Writeoff of Uncollected Commission . |
| Unsettled Guarantee Commission | Click Writeoff icon for corresponding to a record. |
| Write off Unsettled Commission | Enter values in the mandatory and applicable fields. Click the Validate icon to check for errors and overrides. Click the Delivery Preview icon to view the delivery messages. Click the Commit icon. |

This menu allows the user to refund guarantee charges.

To refund the guarantee charges, follow the below steps:

1. Refund of Guarantee Charges .
2. In the Charges Collected on Guarantees screen, click the Refund icon corresponding to a record.
3. In the Refund Of Charges screen, enter values in the mandatory fields.
4. Click the Validate icon to check for errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This enquiry allows the user to change commission for the guarantee issued.

To process the commission rate change, follow the below steps:

1. Change Commission Rate .
2. Enter the required field values, in the CSN Comm Rate Change screen.
3. Click the Validate icon to check for errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.


#### 📊 Outputs

Banks collect guarantee fee based on the assumption of risk that carries the guarantee.

For example, financial guarantee carries more risk and is charged at higher rate when compared to performance guarantee, which carries less risk. Banks can also collect processing and handling charges.


##### Enquiries and Reports

NA


##### SWIFT Messages

NA


##### Advices

The below list of advices are generated by the core banking system pertaining to Commission and Charges.

The below advice is generated when the user performs payment of invocation from the customer account.

The below advice is generated when the user collects the charges on the guarantees.

The below advice is when the user collects margin during the guarantee issuance.


##### Alerts

NA

---


### 3.5  Expiry or Reinstate Expired Guarantee


> **📇 Quick Reference Card**
> 
> **Purpose:** *When a guarantee expires, the liability of the bank to pay under the guarantee becomes void. The bank is no more liable to pay the beneficiary in case of demand. Ideally, the bank guarantee should not have an expiry date. However, if the guarantee provider or their bank insists on an expiry date, th...*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

When a guarantee expires, the liability of the bank to pay under the guarantee becomes void. The bank is no more liable to pay the beneficiary in case of demand. Ideally, the bank guarantee should not have an expiry date. However, if the guarantee provider or their bank insists on an expiry date, then the bank guarantee should clearly and correctly state the amount being guaranteed.


#### ⚙️ Configuration

Expiry of a guarantee and reinstate expired guarantee has no specific configuration to be set up at feature level. The parameter tables are set up at the implementation stage.


#### 📋 Tasks

Related topics:

- Reinstate Expired Guarantee
- Register Claims

Expiry of a Guarantee denotes that the liability of the bank to pay under the guarantee expires and bank is no more liable to pay the beneficiary in case of demand.


##### Enquiries and Reports

This section allows the user to view the below enquiries and reports:

This menu allows the user to process the expiry of guarantees.

To process an expiry of guarantee, follow the below steps:

1. Expiry of Guarantees .
2. In the Guarantees Outstanding screen, click Expiry icon corresponding to a record.
3. In the Expiry of Guarantee screen, enter values in the mandatory and applicable fields.
4. Click the Validate icon to check for errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.


#### 📊 Outputs

There are no Outputs available for Expiry of Guarantee and Reinstate Expired Guarantee feature.

---


### 3.6  Issue Register Guarantee


> **📇 Quick Reference Card**
> 
> **Purpose:** *Bank guarantees are classified as:*
> 
> **Key Fields:** *77C*, *Advise Through Bank*, *Auto Expiry*, *Receiving Bank ID*
> 
> **Sections:** 📖 Introduction | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Bank guarantees are classified as:

- Direct guarantees issued directly to the beneficiary by a bank or through an advising bank. An applicant applies for an indirect guarantee to its bank. If the correspondent bank acts as the advising bank, then the bank verifies the authenticity of the guarantee received from a foreign bank and notifies the beneficiary as requested by the guarantor.
- Indirect guarantees issued to the beneficiary by a correspondent bank of the applicant’s bank. The applicant’s bank issues a counter guarantee to the beneficiary’s bank. Based on this, beneficiary’s bank issues a guarantee to the beneficiary. The system supports the role or activities performed by a guarantor and an advising bank.

The following are major parties in a guarantee cycle that may form part of guarantee contract:

- Principal/Applicant (Optional, maybe same as instructing party)
- Instructing Party
- Guarantor
- Beneficiary

The definition of principal/applicant, instructing party, guarantor and beneficiary as per the International Banking Practice and the Uniform Rules for Demand Guarantees 758 (URDG) of ICC, are as follows:

- Principal/Applicant - The party indicated in the guarantee as having its obligation under the underlying trade contract or relationship supported by the guarantee. The applicant may or may not be the instructing party (Risk Party). In cases, where the applicant may not have the means to procure the issuance of a guarantee through the guarantor, the applicant works with another party, the Instructing Party (IP) to induce a guarantor to issue its guarantee on behalf of the applicant.
- Instructing party - The party who gives instructions to the guarantor bank to issue a guarantee and is responsible for indemnifying the bank. Thus, the credit liability risk is expected to be booked against this party for guarantee.
- Beneficiary - The party in whose favour a guarantee is issued
- Guarantor/Guarantor - The bank who is issuing the guarantee against the credit risk of Instructing Party.


##### Swift Changes 2021 for Issuance of Guarantee

As part of Swift 2021, the category 7 of guarantees and standby L/Cs have been revamped. For Issuance, MT760 format is completely overhauled with 71 new Tags introduced, each capturing specific content of undertaking details a structured format as explained in subsequent sections, whereas in the earlier format, only 7 Tags were available, with all the undertaking details captured under only 1 field 77C . Also, a new message MT761 has been introduced as continuation. In line with the same, the MD Module has been enhanced to support for all these changes.

The following key features are introduced in MD for Issuance as part of changes in SWIFT 2021 MT760/MT761:

- Format changes to existing fields, addition of new fields mapping with corresponding SWIFT Tags introduced.
- Mapping for new SWIFT Message
- Changes in the way a counter-counter or counter guarantee is issued
- Flow changes when guarantee undertaking is advised to beneficiary through another advising bank.

Until Swift 2020, Transact supported the counter undertaking cycle, where, the counter bank issues an undertaking with contract type as Contingent Asset (CA) and requests the receiver of the undertaking to issue the local guarantee / standby LC to the beneficiary. Based on the received guarantee, an undertaking was booked under Contingent Liability (CL )contract type, and the local guarantor issued another independent undertaking to beneficiary with contract type as CA.

As part of the Swift 2021 changes, in counter-counter undertaking, the counter-counter bank issues the undertaking in favour of the counter bank and requests them to issue the counter undertaking to the local bank. The counter bank books the received undertaking with contract type as CL. It also issues the counter undertaking to the local bank as a separate contract under CA. The received counter-counter undertaking (CL contract type) is the master guarantee based on which another child undertaking, that is, the counter undertaking is issued (CA contract type). The master and child undertaking are booked manually as per the existing process, where the user has to book the received and issued undertaking separately. Transact establishes the link between master and child reference for information basis.

The advising flow in counter-counter undertaking cycle is illustrated below:

The advising flow in counter undertaking cycle is illustrated below:

When the advising bank receives an inward guarantee to advice the guarantee / standby letter of credit to the second advising bank, the outward MT760 message is relayed to the second advising bank from the same CL contract. The second advising bank details (Tag 57A), advising bank reference (Tag 23) and purpose of message (Tag 22A) have to be updated to trigger the outward generation of the MT760 message.


##### SWIFT 2023 Changes for Issue of a Demand Guarantee/Standby Letter of Credit

The following fields in MT760 are no longer available in both Seq B and C.

| Status | Tag | Field Name | Content/Options |
|---|---|---|---|
| O | 39D | Additional Amount Information | 12*65z |
| O | 44H | Governing Law and/or Place of Jurisdiction | 2!a[/65x] |

The above fields are now replaced with the following fields (in both Seq B and C).

| Status | Tag | Field Name | Content/Options |
|---|---|---|---|
| O | 39F | Supplementary Information About Amount | 12*65z |
| O | 44J | Governing Law/Jurisdiction | 2!a[/35x] [/65x] |

The field length for 24G is increased to 12*65z in both Seq B and C. Also another field namely, Advise Through Bank is introduced in Seq C to include the Advise Through Bank details.

| Status | Tag | Field Name | Content/Options |
|---|---|---|---|
| O | 57a | Advise Through' Bank | A or D |


#### 📋 Tasks

Related topics:

- Amend Guarantee or Standby LC
- Issue Guarantee
- Issue Counter Guarantee
- Trade Finance and Guarantees Processes
- Corporate Issue Shipping Guarantee
- Corporate- Issue Guarantee

The Miscellaneous Deals or Guarantees module in Temenos Transact allows banks to record the miscellaneous contingent deals that are required to record ‘Guarantee’ type transactions in the bank’s books.


##### Workflow

The user can issue, register and authorise the guarantees using the below procedures:

This screen consists of the following tabs:

This tab displays the list of unauthorised guarantee issued transactions, at this stage, the user can amend, view or delete these transactions.

To amend a guarantee issued transaction, follow the below steps:

1. Guarantee Issued .
2. In the Unauthorised Guarantee Transaction – Issued screen, click the Amend icon corresponding to a record.
3. Enter or amend the field values as required.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

To view a guarantee issued transaction, follow the below steps:

1. Guarantee Issued .
2. In the Unauthorised Guarantee Transaction – Issued screen, click the View icon corresponding to a record.
3. Click the Delivery Preview icon to view the delivery messages.

To delete a guarantee issued transaction, follow the below steps:

1. Guarantee Issued .
2. In the Unauthorised Guarantee Transaction – Issued screen, click the Delete icon corresponding to a record.
3. Verify the guarantee issued transaction details and then click the Delete icon to commit the deletion.

This tab displays the list of unauthorised guarantee received transactions, at this stage, the user can amend, view or delete these transactions.

To amend a guarantee received transaction, follow the below steps:

1. Guarantee Received .
2. In the Unauthorised Guarantees Transaction – Received screen, click the Modify icon corresponding to a record.
3. Enter or modify the field values as required.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

To view a guarantee received transaction, follow the below steps:

1. Guarantee Received .
2. In the Unauthorised Guarantee Transaction – Received screen, click the View Transaction icon corresponding to a record.
3. Click the Delivery Preview icon to view the delivery messages.

To delete a guarantee received transaction, follow the below steps:

1. Guarantee Received .
2. In the Unauthorised Guarantees Transaction – Received screen, click the Delete icon corresponding to a record.
3. Verify the guarantee received transaction details and then click the Delete icon to commit the deletion.

This tab displays the list of unauthorised commission rate change transactions, at this stage, the user can amend, view or delete these transactions.

To amend a commission rate change transaction, follow the below steps:

1. Comm Rate Change .
2. In the Unauthorised CSN Commission Rate Changes screen, click the Edit icon corresponding to a record.
3. Edit the field values as required.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

To view a commission rate change transaction, follow the below steps:

1. Comm Rate Change .
2. In the Unauthorised CSN Commission Rate Changes screen, click the View icon corresponding to a record.
3. Click the Delivery Preview icon to view the delivery messages.

To delete a commission rate change transaction, follow the below steps:

1. Comm Rate Change .
2. In the Unauthorised CSN Commission Rate Changes screen, click the Delete icon corresponding to a record.
3. Verify the commission rate changes and then click the Delete icon to commit the deletion.

This tab displays the list of unauthorised guarantee commission transactions, at this stage, the user can amend, view or delete these transactions.

To amend a guarantee commission transaction, follow the below steps:

1. Guarantee Commission Transactions .
2. In the Unauthorised Guarantee Commission Transactions screen, click the Modify icon corresponding to a record.
3. Enter or modify the field values as required.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

To view a guarantee commission transaction, follow the below steps:

1. Guarantee Commission Transactions .
2. In the Unauthorised Guarantee Commission Transactions screen, click the View icon corresponding to a record.
3. Click the Delivery Preview icon to view the delivery messages.

To delete a guarantee commission transaction, follow the below steps:

1. Guarantee Commission Transactions .
2. In the Unauthorised Guarantee Commission Transactions screen, click the Delete icon corresponding to a record.
3. Verify the guarantee commission transaction details and then click the Delete icon to commit the deletion.

This tab displays the list of unauthorised refund of guarantee charges, at this stage, the user can amend, view or delete the refund of guarantee charges.

To amend a refund of guarantee charge transaction, follow the below steps:

1. Guarantee Charges Refund .
2. In the Refund of Guarantee Charges screen, click the Modify icon corresponding to a record.
3. Modify the field values as required.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

To view a refund of guarantee charge transaction, follow the below steps:

1. Guarantee Charges Refund .
2. In the Refund of Guarantee Charges screen, click the View icon corresponding to a record.
3. Click the Delivery Preview icon to view the delivery messages.

To delete a refund of guarantee charge transaction, follow the below steps:

1. Guarantee Charges Refund .
2. In the Refund of Guarantee Charges screen, click the Delete icon corresponding to a record.
3. Verify the refund of guarantee charges transaction details and then click the Delete icon to commit the deletion.

This menu displays the list of unauthorised MD.DEAL application records which are invoked through the SWIFT messages MT768, MT769, MT787, and MT765. The displayed records are created successfully by automatic process and the user can modify, view the inward swift messages.

To amend an inward guarantee SWIFT message record, follow the below steps:

1. Inward Guarantee Swift Messages .
2. In the MD Records in INAU amended through SWIFT Msg screen, click the Modify icon corresponding to a record.
3. Enter or modify the field values as required.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

To view an inward guarantee swift messages, follow the below steps:

1. Inward Guarantee Swift Messages .
2. In the MD Records in INAU amended through SWIFT Msg screen, click the View SWIFT message icon corresponding to a record.

This menu supports the processing of incoming guarantee messages to create the inward guarantee transactions.

The guarantee transactions generated from the incoming SWIFT messages are kept in On hold status based on the details available in the incoming SWIFT message. Thereafter, the user can input additional details in the transaction.

To create an inward guarantee transactions, follow the below steps:

1. Inward Guarantees Received .
2. In the Inward Guarantees Received through SWIFT screen, click the Modify icon corresponding to a record.
3. Click the View Guarantee icon to view the created guarantee transactions.
4. Click the View incoming message icon to view the incoming swift messages.
5. Click the Validate icon to check for the errors and overrides.
6. Click the Commit icon to submit the record.

This menu displays all the inward SWIFT messages that are received under Trade Finance module with the status and the transaction reference details created in Temenos Transact .

To view an inward trade SWIFT messages, follow the below steps:

1. Inward Trade Swift Messages .
2. In the Inward Trade Finance Swift Messages screen, click the View SWIFT message icon corresponding to a record.
3. Click the View Contract icon to view the contract details.

This menu displays all the inward SWIFT messages that does not create any transaction in Temenos Transact due to the invalid transaction reference provided in tag 21.

The user can view and process the repaired messages. If the user unable to find the related Temenos Transact transaction for the received messages, the user can perform investigation by sending a MT799 to the sender.

To view the repaired messages, follow the below steps:

1. Processing of Repaired Messages .
2. In the Inward Trade Finance Swift Messages screen, click the View SWIFT message icon corresponding to a record.

To process the repaired messages, follow the below steps:

1. Processing of Repaired Messages .
2. In the Inward Trade Finance Swift Message screen, click the Send MT799/MT499 icon corresponding to a record.
3. Select the related transaction reference from the drop-down list.
4. Enter the mandatory field values.
5. Click the Validate icon to check for the errors and overrides.
6. Click the Delivery Preview icon to view the delivery messages.
7. Click the Commit icon to submit the record.

This menu displays all the outstanding letter of credit and guarantee contracts available under Trade Finance module along with the basic details, such as, reference number, currency and amount of the contract.

To send an MT759 SWIFT message, follow the below steps:

1. Outward Ancillary Messages .
2. In the Outstanding Guarantees screen, click the Send MT759 icon corresponding to a record.
3. Enter the mandatory and other field values as required.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu displays all the inward MT759 SWIFT messages.

To view the inward MT759 SWIFT messages, follow the below steps:

1. Inward Ancillary Messages .
2. In the Inward MT759 Swift Messages screen, click the View SWIFT message icon corresponding to a record.

This menu allows the user to send the MT790 and MT490 messages to advise the account owner about the charges, interest or other adjustments to their account.

To send an advice for the charges, follow the below steps:

1. Advice of Charges .
2. In the User Prompt screen, click the Advice of Charges MT790 or Advice of Charges MT490 icon to send the advice of charge message.
3. Enter the field values as required.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to send the MT792 and MT492 messages, requesting the receiver to consider cancellation of the message identified in the request.

To send a cancellation of the message, follow the below steps:

1. Cancellation .
2. In the User Prompt screen, click the Cancellation MT792 or Cancellation MT492 icon to send the cancellation message.
3. Enter the field values along with the cancellation message.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to send the MT795 and MT495 messages, requesting information relating to a previous message or amendment to a previous message.

To send a query on previous message, follow the below steps:

1. Query on sent Message .
2. In the User Prompt screen, click the Query on Sent Message MT795 or Query on Sent Message MT495 icon to send a query on previous message.
3. Enter the necessary field values as required.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to send the MT791 and MT491 requesting for payment of charges, interest or other expenses.

To send a payment request message, follow the below steps:

1. Request of Charges .
2. In the User Prompt screen, click the Request of Charges MT791 or Request of Charges MT491 icon to send a payment request message.
3. Enter the necessary field values as required.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to send the free format messages, such as, MT499, MT799 and MT999.

MT999 can be sent in case of non-availability of SWIFT authentication with the receiver.

To send a free format message, follow the below steps:

1. Send Free Format Message .
2. In the User Prompt screen, click the Free Format Message MT499/MT799 or Free Format Message MT999 icon to send a free format message.
3. Enter the necessary field values as required.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This screen consists of the following tabs:

This menu displays the list of unauthorised guarantee issued transactions. The user can either authorise or delete the transactions.

To authorise a guarantee issued transaction, follow the below steps:

1. Undertaking Issued .
2. In the Unauthorised Guarantee Transaction – Issued screen, click the Authorise icon corresponding to a record.
3. Verify the guarantee issued transaction details and then click the Authorise icon to commit the authorisation.

To delete a guarantee issued transaction, follow the below steps:

1. Undertaking Received .
2. In the Unauthorised Guarantee Transaction – Issued screen, click the Delete icon corresponding to a record.
3. Verify the guarantee issued transaction details and then click the Delete icon to commit the deletion.

This menu displays the list of unauthorised internet request guarantee transactions. The user can either authorise or delete the transactions.

To authorise an internet request guarantee transaction, follow the below steps:

1. Authorise/Delete Internet Requests .
2. In the Internet requests screen, click the Authorise Record icon corresponding to a record.
3. Verify the internet request guarantee transaction details and then click the Authorise icon to commit the authorisation.

To delete an internet request guarantee transaction, follow the below steps:

1. Authorise/Delete Internet Requests .
2. In the Internet requests screen, click the Delete Record icon corresponding to a record.
3. Verify the internet request guarantee transaction details and then click the Delete icon to commit the deletion.

This menu displays the list of unauthorised guarantee received transactions. The user can either authorise or delete the transactions.

To authorise a guarantee received transaction, follow the below steps:

1. Undertaking Received .
2. In the Unauthorised Guarantees Transaction – Received screen, click the Authorise icon corresponding to a record.
3. Verify the guarantee received transaction details and then click the Authorise icon to commit the authorisation.

To delete a guarantee received transaction, follow the below steps:

1. Undertaking Received .
2. In the Unauthorised Guarantees Transaction – Received screen, click the Delete icon corresponding to a record.
3. Verify the guarantee received transaction details and then click the Delete icon to commit the deletion.

This menu displays the list of unauthorised commission rate change transactions. The user can either authorise or delete the transactions.

To authorise a commission rate change transaction, follow the below steps:

1. Commission Rate Change .
2. In the Unauthorised CSN Commission Rate Changes screen, click the Authorise icon corresponding to a record.
3. Verify the commission rate change transaction details and then click the Authorise icon to commit the authorisation.

To delete a commission rate change transaction, follow the below steps:

1. Commission Rate Change .
2. In the Unauthorised CSN Commission Rate Changes screen, click the Delete icon corresponding to a record.
3. Verify the commission rate changes and then click the Delete icon to commit the deletion.

This menu displays the list of unauthorised guarantee commission transactions. The user can either authorise or delete the transactions.

To authorise a guarantee commission transaction, follow the below steps:

1. Authorisation of Guarantee Comm Transactions .
2. In the Unauthorised Guarantee Commission Transactions screen, click the Authorise icon corresponding to a record.
3. Verify the guarantee commission transaction details and then click the Authorise icon to commit the authorisation.

To delete a guarantee commission transaction, follow the below steps:

1. Authorisation of Guarantee Comm Transactions .
2. In the Unauthorised Guarantee Commission Transactions screen, click the Delete icon corresponding to a record.
3. Verify the guarantee commission transaction details and then click the Delete icon to commit the deletion.

This menu displays the list of unauthorised refund of guarantee charges. The user can either authorise or delete the transactions.

To authorise a refund of guarantee charges transaction, follow the below steps:

1. Authorisation Refund of Charges .
2. In the Refund of Guarantee Charges screen, click the Authorise Refund icon corresponding to a record.
3. Verify the refund of guarantee charges transaction details and then click the Authorise icon to commit the authorisation.

To delete a refund of guarantee charges transaction, follow the below steps:

1. Authorisation Refund of Charges .
2. In the Refund of Guarantee Charges screen, click the Delete icon corresponding to a record.
3. Verify the refund of guarantee charges transaction and then click the Delete icon to commit the deletion.

This menu allows the user to authorise or delete the unauthorised MT792 and MT492 cancellation messages.

To authorise the cancellation messages, follow the below steps:

1. Authorise Cancellation Messages .
2. In the List of Incoming n92/95 Messages screen, click the Authorise icon corresponding to a record.
3. Verify the cancellation messages and then click the Authorise icon to commit the authorisation.

To delete the cancellation messages, follow the below steps:

1. Authorise Cancellation Messages .
2. In the List of Incoming n92/95 Messages screen, click the Delete icon to delete a transaction.
3. Verify the cancellation messages and then click the Delete icon to commit the deletion.

This menu allows the user to authorise or delete the free format messages, such as, MT799, MT499 and MT999 from the unauthorised records.

To authorise the free format messages, follow the below steps:

1. Authorise Free Format Messages .
2. In the Inward Free Format Messages screen, click the Authorise icon to authorise a transaction.
3. Verify the free format messages and then click the Authorise icon to commit the authorisation.

To delete the free format messages, follow the below steps:

1. Authorise Free Format Messages .
2. In the Inward Free Forma Messages screen, click the Delete icon to delete a transaction.
3. Verify the free format messages and then click the Delete icon to commit the deletion.

This menu allows the user to authorise or delete the MT795 and MT495 messages from the unauthorised records.

To authorise the MT795 and MT495 messages, follow the below steps:

1. Authorise Query on Sent Messages .
2. In the List of Incoming n92/95 Messages screen, click the Authorise icon to authorise a transaction.
3. Verify the MT795 and MT495 messages and then click the Authorise icon to commit the authorisation.

To delete the MT795 and MT495 messages, follow the below steps:

1. Authorise Query on Sent Messages .
2. In the List of Incoming n92/95 Messages screen, click the Delete icon to delete a transaction.
3. Verify the MT795 and MT495 messages and then click the Delete icon to commit the deletion.

This menu allows the user to authorise or delete the MT790, MT791, MT490 and MT491 messages from the unauthorised list of records.

To authorise the MT790, MT791, MT490 and MT491 messages, follow the below steps:

1. Authorise Request/Advice Charges .
2. In the Unauthorised Records screen, click the Authorise icon to authorise a transaction.
3. Verify the MT790, MT791, MT490 and MT491 messages and then click the Authorise icon to commit the authorisation.

To delete the MT790, MT791, MT490 and MT491 messages, follow the below steps:

1. Authorise Request/Advice Charges .
2. In the Unauthorised Records screen, click the Delete icon to delete a transaction.
3. Verify the MT790, MT791, MT490 and MT491 messages and then click the Delete icon to commit the deletion.

This section consists of,

This menu allows the user to issue a bid bond guarantee.

To issue a bid bond guarantee, follow the below steps:

1. Issue of Bid Bond .
2. In the Issue of Bid Bond screen, enter the mandatory and other required field values.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to issue shipping guarantee under collection and LC.

To issue a shipping guarantee under collection, follow the below steps:

1. Issue of Shipping Guarantee .
2. In the User Prompt screen, select the Shipping Guarantee under Collection tab.
3. In the Issue Shipping Guarantee under Import Collection Document screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

To issue a Shipping Guarantee under LC, follow the below steps:

1. Issue of Shipping Guarantee .
2. In the User Prompt screen, select the Shipping Guarantee under LC tab.
3. In the Issue Shipping Guarantee under LC screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to issue generic guarantees.

To issue a generic guarantee, follow the below steps:

1. Issue of Generic Undertaking .
2. In the Issue of Generic Demand Guarantee screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to issue a performance bond guarantee.

To issue a performance bond guarantee, follow the below steps:

1. Issue of Performance Bond .
2. In the Issue of Performance Bond screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to issue a letter of credit on behalf of its customer to serve as a guarantee to the beneficiary of the letter of credit.

To issue a standby letter of credit, follow the below steps:

1. Issue of Standby LC .
2. In the Issue of Stand By Import LCs screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to advice the generic guarantees and standby LCs to the beneficiary of the received guarantees.

To advice generic guarantees and standby LCs to the beneficiary, follow the below steps:

1. Generic-Guarantee/Standby LC .
2. In the Guarantee Received Generic screen, enter the mandatory and other required field values.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to record and generate necessary SWIFT message for Guarantee Received-Covering Facility.

To record and generate the SWIFT message for Guarantee received-covering facility, follow the below steps:

1. .
2. In the Guarantee Received Covering Facility screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to issue counter or counter-counter guarantees.

To issue counter or counter-counter guarantees, follow the below steps:

1. Issue of Counter/Counter-counter Undertakings .
2. In the Issue of Counter/Counter-counter Guarantee screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to issue a counter standby undertaking.

To issue a counter standby undertaking, follow the below steps:

1. Issue of Standby LC Undertaking .
2. In the Issue of Standby Letter of Credit screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to advice the counter or counter-counter guarantees to the beneficiary of the received guarantees.

To advice counter or counter-counter guarantees to the beneficiary, follow the below steps:

1. Counter / Counter -counter Undertakings .
2. In the Received Counter/Counter-counter Guarantee screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to advice the counter or counter-counter standby guarantees to the beneficiary of the received guarantees.

To advice the counter or counter-counter standby guarantees to the beneficiary, follow the below steps:

1. Counter/Counter-counter Standby LC .
2. In the Received Standby LC Undertaking screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to issue or advice the received guarantees and facilitates to generate the necessary SWIFT messages to the beneficiary’s bank.

To issue or advise the received guarantees, follow the below steps:

1. Generic-Guarantee Received/Advised .
2. In the Guarantee Received Generic screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu displays all the transactions that are created through inward MT760 SWIFT messages. The user can view and process the transactions.

To view the inward guarantee details, follow the below steps:

1. Inward MT760 Messages .
2. In the Guarantees Received screen, click the View Guarantee icon corresponding to a record.

To process the transaction created through inward MT760 messages, follow the below steps:

1. Inward MT760 Messages .
2. In the Guarantees Received screen, click the Modify icon corresponding to a record.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

To view the incoming messages, follow the below steps:

1. Inward MT760 Messages .
2. In the Guarantees Received screen, click the View incoming message icon corresponding to a record.


#### 📊 Outputs

The Miscellaneous Deals or Guarantees module in Temenos Transact allows banks to record the miscellaneous contingent deals that are required to record ‘Guarantee’ type transactions in the bank’s books.


##### Enquiries and Reports

This section helps the user to view the outstanding guarantees received and the guarantees that are due for expiry.

Outstanding Guarantees Issued

This enquiry displays the list of received guarantees, which are outstanding in the books of the bank. The user can view the guarantee record by clicking on the View Record icon.

Guarantees Expire in next 15 days

This enquiry displays the list of guarantees that are due for expiry in the next 15 calendar days (including today) and those that are already expired and not reversed from the books of the bank due to the setting in Auto Expiry field to NO. The user can view the guarantee record by clicking on the View Record icon.


##### SWIFT Messages

Expand the below drop downs to know about SWIFT messages:

This message requests for the movement of funds between financial institutions, related to an underlying customer credit transfer that was sent with the cover message.

This message is sent by the guarantee issuing bank to a counter-party bank, to advise the issue of a guarantee. In the guarantees menu, it is generated while ‘Issuing a Guarantee’.

This message is an acknowledgement by a counter party bank for having received the guarantee from the issuing bank. It is sent to the bank customer specified in the Receiving Bank ID field.

This message is sent by the guarantee issuing bank to a counter-party bank as an extension of MT760.


##### Advices

Expand the below drop downs to know about the Advices:

This advice is sent to the customer as a confirmation for the issuance of guarantee on behalf of them.

This advice is sent to the beneficiary for receiving the guarantee from the issuing bank on their behalf.

This advice is sent to the beneficiary of the received guarantee.


##### Alerts

NA

---


### 3.7  Managing External Requests


> **📇 Quick Reference Card**
> 
> **Purpose:** *Transact and its associated APIs capture external requests for Trade Finance products such as Guarantee and StandBy Letter of Credit. External requests from sources such as corporate users, interbank banking, or other channels are now seamlessly integrated into the system. Once a request is initiate...*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Transact and its associated APIs capture external requests for Trade Finance products such as Guarantee and StandBy Letter of Credit. External requests from sources such as corporate users, interbank banking, or other channels are now seamlessly integrated into the system. Once a request is initiated, the system automatically notifies the Trade Finance bank user so they can perform the necessary action in Transact. This streamlines workflows, ensuring the efficient and secure management of trade finance requests across diverse channels.

Read Home to know more about the published APIs and read Trade Finance to know more about Temenos Digital.


#### ⚙️ Configuration

This feature has no specific configuration to be setup. The parameter applications are setup at the implementation stage.


#### 📋 Tasks

There are no Tasks available for Managing External Requests feature.


#### 📊 Outputs

There are no Outputs available for Managing External Requests feature.

---


### 3.8  Margin or Provision


> **📇 Quick Reference Card**
> 
> **Purpose:** *Margin is the contribution borne by the borrower while availing fund based or non-fund based loan facilities from a commercial bank. A provision is an amount set aside from a company's profits to cover an expected liability or a decrease in the value of an asset, even though the specific amount migh...*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Margin is the contribution borne by the borrower while availing fund based or non-fund based loan facilities from a commercial bank. A provision is an amount set aside from a company's profits to cover an expected liability or a decrease in the value of an asset, even though the specific amount might be unknown.


#### ⚙️ Configuration

Margin or provision has no specific configuration to be set up at feature level. The parameter tables are set up at the implementation stage.


#### 📋 Tasks

Related topics:

- Issue Guarantee
- Trade Finance and Guarantees Processes

Trade Finance application allows margin or provision upto and above hundred percent of the guarantee amount.

In few cases, where there is a tolerance or an additional amount specified for the guarantee, a provision or margin is required in excess of hundred percent of guarantee.


##### Workflow

The Trade Finance Officer can collect margin for the guarantee transactions.

This menu allows the user to release a margin that collected during guarantee issuance.

To release a guarantee margin, follow the below steps:

1. Release Guarantee Margin .
2. In the Release Margin screen, click the Release Margin icon corresponding to a record.
3. In the Guarantee Release Margin screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to release guarantees liability.

To release a guarantee liability, follow the below steps:

1. Release Guarantees Liability .
2. In the Reduce Liability screen, click the Reduce Liability icon corresponding to a record.
3. In the Guarantee Release of Liability screen, enter values in the the mandatory and applicable fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.


#### 📊 Outputs

There are no Outputs available for Margin or Provision feature.

---


### 3.9  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *A guarantee is an undertaking by one party (the guarantor) to stand behind specific obligations (current and future) of a third party (Principal). The Guarantor agrees to compensate the Beneficiary of loss (up to a specified amount) when the third party (Principal) defaults or fails to fulfill the o...*
> 
> **Applications:** `MD.CLAUSES`, `MD.DEAL`
> 
> **Key Fields:** *Account with Bank*, *Accrual Cycle*, *Acct With Bank Bic*, *Acct With Bank Swift Addr.1*, *Acct With Bank Swift Addr.2*, *Additional Info*, *Amount Spec*, *Amount Spec 39C* ... +147 more
> 
> **Sections:** 📖 Introduction | 📊 Outputs


#### 📖 Introduction

Related topics:

- APIs
- Temenos Transact Services
- Syndicate Guarantee
- System Maintained Files

A guarantee is an undertaking by one party (the guarantor) to stand behind specific obligations (current and future) of a third party (Principal). The Guarantor agrees to compensate the Beneficiary of loss (up to a specified amount) when the third party (Principal) defaults or fails to fulfill the obligations under the guarantee.

A guarantee is:

- A security for performance of a contractual obligation
- An irrevocable undertaking from a guarantor
- A commitment independent of the obligations of its underlying contract
- A guarantor’s assurance towards beneficiary whereby the guarantor replaces the client’s (principal’s or applicant’s) credit worthiness with its own
- The guarantor undertakes to pay a specific sum of money to the beneficiary in the event of non-performance or default by the client (principal or applicant).


##### Understanding Guarantees inTemenos Transact

The Miscellaneous Deals (MD) module provides the facility to record guarantee undertaking, which are off balance sheet. The principal amounts involved are booked as contingent entries. Temenos Transact uses the MD module to record different guarantee type transactions on the banks’ books. These range from straight forward guarantees (issued and received) to more specific trade finance related deals (bid and performance bonds). It allows forward dated contracts and collection of charges using standard FT.CHARGE.TYPE and FT.COMMISSION.TYPE tables respectively. Additionally, customised delivery advices can be generated. The MD.DEAL contracts can be linked to the LIMIT and COLLATERAL modules and this parameter setting can be changed at the contract level.

The types of deals that are entered in MD.DEAL are related to contingent liability or assets. The main feature is that the risk is recorded off balance sheet otherwise known as below the line. There are options to utilise the LIMIT updates at contract level, ability to levy charges or commissions and the number of deal types that can be entered.

The below shown is letter of guarantee cycle:


##### ConfiguringMD.DEAL

The configuration required for MD.DEAL is defined in the below parameter tables:

The foundation block for the MD module is the MD.PARAMETER table. The MD.PARAMETER record is set for each COMPANY in Temenos Transact . For example, US0010001.

Each bank has one record of this file, and for each company the bank can create a parameter file. This application provides the user with an option to specify where the accounting entries are passed, what accrual cycles are set, and the transaction codes are used in Temenos Transact . Valid deal types, deal sub types and category code ranges are set up. Overall, level rules are specified.

Some of these fields are explained below:

The following are basic types of contract based on which all deal types are created:

The difference between contingent and memorandum type is negligible. Memo type is considered as the softer type of deals. Exact usage of these types are at the discretion of user.

When the banks are issuers cum beneficiaries, such guarantees are termed as memorandum items. All deal types created should be based on these and should be specified in

.

> **⚠️ Note:** MA and ML type of contract are for registering deals for internal records of the bank

| Type | Description |
|---|---|
| CL | Contingent Liability |
| CA | Contingent Asset |
| ML | Memorandum Liability |
| MA | Memorandum Asset |

MD uses P&L category codes for accrual of charges and commission. The Accrual Cycle field defines the cycle for accruing time-based commission. The frequency can be set to Daily, Weekly or Monthly. The format of the value entered in this field is . For example, DAILY/BSNSS or WEEK1 to WEEK9 or M01 to M12.

Only when a value is entered in this field, the commission schedule accruals are performed. The user is not allowed to leave this field blank once value has been entered and authorised. When the system performs commission accruals, the date on which the accruals are posted is updated and displayed in this field. Respective P&L category codes for accrual of time-based commission can be set up in the Current Accrual , Previous Month and Previous Year fields.

The category code entered in the Current Accrual field is used for posting the current month accruals related to the commission based fees allowed in MD contracts. The value in this field cannot be changed once authorised. However, New Current field can be used to amend the value. This triggers a system change and rebuild the financial information produced by MD. The Previous Month field is used to define category used for posting the accruals of the previous months. The value in this field cannot be changed once authorised.

The Previous Year field is used to set category for posting the accruals of previous year. The value in this field cannot be changed once authorised. The P&L category code must be a valid code ranging from 50000 to 59999. The below screenshot shows the Contract Type CA broken down into different sub-types for specific usage.

Allowed values are Online or End of Day. When set to,

- Online (for negative principal movements) – The limit is updated dynamically for same day, even for negative principal movements. Customer position is updated and contingent entries are raised online for new deals, reversals, same day principal movements and change in principal movements.
- End of Day – The contingent entries are raised only during Close of Business(COB). Limit updation for principal decrease takes place during COB. Limit updation for decreases and accounting entries for changes to principal done only during COB.

The system performs accrual or amortisation of commission at the end of day batch, based on the details of commission setup in each MD.DEAL . The system capitalises the commission amount based on the value at the contract level, ( Process At Sod and Liquidation Mode ) irrespective of the value at the parameter level. Allowed values are Yes or No. When set to,

- Yes – The process takes place during the start of day
- No – The process takes place at the end of day

The bank might want to keep the record in live status, even after the maturity till they receive the original guarantee issued. Temenos Transact provides an option to keep the deal live until the original guarantee is returned. This means that even after the maturity date, the deal stays with the status CUR and LIQ, unless the user sets the Auto Expiry field to Yes in MD.DEAL . This can be controlled from the parameter or record level. For example, even after the expiry, a guarantee can be kept in the live file, until the original guarantee is received on hand.

Allowed values are Manual or Automatic and when set to,

- Manual – The guarantee continues to be in live file even after maturity and has become null and void. This prevents the record to move to history. The Auto Expiry field in MD.DEAL table is defaulted to No. However, this can be overridden at the deal. This caters to scenarios where the record is live until the original guarantee is returned.
- Automatic – The Auto Expiry field in MD.DEAL is defaulted to Yes. On maturity, the record moves to history after the number of days mentioned in the Days Post Maturity field.

1 to 999 working or calendar days can be mentioned as NW/NC. For example, 3 Working days are entered as either 3W or 03W and 5 Calendar days as 5C or 05C.

Impact on limit could be set to less provision amount taken (if any), by setting Include Provision field. Allowed values are Yes or No and when set to,

- Yes – The impact on limit is reduced to the extent of the provision taken against the deal.
- No – Irrespective of any provision taken for the deal, the limit gets hit for the entire principal amount of the deal (full guaranteed amount of the leader’s portion). The value entered in this field is defaulted in the deal. A NULL value however, is treated as No.

Provision can be credited to an internal account. If the credit provision account is not defined in the deal, then an internal account created under the category (10000 – 19999), in which the margin money or cash margin is to be parked. The category code in which the default internal account to be opened is entered in Prov Category field. An internal account is opened in local currency in this category. Temenos Transact automatically creates accounts for other currencies whenever needed.

The feature of netting the proportionate provision amount to be released with the invocation amount and debit the balance amount from the invocation debit account can be setup. The user can choose to net the accounting entries, at the time of payment of invocation amount. Allowed values are Yes or No and when set to,

- Yes – The user can net the provision release entry with the debit invocation account entry at the time of executing invocation.
- No – The user cannot net the provision release entry with the debit invocation account entry at the time of executing invocation. The system defaults the value to No, when the user does not define it.

The transaction code that is used in the accounting entries during debit or credit provision, commission or when a contract is invoked is defined.

- Crediting and debiting provision amounts in Tr Prov Code Cr and Tr Prov Code Dr
- Paying and receiving time based commission in Csn Pay Txn Code and Csn Rec Txn Code
- Crediting and debiting during invocation in Tr Inv Code Dr and Tr Inv Code Cr

In case of syndicated lending for non-funded limits, participant’s share in the commission is temporarily parked in an internal account with category code defined in Part Csn Acc field.

When a shipping guarantee is issued against an import LC, the guarantee limit is also updated in addition to the existing LC liability duplicating the customer's liability. LC liability is reversed when the drawing under the LC is settled and the guarantee liability is reversed on the maturity of the guarantee contract. The Reduce LC Liab field is used to shift the liability from LC to guarantee instead of duplicating the liability entries in both LC and guarantees. Allowed values are Yes or No and when set to,

- Yes – The system automatically create SG type of drawings under LC, thus reversing the LC liability and updating the guarantee liability.
- No – The existing functionality of updating the guarantee liability in addition to the LC liability continues. The user cannot amend the value once defined. The system defaults the value No, if not defined by the user.

The parameter table determines whether the limit should be updated and later checked or blocked at individual deal level. For example, the user may opt not to set up limits for guarantees received from customers. Complete flexibility is available to classify miscellaneous deals into asset and liability products and further into those requiring limit checking.

Separate rules for limit checking can be set if limit has to be made Mandatory, Optional or No input using choices available in respective fields Cont Limit Link , Memo Limit Link , CL Limit Link and ML Limit Link . The Cont Limit Link field indicates the relationship of deal amounts for Contingent Assets (contract type CA) within the LIMITS system. This parameter determines whether an entry has to be made in the Update Limit and Limit Reference fields of a contingent asset MD.DEAL .

The Memo Limit Link field indicates the relationship of Memorandum Assets (contract type MA) with the LIMITS system. This field determines whether an entry has to be made in the Update Limit field and Limit Reference field of a memorandum MD.DEAL . The CL Limit Link field indicates the relationship of Contingent Liabilities (contract type CL) with the LIMITS system. This field determines whether an entry has to be made in the Update Limit field and Limit Reference field of a contingent MD.DEAL . The ML Limit Link field indicates the relationship of Memorandum Liabilities (contract type ML) with the LIMITS system. This field determines whether an entry has to be made in the Update Limit field and Limit Reference field of a memorandum MD.DEAL .

> **⚠️ Note:** If the user leaves these fields blank it is the same as selecting 'Optional'.

The value in this field decides the stage at which the internet banking customer's limit must be updated when request for issuance of guarantee is initiated through internet banking. Allowed values are Yes or No and when set to,

- Yes – The system checks and updates customer's limit, when the corporate customer requests for issuance of guarantee through internet banking.
- No – The customer's limit is checked and updated only when the request is approved at the banks side.

In order to have a soft delivery option for messages, Md Class Type and Eb Class Type fields are setup. To preview messages in soft delivery, Preview is mentioned in the Additional Info field in PGM.FILE for the record MD.DEAL .

When Backward Delivery field is set to Yes, the system continues the old delivery set-up. This field is set to No, for new implementations. Md Class Type and Eb Class Type multi value fields are necessary for soft delivery set up.

> **⚠️ Note:** It is recommended to define values during initial system build so secondary build stage can take care of soft delivery.

In a deal, when debit and credit currency are different, treasury or default buy or sell rate is used for converting amounts, for which a rounding rule can be applied. The default in Temenos Transact is natural rounding. However, the Rounding Rule field in MD.PARAMETER is used to setup new rounding rules. Rounding rule is first setup in the EB.ROUNDING.RULE application and then entered into Rounding Rule field.

Similarly, using the Csn Acct Roundg Rule field in the MD.DEAL application, the user can specify the rounding type for the calculation of commission. Values entered in this field at application level overrides the conditions defined at product level. If the rounding types are not defined in these fields, then it takes place as defined at the product level. Other methods defined in EB.ROUNDING.RULE are attached to the Rounding Type field.

While issuing a guarantee, charges and commissions can be collected at the time of issue or can be scheduled to be taken at a future date. When commission is claimed on the guarantee, the claiming commission amount is recorded in MD.BALANCES application and the commission details are defaulted in a new application where the user transacts the settlement of claimed amount.

The system defines the P&L category code for accounting when already collected charges which have not been amortised and those which have, and commission, either time based or fixed, are refunded or written-off in case of a claimed commission. MD.FEE.SETTLEMENT is used to settle, write-off and refund the commission as well as charges. However, write off and refund category code is defined in the parameter level.These category codes are used to account write-off and refund of commission transactions

Claim Wof Cat field holds the P&L category to be debited while writing off the unsettled claimed commission. Refund Category field holds the P&L category to be debited for the refund of realised portion of commission or charge.

It is possible to reinstate a contract from LIQ to CUR status and it allows all actions that can be performed on a live contract. This option allows user to process the invocation claim and extend the maturity date of the guarantee, when the system date crosses the original maturity date before the contract matures. It allows to reinstate a guarantee after expiry of the contract from EXP to CUR status.

The following fields in MD.PARAMETER caters to the requirement of reinstating a guarantee after expiry:

- The number of days entered in the Expiry Days field by the user is used to calculate the maturity date from the Advice Expiry Date. If this field is amended, then it is applied only to the new contracts. This is an optional field with the format as nnnC or nnnW where, nnn – number of days from 1 to 999 C – calendar days W – working days
- Value entered in the Csn Period field decides the end date for calculating time based commission at the contract level.

- The information in this field defines the number of days within which a decision has to be taken for any invocation claims received. This is used under enquiries. Accepts valid days format - +NNX; where, n stands for two numeric digits representing the number of days X denotes the calendar days (C) or working days (W)
- This is an optional input field.
- Enquiries are created to list the guarantees with outstanding claims, for which decision has to be taken within the specific period.

This field indicates whether commission rate change can be done at the contract level or through MD.CSN.RATE.CHANGE application. Allowed values are Yes or No.

| Fields in MD.PARAMETER | Values in the Field |
|---|---|
| Poa Wash Categ | Valid PO wash account category code as defined in the CATEGORY table |
| Payment Order Categ | Valid record ID of the table PAYMENT.ORDER.PRODUCT |

| Contract Type | Form of Undertaking | Deal Sub type |
|---|---|---|
| CA | DGAR | GTISS |
|  | DGAR | BBOND |
|  | DGAR | PBOND |
|  | DGAR | SGILC |
|  | DGAR | SGCOL |
|  | STBY | STDY |

| Fields in MD.CLAUSES | Fields in MD.DEAL | Swift Tag |
|---|---|---|
| Sender Info 72Z | Sender Info | 72Z |
| Undk Charges71D | Undk Charges | 71D |
| Docs Present Instr 45C | Docs Present Instr | 45C |
| Txn Details 45L | Txn Details | 45L |
| C Docs Present Instr 45C | C Docs Present Instr | 45C |
| C Txn Details 45L | C Transfer Cond | 45L |
| C Undk Charges 71D | C Txn Details | 71D |
| Mt767 Sender Info 72Z | Mt767 Sender Info | 72Z |
| Mt767 Undk Term Cond 77U | Mt767 Undk Term Cond | 77U |
| Mt767 C Undk Term Cond 77L | Mt767 C Undk Term Cond | 77L |
| Mt768 Sender Info 72Z | Mt768 Sender Info | 72Z |
| Mt765 Addl Amount Info 78 | Mt765 Addl Amount Info | 78 |
| Present Comp Dets 77 | Present Comp Dets | 77 |
| Mt765 Send Recv Info 72Z | Mt765 Send Recv Info | 72Z |
| Reason For Refusal 77J | Reason For Refusal | 77J |
| Disp Of Docs 77B | Disp Of Docs | 77B |
| Mt786 Send Recv Info 72Z | Mt786 Send Info | 72Z |
| Inv Bnk To Bnk 72Z | Inv Bnk To Bnk | 72Z |
| Amount Spec 39C | Amount Spec | 39C |
| Mt769 Chg Details 71B | Mt769 Chg Details | 71B |
| Mt769 Sender Info 72Z | Mt769 Sender Info | 72Z |
| Mt787 Sender Info 72Z | Mt787 Sender Info | 72Z |
| Mt785 Sender Info 72Z | Mt785 Sender Info | 72Z |
| Mt750 Sender Info 72Z | Mt750 Sender Info | 72Z |
| Mt754 Sender Info 72Z | Mt754 Sender Info | 72Z |
| Mt752 Sender Info 72Z | Mt752 Sender Info | 72Z |
| Mt756 Sender Info 72Z | Mt756 Sender Info | 72Z |
| Mt756 Sender Info 72Z | Mt756 Narrative | 72Z |

MD.TXN.TYPE.CONDITION table facilitates defaulting provision and commission percentage. It ensures the collection of minimum commission amount for the guarantees issued. The default commission thus collected is defined currency-wise. In the absence of any default value for a given currency, the local currency equivalent is computed and applied.

- Similarly, the percentage of commission is defined for any CATEGORY mentioned in the Deal Sub Type field and the same is defaulted in the deal. The definition of commission percentage becomes mandatory if MD.CSN.RATE.CHANGE is invoked.
- To ensure the recovery of a minimum amount of commission for any deal, a bank can use Min Comm Tenure field. Value entered in this field indicates the minimum tenure represented in days, for which commission is to be calculated. To ensure that a minimum amount of commission is recovered for any Deal, Min.Amount and Min Comm Tenure fields are used.
- When the resultant commission of a deal is greater than the default value, the computed value stays.
- When the resultant commission of a deal is greater than the default value, but the tenor is less than the default value, the computed value stays.
- When the resultant commission of a deal is less than the default value, but the tenor is greater than the default value, the default commission is taken.
- When the resultant commission of a deal is less than the default value and the tenor is less than the minimum period, the commission is recalculated for the default period.
- If this commission is greater than the default commission, it is applied else, the default commission is applied.
- This default commission is defined currency-wise. In the absence of any default value for a given currency, the equivalent of the local currency is computed and applied.
- The percentage of commission for any CATEGORY under a Deal Sub Type can be defined and that is defaulted in the deal. This definition of commission percentage becomes mandatory if MD.CSN.RATE.CHANGE application is to be invoked.

The bank can establish a percentage for a contract group. If required, user may stipulate different provision rates for the same category of guarantee. For example, deal amount-wise.

> **⚠️ Note:** While defining the groups, the user has to ensure that the same contract does not fall in two different groups. If so, the first fit is returned and the grouping may be defected.

APPL.GEN.CONDITION can be used to allocate group codes based on a number of defined conditions and/or local routines for any Temenos Transact application with a STANDARD.SELECTION record for the application. Hence, banks can form different groups for different treatment of charges.

Forming a group for people residing in the US. This can be done by entering the name of the group as USERS in the

field with condition as RESIDENCE EQ US

The APPL.GRP.CONDITION subroutine is called to evaluate the current contract record using relevant APPL.GEN.CONDITON . It returns the first group code where all decision checks evaluate to true. This application can call the evaluation routine from VERSION routines to update local reference fields with the relevant group code.

The Group Id is defined in the APPL.GEN.CONDTION for the MD application. For example, NON-RESIDENT of C-XXXXXX, where XXXXXX is the Customer ID.

The MD.GROUP.CONDITION application can default the following values:

- Applicant’s default provision percentage and the respective debit and credit provision accounts (if applicable).
- Applicant’s commission schedule details such as Csn Perc , CSN Rate , Csn Ccy and CSN Amount .

MD.GROUP.CONDITION is used for setting up provision percentage of a particular group, deal subtype-wise and category-wise. Group ID defined in APPL.GEN.CONDITION is the ID for MD.GROUP.CONDITION . Additionally, C-1001 is accepted as ID, where the customer number is 1001. The specific condition for the customer is defined .

When Provision % field in MD.DEAL is set to Yes, the related fields open up in MD.DEAL . The user can define the account from which provision is to be taken using Debit Prov Acc and into which it is to be kept using Credit Prov Acc fields in MD.GROUP.CONDITION .

The user can define the date on which the provision is to be released using Provision Release Date field in MD.DEAL . Though the default release account is indicated in Debit Prov Acc field in MD.GROUP.CONDITION , the user can specify a different account in Margin Release Acct field in MD.DEAL . Commission can be defined in percentage, fixed rate or fixed amount based on category.


##### MD Build Sequence

The order in which these files should be created is stored within the automated tool for IM. The order sequence in the ascending build reference order is given in the left. Mandatory tables are indicated with a red star mark and optional tables in blue colour.

Wherever there are dependencies for filling up values in the tables in build sequence, the dependencies are shown on the right.


#### 📊 Outputs

Once the system has been configured for the types of deal that are to be used by the bank, the next stage is to define the different type of deals for reporting and financial purpose.

To report the deals to the appropriate ledger line, the following values can be used in Asset Type field of RE.STAT.REP.LINE application.

| Asset Type | Description |
|---|---|
| CONTCR | Contingent liabilities |
| FWDCONTCR | Forward starting – Contingent liabilities |
| CONTBD | Contingent assets |
| FWDCONTCB | Forward starting – Contingent assets |
| MEMOCR | Contingent liabilities (memo basis) |
| FWDMEMOCR | Forward starting – Contingent liabilities (memo basis) |
| MEMODB | Contingent assets (memo basis) |
| FWDMEMODB | Forward starting – Contingent assets (memo basis) |

While the contingent assets or liabilities are reported below the line, the memo equivalents are usually off-balance sheet. However, these can be used for internal ledger purposes.

| GL Accounting and Limit | Value |
|---|---|
| Credit CONTDB | GBP 10,000,000.00 |
| Reduce limit by | GBP 10,000,000.00 |

The online enquiry Claims Received Under Guarantee lists all the claims that are processed under guarantee received.

The online enquiry Claims Paid/Cancelled under Guarantee lists all the claims that are paid or cancelled under guarantee received.

The SBLC Presentations enquiry lists all the presentations in SBLC under which documents are presented.


> **Related Applications:** `MD.CLAUSES`, `MD.DEAL`

---


### 3.10  Multi Party Guarantee


> **📇 Quick Reference Card**
> 
> **Purpose:** *A guarantee can primarily be viewed as a contract between two parties, namely the guarantor or bank and the beneficiary, and is independent of the underlying contract. In depth, a guarantee is not just a two-party relationship between guarantor and beneficiary. It forms part of a multi-party relatio...*
> 
> **Sections:** 📖 Introduction | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

A guarantee can primarily be viewed as a contract between two parties, namely the guarantor or bank and the beneficiary, and is independent of the underlying contract. In depth, a guarantee is not just a two-party relationship between guarantor and beneficiary. It forms part of a multi-party relationship, which apart from the guarantee itself consists of the underlying contractual relationship between:

- Principal debtor and the creditor on the one side
- Principal debtor and bank on the other hand


#### 📋 Tasks

Multiparty guaranty is made by the guarantors in favor of the secured parties.


##### Workflow

The Trade Finance Officer can issue multi-party guarantee and related processes.

This menu allows the user to issue a multi-party guarantee.

To process a multi-party guarantee, follow the below steps:

1. Issue of Multi-party Guarantee .
2. In the Issue of Multi-Party Guarantee screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

This menu allows the user to amend a multi-party guarantee.

To amend multi-part guarantee, follow the below steps:

1. Amendment to Multi-party Guarantee .
2. In the Multi Party Guarantees Issued screen, click the Amend icon corresponding to a record.
3. In the Amendment to Multi Party Guarantee screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to process the participation in another bank’s deal.

To process the participation, follow the below steps:

1. Participation Taken .
2. In the Participation taken screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.


#### 📊 Outputs

There are no Outputs available for Multi-party Guarantee feature.

---


### 3.11  Non Extension Guarantee


> **📇 Quick Reference Card**
> 
> **Purpose:** *The bank user can notify the Non –Extension to the parties in the guarantee. As a part of SWIFT 2021 changes, a new message MT785 is introduced to inform the advising bank/ beneficiary about the non-extension of LC when it is placed under automatic extension method. It may also be used for confirmat...*
> 
> **Key Fields:** *31E*, *Advice Expiry
 Date*, *Advice Thru Bk*, *Advice Thru Bk Name*, *Advising Bk*, *Advising Bk Name*, *Alternate ID*, *Auto Ext Expiry Date* ... +14 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The bank user can notify the Non –Extension to the parties in the guarantee. As a part of SWIFT 2021 changes, a new message MT785 is introduced to inform the advising bank/ beneficiary about the non-extension of LC when it is placed under automatic extension method. It may also be used for confirmation of the final date of expiry of the guarantee.


##### Understanding MT785

MT785 message is sent in any one of two ways:

- By the party that issued the undertaking (guarantee, demand guarantee, standby letter of credit or dependent undertaking) to the beneficiary (that is, only in case of beneficiary being a financial institution) or to a nominated advising party that advised the undertaking to the beneficiary or to another advising party.
- By the party that issued the counter-undertaking (counter-guarantee or counter-standby) to the beneficiary of the counter-undertaking (financial institution).


#### ⚙️ Configuration

Non extension of guarantee has no specific configuration to be set up at feature level. The parameter tables are set up at the implementation stage.


#### 🔧 Working With

As per the changes proposed to MT7XX messages by SWIFT, the MT785 Guarantee/Standby Letter of Credit Non-Extension Notification message is supported in guarantees. This message is initiated by the party obligated on the undertaking (Issuing Bank) to refuse extension beyond the current expiry date.


##### MT785 Guarantee/Standby Letter of Credit Non-Extension Notification

MT785 message is used to notify the beneficiary, if applicable, via one or more advising parties of the non-extension of the referenced undertaking beyond the current expiry date.

The business flow shown in the below diagram generally describes the message flow from issuing bank of the undertaking to the advising bank.

The beneficiary initiates the request for payment for the Guarantee/Standby LC, instructing the advising bank to demand for payment. The outward MT765 sent to the issuing bank to request for the payment.

> **⚠️ Note:** Non extension messages can be generated as a standalone message as well.

| Optional/ Mandatory | Field Tag | Field Name | Field Mapping | Description |
|---|---|---|---|---|
| M | 20 | Transaction Reference No | Alternate ID | Specifies the unique and unambiguous identifier assigned by the issuer of the undertaking. The field specification is 16x. When an advising bank relays the message to Advise Thru Bank, the Reference 1 field is mapped. |
| O | 21 | Related Reference | Reference 1 | Indicates the Reference 1 field. This field specifies the reference which has been assigned by the beneficiary of the undertaking or counter-undertaking. When an advising bank relays the message to Advise Thru Bank, the Reference 4 field is mapped. |
| M | 52A | Issuing Bank ID | Issuing Bk | Specifies the party that issued the undertaking. This is a mandatory field in MT785. The format is: - If the input in the field is a BIC, then the tag 52A is specified. - If the input in the field is ‘Name and address’ of the issuer, then the Tag 52D displays in the SWIFT message |
| M | 52D | Issuing Bank Address | Issuing Bk Name |  |
| M | 31C | Value Date | Value Date | Specifies the date on which the undertaking was issued. The field specification is 6!n |
| O | 59A | Beneficiary | Benef Cust 1 | Indicates the beneficiary customer 1. |
| O | 56A | Advising Bank ID | Advising Bk | Indicates the advising bank. |
| O | 56D | Advising Bank Address | Advising Bk Name | Indicates the advising bank name. |
| O | 57A | Advise Through Bank ID | Advice Thru Bk | Indicates the advising thru bank. |
| O | 57D | Advise Through Bank Add | Advice Thru Bk Name | Indicates the advising thru bank name. |
| O | 31E | Final Date of Expiry | MT785 Advice Expiry Date | Outward For outward message, when MT785 Advice Expiry Date is updated in MD.DEAL , then the same date is updated/replaced in Advice Expiry Date upon authorization of undertaking contract. After undertaking contract is authorised, the date is updated in both the fields ( MT785 Advice Expiry Date and Final Auto Ext Expiry Date ). When the authoriser rejects the changes, the new changes are not updated in the undertaking contract. The process has to be redone. The value present in MT785 Advice Expiry Date is mapped to Tag 31E field. Inward When the value is inputted in for MT785 Advice Expiry Date field, it is defaulted to Final Auto Ext Expiry Date if the Mt785 Advice Expiry Date field is not inputted and does not have any value. If the Final Auto Ext Expiry Date is not entered, the value in the MT785 Advice Expiry Date field is defaulted to Advice Expiry Date and is treated as the expiry date of the guarantee contract. The above defaulting happens for the recently received inward MT785 message. |
| O | 72Z | Sender to Receiver Info | MT785 Sender Info | To be mapped to Tag 72Z. The reason for non-extension can be entered by the issuing bank that is to be conveyed to the advising bank. For the incoming MT785 message, Tag 72Z must be mapped to the Received Bk Info field. |
| O | 23X | File Identification | MT785 File Identification | This field identifies the type of delivery channel and associated file name or reference.It must Contain any one of the following codes COUR EMAL FACT FAXT HOST MAIL OTHR |


##### Outward Processing of MT785

The outward processing of MT785 when the Issuing bank receives a claim /Demand for extension of the undertaking and the bank chooses the refuse the extension it generates MT 785 is illustrated below.

Details for the non-extension are entered and sent to MT765 initiated bank.

Sample preview of a MT785 generated is shown below.


##### Inward Processing of MT785

The inward processing of MT785 ,when the refusal inward MT 785 is received by the receiving bank is shown below.

The inward massage is lodged into the CL contract .


#### 📋 Tasks

Related topics:

- Generate Non-Extension Notification of Guarantee or Standby LC

Non extension of the Guarantee should be intimated to the beneficiary through one or more advising bank/advise thro bank about the non-extension when it is placed under automatic extension method. The non-extension of the referenced undertaking beyond the current expiry date.


##### Workflow

This section allows the user to perform the below tasks:

This menu allows the user to send notification for non-extension of issued guarantee beyond the expiry date.

To process the non-extension notification, follow the below steps:

1. Non-Extension Notification .
2. In the Guarantee Issued screen, click the Edit icon corresponding to a record.
3. In the Non Ext Notification screen, enter values in the mandatory and other required field values.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.


#### 📊 Outputs

There are no Outputs available for Non Extension of Guarantee feature.

---


### 3.12  Pay Reject Claim under Guarantee


> **📇 Quick Reference Card**
> 
> **Purpose:** *When a bank user receives a claim, it must be honoured within a reasonable period. If the guarantor decides to refuse the demand, it should be communicated immediately to the beneficiary. In case the bank is the beneficiary’s bank, it should immediately inform the beneficiary of such notice from the...*
> 
> **Key Fields:** *Claim Credit Account*, *Claim Debit Account*, *Claim Payment Method*, *Narrative*
> 
> **Sections:** 📖 Introduction | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

When a bank user receives a claim, it must be honoured within a reasonable period. If the guarantor decides to refuse the demand, it should be communicated immediately to the beneficiary. In case the bank is the beneficiary’s bank, it should immediately inform the beneficiary of such notice from the guarantor.


#### 📋 Tasks

Related topics:

- Issue Guarantee
- Process Response to Claim Under Guarantee (Received)
- Trade Finance and Guarantees Processes
- Pay or Reject Claim Under Standby LC
- Register Claim Under Standby LC (Received)

The Miscellaneous Deals or Guarantees module is used for recording the miscellaneous contingent deals that are required to record ‘Guarantee’ type transactions in the bank’s books.

The payment or rejection of the claim depends on the examination of the demand by the guarantor.


##### Workflow

This section allows the user to perform the below tasks:

This menu displays the list of guarantee received transactions over which invocation claim is registered and pending for further action of payment of claim or cancellation of claim as the case be.

To pay the claim of a guarantee received transaction, follow the following steps:

1. Pay/Reject Claim under Guarantee Received .
2. In the Pay/Cancel Claim on Guarantee screen, click the Pay Claim icon corresponding to a claim.
3. Enter the values in the mandatory fields such as, Claim Debit Account , Claim Payment Method and Claim Credit Account .
4. Click the Validate icon to check for errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

To reject the claim of a guarantee received transaction, follow the following steps:

1. Pay/Reject Claim under Guarantee Received .
2. In the Pay/Cancel Claim on Guarantee screen, click the Cancel Claim icon corresponding to a claim.
3. Enter a value in the Narrative field in the MT799 tab.
4. Click the Validate icon to check for errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to pay or reject a claim under guarantee.

To pay a claim under guarantee, follow the below steps:

1. Pay/Reject Claim under Guarantee .
2. In the Pay/Reject Claim under Guarantee screen, click the Pay Claim icon corresponding to a record.
3. In the Payment of Claim under Guarantee screen, enter values in the required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

To reject a claim under guarantee, follow the below steps:

1. Pay/Reject Claim under Guarantee .
2. In the Pay/Reject Claim under Guarantee screen, click the Reject Claim icon corresponding to a record.
3. In the Reject Claim Received under Guarantee screen, enter values in the required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to pay or reject a claim under standby LC issued.

To pay a claim under guarantee, follow the below steps:

1. Pay/Reject Claim under Standby LC .
2. In the Pay/Reject Claim under Standby LC screen, click the Pay Claim icon corresponding to a record.
3. In the Payment of Claim under Standby LC screen, enter values in the required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

To reject a claim under guarantee, follow the below steps:

1. Pay/Reject Claim under Standby LC .
2. In the Pay/Reject Claim under Standby LC screen, click the Reject Claim icon corresponding to a record.
3. In the Rejection Claim under Standby LC screen, enter values in the required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to pay or reject a claim under standby LC received.

To pay a claim under guarantee, follow the below steps:

1. Pay/Reject Claim under Standby LC .
2. In the Pay/Reject Invocation of Standby LC Received screen, click the Pay Claim icon corresponding to a record.
3. In the Payment of Claim under Standby LC Received screen, enter values in the required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

To reject a claim under guarantee, follow the below steps:

1. Pay/Reject Claim under Standby LC .
2. In the Pay/Reject Invocation of Standby LC Received screen, click the Cancel Claim icon corresponding to a record.
3. In the Reject Claim Received under Guarantee screen, enter values in the required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to pay or reject a claim under standby LC advised.

To pay a claim under guarantee, follow the below steps:

1. Pay/Reject Claim under Standby LC Advised .
2. In the Pay/Reject Invocation of Standby LC Advised screen, click the Pay Claim icon corresponding to a record.
3. In the Payment of Claim under Standby LC screen, enter values in the required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

To reject a claim under guarantee, follow the below steps:

1. Pay/Reject Claim under Standby LC Advised .
2. In the Pay/Reject Invocation of Standby LC Advised screen, click the Cancel Claim icon corresponding to a record.
3. In the Rejection of Claim under Standby LC screen, enter values in the required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.


#### 📊 Outputs

The Miscellaneous Deals or Guarantees module is used for recording the miscellaneous contingent deals that are required to record ‘Guarantee’ type transactions in the bank’s books.

The payment or rejection of the claim depends on the examination of the demand by the guarantor.


##### Enquiries and Reports

This section allows the user to view the below list of enquiries and reports of Pay/Reject Guarantees feature.

Guarantee Issued

This enquiry displays the details of invocation claims paid under guarantee.

Guarantee Received

This enquiry displays the details of invocation claims received under guarantee.


##### SWIFT Messages

NA


##### Advices

The below list of advices are generated by the core banking system pertaining to Pay or Reject Claim under Guarantee.

The advice is sent to the beneficiary as an acknowledgement for initiation of claim under inward guarantee.

The advice is sent to the guarantor stating that claim initiated stands cancelled.


##### Alerts

NA

---


### 3.13  Presentation under SBLC


> **📇 Quick Reference Card**
> 
> **Purpose:** *Presentation can either refer to the presentation of demand along with complying presentation documents (the act of delivering documents under an independent undertaking) or refer only to documents (the documents that are delivered). For an SBLC contract, this is governed as follows:*
> 
> **Key Fields:** *34b Amount*, *34b Tot Amount*, *750 Charges Added*, *750 Charges Deducted*, *750 Sender Info*, *754 Charges Added*, *754 Charges Deducted*, *@ ID* ... +61 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Presentation can either refer to the presentation of demand along with complying presentation documents (the act of delivering documents under an independent undertaking) or refer only to documents (the documents that are delivered). For an SBLC contract, this is governed as follows:

- ISP98 Rule 1.09(a) defines presentation as: Depending on the context, either the act of delivering documents for examination under a standby or the documents so delivered.
- URDG 758 Article 2 copies this approach, except it also includes: A presentation other than for a demand, for example, a presentation for the purpose of triggering the expiry of the guarantee or a variation of its amount.
- ISP98 Rule 3.02 states: The receipt of a document required by and presented under a standby constitutes a presentation requiring examination for compliance with the terms and conditions of the standby even if not all of the required documents have been presented.The rule implies that presentation does not occur merely by forwarding data or documents to an issuer or guarantor or nominated bank but forwarding them for honour which, in turn, requires examination to determine compliance with the terms and conditions of the undertaking.
- URDG 758 Article 2 also states the similar definition.

The presenter must make a presentation at the place and any location at that place indicated in the standby or provided in the rules that govern the undertaking. It can be:

1. At the place of business from where the standby was issued
2. At the place of business of the confirmer from where the confirmation was issued. It can be made: To the issuer or To the nominated bank whether or not the nominated person elects to act on the nomination. Unless a standby explicitly states that presentation cannot be made to a nominated bank, a nomination implies that presentation of documents may be made to the nominated bank whether or not the nominated person elects to act on the nomination.

Unless a standby explicitly states that presentation cannot be made directly to an issuing bank, presentation can always be made directly to the issuer or guarantor, thus bypassing nominated banks (including the confirmer).

As indicated in Chapter Two (Obligations of Parties to an Independent Undertaking), bypassing the confirmer may discharge the confirmer’s obligation depending on the applicable practice rule and the terms of the standby.

Since there is no provision in URDG 758 for confirmers or other nominated persons, presentation must be made to the issuer or guarantor unless the guarantee expressly provides otherwise. Accordingly, there can be multiple flows supported under presentation of documents:

When the beneficiary presents the documents against the claim, the issuing or the paying bank examines the presentation against the demand or invocation claim and executes or refuses the demand based on the presentation. The flow of registering the presentation and invocation claim go hand in hand or can be a separate process, but the status of the presentation determines if the bank can execute or refute the demand.

When it comes to support of new message types for SBLC cycle from MD based on the presentation and the invocation flow, the system conditionally triggers the delivery messages. The guarantor, the counterparties and the advising parties relay the below advices or messages between each other:

- Presentation of demand request – MT765
- Advice of discrepancy – MT750
- Refusal of the demand request – MT786
- Advice of discharge – MT732
- Authorisation to pay – MT752

Accordingly, following parties involved are important:

Issuing Bank: It is the entity that issues the undertaking. Usually, it is the party that has the authority to provide acceptance or rejection of documents under the SBLC undertaking at the request of the instructing party. Other parties can handle the documents and respond to the presentor based on the authority and instructions provided by the issuing bank.

Confirming Bank: It is the party that undertakes liability on behalf of the issuing bank under an SBLC undertaking and thus accepts claims from beneficiary. It cannot authorise other banks to pay or negotiate or reimburse on their own behalf; however, they can route such requests to the issuing bank and can send the claims on their acceptance.

Nominated Bank/Available With: The issuing bank with whom undertaking is made available, nominates and authorises this bank to pay or negotiate on behalf of issuing bank.

Presentor: The beneficiary can (either themselves or through their correspondent) route the presentation claim through the nominated bank or through another negotiating bank, in which case this bank sends MT750 requesting to pay or negotiate. For a nominated or negotiating bank, the presenter is the beneficiary whereas for an issuing or bank, nominated or negotiating bank is the beneficiary.

Beneficiary Bank: It captures the correspondent bank of the beneficiary.

Negotiating Bank : It captures the bank which has received documents from beneficiary and authorised to pay or negotiate on behalf of the negotiating bank.


#### ⚙️ Configuration

This feature has no specific configuration to be setup. The parameter applications are setup at the implementation stage.


#### 🔧 Working With

The following section describes Presentation under SBLC in detail.


##### Presentation of Documents Process Flow

As stated earlier, in case of Standby LC (SBLC) , both presentation and demand can be processed together or standalone. When both are generated together, the flow is indicated as below.

The beneficiary in the above case presents the required set of documents under SBLC along with the demand for claim for payment to their correspondent bank. This can be an Advise Through Bank or second advising bank in a presentation flow.


##### Presentation Register andMD.PRESENTATION.HIST

As part of SWIFT 2021 changes, the multi-value associated set of fields in MD.DEAL capture the details related to receipt of documents, handle examination of documents and record discrepancies. Together they constitute Presentation and Discrepancy Management in MD.

These set of fields is called the Presentation Register. They include the following:

| Field | Description |
|---|---|
| Docs Received | Specifies if the original documents are received by the bank. This is a mandatory field to trigger presentation of documents. Input in this field makes the multi-value set of fields, namely Presentation Date, Presentor Ref and Presentation Amount mandatory . The allowed values are: YES or NO. |
| Presentor Ref | Captures the reference number of the presentor when documents are received by the bank. The system maps the user input in this field to Tag 21 of outward MT732 after Discrep Status for the documents is updated as Accept or Waived. It takes up to 16 characters of 'x' character set. This is a mandatory field as part of generation of MT732 and should not begin with two slashes '//'. |
| Presentation Date | Specifies the date of receipt of documents. Input in this field enables the associated multi-value set under presentation register and prompts the user to input presentation details. The user has to input this field to enable generation of outward MT732. The system maps this field to Tag 30 of outward MT732, after Discrep Status for the documents are updated as Accept or Waived. This is a mandatory field for both registering presentation of documents under Standby LC and subsequent generation of MT732. Presentation Amount and Presentor Ref become mandatory fields when this field has input. |
| Presentation Amount | Captures the amount of presentation. The system maps the input in this field to Tag 32B of MT732, when Discrep Status for the documents is updated as Accept or Waived. Presentation Amount cannot be greater than Principal Amount. |
| Remarks | Stores any specific details related to a document presented. This field is for internal use, but is mandatory when Re Presentation is input, wherein this field captures the changes to the documents after revised presentation. This field takes input up to 50 lines of 65 characters of 'z' character set. |
| Re Presentation | This field record is updated when the user provides revised Presentation Documents, after the applicant rejects the first set of documents. When the Presentor presents the revised set of documents for the same Presentation, the user can update the fields and modify the records under the same presentation. For example, it accepts input as YES or NO. After this field is updated, the Remarks field becomes a mandatory field. |
| Docs Present | Captures document-specific identification/type. For example, Invoices, Certificate of Origin and Certificate of Completion. |
| Presentation Status | Captures if documents are clean or discrepant. Based on the same, the system generates Acceptance or Rejection messages. |
| Discrep Status | Captures applicant's response to the discrepancies recorded in presentation or received from presenting bank, whether accepted or to be rejected. Generation of outward MT732 depends on input in this field ( MT732 content - Advice by Issuer to take up Acceptance/Payment against documents received with discrepancies). The allowed vales are ACCEPT, WAIVE or REJECT. |
| Advised Status | Captures the bank's response to the discrepancies recorded in presentation or received from the presenting bank, whether accepted or to be rejected. Generation of outward MT732 depends on input in this field (MT732 content - Advice by Issuer to take up Acceptance/Payment against documents received with discrepancies). The allowed values are: Advised to applicant Pending with beneficiary Presented through advising bank Presented through pay/issuing bank |

> **⚠️ Note:** Presentation date, Presentation reference, Docs received, Presentation amount are mandatory fields in the presentation multi-value set.

For each Presentation of documents, the user updates a multi-value set with the requisite values. On authorisation, the system generates applicable outward SWIFT details and these set of values are mapped onto MD.PRESENTATION.HIST.

MD.PRESENTATION.HIST

This table captures the history of presentations made and used for matching with demand claim received against the presentation. It takes record based on ID of MD.DEAL , consists of multi-value associated set of fields wherein each being a corresponding record from Presentation Register. When a document is registered under a Standby undertaking and authorised, the system creates a new sequence under MD.PRESENTATION.HIST with values from Presentation Register populated to the same.

Once the user authorises the MD.DEAL , the system updates the MD.PRESENTATION.HIST with the presentation details under the contract. This system updates the table at the time of presentation of documents, any changes to the discrepancies status and the related invocation claim number updated.

During an Invocation Claim received, the user has to link invocation with Presentations recorded. This linkage happens through the Presentation for Claim field.

User has to specify the Presentation sequence number in this field. This value comes from multi-value serial no. from MD.PRESENTATION.HIST . Thus, the invocation claim and presentation are linked.


##### Presentation for Claim

When the invocation is received, the Presentation For Claim field is updated with presentation number(Example: 1,2,3 and so on). This tags the respective presentation with the demand claim and updates in the MD.INVOCATION.HIST This field is serial number from multi-value set from MD.PRESENTATION.HIST . Thus, every invocation demand record from MD.INVOCATION.HIST is linked with the MD.PRESENTATION.HIST .

The following screenshots show the process of registering documents presented under Standby LC and MD.PRESENTATION.HIST :

The following screenshots show the presentation along with inward MT765:

The following screenshot shows linking invocation and presentation during settlement:


##### Nominated/Negotiating Bank receives Presentations

When the beneficiary presents the documents to the nominated bank, the bank user checks the Docs Received (Documents Received ) field . The system prompts the user to enter values in a set of associated multi-value fields. Update the Presentation Date , Presentation Amount , Presentor Ref , Docs Present from the documents and based upon document examination the user updates Presentation Status, Discp Status and Advised Status . Presentation date is a multi-value field with its others fields as sub-value under it, to accommodate multiple presentation under multiple demands.

The nominated bank (who acts as the presentor) can generate the MT750 message type, requesting the issuing bank to take up the discrepancies, if any , while updating the presentation details.


##### Issuing Bank/Confirming Bank/ receives Presentations

When the paying bank or issuing bank receives the presentation, the bank user has to manually register the presentation of the documents in the related fields. The bank user updates the Presentation Date, Presentation Amount, Presentor Ref, Docs Present from the documents received, and based on document examination, the system updates Presentation Status, Discp Status and Advised Status . Instructing Party is advised on the presentation of the documents, if it’s a clean or discrepant presentation.

In case of discrepant documents, instructing party may decide to take up or reject the discrepancies. The paying bank / issuing bank can generate MT732 to advise the discharge of discrepancies if documents are taken up. In case, MT750 message type is already received, the system relays MT752 as a response to the inward messages instead of MT732.

As a receiving bank, when inward MT750 or MT754 is received, the message is available in the enquiry. Inward tags are not mapped to the contract. The bank user can manually register the presentation on the receipt of the swift message MT750 or MT754 and update the Docs Present field if original presentation is received or not. The receiving bank can view the inward swift message and its contract from the enquiry. If required they can pick the contract in edit mode to generate MT752 as a response to MT750 and MT756 if the documents are clean.

The user may opt to generate MT786 in case of discrepant document (Here, MT786 message can be triggered only when MT765 is received).


##### Other Presentation Scenarios

The presentation can be registered while:

- The demand or invocation request (MT765) is submitted by the beneficiary already, and claim registered already or
- Maybe registered after the presentation of documents or
- Presentation & register of claim can be done at the same time.

The existing invocation process remains the same for generation of the outward MT765.

The bank user should link the presentation with the respective invocation claim for easy trace of the respective presentation and its demand claim in case of multiple or partial demands.


##### Presentation SWIFT Messages Flow

The following section describes the MT732, MT750,MT752,MT754 and MT756 messages in detail.

| Tag Status | Field Tag | SWIFT Tag | Inward Field Mapping | Outward Field Mapping |
|---|---|---|---|---|
| M | 20 | Sender's TRN | Reference 1 | Alternate Id Or @Id Or Reference.1 |
| M | 21 | Presenting Bank's Reference | Presentor Ref | Presentor Ref |
| M | 30 | Date of Advice | Presentation Date | Presentation Date |
| M | 32B | Amount of Utilisation | Presentation Amount | Presentation Amount |
| O | 72Z | Sender to Receiver Information | Mt732 Sender Info | Mt732 Sender Info |

| Tag Status | Field Tag | SWIFT Tag | Inward Field Mapping | Outward Field Mapping |
|---|---|---|---|---|
| M | 20 | Sender's Reference | Presentor Ref | Presentor Ref Or Alternate Id Or @ Id |
| M | 21 | Related Reference | Alternate ID @ID Or Reference 1 | Reference 1 |
| M | 32B | Principal Amount | Presentation Amount | Presentation Amount |
| O | 33B | Additional Amount | Add Claim Amount | Add Claim Amount |
| O | 71D | Charges to be Deducted | 750 Charges Deducted | 750 Charges Deducted |
| O | 73A | Charges to be Added | 750 Charges Added | 750 Charges Added |
| O | 34B | Total Amount to be Paid | 34b Tot Amount | 34b Tot Amount |
| O | 57A | Account With Bank | Acct With Bank | Acct With Bank |
| O | 72Z | Sender to Receiver Information | 750 Sender Info | 750 Sender Info |
| M | 77J | Discrepancies | Reason For Refuse | Reason For Refuse |

| Tag Status | Field Tag | SWIFT Tag | Inward Field Mapping | Outward Field Mapping |
|---|---|---|---|---|
| M | 20 | Documentary Credit Number | Reference 1 | Alternate Id Or @ Id Or Reference.1 |
| M | 21 | Presenting Bank's Reference | Presentor Ref Or Alternate Id Or @ ID | Presentor Ref |
| M | 23 | Further Identification | MT752 Further Identification | MT752 Further Identification |
| M | 30 | Date of Advice of Discrepancy or Mailing | MT752 Advice Date | MT752 Advice Date |
| O | 32B | Total Amount Advised | 34b Tot Amount | 34b Tot Amount |
| O | 71D | Charges Deducted | MT752 Chgs Deducted | MT752 Mt752 Chgs Deducted |
| O | 33A | Net Amount | Net Amount | Net Amount |
| O | 53A | Sender's Correspondent | Our Corrs Bnk | Our Corrs Bnk |
| O | 54A | Receiver's Correspondent | Recv Corrs .Bnk | Recv Corrs Bnk |
| O | 72Z | Sender to Receiver Information | MT752 Sender Info | MT752 Sender Info |
| O | 79Z | Narrative | MT752 Narrative | MT752 Narrative |

| Tag Status | Field Tag | SWIFT Tag | Inward Field Mapping | Outward Field Mapping |
|---|---|---|---|---|
| M | 20 | Sender's Reference | Presentor Ref | Presentor Ref Or Alternate Id Or @ Id |
| M | 21 | Related Reference | Alternate Id / @Id Or Reference 1 | Reference.1 |
| M | 32A | Principal Amount Paid/Accepted/Negotiated | Presentation Amount | Presentation Amount |
| O | 33B | Additional Amount | Add Claim Amount | Add Claim Amount |
| O | 71D | Charges to be Deducted | 754 Charges Deducted | 754 Charges Deducted |
| O | 73A | Charges to be Added | 754 Charges Added | 754 Charges Added |
| O | 34A | Total Amount Claimed | 34b Tot Amount | 34b Tot Amount |
| O | 53A | Reimbursing Bank | Third Party Cust No / Third Party Cust | Third Party Cust.No / Third Party Cust |
| O | 57A | Account With Bank | Acct With Bank | Acct With Bank |
| O | 58A | Beneficiary Bank | Bene Bnk.Id / Bene Bnk Name | Bene Bnk Id / Bene Bnk Name |
| O | 72Z | Sender to Receiver Information | MT754 Sender Info | MT754 Sender Info |
| O | 77 | Narrative | MT754Narrative | MT754 Narrative |

| Field Tag | SWIFT Tag | Tag Status | Inward Field Mapping | Outward Field Mapping |
|---|---|---|---|---|
| 20 | Documentary Credit Number | M | Reference 1 | AlternateId Or @ Id Or Reference.1 |
| 21 | Presenting Bank's Reference | M | Presentor Ref Or Alternate Id Or @ Id | Presentor Ref |
| 32B | Total Amount Claimed | M | 34b Amount | 34b Tot Amount |
| 33A | Amount Reimbursed or Paid | M | Net Amount | Net Amount |
| 53A | Sender's Correspondent | O | Our Corrs Bnk | Our Corrs Bnk |
| 54A | Receiver's Correspondent | O | Recv Corrs Bnk | Recv Corrs Bnk |
| 72Z | Sender to Receiver Information | O | MT756 Sender Info | MT756 Sender Info |
| 79Z | Narrative | O | MT756Narrative | MT756 Narrative |


#### 📋 Tasks

Related topics:

- Register Claims
- Trade Finance and Guarantees Processes
- Accept or Reject Documents Presented Under Standby LC
- Forward Claim Under Standby LC (Advised)
- Register Documents Presented Under Standby LC (Received)

Presentation under standby LC signifies the act of delivering documents under an independent undertaking and sometimes also to signify the documents that are delivered. For an SBLC contract it is defined as per ISP98 rule.


##### Workflow

The user can perform the presentation under standby LC using the workflow below:

This menu allows the user to register the presentation of an issued Standby LC.

To register a presentation under Standby LC, follow the below steps:

1. Register Presentation under Standby LC .
2. In the Register Presentation Under Standby LC screen, click Register Presentation icon corresponding to a record.
3. In the Presentation for Standby LC screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to register presentation under standby LC received.

To register the presentation under standby LC received, follow the below steps:

1. Register Presentation under StandbyLC .
2. In the Register Presentation Under Standby LC Received screen, click the Register Presentation icon corresponding to a record.
3. In the Presentation for Standby LC screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to send advice response to presentation under standby LC.

To register presentation under standby LC, follow the below steps:

1. Advise Response to Presentation under Standby LC .
2. In the Advise Response to Presentation under Standby LC screen, click the Register Presentation icon corresponding to a record.
3. In the Presentation for Standby LC screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.


#### 📊 Outputs

There are no Outputs available for Presentation under Standby Letter of Credit feature.

---


### 3.14  Register Claim under Guarantee


> **📇 Quick Reference Card**
> 
> **Purpose:** *A beneficiary may demand, claim against, invoke, draw upon or call on a guarantee. They always invoke a bank guarantee, when there is a case of not honouring the principal contract. The duty of a guarantor under a guarantee is to pay the sum(s) therein stated on the presentation of a written demand ...*
> 
> **Key Fields:** *Demand Type*, *Inv
 Status*, *Inv Status*, *Reason for Refuse*
> 
> **Sections:** 📖 Introduction | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

A beneficiary may demand, claim against, invoke, draw upon or call on a guarantee. They always invoke a bank guarantee, when there is a case of not honouring the principal contract. The duty of a guarantor under a guarantee is to pay the sum(s) therein stated on the presentation of a written demand for payment and other documents specified in the guarantee.

On receiving a claim or demand, the guarantor must examine the claim, honour it in a given period, and if necessary, reject and inform those concerned immediately. In case of the beneficiary’s bank, the bank forwards the claim to the guarantor. When the claim is honoured, the beneficiary’s bank must make the payment to the beneficiary or in case of rejection inform the beneficiary accordingly.


##### Swift 2021 Changes

The Logic of Registration of claim remains the same ,However a new message is introduced during the course of event namely MT 765 as a part of claim registration process. This message is generated by Beneficiary’s correspondent Bank to the Issuing bank . The relevant SWIFT tags and field mapping in MD are indicated in MT765 .

During the register of claim, based on the input in Demand Type , the user has to handle the invocation in two ways described below.

Demand Payment Flow

Register of Claim Pay/Refuse Claim Undertaking issued Inward MT765 is received for extension with Demand Type mentioned as PAYM Pay: Payment initiated Refusal: Transact bank sends outward MT786 towards the sender of MT765 Undertaking Received Inv Status set as PROCESS Demand Type updated as PAYM Outward MT765 is issued towards the Issuer of the MT760 Pay: Payment received for demand Refusal: Transact bank receives inward MT786 and advises the beneficiary.

Demand Extension Flow

Register of Claim Pay/Refuse Claim Undertaking issued Inward MT765 is received for extension with Demand Type mentioned as PAEX Issuing bank advises the Instructing Party. Extend: When instruction party accepts issuing bank processes the extension by generating a MT 767 to the receiver. When the receiver sends MT787 and issuing bank processes the same, user to set Inv Status as CANCEL manually. Stating the reason for cancellation as ‘Undertaking extended as per beneficiary’s claim.’in Reason for Refuse . Refusal: Outward MT785 issued to the receiver. Based upon beneficiary’s response either claim is processed or cancelled Undertaking received Inv Status set as PROCESS Demand Type updated as PAEX Outward MT765 is issued towards the Issuer of the MT 760 Extend: Inward MT767 is received and advised to Beneficiary. When beneficiary accepts MT787 is sent to the issuing bank. User to manually change Inv Status as CANCEL ‘Undertaking extended by Issuing Bank and accepted by beneficiary . Refusal: Inward MT785 received and advised to beneficiary


##### SWIFT 2023 Changes in Claim

As a part of SR 2023, the below field is available in MT765 to record the new expiry date of the local undertaking.

| Status | Tag | Field Name | Content/Options |
|---|---|---|---|
| O | 31R | Requested New Date of Expiry of Local Undertaking | 6!n |


#### 📋 Tasks

Related topics:

- Amend Guarantee or Standby LC
- Register Claims Under Guarantee (Received)
- Trade Finance and Guarantees Processes

A Bank Guarantee is issued by a lending institution, which promises to cover the loss if a borrower defaults on a loan. The guarantee lets a company buy what it otherwise could not, helping business growth and promoting entrepreneurial activity.

When an invocation claim is received from the beneficiary under an Inward guarantee advised by the bank, the bank can initiate the claim in the system and send the claim to the Issuing bank/Guarantor on behalf of the beneficiary. If needed, the bank can settle the claim by crediting the beneficiary on receipt of funds from the issuing bank. The bank can also cancel the claim in the system. This displays all the ‘Guarantee Received’ contracts. If there is any claim received under this guarantee, the user can register the details of the guarantee from this bank.


##### Workflow

This section allows the user to perform the below tasks:

| SCREENS | WORKFLOW |
|---|---|
|  | Pending with Bank . |
| Internet Claim Requests – Pending with Bank | Click the View Request icon corresponding to a record to view the claim request. |
| Internet Claim Requests – Pending with Bank | Click the Query/Action icon corresponding to a record to send a query or to action on the request. |
| Internet Claim Requests – Pending with Bank | Click the View Gtee icon corresponding to a record to view the guarantee details of the requested claim. |

This menu allows the user to register the details of Arts and Antiques held on behalf of the customers.

To register the details of Arts and Antiques, follow the following steps:

1. Art & Antiques Register .
2. In the Art & Antiques Register screen, enter the mandatory and other required field values.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.

| SCREENS | WORKFLOW |
|---|---|
|  | Register Claim under Guarantee . |
| Register Claim Under Guarantee | Click the FIND button. |
| Register Claim Under Guarantee | Click the Register Claim icon corresponding to a record. |
| Register Claim under Guarantee | Enter values in the mandatory and other required fields. Click the Validate icon to check for errors and overrides. Click the Delivery Preview icon to view the delivery messages. Click the Commit icon to submit the record. |

This menu allows the user to register a claim of an issued standby LC.

To register a claim under standby LC, follow the below steps:

1. Register Claim under Standby LC .
2. In the Register Claim Under Standby LC screen, click the Register Claim icon corresponding to a record.
3. In the Register Claim under Standby LC screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to register claim under standby LC received.

To register claim under standby LC received, follow the below steps:

1. Register Claim under Standby LC .
2. In the Register Claim Under Standby LCs Received screen, click the Initiate Claim icon corresponding to a record.
3. In the Register Claim under Standby LC Received screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to register claim for the standby LC advised.

To register a claim under standby LC received, follow the below steps:

1. Register Claim under Standby LC Advised .
2. In the Register claim under Standby LCs Advised screen, click the Initiate Claim icon corresponding to a record.
3. In the Register Claim under Standby LC screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This menu allows the user to register claim under guarantee received.

To register a claim under guarantee received, follow the below steps:

1. Register Claim under Guarantee Received .
2. In the Guarantees Received screen, click the Initiate Claim icon corresponding to a record.
3. In the Register Claim under Guarantee received screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.


#### 📊 Outputs

Model Bank supports and records the details of Arts and Antiques held on-behalf of customers.


###### Enquiries and Reports

NA


###### SWIFT Messages

The user can view the below SWIFT messages, enquiries and reports while processing and after processing the inward collections.

This message is sent by the party that issued the undertaking to a bank as the beneficiary or to the presenter of the demand. This message type is used only for standby LCs.

This message is used to notify the beneficiary through one or more advising parties of the non-extension of the referenced undertaking beyond the current expiry date, if applicable.

This message is used to demand a payment under an undertaking, and it includes a request to extend the expiry date.


###### Advices

The below list of advices are generated by the core banking system pertaining to Enquiries.

The below advices generates when the user records the details of arts and antiques held on behalf of customers.


###### Alerts

NA

---


### 3.15  Reimbursement Processing SBLC


> **📇 Quick Reference Card**
> 
> **Purpose:** *As part of Swift changes 2020, Temenos Transact can handle the reimbursement cycle for SBLC from the MD module now. As SBLCs can be issued using the MT760 messages and not using MT700, it is deactivated from LC module.*
> 
> **Key Fields:** *31E*, *31E, 32B, 33B, 34B, 39A, 39C, 72Z*, *32B or 33B*, *32B, 33B and 34B*, *34B*, *34a Tot Amount*, *34b Tot Amount*, *740  Applicable Rule, Presentation Amount* ... +67 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

As part of Swift changes 2020, Temenos Transact can handle the reimbursement cycle for SBLC from the MD module now. As SBLCs can be issued using the MT760 messages and not using MT700, it is deactivated from LC module.

Reimbursement Processing includes generation of outward reimbursement-related messages, handling inward reimbursement messages, creation of reimbursement record in case of reimbursement bank, handling amendment and maintenance of the reimbursement record and register of claim and payment of reimbursement.

A reimbursement bank is Nostro bank of the Issuing bank, who are authorised to by them to make payment on their behalf upon receipt of complying claim from pay/negotiating bank and reimburse from them

The reimbursing bank, often located in the country of the SBLC currency, allows an issuing bank to utilise the foreign currency it holds on an account with that bank, rather than face exchange rate risks associated with converting local to a foreign currency on a payment-by-payment basis. Therefore an issuing bank nominates another bank (a reimbursing bank) to provide reimbursement on its behalf.

In such circumstances, the issuing bank, at the time of issuing its SBLC, should send a reimbursement authorisation to the reimbursing bank instructing it to reimburse the claiming bank (a named nominated bank or any bank with SBLC available).

The reimbursing bank only makes payment against a complying claim if funds are available in the account of the issuing bank, or when there is a sufficient overdraft facility in place, unless it has issued its own Irrevocable Reimbursement Undertaking (IRU). An IRU irrevocably binds the reimbursing bank to honour a complying demand.

A reimbursing bank has no concern with regard to the documents that are presented under the SBLC and whether they are compliant or not.

Bank-to-bank reimbursements are made subject to the Uniform Rules for Bank-to-Bank Reimbursements under Standby Letter of Credit, ICC Publication No. 725 ("URR 725") or URDG 758 sub-article 15 and article 24.

The Reimbursement Cycle under Standby Letter of Credit is illustrated below:

The parties involved are:

- Reimbursing Bank – Nostro owner of issuing bank
- Issuing bank authorizes to settle or reimburse on behalf of issuing bank
- Roles: Applicant – Issuer Issuing Bk – Reimbursing Bank Available With Bank, Pay or Negotiating Bank – Beneficiary

The Guarantor, claiming and the reimbursing banks relay below advices/messages between each other:

- Authorisation to reimbursement claim – MT740
- Reimbursement claim – MT742
- Notice of non-confirming reimbursement claim - MT744
- Amendment to authorization of reimbursement - MT747
- Advice of reimbursement - MT756
- Pre-debit notification - MT759


#### ⚙️ Configuration

The initial configuration of SBLC Reimbursement to register it as reimbursement record in Temenos Transact, requires the configurations in parameter table. The bank user defines the Reimbursement record as CL contract with Deal Sub Type as REIMB in both the MD.PARAMETER and MD.DEAL.TYPE.PARAMETER parameter tables. Also, allowed deal type is SBLC for REIMB types of CL contracts in both the tables.

The Deal Sub Type in MD.PARAMETER to be created as REIMB under Contract Type Cl is shown below.

The Deal Sub Type in MD.DEAL.TYPE.PARAMETER to be created as REIMB under Contract Type Cl is shown below.


#### 🔧 Working With

The following diagram shows the process flow of Reimbursement Messages between issuing and reimbursement bank:

During the issuance of the guarantee, in case the parties involved in the undertaking prefers to add a reimbursement to the standby letter of credit (SBLC), the issuing bank can generate an MT740 to the reimbursing bank.

The bank generates this message only for SBLC form of undertaking and for CA type of contracts.


##### MT740 - Authorisation to Reimbursement Claim

The MT740 authorises the reimbursing bank to debit the account of the sender, or one of the sender’s branches (if so indicated) for reimbursements effected in accordance with the instructions in the MT740.

The issuing bank can be a counter-counter SBLC, counter SBLC or local SBLC issuing bank. It is used to request the receiver to honour claims for reimbursement of payment or negotiation(s) under a documentary credit.

The fields structure and mapping are tabulated below:

| Optional or Mandatory | Tag | SWIFT Tag | Content or Options | Field Mapping |
|---|---|---|---|---|
| M | 20 | Documentary Credit Number | 16x | Alternate Id |
| O | 25 | Account Identification | 35x | Mt740 Account No |
| M | 40F | Applicable Rules | 30x | Mt740 Applicable Rule |
| O | 31D | Date and Place of Expiry | 6!n29x | Last Present Date Last Present Place |
| O | 58a | Negotiating Bank | A or D | Negotiating Bk Negotiating Bk Name |
| O | 59 | Beneficiary | (/34x) 4•35x | Ben Address |
| M | 326 | Credit Amount | 31a15d | Currency Principal Amount |
| O | 39A | Percentage Credit Amount Tolerance | 2nt2n | Percentage Cr Tolerance |
| O | 39C | Additional Amounts Covered | 4*35x | MT740 Add Claim Amt |
| M | 41a | Available With ...By .. | A orD | Available With Available By |
| O | 42C | Drafts at.. | 3•35x | Drafts At |
| O | 42a | Drawee | A orD | Drawee Cust No Drawee |
| O | 42M | Mixed Payment Details | 4*35x | Mixed Payment Detail |
| O | 42P | Negotiation/Deferred Payment Details | 4*35x | Neg Def Payment Detail |
| O | 71A | Reimbursing Bank"s Charges | 31a | Reimb Chrg Party |
| O | 71D | Other Charges | 6*35z | MT740 Other Chrgs |
| O | 72Z | Sender to Receiver Information | 6*35? | MT740Sender Info |


##### Conditions for MT740 to be Triggered from Issuing Bank

The system triggers an MT740 message only when the Third Party Cust No field is input with valid customer with BIC.

740 Applicable Rule, Presentation Amount and Available With are mandatory to generate outward MT740 message

Validations for these fields are:

Presentation Amount cannot exceed the Principal Amount . Temenos Transact generates an override: Credit amount is greater than the guarantee outstanding. The date on which the reimbursement authorisation is sent should be stored in the 740 Reimb Dtd field.

The user has to set the Tag 41A in MT740 functionally as BY PAYMENT instead of By Acceptance, By Def Payment , By Mixed Pymt Or By Negotiation even though SWIFT allows the input of the above.

The following screenshot shows the outward MT740 generation page:

Processing of Inward MT740 by Reimbursement Bank

When the reimbursement bank receives the MT740, the user has to fetch the messages from the repair queue as the user only maps fields with the Temenos Transact application and enters the Input Authority for reimbursement.

The following screenshots process of reimbursement messages to register the authority for the guarantee:

After the user lodges the Authority in the system, if the reimbursement bank is required to acknowledge the same it can generate an outward MT759 manually.


##### Process of Amendment of Reimbursement Messages

When the issuing bank prefers to amend the MT740 reimbursement message already sent to the reimbursement bank, it can send an amendment. Any one of the following scenarios arises in the Stand by Letter of Credit contract.

- Amendment of principal amount
- Change of beneficiary or the bank or change in Third Party Cust No (reimbursement bank)
- Any change in undertaking details to be intimated to the reimbursement bank

The bank enters the details in the MT747 details under Amendment of Guarantees.

It is used to inform the Receiver about amendments to the terms and conditions of the credit relevant to the authorisation to reimburse. The amendment is to be considered as part of the authorisation to reimburse. Issuing bank sends outward MT747 toward the reimbursing bank for Amendment to Authorisation to reimburse.

The conditions for MT747 message to be triggered by issuing bank are listed below:

- The bank generates this message generated only for SBLC form of undertaking.
- 740.Reimb.Dtd is mandatory to generate an outward MT747 message from the issuing bank.
- The bank generates an MT747 message from CA type of contracts only.
- The bank generates an MT747 message only when the Third Party Cust No field is input with valid customer with BIC. When Third Party Cust No is not null, the system sends the outward message to the bank mentioned in this field.

The following are network validations and Temenos Transact generates an error even when one of the rules is not met:

- At least one of the 31E, 32B, 33B, 34B, 39A, 39C, 72Z or 77 fields must be present.
- If either 32B or 33B field is present, then the 34B field must also be present.
- If the 34B field is present, the 32B or 33B field must also be present.
- The currency code in the amount fields 32B, 33B and 34B must be the same.

During the amendment event, the issuing bank also sends out the MT 747 to amendment of reimbursement instructions, which are already conveyed through MT 740. For an event, where the amendment is reject by the beneficiary, the issuing bank changes reinstate the amendment change and must send out a MT 759 to the reimbursement bank manually to cancel the MT 747 amendment change for the contract .

In case the issuing bank prefers to change the reimbursement bank, it must add

outward MT747 with the 72Z field set as CANC to cancel the reimbursement authority and send to the given bank. The issuing bank can generate a new MT740 to the amended bank under Third Party Cust No. .

Any new latest date for a reimbursement claim or a new expiry date for the reimbursement authorisation must be indicated in this field and not in the 31E field.

When this field is used to indicate if pre-debit notification from the reimbursing bank to the issuing bank is required, the number and type, that is, banking or calendar of days within which the issuing bank must be notified should also be indicated.

| Tag Status | Field Tag | SWIFT Field Name | Length | Field Mapping |
|---|---|---|---|---|
| M | 20 | Documentary Credit Number | 16x | Reference 1 |
| O | 21 | Reimbursing Bank's Reference | 16x | Alternate Id Or @Id |
| M | 30 | Date of the Original Authorisation to Reimburse | 6!n | 740 Reimb Dtd |
| O | 31E | New Date of Expiry | 6!n | MT767 Advice Expiry Date |
| O | 32B | Increase of Documentary Credit Amount | 3!a15d | Inc Dec Amount |
| O | 33B | Decrease of Documentary Credit Amount | 3!a15d | Inc Dec Amount |
| O | 34B | New Documentary Credit Amount After Amendment | 3!a15d | New Doc Amt |
| O | 39A | Percentage Credit Amount Tolerance | 2n/2n | Percentage Tolerance |
| O | 39C | Additional Amounts Covered | 4*35x | New Add Claim Amount |
| O | 72Z | Sender to Receiver Information | 6*35z | MT767 Sender Info |
| O | 77 | Narrative | 20*35z | MT767 Narrative |


##### Reimbursement Claim Process by Advising bank to Reimbursement Bank

When an advising bank makes a claim for the undertaking, the system allows the user to raise MT742 to the reimbursement bank for the reimbursement of the claim amount, along with demand claim from the issuing bank (or along with MT754 reimbursement message to the issuing bank). The system allows triggering a MT742 message only when the user has captured input in Third Party Custno . There is a possibility of two scenarios based on whether the reimbursement bank honours or rejects the payment.

| Field Tag | SWIFT Field Name | Tag Status | Field Mapping |
|---|---|---|---|
| 20 | Claiming Bank's Reference | M | Alternate ID Or @ID |
| 21 | Documentary Credit Number | M | Referenec 1 |
| 31C | Date of Issue | O | Value Date |
| 52A | Issuing Bank | M | Issuing Bk |
| 32B | Principal Amount Claimed | M | Inv Amount |
| 33B | Additional Amount Claimed as Allowed for in Excess of Principal Amount | O | Add Claim Amount |
| 71D | Charges | O | MT742 Chrgs Deducted |
| 34A | Total Amount Claimed | M | 34a Tot Amount |
| 57A | Account With Bank | O | Acct With Bank / Acct With Bank Id |
| 58A | Beneficiary Bank | O | Bene Bank Id / Bene Bank |
| 72Z | Sender to Receiver Information | O | MT742 Sender Info |

| Optional/Mandatory | Field Tag | Field Name | Format | Field Mapping |
|---|---|---|---|---|
| M | 27 | Sequence of Total | 1!n/1!n | Auto Populated |
| M | 20 | Transaction Reference Number | 16x |  |
| O | 21 | Related Reference Number | 6x | MT759 Rel Ref |
| M | 22D | Form of Undertaking | 4!c | MT759 Form Of Undk |
| M | 23 | Undertaking Number | 16x |  |
| O | 52A | Issuer | A or D |  |
| M | 23H | Function of Message | 8!c | MT759 Function |
| M | 45D | Narrative | 150*65z | MT759 Narrative |
| O | 23X | File Identification | 4!c/65 |  |

| Tag Status | Field Tag | SWIFT Field Name | Length | Outward Mapping details |
|---|---|---|---|---|
| M | 20 | Sender's Reference | 16x | Alternate Id Or @ID |
| M | 21 | Claiming Bank's Reference | 16x | Reference 6 |
| M | 52A | Issuing Bank | A or D | Issuing Bk |
| M | 21A | Documentary Credit Number | 16x | Reference 1 |
| O | 31C | Date of Issue | 6!n | Value Date |
| M | 34A | Total Amount Claimed | A or B | 34a Tot Amount |
| M | 73R | Reason for Non-Payment | 4!c[/35x] | Reason Non Pmt |
| M | 73S | Disposal of Reimbursement Claim | 4!c[/35x] | Disp Of Reimb Claim |
| O | 71D | Reimbursing Bank's Charges | 6*35z | MT744 Reimb Bk Chrgs |
| O | 72Z | Sender to Receiver Information | 6*35z | MT744 Sender Info |


#### 📋 Tasks

Related topics:

- Forward Response Received for Claim Under Standby LC (Advised)
- Process Response to Claim Under Standby LC (Received)
- Receive Claim Under Standby LC

A standby letter of credit reimbursement agreement, under which a bank agrees to issue standby letters of credit on behalf of its customer, the applicant, and the customer agrees to reimburse the bank if the bank makes payments under the standby credit.


##### Workflow

This section allows the user to perform the below reimbursement activities:

This tab allows the user to record the reimbursement authorisation received from the issuing bank by SWIFT MT740.

To create a new authority, follow the below steps:

1. Input Authority .
2. In the Input and Modified Unauthorised Authorities screen, click the New Authority icon corresponding to a record.
3. In the Reimbursement Authority screen, enter values in the mandatory and other required field values.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

To amend an existing authority, follow the below steps:

1. Input Authority .
2. In the Input and Modified Unauthorised Authorities screen, click the Modify icon corresponding to a record.
3. In the Reimbursement Authority screen, modify the required field values.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This tab allows the user to record the amendments received (MT747) from the issuing bank for the existing reimbursement authorisation.

To record the amendments on reimbursement authorisation, follow the below steps:

1. Amend Authority .
2. In the list of Reimbursement Authorities screen, click the Amend icon corresponding to a record.
3. In the Reimbursement Amendment screen, amend values in the required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This tab allows the user to register a reimbursement claim for which the user not holding a reimbursement authority. Therefore, a dummy authority is created to follow up with the issuing bank.

To view the awaiting authority, follow the below steps:

1. Awaiting Authority .
2. In the Authorities created without MT740 based on claim screen, click the View icon corresponding to a record.

To modify a reimbursement authority, follow the below steps:

1. Awaiting Authority .
2. In the Authorities created without MT740 based on claim screen, click the Authority Recd icon corresponding to a record.
3. In the Reimbursement Authority screen, modify the required field values.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

To register a claim with the dummy authority, follow the below steps:

1. Awaiting Authority .
2. In the Awaiting Authorities created without MT740 based on claim screen, click the Register Claim icon corresponding to a record.
3. In the Register Reimbursement claim screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This tab allows the user to register a reimbursement claim received from the claiming bank through SWIFT MT742.

To register a claim received from the claiming bank, follow the below steps:

1. Register Claim .
2. In the Register Reimbursement Claims screen, click the Register Claim icon corresponding to a record.
3. In the Register Reimbursement claim screen, enter values in the mandatory and other required field values.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This tab allows the user to pay fresh claims with current value date and the claims that are registered earlier whose value date falls on current date.

To pay a claim, follow the below steps:

1. Pay Claims .
2. In the List Of Claims Pending screen, click the Pay Claim icon corresponding to a record.
3. In the Payment of Claim under Guarantee screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

To cancel/reject a claim, follow the below steps:

1. Cancel/Reject Claims .
2. In the List of Claims to be Modified or Rejected screen, click the Cancel/Reject icon corresponding to a record.
3. In the Reject Claims under Export LC screen, enter values in the mandatory and other required fields.
4. Click the Validate icon to check for the errors and overrides.
5. Click the Delivery Preview icon to view the delivery messages.
6. Click the Commit icon to submit the record.

This tab displays the list of unauthorised records that are created through inward messages and consists of the following sub-tabs:

This tab displays the list of unauthorised records of MD.DEAL application that are created through the MT740 inward messages.

To amend and view the inward messages, follow the below steps:

1. Inward Messages .
2. Click the Modify icon to enter or modify the values in the required fields.
3. Click the View Inward Message icon to view the messages.
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon to submit the record.

This tab displays the list of inward messages with the Record not created status. These messages are not mapped with the respective applications due to the error messages.

To send and view the inward messages, follow the below steps:

1. Processing of Repaired Messages .
2. Click the View SWIFT Message icon to view the inward messages.
3. Click the Send MT799/MT499 icon to send the SWIFT messages for clarification.
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon.


#### 📊 Outputs

There are no Outputs available for Reimbursement Processing under Standby Letter of Credit feature.

---


### 3.16  RMA Verification


> **📇 Quick Reference Card**
> 
> **Purpose:** *This section explains about Relationship Management Application (RMA) verification in Transact.*
> 
> **Applications:** `PP.RMA`
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

This section explains about Relationship Management Application (RMA) verification in Transact.

When a user initiates any MT7XX SWIFT Message for Guarantees/SBLC, the Temenos system conducts an RMA check. This check allows the user to determine if the Temenos model bank has an RMA with the receiver of the SWIFT message for any Guarantees/SBLC and if the message is delivered.

The system performs this check at field-level in any deal, that is, if multiple MT7XX SWIFT messages are generated, the system checks for each recipient individually and post an override message for each check if RMA is not available. This check is conducted based on both Customer ID and SW-‘BIC’ entered by the user.

Once the MD is committed and has any MT7XX or MT4XX SWIFT messages to be sent, the system consults PP.RMA using the existing DE.CHECK.RMA API (either from the entered customer ID or SW-‘BIC’). If RMA is available, the system proceeds without any override; otherwise, it raises a specific override on the mentioned fields.


#### ⚙️ Configuration

RMA Verification has no specific configuration to be setup. The parameter tables are setup at the implementation stage.


#### 📋 Tasks

There are no Tasks available for RMA Verification feature.


#### 📊 Outputs

There are no Outputs available for RMA Verification feature.


> **Related Applications:** `PP.RMA`

---


### 3.17  Standby Letterr of Credit


> **📇 Quick Reference Card**
> 
> **Purpose:** *A Standby Letter of Credit (SBLC) is a form of undertaking where a bank, on behalf of the buyer, guarantees that the seller (beneficiary) receives the payment upon presentation of specified documents and in the event the buyer fails to pay the beneficiary according to the terms of the contract. Unli...*
> 
> **Key Fields:** *22D*, *48D*, *Alternate ID (Guarantee Ref)*, *Available With (and C Available With)*, *C Docs Present Instr*, *C Transfer Indicator*, *Confirm Instr (Confirmation Instructions)*, *Confirmation Amount* ... +21 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

A Standby Letter of Credit (SBLC) is a form of undertaking where a bank, on behalf of the buyer, guarantees that the seller (beneficiary) receives the payment upon presentation of specified documents and in the event the buyer fails to pay the beneficiary according to the terms of the contract. Unlike a guarantee undertaking, wherein the bank is liable to pay upon demand, a SBLC is a secondary payment method where the bank promises payment if the seller fulfills the terms of the undertaking. These terms and conditions are provided as part of Presentation under Standby Undertaking .

The SBLC is subject to the version 98 of the ICC International Standby Practices (ISP 98), International Chamber of Commerce, Paris, France, which comes in effect from the date of issue of SBLC Undertaking.

As part of the updated SWIFT MT Standards, SBLC is now issued as part of MT760/MT761 instead of the existing MT700/701 from November 2021.

The following diagram illustrates the process flow for SBLC:

The parties of a guarantee contract are also applicable for an SBLC undertaking. In the above diagram, the seller is the beneficiary of the SBLC undertaking and the buyer is the applicant/instructing party. Other than these, there can be other parties involved in an SBLC contract as given below.

Advising Bank - This represents the beneficiary and it may accept the undertaking and collect it on behalf of the beneficiary. Advising Bank can either add confirmation on the undertaking and route it or advise the same either directly or through another advising bank.

Confirming Bank - This is a bank (usually located near the beneficiary) that agrees (confirms) to pay the beneficiary rather than have the issuing bank pay the beneficiary. This party can be the advising bank itself or another bank. The confirming bank after making payment to the beneficiary then collects the amount paid from the issuing bank.

Second Advising Bank - An advising bank can utilise the services of another bank (second advising bank) to advise the Undertaking and any subsequent amendments on the same to the beneficiary. A bank utilising the services of an advising bank or second advising bank to advise a credit, must use the same bank to advise any amendment thereto.

Nominated Bank/Available With - The issuing bank makes the SBLC undertaking available with this bank and nominates this bank to pay or negotiate with the beneficiary. The beneficiary can present the documents and route the claim through this party. This is a mandatory input when a reimbursement is involved in a Standby Letter of Credit.

Presentor - The beneficiary can route the presentation claim either through the nominated bank or through another negotiating bank, in which case, this bank sends an MT750 message requesting nominated or negotiating bank to pay/negotiate.


#### ⚙️ Configuration

Issue or Register SBLC has no specific configuration to be set up at the feature level. The bank must configure the parameter tables at the implementation stage along with the following settings:

To issue an undertaking as Direct Guarantee (DGAR) or Standby (STBY), the user must configure a form of undertaking for each product type (created in the Deal Sub Type field in MD.PARAMETER for each contract type allowed in MD Module) under MD.DEAL.TYPE.PARAMETER.


#### 🔧 Working With

Temenos Transact uses the Miscellaneous Deals (MD) module to record different Standby Letter of Credit (SBLC) undertaking transactions on the banks’ books. These range from straightforward guarantees (issued and received) to more specific trade finance-related deals (bid and performance bonds).

Banks issue the following common types of SBLC Undertakings:

- Registration guarantee/Bid bond/Tender bond
- Performance bond or guarantee
- Advance payment
- Maintenance (or warranty) guarantees
- Repayment guarantee
- Shipping guarantees


##### Issuance of SBLC

As per revised SWIFT MT Standards, the MT760 message type is also applicable for issuance of SBLC undertaking . Based on the product configuration in MD.DEAL.TYPE.PARAMETER and MD.PARAMETER , the system updates the Form of Undertaking as STBY. The system populates the value in the a 22D field of Sequence A of an outward MT760 message.

Temenos Transact allows the user to provide input for the below functionalities related to SBLC:

- Confirm Instr (Confirmation Instructions) – The user can specify whether the advising bank can add their confirmation or not. The allowed values are: Confirm May Add Without Note - When chosen, the user must specify the confirming bank in the Req Conf Party field ( Requested Confirm Bank ).
- Req Conf Party (Requested Confirm Bank) – The issuing bank requests this party to add its confirmation to the undertaking. When the advising bank receives an inward MT760 message of a SBLC then this field is captured with own bank details to add confirmation.
- Available With (and C Available With) – These fields capture the party with whom the undertaking is available. It indicates the party whom the issuing bank has authorised to pay/negotiate on their behalf, which is usually an Advising bank, the Confirming bank itself or any other bank. The issuing bank makes the undertaking available with this bank and nominates this bank to pay or negotiate with the beneficiary. The beneficiary can present the documents and route the claim through this party. This is a mandatory input when a reimbursement is involved in a Letter of Credit.
- Third Party Custno (Reimbursing Bank): This field captures the details of the reimbursing bank for an SBLC undertaking. A reimbursing bank is usually the Nostro bank of the issuing bank. When an SBLC undertaking is issued, the issuing bank can authorie a reimbursing bank to make payment on behalf of issuing bank to pay/negotiating bank after the claim is received. In such case, based on input in this field, the system triggers an outward MT740 towards the reimbursing bank, during an issuance of contract and subsequent amendments. When an advising bank receives an SBLC undertaking, based on the input in this field, the system triggers an outward MT742 reimbursement claim, after the issuing bank accepts the documents and requests for the settlement of the payment/negotiation or pre-debit notification.

Other key SBLC fields (also applicable for non-SBLC undertaking) are as follows:

Transfer Undk (Transferable Undertaking) and CTransfer Undk (Transfer Indicator): This field indicates, if the undertaking can be transferred. The beneficiary (first beneficiary) can request the bank specifically authorised in the undertaking to transfer the same ( available fully or partially) to a secondary beneficiary. The details are specified in the Transfer Cond field for either a Direct Undertaking or C Transfer Cond in case of counter undertaking or counter-counter undertaking (Transfer Conditions )

Apart from the above, the user captures documents and conditions applicable for presentation in the SBLC undertaking in the Docs Present Instr and C Docs Present Instr fields (Presentation Instruction), which are subsequently mapped to Tag 45C under an outward MT760.

The operations applicable for SBLC such as issuance, amendment, cancellation and reinstatement are the same as that of direct guarantees. In case of invocation, presentation of documents is mandatory and each invocation is linked with a presentation. (Read Presentation under SBLC for more information).


##### Confirmation of SBLC

An advising bank receives an inward MT760 from an issuing bank. The following options are available for the advising bank:

1. Advise the undertaking without any risk and responsibility on their part
2. Advise an SBLC undertaking by adding their confirmation and transmitting the same to the beneficiary / second advising bank. In this case, the user sets the Out Purp of Msg field as ACNF, with instruction to Confirm or May Add in the Confirm Instr ( Confirmation Instructions ) field. Also, the bank enters the own bank details in Req Conf Party ( Requested Confirm Bank ) indicating that the undertaking is confirmed by the present bank.

After capturing the above details, the system populates the Confirmation Amount (with the total amount of undertaking) and Confirmation Date fields as Today .

> **⚠️ Note:** Partial Confirmation is not supported under MD.DEAL

Based on the Confirmation Date and Confirmation Amount fields, the user books the liability entry on the Customer/Risk Party input, along with the details of the issuing bank. . The system raises the accounting and contingent entries as CONFIRM as shown in the following screenshot.

The accounting before Authorisation is shown below.

The accounting after Authorisation is shoen below.

If there are subsequent amendments and invocation, the system updates the liability amount confirmed accordingly.


##### Transfer of Local Undertaking

The different types of transfer of local undertaking are described in this section.

> **⚠️ Note:** This functionality is also applicable for Guarantees. However, in any case only the local undertaking can be transferred)

When an issuing bank issues an undertaking toward a beneficiary, the beneficiary can request in prior to transfer the undertaking to another party in full or partial. Hence, the bank issues the undertaking with the condition that it can be transferable, that is, Tag 48D of Sequence B of an outward MT760 is indicated as TRAN if it is direct/local undertaking and Tag 48D of Sequence C of outward MT760 is indicated as TRAN, if it is a counter undertaking. In such case, when the advising bank receives the undertaking, there are two scenarios possible:

The receiving bank registers the received undertaking (transferable) as a CL type contract. When the receiving bank decides to play the role of a transferring bank, the user must issue the transfer undertaking as a separate CA contract other than the local undertaking contract. Under this CA contract, the user must capture the @ID record of the CL contract in the Master Gtee Ref field that is to be transferred. Also, the user must flag the Issue Transfer Undk field (defaulted in Model Bank versions), to differentiate the issuance of local undertaking and transfer the undertaking.

> **⚠️ Note:** The Master Gtee Ref field can be marked only when the master reference number is input in the CA contract and the master reference (CL contract) holds the value as TRAN in the Transfer Indicator field populated from Tag 48 D under Sequence B of inward MT760.

When relaying the transfer undertaking to the second beneficiary, the bank user should not use the Tag 48D Transfer Undk field.

The user can issue both, the local and the transfer undertaking, under the same master guarantee undertaking, that is, two CA contracts under a CL counter undertaking, whenever C Transfer Indicator field is set as TRAN under the CL contract.

The following screenshots show Inward MT760 local undertaking received by the beneficiary's receiving bank.

The following screenshots show Cl Contract for Local Undertaking Received as MT760, with 48D set as TRAN

The following screenshot shows Transfer Undertaking Issued and Issue Transfer Undertaking as Yes to indicate Undertaking is a Transfer.

In a counter undertaking SBLC cycle, only the local bank can be the transferring bank. Hence, a transfer is not applicable under a counter-counter undertaking received nor should the user issue the same. Whenever a bank issues a local undertaking first under a counter undertaking, the value of undertaking can be less than the original counter undertaking. The user has to ensure manually that the transfer undertaking that is subsequently issued under this CA contract is of a value such that the total of local and transfer undertaking does not exceed the liability under the original CL contract. Similarly, when Transfer Undk is set as TRAN and mapped to an outward MT760 for the CA contract with advising bank specified, the user must ensure not to issue transfer undertaking under this CL contract to avoid multi issuance.

The advising bank that advises credit to the second beneficiary relays the transfer undertaking using the MT760 message. . The bank issues a CA contract in favour of the second beneficiary where the user must specify the CL contract’s @ID in the Alternate ID (Guarantee Ref) field and Master Gtee Ref , with issuing bank’s reference from Tag 20 of inward MT760 received under Reference 1 . The system books the liability on the first beneficiary of the transferring undertaking in the CA contract, thus sharing the full liability in the undertaking.

The user can route any subsequent request for extension, claims, presentations or cancellations only through CL contract towards the issuing bank, while transactions based on response from the issuing bank can be processed through the CA contract.

The system flags the Issue Transfer Undk field (defaulted in Model Bank versions), only when the Master Gtee Ref field is input in the CA contract and the master reference (CL contract) must hold the value TRAN in the Transfer Indicator field.

> **⚠️ Note:** When advising the transferring undertaking to the second beneficiary, the system books a CL contract

The following screenshots show Inward Standby Undertaking MT760 that was Advised by another bank.

The following screenshots show Register Inward MT760 as CL Contract for Transferable Standby undertaking received.

The following screenshot shows Issue Transfer Undertaking as CA Contract to second beneficiary linking CL Contract Received with In Purp of Msg as ADVI.

The user can also issue the transferring undertaking through an MT759 message, as allowed by SWIFT. In such a case, the user first issues the contract for the first beneficiary, for the full value. Then the user can generate a separate MT759 under the same contract, by choosing the MT759 Function field as Transfer with details of the transaction in MT759 Narrative and relevant undertaking type in MT759 Form of Undk field.

However, for issuance of transferring undertaking through MT759, the system does not block the liability entries . Hence, to issue separate contingent entries for undertaking in favour of the second beneficiary, the user can use the CA contract.


#### 📋 Tasks

Related topics:

- Issue Guarantee
- Trade Finance and Guarantees Processes
- Accept or Reject Amendment Request of Guarantee or Standby LC (Received)
- Transfer Undertaking of Guarantee or Standby LC (Received)

A transferrable letter of credit is a type of financial guarantee that additionally allows the first beneficiary to transfer some or all of the credit to another party, which creates a secondary beneficiary. The party that initially accepts the transferrable letter of credit from the bank is referred to as the first or primary beneficiary.


##### Workflow

The Trade Finance Officer can perform transfer undertaking using the below workflow.

This menu allows the user to issue transfer undertaking.

To issue a transfer undertaking, follow the below steps:

1. Issue of Transfer Undertaking .
2. In the Issue of Transfer Undertaking screen, enter values in the mandatory and other required fields.
3. Click the Validate icon to check for the errors and overrides.
4. Click the Delivery Preview icon to view the delivery messages.
5. Click the Commit icon to submit the record.


#### 📊 Outputs

There are no Outputs available for Standby Letter of Credit feature.

---


### 3.18  Syndicate Guarantee


> **📇 Quick Reference Card**
> 
> **Purpose:** *Guarantees can be issued as part of the syndicated lending operation.*
> 
> **Sections:** 📖 Introduction | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Guarantees can be issued as part of the syndicated lending operation.


#### 📋 Tasks

There are no Tasks available for Syndicate Guarantee feature.


#### 📊 Outputs

There are no Outputs available for Syndicate Guarantee feature.

---


### 3.19  TBML Check for Guarantee and SBLC


> **📇 Quick Reference Card**
> 
> **Purpose:** *Trade-Based Money Laundering (TBML) in trade finance guarantees or standby letters of credit (sblc) involves the exploitation of trade finance instruments, such as bank guarantees or standby letters of credit, to launder illicit funds. This illicit activity often occurs through the manipulation of t...*
> 
> **Applications:** `DIPO.ITEMS`, `DISPO.ITEMS`
> 
> **Key Fields:** *Status*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Trade-Based Money Laundering (TBML) in trade finance guarantees or standby letters of credit (sblc) involves the exploitation of trade finance instruments, such as bank guarantees or standby letters of credit, to launder illicit funds. This illicit activity often occurs through the manipulation of trade transactions and associated documentation to conceal the origin of criminal proceeds. Following are the ways in which TBML is manifested in trade finance guarantees:

| Method | Description |
|---|---|
| Overvaluation of Goods | Those involved in criminal activities may inflate the value of goods or services involved in trade transactions supported by guarantees. By overpricing the goods, they can create a discrepancy between the actual value of the goods and the reported transaction value, enabling them to launder illicit funds through legitimate trade channels. |
| Fictitious Transactions | TBML perpetrators may engage in creating fictitious trade transactions backed by guarantees. These transactions involve the issuance of guarantees for non-existent or misrepresented goods or services. The guarantee serves as a mechanism to legitimise the movement of illicit funds across borders, making it appear as if they originated from legitimate trade activities. |
| Phantom Shipments | Criminal organisations may exploit trade finance guarantees to facilitate phantom shipments, where goods are invoiced and guaranteed for shipment but are never actually delivered. This scheme allows criminals to create a paper trail of fictitious trade transactions, providing a facade of legitimacy for laundering illicit funds. |
| Round-Tripping | In certain cases, TBML involves round-tripping, where funds are moved through a series of transactions involving multiple jurisdictions and intermediaries to obscure their origin. Trade finance guarantees can be misused in round-tripping schemes to create the appearance of legitimate trade activities while effectively laundering illicit funds. |
| Misrepresentation of Goods | TBML perpetrators may misrepresent the nature or quality of goods involved in trade transactions supported by guarantees. By providing false or misleading information about the goods, they can manipulate the trade finance process to launder illicit funds without attracting suspicion. |
| Layering | TBML often involves layering, where funds are moved through multiple accounts or financial instruments to further obscure their origin. Trade finance guarantees can be used as part of the layering process to facilitate the movement of illicit funds through the international banking system. |

To combat TBML in trade finance guarantees, financial institutions must implement robust anti-money laundering (AML) controls and due diligence measures. This includes conducting thorough customer due diligence, verifying the authenticity of trade transactions and documentation, and implementing transaction monitoring systems to detect suspicious activities. Collaboration between financial institutions, regulators, and law enforcement agencies is also essential to effectively combat TBML in trade finance guarantees and protect the integrity of the global financial system.


#### ⚙️ Configuration

The TRANSACT trade finance application communicates with the TRANSACT FCM through the utilisation of DISPO.ITEMS . Read FCM Architecture and Design for more information on the FCM architecture and design.

The fields and inquiries can be employed to configure and engage with any external TBML engines.


#### 🔧 Working With

This functionality allows the transmission of a trade finance transaction to TBML to be carried out by the bank user across various workflows associated with trade finance products.

The workflow enabled for TBML check involves conducting checks at various stages of trade finance transactions to mitigate risks associated with Trade-Based Money Laundering (TBML). The following workflows are specifically enabled for TBML checks:


##### Issuance of Guarantee/SBLC

During the issuance of Guarantee/SBLC, banks perform TBML checks to ensure compliance with anti-money laundering regulations and to prevent fraudulent activities. This includes verifying the identities of the parties involved, assessing the legitimacy of the underlying trade transactions, and scrutinising the documentation provided to support the guarantee request.


##### Amending of Guarantee/SBLC

During the amendment process of existing guarantees or SBLCs, TBML checks are performed to assess the necessity and validity of the proposed amendments. This involves reviewing the changes made to the guarantee terms, assessing their impact on the transaction, and ensuring compliance with regulatory requirements to mitigate potential TBML risks.


##### Claims or Presentation under Guarantee/SBLC

TBML checks are conducted when the beneficiary presents documentation to claim payment under the guarantee or SBLC. This includes verifying the authenticity of the presented documents, confirming adherence to the terms and conditions of the guarantee, and assessing the legitimacy of the underlying trade transactions. Scrutiny is applied to invoices, bills of lading, certificates of origin, and other relevant documents to detect any anomalies or discrepancies that may indicate potential TBML activities.

In each of these workflows, financial institutions employ various risk-based approaches and due diligence measures to detect and prevent TBML. This includes utilising advanced technology for transaction monitoring, conducting thorough customer due diligence, implementing enhanced controls for high-risk transactions or counterparties, and fostering collaboration with regulatory authorities and law enforcement agencies. By integrating TBML checks into trade finance guarantee workflows, financial institutions aim to safeguard the integrity of the financial system and mitigate the risks associated with money laundering in trade finance transactions.


##### Payload Sent to FCM During Different Events of FCM Contact Points

Payloads transmitted to FCM vary depending on the different events occurring at FCM contact points. These events, along with their corresponding payload and date type, are as follows:

| Events | Payload | Data Type |
|---|---|---|
| Issuance | CUSTOMER | Customer ID/Text |
| APPLICANT.ID | Customer ID/Text |  |
| INSTRUCTING.PARTY | Customer ID/Text |  |
| APPLICANT.ADDRESS | Text |  |
| BEN.ADDRESS | Text |  |
| BENEFICIARY | Customer ID/Text |  |
| RECEIVING BANK | Customer ID/Text |  |
| ADV.RECEIVING.BK | Customer ID/Text |  |
| ADVICE.THRU.BK | Customer ID/Text |  |
| ADVISING.BK.NAME | Customer ID/Text |  |
| AVAILABLE.WITH | Customer ID/Text |  |
| Reimbursement | THIRD.PARTY.CUSTNO | Customer ID/Text |
| THIRD.PARTY | Customer ID/Text |  |
| Amendment | MT767.BENEF.CUST.1 | - |
| MT767.C.BEN.ADDRESS | - |  |
| Payment | ACCT.WITH.BANK | Customer ID/Text |
| SETTLE.ACCOUNT | Customer ID/Text |  |
| INV.BENEFICIARY | Customer ID/Text |  |
| OUR.CORRES.BNK | Customer ID/Text |  |
| INV.REC.BANK | Customer ID/Text |  |
| RE.AC.WITH.BNK | Customer ID/Text |  |
| RECV.CORRES.BANK | Customer ID/Text |  |
| Reimbursement Amendment | THIRD.PARTY.CUSTNO | Customer ID/Text |
| THIRD.PARTY | Customer ID/Text |  |
| THIRD.PARTY | RECEIVING.BANK | Customer ID/Text |
| Other Flows | MT765.RECV.BANK | Customer ID/Text |
| MT786.RECV.BANK | Customer ID/Text |  |
| PRESNT.RECV.BANK | Customer ID/Text |  |
| FCM | MT759.RECV.BANK | Customer ID/Text |
| FCM.FIELD | Text field |  |

The payloads contain various information such as customer IDs, text data, and other relevant details, aiding in the communication and processing of trade finance transactions within the FCM system.

The following are examples of triggering a TBML for Issuance of Guarantee or SBLC.

To trigger a TBML for Issuance of Guarantee or SBLC,

- Input the Contract details for the Issuance of Guarantee or SBLC.
- Check the FCM Enable checkbox to trigger the transaction for TBML check.
- Once the transaction is committed, an override is displayed to show the contract is sent for FCM check.
- The transactions transmitted through FCM are monitored using a specialised inquiry to display the trade transactions for FCM, which can be accessed for viewing.
- Transactions are segregated based in the Status field in the DIPO.ITEMS application.

- Once a transaction undergoes an FCM check, the FCM engine typically responds with one of three outcomes: Approved Rejected Possible


#### 📋 Tasks

There are no Tasks available for the TBML Check for Guarantee and SBLC feature.


#### 📊 Outputs

There are no Outputs available for the TBML Check for Guarantee and SBLC feature.


> **Related Applications:** `DIPO.ITEMS`, `DISPO.ITEMS`

---


---


## Chapter 4: Trade_Banking - SU


Trade_Banking - SU module of Temenos Transact


### Features in Trade_Banking - SU


| # | Feature | Sections |
|---|---------|----------|
| 4.1 | Facility Agreement | Intro, Confi, Worki, Tasks, Outpu |
| 4.2 | Finance Request | Intro, Confi, Worki, Tasks, Outpu |
| 4.3 | Invoice Batching | Intro, Confi, Worki, Tasks, Outpu |
| 4.4 | Invoice Capture | Intro, Confi, Worki, Tasks, Outpu |
| 4.5 | Misc | Intro |


### 4.1  Facility Agreement


> **📇 Quick Reference Card**
> 
> **Purpose:** *A facility is a line of credit or financial arrangement granted to a borrower. Its administration is based on product type, credit nature (revolving or non-revolving), tenor, and currency. The method for calculating the commitment fees and their collection frequency is defined at the facility stage....*
> 
> **Applications:** `AA.ACCOUNT.DETAILS`, `SU.INVOICE.CAPTURE`
> 
> **Key Fields:** *Counterparty*, *Currency*, *Default Grace*, *Default Retention*, *Grace Calc Basis*, *Grace Days*, *Recourse Party*, *Recourse Type* ... +1 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

A facility is a line of credit or financial arrangement granted to a borrower. Its administration is based on product type, credit nature (revolving or non-revolving), tenor, and currency. The method for calculating the commitment fees and their collection frequency is defined at the facility stage. The facility agreement defined under the programme, phases out the disbursements so that each drawing has its own terms and conditions for drawdown management.

When a bank enters into a Supply Chain Finance agreement with a corporate customer the agreement details such as the list of parties involved, retention margin, and grace period are stored within the facility. This ensures that the agreement terms are applied to any drawdown created under the facility.

Borrower limits are configured for the facility, and sub-limits for the facility's counterparties are set up to ensure that the total counterparty usage does not exceed the facility commitment.

Facility Agreement also includes the functionality to capture recourse details. When a bank or financial institution decides to finance invoices, it first establishes an agreement with the borrower that outlines the terms and conditions, which are then applied to the drawings created under the facility. The recourse terms defined in the facility agreement is fixed for the entire tenure of the facility and cannot be amended.

Facility agreements are classified based on the borrower’s liability in the underlying drawings:

- Recourse: Financing is provided with recourse when the risk is owned by the supplier. In this case, the bank or financial institution can seek repayment from the supplier if the debtor defaults.
- Non-Recourse: Financing is provided without recourse when the risk is owned by the ultimate debtor (buyer). In this case, the bank or financial institution cannot seek repayment from the supplier if the debtor defaults.
- Retention Margin: Refers to the percentage of the total invoice which is deducted from the invoice's face value when it is being financed.
- Grace Days: Refers to the additional time frame provided by the bank that allows the buyer to settle the invoice beyond its original due date, extending the buyer's payment deadline.

This distinction is crucial for understanding the risk and liability associated with each type of facility agreement.


#### ⚙️ Configuration

This section explains how to configure a facility agreement.

The recourse type can be selected at the facility level and the recourse and non recourse options can be configured in the Account Product Condition.

When the bank signs an SCF agreement with a corporate customer the agreement details such as the list of parties involved in the facility agreement, retention margin, and grace period must be stored within the facility. This ensures that the terms of the agreement are applied to any drawdown created under the facility.

The sub-arrangement rules property class accommodates the retention margin and grace period, which can be defined for the supplier under the facility arrangement. Additionally, the retention margins and grace days can be defined for a specific counterparty by currency. If the retention margins and grace days are not defined at the counterparty level, the default definitions are applied. The following fields are available in the Sub Arrangement Rules property class:

| Field | Description |
|---|---|
| Default Retention | Specifies the default retention margin for the facility agreement. |
| Default Grace | Specifies the default grace days for the facility agreement. Grace days are set to calendar days by default. If no Grace days are defined for a counterparty then default grace is considered. However, banks can change them to working days by appending ‘W’ to the number of days. Grace days can be defined as: 8W: 8 working days 8C: 8 calendar days 8: 8 calendar days This field is optional. |
| Grace Calc Basis | Allows the bank to determine how the maturity date is extended and charges are calculated for the grace days. The available options are: Maturity Date: Extends the maturity date of the loan. Charge: Calculates the charge for the grace days. This field becomes mandatory, when grace days are defined in arrangement rules. |
| Counterparty | Specifies the counterparty details in a facility agreement. It refers to customer table. This field is optional and becomes mandatory when currency, retention margin, or grace days are defined. |
| Currency | Specifies the currency details for retention and grace in a facility agreement. This field is optional and becomes mandatory when currency, retention margin, or grace days are defined. |
| Retention Margin | Specifies the retention details for the counterparty in a facility agreement. |
| Grace Days | Specifies the grace days details for the counterparty in a facility agreement. Grace days are set to calendar days by default. However, banks can change them to working days by appending ‘W’ to the number of days. Grace days can be defined as: 8W: 8 working days 8C: 8 calendar days 8: 8 calendar days This field is optional. |

The below screenshot displays the Default Retention and Default Grace details in the agreement tab of sub arrangement rules.

The below screenshot shows the types of Grace Calc Basis available.


#### 🔧 Working With

This section details the calculation of retention margin and grace days for a facility agreement.


##### Calculating Retention Margin

Retention is a percentage of the total invoice which is deducted from the invoice's face value when it is being financed. In SCF, when a corporate customer makes an agreement with the bank, retention margin is one of the agreement details that can be established either at the supplier level or at the counterparty level. Once the agreement is confirmed, the retention margin details are stored in the sub-arrangement rules by currency.

When an SCF drawing is created (loan creation), the system determines the amount to be withheld (retention amount). The system:

- Examines the sub-arrangement rules associated with the drawing, which define how payments are handled for specific agreements.
- Verifies if a retention definition exists within the sub-arrangement rules. This definition specifies the retention margin (percentage of the invoice amount to be withheld). If a retention definition is identified, the system retrieves the retention margin value.
- Calculates the finance amount after deducting the retention amount from the total invoice value.

When creating SCF drawings, the system uses the following approaches to identify if a retention margin is applicable.

- Counterparty-Specific Retention: The system prioritizes checking if a retention margin is defined for the specific counterparty involved in the drawing, which is likely recorded in the sub-arrangement rules. If a counterparty-specific retention margin is identified, the system retrieves and applies that percentage to calculate the finance amount (loan amount) for the drawing. This represents the amount to be financed after withholding the retention amount. The drawing only stores the finance amount in the designated field and not the retention margin.
- Supplier-Level Retention: If counterparty-specific retention is not defined for the currency, the system checks if a default retention margin is set at the supplier level. If yes, the system retrieves and applies that percentage to calculate the finance amount for the drawing.
- No Retention Margin: If the retention margin is not defined at either the counterparty or supplier level, the system disburses the full invoice amount as the finance amount.


##### Calculating Grace Days

Grace days refer to an additional time frame provided by the bank that allows the buyer to settle the invoice beyond its original due date, extending the buyer's payment deadline.

Similar to retention margins, grace days can be defined at two levels:

- Counterparty Level: A specific grace period can be set for a particular counterparty involved in the drawing, which is likely recorded in the sub-arrangement rules and applies to invoices in a specific currency.
- Supplier Level: If a counterparty-specific grace period is not defined, a default grace period defined at the supplier level is applied.
- No Grace Days: If no grace days are configured for both the counterparty or supplier level, the system considers the tenure as it is in the invoice for the drawing.

The grace period can be calculated using the following options:

The grace period can be used to extend the invoice's maturity date. In this scenario, interest is calculated for the additional period granted by the grace period, which essentially extends the final due date for the buyer adding financing costs.

When creating SCF drawings, the system uses the following approaches to identify if grace days are applicable.

- Counterparty-Specific Grace Days: The system prioritizes checking if grace days are defined for the specific counterparty involved in the drawing, which is likely recorded in the sub-arrangement rules. If counterparty-specific grace days are identified, the system applies the number of days to extend the invoice’s due date.
- Supplier-Level Grace Days: If counterparty-specific grace days are not defined for the currency, but are available at the supplier level, the system applies the Grace Days defined for the supplier to the SCF drawings.
- Grace Days Not Applicable: If grace days are not defined at either the counterparty or supplier level, the SCF drawings have no grace period. The due date remains the original maturity date of the invoice.

The grace period can be used to calculate an additional charge on the invoice’s advance payment for the grace days. However, the maturity date of the drawing remains the same as the original invoice maturity date.

When SCF drawings use ‘Charge’ as the basis for calculating the grace period, the borrower incurs an additional fee for the extended payment period.

- Charge Collection: The system calculates a charge for the grace period days, which is collected as an Activity Charge associated with the New Arrangement Activity. This activity charge is deducted from the disbursement amount and the remaining amount is then financed for the customer.
- Charge Calculation: A separate charge routine handles the calculation of this additional fee. The charge is based on the finance amount and the prevailing interest rate applied to the SCF drawings.
- Charge Accrual/Amortization: The borrower is responsible for the charge over the life of the loan (loan maturity), which can be Amortized, Accrued, or Itemized.

The grace period can be defined in the following ways:

- Calendar Days: The charge is calculated based on the exact number of calendar days configured in the grace period.
- Working Days: The charge is calculated based on the number of business days that fall within the grace period, starting from the invoice maturity date.


##### Use Cases

The following examples show the scenarios where the default and counterparty-specific retention margin and default grace days are defined at the Facility level.

| Supplier | Counterparty | Invoice Face Value | Ccy | Invoice Mat Date | Retention | Finance Amt | Grace | Grace Calc Basis | Maturity Date |
|---|---|---|---|---|---|---|---|---|---|
| 100363 | Dell Computer | 15000 | USD | 31/05/2024 | 10% | 13500 | 5D | Maturity Date | 05/06/2024 |

| Supplier | Counterparty | Invoice Face Value | Ccy | Invoice Mat Date | Retention | Finance Amt | Grace | Grace Calc Basis |
|---|---|---|---|---|---|---|---|---|
| 100363 | Dell Computer | 20000 | USD | 12/06/2024 | 5% | 19000 | 10W | Charge |


##### Recourse

The Recourse Type field in Account product conditions stores the recourse information of the agreement. Allowed values are ‘Recourse’ and ‘Non Recourse’. This field is configured during facility creation and cannot be amended once the facility agreement is established. Upon disbursement through a finance request, the system updates the Recourse Type field in the underlying drawings with the recourse information from the facility agreement. Manual configuration of the Recourse Type field at the drawing level is not possible. Based on the Recourse Type field, the system updates the Recourse Party field in the drawing agreement.

- Recourse: The system updates the borrower reference in the Recourse Party field at the customer product condition, making this borrower the beneficial owner or liable party for the drawing agreement.
- Non-Recourse: The system updates the counterparty reference in the Recourse Party field at the customer product condition, making this counterparty the liable party for the drawing agreement.

Additionally, the recourse type is updated in the AA.ACCOUNT.DETAILS application for SCF arrangements (facility or drawing) for reporting purposes. During facility agreement creation, the Recourse Type field in the Account Product Condition must be selected as either ‘Recourse’ or ‘Non Recourse’.

The below screenshot shows the Account PC during facility creation.

Finance Liability Details.

Once the recourse party is defined in the criteria, the below screen is displayed.


##### Limits for SCF

The limit structure is available for Supply Chain Finance with both the Limit and sub-limits . In Transact, the limit and sub limits are set for the buyer, but in case of SCF it differs.

In SCF, sub-limits are enhanced for the counterparty as part of the supplier-led financing. These sub-limits are defined at the facility level to limit or restrict a specified limit. This is used to reduce the chance of risk for the buyer entering the agreement. The limit is decided by the bank at the origination stage (facility creation) and not by the supplier or buyer. Read Introduction to Limits for more information on sub-limit processing.


#### 📋 Tasks

There are no Tasks available for Facility Agreement.


#### 📊 Outputs

There are no Outputs available for Facility Agreement.


> **Related Applications:** `AA.ACCOUNT.DETAILS`, `SU.INVOICE.CAPTURE`

---


### 4.2  Finance Request


> **📇 Quick Reference Card**
> 
> **Purpose:** *When a borrower approaches the bank for funding based on submitted invoices, the bank provides the funds through the SU.FINANCE.REQUEST application. This process involves the following key steps based on the action performed:*
> 
> **Applications:** `CURRENCY`, `SU.FINANCE.REQUEST`, `SU.INVOICE.BATCH`, `SU.INVOICE.CAPTURE`
> 
> **Key Fields:** *Action*, *Batch Reference*, *Borrower*, *Borrower Role*, *Counterparty*, *Counterparty Role*, *Currency*, *Currency Market* ... +21 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

When a borrower approaches the bank for funding based on submitted invoices, the bank provides the funds through the SU.FINANCE.REQUEST application. This process involves the following key steps based on the action performed:

1. Initiating the Finance Request: The actual funding process begins after ensuring that the borrower and counterparties are part of the attached facility. The facility tenure exceeds the tenure of the invoice or batches attached, and there is sufficient balance available at the facility to finance the Invoice or Batches.
2. Selection of Disbursement Method: When initiating a finance request, the user has an option to disburse the entire value of the request. However, if the facility balance is insufficient or the user wants a specific amount to be disbursed, the finance request can be disbursed partially by selecting the disbursement method as ‘Partial’ and proceeding with further processing.
3. Generating Finance Quotations: Quotations are generated to inform the borrower regarding the net disbursement amount, taxes, interest on the invoices, and other financial details related to the Financing Request.
4. Disbursement of Finance Request: The finance request is disbursed using the ‘Disburse’ action. An actual loan is then created under the facility based on the drawing product specified in the finance request and the net disbursement amount is credited to the borrower.
5. Settlement of Invoice: Invoice repayment details can be manually recorded, and the fully repaid invoices can be updated to the ‘Settled’ status. This process ensures that both the bank and the borrower have clear visibility of invoices that are completely settled.

This process ensures efficient and accurate funding through the Finance Request application. Transact allows users to modify finance request details at any point before the disbursement action.If the facility has sufficient funds, the user can also fund partially disbursed finance requests. Additionally, it provides the option to unbatch the invoices from a batch if unexpected issues occur during the disbursement action. If the facility has insufficient funds, the user can also request for partial disbursement up to the available amount. Additionally, Transact provides an option to unbatch invoices from a batch if the status of the finance request is ‘Completed with Errors’ during the disbursement process. The invoices can be processed further once they are unbatched form the finance request.

SCF supports cross-currency financing (financing of invoices in a foreign currency). Procuring from multiple suppliers in different countries can reduce the reliability on a single currency, which helps to mitigate risks associated with currency fluctuations.

Lending Products in AA support multicurrency drawings under a facility. To facilitate drawings in currencies other than the Facility currency, the system should support multicurrency drawings for Supply Chain Finance.


#### ⚙️ Configuration

This section explains how to configure the Exchange Rate property class to support multi-currency financing.

To configure the Exchange Rate property class for multi-currency financing, enter the exchange rate to be applied in the Exchange Rate field. This enables the system to convert the facility or drawing balances to its parent currency.

If the Exchange Rate field is not configured, the system considers the mid reval rate from the CURRENCY application as the exchange rate.

By default, the Currency Market is set as 1, the system takes the mid rate for this currency market to enable multicurrency financing.

The other option is to negotiate the Exchange Rate in the Exchange Rate property class.


#### 🔧 Working With

When the borrower approaches the bank for funding an invoice or batch, the first step is to initiate a finance request. This involves configuring the mandatory fields such as the borrower, borrower role, currency of the requested finance, reference to the facility under which the finance is requested, drawing product, financing date, and reference of the invoice or batch that is requested for financing.

The following fields are available in the SU.FINANCE.REQUEST application:

| Field | Description |
|---|---|
| Action | This field contains the following predefined set of actions which can be executed on the funding request: BLANK - Allows the template to be committed without any action by simply validating the template. DISBURSE - Triggers the disbursement for the funding request. Upon triggering, the SCF drawings are created under the selected facility, and funds are disbursed to the borrower. This action is executed through a service. GET.QUOTE– Runs simulation on the batched invoices and fetches the final disbursement amount. RESUBMIT – Triggers the disbursement for the finance request, which are in the error queue. |
| Borrower | Specifies the customer for whom the finance is to be disbursed. |
| Borrower Role | Holds the role of the customer. |
| Counterparty | Specifies the counterparty reference. This field is mandatory only when an invoice reference is added to a funding request for a single invoice disbursement. When a batch reference is added, the counterparty details for disbursement are taken from the batch reference. The counterparty field is not allowed when a batch reference is updated. |
| Counterparty Role | Holds the role of the counterparty. |
| Facility Reference | Holds the facility reference under which the invoices will be funded. |
| Product | Holds the AA.PRODUCT reference. When the funding request is approved, the amount disbursed to the borrower is processed through an AA loan, and the loan is created for the product specified in this field. |
| Currency | Holds the currency in which fund will be disbursed. This value should match the currency defined in SU.INVOICE.BATCH when a batch reference is provided, else, it should match the invoice currency when an invoice reference is given. |
| Financing Date | Indicates the date on which the funds are disbursed to the borrower. It can be backdated, current-dated, or future-dated. |
| Invoice Reference | Specifies the invoice reference which corresponds to the SU.INVOICE.CAPTURE table. The status of the invoice entered must be ‘NEW’. Either a batch reference or an invoice reference is required. |
| Batch Reference | Holds the SU.INVOICE.BATCH reference, allowing the bank user to attach the batch reference for initiating disbursement. It is mandatory when an invoice reference is not given. The system must validate that the borrower reference in the batch matches the one specified in the funding request. |
| Quotation Status | Holds the status of the quotation. |
| Status | Holds the status of the finance request. |
| Recourse Type | Holds the type of the recourse associated with the facility arrangement. |
| Delink Invoice | Delinks the failed invoices from the Finance Request. This is a User Input Field. This field can be set as ‘Yes’ only when the Finance Request is in the ‘Completed with Error’ status. If it is set as ‘Yes’, the system only allows the ‘Resubmit’ action to be performed, which delinks the failed invoice from the Finance Request. This field is optional. |
| Drawing Reference | Holds the Arrangement reference for the invoices that are successfully created under a batch. This field is updated by the system with the Drawing Arrangement ID. |
| Failed Invoices | Holds the reference for the invoices for which drawing creation has failed. The failed invoices under the finance request will be in the Invoices ID*AAA reference format. This field is updated by the system. |
| Inv Drawing Reference | Holds the Arrangement reference for the invoice that is successfully created. This field is updated by the system with the Drawing Arrangement ID. |
| Inv Failure Reference | Holds the AA.ARRANGEMENT.ACTIVITY reference when the drawings creation has failed for the given invoice reference. |
| Disbursement Method | Specifies the disbursement method. Allowed values are: Full : Enables the user to disburse the finance request to the full available amount for a newly initiated finance request and the existing partially financed finance requests. Partial : Allows the user to input a specific amount for a finance request. This field is optional. If no input is given, the system considers the value 'Full' by default. |
| Inv Available Amount | Specifies the fundable amount for an invoice attached to the finance request. This is calculated based on the face value of the invoice, deducting the retention margin configured at the facility attached in the finance request. |
| Inv Requested Amount | Specifies the amount requested by the user for an invoice. If no specific amount is requested, Inv Available Amount is considered as the Inv Requested Amount . |
| Total Available Amount | Specifies the total fundable amount for a finance request. For multiple batches, it is calculated based on the batch amount, deducting the retention margin configured at the facility. For multiple invoices, it is the sum of all the Inv Available Amount . |
| Requested Amount | Specifies the amount requested by the user for batches. If no specific amount is requested, the Total Available Amount is considered as the requested amount. This field becomes mandatory when Disbursement Method is set as ‘Partial’ for the finance requests with batches. |


##### Initiating Finance Request

Initiating the Finance Request is an important step in the financing process. The actual financing begins when a borrower requests financing for multiple sets of batched invoices. The necessary details for financing are validated and stored. Once validation is complete, the Finance Request can proceed to quotation generation or disbursement, based on the bank's convenience.

In the finance request validation process, several critical checks are performed to ensure accuracy and compliance. These include:

1. Verifying the borrower against the facility customer and checking the borrower and their role against the details in the Batch or Invoice.
2. Validating the counterparty defined at the facility with the counterparty in the attached batches, and the currency is checked against the Invoice or Batch currency.
3. Validating the tenure of the facility with the tenures of the attached Invoice or Batches.
4. Comparing the facility balance with the finance amount to prevent unforeseen errors during disbursement.
5. Validating the drawing product against the allowed product list in the facility.

These comprehensive checks are essential for maintaining the integrity and smooth processing of the finance requests.

To initiate a finance request,

1. Input Finance Request.
2. Configure the mandatory fields such as borrower, borrower role, facility reference, drawing product, currency, and invoice/batch reference as shown below.

The screenshot below illustrates how to finance a multiple invoice batch. The user can add multiple batch references in the batch details section.

The below screenshots illustrate how to finance invoices within a finance request. The user can add up to 25 invoices in a single finance request for further processing.

> **⚠️ Note:** Transact supports attaching and processing of up to 25 invoices manually in a single finance request which are not linked to any batch or finance request.

During the initiation of a finance request, once the user updates all the mandatory fields, the system validates the available balance at the facility. If the balance is insufficient but the borrower needs immediate funds, the finance request can be partially disbursed by setting the Disbursement Method field to ‘Partial’. The user can then fund the finance request up to the available facility balance by capturing the Requested Amount .

Disbursement Method can be set to ‘Partial’ for scenarios involving multiple invoices and multiple batches.

- For Invoices : If one or more invoices are attached to the finance request, upon validation with the Disbursement Method (set to ‘Partial’), the system updates the Inv Available Amount field. This updates the user with the maximum available amount for disbursement in each invoice, preventing the user from requesting an amount greater than the invoice value. This field is updated for all attached invoices, considering the retention amount configured at the facility level. The user can request funding for a single invoice or the entire set of attached invoices using the Inv Requested Amount field. If the invoice requested amount is not provided, the entire available amount is considered for financing.
- For Batches : If one or more batches are attached to the finance request, upon validation with the Disbursement Method (set to ‘Partial’), the system updates the Total Available Amount field with the total available amount for disbursement in the attached batches. This field is updated for batches, considering the retention margin configured at the facility level. The user can then input the requested amount for further processing of the finance request.

> **⚠️ Note:** If one or more invoices are attached, the Inv Requested Amount and Inv Available Amount fields are updated. If one or more batches are attached, the Requested Amount and Total Available Amount fields are updated.

The below screenshot illustrates the definition of Requested Amount in case of a finance request with single or multiple batches.

The below screenshot illustrates the definition of Inv Requested Amount in case of a finance request with single or multiple invoices.


##### Amending and Reversing Finance Request

Banks can modify the Finance request record at any time before the disbursement action is triggered. Additionally, it provides an option to reverse a finance request before Disbursement.

Manage Finance Request.

The below screenshot shows the navigation and options available in the finance request after initiation, such as View, Amend, Reverse, and Generate Quotation. The record can be amended or reversed at the bank's convenience, accommodating any changes in the financing request from the borrower.


##### Quotation Generation of Finance Request

Quotation can be generated when a borrower requests the Net Disbursement details for a set of invoices. This quotation provides detailed financing information, including updates to the facility's available balance and the Net Disbursement Amount to be credited to the borrower upon disbursement. This functionality enables both the bank and the borrower to adjust the batches linked to the finance request, ensuring that the net disbursement amount matches the requested finance amount before the disbursement action.

This feature is enabled by the ‘Get Quote’ action in the SU.FINANCE.REQUEST application. Quotation can be generated by the following ways:

- By defaulting the finance request with the ‘Get Quote’ action at the time of initiation
- By generating a quotation from an existing pending Finance Request.

> **⚠️ Note:** Multiple quotations can be generated for the same finance request before disbursement, with the ability to edit the finance request and change the attached batches.

To generate a quotation, ensure that the SU.FUNDING.SERVICE and AA.SIMULATION.SERVICE services are running.

To generate quotation through Manage Finance Request,

1. Manage Finance Request .
2. Select the Generate Quotation option as shown below.

> **⚠️ Note:** Transact allows the users to generate a quotation and initiate a finance request simultaneously by configuring the ‘Get Quote’ field and providing the required finance request details.

To generate quotation,

1. Input Finance Quotation .
2. Configure the mandatory fields such as borrower, borrower role, facility reference, drawing product, currency, and invoice/batch reference as shown below.

> **⚠️ Note:** If Disbursement Method is set as ‘Partial’, the quotation is generated solely based on the Request Amount for finance requests with multiple batches and the Inv Requested Amount for finance requests with multiple invoices.

View Quotation.

After processing the finance request in services, the financial details can be accessed through the above navigation. The generated quotation includes comprehensive details of the finance request, such as facility balances (sanctioned amount, available balance, and new outstanding balance if the finance request is disbursed). It also provides the details on interest, charges, taxes, and the net disbursement amount for each batch attached to the finance request.

The below screenshot shows an example of a generated finance quotation with multiple batches.

Finance requests that are in the error queue can also be displayed during quotation generation. These finance requests can be identified by a red flag, as shown in the below screenshot. Additionally, the reason for the failure is displayed in the error log when the bank reviews the finance request record.


##### Disbursement of Finance Request

The disbursement of funds for the invoice or batch of invoices attached to the finance request is triggered through the “Disburse” action in finance request. Once this action is triggered, the system creates a loan under the attached facility for each invoice, based on the product described in the finance request. The invoice amount is set as the loan amount, with any applicable retention detected. The tenure of the loan is determined from the financing date to the invoice maturity date, including any applicable grace days.

If Disbursement Method is set to ‘Partial’ and Action is set to ‘Disburse’, the requested amount is used to process the loan arrangement.

- For multiple invoices, the requested amount for each invoice is taken as the loan amount, accounting for any retention specified in the facility agreement.
- For batches, the requested amount is processed by the service, which selects a set of invoices such that their total sum equals the requested amount. The service prioritizes batches based on their payment due dates, starting with those closest to the finance date. If multiple batches share the same payment due date, the order in which they are attached to the finance request is considered. Only these selected invoices are financed, leaving the rest unfinanced or partially financed.

At the end of the service processing, the system updates the available amount fields in both the invoice and batch records. This update enables the user to know the amount available for future disbursements.

Transact supports multiple partial disbursements for the same finance request multiple times until the total available amount in the finance request is fully utilised. From the second partial disbursement, the LENDING-INCREASE-COMMITMENT activity class is triggered when the user specifies the requested amount and selects the ‘Disburse’ action in the finance request. This action increases the existing loan amount and the principal outstanding on the date of each partial disbursement. Additionally, the corresponding interest, tax, and charges are collected at the time of each disbursement.

The loan created for each invoice will follow the lending life cycle and the document status of the invoice is updated as 'Financed'.

To disburse the finance request,

1. Ensure that the SU.FUNDING.SERVICE service is running.
2. Pending Disbursement .
3. Select the Disburse Record option.

> **⚠️ Note:** The finance request details can be edited at any point before the initiating the disbursement action. If no changes are required, the record can be processed further for disbursement through the service.

After processing and disbursing the finance request, the net disbursement amount is credited to the borrower. On successful disbursement, the finance request can be viewed with the details such as the finance request itself, facility overview, each drawing overview, and other basic information like invoice amount, financed amount, maturity date, and drawing reference.

Disbursed Finance Request.

The below screenshot shows an example of a successfully disbursed finance request with the Invoice Batch details. From the batch, the bank can view the list of drawings for the invoices.

The below screenshot shows the details of the loan created for the invoices in the batch.

The below screenshot shows an example of a successfully disbursed finance request with the single invoice details.

> **⚠️ Note:** Drawings created for an invoice are based on the product specified in the finance request. The Receivables Discounting product includes an Advance Interest feature, where interest and tax on the loan amount are deducted at disbursement, and the net amount is credited to the borrower. In contrast, the Factoring product collects interest at the time of maturity.

The exchange rate is enhanced for both the facility and drawings in SCF. It is triggered when the arrangements are created in different currencies. For example, consider a scenario where the programme is created in GBP currency and the facility is created in EUR.

When the multi-currency record is financed, a drawing is created under the above facility in USD.

The container bill is raised in the drawing currency. The system considers the currency conversion from the mid reval rate from the CURRENCY table to update the facility balance.

The following are the restrictions in SCF regarding exchange rate:

- Any backdated exchange rate activity is restricted for both facility and drawing. If any backdated exchange rate activity is performed, the system throws the below error.
- The Initiation and Prior Days fields in the exchange rate are disabled for SCF.

Read Working with Multi-Currency Facility and Drawings section for more information on exchange rates.


##### Resubmission and Delinking of Invoice in Finance Request

If a bank user finances a batch and unexpected issues cause the finance request to move to the error queue, Transact offers a functionality to identify and resolve these errors, enabling the process to continue toward disbursement. The bank has two options to proceed with the finance request:

- Delinking Invoices: Similar to unbatching, the bank can delink the invoices from the batch facing issues.
- Rectifying Errors and Resubmitting: The bank can rectify the error and proceed with the ‘Resubmit’ action to credit the net disbursement amount to the borrower.

To delink and resubmit the finance request,

1. Ensure that the SU.INVOICE.SERVICE and SU.FUNDING.SERVICE services are running.
2. Unsuccessful Disbursement.
3. Select the Resubmit option once the bank rectifies the error to process the finance request.

Upon successful completion, the net disbursement amount is credited to the borrower.

The below screenshot shows the option to delink an invoice within the error queue.


##### Loan Repayment

Repayment .

The below screenshot shows a loan being repaid with the invoice reference.

Once the loan is repaid in full, the loan status moves to ‘closed’. The below screenshot shows the status of the loan arrangement.


##### Invoice Settlement

When the underlying loan associated with an invoice is closed and the retention amount is repaid by the borrower or counterparty, the bank can settle the invoice for tracking purposes. The Transact system also allows recording repayment details on the invoice, facilitated by attributes in the invoice capture application.

To settle an invoice,

1. Invoice Settlement. The invoice appears at in the Invoice settlement section only after the loan status is updated to closed.
2. Select the Settle Invoice option and authorize the record.

The status of the invoice is changed to ‘Settled’ and the invoice archival occurs subsequently based on the configuration in the Invoice Parameter application.

The below screenshot illustrates the Invoice settlement process.

Authorise Invoice . Once the record is authorised, the invoice updates it’s document status as ‘Settled’ as shown below.

Settlement of the invoice marks the end of the life-cycle for the captured invoice and implies that all dues on the loan for the invoice is cleared.


#### 📋 Tasks

There are no Tasks available for Finance Request.


#### 📊 Outputs

There are no Outputs available for Finance Request.


> **Related Applications:** `CURRENCY`, `SU.FINANCE.REQUEST`, `SU.INVOICE.BATCH`, `SU.INVOICE.CAPTURE`

---


### 4.3  Invoice Batching


> **📇 Quick Reference Card**
> 
> **Purpose:** *In Transact, Invoice batching refers to the process of grouping multiple invoices based on predefined and configurable selection criteria for financing purposes. By default, invoices are grouped into batches based on their Payment Due Date, that is, invoices with the same Payment Due Date are groupe...*
> 
> **Applications:** `SU.BATCH.CONDITION`, `SU.INVOICE.BATCH`, `SU.INVOICE.CAPTURE`
> 
> **Key Fields:** *Auto Batch*, *Auto Batch Reference*, *Available Amount*, *Batch Reference*, *Borrower*, *Borrower Role*, *Counterparty*, *Counterparty Role* ... +11 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

In Transact, Invoice batching refers to the process of grouping multiple invoices based on predefined and configurable selection criteria for financing purposes. By default, invoices are grouped into batches based on their Payment Due Date, that is, invoices with the same Payment Due Date are grouped together.

For operational convenience, Transact offers the flexibility to group invoices using Bank-Defined Criteria through Batching Conditions. These conditions allow the users to configure batching criteria based on Invoice Amount, Payment Due Date, and Financing Date. Batching Conditions can be set both at the Company and Borrower levels. If conditions are set at both the levels, the system prioritizes the Borrower-specific conditions while grouping the invoices into batches.


#### ⚙️ Configuration

There is no specific configuration required for this feature.


#### 🔧 Working With

This section explains the creation and reversal of batching conditions, creating invoice batches and unbatching invoices.


##### Defining Batching Condition

In Transact, the bank can define a set of criteria to group invoices and improve operational efficiency. This functionality is enabled through the SU.BATCH.CONDITION application. Users can define the criteria for the entire company or for specific borrowers using combinations of the Amount, Payment Due Date, and Financing Date fields from Captured Invoices. This helps the user to streamline the batching process and it is at the bank’s convenience to create a batching condition.

> **⚠️ Note:** The SU.BATCH.CONDITION application is used for creating batching conditions to group multiple Invoices. Batching Condition is an additional feature in Transact for grouping of invoices, and not a prerequisite for grouping of invoices.

The following fields are available in the SU.BATCH.CONDITION application to define conditions for batching.

| Field | Description |
|---|---|
| Description | Holds the description for the record. |
| Invoice Field | Holds the field reference from the SU.INVOICE.CAPTURE application. |
| Decision | Holds the decision parameters like EQ, LT, GT, LE, GE, RG, and so on. |
| Value From | Holds the criterion value for the Invoice Capture field. |
| Value To | Holds the criterion end value for the Invoice Capture field. |
| Available Amount | Specifies the available amount for disbursement for the batch attached to the finance request. This is calculated based on the sum of the face values of the attached invoices, deducting the retention margin configured at the facility attached in the finance request. This is updated at the end of each ‘Disburse’ action through a service. |

Batching Conditions .

A batching condition record can be created in the following ways:

To optimise the process of grouping invoices, banks can establish company-level batching criteria using the combinations of the following attributes from the captured invoices:

- Payment Due Date
- Invoice Amount (Face Value)
- Financing Date

Invoices that meet the defined batching conditions are grouped and processed accordingly as shown below.

The below screenshot shows an example of the company-level batching criteria, using the company reference as the record reference, where the invoices with a face value ranging from 10,000 to 20,000 are grouped into a single batch.

Banks can also set and modify conditions for batching invoices based on borrower-specific criteria. These conditions can be adjusted multiple times to reflect the changes in invoice processing terms with the borrower. For example, if the borrower initially requested funding for invoices ranging from $100 to $1,000, but now there is a new request to fund invoices ranging from $500 to $1,500. The invoices that are about to be batched adhere to the newly updated conditions.

Similar to the company-level batching conditions, the borrower-specific batching criteria allows the bank to create conditions for batching invoices based on the following attributes available in the Invoice Capture application:

- Payment Due Date
- Invoice Amount (Face Value)
- Financing Date

Using this combination, banks can group invoices from a borrower that match these selection criteria, facilitating the financing process.

The below screenshot shows an example of the borrower-specific batching criteria, the standard format "C- " for record references, where the invoices with a payment due date later than January 30, 2024, are selected for grouping.


##### Reversing Batch Condition

Batch conditions can be reversed at the bank's convenience if the batching condition for a specific company or borrower becomes obsolete. To reverse the batching condition,

1. Reverse Batching Conditions. Each batch condition has options to view and reverse the record.
2. Select the Reversal Record option to trigger the reversal of the batching condition as shown below.


##### Creating Invoice Batch

When invoices are grouped under a batch record, the system updates the status of each invoice as ‘Batched’ and records the batch reference in the invoice.

Below are the attributes available in the SU.INVOICE.BATCH application,

| Field | Description |
|---|---|
| Borrower | Specifies the Transact customer reference for whom the finance is disbursed. This is a mandatory field. |
| Borrower Role | Specifies the role of the customer. This field is mandatory when BORROWER is updated. |
| Counterparty | Specifies the counterparty reference. This is a mandatory field. |
| Counterparty Role | Specifies the role of the counterparty. This field is mandatory when a counterparty is defined. |
| Currency | Specifies the currency in which finance will be disbursed. This is a mandatory field. |
| Invoice Reference | Specifies the reference of the grouped invoices. A minimum of two Invoices should be given when batching action is performed. And a maximum of 10 Invoices can only be updated manually by the bank user. |
| Unbatch | Used to unbatch already batched invoices. |
| No of Invoices | Specifies the number of invoices selected under a batch. |
| Finance Request | Specifies the Finance Request ID under which the batch is financed. |
| Upload Reference | Specifies the upload reference for the invoices that were processed through bulk upload. This is used as a criterion for batching by upload reference. |
| Auto Batch | Used to initiate batching by selection based on the given criteria. This field is optional. |
| Batch Reference | Specifies the Sub-Batch reference created during Auto batch. |
| Auto Batch Reference | Specifies the batch reference created during Auto batch. This is a system-updated field, and is updated only during the Auto batching process. |

Following are the ways to batch invoices for further processing:

This feature enables users to group invoices when fewer invoices are requested for financing, making operations more efficient. Banks can manually group two to ten invoices into a single batch, which is then identified with a batch reference for further processing.

Manual batching of invoices requires user input for the common attributes such as Borrower , Borrower Role , Counterparty , Counterparty Role , and Currency . Additionally, all the invoices in the batch must have the same payment due date.

> **⚠️ Note:** The system does not adhere to the batching condition for manual batching of invoices.

To manually batch the invoices,

1. Manual Batch .
2. Configure the mandatory fields such as Borrower , Borrower Role , Counterparty , Counterparty Role , Currency , and Invoices (2 to 10 Invoice) that needs to be grouped together as shown below. The below screenshot shows the sample input to Invoice Reference field, which can be multivalued and a maximum of ten invoices can be added manually.

To authorise or delete a manual batch,

1. Authorise/ Delete Batch.
2. Select the Authorise option to initiate authorisation.
3. Select the Delete option to delete the batch before authorisation.

When a batch record is deleted, the system updates the status of the invoices in that batch back to ‘New’, making them available for further processing.

Below is the sample output of manual batch.

Transact allows the bank to reverse existing manual batch records, provided they are not part of any finance request. When a batch record is reversed, the system updates the status of the invoices in that batch back to ‘New’, making them available for further processing.

To reverse a batch record,

1. Reverse Batch . Each batch condition has options to view and reverse the record.
2. Select the Reversal Record option to trigger the reversal of the batching condition as shown below.

This feature enables banks to consolidate a large number of invoices into a single batch with minimal input in the mandatory fields such as Borrower, Borrower Role, and Currency. This reduces the operational time required to batch a large volume of invoices. Auto batching is a process of grouping invoices based on predefined and bank-configured criteria such as borrower details, currency, upload reference, and counterparty details.

Once the invoices are batched, a Batch Reference is created to represent the group of invoices (Auto-Batch Reference). This Auto-Batch can include multiple child batches which are referred to as Sub-batches.

Sub-batches are formed in the following scenarios:

- When Borrower details and Currency are provided in the Batch record without specifying Counterparty details, the system groups invoices with shared attributes. If these grouped invoices involve multiple counterparties, they are further divided into sub-batches by counterparty to ensure consistent batch structure.
- If the grouped invoices have multiple payment due dates, the system applies predefined criteria, such as the payment due date, to create sub-batches. Invoices with the same due date are grouped together within a sub-batch.

These sub-batch references are stored under the Auto-Batch Reference. To perform Auto-Batching of the invoices, ensure that the SU.INVOICE.SERVICE service is running.

Auto-Batching can be performed in the following ways:

Batching by Selection is the process of grouping all the invoices in the system based on borrower, borrower role, currency, and any batching conditions. This method allows the system to batch invoices with common attributes based on user input. Transact offers the flexibility to include counterparty and counterparty role as criteria, tailored to the bank's requirements. This approach enhances operational efficiency in the further processing.

Batching by Selection .

The below screenshot shows a sample input for the mandatory fields. When the record is committed, the system groups the invoices with similar attributes and batches them accordingly.

Batching by Upload Reference is the process of grouping invoices submitted by a borrower, identified by an upload reference. This involves grouping of invoices based on Borrower , Borrower Role , Currency , Upload Reference , and any Batch conditions (defined earlier in SU.BATCH.CONDITION ) as basic criteria. Banks can include Counterparty and Counterparty Role as additional criteria.

Batching by Upload Reference .

The below screenshot shows a sample input for the mandatory fields, including the Upload Reference. When the record is committed, the system groups the invoices with similar attributes and batches them accordingly.

The below screenshot shows a sample of the auto-batch record created with multiple sub-batches.

The Reversal functionality in Transact allows the bank to reverse existing Auto or Sub batch records, provided they are not part of any finance request. When a batch record is reversed, the system updates the invoice status as ‘New’ in that batch, making them available for further processing.

To reverse an auto batch and sub-batch,

1. Reverse Auto Batch.
2. Reverse Individual Batch.
3. Select the Reverse Batch option to reverse the invoice batch record as shown below.


##### Un-Batching of Invoices

Transact provides an option to unbatch invoices from the batch record before initiating a finance request. This functionality allows the users to remove an invoice from a batch if required, for example, when the borrower no longer wants financing for a specific invoice, or the bank decides not to fund it. Unbatching can be performed at any time before initiating the financing process.

Additionally, Transact offers the flexibility to remove failed invoices during the drawing creation process. This ensures that funds can be provided to the borrower without reversing the entire batch and redoing the process. Invoices can be unbatched until the invoice count in the batch record is reduced to a minimum of two.

To unbatch invoices, ensure that the SU.INVOICE.SERVICE service is running. Following are the options provided to unbatch invoices:

Banks can use the following operations to unbatch invoices before financing:

- Un-batch: To unbatch a single invoice or multiple invoices from a batch.
- Un-batch All: To unbatch the invoices from multiple batches simultaneously.

To unbatch the invoices before financing,

1. Unbatch .
2. Use the batch reference to select the invoice batch that needs to be unbatched.
3. Once the batch details are displayed, provide the sample input to un-batch the invoice from the respective batch record as shown below.

During financing, banks can unbatch the invoices in the failed status.

To unbatch failed invoices,

1. Add/Remove Invoice .
2. Use the batch reference to select the invoice batch that needs to be unbatched.
3. Once the batch details are displayed, enable the Unbatch checkbox to remove the invoice from the specified batch as shown in below.


#### 📋 Tasks

There are no Tasks available for Invoice Batching.


#### 📊 Outputs

There are no Outputs available for Invoice Batching.


> **Related Applications:** `SU.BATCH.CONDITION`, `SU.INVOICE.BATCH`, `SU.INVOICE.CAPTURE`

---


### 4.4  Invoice Capture


> **📇 Quick Reference Card**
> 
> **Purpose:** *An invoice is the major financial document that represents a transaction between a supplier and buyer. The supplier raises an invoice in favor of the buyer once they ship the underlying goods. In the realm of Supply Chain Finance, the invoices, and their attributes such as face value, invoice due da...*
> 
> **Applications:** `AA.CUSTOMER.ROLE`, `CURRENCY`, `EB.DUPLICATE.TYPE`, `EB.FILE.UPLOAD`, `SU.INVOICE.CAPTURE`, `SU.INVOICE.TYPE`, `SU.PARAMETER`
> 
> **Key Fields:** *Amount*, *Available Amount*, *Batch Reference*, *Currency*, *Days Post Mat*, *Days Post Maturity*, *Document Status*, *Document Type* ... +21 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

An invoice is the major financial document that represents a transaction between a supplier and buyer. The supplier raises an invoice in favor of the buyer once they ship the underlying goods. In the realm of Supply Chain Finance, the invoices, and their attributes such as face value, invoice due date, and so on determine the various aspects of finance against invoices, such as the loan amount, the loan maturity date, and so on. It is therefore important to create a record of these invoices in Transact for future processing of loans against these invoices. In Transact, the invoices can be uploaded in the following ways:

- Manual Capture: Manual capture is used when the bank user wants to manually input a set of invoices into the system one-by-one.
- Bulk Capture: Bulk Capture is used when there are multiple invoices or batches of invoice that needs to be captured in bulk. The invoices are uploaded in a defined file format (.csv) through the EB.FILE.UPLOAD application which helps with the upload of invoices in bulk.


#### ⚙️ Configuration

Parameters .

The following fields are available in the SU.PARAMETER application:

| Field | Description |
|---|---|
| Days Post Maturity | Stores the number of days after which the invoices with settled status will be automatically transferred to the History file. This field is mandatory. |
| Duplicate Check | Holds the duplicate check definition for the SU.INVOICE.CAPTURE table to prevent duplicate upload of Invoices. The ID of EB.DUPLICATE.TYPE must be updated in this field to enable the duplicate check functionality. This field is optional. |
| Document Type | Specifies the document type used in SU.INVOICE.CAPTURE . This field refers to the virtual table SU.INVOICE.TYPE . Only the document types defined here are permitted in SU.INVOICE.CAPTURE . It is mandatory to define at least one document type. |
| Role | Holds the list of participants permitted for the specified document type. A minimum of two roles must be defined when configuring the document type. This field refers to AA.CUSTOMER.ROLE and becomes mandatory when a document type is specified. |
| Role Required | Holds the list of participants permitted for the specified document type. A minimum of two roles must be defined when configuring the document type. This field refers to AA.CUSTOMER.ROLE and becomes mandatory when a document type is specified. |

The EB.DUPLICATE.TYPE application has the configurations that contains the definition for duplicate check on the uploaded invoice. For an invoice, is the original reference, document type for duplicate check fields are replicated, the system throws an error. This duplicate check is handled in the SU.PARAMETER application as it serves as the base configuration at the company level.

> **⚠️ Note:** When more than one invoice must be uploaded, bulk uploading can be performed. Read EB.FILE.UPLOAD section for more information.


#### 🔧 Working With

When a bank engages in invoice financing, it is mandatory to capture the invoice information, which must be stored within the system to facilitate efficient invoice management. The SU.INVOICE.CAPTURE application captures the invoice details and serves as a repository for the invoice particulars and finance-related information, ensuring seamless tracking and management of the invoices. The following fields are available in the SU.INVOICE.CAPTURE application:

| Field | Description |
|---|---|
| Original Reference | Specifies the invoice reference number imported from the customer-submitted invoice. This field is an alpha numeric field with a maximum of 35 characters. It is a mandatory field. |
| Document Type | Holds the document type. It refers to virtual table SU.INVOICE.TYPE . The user can select the invoice types that are defined in the SU.PARAMETER . This field is mandatory. |
| Party | Specifies the customer who is part of the document. Holds the Transact customer reference and Mnemonic. This is a mandatory field. |
| Role | Specifies the role of the customer, for example, whether the captured customer is a SUPPLIER or BUYER. It refers to AA.CUSTOMER.ROLE. This is a mandatory field when Party is defined. The system only allows the roles that are part of the parameter defined for the document type. |
| Currency | Holds the currency of the invoice. It refers to the CURRENCY table for validation. It should be a valid record in the CURRENCY table. This is a mandatory field. |
| Amount | Holds the value of invoice amount which should be greater than 0.00. This is a mandatory field. |
| Issued Date | Specifies the date on which the invoice was issued by the drawer. It should be in standard date format (cannot be a future date). This is imported from the invoice submitted by the customer. This is a mandatory field. |
| Payment Due Date | Specifies the date on which the invoice is due for payment, and the drawee is expected to pay the Invoices. It is a standard date format field. The value should be greater than issued date. This is a mandatory field. |
| Financing Date | Specifies the date on which the borrower wants the invoices to be financed. It is a standard date format field. The date should not be greater than the payment due date and less than the issue date. This is an optional field. |
| Remarks | Stores remarks or comments if any. This is an optional field with a maximum of 100 characters. |
| Upload Reference | Stores the upload reference when the invoices are uploaded in bulk. |
| Document Status | This is a system-maintained field which holds the status of the invoice at various stages. Following are the possible values: NEW – updated when the Invoice is uploaded. BATCHED - updated when the Invoice is Batched. Unbatching the Invoice from the batch reverses the status back to NEW. FINANCED - updated when the Invoice is financed. FINANCE REQUESTED - updated when the Invoice is directly attached to the finance request for finance disbursement. Removing the invoice reference from the finance request reverses the status back to NEW. SETTLED - updated when the loan on the Invoice is fully settled and the SETTLE.INVOICE field is set. |
| Status Date | Specifies the date on which the status was last updated. |
| Batch Reference | Holds the batch reference under which the respective invoice is batched. This is a system-updated field. This field also holds the finance request reference when one invoice is financed from a finance request. |
| Financing Request | Holds the Finance Request Reference ID of the captured invoice upon requesting for finance. This is a system-updated field. |
| Finance Amount | Holds the finance amount. This field is updated by the system when the invoice is financed. |
| Drawing Reference | Contains the Drawing Reference ID generated for the specific invoice upon disbursement as part of financing. This is a system-updated field. |
| Payment Type | Holds the payment type. This field can be configured by the user from the virtual table EB.LOOKUP - SU.PAYMENT.TYPE. |
| Payment Currency | Holds the currency of the payment amount done on the invoice, which should be a valid currency defined in the CURRENCY table. |
| Payment Amount | Holds the payment amount done on the invoice. This is a system-updated field. |
| Payment Date | Holds the date of payment done on the invoice. This is a system-updated field. |
| Reference | Holds the payment reference. This is a free text field, with the length of 50 character. This field is optional. |
| Settle Invoice | This is an optional field which allows the user to settle the invoice. This field can be configured only when the invoice is already financed. If the underlying loan status is neither close nor pending closure, the system throws a validation error on committing the SU.INVOICE.CAPTURE with SETTLE.INVOICE set to Yes. On successful commit, the document status for the invoice is updated as ‘Settled’. |
| Available Amount | Specifies the available amount for disbursement in the invoice batch attached to the finance request. This is calculated based on the sum of the face values of the invoice, deducting the retention margin configured at the facility attached in the finance request. This is updated at the end of each ‘Disburse’ action through a service. |


###### Manual Upload of Invoices

Invoice Capture.

The below screenshot displays the manual capture of invoices.


###### Bulk Upload of Invoices

Bulk upload is introduced to process multiple invoices as each invoice cannot be captured manually. To streamline this process, all the invoice details are recorded in a csv file and can be uploaded through EB.FILE.UPLOAD . Click here to view the sample csv file created for the bulk upload of invoices.

> **⚠️ Note:** In the above file, the invoices are entered in the file and are uploaded through the bulk upload.

The below table shows the sequence of data updates in Transact when invoices are uploaded through a bulk file.

| Sequence | Fields updated |
|---|---|
| 1 | Original Reference |
| 2 | Document Type |
| 3 | Party |
| 4 | Role |
| 5 | Currency |
| 6 | Amount |
| 7 | Issue Date |
| 8 | Payment Due Date |
| 9 | Financing Date |
| 10 | Upload Reference |

To capture the invoices in bulk,

1. Bulk Upload .
2. Choose the file to be uploaded.
3. Capture the invoice details in SU.INVOICE.CAPTURE application and commit the record. The below screenshot shows the captured invoice. The below screenshot shows the party and their roles in the invoice captured. The below screenshot shows the status of the invoice captured. When a similar invoice is replicated and the record is committed, the system throws the below validation.
4. After uploading the file through bulk upload, commit the record. After authorising the record, the uploaded invoices can be viewed after running the T24.UPLOAD.PROCESS service. If the data in the sample csv file is correct without any errors, after running the above services the data is available in enquiry invoice list.
5. Invoice List. The below screenshot shows the invoice list enquiry criteria. If the highlighted criteria in the above screen is selected, the list of invoices are displayed as shown below.
6. Invoice List . To view the invoice, provide the upload reference of the bulk upload as shown below. Once the upload reference is given, all the invoices captured through the bulk capture are displayed. The highlighted invoice reference in the below picture shows the amended invoice of invalid currency. All the invoices with errors must be rectified before they move on to the next stage.


###### Archival of Invoices

Settled Invoices and the invoices that have crossed maturity but not financed from SU.INVOICE.CAPTURE application are moved to the $HIS file after Days Post Mat is configured in SU.PARAMETER . Below is the SU.PARAMETER record which has Days Post Mat defined.

Archival is the process of removing the invoices in the $HIS file to the archival database, which is performed through the ARC.GENERIC.PROCESS service. Below is the archive record released by Temenos for the archival process.


#### 📋 Tasks

There are no Tasks available for Invoice Management.


#### 📊 Outputs

There are no Outputs available for Invoice Management.


> **Related Applications:** `AA.CUSTOMER.ROLE`, `CURRENCY`, `EB.DUPLICATE.TYPE`, `EB.FILE.UPLOAD`, `SU.INVOICE.CAPTURE`, `SU.INVOICE.TYPE`, `SU.PARAMETER`

---


### 4.5  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *Supply Chain Finance (SCF), also known as supplier finance or reverse factoring, is a financing solution where suppliers can receive early payment on their invoices by reducing the risk of supply chain disruption and enabling both the buyers and suppliers to optimise their working capital.*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Supply Chain Finance (SCF), also known as supplier finance or reverse factoring, is a financing solution where suppliers can receive early payment on their invoices by reducing the risk of supply chain disruption and enabling both the buyers and suppliers to optimise their working capital.

Transact facilitates supplier-led financing, wherein the supplier provides goods or services to the buyer and subsequently submits the relevant invoice to the financial institution for processing. Upon approval of the invoice, the supplier needs to request early payment from a financing provider, typically a bank or financial institution.

The parties involved in SCF are:

- Buyers
- Suppliers
- Financial Institutions


##### Supplier-led Supply Chain Programme

Following are the attributes that are typically associated with supplier-led finance.

- Initiator: The financing arrangement is initiated by the suppliers.
- Process: The supplier typically factors their invoices to a financial institution to receive early payment at a discount. (Typically, discounted interest is collected in advance, calculated based on the number of days from the finance date to the invoice maturity date, along with any additional upfront fees that may be charged by the financial institution).
- Onus of Re-Payment: The onus of re-payment is on the buyer if the agreement is without recourse and it is on the supplier if the agreement is with recourse.

Following are the techniques for supplier-led supply chain programme:

Receivables Discounting: This method allows funding based on receivables, such as invoices. Usually, financing is provided at a rate between 75-100% of the receivables’ value, which is then repaid in full to the finance provider by the debtor. Any remaining portion of the receivables that were not financed is returned.

Factoring: Sellers of goods and services sell their receivables represented by outstanding invoices, at a discount to a finance provider (commonly used as a factor). The finance provider advances the funds, manages the debtor portfolio (including collection of the underlying receivables), and provides protection against the obligors’ insolvency.


##### SCF Life Cycle

This section explains the functions involved in Supply Chain Finance.

The below diagram illustrates the invoice life cycle.

The below diagram illustrates the agreement and loan life cycle.

Following are the steps involved in the SCF life-cycle:

- Supply Chain Finance Programme is a Financial arrangement between the Borrower and the Financial Institution, where suppliers can receive early payment on their invoices at a discounted rate, facilitated by a financial institution.
- Facility Agreement is where the agreements between the buyer, supplier, and finance provider is set up and it is a crucial step in structuring a Supply Chain Finance (SCF) transaction. These agreements delineate the roles, responsibilities, and conditions for all parties involved. This process includes defining retention margin of the invoice face value, defining grace days for repayment, and defining counterparty limits and any agreement level fees.
- Invoice Management in Supply Chain Finance encompasses the collection of invoice details for financing the invoices. This includes critical information such as the Invoice amount, Issue date, and payment due date. Additionally, it involves monitoring invoices throughout their lifecycle stages to facilitate reconciliation and auditing.
- Invoice Batching is the process of batching invoices when the loan is requested on more than one Invoice. When more than one invoices are considered for financing they are batched to proceed further for financing. Financing of invoices is done in the same currency and for the same borrower (supplier in supplier-led financing). Batches must be of same payment due date.
- Invoice Financing in SCF is a process that enables the suppliers to obtain early payment for their invoices, thereby enhancing their cash flow and overall financial health.
- Invoice Repayment is the process where the buyer repays the invoices on the payment due date, which is used to settle the Finance obtained by the supplier.


##### Configuring Supply Chain Finance

The following property classes are specific to the SCF products:

| Column 1 | Column 2 | Column 3 |
|---|---|---|
| Account | Accounting | Activity Mapping |
| Customer | Tax | Term Amount |
| Activity Presentation | Payout Rules | Payoff |
| Settlement | Payment Rules | Charge |
| Overdue | Pricing Grid | Exchange Rate |
| Activity Messaging | Limit | Inheritance |


##### Illustrating Model Products

The Supply Chain Finance module is pre-configured with the following model products.

| Sl.no | Product Name | Product Attributes |
|---|---|---|
| 1 | SCF Programme | SCF Deal |
| 2 | SCF Facilities | SCF Revolving Facility SCF Term Facility |
| 3 | SCF Drawings | Factoring Receivables Discounting |

---


---


## Chapter 5: Trade_Banking - TCIB


Trade_Banking - TCIB module of Temenos Transact


### Features in Trade_Banking - TCIB


| # | Feature | Sections |
|---|---------|----------|
| 5.1 | Collection | Intro, Confi, Tasks, Outpu |
| 5.2 | Export Drawings | Intro, Confi, Tasks, Outpu |
| 5.3 | Export LC Advising | Intro, Confi, Worki, Tasks, Outpu |
| 5.4 | Export LC Amendemnt Advising | Intro, Confi, Tasks, Outpu |
| 5.5 | Guarantee Amendment | Intro, Confi, Tasks, Outpu |
| 5.6 | Guarantee Claims | Intro, Confi, Tasks, Outpu |
| 5.7 | Guarantee Issuance | Intro, Confi, Tasks, Outpu |
| 5.8 | Guarantees Received | Intro, Confi, Tasks, Outpu |
| 5.9 | Import Drawings | Intro, Confi, Worki, Tasks, Outpu |
| 5.10 | Import LC Amendment | Intro, Confi, Tasks, Outpu |
| 5.11 | Import LC Issuance | Intro, Confi, Tasks, Outpu |
| 5.12 | Misc | Intro |
| 5.13 | TCIB Dashboard | Intro, Confi, Tasks, Outpu |


### 5.1  Collection


> **📇 Quick Reference Card**
> 
> **Purpose:** *The exporter or importer handling trade collections stands to benefit by placing their collection instruction using online banking platform which provide real time intimation of the transaction. The movement of the actual documents to the bank or received from the bank happens later.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The exporter or importer handling trade collections stands to benefit by placing their collection instruction using online banking platform which provide real time intimation of the transaction. The movement of the actual documents to the bank or received from the bank happens later.


#### ⚙️ Configuration

There are no specific configuration to be setup at feature level. The parameter tables are setup at the implementation stage.


#### 📋 Tasks

There are no Tasks available for Collection feature.


#### 📊 Outputs

There are no Outputs available for Collection feature.

---


### 5.2  Export Drawings


> **📇 Quick Reference Card**
> 
> **Purpose:** *An export LC presentation using an online platform reduces turnaround time for parties involved, while establishing a precedent for faster, secure and cost-efficient settlement of cross-border trade transaction.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

An export LC presentation using an online platform reduces turnaround time for parties involved, while establishing a precedent for faster, secure and cost-efficient settlement of cross-border trade transaction.


#### ⚙️ Configuration

There are no specific configuration to be setup at feature level. The parameter tables are setup at the implementation stage.


#### 📋 Tasks

There are no Tasks available for Export Drawings feature.


#### 📊 Outputs

There are no Outputs available for Export Drawings feature.

---


### 5.3  Export LC Advising


> **📇 Quick Reference Card**
> 
> **Purpose:** *This service allows the beneficiary to get a single point access to the repository of all advised LCs using online banking platform, (before it gets the physical authentic LC). The exporter receives real time intimation once LC is transmitted and advised. Additionally, SWIFT message of LC is viewed ...*
> 
> **Key Fields:** *Bank to Customer info*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

This service allows the beneficiary to get a single point access to the repository of all advised LCs using online banking platform, (before it gets the physical authentic LC). The exporter receives real time intimation once LC is transmitted and advised. Additionally, SWIFT message of LC is viewed or downloaded according to the requirement.


#### ⚙️ Configuration

There are no specific configuration to be setup at feature level. The parameter tables are setup at the implementation stage.


#### 🔧 Working With

Export Letter of Credit (LC) is advised using Temenos Internet Banking Channel (TCIB), where the summary of the LC details and preview of the electronic copy of LC is available for the corporate customer (who has signed up and on-boarded into the internet banking channel). The corporate customer can download the summary and electronic copy of LC in PDF format.

The below steps are involved in the export LC Advising internet banking flow:

When an incoming MT700 is received by the bank, the system auto processes the swift message and creates a LC record in the system and places it in the respective enquiry (for the user for further action).

The user can do the following:

- Edit the record created by the system
- Update further details
- Collect charges (if customer account details are available)
- Authorise the record in the system

> **⚠️ Note:** For non-swift LCs the user manually creates the record.

The bank user updates the information that needs to be communicated to the corporate user in respect to the subject export LC using Bank to Customer info field.

> **⚠️ Note:** The user can enter a value in this field, only if the beneficiary of the LC to be advised is an internet banking enabled customer.

The record is then displayed in TCIB channel after due authorisation in the system by the bank user.

The corporate customer can view the summary of the export LC details, preview and download the copy of the LC details and electronic copy of incoming MT700. If charges are collected by the bank, then debit advice is available for preview and download.

More Details available in the Detailed Descriptions section display the additional details in a pop-up screen.

Respective delivery messages and advices addressed to the corporate customer is displayed in the Swift messages and advices section for preview in TCIB. TCIB corporate user can download the summary of LC details, delivery messages and advices in PDF format from the TCIB screen.


#### 📋 Tasks

There are no Tasks available for Export LC Advising feature.


#### 📊 Outputs

There are no Outputs available for Export LC Advising feature.

---


### 5.4  Export LC Amendemnt Advising


> **📇 Quick Reference Card**
> 
> **Purpose:** *This service enables the beneficiary to get a single point access to the repository of all amendments to the existing LCs using online banking platform, (before receiving physical authentic LC amendment). The exporter receives real time intimation once LC amendment is transmitted and advised. Additi...*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

This service enables the beneficiary to get a single point access to the repository of all amendments to the existing LCs using online banking platform, (before receiving physical authentic LC amendment). The exporter receives real time intimation once LC amendment is transmitted and advised. Additionally, SWIFT message of LC is viewed or downloaded according to the requirement.


#### ⚙️ Configuration

There are no specific configuration to be setup at feature level. The parameter tables are setup at the implementation stage.


#### 📋 Tasks

There are no Tasks available for Export LC Amendment Advising feature.


#### 📊 Outputs

There are no Outputs available for Export LC Amendment Advising feature.

---


### 5.5  Guarantee Amendment


> **📇 Quick Reference Card**
> 
> **Purpose:** *The corporate customer can place a request to issue an amendment to the guarantee using online banking platform (this is similar to a guarantee Issuance request).*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The corporate customer can place a request to issue an amendment to the guarantee using online banking platform (this is similar to a guarantee Issuance request).


#### ⚙️ Configuration

There are no specific configuration to be setup at feature level. The parameter tables are setup at the implementation stage.


#### 📋 Tasks

There are no Tasks available for Guarantee Amendment feature.


#### 📊 Outputs

There are no Outputs available for Guarantee Amendment feature.

---


### 5.6  Guarantee Claims


> **📇 Quick Reference Card**
> 
> **Purpose:** *Guarantee claim handling is done using online banking platform, which gives the customer the convenience for submitting trade transaction on-time for immediate action and process.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Guarantee claim handling is done using online banking platform, which gives the customer the convenience for submitting trade transaction on-time for immediate action and process.


#### ⚙️ Configuration

There are no specific configuration to be setup at feature level. The parameter tables are setup at the implementation stage.


#### 📋 Tasks

There are no Tasks available for Guarantee Claims feature.


#### 📊 Outputs

There are no Outputs available for Guarantee Claims feature.

---


### 5.7  Guarantee Issuance


> **📇 Quick Reference Card**
> 
> **Purpose:** *Corporate customer can place a request to issue guarantees using online banking platform, thereby ensuring transparency in the entire process and making audit trail a possibility in real time. Customer is assured of quicker turnaround time to complete the transaction.*
> 
> **Key Fields:** *Ib Limit*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Corporate customer can place a request to issue guarantees using online banking platform, thereby ensuring transparency in the entire process and making audit trail a possibility in real time. Customer is assured of quicker turnaround time to complete the transaction.


#### ⚙️ Configuration

Limit checkoccurs during the request initiation in TCIB, if Ib Limit set as Yes at the Parameter level. The setup occurs at the parameter level, (if required for a specific group of customers, the it is done using MD.GROUP.CONDITION ).


#### 📋 Tasks

There are no Tasks available for Guarantees Issuance feature.


#### 📊 Outputs

There are no Outputs available for Guarantees Issuance feature.

---


### 5.8  Guarantees Received


> **📇 Quick Reference Card**
> 
> **Purpose:** *The beneficiary of the guarantee can view all advised guarantees, (once it is advised or transmitted, using online banking platform before it gets the physical authentic guarantee).*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The beneficiary of the guarantee can view all advised guarantees, (once it is advised or transmitted, using online banking platform before it gets the physical authentic guarantee).


#### ⚙️ Configuration

There are no specific configuration to be setup at feature level. The parameter tables are setup at the implementation stage.


#### 📋 Tasks

There are no Tasks available for Guarantees Received feature.


#### 📊 Outputs

There are no Outputs available for Guarantees Received feature.

---


### 5.9  Import Drawings


> **📇 Quick Reference Card**
> 
> **Purpose:** *An import LC presentation using an online platform reduces turn-around-time for parties involved, while establishing a precedent for faster, secure and cost-efficient settlement of cross-border trade transaction.*
> 
> **Key Fields:** *Discrepancy*, *Discrepancy Status*, *Documents Received*, *Draw Type*, *Event Status*, *IB Event Status*, *Ib Event Status*, *Ib Limit* ... +2 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

An import LC presentation using an online platform reduces turn-around-time for parties involved, while establishing a precedent for faster, secure and cost-efficient settlement of cross-border trade transaction.


#### ⚙️ Configuration

The Ib Limit field in LC.PARAMETERS is setup. There are no specific configuration to be setup at feature level. The parameter tables are setup at the implementation stage.


#### 🔧 Working With

Corporate client can view document details, list of discrepancies and provide instructions using online channel for a drawing under import Letter of Credit (LC). The bank user can advise the discrepancies to TCIB corporate immediately using online channel and then TCIB corporate user responds (online) immediately.

The discrepancies identified by the bank in import drawing are listed in TCIB for the corporate user to make a choice. The Discrepancy field lists the discrepancies in the record and the user can Waive or Reject each discrepancy. When there are more than one discrepancy, the corporate user can set the Response to Discrepancies as 'Waive All' or 'Reject All' in TCIB.

- The user need not manually enter the value for each discrepancy. When a choice is made, the system automatically updates Discrepancy for all the discrepancies as 'Waive' or 'Reject' accordingly.
- For any additional discrepancies, the corporate user should manually enter the Discrepancy Status for all discrepancies listed.


##### Import Drawings Flow

The following are the steps involved in the import drawings flow using internet banking:

| Section | Description |
|---|---|
| LC Summary | Displays the details of the LC. More details are displayed in pop-up window on selecting the ‘Details view’. |
| Drawings Details | Displays the details of the drawing, including the documents status (Clean documents) and other related details. Incoming MT754 can be viewed and downloaded from the ‘View delivery details’. |
| Payment Details | Allows the corporate user to select the account number from which the payment needs to be effected. |

Incoming MT750 Received

The system auto processes an incoming MT750 and creates an import drawing record (with Draw Type DC) and place the record (in IHLD) in the respective enquiry for the bank user to further process. The bank user then updates the record with details and Event Status field as With Customer to receive the payment or acceptance instructions from the TCIB corporate.

The corporate customer can view the drawings (after bank authoriser authorises the record) and provide acceptance of discrepancies.

TCIB corporate user can provide response to the discrepancies using the Response to Discrepancies field.

The record is listed under Drawings tab as Pend Bank Approval.

The bank user can then pick the record from the respective enquiry and proceed with the payment or acceptance and select the Event Status as Approved. The user can select the Draw Type (SP for sight and AC for usance) to proceed with payment or acceptance.

Payment details are displayed in TCIB and the details along with the SWIFT messages and delivery advices can be viewed and downloaded in PDF format.

When the discrepancies are rejected by the corporate customer, the bank user rejects documents (by generating MT734) and setting Draw Type from DC to CR. The record is displayed as ‘Rejected’ in TCIB.

New Documents Received under Import LC (Incoming MT754 or MT750 is not Received).

In this scenario, the bank user proceeds with the existing process of registering the drawing (RD draw type) and after the documents have been checked the document details and discrepancies (DC draw type), if any is listed in the record and bank user should be able to select IB Event Status field as 'With Customer', so that the record is placed in the TCIB Corporate user’s dashboard for further action.

If Documents Received is set to Yes, then document upload version opens.

Once the record is committed, the user can upload documents in the Upload Documents screen.

Subsequently, if the bank user enters document status, discrepant or clean, and updates event status to ‘With customer’, then the record is displayed in TCIB for further action by the TCIB Corporate user.

TCIB displays all details of the payment or acceptance, once the record is paid or accepted. The SWIFT messages and delivery advices are displayed in TCIB for view and download purposes.


#### 📋 Tasks

There are no Tasks available for Import Drawings feature.


#### 📊 Outputs

There are no Outputs available for Import Drawings feature.

---


### 5.10  Import LC Amendment


> **📇 Quick Reference Card**
> 
> **Purpose:** *Corporate customers can submit trade transaction online. They can place an amendment request to an existing import Letter of Credit (LC) using internet banking platform.*
> 
> **Key Fields:** *Ib Limit*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Corporate customers can submit trade transaction online. They can place an amendment request to an existing import Letter of Credit (LC) using internet banking platform.


#### ⚙️ Configuration

Ib Limit field in LC.PARAMETERS is setup. There are no other specific configuration to be setup at feature level. The parameter tables are setup at the implementation stage.


#### 📋 Tasks

There are no Tasks available for Import LC Amendment feature.


#### 📊 Outputs

There are no Outputs available for Import LC Amendment feature.

---


### 5.11  Import LC Issuance


> **📇 Quick Reference Card**
> 
> **Purpose:** *Corporate customer can place a request to issue Letters of Credit (LC) using internet banking. The customer saves time and ensures faster delivery by applying for a LC using online banking platform.*
> 
> **Key Fields:** *Ib Limit*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Corporate customer can place a request to issue Letters of Credit (LC) using internet banking. The customer saves time and ensures faster delivery by applying for a LC using online banking platform.


#### ⚙️ Configuration

Ib Limit field in LC.PARAMETERS to be setup. There are no other specific configuration setup. The parameter tables are setup at the implementation stage.


#### 📋 Tasks

There are no Tasks available for Import LC Issuance feature.


#### 📊 Outputs

There are no Outputs available for Import LC Issuance feature.

---


### 5.12  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *TCIB provides 24/7 online access to core banking functions across all business lines. TCIB has the following advantages:*
> 
> **Key Fields:** *Ib Limit*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- Temenos Transact Services

TCIB provides 24/7 online access to core banking functions across all business lines. TCIB has the following advantages:

- Cost effective and resilient.
- Seamless integration with Temenos Transact .
- Support of a scalable internet banking infrastructure.
- Effortless navigation by customers to the required service or function.

Advancements in technology have raised the bar of expectations of the corporate customers. They prefer to reach out to banks, which can provide efficient, web driven, cohesive and integrated services to suit individual customer needs. Customers initiating banking transactions using various online channels such as, internet and mobile are gaining popularity. When it comes to trade finance, the corporate customers prefers to do their banking related business transactions using internet banking.

Corporate customers for whom TCIB is enabled, can do the following:

- Place requests online.
- View status of the transactions.
- Provide instructions for further action to the bank.

The bank can send queries or clarification and receive response from the corporate customer online. TCIB is a comprehensive solution and unique platform designed to meet the end-to-end requirements of our trade customers.

Trade finance customers expect banks to do the following:

- Provide solutions that allow them to seamlessly connect with the bank in order to complete their international trade transactions through web portals and/or handheld devices.
- Perform follow up activities required in completing life cycle of a trade.
- Be one-stop-shop for all trade instrument needs such as, documentary credits, guarantee products and collections.
- Meet SLAs for processing the trade transactions without any error.


##### Configuration

The below tables are setup for TCIB.

When a LC issuance or amendment request is placed for an import LC by corporate customers using TCIB channel, the Ib Limit field in LC.PARAMETERS determines the stage at which the customer (applicant) limit is impacted. Allowed values are Yes or No and when set to,

- Yes – Limit entries are raised immediately after the transaction is entered by the corporate user.
- No – Limit is hit after authorisation of the transaction.

When a guarantee issuance or amendment request is placed by corporate customers using TCIB channel, the Ib Limit field in MD.PARAMETER determines the stage at which the customer (applicant) limit is impacted. Allowed values are Yes or No and when set to,

- Yes – Limit entries are raised immediately after the transaction is entered by the corporate user.
- No – Limit is hit only after bank authorisation of the transaction.

The below are the other requirements required to configure TCIB:

- Model bank environment.
- TCIB is mandatory and is available by default.
- Cache expiry in channel parameter (recommended).

The roles (Clerk and Manager) are released as part of model bank. However, the client or services team can configure by creating master arrangement with all permissions by default and restrict the sub arrangement based on the user roles or profiles.

Read Internet Banking Corporate - Channels user guide for Technology, Web Server and Channels related configuration.

---


### 5.13  TCIB Dashboard


> **📇 Quick Reference Card**
> 
> **Purpose:** *A dashboard is a business intelligence tool used to display data visualisations that are immediately understood. It visually tracks, analyses and displays key performance indicators (KPI), metrics and key data points to monitor the day-to-day business or a specific process. They are customisable to ...*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

A dashboard is a business intelligence tool used to display data visualisations that are immediately understood. It visually tracks, analyses and displays key performance indicators (KPI), metrics and key data points to monitor the day-to-day business or a specific process. They are customisable to meet the specific needs of each bank or based on the role of a corporate customer.


#### ⚙️ Configuration

There are no specific configuration to be setup at feature level. The parameter tables are setup at the implementation stage.


#### 📋 Tasks

There are no Tasks available for TCIB Dashboard feature.


#### 📊 Outputs

There are no Outputs available for TCIB Dashboard feature.

---


---


## Appendix A: Glossary of T24 Applications & Fields


This glossary lists all T24/Transact application names and field names referenced throughout this document, with descriptions where available.


### Applications


| Application | Description |
|------------|-------------|
| `AA.ACCOUNT.DETAILS` | T24 application: AA.ACCOUNT.DETAILS |
| `AA.ARRANGEMENT` | T24 application: AA.ARRANGEMENT |
| `AA.CUSTOMER.ROLE` | T24 application: AA.CUSTOMER.ROLE |
| `BL.REGISTER` | T24 application: BL.REGISTER |
| `CURRENCY` | T24 application: CURRENCY |
| `DIPO.ITEMS` | T24 application: DIPO.ITEMS |
| `DISPO.ITEMS` | T24 application: DISPO.ITEMS |
| `DRAWINGS` | T24 application: DRAWINGS |
| `EB.DUPLICATE.TYPE` | T24 application: EB.DUPLICATE.TYPE |
| `EB.FILE.UPLOAD` | T24 application: EB.FILE.UPLOAD |
| `LC` | T24 application: LC |
| `LC.AMENDMENTS` | T24 application: LC.AMENDMENTS |
| `LC.PARAMETERS` | T24 application: LC.PARAMETERS |
| `LC.TYPES` | T24 application: LC.TYPES |
| `MD.CLAUSES` | T24 application: MD.CLAUSES |
| `MD.DEAL` | T24 application: MD.DEAL |
| `PP.RMA` | T24 application: PP.RMA |
| `SU.BATCH.CONDITION` | T24 application: SU.BATCH.CONDITION |
| `SU.FINANCE.REQUEST` | T24 application: SU.FINANCE.REQUEST |
| `SU.INVOICE.BATCH` | T24 application: SU.INVOICE.BATCH |
| `SU.INVOICE.CAPTURE` | T24 application: SU.INVOICE.CAPTURE |
| `SU.INVOICE.TYPE` | T24 application: SU.INVOICE.TYPE |
| `SU.PARAMETER` | T24 application: SU.PARAMETER |


### Fields Referenced


| Field | Field | Field |
|-------|-------|-------|
| `22D` | `31E` | `31E, 32B, 33B, 34B, 39A, 39C, 72Z` |
| `32B or 33B` | `32B, 33B and 34B` | `34B` |
| `34a Tot Amount` | `34b Amount` | `34b Tot Amount` |
| `48D` | `740 Applicable Rule, Presentation Amount` | `740 Reimb Dtd` |
| `740.Reimb.Dtd` | `750 Charges Added` | `750 Charges Deducted` |
| `750 Sender Info` | `754 Charges Added` | `754 Charges Deducted` |
| `77` | `77C` | `@ ID` |
| `@ Id` | `@ Id Or` | `@ID Or` |
| `@Id Or` | `@Id Or Reference 1` | `Account with Bank` |
| `Accrual Cycle` | `Acct With Bank` | `Acct With Bank / Acct With Bank Id` |
| `Acct With Bank Bic` | `Acct With Bank Swift Addr.1` | `Acct With Bank Swift Addr.2` |
| `Action` | `Add Claim Amount` | `Additional Info` |
| `Advice Expiry Date` | `Advice Thru Bk` | `Advice Thru Bk Name` |
| `Advise Through Bank` | `Advised Status` | `Advising Bk` |
| `Advising Bk Name` | `Alternate ID` | `Alternate ID (Guarantee Ref)` |
| `Alternate ID Or @ID` | `Alternate Id` | `Alternate Id /` |
| `Alternate Id Or` | `Alternate Id Or @ID` | `Alternate Id Or @Id` |
| `Alternate Id Or` | `AlternateId Or @ Id Or Reference.1` | `Amend Del` |
| `Amendment No` | `Amort Trans` | `Amortisation Cycle Foreign Currency` |
| `Amortisation Cycle Local Currency` | `Amortise Charges` | `Amount` |
| `Amount Spec` | `Amount Spec 39C` | `Applicant` |
| `Application` | `Asset Type` | `Authority Amount` |
| `Authority Currency` | `Auto Batch` | `Auto Batch Reference` |
| `Auto Expiry` | `Auto Ext Expiry Date` | `Available Amount` |
| `Available With` | `Available With (and C Available With)` | `Available With Available By` |
| `BL Type` | `Back-to- Back` | `Back-to-Back LC` |
| `Backward Delivery` | `Bank To Bank Info` | `Bank to Customer info` |
| `Batch Reference` | `Batching/Rebatching` | `Ben Address` |
| `Ben Post Addr Line` | `Bene Bank Id / Bene Bank` | `Bene Bnk Id / Bene Bnk Name` |
| `Bene Bnk.Id / Bene Bnk Name` | `Benef Cust 1` | `Beneficiary` |
| `Beneficiary Account No` | `Beneficiary Country Code` | `Beneficiary Customer` |
| `Beneficiary Name` | `Bill Paid UnderReserve Returned Unpaid` | `Bill Register` |
| `Bill Type` | `Borrower` | `Borrower Role` |
| `By Acceptance, By Def Payment` | `By Mixed Pymt Or By Negotiation` | `C Docs Present Instr` |
| `C Docs Present Instr 45C` | `C Transfer Cond` | `C Transfer Indicator` |
| `C Txn Details` | `C Txn Details 45L` | `C Undk Charges 71D` |
| `CHANGE.PRODUCT` | `CL Limit Link` | `CSN Amount` |
| `CSN Currency` | `CSN Rate` | `Cancellation Request` |
| `Cat Ira` | `Category` | `Category Code` |
| `Category code` | `Ccy` | `Charge Ccy Mkt` |
| `Charge Code` | `Charge Codes` | `Charge Currency` |
| `Charge Period` | `Charge Routine` | `Charge Settled From` |
| `Charge Status` | `Chg Discount Amt` | `Chg Maximum Amt` |
| `Chg Minimum Amt` | `Chg Premium Amt` | `Claim Credit Account` |
| `Claim Credit Date` | `Claim Debit Account` | `Claim Payment Method` |
| `Claim Wof Cat` | `Claim amount` | `Classification` |
| `Clauses Text` | `Clean Colln Type` | `Closing Date` |
| `Closure Days` | `Coll Extn Days` | `Collateral` |
| `Collections Due` | `Comm Discount Amt` | `Comm Maximum Amt` |
| `Comm Minimum Amt` | `Comm Premium Amt` | `Con Cus Link` |
| `Confirm Instr (Confirmation Instructions)` | `Confirmation Amount` | `Confirmation Date` |
| `Cont Limit Link` | `Contract Group` | `Contract Type` |
| `Counterparty` | `Counterparty Role` | `Country Code` |
| `Credit Acct` | `Credit Prov Acc` | `Csn Acct Roundg Rule` |
| `Csn Ccy` | `Csn Pay Txn Code` | `Csn Perc` |
| `Csn Period` | `Csn Rec Txn Code` | `Currency` |
| `Currency Market` | `Currency Principal Amount` | `Current Accrual` |
| `Cust By Order` | `Customer` | `Customer Float` |
| `Customer Id` | `Customer Link` | `Days Post Mat` |
| `Days Post Maturity` | `Days to settle Invocation` | `Deal Sub Type` |
| `Deal Subtypes` | `Debit Prov Acc` | `Decision` |
| `Default Grace` | `Default Internal Accounts` | `Default Retention` |
| `Del With No Discrep` | `Delink Invoice` | `Demand Indicator` |
| `Demand Type` | `Description` | `Details of Guarantee` |
| `Dis Retain Code` | `Disbursement Method` | `Disc Cat Code` |
| `Disc Tran Code Cr` | `Disc Tran Code Dr` | `Discp Status` |
| `Discrep Status` | `Discrepancies.1` | `Discrepancy` |
| `Discrepancy Status` | `Discrepancy Type` | `Disp Of Docs` |
| `Disp Of Docs 77B` | `Disp Of Reimb Claim` | `Disposal of Docs` |
| `Doc Amount` | `Doc Back Val Days` | `Docs` |
| `Docs Present` | `Docs Present Instr` | `Docs Present Instr 45C` |
| `Docs Received (Documents Received` | `Document Amount` | `Document Code` |
| `Document Code.1` | `Document Currency` | `Document Status` |
| `Document Type` | `Documentary Credit No` | `Documents Received` |
| `Documents Released under Trust` | `Documents Required` | `Drafts At` |
| `Draw Type` | `Drawee` | `Drawee Cust No Drawee` |
| `Drawee ID` | `Drawer` | `Drawer ID or Drawer Name & Address` |
| `Drawing Reference` | `Drawing Type` | `Drawings Type` |
| `Duplicate Check` | `Eb Class No` | `Eb Class Type` |
| `End Date` | `End Range.1.` | `End To End Reference` |
| `Event Status` | `Events Processing` | `Exch Prft Cat` |
| `Exch Tolerance` | `Exchange Rate` | `Expiry Date` |
| `Expiry Days` | `Expiry Mode` | `Expiry/Reversal Date` |
| `External Ref` | `Facility Reference` | `Failed Invoices` |
| `Fields` | `Final Auto Ext Expiry Date` | `Final Rejection of Documents (Imports)` |
| `Final Rejection of Documents(Exports)` | `Finance Amount` | `Finance Request` |
| `Financing Date` | `Financing Request` | `Form of Undertaking` |
| `Form of Undk` | `Grace Calc Basis` | `Grace Days` |
| `Group Id` | `IB Event Status` | `Ib Event Status` |
| `Ib Limit` | `Import Export` | `Import/Export` |
| `In Purp of Msg` | `Inc Dec Amount` | `Include Provision` |
| `Info` | `Info Liability` | `Initiation` |
| `Instruction Id Ref` | `Instructions from Intermediary Bank` | `Int Amort Freq` |
| `Int Log File` | `Int Rate Type` | `Interest Key` |
| `Interest Rate` | `Interest Rate (Fixed).1` | `Interest Spread` |
| `Intermed Bank Customer Name` | `Intermed Bank Postal Addr Type` | `Intermed Bic` |
| `Intermediary Bank` | `Internal Amendment Ref` | `Inv Status` |
| `Inv Amount` | `Inv Available Amount` | `Inv Bnk To Bnk` |
| `Inv Bnk To Bnk 72Z` | `Inv Drawing Reference` | `Inv Failure Reference` |
| `Inv Requested Amount` | `Inv Status` | `Invocation Amount` |
| `Invocation Status` | `Invoice Amount` | `Invoice Field` |
| `Invoice Number, Invoice Date` | `Invoice Reference` | `Is Payment Category` |
| `Issue Date` | `Issue Transfer Undertaking` | `Issue Transfer Undk` |
| `Issued Date` | `Issuing Bank id` | `Issuing Bk` |
| `Issuing Bk Name` | `Items Upd Appl` | `LC Currency` |
| `Last Present Date Last Present Place` | `Lc Amount` | `Lc Class Type` |
| `Lc Currency` | `Lc Type` | `Lc Types` |
| `Liability Pty` | `Limit Reference` | `Limit With Prov` |
| `Limit if available to Internet Customer` | `Linked Merchant Trade Reference` | `Liquidation Mode` |
| `Load Cat Code` | `Load Tran Code Cr` | `Load Tran Code Dr` |
| `Loan Maturity Date` | `Log Level` | `ML Limit Link` |
| `MT740 Add Claim Amt` | `MT740 Other Chrgs` | `MT740Sender Info` |
| `MT742 Chrgs Deducted` | `MT742 Sender Info` | `MT744 Reimb Bk Chrgs` |
| `MT744 Sender Info` | `MT752 Advice Date` | `MT752 Narrative` |
| `MT752 Sender Info` | `MT752 Advice Date` | `MT752 Chgs Deducted` |
| `MT752 Further Identification` | `MT752 Mt752 Chgs Deducted` | `MT752 Narrative` |
| `MT752 Sender Info` | `MT754 Narrative` | `MT754 Sender Info` |
| `MT754Narrative` | `MT756 Narrative` | `MT756 Sender Info` |
| `MT756Narrative` | `MT759 Form Of Undk` | `MT759 Function` |
| `MT759 Narrative` | `MT759 Rel Ref` | `MT767 Advice Expiry Date` |
| `MT767 Narrative` | `MT767 Sender Info` | `MT785 File Identification` |
| `MT785 Advice Expiry Date` | `MT785 Advice Expiry Date` | `MT785 Sender Info` |
| `Margin Release Acct` | `Master Gtee Ref` | `Master Gtee Ref field` |
| `Maturity Usance` | `Max Int Rate` | `Md Class Type` |
| `Memo Limit Link` | `Merchant Trade` | `Message/Response to Bank*` |
| `Min Comm Tenure` | `Min.Amount` | `Minimum Interest Rate` |
| `Minimum Period` | `Mixed Payment Detail` | `Mt732 Sender Info` |
| `Mt740 Account No` | `Mt740 Applicable Rule` | `Mt750 Sender Info` |
| `Mt750 Sender Info 72Z` | `Mt752 Sender Info` | `Mt752 Sender Info 72Z` |
| `Mt754 Sender Info` | `Mt754 Sender Info 72Z` | `Mt756 Narrative` |
| `Mt756 Sender Info` | `Mt756 Sender Info 72Z` | `Mt759 Form Of Undk` |
| `Mt759 Function (23h)` | `Mt765 Addl Amount Info` | `Mt765 Addl Amount Info 78` |
| `Mt765 Send Recv Info` | `Mt765 Send Recv Info 72Z` | `Mt767 C Undk Term Cond` |
| `Mt767 C Undk Term Cond 77L` | `Mt767 Sender Info` | `Mt767 Sender Info 72Z` |
| `Mt767 Undk Term Cond` | `Mt767 Undk Term Cond 77U` | `Mt768 Sender Info` |
| `Mt768 Sender Info 72Z` | `Mt769 Chg Details` | `Mt769 Chg Details 71B` |
| `Mt769 Sender Info` | `Mt769 Sender Info 72Z` | `Mt785 Advice Expiry Date` |
| `Mt785 Sender Info` | `Mt785 Sender Info 72Z` | `Mt786 Send Info` |
| `Mt786 Send Recv Info 72Z` | `Mt787 Sender Info` | `Mt787 Sender Info 72Z` |
| `Narrative` | `Neg Def Payment Detail` | `Negotiate/Discount Sight Bill (Export)` |
| `Negotiating Bk Negotiating Bk Name` | `Net Amount` | `New Add Claim Amount` |
| `New Bill Type` | `New Cat Ira` | `New Category` |
| `New Current` | `New Doc Amt` | `New Maturity Date` |
| `No of Invoices` | `Operation` | `Operation Type` |
| `Ordering Cust Name` | `Ordering Post Address Type` | `Original Reference` |
| `Our Corrs Bnk` | `Overall Max Amt` | `Overall Min Amt` |
| `Part Csn Acc` | `Part Settlement` | `Part Shipments` |
| `Participant’s Commission` | `Party` | `Pay Subdivision` |
| `Pay Trans Cr` | `Pay Trans Dr` | `Pay Under Reserve/Approval/Collection` |
| `Pay type` | `Payment Amount` | `Payment Currency` |
| `Payment Date` | `Payment Due Date` | `Payment Order` |
| `Payment Order Categ` | `Payment Order Product` | `Payment Order product` |
| `Payment Type` | `Payment Types` | `Payment of SightBill Paid Under Reserve` |
| `Payment types` | `Percentage Cr Tolerance` | `Percentage Tolerance` |
| `Po Product` | `Po Wash Categ` | `Poa Wash Categ` |
| `Pre Advise Days` | `Present Comp Dets` | `Present Comp Dets 77` |
| `Presentation Amount` | `Presentation Amount mandatory` | `Presentation Date` |
| `Presentation Date, Presentation Amount, Presentor Ref, Docs Present` | `Presentation Date, Presentor Ref` | `Presentation For Claim` |
| `Presentation Status, Discp Status` | `Presentation Status, Discp Status and Advised Status` | `Presentation date` |
| `Presentation date, Presentation reference, Docs received, Presentation amount` | `Presentor ID` | `Presentor Name.1` |
| `Presentor Ref` | `Presentor Ref Or` | `Presentor Ref Or Alternate Id Or` |
| `Presentor Ref Or Alternate Id Or` | `Presentor Reference` | `Previous Month` |
| `Previous Year` | `Principal Amount` | `Principal Amount.` |
| `Principal Amt` | `Prior Days` | `Pro Category` |
| `Process At Sod` | `Process at SOD` | `Product` |
| `Prov Calc Base` | `Prov Category` | `Prov Netting` |
| `Prov Percent` | `Provis Acct` | `Provision` |
| `Provision %` | `Provision Cr` | `Provision Dr` |
| `Provision Rate` | `Provision Release Date` | `Purge Days` |
| `Quotation Status` | `Rate Change` | `Re Presentation` |
| `Reason For Refusal` | `Reason For Refusal 77J` | `Reason For Refuse` |
| `Reason Non Pmt` | `Reason for Refuse` | `Recalculate Amort` |
| `Received` | `Received Bk` | `Receiving Bank ID` |
| `Record Type` | `Recourse Party` | `Recourse Type` |
| `Recv Corrs .Bnk` | `Recv Corrs Bnk` | `Reduce LC Liab` |
| `Reduce Lc Liab` | `Reference` | `Reference 1` |
| `Reference 4` | `Reference 6` | `Reference 6, 34a Tot Amount, Reason Non Pmt` |
| `Reference 7` | `Reference.1` | `Referenec 1` |
| `Refund Category` | `Reimb Chrg Party` | `Reimb Trans Cr` |
| `Reimburse Days` | `Reject Documents under Export LC` | `Remarks` |
| `Remittance Information` | `Remitting Bank ID or Remitting Bank Name and Drawee ID (Our Customer)` | `Remitting Bank Ref` |
| `Req Conf Party (Requested Confirm Bank)` | `Request Amount` | `Requested Amount` |
| `Required Credit Value Date` | `Response to Discrepancies` | `Retention Margin` |
| `Revocable` | `Revol Advice Days` | `Risk Party` |
| `Role` | `Role Required` | `Round Rule` |
| `Rounding Rule` | `Rounding Type` | `SELLER.REFERENCE` |
| `Send Message?.1` | `Sender Info` | `Sender Info 72Z` |
| `Sender to Receiver Information` | `Settle Invoice` | `Settlement Terms` |
| `Short Description` | `Start Date` | `Start Range.1` |
| `Status` | `Status Date` | `Sub Cat End` |
| `Sub Cat Starting` | `Switch Limit` | `Synd Chg Code` |
| `Syndicate Charge` | `TF Drawing Ref` | `Take Margin?` |
| `Take/Reduce Margin` | `Takeover Process` | `Tenor.1` |
| `Third Party Cust No` | `Third Party Cust No / Third Party Cust` | `Third Party Cust No.` |
| `Third Party Cust.No (Reimbursement Bank)` | `Third Party Cust.No / Third Party Cust` | `Third Party Custno` |
| `Third Party Custno (Reimbursing Bank):` | `Total Available Amount` | `Tr Inv Code Cr` |
| `Tr Inv Code Dr` | `Tr Prov Code Cr` | `Tr Prov Code Dr` |
| `Trace Date` | `Trace Date Req` | `Tracer Date` |
| `Tracer stat` | `Trans Ref` | `Transaction Ref` |
| `Transaction Reference` | `Transaction Type` | `Transfer Cond` |
| `Transfer Cond field` | `Transfer Indicator` | `Transfer Undertaking Issued` |
| `Transfer Undk` | `Transfer Undk (Transferable Undertaking) and CTransfer Undk (Transfer Indicator):` | `Txn Details` |
| `Txn Details 45L` | `Unbatch` | `Uncollected Catrg` |
| `Uncollected Tr Cr` | `Unconfirmed Limit` | `Undk Charges` |
| `Undk Charges71D` | `Update Limit` | `Upload Reference` |
| `Upload Type` | `Value Date` | `Value From` |
| `Value To` | `Waive Charge (Y/N)` | `Write Off Pl` |
| `Write Off Tr Cr` | `payment method` |  |


---


## Appendix B: Consolidated Field Reference


This appendix consolidates all field description tables from across the documentation, grouped by sub-module. This provides a single reference for all field definitions.


### Trade_Banking - FF (FF)


**Misc**

| Table Name | Short Name | Description |
|---|---|---|
| BL.PARAMETER | BP | Company level parameter |
| BL.TYPE | BT | Bill type definitions |
| BL.TXN.TYPE.CONDITION | BTTC | Bill types and transactions |
| APPL.GEN.CONDITION | AGC | Bill contract group definition |
| BL.GROUP.CONDITION | BGC | Defining customer or group conditions |

**Misc**

| Field | Description |
|---|---|
| Int Amort Freq | Determines the frequency for interest amortisation when a bill is discounted or purchased. Indicates he start period for amortisation. Accepts values, such as Daily, Monthly or Weekly. Updates dynamically when the Close of Business (COB) process is run in the system. |
| Days Post Maturity | Defines the number of days post maturity of the contract after which the records are moved to the history file. |
| Max Int Rate | The value mentioned in this field is used to check if the calculated effective rate of interest is within the permissible limits. The maximum interest rate should not exceed the rate specified in this field. When the effective rate comes below the rate mentioned in this field, an override message is generated. This is an optional field. |
| Minimum Interest Rate | The values specified in this field is used to check if the calculated effective rate of interest is within the the permissible limits. The minimum interest rate should not go below the rate specified in this field. When the effective rate goes below the rate mentioned in this field, an override message is generated. |
| Grace Days | Determines the number of days within which a bank’s customer has to settle a bill repayment. At the end of this period, a penalty is charged based on the outstanding debit balance on the bill account. |

**Misc**

| BL.TYPE | Description |
|---|---|
| 1 | Discounted bill with recourse |
| 2 | Discounted bill without recourse |
| 3 | Collection bills |
| 8 | Factoring transaction with recourse |
| 9 | Factoring transaction non-recourse |

**Misc**

| Field | Description |
|---|---|
| Grace Days | Determines the number for calculation of grace days. For example, 2C – 2 calendar days and 2W – 2 working days. This is an optional field. |
| Currency | Indicates the currency in which the charges are defined. The other associated fields are Interest Key , Interest Spread and Interest Rate . |
| Interest Rate | Determines the interest rate that is used at the transaction processing level. This is an optional field associated with Currency , Interest Key and Interest Spread . |
| Max Int Rate | Checks if the calculated effective rate of interest is within the permissible limits. When the interest rate is defined, the maximum interest rate should not breach the rate specified in this field. An override message is generated when the effective rate is breached. This is an optional field. |
| Minimum Interest Rate | Checks if the calculated effective rate of interest is within the permissible limits. When the interest rate is defined, the minimum interest rate should not breach the rate specified in this field. An override message is generated when the effective rate is breached. |

**Misc**

| Field | Description |
|---|---|
| Chg Maximum Amt | Defines the maximum amount charged for the applicable charge type. |
| Chg Minimum Amt | Defines the minimum amount charged for the applicable charge type. |
| Chg Discount Amt | Specifies the amount deducted from the charge amount calculated. |
| Chg Premium Amt | Specifies the amount added to the charge amount calculated. |

**Misc**

| Table Name | Description |
|---|---|
| BILL.PARAMETER | This is a module level parameter file for bills. It is set before entering any bills contract along with the other parameter files. The disbursement, repayment and amortisation transaction code along with the interest rate caps, Profit and loss category for IRA Interest Received in Advance (IRA) are defined. The user can amend these pre-defined and fixed files. |
| BILL.TXN.TYPE.CONDITION | This parameter table defines the defaulting values for different combination of bill type and bill operation. ID of the table is DISCOUNT, COLLATERAL and COLLECTION, which are the supported bill operations. |
| APPLICATION.CONDITION ; | Contract groups are defined in this application based on category (product) code. This grouping is used to set default charge, commission and interest using the BILL.GROUP.CONDITION . The record ID to this table is BL.BILL to define bill groups. |
| BILL.GROUP.CONDITION | This parameter table is used to modify or override the values defaulted from a BL.TXN.TYPE.CONDITION record. Default charge, commission and interest can be defined for an individual customer or a group defined in APPL.GEN.CONDITION . |
| BILL.TYPE | Parameter settings for various types of bills (such as, discounted, collection), which are defaulted while entering a bill register record. It defines the contract category for various bill types and determines the liability customer in case of dishonour of a bill for each defined bill type. |
| BILL.STATUS | This application defines the status on the movement of bills. This status is given at bill register or bill batch level. |
| EB.DUPLICATE.TYPE | This application determines the duplicate records created in BL.REGISTER application. The system generates an override when the fields defined in the EB.DUPLICATE.TYPE and BL.REGISTER are same. |
| FILE.UPLOAD.TYPE | File upload type application allows the user to pre configure the upload directory, application and version details to process the header or item record in the uploaded file. This application displays all the records with value BILL.REGISTER in the Items Upd Appl field. |
| PRODUCT.CONDITIONS | BL.BATCH.CONDITIONS table defines the conditions for updating the product type in the BL registers based on the default conditions or customer specific conditions. Record ID format is . |
| CHANGE.PRODUCT.CONDITIONS | BL.BATCH.CONDITIONS table defines the conditions for updating the product type in the BL registers based on the default conditions or customer specific conditions. Record ID format is . |
| BATCH.CONDITIONS | This application defines the soft conditions for determining product types, batching and change product conditions for the bulk upload of invoices. |
| BUYER.SELLER. LIMIT | This application records the buyer-seller limit for information purpose. This holds buyer's maximum exposure for which the record is setup. |

**Misc**

| Product Name | Features |
|---|---|
| Bills for collection | Collection bills that can neither be discounted (purchased) nor taken as collateral. The invoice or bill of exchange amount is credited to a customer’s account only after the credit is made to Nostro account. |
| Bills for discounting | Collection bill that is discounted (purchased) by the bank for value and the invoice or bill of exchange amount is credited to the customer even before it is realised This loan is extended to the customer (drawee) The loan is settled when the bill is realized or returned without payment |
| Bills for collateral | Bill collateral product is a trade bill that is taken as a collateral for establishing an account limit for lending. |
| Creation of bills contract | Lodging a bill in transact system Bill contract involves 3 steps |
| Manual upload and batching | Manual upload and batching provides the users with the options to register, batch and rebatch the receivables with authorisation. Creation of BILL.REGISTER Creation of BL.BATCH Creation of BL.BILL |
| Automatic upload and batching | Automatic upload and batching provides the users with the options to register, batch and rebatch the receivables with zero authorisation. |
| Disbursement and settlement | Disbursement and settlement provides the users with the options to input, amend, reverse and delete the disbursed and settled records. |


### Trade_Banking - LC (LC)


**Amendment**

| Tag | Field Name |
|---|---|
| 44A | Place of Taking in Charge/Dispatch from .../Place of Receipt |
| 44E | Port of Loading/Airport of Departure |
| 44F | Port of Discharge/Airport of Destination |
| 44B | Place of Final Destination/For Transportation to.../Place of Delivery |

**Issuance or Register of a LC**

| Tag | SWIFT Field Name |
|---|---|
| 44A | Place of Taking in Charge/Dispatch from .../Place of Receipt |
| 44E | Port of Loading/Airport of Departure |
| 44F | Port of Discharge/Airport of Destination |
| 44B | Place of Final Destination/For Transportation to.../Place of Delivery |

**Misc**

| Field | Description |
|---|---|
| Reimburse Days | Sends reimbursement message in case of usance drawing before maturity. It is also used to decide when to send a MT 742 and MT754 SWIFT messages. |
| Revol Advice Days | Sends a revolution advice before the next revolution. |
| Maturity Usance | Reports imminent maturity of usance drawings. |
| Collections Due | Reports imminent due date of collections. |

**Misc**

| Code | Description of Use |
|---|---|
| P | Pre-advises a LC. This function accepts a reduced amount of information regarding the LC and when authorised, generates appropriate advices for despatch to the various patties in the transaction. |
| O | Opens a new LC or documentary collection. Converts a pre-advised LC into a live LC. At this point the credit limits are checked and utilised, contingent accounting entries are raised and initial charges may be taken. |
| A | Amends an existing LC or documentary collection. Allows the details to be modified. When requested, the system automatically generates amendment advices to be despatched to the parties to the transaction. |
| C | Takes direct charges. This code applies a direct charge to the LC or documentary collection. Charge input is performed on this record but the charges are immediately transferred to the LC.ACCOUNT.BALANCES file where they can be viewed and, in a limited way, amended. |
| T | Traces a documentary collection. This function applies only to documentary collections. Generates tracer messages such as a SWIFT MT420. |

**Misc**

| Table Name | Description |
|---|---|
| LC.TXN.TYPE.CONDITION | This parameter file is used to setup the default charges for all LC or documentary collections and drawing types. The system has a set of default charges setup in this file for each LC transaction entered. The defaulting mechanism works by defining a record in this file, corresponding to each type of LC ( LC.TYPE ), together with the operations that is performed. |
| LC.GROUP.CONDITION | Defines special rules for a group of customers or specific customers for, (charges, commissions, exchange rate spread and payment value dating). When the definition is for a group of customers, the LC.GEN.CONDITION record must exist before any associated group condition is specified. |
| LC.TYPES | The users can setup customised LC and documentary collections. Defines LC types allowed in the system with their narrative descriptions. Verifies the credit types and sets the default Category Code , during input and validation of LC. It is used for the maintenance of LC statistics in the form of a counter, which is updated when LC is pre-advised, opened, expired and closed. |
| LC.ADVICE.TEXT | Holds static narrative information that helps to map the construction of LC advices or documents that are generated by LC transactions, within the Temenos Transact delivery application. Creates document code and text message related to the documents required in LC. Additionally, provision is available to default the required documents based on customer ID-Inco Terms, and mode of shipment. The record ID is as follows: Customer ID-Inco Terms-Mode of Shipment Inco Terms-Mode of Shipment Customer ID Free Text When opening an import LC in Temenos Transact , the user can select document code against Documents Required field (Swift field 46-A) instead of typing text message. When the user wants to edit the text message, it can be done at contract level. |
| LC.CLAUSES | Holds static narrative information that helps in mapping the construction of LC advices or documents that are generated by LC transactions, within the Temenos Transact delivery application. By creating a record in this file, the user can select the record instead of typing additional conditions (Swift field 47-A) while opening LC. LC.CLAUSES details can also be defaulted at the transaction level based on the applicant's customer ID, inco terms and mode of shipment. The preferential order of the record ID is: Customer ID-Inco Terms-Mode of Shipment Inco Terms-Mode of Shipment Customer ID Free Text |
| DR.DISCREPANT.TYPE | Holds records of discrepant type, EB.ACTIVITY , tickler days, risk party and reduce liability. When discrepant LC export document is payable to beneficiary under payment under reserve, the system updates records based on the setup made in this application. The related activity codes triggers production of advices and swift messages. |
| LC.GEN.CONDITION | Identifies a specific group of customers who are cross-related to the LC.GROUP.CONDITION table to define LC conditions applicable to that group. The key to this table is also the key to the associated LC.GROUP.CONDITION record. LC groups are determined based on customer details such as, sector and target. The criteria used and their priority are specified in the Condition Priority file, in the record whose ID is LETTER.OF.CREDIT . |
| LC.PARAMETERS | Contains data and parameter fields required for LC processing, which are not available in any other file, (there is only one record). Holds static data that is standard for LC and drawings processing. It is used to: Input defaults (closure days, currency, market, position type) Entries generation (transaction codes and account numbers) End of day processing (pre-advise days, accrual or amortisation cycle) |

**Misc**

| Product Name | Features |
|---|---|
| Issuance of import LCs | The LC module within model bank ( Temenos Transact ) is used to record the contingent deals that are required to record LC type transactions in the banks’ books. A bank user opens a credit record in Temenos Transact based on the application received from the customer. The initiation to issue a LC can be directly from the corporate client through Corporate Internet Banking channel. The following types of import LCs are issued: Sight payment Usance Negotiation. Mixed payment Stand by The following types of export LCs are advised to the beneficiary: Sight payment Usance Negotiation Mixed payment. Stand by Transfer |
| Maintenance of import LCs | Any changes or cancellation of LC, which is communicated to third parties like advising bank or beneficiary through the generation of the message. Amendment can be either internal or external. Collection and reversal of provision can be done through maintenance of LC’s |
| Drawings under import LCs | Drawings under Import LCs has a flexible payment and reimbursement mechanism whereby funds are collected or paid through a number of intermediaries, and even be paid to parties not involved in the LC. Temenos Transact automatically produces the payment instructions necessary for these facilities. |
| Discounting of usance bills under LC | Issuing bank makes the payment to the beneficiary or negotiating bank before the accepted maturity of the said drawing or bill and then recovers the payment amount from the applicant on the accepted maturity date. |
| Collections | The LC module within model bank ( Temenos Transact ) also facilitate documentary collections (outward and inward). The following types of collections are processed: Documents against payment Documents against acceptance Clean collection |
| Open Account Trade | The LC module within model bank (Temenos Transact) also facilitates Open Account Trade (Import and Outward). The following types of contracts are processed: Lodge import trade documents Lodge export trade documents |
| Trade Evidence for Advance Payments | The LC module within model bank (Temenos Transact) also facilitates registering of trade evidence against the advance payments. |

**Pre advice of a LC**

| Tag | SWIFT Tag Name |
|---|---|
| 44A | Place of Taking in Charge/Dispatch from.../Place of Receipt |
| 44B | Place of Final Destination/For Transportation to.../Place of Delivery |
| 44E | Port of Loading/Airport of Departure |
| 44F | Port of Discharge/Airport of Destination |

**Tickler and Tracers**

| Field | Description |
|---|---|
| Trace Date Req | Tracer mechanism is mandatory for each discrepant type defined in DR.DISCREPANT.TYPE . When set to Yes, Trace Date field in DRAWINGS becomes mandatory and vice-versa. This field controls the Trace Date field in a DRAWINGS which uses this discrepant type. |


### Trade_Banking - MD (MD)


**Amendment of Issued or Registered Guarantees**

| Status | Tag | Field Name | Content/Options |
|---|---|---|---|
| O | 23 | Advising Bank Reference | 16x |

**Issue Register Guarantee**

| Status | Tag | Field Name | Content/Options |
|---|---|---|---|
| O | 39D | Additional Amount Information | 12*65z |
| O | 44H | Governing Law and/or Place of Jurisdiction | 2!a[/65x] |

**Issue Register Guarantee**

| Status | Tag | Field Name | Content/Options |
|---|---|---|---|
| O | 39F | Supplementary Information About Amount | 12*65z |
| O | 44J | Governing Law/Jurisdiction | 2!a[/35x] [/65x] |

**Issue Register Guarantee**

| Status | Tag | Field Name | Content/Options |
|---|---|---|---|
| O | 57a | Advise Through' Bank | A or D |

**Misc**

| Asset Type | Description |
|---|---|
| CONTCR | Contingent liabilities |
| FWDCONTCR | Forward starting – Contingent liabilities |
| CONTBD | Contingent assets |
| FWDCONTCB | Forward starting – Contingent assets |
| MEMOCR | Contingent liabilities (memo basis) |
| FWDMEMOCR | Forward starting – Contingent liabilities (memo basis) |
| MEMODB | Contingent assets (memo basis) |
| FWDMEMODB | Forward starting – Contingent assets (memo basis) |

**Misc**

| Type | Description |
|---|---|
| CL | Contingent Liability |
| CA | Contingent Asset |
| ML | Memorandum Liability |
| MA | Memorandum Asset |

**Misc**

| Fields in MD.PARAMETER | Values in the Field |
|---|---|
| Poa Wash Categ | Valid PO wash account category code as defined in the CATEGORY table |
| Payment Order Categ | Valid record ID of the table PAYMENT.ORDER.PRODUCT |

**Misc**

| Fields in MD.CLAUSES | Fields in MD.DEAL | Swift Tag |
|---|---|---|
| Sender Info 72Z | Sender Info | 72Z |
| Undk Charges71D | Undk Charges | 71D |
| Docs Present Instr 45C | Docs Present Instr | 45C |
| Txn Details 45L | Txn Details | 45L |
| C Docs Present Instr 45C | C Docs Present Instr | 45C |
| C Txn Details 45L | C Transfer Cond | 45L |
| C Undk Charges 71D | C Txn Details | 71D |
| Mt767 Sender Info 72Z | Mt767 Sender Info | 72Z |
| Mt767 Undk Term Cond 77U | Mt767 Undk Term Cond | 77U |
| Mt767 C Undk Term Cond 77L | Mt767 C Undk Term Cond | 77L |
| Mt768 Sender Info 72Z | Mt768 Sender Info | 72Z |
| Mt765 Addl Amount Info 78 | Mt765 Addl Amount Info | 78 |
| Present Comp Dets 77 | Present Comp Dets | 77 |
| Mt765 Send Recv Info 72Z | Mt765 Send Recv Info | 72Z |
| Reason For Refusal 77J | Reason For Refusal | 77J |
| Disp Of Docs 77B | Disp Of Docs | 77B |
| Mt786 Send Recv Info 72Z | Mt786 Send Info | 72Z |
| Inv Bnk To Bnk 72Z | Inv Bnk To Bnk | 72Z |
| Amount Spec 39C | Amount Spec | 39C |
| Mt769 Chg Details 71B | Mt769 Chg Details | 71B |
| Mt769 Sender Info 72Z | Mt769 Sender Info | 72Z |
| Mt787 Sender Info 72Z | Mt787 Sender Info | 72Z |
| Mt785 Sender Info 72Z | Mt785 Sender Info | 72Z |
| Mt750 Sender Info 72Z | Mt750 Sender Info | 72Z |
| Mt754 Sender Info 72Z | Mt754 Sender Info | 72Z |
| Mt752 Sender Info 72Z | Mt752 Sender Info | 72Z |
| Mt756 Sender Info 72Z | Mt756 Sender Info | 72Z |
| Mt756 Sender Info 72Z | Mt756 Narrative | 72Z |

**Non Extension Guarantee**

| Optional/ Mandatory | Field Tag | Field Name | Field Mapping | Description |
|---|---|---|---|---|
| M | 20 | Transaction Reference No | Alternate ID | Specifies the unique and unambiguous identifier assigned by the issuer of the undertaking. The field specification is 16x. When an advising bank relays the message to Advise Thru Bank, the Reference 1 field is mapped. |
| O | 21 | Related Reference | Reference 1 | Indicates the Reference 1 field. This field specifies the reference which has been assigned by the beneficiary of the undertaking or counter-undertaking. When an advising bank relays the message to Advise Thru Bank, the Reference 4 field is mapped. |
| M | 52A | Issuing Bank ID | Issuing Bk | Specifies the party that issued the undertaking. This is a mandatory field in MT785. The format is: - If the input in the field is a BIC, then the tag 52A is specified. - If the input in the field is ‘Name and address’ of the issuer, then the Tag 52D displays in the SWIFT message |
| M | 52D | Issuing Bank Address | Issuing Bk Name |  |
| M | 31C | Value Date | Value Date | Specifies the date on which the undertaking was issued. The field specification is 6!n |
| O | 59A | Beneficiary | Benef Cust 1 | Indicates the beneficiary customer 1. |
| O | 56A | Advising Bank ID | Advising Bk | Indicates the advising bank. |
| O | 56D | Advising Bank Address | Advising Bk Name | Indicates the advising bank name. |
| O | 57A | Advise Through Bank ID | Advice Thru Bk | Indicates the advising thru bank. |
| O | 57D | Advise Through Bank Add | Advice Thru Bk Name | Indicates the advising thru bank name. |
| O | 31E | Final Date of Expiry | MT785 Advice Expiry Date | Outward For outward message, when MT785 Advice Expiry Date is updated in MD.DEAL , then the same date is updated/replaced in Advice Expiry Date upon authorization of undertaking contract. After undertaking contract is authorised, the date is updated in both the fields ( MT785 Advice Expiry Date and Final Auto Ext Expiry Date ). When the authoriser rejects the changes, the new changes are not updated in the undertaking contract. The process has to be redone. The value present in MT785 Advice Expiry Date is mapped to Tag 31E field. Inward When the value is inputted in for MT785 Advice Expiry Date field, it is defaulted to Final Auto Ext Expiry Date if the Mt785 Advice Expiry Date field is not inputted and does not have any value. If the Final Auto Ext Expiry Date is not entered, the value in the MT785 Advice Expiry Date field is defaulted to Advice Expiry Date and is treated as the expiry date of the guarantee contract. The above defaulting happens for the recently received inward MT785 message. |
| O | 72Z | Sender to Receiver Info | MT785 Sender Info | To be mapped to Tag 72Z. The reason for non-extension can be entered by the issuing bank that is to be conveyed to the advising bank. For the incoming MT785 message, Tag 72Z must be mapped to the Received Bk Info field. |
| O | 23X | File Identification | MT785 File Identification | This field identifies the type of delivery channel and associated file name or reference.It must Contain any one of the following codes COUR EMAL FACT FAXT HOST MAIL OTHR |

**Presentation under SBLC**

| Field | Description |
|---|---|
| Docs Received | Specifies if the original documents are received by the bank. This is a mandatory field to trigger presentation of documents. Input in this field makes the multi-value set of fields, namely Presentation Date, Presentor Ref and Presentation Amount mandatory . The allowed values are: YES or NO. |
| Presentor Ref | Captures the reference number of the presentor when documents are received by the bank. The system maps the user input in this field to Tag 21 of outward MT732 after Discrep Status for the documents is updated as Accept or Waived. It takes up to 16 characters of 'x' character set. This is a mandatory field as part of generation of MT732 and should not begin with two slashes '//'. |
| Presentation Date | Specifies the date of receipt of documents. Input in this field enables the associated multi-value set under presentation register and prompts the user to input presentation details. The user has to input this field to enable generation of outward MT732. The system maps this field to Tag 30 of outward MT732, after Discrep Status for the documents are updated as Accept or Waived. This is a mandatory field for both registering presentation of documents under Standby LC and subsequent generation of MT732. Presentation Amount and Presentor Ref become mandatory fields when this field has input. |
| Presentation Amount | Captures the amount of presentation. The system maps the input in this field to Tag 32B of MT732, when Discrep Status for the documents is updated as Accept or Waived. Presentation Amount cannot be greater than Principal Amount. |
| Remarks | Stores any specific details related to a document presented. This field is for internal use, but is mandatory when Re Presentation is input, wherein this field captures the changes to the documents after revised presentation. This field takes input up to 50 lines of 65 characters of 'z' character set. |
| Re Presentation | This field record is updated when the user provides revised Presentation Documents, after the applicant rejects the first set of documents. When the Presentor presents the revised set of documents for the same Presentation, the user can update the fields and modify the records under the same presentation. For example, it accepts input as YES or NO. After this field is updated, the Remarks field becomes a mandatory field. |
| Docs Present | Captures document-specific identification/type. For example, Invoices, Certificate of Origin and Certificate of Completion. |
| Presentation Status | Captures if documents are clean or discrepant. Based on the same, the system generates Acceptance or Rejection messages. |
| Discrep Status | Captures applicant's response to the discrepancies recorded in presentation or received from presenting bank, whether accepted or to be rejected. Generation of outward MT732 depends on input in this field ( MT732 content - Advice by Issuer to take up Acceptance/Payment against documents received with discrepancies). The allowed vales are ACCEPT, WAIVE or REJECT. |
| Advised Status | Captures the bank's response to the discrepancies recorded in presentation or received from the presenting bank, whether accepted or to be rejected. Generation of outward MT732 depends on input in this field (MT732 content - Advice by Issuer to take up Acceptance/Payment against documents received with discrepancies). The allowed values are: Advised to applicant Pending with beneficiary Presented through advising bank Presented through pay/issuing bank |

**Presentation under SBLC**

| Tag Status | Field Tag | SWIFT Tag | Inward Field Mapping | Outward Field Mapping |
|---|---|---|---|---|
| M | 20 | Sender's TRN | Reference 1 | Alternate Id Or @Id Or Reference.1 |
| M | 21 | Presenting Bank's Reference | Presentor Ref | Presentor Ref |
| M | 30 | Date of Advice | Presentation Date | Presentation Date |
| M | 32B | Amount of Utilisation | Presentation Amount | Presentation Amount |
| O | 72Z | Sender to Receiver Information | Mt732 Sender Info | Mt732 Sender Info |

**Presentation under SBLC**

| Tag Status | Field Tag | SWIFT Tag | Inward Field Mapping | Outward Field Mapping |
|---|---|---|---|---|
| M | 20 | Sender's Reference | Presentor Ref | Presentor Ref Or Alternate Id Or @ Id |
| M | 21 | Related Reference | Alternate ID @ID Or Reference 1 | Reference 1 |
| M | 32B | Principal Amount | Presentation Amount | Presentation Amount |
| O | 33B | Additional Amount | Add Claim Amount | Add Claim Amount |
| O | 71D | Charges to be Deducted | 750 Charges Deducted | 750 Charges Deducted |
| O | 73A | Charges to be Added | 750 Charges Added | 750 Charges Added |
| O | 34B | Total Amount to be Paid | 34b Tot Amount | 34b Tot Amount |
| O | 57A | Account With Bank | Acct With Bank | Acct With Bank |
| O | 72Z | Sender to Receiver Information | 750 Sender Info | 750 Sender Info |
| M | 77J | Discrepancies | Reason For Refuse | Reason For Refuse |

**Presentation under SBLC**

| Tag Status | Field Tag | SWIFT Tag | Inward Field Mapping | Outward Field Mapping |
|---|---|---|---|---|
| M | 20 | Documentary Credit Number | Reference 1 | Alternate Id Or @ Id Or Reference.1 |
| M | 21 | Presenting Bank's Reference | Presentor Ref Or Alternate Id Or @ ID | Presentor Ref |
| M | 23 | Further Identification | MT752 Further Identification | MT752 Further Identification |
| M | 30 | Date of Advice of Discrepancy or Mailing | MT752 Advice Date | MT752 Advice Date |
| O | 32B | Total Amount Advised | 34b Tot Amount | 34b Tot Amount |
| O | 71D | Charges Deducted | MT752 Chgs Deducted | MT752 Mt752 Chgs Deducted |
| O | 33A | Net Amount | Net Amount | Net Amount |
| O | 53A | Sender's Correspondent | Our Corrs Bnk | Our Corrs Bnk |
| O | 54A | Receiver's Correspondent | Recv Corrs .Bnk | Recv Corrs Bnk |
| O | 72Z | Sender to Receiver Information | MT752 Sender Info | MT752 Sender Info |
| O | 79Z | Narrative | MT752 Narrative | MT752 Narrative |

**Presentation under SBLC**

| Tag Status | Field Tag | SWIFT Tag | Inward Field Mapping | Outward Field Mapping |
|---|---|---|---|---|
| M | 20 | Sender's Reference | Presentor Ref | Presentor Ref Or Alternate Id Or @ Id |
| M | 21 | Related Reference | Alternate Id / @Id Or Reference 1 | Reference.1 |
| M | 32A | Principal Amount Paid/Accepted/Negotiated | Presentation Amount | Presentation Amount |
| O | 33B | Additional Amount | Add Claim Amount | Add Claim Amount |
| O | 71D | Charges to be Deducted | 754 Charges Deducted | 754 Charges Deducted |
| O | 73A | Charges to be Added | 754 Charges Added | 754 Charges Added |
| O | 34A | Total Amount Claimed | 34b Tot Amount | 34b Tot Amount |
| O | 53A | Reimbursing Bank | Third Party Cust No / Third Party Cust | Third Party Cust.No / Third Party Cust |
| O | 57A | Account With Bank | Acct With Bank | Acct With Bank |
| O | 58A | Beneficiary Bank | Bene Bnk.Id / Bene Bnk Name | Bene Bnk Id / Bene Bnk Name |
| O | 72Z | Sender to Receiver Information | MT754 Sender Info | MT754 Sender Info |
| O | 77 | Narrative | MT754Narrative | MT754 Narrative |

**Presentation under SBLC**

| Field Tag | SWIFT Tag | Tag Status | Inward Field Mapping | Outward Field Mapping |
|---|---|---|---|---|
| 20 | Documentary Credit Number | M | Reference 1 | AlternateId Or @ Id Or Reference.1 |
| 21 | Presenting Bank's Reference | M | Presentor Ref Or Alternate Id Or @ Id | Presentor Ref |
| 32B | Total Amount Claimed | M | 34b Amount | 34b Tot Amount |
| 33A | Amount Reimbursed or Paid | M | Net Amount | Net Amount |
| 53A | Sender's Correspondent | O | Our Corrs Bnk | Our Corrs Bnk |
| 54A | Receiver's Correspondent | O | Recv Corrs Bnk | Recv Corrs Bnk |
| 72Z | Sender to Receiver Information | O | MT756 Sender Info | MT756 Sender Info |
| 79Z | Narrative | O | MT756Narrative | MT756 Narrative |

**Register Claim under Guarantee**

| Status | Tag | Field Name | Content/Options |
|---|---|---|---|
| O | 31R | Requested New Date of Expiry of Local Undertaking | 6!n |

**Reimbursement Processing SBLC**

| Optional or Mandatory | Tag | SWIFT Tag | Content or Options | Field Mapping |
|---|---|---|---|---|
| M | 20 | Documentary Credit Number | 16x | Alternate Id |
| O | 25 | Account Identification | 35x | Mt740 Account No |
| M | 40F | Applicable Rules | 30x | Mt740 Applicable Rule |
| O | 31D | Date and Place of Expiry | 6!n29x | Last Present Date Last Present Place |
| O | 58a | Negotiating Bank | A or D | Negotiating Bk Negotiating Bk Name |
| O | 59 | Beneficiary | (/34x) 4•35x | Ben Address |
| M | 326 | Credit Amount | 31a15d | Currency Principal Amount |
| O | 39A | Percentage Credit Amount Tolerance | 2nt2n | Percentage Cr Tolerance |
| O | 39C | Additional Amounts Covered | 4*35x | MT740 Add Claim Amt |
| M | 41a | Available With ...By .. | A orD | Available With Available By |
| O | 42C | Drafts at.. | 3•35x | Drafts At |
| O | 42a | Drawee | A orD | Drawee Cust No Drawee |
| O | 42M | Mixed Payment Details | 4*35x | Mixed Payment Detail |
| O | 42P | Negotiation/Deferred Payment Details | 4*35x | Neg Def Payment Detail |
| O | 71A | Reimbursing Bank"s Charges | 31a | Reimb Chrg Party |
| O | 71D | Other Charges | 6*35z | MT740 Other Chrgs |
| O | 72Z | Sender to Receiver Information | 6*35? | MT740Sender Info |

**Reimbursement Processing SBLC**

| Tag Status | Field Tag | SWIFT Field Name | Length | Field Mapping |
|---|---|---|---|---|
| M | 20 | Documentary Credit Number | 16x | Reference 1 |
| O | 21 | Reimbursing Bank's Reference | 16x | Alternate Id Or @Id |
| M | 30 | Date of the Original Authorisation to Reimburse | 6!n | 740 Reimb Dtd |
| O | 31E | New Date of Expiry | 6!n | MT767 Advice Expiry Date |
| O | 32B | Increase of Documentary Credit Amount | 3!a15d | Inc Dec Amount |
| O | 33B | Decrease of Documentary Credit Amount | 3!a15d | Inc Dec Amount |
| O | 34B | New Documentary Credit Amount After Amendment | 3!a15d | New Doc Amt |
| O | 39A | Percentage Credit Amount Tolerance | 2n/2n | Percentage Tolerance |
| O | 39C | Additional Amounts Covered | 4*35x | New Add Claim Amount |
| O | 72Z | Sender to Receiver Information | 6*35z | MT767 Sender Info |
| O | 77 | Narrative | 20*35z | MT767 Narrative |

**Reimbursement Processing SBLC**

| Field Tag | SWIFT Field Name | Tag Status | Field Mapping |
|---|---|---|---|
| 20 | Claiming Bank's Reference | M | Alternate ID Or @ID |
| 21 | Documentary Credit Number | M | Referenec 1 |
| 31C | Date of Issue | O | Value Date |
| 52A | Issuing Bank | M | Issuing Bk |
| 32B | Principal Amount Claimed | M | Inv Amount |
| 33B | Additional Amount Claimed as Allowed for in Excess of Principal Amount | O | Add Claim Amount |
| 71D | Charges | O | MT742 Chrgs Deducted |
| 34A | Total Amount Claimed | M | 34a Tot Amount |
| 57A | Account With Bank | O | Acct With Bank / Acct With Bank Id |
| 58A | Beneficiary Bank | O | Bene Bank Id / Bene Bank |
| 72Z | Sender to Receiver Information | O | MT742 Sender Info |

**Reimbursement Processing SBLC**

| Optional/Mandatory | Field Tag | Field Name | Format | Field Mapping |
|---|---|---|---|---|
| M | 27 | Sequence of Total | 1!n/1!n | Auto Populated |
| M | 20 | Transaction Reference Number | 16x |  |
| O | 21 | Related Reference Number | 6x | MT759 Rel Ref |
| M | 22D | Form of Undertaking | 4!c | MT759 Form Of Undk |
| M | 23 | Undertaking Number | 16x |  |
| O | 52A | Issuer | A or D |  |
| M | 23H | Function of Message | 8!c | MT759 Function |
| M | 45D | Narrative | 150*65z | MT759 Narrative |
| O | 23X | File Identification | 4!c/65 |  |

**Reimbursement Processing SBLC**

| Tag Status | Field Tag | SWIFT Field Name | Length | Outward Mapping details |
|---|---|---|---|---|
| M | 20 | Sender's Reference | 16x | Alternate Id Or @ID |
| M | 21 | Claiming Bank's Reference | 16x | Reference 6 |
| M | 52A | Issuing Bank | A or D | Issuing Bk |
| M | 21A | Documentary Credit Number | 16x | Reference 1 |
| O | 31C | Date of Issue | 6!n | Value Date |
| M | 34A | Total Amount Claimed | A or B | 34a Tot Amount |
| M | 73R | Reason for Non-Payment | 4!c[/35x] | Reason Non Pmt |
| M | 73S | Disposal of Reimbursement Claim | 4!c[/35x] | Disp Of Reimb Claim |
| O | 71D | Reimbursing Bank's Charges | 6*35z | MT744 Reimb Bk Chrgs |
| O | 72Z | Sender to Receiver Information | 6*35z | MT744 Sender Info |

**TBML Check for Guarantee and SBLC**

| Method | Description |
|---|---|
| Overvaluation of Goods | Those involved in criminal activities may inflate the value of goods or services involved in trade transactions supported by guarantees. By overpricing the goods, they can create a discrepancy between the actual value of the goods and the reported transaction value, enabling them to launder illicit funds through legitimate trade channels. |
| Fictitious Transactions | TBML perpetrators may engage in creating fictitious trade transactions backed by guarantees. These transactions involve the issuance of guarantees for non-existent or misrepresented goods or services. The guarantee serves as a mechanism to legitimise the movement of illicit funds across borders, making it appear as if they originated from legitimate trade activities. |
| Phantom Shipments | Criminal organisations may exploit trade finance guarantees to facilitate phantom shipments, where goods are invoiced and guaranteed for shipment but are never actually delivered. This scheme allows criminals to create a paper trail of fictitious trade transactions, providing a facade of legitimacy for laundering illicit funds. |
| Round-Tripping | In certain cases, TBML involves round-tripping, where funds are moved through a series of transactions involving multiple jurisdictions and intermediaries to obscure their origin. Trade finance guarantees can be misused in round-tripping schemes to create the appearance of legitimate trade activities while effectively laundering illicit funds. |
| Misrepresentation of Goods | TBML perpetrators may misrepresent the nature or quality of goods involved in trade transactions supported by guarantees. By providing false or misleading information about the goods, they can manipulate the trade finance process to launder illicit funds without attracting suspicion. |
| Layering | TBML often involves layering, where funds are moved through multiple accounts or financial instruments to further obscure their origin. Trade finance guarantees can be used as part of the layering process to facilitate the movement of illicit funds through the international banking system. |


### Trade_Banking - SU (SU)


**Facility Agreement**

| Field | Description |
|---|---|
| Default Retention | Specifies the default retention margin for the facility agreement. |
| Default Grace | Specifies the default grace days for the facility agreement. Grace days are set to calendar days by default. If no Grace days are defined for a counterparty then default grace is considered. However, banks can change them to working days by appending ‘W’ to the number of days. Grace days can be defined as: 8W: 8 working days 8C: 8 calendar days 8: 8 calendar days This field is optional. |
| Grace Calc Basis | Allows the bank to determine how the maturity date is extended and charges are calculated for the grace days. The available options are: Maturity Date: Extends the maturity date of the loan. Charge: Calculates the charge for the grace days. This field becomes mandatory, when grace days are defined in arrangement rules. |
| Counterparty | Specifies the counterparty details in a facility agreement. It refers to customer table. This field is optional and becomes mandatory when currency, retention margin, or grace days are defined. |
| Currency | Specifies the currency details for retention and grace in a facility agreement. This field is optional and becomes mandatory when currency, retention margin, or grace days are defined. |
| Retention Margin | Specifies the retention details for the counterparty in a facility agreement. |
| Grace Days | Specifies the grace days details for the counterparty in a facility agreement. Grace days are set to calendar days by default. However, banks can change them to working days by appending ‘W’ to the number of days. Grace days can be defined as: 8W: 8 working days 8C: 8 calendar days 8: 8 calendar days This field is optional. |

**Finance Request**

| Field | Description |
|---|---|
| Action | This field contains the following predefined set of actions which can be executed on the funding request: BLANK - Allows the template to be committed without any action by simply validating the template. DISBURSE - Triggers the disbursement for the funding request. Upon triggering, the SCF drawings are created under the selected facility, and funds are disbursed to the borrower. This action is executed through a service. GET.QUOTE– Runs simulation on the batched invoices and fetches the final disbursement amount. RESUBMIT – Triggers the disbursement for the finance request, which are in the error queue. |
| Borrower | Specifies the customer for whom the finance is to be disbursed. |
| Borrower Role | Holds the role of the customer. |
| Counterparty | Specifies the counterparty reference. This field is mandatory only when an invoice reference is added to a funding request for a single invoice disbursement. When a batch reference is added, the counterparty details for disbursement are taken from the batch reference. The counterparty field is not allowed when a batch reference is updated. |
| Counterparty Role | Holds the role of the counterparty. |
| Facility Reference | Holds the facility reference under which the invoices will be funded. |
| Product | Holds the AA.PRODUCT reference. When the funding request is approved, the amount disbursed to the borrower is processed through an AA loan, and the loan is created for the product specified in this field. |
| Currency | Holds the currency in which fund will be disbursed. This value should match the currency defined in SU.INVOICE.BATCH when a batch reference is provided, else, it should match the invoice currency when an invoice reference is given. |
| Financing Date | Indicates the date on which the funds are disbursed to the borrower. It can be backdated, current-dated, or future-dated. |
| Invoice Reference | Specifies the invoice reference which corresponds to the SU.INVOICE.CAPTURE table. The status of the invoice entered must be ‘NEW’. Either a batch reference or an invoice reference is required. |
| Batch Reference | Holds the SU.INVOICE.BATCH reference, allowing the bank user to attach the batch reference for initiating disbursement. It is mandatory when an invoice reference is not given. The system must validate that the borrower reference in the batch matches the one specified in the funding request. |
| Quotation Status | Holds the status of the quotation. |
| Status | Holds the status of the finance request. |
| Recourse Type | Holds the type of the recourse associated with the facility arrangement. |
| Delink Invoice | Delinks the failed invoices from the Finance Request. This is a User Input Field. This field can be set as ‘Yes’ only when the Finance Request is in the ‘Completed with Error’ status. If it is set as ‘Yes’, the system only allows the ‘Resubmit’ action to be performed, which delinks the failed invoice from the Finance Request. This field is optional. |
| Drawing Reference | Holds the Arrangement reference for the invoices that are successfully created under a batch. This field is updated by the system with the Drawing Arrangement ID. |
| Failed Invoices | Holds the reference for the invoices for which drawing creation has failed. The failed invoices under the finance request will be in the Invoices ID*AAA reference format. This field is updated by the system. |
| Inv Drawing Reference | Holds the Arrangement reference for the invoice that is successfully created. This field is updated by the system with the Drawing Arrangement ID. |
| Inv Failure Reference | Holds the AA.ARRANGEMENT.ACTIVITY reference when the drawings creation has failed for the given invoice reference. |
| Disbursement Method | Specifies the disbursement method. Allowed values are: Full : Enables the user to disburse the finance request to the full available amount for a newly initiated finance request and the existing partially financed finance requests. Partial : Allows the user to input a specific amount for a finance request. This field is optional. If no input is given, the system considers the value 'Full' by default. |
| Inv Available Amount | Specifies the fundable amount for an invoice attached to the finance request. This is calculated based on the face value of the invoice, deducting the retention margin configured at the facility attached in the finance request. |
| Inv Requested Amount | Specifies the amount requested by the user for an invoice. If no specific amount is requested, Inv Available Amount is considered as the Inv Requested Amount . |
| Total Available Amount | Specifies the total fundable amount for a finance request. For multiple batches, it is calculated based on the batch amount, deducting the retention margin configured at the facility. For multiple invoices, it is the sum of all the Inv Available Amount . |
| Requested Amount | Specifies the amount requested by the user for batches. If no specific amount is requested, the Total Available Amount is considered as the requested amount. This field becomes mandatory when Disbursement Method is set as ‘Partial’ for the finance requests with batches. |

**Invoice Batching**

| Field | Description |
|---|---|
| Description | Holds the description for the record. |
| Invoice Field | Holds the field reference from the SU.INVOICE.CAPTURE application. |
| Decision | Holds the decision parameters like EQ, LT, GT, LE, GE, RG, and so on. |
| Value From | Holds the criterion value for the Invoice Capture field. |
| Value To | Holds the criterion end value for the Invoice Capture field. |
| Available Amount | Specifies the available amount for disbursement for the batch attached to the finance request. This is calculated based on the sum of the face values of the attached invoices, deducting the retention margin configured at the facility attached in the finance request. This is updated at the end of each ‘Disburse’ action through a service. |

**Invoice Batching**

| Field | Description |
|---|---|
| Borrower | Specifies the Transact customer reference for whom the finance is disbursed. This is a mandatory field. |
| Borrower Role | Specifies the role of the customer. This field is mandatory when BORROWER is updated. |
| Counterparty | Specifies the counterparty reference. This is a mandatory field. |
| Counterparty Role | Specifies the role of the counterparty. This field is mandatory when a counterparty is defined. |
| Currency | Specifies the currency in which finance will be disbursed. This is a mandatory field. |
| Invoice Reference | Specifies the reference of the grouped invoices. A minimum of two Invoices should be given when batching action is performed. And a maximum of 10 Invoices can only be updated manually by the bank user. |
| Unbatch | Used to unbatch already batched invoices. |
| No of Invoices | Specifies the number of invoices selected under a batch. |
| Finance Request | Specifies the Finance Request ID under which the batch is financed. |
| Upload Reference | Specifies the upload reference for the invoices that were processed through bulk upload. This is used as a criterion for batching by upload reference. |
| Auto Batch | Used to initiate batching by selection based on the given criteria. This field is optional. |
| Batch Reference | Specifies the Sub-Batch reference created during Auto batch. |
| Auto Batch Reference | Specifies the batch reference created during Auto batch. This is a system-updated field, and is updated only during the Auto batching process. |

**Invoice Capture**

| Field | Description |
|---|---|
| Days Post Maturity | Stores the number of days after which the invoices with settled status will be automatically transferred to the History file. This field is mandatory. |
| Duplicate Check | Holds the duplicate check definition for the SU.INVOICE.CAPTURE table to prevent duplicate upload of Invoices. The ID of EB.DUPLICATE.TYPE must be updated in this field to enable the duplicate check functionality. This field is optional. |
| Document Type | Specifies the document type used in SU.INVOICE.CAPTURE . This field refers to the virtual table SU.INVOICE.TYPE . Only the document types defined here are permitted in SU.INVOICE.CAPTURE . It is mandatory to define at least one document type. |
| Role | Holds the list of participants permitted for the specified document type. A minimum of two roles must be defined when configuring the document type. This field refers to AA.CUSTOMER.ROLE and becomes mandatory when a document type is specified. |
| Role Required | Holds the list of participants permitted for the specified document type. A minimum of two roles must be defined when configuring the document type. This field refers to AA.CUSTOMER.ROLE and becomes mandatory when a document type is specified. |

**Invoice Capture**

| Field | Description |
|---|---|
| Original Reference | Specifies the invoice reference number imported from the customer-submitted invoice. This field is an alpha numeric field with a maximum of 35 characters. It is a mandatory field. |
| Document Type | Holds the document type. It refers to virtual table SU.INVOICE.TYPE . The user can select the invoice types that are defined in the SU.PARAMETER . This field is mandatory. |
| Party | Specifies the customer who is part of the document. Holds the Transact customer reference and Mnemonic. This is a mandatory field. |
| Role | Specifies the role of the customer, for example, whether the captured customer is a SUPPLIER or BUYER. It refers to AA.CUSTOMER.ROLE. This is a mandatory field when Party is defined. The system only allows the roles that are part of the parameter defined for the document type. |
| Currency | Holds the currency of the invoice. It refers to the CURRENCY table for validation. It should be a valid record in the CURRENCY table. This is a mandatory field. |
| Amount | Holds the value of invoice amount which should be greater than 0.00. This is a mandatory field. |
| Issued Date | Specifies the date on which the invoice was issued by the drawer. It should be in standard date format (cannot be a future date). This is imported from the invoice submitted by the customer. This is a mandatory field. |
| Payment Due Date | Specifies the date on which the invoice is due for payment, and the drawee is expected to pay the Invoices. It is a standard date format field. The value should be greater than issued date. This is a mandatory field. |
| Financing Date | Specifies the date on which the borrower wants the invoices to be financed. It is a standard date format field. The date should not be greater than the payment due date and less than the issue date. This is an optional field. |
| Remarks | Stores remarks or comments if any. This is an optional field with a maximum of 100 characters. |
| Upload Reference | Stores the upload reference when the invoices are uploaded in bulk. |
| Document Status | This is a system-maintained field which holds the status of the invoice at various stages. Following are the possible values: NEW – updated when the Invoice is uploaded. BATCHED - updated when the Invoice is Batched. Unbatching the Invoice from the batch reverses the status back to NEW. FINANCED - updated when the Invoice is financed. FINANCE REQUESTED - updated when the Invoice is directly attached to the finance request for finance disbursement. Removing the invoice reference from the finance request reverses the status back to NEW. SETTLED - updated when the loan on the Invoice is fully settled and the SETTLE.INVOICE field is set. |
| Status Date | Specifies the date on which the status was last updated. |
| Batch Reference | Holds the batch reference under which the respective invoice is batched. This is a system-updated field. This field also holds the finance request reference when one invoice is financed from a finance request. |
| Financing Request | Holds the Finance Request Reference ID of the captured invoice upon requesting for finance. This is a system-updated field. |
| Finance Amount | Holds the finance amount. This field is updated by the system when the invoice is financed. |
| Drawing Reference | Contains the Drawing Reference ID generated for the specific invoice upon disbursement as part of financing. This is a system-updated field. |
| Payment Type | Holds the payment type. This field can be configured by the user from the virtual table EB.LOOKUP - SU.PAYMENT.TYPE. |
| Payment Currency | Holds the currency of the payment amount done on the invoice, which should be a valid currency defined in the CURRENCY table. |
| Payment Amount | Holds the payment amount done on the invoice. This is a system-updated field. |
| Payment Date | Holds the date of payment done on the invoice. This is a system-updated field. |
| Reference | Holds the payment reference. This is a free text field, with the length of 50 character. This field is optional. |
| Settle Invoice | This is an optional field which allows the user to settle the invoice. This field can be configured only when the invoice is already financed. If the underlying loan status is neither close nor pending closure, the system throws a validation error on committing the SU.INVOICE.CAPTURE with SETTLE.INVOICE set to Yes. On successful commit, the document status for the invoice is updated as ‘Settled’. |
| Available Amount | Specifies the available amount for disbursement in the invoice batch attached to the finance request. This is calculated based on the sum of the face values of the invoice, deducting the retention margin configured at the facility attached in the finance request. This is updated at the end of each ‘Disburse’ action through a service. |

**Invoice Capture**

| Sequence | Fields updated |
|---|---|
| 1 | Original Reference |
| 2 | Document Type |
| 3 | Party |
| 4 | Role |
| 5 | Currency |
| 6 | Amount |
| 7 | Issue Date |
| 8 | Payment Due Date |
| 9 | Financing Date |
| 10 | Upload Reference |

**Misc**

| Sl.no | Product Name | Product Attributes |
|---|---|---|
| 1 | SCF Programme | SCF Deal |
| 2 | SCF Facilities | SCF Revolving Facility SCF Term Facility |
| 3 | SCF Drawings | Factoring Receivables Discounting |


### Trade_Banking - TCIB (TCIB)


**Import Drawings**

| Section | Description |
|---|---|
| LC Summary | Displays the details of the LC. More details are displayed in pop-up window on selecting the ‘Details view’. |
| Drawings Details | Displays the details of the drawing, including the documents status (Clean documents) and other related details. Incoming MT754 can be viewed and downloaded from the ‘View delivery details’. |
| Payment Details | Allows the corporate user to select the account number from which the payment needs to be effected. |


---
