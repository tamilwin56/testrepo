
# Temenos Transact — Reconciliation_Matching Module Documentation


> **Comprehensive User Guide**
> Generated: 13 April 2026
> Content: Configuration | Reference | Field Descriptions | Glossary


## Table of Contents

  - [Reconciliation_Matching Module Overview](#reconciliation_matching-module-overview)
    - [Sub-Module Summary](#sub-module-summary)
    - [How to Use This Guide](#how-to-use-this-guide)
  - [Chapter 1: Reconciliation_Matching - ER](#chapter-1-reconciliation_matching---er)
    - [Features in Reconciliation_Matching - ER](#features-in-reconciliation_matching---er)
    - [1.1  AutomaticCreationRegularReceipts](#11-automaticcreationregularreceipts)
    - [1.2  CorrespondentBankLimitChecking usingER](#12-correspondentbanklimitchecking-usinger)
    - [1.3  Creation ExpectedReceipts](#13-creation-expectedreceipts)
    - [1.4  Matching AdvisedFunds](#14-matching-advisedfunds)
    - [1.5  Matching ExpectedReceiptsPayments](#15-matching-expectedreceiptspayments)
    - [1.6  Matching gpi Cover Message with Payment Instruction](#16-matching-gpi-cover-message-with-payment-instruction)
    - [1.7  MatchingPaymentInstructions CoverPayments](#17-matchingpaymentinstructions-coverpayments)
    - [1.8  Misc](#18-misc)
    - [1.9  Pre-AuthorisedCredits](#19-pre-authorisedcredits)
  - [Chapter 2: Reconciliation_Matching - NR](#chapter-2-reconciliation_matching---nr)
    - [2.1  Misc](#21-misc)
  - [Appendix A: Glossary of T24 Applications & Fields](#appendix-a-glossary-of-t24-applications-fields)
    - [Applications](#applications)
    - [Fields Referenced](#fields-referenced)
  - [Appendix B: Consolidated Field Reference](#appendix-b-consolidated-field-reference)
    - [Reconciliation_Matching - ER (ER)](#reconciliation_matching---er-er)
    - [Reconciliation_Matching - NR (NR)](#reconciliation_matching---nr-nr)

---


## Reconciliation_Matching Module Overview


This document provides comprehensive documentation for the **Reconciliation_Matching** module of Temenos Transact. It covers **2 sub-modules** with a total of **10 feature areas**.


### Sub-Module Summary


| # | Sub-Module | Code | Features | Description |
|---|-----------|------|----------|-------------|
| 1 | **Reconciliation_Matching - ER** | `ER` | 9 | Reconciliation_Matching - ER module of Temenos Transact |
| 2 | **Reconciliation_Matching - NR** | `NR` | 1 | Reconciliation_Matching - NR module of Temenos Transact |


### How to Use This Guide


Each feature in this document is organized into the following sections:

- 📖 **Introduction** — Overview and purpose of the feature
- ⚙️ **Configuration** — How to set up and configure the feature
- 🔧 **Working With** — Operational usage and field descriptions
- 📋 **Tasks** — Step-by-step procedures
- 📊 **Outputs** — Reports, enquiries, and generated outputs

Each feature includes a **Quick Reference Card** at the top with application names, key fields, prerequisites, and a summary. Appendices provide a full glossary, consolidated field tables, and end-to-end use-case scenarios.

---


## Chapter 1: Reconciliation_Matching - ER


Reconciliation_Matching - ER module of Temenos Transact


### Features in Reconciliation_Matching - ER


| # | Feature | Sections |
|---|---------|----------|
| 1.1 | AutomaticCreationRegularReceipts | Intro, Confi, Worki, Tasks, Outpu |
| 1.2 | CorrespondentBankLimitChecking usingER | Intro, Confi, Worki, Tasks, Outpu |
| 1.3 | Creation ExpectedReceipts | Intro, Confi, Worki, Tasks, Outpu |
| 1.4 | Matching AdvisedFunds | Intro, Confi, Worki, Tasks, Outpu |
| 1.5 | Matching ExpectedReceiptsPayments | Intro, Confi, Worki, Tasks, Outpu |
| 1.6 | Matching gpi Cover Message with Payment Instruction | Intro, Confi, Worki, Tasks, Outpu |
| 1.7 | MatchingPaymentInstructions CoverPayments | Intro, Confi, Worki, Tasks, Outpu |
| 1.8 | Misc | Intro |
| 1.9 | Pre-AuthorisedCredits | Intro, Confi, Worki, Tasks, Outpu |


### 1.1  AutomaticCreationRegularReceipts


> **📇 Quick Reference Card**
> 
> **Purpose:** *The STANDING.ORDER application is used for scheduled expected receipts. Such scheduled receipts are known as regular receipts.*
> 
> **Applications:** `AC.EXPECTED.RECS`, `ER.PARAMETER`, `FUNDS.TRANSFER`, `STANDING.ORDER`, `STO.GEN.EXP.RECS`, `STO.TYPE`
> 
> **Key Fields:** *Details*, *Diary*, *Routine*, *User*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The STANDING.ORDER application is used for scheduled expected receipts. Such scheduled receipts are known as regular receipts.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 🔧 Working With

When a regular set of receipts are expected and to be monitored, Temenos Transact allows to create the receipt records automatically by using a local routine in the STANDING.ORDER application. The following workflow is required to create AC.EXPECTED.RECS on a regular automated basis. The ability to create regular receipts is dependent on a few pre-conditions.


##### Amending or Using the CorrectSTO.TYPE

The STO.TYPE used on the STANDING.ORDER must have the use of local routines enabled.


##### Settings inER.PARAMETER

The ER.PARAMETER must contain the funds types Regular Receipts (RR) and its partner Expected Regular Receipts (ERR) as required. These are similar to the standard ER and RECEIPT types but are distinguished due to the method of creation in STANDING.ORDER .


##### User Routine

The STO.GEN.EXP.RECS is provided as a template for any local developments. In order to use a different routine the programs must exist and must be compiled, but must also have a record in PGM.FILE with the program name. The user routine is called to create the records in AC.EXPECTED.RECS as per local requirements and must return the ID(s) back to the record in STANDING.ORDER .

Certain fields are validated based on STO.TYPE having the User Routine field set to Yes and other fields are based on the use of the local routine name placed in the Diary Details field. When STANDING.ORDER is authorised, it creates the record in AC.EXPECTED.RECS for the first instalment, and further records are based on the cycle frequency. They are matched (fully or partially) by incoming payments in FUNDS.TRANSFER .

Processing incoming payments and creation of the opposite receipts are same as standard AC.EXPECTED.RECS . This feature is simply a method to create the expected receipts.


#### 📋 Tasks

There are no Tasks available for Automatic Creation of Regular Receipts feature.


#### 📊 Outputs

There are no Outputs available for Automatic Creation of Regular Receipts feature.


> **Related Applications:** `AC.EXPECTED.RECS`, `ER.PARAMETER`, `FUNDS.TRANSFER`, `STANDING.ORDER`, `STO.GEN.EXP.RECS`, `STO.TYPE`

---


### 1.2  CorrespondentBankLimitChecking usingER


> **📇 Quick Reference Card**
> 
> **Purpose:** *In case the payments transaction between two different banks take place in different currencies, there is a cover (margin) payment involved. The payment instruction for such cover payments are held until the receiver is satisfied that the cover payment has been made.*
> 
> **Applications:** `AC.EXPECTED.RECS`, `AC.EXPECTEDS.RECS`, `EB.FREE.MESSAGE`, `EB.QUERIES.ANSWERS`, `ER.COVER.LIMIT`, `ER.PARAMETER`, `FT.APPL.DEFAULT`, `FT.TXN.TYPE.CONDITION`
> 
> **Key Fields:** *Account*, *Adv*, *Amount*, *Av*, *Available Limit*, *Await*, *Cancel*, *Cancel Query* ... +24 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

In case the payments transaction between two different banks take place in different currencies, there is a cover (margin) payment involved. The payment instruction for such cover payments are held until the receiver is satisfied that the cover payment has been made.

The payment requests are automatically authorised by the system without the receipt of cover payment confirmation, where the sending bank does not hold vostro account with receiver bank but has a preset allowance. For this purpose, a record in ER.COVER.LIMIT application is created to check whether a cover is received or not within the specified escalating period.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 🔧 Working With

Banks may receive the MT103 messages requesting for payments made by the receiver bank, which does not hold accounts in the transacting currency with the receiver bank. The receiver bank expects a cover payment to be made by the sender through one of its correspondents, who notifies the receiver of the cover payment in some method. The payment instruction is held until the receiver is satisfied that the cover payment has been made.

Temenos Transact automatically authorises the payment requests, without the receipt of cover payment confirmation, where the sending bank does not hold a vostro account with the receiver bank but it has a preset allowance. MT195s are produced to query an unauthorised payment and it is finally cancelled (when it has been authorised within an unused limit), if a cover is not received within specified escalating period.

For cover payments during MT103 inward processing, a record is created in AC.EXPECTED.RECS application with the Funds Type field set to EC (Expected Cover) and the Status field set appropriately based on the limit availability. Then create a record in the ER.COVER.LIMIT application with the sender’s bank identification code (BIC) and limit affected to the extent of incoming transaction amount. The FUNDS.TRANSFER (FT) record is created in hold or live, based on the available limit with the incoming MT103 details.

In AC.EXPECTED.RECS , the cover details received for MT103 payment can be input manually with the Funds Type field set to RC (Received Cover). When MT103 is received for payment, the system checks for matching cover details before processing and when the matching cover is available, the system matches RC and EC records. If the match is not found, the available limit is reduced to the extent of the transaction amount, as defined in ER.COVER.LIMIT for the sender of MT103. To match the EC record with the RC record, the matching criteria like Account No , Currency , Amount , Value Date and Reference can be specified in ER.PARAMETER .

In AC.EXPECTED.RECS application, the EC records can be created only through inward message processing. The RC records can be created through manual input or through an interface using the statement entry details or cover payment details. The related ID of AC.EXPECTED.RECS is available in FT and the ID of ER.COVER.LIMIT is available in AC.EXPECTED.RECS for cross-reference. The EB.FREE.MESSAGE application raises MT195 (queries) for the unmatched AC.EXPECTED.RECS during Close of Business (COB) batch process for follow-up.


##### Correspondent Cover Limit Processing

This section covers the steps to process correspondent cover limit.

The Await Cover field in FT.APPL.DEFAULT is set as required. The following are the option in this field:

- LIM – Indicates that the limit correspondent checking functionality is used when inward MT103 is received.
- YES – Indicates that the FT’s created through inward processing are always put into HOLD and the user has to manually check the cover details.
- Blank or Null – Indicates that the HOLD or approve cover limit processing is not activated.

Create a record in ER.PARAMETER with ID as COVER. Enter the matching criteria for payment request cover limits and retention days for moving the matched records to history. The SYSTEM record in this application controls the expected payment or receipt (ER or EC) functionality.

Specify the limit allotted to a bank with no vostro account holdings in ER.COVER.LIMIT . The ID for this application accepts eight or eleven characters-valid BIC code. When a record for the sender of MT103 is not available in this application, the system automatically creates a record with available limit as 0. To setup a limit for a bank that can be used by all branches, the ID must be created with eight characters (that is, without branch code or XXX).

A limit is created for USD 1,000,000 that is available up to 31 Dec 2005 and covers all the SWIFT branches for that customer.

The Expected Recs field is set in the FT.TXN.TYPE.CONDITION for the relevant FUNDS.TRANSFER or FT.TYPE records.

> **⚠️ Note:** The inward delivery process may use several different types according to the message content, so set all relevant fields.

Following are the scenarios when an inward MT103 message is received from a non-vostro customer.

If the limit is not defined in ER.COVER.LIMIT for the customer. The system creates a FT on hold and EC record is created in AC.EXPECTED.RECS application with the Status field set as UA (unauthorised). Also, the record is created in ER.COVER.LIMIT with the Available Limit field as 0.

If the limit is defined and available for the customer,

An FT record is created and authorised, and an EC record is created in AC.EXPECTED.RECS with the Status field set as AU (authorised). The limit amount is reduced from ER.COVER.LIMIT for the customer to the extent of payment amount.

Since the limit is already defined and available for the customer, the FT is created and authorised, and

is created with the

field as AU.

If the incoming message amount is in excess of any limit amount available, then the FT is created on hold and AC.EXPECTED.RECS is created with the Status field as UAL (unavailable limit).

If the cover details is available for a payment, then the FT record is authorised, an EC record is created and matched with the respective RC record with the Status field as M (matched). However, the limit is not affected as cover for the payment is received.

In this case, the RC record is entered manually with the reference details.

During the processing of an inward MT103 message, an EC record is created with incoming details and the system matches the EC record with RC details (as per the matching criteria), and the Status field set as M (matched) for both the records.

In case, the FT created through inward processing is changed manually, then the Status field is changed to MA (manually affected or authorised) in the relevant AC.EXPECTED.RECS and when the corresponding RC is received the same is matched.

The matched EC or RC type of AC.EXPECTED.RECS records are moved to history after the retention period as specified in ER.PARAMETER with SYSTEM.ID as COVER.

In case, the EC record in AC.EXPECTED.RECS remains unmatched after the number of days as specified in Request Adv Days field (available in ER.PARAMETER ) from the creation date, an MT195 queries message is sent using EB.FREE.MESSAGE application with the inward message detailing to the sender of MT103 with the non-receipt of cover funds.

In the above

record, the status is in UAL (unauthorised limit), after two days as specified in the

field in

and from the date of creation, creates a record in

with details as received. Then MT195 is sent to the sender of the original MT103 message seeking clarification.

If the EC record remains unmatched after the number of days as specified in ER.PARAMETER in Cancel Adv Days field from the date of creation of AC.EXPECTED.RECS record, then MT195 queries are sent using the EB.FREE.MESSAGE application. It informs the cancellation of the message because of non-receipt of cover funds even after a reminder. The relevant AC.EXPECTED.RECS record is changed to BC (batch cancelled) status.

The user level query details related to request or cancel for Field 75 in MT195 can be specified in the Request Query or Cancel Query at the respective AC.EXPECTED.RECS record and the same is used while generating MT195 using EB.QUERIES.ANSWERS application.

If the details are not specified in individual AC.EXPECTED.RECS , then query details for MT195 message ( Field 75 ) are defaulted to 2 for request and 36 for cancel event.

To process EC records that are waiting for cover payment for the ID entered in the Related Cover Id field, after entering RC details in AC.EXPECTED.RECS , then the Process Payments field is set to YES. Based on the matching criteria as specified in ER.PARAMETER , the system matches unmatched EC record (status as UAL) with RC in online process and the related FT record is authorised by the system.

During the above process the available cover limit for the Account No increases. To utilise this available limit for the remaining unmatched EC records, to authorise FT records while entering RC records in AC.EXPECTEDS.RECS , the Process Av Limit field is set to YES.

If the user wants to skip the limit and matching process during RC input, as it involves some time for processing online, the Process Av Limit and Process Payments fields in AC.EXPECTED.RECS can be left blank. In this case, the COB batch process related to AC.EXPECTED.RECS handles the matching and utilisation of available limit with the unmatched EC records, and the relative FT is authorised.


#### 📋 Tasks

There are no Tasks available for Correspondent Bank Limit Check using Expected Receipts feature.


#### 📊 Outputs

There are no Outputs available for Correspondent Bank Limit Check using Expected Receipts feature.


> **Related Applications:** `AC.EXPECTED.RECS`, `AC.EXPECTEDS.RECS`, `EB.FREE.MESSAGE`, `EB.QUERIES.ANSWERS`, `ER.COVER.LIMIT`, `ER.PARAMETER`, `FT.APPL.DEFAULT`, `FT.TXN.TYPE.CONDITION`

---


### 1.3  Creation ExpectedReceipts


> **📇 Quick Reference Card**
> 
> **Purpose:** *The AC.EXPECTED.RECS application is created for recording the upcoming or expected payments or receipts. The ER.PARAMETER application is used to specify the account in which the payment or receipt is monitored. After entering the basic account details in ER.PARAMETER and authorising it, the rest of ...*
> 
> **Applications:** `AC.EXPECTED.RECS`, `DE.I.HEADER`, `DE.MESSAGE`, `ER.PARAMETER`, `FT.TXN.TYPE.CONDITION`, `OFS`
> 
> **Key Fields:** *Expected*, *Funds*, *Ofs*, *Recs*, *Source*, *Type*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The AC.EXPECTED.RECS application is created for recording the upcoming or expected payments or receipts. The ER.PARAMETER application is used to specify the account in which the payment or receipt is monitored. After entering the basic account details in ER.PARAMETER and authorising it, the rest of the details are entered in AC.EXPECTED.RECS .


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 🔧 Working With

This topic explains the manual and auto creation of expected funds in Temenos Transact .


##### Manual Creation of Expected Funds

For manual entry, the Funds Type field is set to ER for purchase and receipt of bonds (as shown in the below screenshot).


##### Auto Creation of Expected Funds from Inward MT210 SWIFT

Temenos Transact can create a record in AC.EXPECTED.RECS from an inward MT210 SWIFT message automatically for the qualifying account(s). For auto creation, the following setup is done:

- The OFS details.
- The VERSION record for use.
- The sub-routine in the DE.MESSAGE record for 210.

Run the inward delivery service to check the record in DE.MESSAGE . The delivery system uses the program defined to create the appropriate Temenos Transact record, for example, the DE.MESSAGE is setup with OFS settings for the records in AC.EXPECTED.RECS .

The record ID of OFS.SOURCE is defined in the Ofs Source field. The TESTOFS record must have the Source Type field set to GLOBUS and may be used by other inward delivery processing.

The number of authorisers in AC.EXPECTED.RECS , OFS version is set to one and all records in AC.EXPECTED.RECS created are in INAU (no errors), if there are errors then the status is changed to IHLD.

> **⚠️ Note:** The INPUTTER for these records is GTUSER (OFS_ID).

The IHLD messages must be completed manually or deleted (if required) and INAU records must be authorised before the end of business day. If not the system deletes the messages in the batch. This applies to any records entered manually or created by any other automatic process.

The complete cycle of the expected funds received notification through inward SWIFT MT210 and the corresponding record created in AC.EXPECTED.RECS is explained below:

- The inward SWIFT message (in basic form) is viewed with the INCOMING.MSG enquiry.
- The DE.I.HEADER application shows the message being processed.
- At this stage, the message processed by the AC.EXPECTED.RECS deal is not completed.

- The unauthorised AC.EXPECTED.RECS record which the incoming process created. Once this is authorised, it updates the DE.I.HEADER with a better audit trail information.


##### Auto Creation of Expected Funds and Payments from FT

The system can be setup to create the receipt or payment records in the AC.EXPECTED.RECS from the incoming FT. For auto creation, the Expected Recs field in FT.TXN.TYPE.CONDITION must be set to Yes.

Once this is defined, qualifying payment FTs trigger the generation of an expected payment record when unauthorised. Authorising the qualifying FT receipt or payment records trigger the generation and matching of the receipt or payment records in AC.EXPECTED.RECS .

> **⚠️ Note:** If the Expected Recs field is not set to Yes in FT.TXN.TYPE.CONDITION and if it is not for the qualifying account, then a record is not created in AC.EXPECTED.RECS .

If an expected receipt or payment record is created, then the ID of this record is displayed in the information box. If there is an expected record to which this receipt is automatically matched, then a message to this effect is displayed.

The manually FT entered triggers a match with an expected receipt. The inward charge of USD15 is applied, so that the match is partial as the expected amount is USD 16,000.00. The auto creation of

from FT with the information of the ID is shown in the below screenshots.

The FT input auto creation of AC.EXPECTED.RECS is shown in the below screenshots.

The matched records are displayed with auto SWIFT and auto created FT.


#### 📋 Tasks

The AC.EXPECTED.RECS application is used to record the upcoming or expected payments or receipts. The ER.PARAMETER application is used to specify the account in which the payment or receipt is monitored.


##### Workflow

The user can perform the following activities:

The ER.MATCHING.CONDITION,ADMIN.INPUT version allows the user to indicate more define, flexible matching criteria and match different attributes in the expected cover and received cover.

1. Expected Receipts Matching Conditions .
2. In the List of ER Match Condition Records screen, click the Amend Entry icon corresponding to a record.
3. In the Er Matching Condition Admin Input screen, enter values in the following mandatory fields:
4. Click the Validate icon to check for errors and overrides
5. Click the Commit icon to submit the record.

The ER.FUNDS.TYPE.PARAM,ADMIN.INPUT version allows the user to parameterise funds type receipts.

1. Expected Receipts Funds Type Parameter .
2. In the List of ER Funds Type Param Records screen, click the Amend Entry icon corresponding to a record.
3. In the ER Funds Type Parameter screen, enter values in the following mandatory fields:
4. Click the Validate icon to check for errors and overrides
5. Click the Commit icon to submit the record.

To capture the expected receipts for CAMT057, follow the below steps:

1. Create camt057 Expected Receipts .
2. In the Expected Receipts-Create CAMT057 screen, enter values in the following fields: From Bic Reference Id Related Reference Acc Identification Expected Value Date Currency Item Amount Correspondent BIC
3. Click the Validate icon to check for error and overrides.
4. Click the Commit icon to create the ER record.

1. ER Message For PACS009 .
2. In the Expected Receipts For PACS009 screen, enter values in the below fields: Sender Bic Reference Id Related Reference Account Id Value Date Currency Amount Correspondent Account Correspondent BIC UETR
3. Click the Validate icon to check for error and overrides.
4. Click the Commit icon to create the ER record.


#### 📊 Outputs

There are no Outputs available for Creation of Expected Receipts feature.


> **Related Applications:** `AC.EXPECTED.RECS`, `DE.I.HEADER`, `DE.MESSAGE`, `ER.PARAMETER`, `FT.TXN.TYPE.CONDITION`, `OFS`

---


### 1.4  Matching AdvisedFunds


> **📇 Quick Reference Card**
> 
> **Purpose:** *This functionality describes how the Delivery module receives the SWIFT CBPR+ ISO20022 camt.057.001.06 (equivalent SWIFT MT210) and CBPR+ ISO20022 camt.058.001.08 messages, processed and matched by the Expected Receipts module. The system matches,*
> 
> **Applications:** `AC.EXPECTED.REC`, `AC.EXPECTED.RECS`, `DE.CARRIER`, `DE.I.HEADER`, `DE.MESSAGE`, `ER.FUNDS.TYPE.PARAM`, `ER.MATCHING.CONDITION`, `ER.MATCHING.CONIDITION` ... +3 more
> 
> **Key Fields:** *Account Id*, *Account No*, *Amount*, *Application Format*, *Cancel Adv Days*, *Check Cut Off*, *Corresp Account*, *Currency* ... +31 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

This functionality describes how the Delivery module receives the SWIFT CBPR+ ISO20022 camt.057.001.06 (equivalent SWIFT MT210) and CBPR+ ISO20022 camt.058.001.08 messages, processed and matched by the Expected Receipts module. The system matches,

- The MT210 SWIFT or CBPR+ ISO20022 camt.057.001.06 messages against the MT103, MT202, ISO20022 pacs.008 or pacs.009 messages received by TPH.
- The CBPR+ ISO20022 camt.058.001.08 messages against the CBPR+ ISO20022 camt.057.001.06 messages.

The MT210 or the ISO20022 CBPR+ camt.057.001.06 messages allow the account owner or the party authorised by the account owner to send an advance notification to announce that the funds will be credited to their account and serviced by the receiver of the message through a correspondent.

Temenos Payments Hub (TPH) receives the actual payment as an MT202, MT103, or their ISO20022 equivalents, that is, pacs.008 and pacs.009 messages. Even though the actual payment is received after the cut-off time, the value date can still be considered as the bank is advised in-time through a corresponding MT210 or camt.057.

The CBPR+ ISO20022 camt.058.001.08 message is sent by an account owner (or by a party acting on the account owner's behalf) to one of the account owner's account servicing institutions. It is used to advise the account servicing institution about the cancellation of one or more notifications in the previous CBPR+ ISO20022 camt.057 message.


#### ⚙️ Configuration

Three records are released in ER.MATCHING.METADATA for the Expected Receipt (MT210) and Receipt (MT103 and MT202), to indicate that the correspondent account (CORRESP.ACCOUNT) is required as a matching criteria in the matching process. Two records are released in ER.FUNDS.TYPE.PARAM for ER and Receipt. Based on these records it indicates the matching condition that is applicable for the below two types of funds:

- Match ER with Receipt
- Match Receipt with ER

The ER.MATCHING.CONDITION releases the ER.WITH.RECEIPT and RECEIPT.WITH.ER records, to indicate that the matching criteria must be used for matching ER with Receipt. To match MT210 with the MT103 or MT202, the matching fields to be considered are:

- Amount
- Value Date
- Correspondent Account
- Account

The below record indicates the attributes in the receipt which are matched against the attributes from the expected receipts ( Match Field and Match With Field ).

The ERCANCEL (funds type) record is released in ER.FUNDS.TYPE.PARAM and is used to capture the notifications to receive cancellation messages (camt.058 messages).

The below parameterisation records released in ER.MATCHING.CONDITION indicate the criteria that is used for matching items of ERCANCEL (used for camt.058 messages) against the ER Funds type (used for MT210 or camt.057 messages) and vice versa.

- ERCANCEL.WITH.ER
- ERCANCEL.WITH.ERUETR
- ER.WITH.ERCANCEL
- ER.WITH.ERCANCELUETR

The following field values are considered for matching.

- SENDER.BIC
- ORIG.MESSAGE.ID
- TRAN.REFERENCE
- REFERENCE
- END.TO.END.REF

The below record indicates that the attributes in the ERCANCEL that are matched against the attributes of the expected receipts ( Match Field and Match with Field ).


##### Routing Inward CBPR+ camt.057 and camt.058 Messages to Expected Receipt Module

The Interact ISO20022 messages are received by the Delivery Transformation Layer through the integration queues and routed to the business application based on the routing rules configured in the QueueConfigMX properties file.

The rule in the QueueConfigMX properties file decides the internal channel to which the inward messages received from swift.finplus service are routed to.

- Inward camt.057 messages to CAMT57 internal channel.
- Inward camt.058 messages to CAMT58 internal channel.

The Delivery Transformation Layer handles the messages assigned to the CAMT57 and CAMT58 internal channels according to the attributes defined in their respective properties files.

The CBRPLUS Delivery Carrier is assigned to the message as indicated by the Carrier attribute. The Queue Configurations are shown below.

- CAMT057
- CAMT058

Temenos Transact Delivery subsystem uses the routine configured in Inward Ofs Rtn in DE.MESSAGE for CAMT057 and CAMT058 to process the transformed payload message.


##### Matching Metadata

The ER.MATCHING.METADATA application defines the mandatory attributes for the matching items. The elements which are included in the matching criteria can be specified here to ensure the matching items go in exception if an element part of the matching criteria is blank. When a new matching item is created in the AC.EXPECTED.RECS application, the system combines the value of the Funds Type and the Message Type fields, separated through ‘.’ (dot) and checks if there is a record with this id in the ER.MATRCHING.METADATA application. The matching item is placed in exception queue if the required fields (Required = Yes) identified by the setup in the Matching Field are blank.

For example, in the matching items which have funds type as ER (Expected Receipt), created through 210 messages, the Correspondent Account must be present. If the value of this field is blank, the matching item should go into exception queue so the bank user can review and action the matching item manually.


##### Parameterisation for ER (Expected Receipt), Receipt Funds Type, and ERCANCEL (Expected Receipt Cancellation)

The parameterisation for ER (Expected Receipt), Receipt Funds Type, and ERCANCEL (Expected Receipt Cancellation) is explained below.

- The ER value of Funds Type indicates matching items created by the notification to receive messages.
- The Receipt value of Funds Type denotes matching items created by the system for payments.
- The ERCANCEL value of Funds Type denotes matching items created for notification to receive cancellation messages.

ER.FUNDS.TYPE.PARAM describes the main characteristics of each type of matching items presented below.

The notification to receive messages (MT210 or camt.057) can help banks to effectively manage their liquidity on the Nostro accounts – knowing in advance that they will receive funds in those accounts, they can take better decisions. The bank can indicate if they want forward entries to be raised when the matching item is created but is not matched – the fields in the AC.EXPECTED.RECS application which identify the debit account and the respective transaction codes are set here. For example, when an ER type of matching item is created, the bank can decide whether they want forward debits to be raised on the correspondent account to include the notifications to receive funds messages in the Nostro’s account position.

Banks are usually compensating their clients for sending these type of messages by respecting the payment the value date, even if the payment is received after the payment cut off time. However, to take decisions in time, it is important for the bank to receive these messages in time – the cut off time for MT210/camt.057 is defined in TPH. The Check Cut Off field in the ER.FUNDS.TYPE.PARAM application indicates if the ER module should check the cut off time for MT210/camt.057 messages. This option should be set for ER matching items as shown in the picture below. The AC.EXPECTED.REC defaults the Rcvd After Cut Off field to Yes if the Check Cut Off in the ER.FUNDS.TYPE.PARAM is set to Yes and the MT210 or camt.057 message is received after their cut off.

The ER.FUNDS.TYPE.PARAM application also defines the matching conditions – the matching items with Funds Type defined by the id of the ER.FUNDS.TYPE.PARAM will be matched with items with the Funds Type defined in Match Funds Type , using the rule specified in the Match Condition field – which points to the ER.MATCHING.CONDITION application.

For example, in the configuration released in Model Bank for ER funds type as shown in the above screenshot.

- Initially, the system attempts to match the ER Funds Type items with ERCANCEL Funds Type items using the criteria defined in the MatchERwithERCancelUETR matching condition.
- If a match is not found, the system checks for the second matching condition and it attempts matching the ER Funds Type items with ERCANCEL Funds Type items using the criteria defined in the MatchERwithERCancel matching condition.
- If a match is not found, then the system checks for the third matching condition and it attempts matching the ER Funds Type items with Receipt Funds Type items using the criteria defined in the MatchERwithReceipt matching condition.

Model Bank is configured in a similar way for RECEIPT and ERCANCEL items indicating that they are matched with ER items and the corresponding matching conditions.

The parameter setup in the ER.FUNDS.TYPE.PARAM application overrides the parameter setup in the ER.PARAMETER application. If the ER.FUNDS.TYPE.PARAM application is not defined, then the setup in the ER.PARAMETER application is considered for matching.

Exclude Currencies in the ER.FUNDS.TYPE.PARAM application allows the bank to indicate the list of currencies for which they do not want to match the notification to receive messages (usually, for local currency). If an MT202 or camt.057 message is received and the currency is excluded, the matching item is placed in exception.


##### Matching Condition Parameterisation

The ER.MATCHING.CONDITION application defines the matching criteria for the matching items. Matching With Field indicates the field in the funds type matching item to which the matching condition is linked in ER.FUNDS.TYPE.PARAM . Matching With Field indicates the field in the Match Funds Type matching item associated with the matching condition in the in ER.FUNDS.TYPE.PARAM . For example, consider the setup shown below:

The MatchERwithReceiptUETR ER.MATCHING.CONIDITION record is referred in the definition of the ER ER.FUNDS.TYPE.PARAM , therefore Matching Field indicates a field in the ER matching item. Match Funds Type associated with the Match Condition MatchERwithReceiptUETR indicates RECEIPT, therefore Matching With Field represents a field in the RECEIPT matching item. Looking at the above, the value CCY.AMOUNT value in the ER matching item must match the CCY.AMOUNT value in the RECEIPT matching item, and so on.

As shown above, the matching condition defines the following matching criteria for the ER (notice to receive messages) and RECEIPT matching items (payment messages), no tolerance, no partial matching:

- Amount
- Value Date
- Correspondent Account
- Account
- End To End Ref (UETR)


#### 🔧 Working With

The ER module reconciles the inward notice to receive messages (MT210, CBPR+ camt.057) with the inward notice to receive cancellation message (CBPR+ camt.058) or with the corresponding payment messages (MT103, MT202, pacs.008, pacs.009) received by TPH.

The Delivery Transformation Layer receives and transforms MT210, CBPR+ camt.057, and camt.058 and the Delivery module routes them to the ER module. The ER module creates matching items in AC.EXPECTED.RECS . Funds Type is set as ER (Expected Receipt) for MT210/camt.57 and ERCANCEL for camt.58.

When the payment is received, TPH sends a request to the ER module that creates a matching item in AC.EXPECTED.RECS with Funds Type set as Receipt.


##### Manually Capture MT210 inAC.EXPECTED.RECS

The ER module offers the option to manually capture a notice to receive, which can be received by fax or e-mails similar to the SWIFT MT210.

The following are the mandatory fields for capturing a notice to receive:

- Message Type (defaulted to 210)
- Sender BIC
- Value Date
- Currency Code
- Amount
- Reference
- Related Reference


##### Receive Directly an MT210 inAC.EXPECTED.RECS

An MT210 message can be either entered in the system by the user (using the option to manually capture the notice to receive) or the MT210 message can be directly received by the ER module from delivery. Based on this, an AC.EXPECTED.RECS record with the Funds Type field as ER (Expected Receipt) is created in the system.

Record, ACER0935700109, is created in

with the

field set to ER and the

field set to WAITING.

When the payment (MT103 or MT202) is received by TPH, the system sends a request to the ER module and an AC.EXPECTED.RECS record with the Funds Type field as Receipt is created.

Based on the defined matching criteria, the receipt record is matched with the expected receipt record. The status of the receipt and expected receipt records are updated to MATCHED and the Matched With field is updated with the reference of the Expected Receipt or Receipt.

The receipt record (ACER0935700112) is created with the Status field as MATCHED, that is, the Matched With field mapped to the Expected Receipt transaction (ACER0935700109).


##### Capturing camt.058 inAC.EXPECTED.RECSManually

The user can manually capture a notice to receive cancelation messages using the ER module.

The following are the mandatory fields for capturing a notice to receive cancelation message manually.

- Message Type (defaulted to CAMT058)
- From BIC
- Expected Value Date
- Currency
- Item Amount
- Reference/Item Id
- Tran Reference
- Original Notification Identification
- Notification Ids
- Reason code for cancellation


##### Receiving camt.058 message inAC.EXPECTED.RECS

The user enters the camt.058 message in the system (using the Create camt058 Expected Receipt Model Bank version to manually capture the notice to receive cancellation message) or it can be directly received by the ER module through the Transact Delivery module. Based on the inward message, the system creates a matching item in AC.EXPECTED.RECS with Funds Type as ERCANCEL (Expected Receipt Cancellation).

The camt.057 message is received by ER Module through Transact Delivery module and a matching item, ACER0935703404, is created in AC.EXPECTED.RECS with Funds Type set to ER and Status set to W - Waiting.

When the ER module receives the notice to receive cancellation message (camt.058) through Transact Delivery module, the system creates a new matching item with Funds Type as ERCANCEL.

The system automatically compares the notice to receive cancellation matching with the notice to receive matching item based on the defined matching criteria and finds the match.

- The system updates the Status of the ER matching item to M - Matched and populates Matched With with the reference of the ERCANCEL matching item.
- The system updates the Status of the ERCANCEL matching item (ACER0935877156) as MATCHED and populates Matched With with the reference of the ER (ACER0935703404).


##### Auto-Matching Expected Receipt Items with Receipt Items

When a new matching item is created in AC.EXPECTED.RECS , the system checks the parameterisation for the respective funds type in the ER.FUNDS.TYPE.PARAM and ER.PARAMETER . Read Configuration section for more information. Based on this configuration, it determines the corresponding matching condition and the relevant Matching Funds Type, selects all the unmatched items with this type and finds the one which matches the new item, based on the defined criteria.

If a matching item is not found, the matching process continues with the next matching condition. If all the defined matching conditions have been considered and matching item is not identified by the auto match process, the new record in AC.EXPECTED.RECS is left unmatched with Status as W - Waiting and is cancelled based on the parameterisation in the Cancel Adv Days in ER.PARAMETER .

For example, if an MT210/CBPR+ camt.057 is received in ER, one or more matching items with ER funds type are created (one for each credit item received in the inward message). Based on the setup indicated in the configuration section, the system determines that the ER funds type items must be matched with RECEIPT items, using the MatcERwithReceiptUETR matching condition. Therefore, it selects and evaluates all the existing unmatched Receipt items and compares them with the new item, considering the criteria defined in the matching condition. If an item satisfies the criteria, both items are marked as Matched and TPH is notified that the match has been found. If no item satisfies the criteria, then it continues with the next matching condition, if defined. If at the end of the process, the system could not find a match for the current item, it leaves this in the Waiting Status.

Similarly, when TPH receives an incoming payment (MT103, MT202, pacs.008 or pacs.009), it sends a request to the ER module for matching. The ER module creates a Receipt matching item which, based on the setup, is evaluated against all the unmatched ER items. If a matching item is found, then both items are marked as Matched and the response is sent to TPH.

The response or notification sent to TPH also indicates if the ER matching item has been received after the cut-off time for the advice (MT210/camt.057). Based on this, TPH moves the payment to repair so the bank user can decide the value date given to the customer or respects the value date indicated in the message.


##### Expected Receipts Matched Items

After the expected receipt and receipt record are matched, the user can view the records in the Expected Receipts Matched Items enquiry.

The ER record that is received following an MT210 message is shown in the below screenshot.

From this enquiry the user can:

- View Item – Displays the details of the AC.EXPECTED.RECS .
- View Related Matched Item(s) – Displays the related matched item(s) indicated in Matched With field and then the user can drill down to their details.
- View MT210 – Displays the incoming message details of the MT210 delivery message, if there is a delivery item linked to it.
- Unmatch – This option changes the status of the AC.EXPECTED.RECS item from MATCHED to WAITING.

The Unmatch option that changes the status of the AC.EXPECTED.RECS item from MATCHED to WAITING.


##### Expected and Receipts Unmatched Items

The records that were not matched in the ER module based on the matching criteria with the Status as WAITING are displayed in the Expected and Receipts Unmatched Items enquiry. From this enquiry the user can:

- View Details – Allows the user to view all the details of the item.
- View MT210 – Allows the user to view the incoming SWIFT MT210 (only for items created automatically based on an incoming SWIFT message).
- Modify Expected Receipt – Allows the user to amend the details of the expected receipt item.
- Cancel Expected Receipt – Allows the user to cancel the expected receipt item.
- Book Expected Receipt – Allows the user to book the expected receipt item.

The Cancel option that allows the user to enter the reason for the cancellation in the User Notes.

The Booked option that allows the user to book the transfer (debit the correspondent account, credit the customer account with the indicated value date). The FT module automatically creates a matching item that is automatically matched with the ER item.

The booked record created by FT are shown in the below screen shot.


##### Expected Receipts in Exception (Repair)

All the unmatched items with wrong currency, non-opening date or any other unmatched conditions are stored in the repair queue (exception queue). From this list the user can amend, delete or send the MT295 message.

The Amend option that allows the user to amend the matching item and modify the details.

The Delete option that allows the deletion of the matching item.

The Send MT295 option, which allows the user to send an MT295 message (queries), if the matching items are created based on the incoming MT210. The Send MT295 option is used to initiate an investigation for the received MT210.


##### Receiving Inward CBPR+ camt.057 and camt.058 in ER Module

The Delivery Transformation Layer receives the Interact ISO20022 messages from Temenos SWIFT Connector or from ESB. It routes the messages to the business applications based on the rules configured in the QueueConfigMX properties file. Read the Routing inward CBPR+ camt.057 and camt.058 messages to Expected Receipt Module section.

The Delivery Transformation Layer identifies the internal channel for the inward camt.057 and camt.058 messages received from the swift.finplus service (the SWIFTNet service used by CBPR+) based on the routing rules defined in the properties file. The attributes for this channel indicate that a transformation must be applied to the business document. The Delivery Carrier associated with the message is CBPRPLUS and the target business module is ER. The transformation extracts each item included in the inward camt.057, camt.58 and sends a message to Temenos Transact Delivery subsystem along with the header details and the original message.

Once the Temenos Transact Delivery subsystem receives the message, the system creates a record in DE.I.HEADER with Message Type as CAMT057 (for inward camt.057), CAMT058 (for inward camt.058), Application Format as ER, and Disposition as Unformatted. It also updates the technical header, business application header, and the transformed message files linked with this header for audit reasons.

As the CBPRPLUS record in DE.CARRIER indicates that the formatting module is XMLISO, the Delivery module adds the message in the XMLISO inward processing queue. After the XMLISO.IN service runs, it checks the definition of the DE.MESSAGE for CAMT.057 and CAMT.058. Using the Inward OFS routine, the Delivery module creates the AC.EXPECTED.RECS record from the received (transformed) payload. Depending on the processing, it updates Disposition in the DE.I.HEADER record to Formatted or Repair and this record is a valid ID of AC.EXPECTED.RECS .


##### Update Nostro/Vostro Position based on Notice to Receive

The bank can set up the ER module to update the position of the Nostro/Vostro account when notifications to receive messages are received. Read Configuration section for more information.

For example, the following set indicates the system must raise debit forward entries on the CORRESP.ACCOUNT specified in the AC.EXPECTED.RECS with ER funds type. The transaction code for the forward entry is set in the Fwd Db Txn Code . Similarly the system will raise a credit forward entry on the Account Id specified in the AC.EXPECTED.RECS with ER funds type using the transaction code set in the Fwd Cr Txn Code .

When a matching item is created (record is authorised) and is left unmatched by the auto-matching or manual process, the system checks the in the ER.FUNDS.TYPE.PARAM application to determine whether forward accounting entries must be raised.

The matching item with Funds Type ER and status Waiting are shown in the below screenshot.

Considering the setup above and the matching item shown in the above picture, the image below shows the debit forward entries raised on the account 10012312301 populated in the Corresp Account field and credit forward entries on the account 10020207901 indicated by the Account No field of the matching item. The Reference of the entries are pointing to the id of the AC.EXPECTED.RECS record of the above matching item.

When the matching item is matched, cancelled or moved to history, the forward entries are dropped. When a matched item is unmatched, the forward entries are re-created.

The ID of the related forward entry is stored in the AC.EXPECTED.RECS record.

The value date in the forward entry is the latest between the Value Date field in the AC.EXPECTED.RECS record and the current business date as the projection is shown from current business date forward. If an Expiry Date is captured in the AC.EXPECTED.RECS record, the system drops the forward entry when it reaches the Expiry Date, even if the matching item is still unmatched.

During COB, if the expected receipt has neither been matched nor cancelled, the Value Date in the projected entry is cycled forward to the next working day date and the balance in the available balance ladder is updated to next working date.


#### 📋 Tasks

Related topics:

- Perform Matching of Payment Notifications with Cover Payments

An MT210 message can be either entered in the system by the user (using the option to manually capture the notice to receive) or the MT210 message can be directly received by the ER module from delivery. Based on this, an AC.EXPECTED.RECS record with the Funds Type field as ER (Expected Receipt) is created in the system.

When the payment (MT103 or MT202) is received by TPH, the system sends a request to the ER module and an AC.EXPECTED.RECS record with the Funds Type field as Receipt is created.

Based on the defined matching criteria, the receipt record is matched with the expected receipt record. The status of the receipt and expected receipt records are updated to MATCHED and the Matched With field is updated with the reference of the Expected Receipt or Receipt.


##### Workflow

This section helps the user to perform the below tasks:

| SCREENS | WORKFLOW |
|---|---|
|  | Expected & Receipts Unmatched Items . |
| Records Waiting Match | Click the View Expected Receipts icon of a corresponding record. |
| AC Expected Receipts | View the expected receipt record details. |

| SCREENS | WORKFLOW |
|---|---|
|  | Expected & Receipts Matched Items . |
| Matched Records | Click the View Expected Receipts icon of a corresponding record. |
| AC Expected Receipts | View the expected receipt record details. |


#### 📊 Outputs

There are no Outputs available for Matching of Advised Funds feature.


> **Related Applications:** `AC.EXPECTED.REC`, `AC.EXPECTED.RECS`, `DE.CARRIER`, `DE.I.HEADER`, `DE.MESSAGE`, `ER.FUNDS.TYPE.PARAM`, `ER.MATCHING.CONDITION`, `ER.MATCHING.CONIDITION`, `ER.MATCHING.METADATA`, `ER.MATRCHING.METADATA`, `ER.PARAMETER`

---


### 1.5  Matching ExpectedReceiptsPayments


> **📇 Quick Reference Card**
> 
> **Purpose:** *The objective of AC.EXPECTED.RECS is to record the upcoming or expected payments which helps the bank to determine the projected balances and to maintain the books balanced. Once the bank receive the actual payment, the actuals are matched with the expected. In order to match the payments, the follo...*
> 
> **Applications:** `AC.EXPECTED.RECS`, `ACCOUNT`, `ER.PARAMETER`
> 
> **Key Fields:** *Account*, *Amount*, *Balance*, *Ccy*, *Currency*, *Ep*, *Er*, *Er Balance* ... +9 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The objective of AC.EXPECTED.RECS is to record the upcoming or expected payments which helps the bank to determine the projected balances and to maintain the books balanced. Once the bank receive the actual payment, the actuals are matched with the expected. In order to match the payments, the following methods are used:

- Auto matching
- Manual matching


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 🔧 Working With

This topic details the methods used to match the receipts or payments.


##### Auto Matching

This section covers the workflow of auto matching method.

Whenever a new record is authorised in AC.EXPECTED.RECS , the automatic matching process is started. The system attempts to match the new record with the existing records of the contrary Funds Type (new RECEIPT or PAYMENT is matched with the ER/EP or new ER/EP is matched with the existing RECEIPT or PAYMENT) and matches with all the Match With fields defined in the ER.PARAMETER .

If the exact match is not found and the tolerance is specified in the ER.PARAMETER , then the lower limit and higher limit values are calculated using the base values of the new record and the tolerance specified. The lower limit and higher limit values are used for Tolerance and Match With fields, and the exact match is specified in the non-tolerance Match With fields to find the match from the existing records.

If there is more than one matched record, then the first record is selected from the match list.

When two records are matched, the Status field is updated as MATCHED and the Matched With field has the corresponding matching record ID.


##### Manual Matching

This section covers the workflow of manual matching method.

Temenos Transact allows manual match of the expected receipt or payment records. Follow the below steps to use the basic method of matching:

1. Navigate to the AC.EXPECTED.RECS application or launch a version, such as AC.EXPECTED.RECS,MATCH
2. Use the input function and select the record to be matched (the current value in the Status field must be WAITING or PARTIAL MATCHED), change the value in the Status field to F (force manual match).
3. Then insert or select the ID of the record to be matched with in Match With field.
4. If the records are compatible, that is, if the Account No and Currency field values are same and the Funds Type field value is different, then these records are matched.
5. The record with a lower amount has the Status field as MATCHED, which is, fully matched.
6. The record with the higher amount has the Status field as PARTIAL MATCHED. The PARTIAL MATCHED record can be manual matched again with another record.

Temenos Transact has defined enquiries and versions which can be used to match manually the expected receipts or payments. The Expected Funds Waiting Match enquiry displays the expected receipt or payment messages with the Funds field as EXPECTED and the Status field as WAITING or PARTIAL MATCHED.

The Receipt Funds Waiting Match enquiry displays the records with the Funds Type field as RECEIPT or PAYMENT and the Status field as either WAITING or PARTIAL MATCHED.

The Expected Funds Waiting Match enquiry has the Details and Match Expected with Receipts options as shown in the below screen shot. Select the Match Expected with Receipts option to initiate the AC.EXPECTED.RECS,MATCH version.

The Manual Match – Expected with Receipt or Payment screen is displayed as shown in the below screen shot.

The user can either run the Receipt Funds Waiting Match enquiry or drill down on the Match With field, to fetch the record in AC.EXPECTED.RECS .

When there are match records with in the Ccy Amount tolerances, it is unavoidable that the small balances remains in the Er Balance and Ep Balance fields of the ACCOUNT application, although the expected fund is fully matched with the receipt fund. The balance can be offset with a compensating receipt, payment or expected record.

When the expected funds are for one value date but received or paid with a different value date, then the Er Balance or Ep Balance fields in the ACCOUNT application has a positive amount for the EXPECTED funds for the expected value date and negative amount for the RECEIPT or PAYMENT value date. If the tolerance is set, then these two field value are matched in AC.EXPECTED.RECS but the ACCOUNT gives a distorted information. This can be rectified by performing two opposite records for the two dates.


#### 📋 Tasks

Related topics:

- Perform Matching of Payment Notifications with Cover Payments

The objective of the AC.EXPECTED.RECS application is to record the upcoming or expected payments, which helps the bank to determine the projected balances and to maintain the books balanced. Once the bank receives the actual payment, it matches the payment against the expected receipt. The following screens and enquiries help the user to perform the matching activities.


##### Workflow

The user can perform the following activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Start Manual Matching . |
| Payment & Cover Unmatched Items | Enter values in the required fields. Click the FIND button. |
| Payment & Cover Unmatched Items | Click the View Details icon corresponding to a record. |
| AC Expected Receipts | The system opens the record in view mode. |

This enquiry displays the unauthorised payment and cover items from the AC.EXPECTED.RECS$NAU application.

To authorise the record, perform the following steps:

1. Authorise/Delete Payment & Cover Items .
2. In the Authorise/Delete Payment & Cover Items screen, click the Authorise icon corresponding to a record.
3. In the AC Expected Receipts screen, verify the details and then click the Authorise icon.

To delete the record, perform the following steps:

1. Authorise/Delete Payment & Cover Items .
2. In the Authorise/Delete Payment & Cover Items screen, click the Delete icon corresponding to a record.
3. In the AC Expected Receipts screen, click the Delete icon.

This enquiry displays the payment and cover matched items by the system and it fetches the data from the AC.EXPECTED.RECS application.

To view the record details , perform the following steps:

1. Payment & Cover Matched Items .
2. In the Payment & Cover Matched Items screen, click the View Details icon corresponding to a record.

To view the related matched item , perform the following steps:

1. Payment & Cover Matched Items .
2. In the Payment & Cover Matched Items screen, click the View Related Matched Item icon corresponding to a record.


#### 📊 Outputs

There are no Outputs available for Matching of Expected Receipts of Payments feature.


> **Related Applications:** `AC.EXPECTED.RECS`, `ACCOUNT`, `ER.PARAMETER`

---


### 1.6  Matching gpi Cover Message with Payment Instruction


> **📇 Quick Reference Card**
> 
> **Purpose:** *This functionality allows the matching of a payment message (MT103) against a gpi cover message (MT299 from gpi tracker), if received, or alternatively, against a cover message received from the correspondent bank (MT202COV). Temenos Payment Hub (TPH) receives and processes the payment (MT103) and c...*
> 
> **Key Fields:** *Amount*, *Correspondent BIC*, *Currency*, *End to End Reference*, *Funds Type*, *Match Funds Type*, *Matched With*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

This functionality allows the matching of a payment message (MT103) against a gpi cover message (MT299 from gpi tracker), if received, or alternatively, against a cover message received from the correspondent bank (MT202COV). Temenos Payment Hub (TPH) receives and processes the payment (MT103) and cover messages (MT202COV). The confirmation message (MT299) sent by the gpi tracker is received by the EB.FREE.MESSAGE application, which sends or passes the details of the received message to TPH.

TPH determines if the payment, cover or gpi confirmation is in the scope of matching and sends a matching request to the Expected Receipts (ER) module. This request creates a matching item with funds type as EC (Expected Cover) for MT103 payment messages. In the case of cover messages (MT202COV), the matching items have the funds type as RC (Received Cover). For gpi confirmation messages (MT299), TPH sends a request for matching with funds type as GC (GPI Cover).


#### ⚙️ Configuration

This section explains the configuration of Matching gpi Cover Message with Payment Instruction.


##### Enable the Matching of MT299 with the MT103 Message

Enabling the Matching of MT299 with MT103 in the Expected Receipts module, the following setup must be done in the ER.FUNDS.TYPE.PARAM application:

- Capture a new record GC in ER.FUNDS.TYPE.PARAM , representing the funds type for the GPI Cover.
- In the GC record, define MatchGCwithEC as the matching condition. This indicates that the MT299 message (GC – GPI Cover) is matched with the MT103 message (EC – Expected Cover).
- Then, define the value EC under the Match Funds Type field. This indicates that the GC Funds Type record is matched with the EC funds type record.


#### 🔧 Working With

This section explains the working of Matching of gpi Cover with Payment Instruction.

The EB.FREE.MESSAGE application receives the gpi cover message (MT299) and passes the information to Temenos Payment Hub (TPH). If the gpi cover message is in the scope of matching, TPH sends a matching request to the Expected Receipts (ER) module. This request creates a record in AC.EXPECTED.RECS with Funds Type as GC (GPI Cover) for the MT299 message.

The following screenshot is an example of an MT299 record created in the AC.EXPECTED.RECS application, for the GC funds type, with the status as W (Waiting), indicating that the record is waiting to be matched.

For the matching process, the ER.FUNDS.TYPE.PARAM application is used to store the main parameters related to the GPI Cover funds type.

The following screenshot is an example of the gpi cover model record released, which indicates the MatchGCwithEC matching condition that is to be used for the matching. According to this, the GPI Cover is matched with the Expected Cover.

The matching criteria to be used for this matching condition is MatchGCwithEC, which is retrieved from the ER.MATCHING.CONDITION application. The following screenshot is an example of the matching criteria used for matching the GPI Cover with Expected Cover.

According to the MatchGCwithEC matching condition, the following three fields (which are part of multiple applications) are considered as matching criteria for the two received messages (MT299 and MT103):

- End to End Reference (UETR) from Header Block 3
- Amount and Currency
- Correspondent BIC

If all the three criteria match in the two messages (MT103 and MT299), then the records are matched and their status is updated as M (Matched) in AC.EXPECTED.RECS . Otherwise, if the values from the three fields differ, the matching is not done and the two messages remain unmatched.

The MT103 payment is received and processed by TPH, which further sends a request to the ER Module. This request creates a record in AC.EXPECTED.RECS with funds type as EC for the received MT103 payments messages.

Based on the defined matching criteria (presented in the following screenshot), the EC can be alternatively matched with the RC (Received Cover – MT202COV) or GC, in case the matching with the first option (RC) could not be done. Below is an example of the EC record, which indicates the two alternative matching conditions for the matching MT103 payment:

- The matching condition, MatchECwithRC, is indicated first, which means the system will first try to match the MT103 with the Receive Cover (MT202COV).
- If the MT103 cannot be matched with the corresponding MT202COV, the system tries to match the MT103 based on the second matching condition, which means the system will try to match the MT103 with the GPI Cover, MatchECwithGC.

The first matching condition to be used for the matching is MatchECwithRC. This matching condition contains the following matching criteria to match the EC with RC.

The second matching condition to be used for the matching is MatchECwithGC. This matching condition contains the following matching criteria to match the EC with GC.

According to this matching condition, the following three fields are considered as matching criteria for the two received messages (MT103 and MT299):

- End to End Reference (UETR) from Header Block 3
- Amount and Currency
- Correspondent BIC

If all the three criteria match in the two messages (MT103 and MT299), then the records are matched and their status is updated as M (Matched) in AC.EXPECTED.RECS . Otherwise, if the values from the three fields differ, the matching is not done and the two messages remain unmatched.

In the below example, an MT103 message is matched with an MT299 message, where the MT103 message creates a record in AC.EXPECTED.RECS , with the reference ACER0935787460 and the Funds Type as Ec.

The MT299 message creates a record in AC.EXPECTED.RECS , with the reference ACER0935730329 and Funds Type as Gc.

Based on the record from ER.FUNDS.TYPE.PARAM for EC funds type, two matching conditions are indicated, as mentioned above:

- The first condition is MatchECwithRC
- The second condition is MatchECwithGC

The first matching condition (MatchECwithRC) is picked-up, but no match is found (as no RC record is present in AC.EXPECTED.RECS ).

The system then tries to match with the next condition MatchECwithGC.

The matching fields considered for matching are retrieved from the ER.MATCHING.CONDITION application, from the MatchECwithGC record, as displayed below:

As the values from these three fields ( End to End Reference , Amount and Currency and Correspondent BIC ) are the same in the two messages from AC.EXPECTED.RECS , the two ACER records are updated to the M (Matched) Status, and the Matched With field is updated with the reference of the counterparty transaction the matching was made with.

The Payment & Cover Unmatched Items and Payment & Cover Matched Items enquiries display the AC.EXPECTED.RECS records with Funds Type as GPI Cover, corresponding to the MT299 messages received from the gpi Tracker.

Payment & Cover Unmatched Items :

The following screenshot is an example of the Payment & Cover Unmatched Items enquiry.

Payment & Cover Matched Items :

The following screenshot is an example of the Payment & Cover Matched Items enquiry.


#### 📋 Tasks

There are no Tasks available for Matching gpi Cover Message with Payment Instruction feature.


#### 📊 Outputs

There are no Outputs available for Matching gpi Cover Message with Payment Instruction feature.

---


### 1.7  MatchingPaymentInstructions CoverPayments


> **📇 Quick Reference Card**
> 
> **Purpose:** *The bank can receive payments from parties with whom they do not have a direct relationship; the actual settlement of the funds being done through a correspondent bank. A common practice is that banks wait for a confirmation that cover is received before booking the payment on the beneficiary accoun...*
> 
> **Applications:** `AC.EXPECTED.RECS`, `ER.COVER.LIMIT`, `ER.FUNDS.TYPE.PARAM`, `ER.MATCHING.CONDITION`
> 
> **Key Fields:** *Funds Type*, *Matched With*, *Matching Condition*, *Matching Field*, *Matching With Field*, *Settlement Method*, *Status*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The bank can receive payments from parties with whom they do not have a direct relationship; the actual settlement of the funds being done through a correspondent bank. A common practice is that banks wait for a confirmation that cover is received before booking the payment on the beneficiary account, giving them access to funds. In some circumstances, the banks are willing to give some provision to some counterparties and set up cover limits, allowing the payments to be processed without the cover being received, if the cover limit defined for the sender of the payment is not reached.

The sender of the payment can specify the correspondent through which the funds are reimbursed. The correspondent can reimburse the receiving institution through either of the following methods:

- By crediting the vostro account of the receiving bank and sending a credit notification through MT910/CBPR+ camt.054 message
- By sending a MT202 cover payment
- By sending money through an RTGS

This functionality describes how the MT910 SWIFT message, or its equivalent CBPR+ ISO20022 camt.054.001.08 message, is received through Delivery, uploaded directly in the Expected Receipts module and matched against the MT103, MT202 SWIFT or their ISO20022 equivalents – pacs.008 or pacs.009 messages.

In few scenarios, the bank could receive MT202 or the ISO20022 equivalent, pacs.009 cover messages, directly in Temenos Payments Hub (TPH), these are also considered and matched with the received payments.


#### ⚙️ Configuration

Two records (as shown in the below screenshots) are released in ER.FUNDS.TYPE.PARAM for Expected Cover (EC) and Received Cover (RC). Based on these records the Matching Condition is indicated as MatchECwithRC and MatchRCwithEC.

The MatchECWithRC and MatchRCwithEC records (as shown in the below screenshots) are released in ER.MATCHING.CONDITION which indicates the matching criteria to be used for the matching of EC with RC.


##### Routing Inward CBPR+ camt.054 Messages to Expected Receipt Module

The Interact ISO20022 messages are received by the Delivery Transformation Layer through the integration queues and routed to the business application based on the routing rules configured in the QueueConfigMX properties file.

A rule in this file decides whether the inward camt.054 messages received from swift.finplus service are routed to the CAMT54 internal channel.

Delivery Transformation Layer handles the messages assigned to the CAMT54 internal channel according to the attributes defined in the properties file.

The SkipRouting = NO indicates that Temenos Transact Delivery subsystem routes the message.

The transformation, identified by the Xslt attribute, is applied to the payload before the Delivery Transformation Layer sends the message Temenos Transact Delivery subsystem, through the queue specified by the ACTIVEMQ attribute.

The CBRPLUS Delivery Carrier is assigned to the message as indicated by the Carrier attribute.

Temenos Transact Delivery subsystem uses the routine configured in the Inward OFS Rtn in DE.MESSAGE for CAMT.054 to process the transformed payload message.


##### Matching Metadata

The ER.MATCHING.METADATA application allows the user to define the mandatory attributes for a Funds Type. The elements that are matching criteria can be defined here to ensure the matching item goes in exception if an element part of the matching criteria is blank. For example, in the matching items with funds type ER (Expected Receipt), the Correspondent Account, part of the matching criteria, must be present. If this is not populated, the matching item should go in Repair.

The ER.MATCHING.METADATA application defines the mandatory attributes for the matching items. The elements which are included in the matching criteria can be specified here to ensure the matching items go in exception if an element part of the matching criteria is blank. When a new matching item is created in the AC.EXPECTED.RECS application, the system combines the value of the Funds Type and the Message Type fields, separated through ‘.’ (dot) and checks if there is a record with this id in the ER.MATRCHING.METADATA application. The matching item is placed in exception queue if the required fields (Required = Yes) identified by the setup in the Matching Field are blank.


##### Parameterisation for EC (Expected Cover) and RC (Receipt Cover) Funds Type

The EC funds type indicates matching items created for payments messages. The RC funds type denotes matching items created for cover or credit notifications messages.

The ER.FUNDS.TYPE.PARAM application describes the main characteristics of the funds type that are relevant to EC and RC funds type are summarized below.

The Corresp BIC field in the AC.EXPECTED.REC application is used in matching. To consider the BIC8 of the correspondent for matching, irrespective of how this is indicated in the message, the Store BIC8 field must be set to Yes. This ensures the Corresp BIC field in AC.EXPECTED.REC is populated with the BIC8 of the Org Corresp BIC field which stores the exact BIC indicated in the message.

The ER.FUNDS.TYPE.PARAM application also defines with which type of matching items a certain funds type is matched, as well as the relevant matching condition. The EC funds type parameterisation specifies the matching conditions for Expected Cover matching items with Receipt Cover matching items. The RC funds type parameterisation indicates the opposite, the matching conditions for Receipt Cover items with Expected Cover items.

For example, in the configuration released in Model Bank for EC funds type, two matching conditions are indicated – first, the system will attempt to match the funds type matching items with receipt matching items, using the criteria defined in the MatcERwithReceiptUETR matching condition. If no match is found, it will attempt to match them again with receipt items using the second matching condition MatcERwithReceipt.

The parameter setup in ER.FUNDS.TYPE.PARAM overrides the parameter setup in ER.PARAMETER . If the ER.FUNDS.TYPE.PARAM application is not defined, then the setup in ER.PARAMETER is considered for matching.


##### Matching Condition Parameterisation

The ER.MATCHING.CONDITION application defines the matching criteria for the matching items. The Matching With Field indicates the field in the funds type matching item to which the Matching Condition is linked in ER.FUNDS.TYPE.PARAM , the Matching With Field indicates the field in the Match Funds Type matching item associated with the Matching Condition field. For example, consider the following Model Bank setup shown in the picture below as well as the ER.FUNDS.TYPE.PARAM shown above:

This matching condition is attached to the RC funds type definition above. The Matching Field indicates the field in the RC funds type matching item which must match the field defined in Matching With Field , in the EC type matching item, where EC is the Matching Funds Type associated with the matching condition in the RC ER.FUNDS.TYPE.PARAM shown above. The matching condition defines the following matching criteria for the payment with cover:

- Related Reference in Cover with the Reference of the Payment
- Amount
- Value Date
- Sender BIC of the Cover message with the Correspondent BIC from the Payment


#### 🔧 Working With

The ER module is used to reconcile payments message details against cover message details. The matching items are stored in the AC.EXPECTED.RECS application. The inward MT910 and CBPR+ camt.054 messages are received through the Temenos Delivery module and are routed to the ER module. A record in AC.EXPECTED.RECS with the Funds Type field set as RC is created for them.

The payment (MT103, MT202 and their ISO20022 equivalent pacs.008, pacs.009) messages and cover messages (MT202, MT202 COV and their ISO20022 equivalent pacs.009 cover) are received and processed by TPH. If the payment and cover matching is in scope, TPH sends a matching request to the ER module when an inward payment or cover is received. This request creates a record in AC.EXPECTED.RECS with the Funds Type field set as EC for MT103, MT202, pacs.008, pacs.009 payment messages. For cover messages the AC.EXPECTED.RECS record has the Funds Type field as RC.

When a new record is created in AC.EXPECTED.RECS , the system considers the unmatched items and auto-matches a record with the Funds Type field set as EC against a record with the Funds Type field set as RC, based on the matching criteria indicated in the ER.FUNDS.TYPE.PARAM ER.PARAMETER – see Configuration section for details. If no matching item is found, the new record in AC.EXPECTED.RECS is left unmatched with status Waiting and a response or notification is sent to TPH to return the matching status.


##### Receiving MT910 in AC.EXPECTED.RECS

The ER module processes the incoming SWIFT MT910 received through Delivery module and creates a RC matching item and automatically updates the matching process with the cover matching item created by MT910.

The record in

is set with the amount of 666 USD and with the

field set as RC which created based on the received MT910 message.

The MT103 payment is received and processed by TPH which further sends a request to the ER module. This request creates a record in AC.EXPECTED.RECS with the Funds Type field set as EC for the received MT103 payment messages.

Based on the matching criteria defined, the RC record is matched with the EC record.

The following example shows the record in AC.EXPECTED.RECS set and updated.

The record in

is set with amount of USD 666 and

field set as EC. This is created following the MT103 message received from TPH. After the matching process, the record is updated with the

field as MATCHED and the

field is updated with the reference of RC record.


##### Receiving MT202COV in AC.EXPECTED.RECS

The MT202COV cover message is received and processed by TPH. If the cover message is in the scope of matching, TPH sends a matching request to ER module. This request creates an record in AC.EXPECTED.RECS with the Funds Type field as RC for the MT202COV message.

Also, the MT103 payment is received and processed by TPH which further sends a request to the ER module. This request creates a record in AC.EXPECTED.RECS with the Funds Type field as EC for the received MT103 payment messages.

Based on the matching criteria defined, the record in RC is matched with the EC record.

The matching process is similar to the matching of MT910 message with the MT103 payment message.

When a new matching item is created in AC.EXPECTED.RECS , the system checks the paramterisation for the respective funds type in the ER.FUNDS.TYPE.PARAM / ER.PARAMETER – see Configuration section for details. Based on this configuration, the system determines the corresponding matching condition and the relevant Matching Funds Type, selects all the unmatched items with this type and finds the one which matches the new item, based on the defined criteria.

If no matching item is found, it continues with the next matching condition. If all the defined matching conditions have been considered and no matching item is identified by the auto match process, the new AC.EXPECTED.RECS record is left unmatched.

For example, if an MT910/CBPR+ camt.054 is received in ER module, one or multiple matching items with RC funds type are created (depending on how many credit items are indicated in the received message). Based on the setup indicated in the Configuration section, the system determines this funds type must be matched with EC items, using the MatcRCwithEC matching condition and therefore it evaluates all the existing unmatched EC items and compares them considering the criteria defined in the matching condition. If an item satisfy the matching criteria, both items are marked as Matched and TPH is notified that a cover has been received and matched. If no item satisfies the criteria, it continues with the next matching condition, if defined. If at the end of the process, the system could not find a match for the current item, the system leaves this in the Waiting status.

Similarly, when TPH receives an incoming payment (MT103, MT202, pacs.008, pacs.009) or a cover (MT202 COV, pacs.009 cov), it sends a request to the ER module for matching. The ER creates ab Expected Cover or Received Cover matching item which, based on the setup, is evaluated against all the unmatched RC or EC items. If a matching item is found, both items are marked as Matched and the response is sent to TPH.

In the ER module, the bank can define the cover limits which can be used for the senders of SWIFT messages, who does not have a vostro or nostro relationship with the bank. The cover limits are defined in ER.COVER.LIMIT application and they are defined based on the bank identifier code (BIC).

The sender’s cover limits are checked based on the requested settlement method indicated by TPH in the request. If the settlement method (from AC.EXPECTED.RECS ) is equal to limit, then the system checks the ER.COVER.LIMIT record associated with the sender BIC.

If the available amount is greater or equal to the payment amount, then the sender’s cover utilised amount is increased and matching item is reflected as authorised.

If the available amount is lesser than the payment amount, then the status of the matching item is reflected as unauthorised, the cover limit is not impacted and a response is sent to TPH. Based on this response TPH moves the payment to repair.

If the Settlement Method field has any value other than LIMIT, the sender’s cover limit is not checked and the Status field is set to Unmatched.

The payment and cover matching items (with Funds Type field as EC or RC and Status field as UNAUTHORISED, AUTHORISED or UNMATCHED) that were not matched in the ER module are displayed in the Payment & Cover Unmatched Items enquiry.

From this enquiry the user can:

- View Details – Allows the user to view all the matching item details.
- View SWIFT Message Detail – Allows the user to view the incoming SWIFT message, if any.
- Amend Matching Item – Allows the user to amend the details of the matching item and add a comment.
- Cancel Matching Item – Allows the user to cancel the matching item, if forward entries are raised for this matching item they are dropped.
- Send MTn95 – Allows the user to create an MT195 or MT295 based on the original SWIFT message.
- Match Items – Allows the user to manually search an item and then match that against another item.
- Create Matching Cover – Allows the user to indicate if a matching cover item should be created for payment.

The View details options which allows the user to view all the matching item details:

The Amend option which allows the user to amend the details of the matching item:

The Cancel option which allows the user to cancel the matching item:

The Send MTn95 option which allows the user to create an MT195 or MT295 based on the original SWIFT message:

The Manually Match option which allows the user to manually search an item and then match it against another item:

The Create Matching Cover option which allows the user to indicate if a matching cover item should be created for payment:

After matching EC and RC record, the user can view the records through the Payment & Cover Matched Items enquiry.

From this enquiry the user can:

- View Details – Allows the user to view the matching item details.
- Related Matching Details – Allows the user to view the related matching items, drill down and view each item.
- Send MTn95 – Allows the user to create an MT195 or MT295 based on the original SWIFT message.

The View Details option which allows the user to view the matching item details:

The Related Matching Details option which allows the user to view the related matching item:

The option which allows the user to create an MT195 or MT295 based on the original SWIFT message:

The Interact ISO20022 messages are received by the Delivery Transformation Layer from Temenos SWIFT Connector or from ESB, through queues. Delivery Transformation Layer routes the messages to the business applications based on the routing rules configured in the QueueConfigMX properties file – see configuration section Routing inward CBPR+ camt.054 messages to Expected Receipt module.

Based on the routing rules defined in the properties, the Delivery Transformation Layer identifies the internal channel for the inward camt.054 messages received from the swift.finplus service (the SWIFTNet service used by CBPR+). The attributes for this channel indicate that a transformation must be applied to the business document, the Delivery Carrier associated with the message is CBPRPLUS and the target business module is ER. The transformation extracts each credit item included in the inward camt.054 and sends a message to Temenos Transact Delivery subsystem, along with the header and the original message details.

Temenos Transact Delivery subsystem receives the message, creates a DE.I.HEADER record with the Message Type as CAMT054, Application ER and Unformatted Status. It also updates the technical header, business application header as well as the transformed message files linked with this header for audit reasons.

As the CBPRPLUS DE.CARRIER record is using the Formatting Module XMLISO, Delivery also adds the message in the XMLISO inward processing queue. After the XMLISO.IN service runs, it checks the definition of the CAMT.054 DE.MESSAGE and, using the Inward OFS Rtn, creates the AC.EXPECTED.RECS record from the received (transformed) payload. Depending on the processing result, it updates the disposition of the DE.I.HEADER record to Formatted or Repair.


#### 📋 Tasks

Related topics:

- Perform Matching of Payment Notifications with Cover Payments

Banks can receive payments from third parties with whom they do not have a direct relationship; the actual settlement of the funds being done through a correspondent bank. As a practice, banks wait for a confirmation that cover is received before booking/crediting the payment on the beneficiary account.

This functionality describes how the MT910 SWIFT message, or its equivalent CBPR+ ISO20022 camt.054.001.08 message, is received through Delivery, uploaded directly in the Expected Receipts module and matched against the MT103, MT202 SWIFT or their ISO20022 equivalents – pacs.008 or pacs.009 messages.


##### Workflow

In this feature, the user can perform the following tasks:

| SCREENS | WORKFLOW |
|---|---|
|  | Start Manual Matching . |
| Payment & Cover Unmatched Items | Enter values in the required fields. Click the FIND button. |
| Payment & Cover Unmatched Items | Click the View Details icon corresponding to a record. |
| AC Expected Receipts | View the record details. |


#### 📊 Outputs

There are no Outputs available for Matching Payment Instructions and Cover Payments feature.


> **Related Applications:** `AC.EXPECTED.RECS`, `ER.COVER.LIMIT`, `ER.FUNDS.TYPE.PARAM`, `ER.MATCHING.CONDITION`

---


### 1.8  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *The expected funds or payments in Temenos Transact are recorded in the AC.EXPECTED.RECS application. It allows the bank to determine the projected balances and assist them to perform their business more efficiently. When the funds are received or payments are made, the movements are recorded and mat...*
> 
> **Applications:** `AC.EXPECTED.RECS`, `ACCOUNT`, `ER.PARAMETER`
> 
> **Key Fields:** *Ac*, *Account*, *Amount*, *Balance*, *Category*, *Ccy*, *Date*, *Days* ... +12 more
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- Temenos Transact Services

The expected funds or payments in Temenos Transact are recorded in the AC.EXPECTED.RECS application. It allows the bank to determine the projected balances and assist them to perform their business more efficiently. When the funds are received or payments are made, the movements are recorded and matched with the expected funds or payments.

The received funds are notified through incoming SWIFT MT210, telex or phone and the like. When a notification is received through SWIFT MT210 inward message, the expected receipt record is created automatically in the AC.EXPECTED.RECS application with the Status field set to WAITING and the Er Balance field in the ACCOUNT application is updated with the expected balance for the value date. Similarly, expected payments may be recorded manually or automatically, when an unauthorised funds transfer (FT) is entered and the Ep Balance field in the ACCOUNT application is updated with the expected balance for the value date.

Temenos Transact automatically creates the RECEIPT or PAYMENT record in AC.EXPECTED.RECS with the Status field defaulting to WAITING, when Temenos Transact records the fund receipt in FT or authorise a payment. The AC.EXPECTED.RECS attempts to match the created record with the EXPECTED records in the system. The Status fields of these records are updated as MATCHED, if a match is found. If the RECEIPT record is not matched, then the funds are received without notification or the funds are received before the notification. Further, the system attempts to match the EXPECTED funds with RECEIPT or PAYMENT funds, whenever the EXPECTED fund record is created.

In the ACCOUNT application, the expected receipt and payment balances for the value date is updated for all the expected funds in AC.EXPECTED.RECS for the accounts. The expected funds amount is added to the appropriate field and the receipt or payment amount is subtracted from the value date.

Also, the AC.EXPECTED.RECS allows the user to enter manually the expected funds record .


##### Product Configuration of Expected Receipts

The following parameter must be configured to use the AC.EXPECTED.RECS application.

| Field | Description |
|---|---|
| Account No and Category | Defines the accounts qualifying for selection in AC.EXPECTED.RECS . |
| Ac Over Days and Ac Ret Days fields | Allows the user to set the number of days the unmatched and matched items are kept in the system for an account. |
| Overdue Days and Retention Days | Defines the system and default values (when not set for individual account). |
| Match Field | Specifies the fields used in the matching process. |
| Account No , Ccy Amount and Value Date | Indicates the mandatory fields for matching the items in the system. |
| Tolerance | Specifies the tolerance to be used in finding the match, the tolerance is only allowed in the Ccy Amount and Value Date fields. |
| Ccy Amount | Indicates the tolerance defined as a percentage of the expected amount. The RECEIPT and PAYMENT records within the limit of the expected records are matched. If there is one or more matching records, then the first entry in the list is matched. The system first attempts for the exact match before attempting for the tolerance match, but if it is not found the first record found within the tolerance limits is matched. |
| Value Date | Indicates the tolerance defined as number of days (before and after the value date) on the matching record, these are the calendar days. Further, the tolerance is used in the record to be matched and the first attempt is for the exact match and if the exact match fails then the tolerance is used. Also, in the matching process the receipt funds are matched with the expected and vice versa. |


##### Illustrating Model Parameters

This section covers the high-level specifications required for the AC.EXPECTED.RECS application.

| S.No | Parameters | Description |
|---|---|---|
| 1. | ER.MATCHING.CONDITION | It allows the user to match different attributes in the payment or cover matching items. |
| 2. | ER.FUNDS.TYPE.PARAM | It allows the user to parameterise funds type. |
| 3. | ER.MATCHING.METADATA | It allows the user to decide the meta-data to be determined for the reconciliation process and, if needed to plug local logic. |


> **Related Applications:** `AC.EXPECTED.RECS`, `ACCOUNT`, `ER.PARAMETER`

---


### 1.9  Pre-AuthorisedCredits


> **📇 Quick Reference Card**
> 
> **Purpose:** *The system allows pre-authorised credits as STMT.ENTRY postings of type F (forward) to be raised by the AC.EXPECTED.RECS application.*
> 
> **Applications:** `AC.EXPECTED.RECS`, `ACCOUNT.PARAMETER`, `EB.CONTACT.BALANCES`, `ER.PARAMETER`, `STMT.ENTRY`
> 
> **Key Fields:** *Ac*, *Cash*, *Check*, *Code*, *Credit*, *Date*, *Days*, *Expiry* ... +16 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The system allows pre-authorised credits as STMT.ENTRY postings of type F (forward) to be raised by the AC.EXPECTED.RECS application.


#### ⚙️ Configuration

This topic details the setup for pre-authorised credits.


##### Setting upER.PARAMETER

The Fwd Funds Types field in the ER.PARAMETER application defines what type of funds raises the forward entries on the account. The Fwd Db Txn Code and Fwd Cr Txn Code fields define the transaction codes for the forward entries.


##### Setting upAC.EXPECTED.RECS

The Expiry Date field (optional field) in the AC.EXPECTED.RECS represents the day on which the record expires and is removed. The record is then passed to the HISTORY table. If the Expiry Date field is not populated during the creation of the record in AC.EXPECTED.RECS , then the system uses the existing logic based on the value date and tolerance days in the Overdue Days or Ac Over Days fields in ER.PARAMETER (if set).

The value in this field cannot be less than the system date and should be greater or equal to the value of the Value Date field (existing field).


#### 🔧 Working With

This topic covers the workflow of pre-authorised credits.


##### Changes in Updating the Account’s Funds Availability

The system raises forward (F) entries for different types of funds in the AC.EXPECTED.RECS .

The Fwd Funds Types field in ER.PARAMETER allows the forward entries to be registered in the system as unconfirmed entries posted against the account. The possible values for input in this field are the existing values from Funds Type field in the AC.EXPECTED.RECS application (like, EP, ER and ERR).

For registering expected payments the AC.EXPECTED.RECS records can be created in the system either manually by the user or automatically (through interfaces). When an AC.EXPECTED.RECS record is authorised by the system with Funds Type field as ER, the system raises forward entries on the account, updates the available balance with the specified amount.

No actual entry is registered in the ledger due to received pre-authorised credit. No booked or value dated balance of the account is updated in response to the pre-authorised credit transaction (Expected Receipt Transaction) received in the system. The system raises forward (F) entries on the account based on the value date set in the record. Funds are available on the accounts starting with the date set in the Value Date field. The F entries are raised even if the value date is equal to the current date.

According to the expiration date or value date, the funds remain available:

- Until the start of day of the date set in field, if it is set to a date in the future.
- Until start of day of the following day.
- If it is set as current date.

After this date, the same amount which was originally set in the record is reversed updating the available balance.

If the expiry date is set differently from the value date and is set to a date in the future, the system considers these funds in the available balance every day until the expiry date is met or until a settlement match is entered in the system (whichever comes first).

An expected payment is introduced in the system with a

equal to the current date (20th December) and the

set to 23rd December, for the credit amount of USD 2,000, this amount is considered in the available balance until a settlement matching payment is received.

If a settlement payment did not arrive in the system to match the original expected receipt record, then the record is deleted taking into consideration the expiry date. Funds are reversed at the start of day set as 23rd December. The pre-authorised credit record has the Status field Waiting until a matching settlement entry arrives in the system or until the record expires, according to the expiry date. The system recognises the unconfirmed entries when a debit transaction is posted on the accounts.

If Credit Check field is set to AVAILFWD and Cash Flow Days field is left blank in the ACCOUNT.PARAMETER , the system considers the forward entries posted through AC.EXPECTED.RECS when the system performs cover control on the specified account in case of a debit transaction. The F entries are considered in the available balance starting from the value date until the expiry date or until a matching settlement payment is posted. In case the expiry date is not provided, the value date and tolerance days are taken into consideration. A matching settlement payment can be setup in the system using the AC.EXPECTED.RECS , either manually or automatically.

If a match exists, the system updates the status of the original transaction to Matched.

In case of matched settlement transaction, the system reverses automatically the F entry from the STMT.ENTRY posted against the account by the ER transaction. Funds available on the account are deducted for the amount specified in the original ER record and posted back using the accounting entries raised by the settlement transaction.

Funds are also reversed from the account, if the expiry date is met.

The following example illustrates the creation of a record in ER.PARAMETER and funds available after updating the expected amount.

- A record is created in ER.PARAMETER , to enable the system to raise forward entries for the ER funds type, when an AC.EXPECTED.RECS record is created.

- An expected receipt for the Account 10010001101 is created using the AC.EXPECTED.RECS . The expected amount to be received is USD 1,100. The record has as an expiry date of 24th December 2009 (the system date is 23rd December 2009).

- The expected amount is updated as available funds in EB.CONTACT.BALANCES .

- Funds are available in the account until 24th December 2009 start of day or until a settlement payment is received.


#### 📋 Tasks

There are no Tasks available for Pre-Authorised Credits feature.


#### 📊 Outputs

There are no Outputs available for Pre-Authorised Credits feature.


> **Related Applications:** `AC.EXPECTED.RECS`, `ACCOUNT.PARAMETER`, `EB.CONTACT.BALANCES`, `ER.PARAMETER`, `STMT.ENTRY`

---


---


## Chapter 2: Reconciliation_Matching - NR


Reconciliation_Matching - NR module of Temenos Transact


### 2.1  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *Nostro account is the record of the bank that has deposited money at another bank. It differs from standard demand deposit bank accounts in that it is held by financial institutions, and is normally denominated in foreign currency. Nostro means ‘our money that is on deposit at your bank’. These acco...*
> 
> **Key Fields:** *External Location*, *Match Field Ledger*, *Match Field Stmt*, *Retention Days*, *Shut Out Carr*, *Split Items*, *T24 Location*, *Trans Type*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- Temenos Transact Services

Nostro account is the record of the bank that has deposited money at another bank. It differs from standard demand deposit bank accounts in that it is held by financial institutions, and is normally denominated in foreign currency. Nostro means ‘our money that is on deposit at your bank’. These accounts are often used to simplify settlements of trade and foreign exchange transactions.

Nostro Reconciliation involves the matching of the debit and credit activity in the domestic bank’s account with the statement of the account provided by the nostro account holding bank. This matching is done by the Nostro Reconciliation module and depends on the matching criteria defined by the user, such as matching by value date, currency, amount, transaction reference and reporting un-reconciled postings. Nostro Reconciliation module is used across any module (in Temenos Transact ) that uses nostro accounts for its transaction processing.

The following image shows the process map for Nostro Reconciliation.


##### Product Configuration

The nostro reconciliation module consists of the following processes:

- Message capture for incoming SWIFT MT940 and MT950 messages
- Capture of nostro ledger data in the form of MT940 messages diverted from DELIVERY module
- Statement extraction from aforementioned messages into Temenos Transact files
- Definition of matching parameters and controls
- Automatic matching procedure
- Manual matching procedure
- Manual unmatching procedure
- Manual statement input procedure

Nostro Reconciliation dependencies:

- Customer application for creating customer (counter parties) records of nostro banks.
- Account application for creating internal and nostro accounts meant for reconciliation purpose.
- Accounting application for generation of ledgers and receiving statements from nostro banks.
- Agency file for creating nostro agency arrangements.
- Delivery module for sending and receiving statements, that is, MT940/MT950 from nostro banks for reconciliation.
- Static tables like country and currency.

The NR.PARAMETER is the main application for the reconciliation process. User should setup the incoming and outgoing requirements before the user can input and authorise this record.

- One record is created for every company.
- Specifies matching rules for reconciliation process.
- Transaction codes for automatic matching process to be identified in Trans Type (transaction) field. This field allows determining how certain transactions are matched. For example, for items in SWIFT statement the user may wish to match miscellaneous transactions by value date and amount but matching cheques by amount only. The items are matched in the automatic matching process.
- The code to be prefixed with N (for nostro) and for entries which are advised first by the statement starts with F followed by any of the following: BOE – Bill of Exchange BRF – Brokerage Fee CHG – Charges and other Expenses CHK – Cheques CLR – Cash Letter or Cheques Remittance COL – Collections COM – Commission DCR – Documentary Credit DIV – Dividends Warrants EQA – Equivalent Amount ECK – Euro Cheques FEX – Foreign Exchange INT – Interest LBX – Lock Box LDP – Loan Deposit MSC – Miscellaneous RTI – Returned Items SEC – Securities STO – Standing Order TCK – Traveller’s cheque TRF – Transfer VDA – Value Date Adjustment

- Match Field Stmt and Match Field Ledger fields contain values from NR.STATEMENTS , which should be matched with the ledger from the system and statement from the nostro bank in case of automatic matching. This is a multi-valued field and any kind of combinations for matching processing can be specified.
- Split Items field allows to determine whether item splits are allowed in the manual matching process. Item splits are not allowed for auto matching process. This is used in cases where amounts are received with unexpected charges deducted. Larger amount can be allowed to split into two items. Main amount is matched with the statement amount received and the charge amount is to be left as outstanding one which is awaiting resolution. This is result of manually matching unequal amounts and acknowledging override messages.
- Number of days that a matched item needs to be in live file before moving into history file is specified in Retention Days field.
- T24 Location field defines the place from where these statements are located.
- External Location field defines the place from where these statements are located.
- Provides for usage of local reference fields to facilitate local customisations to cater to specific bank requirement.

Message capture uses MT940 and MT950 formats. The MT940 (customer statement) and MT950 messages are quite similar, with the exception being additional fields on the MT940 message namely, forward available balance and information to the account owner. Messages in the MT950 format can be produced from the nostro ledgers to pass a controlled set of postings to the reconciliations product. The messages are not sent to SWIFT. Within Temenos Transact , the Delivery module performs the function of mapping and formatting messages for delivery of outgoing and incoming messages either by SWIFT or other proprietary transfer mechanisms.

The following should be setup in Delivery module and the below section illustrates the required configuration.

DE.INTERFACE contains details of the protocols for all interfaces, which use the generic delivery interface. The ID of the file is the interface as defined in the Interface field on DE.CARRIER . For reconciliation, a RECS record needs to be setup.

The following screenshot shows the RECS record in Delivery Interface Parameter.

The messages to this interface is written to the F.DE.O.MSG.RECS file. Delivery interface parameter record name is entered in the record of NR.PARAMETER to instruct the statement decoding process find the messages location.

The DE.CARRIER contains details of all the carriers available in delivery. The user can enable a carrier by specifying it in the DE.PARM application. This contains formats, interface and address for every specific carrier record.

A record must be setup for defining the carrier to which the user route’s ledger MT940 or 950 messages.

A record should be available for each correspondent customer in DE.ADDRESS for the RECS carrier.

The following screenshot shows the DE.ADDRESS details.

The DE.CARRIER contains names and address of bank’s customers and each company within the banking organisation. This table is used for entering all addresses like SWIFT address, TELEX address and special postal address. ID to be used for reconciliation is . . (for example, US001001.C-100188.RECS.1) where RECS is ID in DE.CARRIER application.

If statements for internal accounts are produced for reconciliation, there must be a similar address record without customer component. For example, US001001.C-100188.RECS.1.

A record should be setup for each nostro account to be reconciled on DE.PRODUCT , to send the messages to the reconciliations carrier.

The following screenshot shows the MT950.

The following screenshot shows the MT940.

DE.PARM contains a single record that holds a number of parameters for controlling the processing of messages. The file contains the parameters that allow the operator to shut down the carrier control modules and the inward and outward formatting modules.

For nostro reconciliation, the RECS record created in DE.INTERFACE is added to the record in DE.PARM providing appropriate Shut Out Carr field.

The following screenshot shows the delivery carrier parameter record.

DE.MESSAGE table defines the contents of each basic message type. It lists the fields and describes them as single or multi values and states whether each field is mandatory or optional. ID is a valid swift type and MT950 is used for reconciliation.

The DE.SWIFT.DIVERSION application enables both inward and outward message to divert SWIFT message for given SWIFT message type and SWIFT address from SWIFT carrier to another file. The inward parameter is used to divert a copy of all incoming MT950 message to IN record in F.NR.DIVERT. If the user is diverting a copy of outgoing message for some other purpose, the user can leave the outward parameters unchanged. The outward fields are mandatory. The generic carrier is used to capture outgoing records for reconciliation.

For the reconciliation activity to begin, a record '950' must be setup.

The SWIFT carrier is expected to be running for the messages to be diverted to the diversion file.

The file that contains the incoming messages is named in DE.SWIFT.DIVERSION and in the External Location field in NR.PARAMETER . This is required for both incoming and outgoing delivery requirements before NR.PARAMETER is created.


##### Illustrating Model Parameters

This section covers the high-level specifications required for Nostro Reconciliation (NR) Module.

| S.No. | Parameters | Description |
|---|---|---|
| 1. | NR.PARAMETER | This application allows the user to specify matching rules for reconciliation process. It also allows the user to define transaction codes, which determine how transactions are matched. User can also define statement fields and ledger fields, which must be matched with the Nostro bank’s ledger of the system and statement. User can define retention days. The retention days are the number of days that a matched item must be in the LIVE table before moving it to HISTORY. User can define Temenos Transact location and external location where the NR statements from the Nostro bank must be located. |
| Apart from the specification in NR module, the following setup is also required in Delivery (DE) module. |  |  |
| 1. | DE.INTERFACE | The delivery interface parameter record is required to instruct the statement decoding process. |
| 2. | DE.CARRIER | This application allows the user to define the formats, interface and address required for the reconciliation carrier record. |
| 3. | DE.ADDRESS | This application allows the user to define the name and address of the bank’s customer for reconciliation delivery carrier record. User can also define delivery addresses for other carriers like SWIFT, TELLEX and special postal address. |
| 4. | DE.PRODUCT | This application allows the user to define a record for each Nostro reconciliation account to send messages to reconciliation carrier. |
| 5. | DE.PARM | The delivery parameter application allows user to shut down the reconciliation carrier control modules and inward, outward formatting modules. |
| 6. | DE.MESSAGE | This application allows the user to define the contents of message type MT940 and MT950 that used for reconciliation. |
| 7. | DE.SWIFT.DIVERSION | This application allows the user to divert SWIFT messages MT940 and MT950 from the SWIFT carrier to the diversion file for reconciliation purpose. |

---


---


## Appendix A: Glossary of T24 Applications & Fields


This glossary lists all T24/Transact application names and field names referenced throughout this document, with descriptions where available.


### Applications


| Application | Description |
|------------|-------------|
| `AC.EXPECTED.REC` | T24 application: AC.EXPECTED.REC |
| `AC.EXPECTED.RECS` | T24 application: AC.EXPECTED.RECS |
| `AC.EXPECTEDS.RECS` | T24 application: AC.EXPECTEDS.RECS |
| `ACCOUNT` | T24 application: ACCOUNT |
| `ACCOUNT.PARAMETER` | T24 application: ACCOUNT.PARAMETER |
| `DE.CARRIER` | T24 application: DE.CARRIER |
| `DE.I.HEADER` | T24 application: DE.I.HEADER |
| `DE.MESSAGE` | T24 application: DE.MESSAGE |
| `EB.CONTACT.BALANCES` | T24 application: EB.CONTACT.BALANCES |
| `EB.FREE.MESSAGE` | T24 application: EB.FREE.MESSAGE |
| `EB.QUERIES.ANSWERS` | T24 application: EB.QUERIES.ANSWERS |
| `ER.COVER.LIMIT` | T24 application: ER.COVER.LIMIT |
| `ER.FUNDS.TYPE.PARAM` | T24 application: ER.FUNDS.TYPE.PARAM |
| `ER.MATCHING.CONDITION` | T24 application: ER.MATCHING.CONDITION |
| `ER.MATCHING.CONIDITION` | T24 application: ER.MATCHING.CONIDITION |
| `ER.MATCHING.METADATA` | T24 application: ER.MATCHING.METADATA |
| `ER.MATRCHING.METADATA` | T24 application: ER.MATRCHING.METADATA |
| `ER.PARAMETER` | T24 application: ER.PARAMETER |
| `FT.APPL.DEFAULT` | T24 application: FT.APPL.DEFAULT |
| `FT.TXN.TYPE.CONDITION` | T24 application: FT.TXN.TYPE.CONDITION |
| `FUNDS.TRANSFER` | T24 application: FUNDS.TRANSFER |
| `OFS` | T24 application: OFS |
| `STANDING.ORDER` | T24 application: STANDING.ORDER |
| `STMT.ENTRY` | T24 application: STMT.ENTRY |
| `STO.GEN.EXP.RECS` | T24 application: STO.GEN.EXP.RECS |
| `STO.TYPE` | T24 application: STO.TYPE |


### Fields Referenced


| Field | Field | Field |
|-------|-------|-------|
| `Ac` | `Account` | `Account Id` |
| `Account No` | `Adv` | `Amount` |
| `Application Format` | `Av` | `Available Limit` |
| `Await` | `Balance` | `Cancel` |
| `Cancel Adv Days` | `Cancel Query` | `Cash` |
| `Category` | `Ccy` | `Check` |
| `Check Cut Off` | `Code` | `Corresp Account` |
| `Correspondent BIC` | `Cover` | `Credit` |
| `Currency` | `Currency Code` | `Date` |
| `Days` | `Delivery In Ref` | `Details` |
| `Diary` | `Disposition` | `End to End Reference` |
| `Ep` | `Er` | `Er Balance` |
| `Exclude Currencies` | `Expected` | `Expected Value Date` |
| `Expiry` | `Expiry Date` | `External Location` |
| `Field` | `Field 75` | `Flow` |
| `From BIC` | `Funds` | `Funds Type` |
| `Funds Types` | `Fwd` | `Fwd Cr Txn Code` |
| `Fwd Db Txn` | `Fwd Db Txn Code` | `Fwd Funds Types` |
| `Id` | `Inward Ofs Rtn` | `Item Amount` |
| `Limit` | `Match` | `Match Condition` |
| `Match Field` | `Match Field Ledger` | `Match Field Stmt` |
| `Match Funds Type` | `Match With Field` | `Match with Field` |
| `Matched` | `Matched With` | `Matching Condition` |
| `Matching Field` | `Matching With Field` | `Message Type` |
| `No` | `Notification Ids` | `Ofs` |
| `Original Notification Identification` | `Over` | `Overdue` |
| `Payments` | `Process` | `Process Av Limit` |
| `Process Payments` | `Rcvd After Cut Off field` | `Reason code for cancellation` |
| `Recs` | `Reference` | `Reference/Item Id` |
| `Related` | `Related Reference` | `Request` |
| `Request Adv Days` | `Request Query` | `Ret` |
| `Retention` | `Retention Days` | `Routine` |
| `Sender BIC` | `Settlement Method` | `Shut Out Carr` |
| `Source` | `Split Items` | `Status` |
| `T24 Location` | `Tolerance` | `Tran Reference` |
| `Trans Type` | `Type` | `User` |
| `User Notes` | `Value` | `Value Date` |
| `With` | `or` |  |


---


## Appendix B: Consolidated Field Reference


This appendix consolidates all field description tables from across the documentation, grouped by sub-module. This provides a single reference for all field definitions.


### Reconciliation_Matching - ER (ER)


**Misc**

| Field | Description |
|---|---|
| Account No and Category | Defines the accounts qualifying for selection in AC.EXPECTED.RECS . |
| Ac Over Days and Ac Ret Days fields | Allows the user to set the number of days the unmatched and matched items are kept in the system for an account. |
| Overdue Days and Retention Days | Defines the system and default values (when not set for individual account). |
| Match Field | Specifies the fields used in the matching process. |
| Account No , Ccy Amount and Value Date | Indicates the mandatory fields for matching the items in the system. |
| Tolerance | Specifies the tolerance to be used in finding the match, the tolerance is only allowed in the Ccy Amount and Value Date fields. |
| Ccy Amount | Indicates the tolerance defined as a percentage of the expected amount. The RECEIPT and PAYMENT records within the limit of the expected records are matched. If there is one or more matching records, then the first entry in the list is matched. The system first attempts for the exact match before attempting for the tolerance match, but if it is not found the first record found within the tolerance limits is matched. |
| Value Date | Indicates the tolerance defined as number of days (before and after the value date) on the matching record, these are the calendar days. Further, the tolerance is used in the record to be matched and the first attempt is for the exact match and if the exact match fails then the tolerance is used. Also, in the matching process the receipt funds are matched with the expected and vice versa. |

**Misc**

| S.No | Parameters | Description |
|---|---|---|
| 1. | ER.MATCHING.CONDITION | It allows the user to match different attributes in the payment or cover matching items. |
| 2. | ER.FUNDS.TYPE.PARAM | It allows the user to parameterise funds type. |
| 3. | ER.MATCHING.METADATA | It allows the user to decide the meta-data to be determined for the reconciliation process and, if needed to plug local logic. |


### Reconciliation_Matching - NR (NR)


**Misc**

| S.No. | Parameters | Description |
|---|---|---|
| 1. | NR.PARAMETER | This application allows the user to specify matching rules for reconciliation process. It also allows the user to define transaction codes, which determine how transactions are matched. User can also define statement fields and ledger fields, which must be matched with the Nostro bank’s ledger of the system and statement. User can define retention days. The retention days are the number of days that a matched item must be in the LIVE table before moving it to HISTORY. User can define Temenos Transact location and external location where the NR statements from the Nostro bank must be located. |
| Apart from the specification in NR module, the following setup is also required in Delivery (DE) module. |  |  |
| 1. | DE.INTERFACE | The delivery interface parameter record is required to instruct the statement decoding process. |
| 2. | DE.CARRIER | This application allows the user to define the formats, interface and address required for the reconciliation carrier record. |
| 3. | DE.ADDRESS | This application allows the user to define the name and address of the bank’s customer for reconciliation delivery carrier record. User can also define delivery addresses for other carriers like SWIFT, TELLEX and special postal address. |
| 4. | DE.PRODUCT | This application allows the user to define a record for each Nostro reconciliation account to send messages to reconciliation carrier. |
| 5. | DE.PARM | The delivery parameter application allows user to shut down the reconciliation carrier control modules and inward, outward formatting modules. |
| 6. | DE.MESSAGE | This application allows the user to define the contents of message type MT940 and MT950 that used for reconciliation. |
| 7. | DE.SWIFT.DIVERSION | This application allows the user to divert SWIFT messages MT940 and MT950 from the SWIFT carrier to the diversion file for reconciliation purpose. |


---
