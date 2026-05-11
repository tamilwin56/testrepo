
# Temenos Transact — Customer_Output Module Documentation


> **Comprehensive User Guide**
> Generated: 13 April 2026
> Content: Configuration | Reference | Field Descriptions | Glossary


## Table of Contents

  - [Customer_Output Module Overview](#customer_output-module-overview)
    - [Sub-Module Summary](#sub-module-summary)
    - [How to Use This Guide](#how-to-use-this-guide)
  - [Chapter 1: Customer_Output - BE](#chapter-1-customer_output---be)
    - [Features in Customer_Output - BE](#features-in-customer_output---be)
    - [1.1  Alert Processing](#11-alert-processing)
    - [1.2  Business Events](#12-business-events)
    - [1.3  Misc](#13-misc)
  - [Chapter 2: Customer_Output - DE](#chapter-2-customer_output---de)
    - [Features in Customer_Output - DE](#features-in-customer_output---de)
    - [2.1  BIC Database Upload](#21-bic-database-upload)
    - [2.2  Contact Preferences](#22-contact-preferences)
    - [2.3  Customer Address in Delivery Output](#23-customer-address-in-delivery-output)
    - [2.4  DefiningPrintFormat](#24-definingprintformat)
    - [2.5  DeliveryasMicroserviceEvents](#25-deliveryasmicroserviceevents)
    - [2.6  Detailed workflow Outward Delivery Messages](#26-detailed-workflow-outward-delivery-messages)
    - [2.7  DetailedWorkflow InwardDeliveryMessages](#27-detailedworkflow-inwarddeliverymessages)
    - [2.8  Diverting SWIFT MT Messages](#28-diverting-swift-mt-messages)
    - [2.9  Email SMS Secure Messaging](#29-email-sms-secure-messaging)
    - [2.10  Emitting Delivery Messages to Event Store](#210-emitting-delivery-messages-to-event-store)
    - [2.11  EndPeriodProcessing](#211-endperiodprocessing)
    - [2.12  Financial Messaging](#212-financial-messaging)
    - [2.13  Free Format Messages](#213-free-format-messages)
    - [2.14  Generation of MX Message using ISOMX Carrier](#214-generation-of-mx-message-using-isomx-carrier)
    - [2.15  Generic Delivery Interface](#215-generic-delivery-interface)
    - [2.16  Hold OutputDelivery Carriers](#216-hold-outputdelivery-carriers)
    - [2.17  Interbank Statement Request](#217-interbank-statement-request)
    - [2.18  Interim Intraday Transaction Report](#218-interim-intraday-transaction-report)
    - [2.19  InwardDeliveryMessageProcessing](#219-inwarddeliverymessageprocessing)
    - [2.20  Misc](#220-misc)
    - [2.21  Mx Message FW](#221-mx-message-fw)
    - [2.22  Recovery DeliveryTables](#222-recovery-deliverytables)
    - [2.23  Relationship Management Authorisations](#223-relationship-management-authorisations)
    - [2.24  Request for Transfer of Funds](#224-request-for-transfer-of-funds)
    - [2.25  Soft Delivery](#225-soft-delivery)
    - [2.26  StaticProcessing Messages](#226-staticprocessing-messages)
    - [2.27  Straight Through Processing](#227-straight-through-processing)
    - [2.28  SWIFT2024 Rulebook Changes](#228-swift2024-rulebook-changes)
    - [2.29  SWIFT 2017 Rulebook Changes](#229-swift-2017-rulebook-changes)
    - [2.30  SWIFT 2018 Rulebook Changes](#230-swift-2018-rulebook-changes)
    - [2.31  SWIFT 2019 Rulebook Changes](#231-swift-2019-rulebook-changes)
    - [2.32  SWIFT 2020 Rulebook Changes](#232-swift-2020-rulebook-changes)
    - [2.33  SWIFT 2021 Rulebook Changes](#233-swift-2021-rulebook-changes)
    - [2.34  SWIFT MT Stop Delivery Service](#234-swift-mt-stop-delivery-service)
    - [2.35  Swift Security Program-Local Authentication](#235-swift-security-program-local-authentication)
    - [2.36  SwiftNet Interact MX Services](#236-swiftnet-interact-mx-services)
    - [2.37  TemplateFormat Printing](#237-templateformat-printing)
    - [2.38  Translation DeliveryMessages](#238-translation-deliverymessages)
    - [2.39  Unique End-to-End Transaction Reference](#239-unique-end-to-end-transaction-reference)
    - [2.40  Misc](#240-misc)
    - [2.41  Treasury Settlement](#241-treasury-settlement)
  - [Chapter 3: Customer_Output - DEMXTR](#chapter-3-customer_output---demxtr)
    - [Features in Customer_Output - DEMXTR](#features-in-customer_output---demxtr)
    - [3.1  SwiftNet Interact MX Services](#31-swiftnet-interact-mx-services)
    - [3.2  Generating Message Flow](#32-generating-message-flow)
    - [3.3  Misc](#33-misc)
    - [3.4  Transform messages to Payment](#34-transform-messages-to-payment)
    - [3.5  Translating Messages](#35-translating-messages)
  - [Chapter 4: Customer_Output - IX](#chapter-4-customer_output---ix)
    - [Features in Customer_Output - IX](#features-in-customer_output---ix)
    - [4.1  Archiving XML Statement Related Tables](#41-archiving-xml-statement-related-tables)
    - [4.2  Camt.53 and Camt.54 Statement Summary](#42-camt53-and-camt54-statement-summary)
    - [4.3  Camt Generation Process](#43-camt-generation-process)
    - [4.4  Camt XML Message Production](#44-camt-xml-message-production)
    - [4.5  Changes in Camt Processing to Improve Performance](#45-changes-in-camt-processing-to-improve-performance)
    - [4.6  Exception Handling of Camt Messages](#46-exception-handling-of-camt-messages)
    - [4.7  Generation of a Camt Message to Multiple Recipients](#47-generation-of-a-camt-message-to-multiple-recipients)
    - [4.8  Misc](#48-misc)
    - [4.9  User-Definable Content of the Camt Message](#49-user-definable-content-of-the-camt-message)
  - [Appendix A: Glossary of T24 Applications & Fields](#appendix-a-glossary-of-t24-applications-fields)
    - [Applications](#applications)
    - [Fields Referenced](#fields-referenced)
  - [Appendix B: Consolidated Field Reference](#appendix-b-consolidated-field-reference)
    - [Customer_Output - DE (DE)](#customer_output---de-de)
    - [Customer_Output - DEMXTR (DEMXTR)](#customer_output---demxtr-demxtr)
    - [Customer_Output - IX (IX)](#customer_output---ix-ix)

---


## Customer_Output Module Overview


This document provides comprehensive documentation for the **Customer_Output** module of Temenos Transact. It covers **4 sub-modules** with a total of **58 feature areas**.


### Sub-Module Summary


| # | Sub-Module | Code | Features | Description |
|---|-----------|------|----------|-------------|
| 1 | **Customer_Output - BE** | `BE` | 3 | Customer_Output - BE module of Temenos Transact |
| 2 | **Customer_Output - DE** | `DE` | 41 | Customer_Output - DE module of Temenos Transact |
| 3 | **Customer_Output - DEMXTR** | `DEMXTR` | 5 | Customer_Output - DEMXTR module of Temenos Transact |
| 4 | **Customer_Output - IX** | `IX` | 9 | Customer_Output - IX module of Temenos Transact |


### How to Use This Guide


Each feature in this document is organized into the following sections:

- 📖 **Introduction** — Overview and purpose of the feature
- ⚙️ **Configuration** — How to set up and configure the feature
- 🔧 **Working With** — Operational usage and field descriptions
- 📋 **Tasks** — Step-by-step procedures
- 📊 **Outputs** — Reports, enquiries, and generated outputs

Each feature includes a **Quick Reference Card** at the top with application names, key fields, prerequisites, and a summary. Appendices provide a full glossary, consolidated field tables, and end-to-end use-case scenarios.

---


## Chapter 1: Customer_Output - BE


Customer_Output - BE module of Temenos Transact


### Features in Customer_Output - BE


| # | Feature | Sections |
|---|---------|----------|
| 1.1 | Alert Processing | Confi |
| 1.2 | Business Events | Confi, Tasks |
| 1.3 | Misc | Tasks |


### 1.1  Alert Processing


> **📇 Quick Reference Card**
> 
> **Sections:** ⚙️ Configuration


#### ⚙️ Configuration

You can generate alert requests based on the customer role.

It is possible to configure an event for multiple customers with different conditions.

If you post 2000 as the debit amount, then the both Event conditions will be satisfied.

The system triggers the AA.ARRANGEMENT.ACTIVITY for the above Funds Transfer.

The system updates the Event list file with the two Events under the FT transaction reference.

The system updates the Event log with the both Alert request references.

After running the EVENT service, the system changes the Event status to HANDOFF and generates the delivery references for both the Events.

The system generates the alert for the customer 300840.

The system generates the alert for the customer 10.

After the alert subscription, the system updates the arrangement with the details of the customer 300840 displaying the allowed role.

The system updates the arrangement record with the customer details.

You can post the FT as shown in the below screenshot.

As a result, the system triggers the Event only for the customer 300840.

The system does not triggers the Event for customer 10.

---


### 1.2  Business Events


> **📇 Quick Reference Card**
> 
> **Sections:** ⚙️ Configuration | 📋 Tasks


#### ⚙️ Configuration

This section explains the architecture of business events.


##### Parameters for Defining an Event

Business Events architecture has the following two parameter tables for defining an Event:

EB.EVENT.TYPE is the touchpoint between the actual event happening in Temenos Transact and the TEC.ITEMS configuration. Temenos Transact Model Bank supplies several touchpoints which indicates the occurrence of an event.

Most of the touchpoints are instances where a table gets updated. But there are some touchpoints, which are not triggered from the table update.

Direct Debit, Standing Order Executions and Failures.

When an EB.EVENT.TYPE is called, the instruction is delivered from this event type with an EB.ACTIVITY value. This is linked to an EB.ADVICES record, which is linked to the DE.MESSAGE functionality.

This table handles both technical alerts, which are the errors in processing and business alerts, which is the information for customers and account officers about business events.

It is likely that the overall touchpoint is too high-level to be of use for determining an event.

User does not wants to know every time a record changes but needs to know when a particular field on that record changes.

Using TEC.ITEMS , banks can fine-tune the nature of the event based on the requirement. An event can be generated every time a touchpoint , EB.EVENT.TYPE is triggered but possibly under specific circumstances. Users can subscribe to these fine-tuned circumstances. TEC.ITEMS clarifies the nature of the Event through the following settings:

- Subscriber This setting indicates that the medium the alert is sent when an event occurs. Model Bank comes configured with the functionality to communicate this over the DELIVERY system. In future, other subscribers such as Process Workflow or a Business Activity Monitoring mechanism also be included.
- Event Type This setting describes the underlying touchpoint and it is set in the EVENT.TYPE field.
- Subscription Type This setting describes the type of subscription whether this is monitored by customer or accounts officer or both of them and is it a mandatory field for everyone. This is set in the SUBSCRIPTION.LEVEL field. There are queries in Model Bank and validation to ensure that the internal subscribers such as account officers cannot subscribe to external events and vice-versa.
- Field Level Specification This setting is the main source of events such as where an event relates to entry into a Temenos Transact table and what sort of checking the system should perform to ascertain whether an event has taken place. Events are related to an update to the ACCOUNT table, so update to ACCOUNT is a touchpoint but different events are derived from this. It depends on whether it is WORKING.BALANCE or ACCOUNT.INACTIVE or even CURR.NO fields on account. Following are the additional considerations: An event occurs depending on the updates to two or more fields. An event is triggered if the WORKING.BALANCE field changes and the CATEGORY.CODE is in 1000–1999 range. Operands : Event functionality compares new values with old values to determine whether an event has occurred. Therefore, along with the usual operands such as greater than, less than, begins with, ends with, equals, does not equal, is/is not in the range of and so on, there are also comparative operands such as changed, changed from and changed to. If the EVENT.TYPE is based on a table, the same table should be entered in the TABLE field . An event is also defined by a KEYWORD . At times, it is impossible to determine whether an event has happened purely by looking at the fields and their values. An event being raised during the following scenarios: A record is reversed so the event based on FUNCTION is used. A particular VERSION is used. After the FIRST authorizer (not necessarily the final authorizer). A particular CHANNEL is used so an event occurs if channel A is used but not channel B. A particular APPLICATION is used. For the above requirements, Keywords are used rather than a specific table. Following are the Keywords allowed: - !APPLICATION (Application) - !V$FUNCTION (Function) - !PGM.VERSION (Version of the Application) - !CHANNEL (Channel defined in ofs.source ) - !AUTH.NO (Number of Authorizers)

Following are the parameters in TEC.ITEMS:

Events themselves have subscribers such as Customer or Account Officer as variables, which determine whether the event has happened. These are set in INHERIT field within the FIELD.TYPE – INHERIT multivalue set.

A customer prefers to receive an alert for an event when their working balance falls below 500, another customer prefers to receive only when the working balance falls below 100.

Some events take priority over others. These ars set in the PRECEDENCE field.

There is an event to alert the customer when the balance falls below 100 and another event, which alerts the customer when the overdraft limit is exceeded. In this case, the customer only receive the second alert if a single transaction triggers both alerts.

Some events occurs only once, such events are specified in the ONE.TIME.SUB field.

A customer prefers to receive an alert when a cheque book is issued or a loan is authorized. Once this happens, the alert is issued, the event should automatically be

, as it is unnecessary and inefficient for the customer to unsubscribe it.

Each TEC.ITEMS is classified with a severity level. It is used for information or reporting purposes and is used to determine the alert carrier.

TEC.ITEMS can be turned on or off for all subscribers through a STATUS field. When it is set to Inactive , then the TEC.ITEMS is not triggered.


##### Defining an Event

Procedure

1. Identify or configure the message that should be sent in EB.ADVICES and EB.ACTIVITY .
2. Identify the touchpoint behind the event and ensure that it has the correct message specified.
3. Create the TEC.ITEMS , specifying the touchpoint and the additional specifications to identify when an event is triggered.
4. After configuring the event, test the event by creating EB.ALERT.REQUEST to subscribe to the above TEC.ITEMS record, which includes any variables that need to be entered due to the INHERIT flag being set on TEC.ITEMS .
5. Update Temenos Transact to trigger the EB.ALERT.REQUEST .
6. Review the EVENT.LOG files to confirm that an alert is triggered in line with the configuration.

> **⚠️ Note:** You must run the relevant services for processing the events to generate alerts.


#### 📋 Tasks

Business events are a mechanism through which the customer or an account officer receives notification for any update or change made by the customer or bank.

Configuring Business Events

Grouping of similar events into a group is called as an Event Type or a Pattern of event. This section guides you in configuring a business event.

Subscribing to Business Events

This section explains who can subscribe to events and how to subscribe to an event.

Delivery

This section describes the delivery process when an alert is triggered.

Business Events Services

This sections explains the services associated with Business Events.

TEC Subscribers

This section explains the TEC subscribers.

Role Based Subscription

You can subscribe alerts to a customer and generate events based on the customer role.

---


### 1.3  Misc


> **📇 Quick Reference Card**
> 
> **Sections:** 📋 Tasks


#### 📋 Tasks

Customers and accounts officers can subscribe to receive alerts or events instantly. This section explains you how business events and alerts are processed to customer and account officer.

Business Events

Business events are a mechanism through which the customer or an account officer receives notification for any update or change made by the customer or bank.

---


---


## Chapter 2: Customer_Output - DE


Customer_Output - DE module of Temenos Transact


### Features in Customer_Output - DE


| # | Feature | Sections |
|---|---------|----------|
| 2.1 | BIC Database Upload | Intro, Confi, Tasks, Outpu |
| 2.2 | Contact Preferences | Intro, Confi, Tasks, Outpu |
| 2.3 | Customer Address in Delivery Output | Intro, Confi, Worki, Tasks, Outpu |
| 2.4 | DefiningPrintFormat | Intro, Confi, Worki, Tasks, Outpu |
| 2.5 | DeliveryasMicroserviceEvents | Intro, Confi, Worki, Tasks, Outpu |
| 2.6 | Detailed workflow Outward Delivery Messages | Intro, Confi, Worki, Tasks, Outpu |
| 2.7 | DetailedWorkflow InwardDeliveryMessages | Intro, Confi, Worki, Tasks, Outpu |
| 2.8 | Diverting SWIFT MT Messages | Intro, Confi, Worki, Tasks, Outpu |
| 2.9 | Email SMS Secure Messaging | Intro, Confi, Worki, Tasks, Outpu |
| 2.10 | Emitting Delivery Messages to Event Store | Intro, Confi, Worki, Tasks, Outpu |
| 2.11 | EndPeriodProcessing | Intro, Confi, Worki, Tasks, Outpu |
| 2.12 | Financial Messaging | Intro, Confi, Worki, Tasks, Outpu |
| 2.13 | Free Format Messages | Intro, Confi, Tasks, Outpu |
| 2.14 | Generation of MX Message using ISOMX Carrier | Intro, Confi, Worki, Tasks, Outpu |
| 2.15 | Generic Delivery Interface | Intro, Confi, Worki, Tasks, Outpu |
| 2.16 | Hold OutputDelivery Carriers | Intro, Confi, Worki, Tasks, Outpu |
| 2.17 | Interbank Statement Request | Intro, Confi, Tasks, Outpu |
| 2.18 | Interim Intraday Transaction Report | Intro, Confi, Tasks, Outpu |
| 2.19 | InwardDeliveryMessageProcessing | Intro, Confi, Worki, Tasks, Outpu |
| 2.20 | Misc | Intro |
| 2.21 | Mx Message FW | Intro, Confi, Worki, Tasks, Outpu |
| 2.22 | Recovery DeliveryTables | Intro, Confi, Worki, Tasks, Outpu |
| 2.23 | Relationship Management Authorisations | Intro, Confi, Worki, Tasks, Outpu |
| 2.24 | Request for Transfer of Funds | Intro, Confi, Tasks, Outpu |
| 2.25 | Soft Delivery | Intro, Confi, Tasks, Outpu |
| 2.26 | StaticProcessing Messages | Intro, Confi, Worki, Tasks, Outpu |
| 2.27 | Straight Through Processing | Intro, Confi, Worki, Tasks, Outpu |
| 2.28 | SWIFT2024 Rulebook Changes | Intro, Confi, Tasks, Outpu |
| 2.29 | SWIFT 2017 Rulebook Changes | Intro, Confi, Worki, Tasks, Outpu |
| 2.30 | SWIFT 2018 Rulebook Changes | Intro, Confi, Worki, Tasks, Outpu |
| 2.31 | SWIFT 2019 Rulebook Changes | Intro, Confi, Worki, Tasks, Outpu |
| 2.32 | SWIFT 2020 Rulebook Changes | Intro, Confi, Worki, Tasks, Outpu |
| 2.33 | SWIFT 2021 Rulebook Changes | Intro, Confi, Worki, Tasks, Outpu |
| 2.34 | SWIFT MT Stop Delivery Service | Intro, Confi, Worki, Tasks, Outpu |
| 2.35 | Swift Security Program-Local Authentication | Intro, Confi, Worki, Tasks, Outpu |
| 2.36 | SwiftNet Interact MX Services | Intro, Confi, Tasks, Outpu |
| 2.37 | TemplateFormat Printing | Intro |
| 2.38 | Translation DeliveryMessages | Intro, Confi, Worki, Tasks, Outpu |
| 2.39 | Unique End-to-End Transaction Reference | Intro, Confi, Worki, Tasks, Outpu |
| 2.40 | Misc | Intro |
| 2.41 | Treasury Settlement | Worki |


### 2.1  BIC Database Upload


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Bank Directory Plus file must be downloaded from SWIFT. This file is uploaded into the Temenos Transact system and is accessible to all applications for verification. Series of applications are provided to facilitate the smooth transfer of this data from its native source into the Temenos Transa...*
> 
> **Key Fields:** *Coll Rem Bk*, *Mapping Api*, *Receiver Bank*, *Swift Auth Key*, *Validate Bic*, *Validate Sak*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The Bank Directory Plus file must be downloaded from SWIFT. This file is uploaded into the Temenos Transact system and is accessible to all applications for verification. Series of applications are provided to facilitate the smooth transfer of this data from its native source into the Temenos Transact system. The Temenos Transact applications will allow the setting of default parameters, generating an automatic ID, uploading of the database and maintaining new or existing records on the BIC file within the system.

> **⚠️ Note:** Every effort needs to be made to ensure that Temenos’ release instructions are current with the latest Bank Directory Plus product, it is always advisable to read the instructions supplied with it, however unlikely, SWIFT may have included alterations without notice.


#### ⚙️ Configuration

This section explains the configuration of the BIC database upload feature.

The BICPlusIBAN program allows the export of data to a flat file using a TAB delimiter.

- Export the field names in the first row using the option in Bic Database Plus.
- Import this into excel and save as bicplus.txt (a TAB delimited file). This will add the extra TAB characters for the empty fields.
- Delete the first line containing the field names.

> **⚠️ Note:** Every effort is made to ensure that the Temenos Transact release instructions are in current with the latest BICPlusIBAN product. It is always advisable to read the instructions supplied with it, however unlikely, SWIFT may have included alterations without notice.

Once inside Temenos Transact , these records can be maintained or additional BIC records added. For example, it may be required to include branches that have not been released previously. A series of applications have been provided to facilitate the smooth transfer of this data from its native source into Temenos Transact . This allows the user to set the default parameters, automatic ID generation, action the upload of the database and maintain new or existing records in the BIC file within Temenos Transact .


##### DE.BIC.PARAMETER

The SYSTEM record in DE.BIC.PARAMETER holds the information used by the related DE.BIC and DE.BIC.LOAD applications.

- The Mapping Api field is optional and can contain a subroutine named as an alternative API call that the DE.BIC.LOAD routine can use to override the default formatting of records from the BIC database into Temenos Transact .
- Validate Bic is an optional field, which determines whether the BIC code entered has to be validated against the BIC codes (SWIFT address) available in the DE.BIC application. A BIC code can be entered in Temenos Transact applications in one of the following ways: As BIC code (like, in NETTING.AGREEMENT ) or Prefixed with SW (like in FUNDS.TRANSFER )

This field can be set to Yes to validate BIC codes entered in applications against the records in DE.BIC (where a BIC database is maintained). An error message is raised in case a non-existent BIC record is entered in a Temenos Transact application.

To raise an error message based on the above information after input of a BIC in applications, records in the DE.BIC application are checked as follows:

- When a BIC is entered as 11 characters (for example, bank, country, location and branch) the exact match record is checked.
- When a BIC is entered as eight characters (for example, bank, country and location), the first exact eight characters of the BIC are checked. If the exact match is not found, the given eight character BIC padded with XXX (default branch code), is checked against records in the DE.BIC application.

Validate Sak is an optional field in the DE.BIC.PARAMETER application which is used for validating the existence of a SWIFT key with the bank to whom the message is addressed. When it is set to Yes, a check is done when a SWIFT code is (BIC code prefixed with ‘SW-‘) used in the Receiver Bank and Coll Rem Bk fields in FUNDS.TRANSFER (FT) and the Receiver Bank field in STANDING.ORDER (STO). If Swift Auth Key is not in existence, then an override message is displayed during the creation of the FT and STO.

For the above functionality, the Swift Auth Key field in the DE.B IC application can be set to Yes to indicate the existence of the SWIFT key arrangement for the relevant BIC.


#### 📋 Tasks

There are no Tasks available for BIC Database Upload feature.


#### 📊 Outputs

There are no Outputs available for BIC Database Upload feature.

---


### 2.2  Contact Preferences


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Delivery module provides flexibility for the banks to send the advices or alerts to their customers either as a printed message or through various electronic carrier systems such as SWIFT, E-Mail and SMS. The Contact Preferences feature facilitates banks to capture the contact preferences of the...*
> 
> **Key Fields:** *Customer Number*, *Customer/Account Number*, *Pgm Autom Id*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The Delivery module provides flexibility for the banks to send the advices or alerts to their customers either as a printed message or through various electronic carrier systems such as SWIFT, E-Mail and SMS. The Contact Preferences feature facilitates banks to capture the contact preferences of their customers in the system. The Preferences cover the following attributes:

- Carrier through which the messages must be sent
- The address where the message has to be delivered (identified by the carrier and the address sequence number)
- Special format of the message
- Language definition
- Number of copies needed

The outward delivery message or alert for a customer will be processed based on the respective customer contact preferences as recorded in the system.


##### Account, Portfolio, Customer Level Contact Preferences

Contact preferences can be defined at the account, portfolio or customer level.

- Any alerts or messages generated for an account will be processed based on the account-level contact preferences.
- Any alerts or messages generated for the contracts underlying the portfolio will be processed based on the portfolio-level contact preferences, unless there are any contact preferences defined explicitly for the contract, that is, Account itself.
- Any alerts or messages generated for a customer will be processed based on the customer-level contact preferences, unless there are any contact preferences defined explicitly for the contract, that is, account or portfolio.


##### Contact Preferences for Other Recipients

The Delivery module allows the user to send an additional copy or redirect a customer delivery message or alert to other recipients, based on the preferences indicated by the primary customer. For example, while defining contact preferences for Customer A, it is also possible to indicate the preferences to send the output generated for Customer A to Customer B, in addition (as copies) or instead of sending to Customer A (output is sent to Customer B instead of A).


#### ⚙️ Configuration

The following features of the DE.CUSTOMER.PREFERENCES application are supported only for records with an auto-generated ID.

- Contact Preferences for Other Recipients
- Portfolio-Level Contact Preferences

Configure the DE.CUSTOMER.PREFERENCES application in the Pgm Autom Id field in the COMPANY application for all applicable company records as shown in the following screenshot.

> **⚠️ Note:** It is possible to create records with ID as Customer Number or Account Number in the DE.CUSTOMER.PREFERENCES application with the above-mentioned configuration (the Pgm Autom Id field is set as DE.CUSTOMER.PREFERENCES ).


#### 📋 Tasks

Banks use DE.CUSTOMER.PREFERENCES as a front end tool to record customer mailing preferences. It has an inbuilt intelligence to create the appropriate DE.PRODUCT records, based on the preferences defined by the customer, which will be used to format the delivery messages.


##### Workflow

In Contact Preferences, the user can perform the below activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Customer Delivery Preferences . |
| Find Customer | Enter a value in the Customer Number field. Click the FIND button. |
| List of Customer Preferences | Click the New deal icon. |
| Customer ID | Enter values in the below fields: Message Group Carrier Required Address Format Language Click the Validate icon to check for errors and overrides. Click the Commit icon. |

| SCREENS | WORKFLOW |
|---|---|
|  | Customer Delivery Products . |
| Find Customer | Enter a value in the Customer/Account Number field. Click the FIND button. |
| Customer/Product Delivery Conditions | Click the New icon to a create record. |
| Delivery Product | Enter values in the below fields: Carrier Language Format Copies Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to Contact Preferences in the core banking system.


##### Enquiries and Reports

This section allows the user to view the below enquiries and reports:

Customer Delivery Address Links

This enquiry displays the list of delivery product and deliver preferences linked to customer delivery address based customer's company level. Further drill-down of the enquiry allows the user to view delivery product and delivery preferences in detail.

Customer Delivery Preferences

This enquiry displays the details of customer preferences with operation mode to self or extended to others.

Customer Delivery Product

This enquiry displays the details of delivery product, such as, address, copies, language, message group and so on.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


### 2.3  Customer Address in Delivery Output


> **📇 Quick Reference Card**
> 
> **Purpose:** *The content of the customer address is configurable by defining rules. The system allows the Country Model Bank or implementations layers to define the rules that describe how the system handles the addresses in the delivery output.*
> 
> **Key Fields:** *Address Attribute*, *Address Country*, *Api Output Format*, *Apply Address Rules*, *Building Name*, *Building Number*, *Carrier Type*, *Country* ... +27 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The content of the customer address is configurable by defining rules. The system allows the Country Model Bank or implementations layers to define the rules that describe how the system handles the addresses in the delivery output.

> **⚠️ Note:** The address output rules feature is optional for existing and new customers (banks).


#### ⚙️ Configuration

The following parameters and applications are updated to support this feature:

- ADDRESS.OUTPUT.FORMAT – Allows the banks to describe the address output format.
- ADRESS.OUTPUT.RULES – Allows the banks to define the output address format that are used for the address country.
- COUNTRY.PARAMETER – Allows the bank to decide if they should apply the address output rules and to indicate the default output rules that are used when output rules are not defined for a specific country and delivery address type.

| Field | Description |  |  |  |  |  |  |
|---|---|---|---|---|---|---|---|
| ID | Represents the identification ID of the address output format. |  |  |  |  |  |  |
| Description | Specifies the description of address output format. |  |  |  |  |  |  |
| Output Item | Identifies an output component and it can have one or more lines. This is a multi-value field and has sub values. The logic applied (rules) on how the system handles the output item is described below: By giving the same name to the Output Item field to different output items, the system evaluates the first output line and if this is null it continues with the next one. Different output item names implies that each output item is included in the address output. The output item number/value given by the bank user does not reflect the position a line has in the address. The position of a line in an address output is implied by the order in which the output items are defined into the address output format. The output items must be described top-down, in the order in which they must appear in the output. Example The below table shows the position of a line in the address output display. Attributes Address Output Display Length=15 Number of Lines Per Output Item=1 Address Attribute.1.1=BUILDINGNO=50 Address Attribute.1.2=STREET=Luliu Maniu Address Attribute.1.3=FLAT NO=502 50 Luliu Maniu Length=15 Number of Lines Per Output Item =2 Address Attribute.1.1=BUILDINGNO=50 Address Attribute.1.2=STREET=Luliu Maniu Address Attribute.1.3=FLAT NO=502 50 Luliu Maniu 502 | Attributes | Address Output Display | Length=15 Number of Lines Per Output Item=1 Address Attribute.1.1=BUILDINGNO=50 Address Attribute.1.2=STREET=Luliu Maniu Address Attribute.1.3=FLAT NO=502 | 50 Luliu Maniu | Length=15 Number of Lines Per Output Item =2 Address Attribute.1.1=BUILDINGNO=50 Address Attribute.1.2=STREET=Luliu Maniu Address Attribute.1.3=FLAT NO=502 | 50 Luliu Maniu 502 |
| Attributes | Address Output Display |  |  |  |  |  |  |
| Length=15 Number of Lines Per Output Item=1 Address Attribute.1.1=BUILDINGNO=50 Address Attribute.1.2=STREET=Luliu Maniu Address Attribute.1.3=FLAT NO=502 | 50 Luliu Maniu |  |  |  |  |  |  |
| Length=15 Number of Lines Per Output Item =2 Address Attribute.1.1=BUILDINGNO=50 Address Attribute.1.2=STREET=Luliu Maniu Address Attribute.1.3=FLAT NO=502 | 50 Luliu Maniu 502 |  |  |  |  |  |  |
| Address Attribute | Identifies a name or address attribute that is included in the Output Item field and is part of the output item group. This field is multi-value field allowing the user to include one or more name and address fields in the output. The logic applied (rules) on how the system handles the output item is described below: The DE.ADDRESS fields alone can be specified. Adding multiple address attributes within the same output item, implies that all the address attributes are combined together within the same output item (it applies the and logic) in the order specified by the user. Attributes that are combined together are separated by a space. |  |  |  |  |  |  |
| Prefix Text | Associated with the value given in Address Attribute and identifies the text to precede the address attribute. If the Address Attribute field is blank, then its prefix is not considered in the output. |  |  |  |  |  |  |
| Suffix Text | Associated with the value given in Address Attribute . It identifies the text to follow the address attribute. If the Address Attribute field is blank then its prefix is not considered in the output. |  |  |  |  |  |  |
| Max Length | 1, the system returns the first character up to max length for the first line and then continues with the output for the next lines. If the max line is exceeded the next chars are ignored. |  |  |  |  |  |  |
| No Lines Per Output Item | Represents the maximum number of lines to use for an output item (Output Item). The maximum number of lines per output item combined with the maximum number of characters per output item gives an indication of the name or address attributes to be displayed on each line in the output. If this field is left blank, the default value is 1. |  |  |  |  |  |  |
| Maximum Lines | Indicates the maximum lines to be entered for the respective address output, including all the output items. When applying this format to an address, if the system determines the output has more lines than the maximum lines defined here, then the system considers only the first maximum lines and the remaining lines are ignored. |  |  |  |  |  |  |
| Null Lines Allowed | Indicates if the system should include an output item which is evaluated as blank in the address output. The logic applied (rules) on how the system handles the output item is described below: If set to YES, the system does not remove the null output items. If set to NO or left blank, the system removes the null output items. |  |  |  |  |  |  |
| Api Output Format | Identifies the routine to be called by the system. It attaches a routine to implement more complex output format rules. |  |  |  |  |  |  |

| Field | Description |
|---|---|
| ID | Indicates the country code. |
| Description | Specifies the description of the address country output rule for a specific country for various carriers. |
| Carrier Type | Indicates the name of the carrier for which these rules are applied. It must be a defined carrier. This is a multi-value field and has sub values. The existing conversion can be mapped differently depending on the carrier type. |
| To Addr Output Fmt | Indicates the name and address output format applied to the address when the output is sent. It is part of the carrier group and refers to the ADDRESS.OUTPUT.FORMAT record. At least one of the To Addr Output Fmt and De Format Conversion fields must be populated. |
| De Format Conversion | Indicates a CUS conversion used in the delivery format. It is part of the carrier group and sub group with associated values. The CUS conversions are notations, which are used in the delivery formats to indicate that the customer’s address should be included in the output. The system provides a set of CUS conversions, which are hard coded rules and are carrier specific. For example, CUS*FULL. |
| Output Format | Specifies the name of the address output format, which is to be used by the delivery when the associated CUS conversion is indicated in a delivery format. It refers to a record in ADDRESS.OUTPUT.FORMAT . |
| Unstruct Addr Default Format | Identifies an unstructured address output format. |

| Field | Description |
|---|---|
| Carrier Type | Indicates the name of the carrier for which the default output rules are defined. |
| Default To Addr Out Fmt | Indicates the default address output format, which is applied to the address where the output is sent. |
| De Format Conversion | This field is part of the carrier group, sub-group with the associated values. It identifies the output format that is used when a conversion is indicated in the delivery format for the defined carrier. |
| Default Output Fmt | Indicates the default address output format, which is used by delivery when this conversion is indicated in a delivery format. It refers to a record in ADDRESS.OUTPUT.FORMAT . |
| Unstruct Addr Default Format | Identifies an unstructured address output format. |


#### 🔧 Working With

This section explains the address format in output and the API for formatting it.

The following logic determines the address output rules for generating delivery messages:

1. When the Address Country field is not captured in the DE.ADDRESS application, the system does not apply any output address rules. The output is generated according to the existing delivery functionality.
2. When the Address Country field is captured in the DE.ADDRESS application, the system first checks if the address output rules must be applied when a message is delivered to a customer: If the Apply Address Rules field is blank in the COUNTRY.PARAMETER application, then the address output formats are not used and the output is generated based on the existing functionality. If the Apply Address Rules field is set to Yes in the COUNTRY.PARAMETER application for the current company, then the system uses the following logic to determine the address output rule that is to be applied: If address output rule is not defined for the Address Country field, then the system uses the default rules defined in the COUNTRY.PARAMETER application. If the address output rule is defined for the Address Country field and if a setup for the delivery carrier is not defined, then the system checks if there is any default address output defined in the COUNTRY.PARAMETER application. The following scenarios can occur: The Default Output Fmt field is defined for the 'To Address' and 'De Format' outputs, then the default output format applies and takes precedence over the existing functionality. The Default To Addr Out Fmt field is not defined for a specific carrier, the existing functionality is used. If the address output rule is defined for the Address Country field, and the respective carrier for the 'To Address' and 'De Format' address output formats, then the customised or soft address output rules apply for the respective delivery carrier and takes precedence over the existing functionality. If there are only 'To Address' output format address rules assigned for the respective carrier, then the soft address output rules apply for the 'De Format' output. The following scenarios can occur: The default 'De Format' output format rules apply, if it is defined in the COUNTRY.PARAMETER application. The current output format rules apply, if default 'De Format' output format rules are not defined. If there are only 'De Format' address output rules assigned for the respective carrier, then the soft address output rules apply and for the 'To Address' output format, the following scenarios can occur: The default 'To Address' output format rules apply, if these are defined in the COUNTRY.PARAMETER application. The current output format rules apply, if default 'To Address' output is not defined. The difference between the 'To Address' and 'De Format' outputs is described below. The 'To Address' output format is used to format the specific PRINT delivery address to which the output is sent (like, PRINT.1 and PRINT2). This is the address in the HEADER section. The 'De Format' is used to format the customer main or additional address (PRINT.1), when this is included in the content of the output.

The processing of how the output rules are defined and what is the address output based on the output rule configuration is shown in the below screenshot. The bank user defines an output rule for Italy, which is used when a delivery message is sent to the address of correspondence of the customer.

The bank user introduces the below address attributes for the corresponded record in DE.ADDRESS records. The different output variations based on the Maximum Lines and Null Lines Allowed fields are shown below.

The address API (routine) allows the caller to indicate a delivery address and returns the formatted message. The getFormatedAddressAPI routine accepts a delivery address and optionally a CUS conversion.

- If the CUS conversion is present, it determines and applies the Output Format field value for the respective carrier and conversion, based on the configuration in the ADDRESS.OUTPUT.RULE and COUNTRY.PARAMETER applications.
- If CUS conversion is not supplied, the API determines and applies the To Addr Output Fmt field value for the respective carrier, based on configuration in the ADDRESS.OUTPUT.RULE and COUNTRY.PARAMETER applications.
- If the delivery address is not found, an error message is returned.

The getCustomerAddressOutput API, which is used by Temenos business applications (such as Temenos Payments Hub (TPH) and Payment Orders) and other external channels, retrieves and returns the customer main address in a structured and/or unstructured format. This API is also exposed as an IRIS API.

The end point URL is /v2.0.0/party/customers/{customerId}/addressOutput , where {customerId} value can be replaced with any existing customer for whom the address needs to be returned.

The API receives the following details:

- The customer number.
- Address option – Structured, Unstructured or Both. This is an optional input. If not provided, Structured is considered as the default option.
- Address output format – Optional.

The API returns the following details:

- Structured Address – If the Address option is Structured or Both. Structured address will contain an array with information for the following fields: Department , Sub Department , Street Name , Building Number , Building Name , Floor , Po Box Number , Flat , Post Code , Town Name , Town Location Name , District Name , Country Subdivision , Address Country and Country .
- Unstructured Address – If the Address option is Unstructured or Both.

The Unstructured Address will be formatted as follows:

- If an address output format is supplied by the business application, the Unstructured Address will be formatted using the supplied format, provided the supplied address format is configured in Temenos Transact, else it will return an error to indicate that the supplied format does not exist.
- If an address output format is not supplied by the business application and if the output address rules defined in the COUNTRY.PARAMETER application are configured to be applied:
- If the Address Option parameter is Both or Unstructured and Unstruct Addr Default Format is not defined either in ADDRESS.OUTPUT.RULES or in COUNTRY.PARAMETER , the API will return an error indicating that: No format is defined for the Unstructured Address.
- If an address output format is not supplied by the business application, if the output address rules defined in COUNTRY.PARAMETER are configured not to be applied and the address option supplied by the business application is Both or NULL, only the structured address will be returned.
- If an address output format is not supplied by the business application, if the output address rules defined in COUNTRY.PARAMETER are configured not to be applied and the address option supplied by the business application is Unstructured, the API will return an error because the unstructured address will be applicable only when the Apply Address Rules field in COUNTRY.PARAMETER is selected.


#### 📋 Tasks

Related topics:

- Amend Customer Details

The content of the customer address is configurable by defining rules. The system allows the Country Model Bank or implementations layers to define the rules that describe how the system handles the addresses in the delivery output.


##### Workflow

The user can process theCustomer Address in Delivery Output by using the below workflow:

| SCREENS | WORKFLOW |
|---|---|
|  | Additional address of the customer . |
| Customer Address-Print Swift Add. | Enter a value in the Customer field and then click the FIND icon. |
| Address List | Select the Add Print Address option from the drop-down and then click the Launch icon. |
| Input Customer Address | Enter values in the following fields and address details of the customer against respective fields. Address Type Address Country Short Name Full Name Click the Validate icon to check for errors and overrides. Click the Commit icon to submit the record. |


#### 📊 Outputs

There are no Outputs available for Customer Address in Delivery Output feature.

---


### 2.4  DefiningPrintFormat


> **📇 Quick Reference Card**
> 
> **Purpose:** *The DE.FORMAT.PRINT application holds the definitions for all printed messages in Delivery. This application is complicated due to the great flexibility offered by the print format definitions. The main methods and fields used in creating and amending the DE.FORMAT.PRINT records are described briefl...*
> 
> **Applications:** `,`, `CUSTOMER`, `DE`, `DE.ADDRESS`, `DE.FORM.TYPE`, `DE.FORMAT.PRINT`, `DE.I.HEADER`, `DE.MESSAGE` ... +11 more
> 
> **Key Fields:** *).*, *320.MM1030.20.FR*, *App Pde*, *Calculation*, *Cet*, *Complete*, *Cond*, *Confid* ... +40 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The DE.FORMAT.PRINT application holds the definitions for all printed messages in Delivery. This application is complicated due to the great flexibility offered by the print format definitions. The main methods and fields used in creating and amending the DE.FORMAT.PRINT records are described briefly in this section.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 🔧 Working With

The following fields in the DE.FORMAT.PRINT application aids in printing the formatted messages.


##### ID of Print Format

The ID of the DE.FORMAT.PRINT record is NNNN.AANNNN.NNN.AA, where:

- NNNN is the message type.
- AANNNN is the application format, which is either application code or numeric or application code followed by up to four numeric characters.
- NNN is the format version number.
- AA is the language.

If the message type is 320, the application format is MM1030, the format version is 20 and the language is FR, then the ID of

record is

.

The application format is passed from the banking application, which originally generated the message. The format version number is specified in the DE. PRODUCT record and determines the format to be used. Therefore, when assigning the ID, it must be decided whether the banking application invoking the message or the fields in the DE. PRODUCT ID (that is, the company code, customer number, account number, message type and application code), or both determines the format to be used.


##### Form Size

The size of the stationery to be used is determined first for creating a new print format layout. The Form T ype field in the DE.FORM.TYPE application specifies the name of the form type to be used. If this field is left blank, DEFUALT stationery is used. A record with Form Type as DEFALUT should exist in DE.FORM.TYPE .

This application describes the form width (number of characters), form depth (number of lines), the printer to be used and the special print attributes to be used for printing the report. The existing F orm T ypes should be used if possible, since the operator is asked to load different stationery (the form type name). However, if the operator has to load pre-printed stationery, a special form type should be specified, even if the form type dimensions are the same as other form types being used.

The following fields in the DE.FORMAT.PRINT record, that is, Line S to Page Overflow are multi-value associated fields and are used to describe what fields are to be printed, where they are printed and any special conversions, masks that should be used.


##### LINE(s)

The LINE(S) field specifies the number of lines down a page the item defined in Field Text should be printed. It contains either an explicit line number or the line number relative to the last item printed. Additionally, it is possible to specify the highest line number that this item may be printed on or the maximum number of lines to print. Fields or text to be printed must be defined in sequence, down the page.

This field contains:

1. Either: The line number (counting from one at the top of the page) on which to print. For example, 1 (print at the top of the page) or The relative line position that is the number of lines to move down the page from the last item printed. For example, +2 (miss one line after the last item and then print on next line).
2. '-'
3. Either: The highest line number to be used. For example, +1-55 (print on the next line, but not if line is 56 or higher). '+' and the maximum number of lines to be printed. For example, +0-+5 (print on the same line as the last item, then print subsequent multi or sub-values on the following lines, but do not print more than five lines).

Part 1 is always required but Parts 2 and 3 specified together are optional.

> **⚠️ Note:** When Part 1-a (in the above details) is used, it differs from Part 3-b as follows: ’+’ in 1-b specifies a displacement of the given number of lines from the previous field printed. ’+’ in 3-b specifies the maximum number of lines to be printed, not the maximum displacement from the previous field position.

| Line number | Description |
|---|---|
| 02 | Print on line two |
| +2 | Print two lines down from the last item printed (miss one line) |
| +0 | Print on the same line as the last item |
| 1-10 | Start printing on line one, put the next multi-value on line two and put the 10th value on line 10 .If more than 10 values exist, page overflow*** occurs |
| +2-55 | Start printing two lines down from the last item printed and do not print past line 55. If the previous item was printed on line 54 or more, this item overflows*** immediately to the next page |
| +4-+2 | Start printing four lines down from the last item printed and do not print more than two lines |

***If the number of multi-values or sub-values in a field exceeds the number of lines specified, then page overflow is required. If the Page Overflow field is set to NO, the message is placed in repair queue. If Page Overflow is set to Y and the item has overflowed, nothing else with a relative line position (that is, line number starts with ’+’) is printed on that page, unless it has the Heading field set to B or S.

| Field in DE.FORMAT.PRINT | Value |
|---|---|
| Line S | 3-55 |
| Field Text | AMOUNT |
| Line S | +2 |
| Field Text | TOTAL |

If AMOUNT needs to go beyond line 55, the page overflow occurs. If TOTAL, which has a relative line position, does not print until all the values of AMOUNT have been printed, even though TOTAL is allowed to be printed past line 55.


##### Indent

The Indent field specifies the position of the field across the page and is expressed as the number of characters across the page. This field contains a numeric value. Unless a Mask is specified, printing is justified and that the field is printed starting at the number of characters specified in the Indent field.

If the

field is set as 5, then the field or text is printed starting at the fifth character across the page.

All fields to be printed must be defined in the sequence down a page, but fields may be superimposed across a line, so that when one field is not present, another will be displayed.

When a field is positioned on a line, it starts from the character position defined in the Indent field, then regardless of the length of the field, the gap between the end of the field and the end of the print line is set to blanks. There is an advantage of a short field optionally used, overwrites a long field. But variables cannot be inserted into text. Fields can be printed on the same line as follows:

| Field in DE.FORMAT.PRINT | Value |
|---|---|
| Line S | 2 |
| Indent | 10 |
| Field Text | CUSTOMER NAME: |
| Line S | +0 |
| Indent | 25 |
| Field Text | CUSNAME |

The printed line is in the 'Customer name: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx' format. Where the multi-value or sub-value fields are specified as appearing on a group of lines, all other fields/ or text to be printed on these lines must be specified as appearing on the same group of lines, even though they contain only a single field.

| Field in DE.FORMAT.PRINT | Value |
|---|---|
| Line S | +2-+4 |
| Indent | 10 |
| Field Text | ADDRESS |
| Line S | +0-+4 |
| Indent | 60 |
| Field Text | DATE |


##### Heading

This field is used to control on which page a field or text is printed:

- If B is entered, the field or text is printed on all pages.
- If S is entered, the field or text is printed on all subsequent pages (that is, on all pages except the first).
- If it is left blank, the field or text is printed only once.


##### Multi

This field specifies whether the field contains:

- M means multi-values.
- S means sub-values.
- Blank means the field or text contains a single value.

If this field is left blank and the field does contain multi or sub-values, all values are printed alongside each other, separated by spaces. If the field contains a single value or is text, but this field is entered as M, then the field or text is printed on every line in a group of lines alongside the multi-value set.

| Field in DE.FORMAT.PRINT | Value |
|---|---|
| Line S | +2-+4 |
| Indent | 1 |
| Field Text | ADDRESS |
| Multi | M |
| Line S | +0-+4 |
| Indent | 10 |
| Field Text | ADDRESS |
| Multi | M |


##### Complete

This field specifies whether a set of sub-values in a multi-value field should be printed only if there is enough space on the current page to print all the sub-values together. This field is used only if the Multi field is set to S (sub-values). If there is not enough space, the sub-values are printed on the next page (if Page Overflow field is set to Y, otherwise the message is place in the repair queue). If enough space is not available to print all the sub-values together on a page, then printing begins on the current page.

If the Line S field is specified as +2+4 with the Complete field set to Y and the Page Overflow field set to Y.

Then, 1, 2 and 3 are always printed together, even if it is necessary to go onto the next page before printing. 1, 4 and 5 are printed together, even if it is necessary to go onto the next page before printing. 4, 6, 7, 8, 9 and 10 could never be printed together, since only 4 lines have been specified in the Line S) field. Therefore, 6 lines are printed on the current page with as many sub-values as possible, before printing the rest of the lines on the next page.


##### Field text

This field indicates what is actually to be printed at the position specified. It can contain:

- A field name, which must be defined in the corresponding DE.MESSAGE record.
- Text, contained in quotes, for example, 'Name'.
- A reserved word as follows: TOTAL.n – Where n is 1 to 9. Print formatting can maintain totals when printing amounts. Specifying a FIELD/"TEXT" of TOTAL.n causes the previously calculated total to be printed. PAGE.NO – Prints the current page number. DATE – Prints the current bank date. TIME – Prints the current time. TO.ADDRESS – The address to which the message is being sent, as specified in the To Address field in the DE.O.HEADER record. DELIVERY.REF – The delivery reference of the message being printed. &ATTIxxxxxx or &ATTRxxxxxx – If the message is destined for a printer which supports various graphics or character attributes (such as, bold or underlined), these facilities can be used within the delivery messages. The FIELD/"TEXT" field may contain a link to the PRINTER.ATTRIBUTES application (such as, &ATTIBOLD&). &ATTIxxxxxx specifies the initiation of the attribute and &ATTRxxxxxx specifies the resetting of the attribute. This is converted at printing time to an escape sequence to invoke the attribute for the printer concerned. The name of the attribute (BOLD in this example) is prefixed with the printer type from the PRINTER.ID application and is looked up on the PRINTER.ATTRIBUTES application. For example, LASERJET.BOLD. If the LASERJET.BOLD attribute is not defined, the control word (BOLD) is ignored. For example, LASERJET.BOLD. If the LASERJET.BOLD attribute is not defined, the control word (BOLD) is ignored. Such attribute control words may be inserted anywhere within the text of a message and be used and reset as many times, as required. They are not displayed on the screen when the message is viewed and is removed from the body of the message when it is written to history.


##### Conversion

This field specifies the special treatment of the field named in Field Text , as explained below:

If this field contains a company code or customer number, the name and address are retrieved from the DE.ADDRESS application. If the field contains neither a company code nor a customer number, it is assumed that it contains a name and an address. CUS must be followed by:

- Either *FULL to print the full address
- Or one of the following to print one line of the address: *SHORT.NAME *NAME.1 *NAME.2 *STREET.ADDRESS *TOWN.COUNTY *POST.CODE *COUNTRY

For example, CUS*TEXT*ORD.

The system prints the standard text from the ORD record in the DE.TRANSLATION application in the language of the receiving bank when the Confid Txt field in the CUSTOMER record is set to YES, otherwise the customer short name and address is printed. If the text in the DE.TRANSLATION is set to NO, then the text bypasses this conversion and uses the default method.

A conversion of table is used to specify a lookup of the DE.TRANSLATION application. If xxxx is entered, the field is prefixed with xxxx before the table lookup, otherwise the field is prefixed by SW before the DE.TRANSLATION application is accessed. The field is replaced with the translation code in the language.

- GBP Field contains GBP Conversion is specified as TABLE Text to be printed is found by looking up SWGBP in the DE.TRANSLATION application.
- CCY/GBP Field Conversion is specified as TABLE CCY/ Text to be printed is found by looking up CCY/GBP in the DE.TRANSLATION application.

If the field is a multi-value set and Conversion of TABLE xxxxxx is specified, only the values prefixed by ’:’ is looked up in the DE.TRANSLATION application (the prefix of ’:’ is removed before the lookup). This is so that multi-value fields can contain a mixture of fields, which should be translated and fields for which no translation is required.

| Value | Format | Description |
|---|---|---|
| DATE | DD MMM YYYY | Three letter month |
| DATE/F | DD MMMMMMMMM YYYY | Full month name |
| DATE/S | DD MM YY | Two digit month |
| DATE/US | MMM DD YYYY | Three letter month |
| DATE/F/US | MMMMMMMMM DD YYYY | Full month name |
| DATE/S/US | MM DD YY | Two digit month |
| DATE/U | Defaults from the value of the USER definition held on the DE.FORMAT.PRINT record in TSA.SERVICE . | As per USER or LANGUAGE , the definition of the Date Format field. |

Translates numbers into words in the appropriate language (for example, 22 is translated as twenty two). Large amounts require two lines, therefore the Multi field should be set as M.

The field or text specified is printed only if the formatted message is a copy, that is, the message has previously been successfully formatted for printing (possibly with a different To Address ). The disposition of the original printed message must be Formatted, WACK or ACK.

The field or text specified is printed only if the formatted message is a duplicate message, that is, the message is set as PDE (possible duplicate entry) in the DE.I.HEADER or DE.O.HEADER records ( Msg Pde field), as it has to be formatted twice or because the banking application which generated the message sets the App Pde header field .

A user-created subroutine to carry out customised conversions. The subroutine must exist in PGM.FILE with TYPE field as S. The leading @ character must be entered before the subroutine name or it is not recognised. The arguments used in calling the subroutine are:

- IN.FIELD - Unconverted data from calling routine.
- HEADER.REC - Dynamic variable containing current DE.I.HEADER or DE.O.HEADER records from calling routine.
- MV.NO - Current value number for carrier address (references to the DE.I.HEADER or DE.O.HEADER records) from calling routine.
- OUT.FIELD - Converted data from subroutine.
- ERROR.MSG - Text error message generated by subroutine. If this is not null on return from the subroutine, the calling program aborts the conversion and the message is placed in the repair queue.

This conversion prints the time as passed from the application and adds the Cet Time Diff field value after the time in the SWIFT format. The Cet Time Diff field is defined in the DE.PARM application.


##### Mask

This field controls the formatting of fields, as follows (n is 1 or more digits and x is 1 or more characters):

| Value | Description |
|---|---|
| Bn | Right adjust into a length of n by inserting blanks on the left |
| *n | Right adjust into a length of n by inserting asterisks (*) on the left |
| Zn | Right adjust into a length of n by inserting zeros (0) on the left |
| , | Insert commas (,) to separate thousands |
| . | Change decimal points (.) to commas (,) |
| . , | Insert points (.) to separate thousands and use a comma for decimals |
| , . | As above |
| - | Put the sign after the amount (the sign normally precedes the amount) |
| A | Print the absolute value (that is, without a sign) |
| D | Print DR after the amount, if it is negative |
| C | Print CR after the amount, if it is positive and DR if negative |
| % | Print % after the data |
| 00x00x000x | Digits are substituted for the zeros. Any other characters are printed in the non-zero representations of the mask (that is, x represents 1 or more characters). For example, Field contains 123456, mask is 00-(00-00), the field is output as 12-(34-56) |

> **⚠️ Note:** More than one mask parameter can be specified, separated by a space. For example,"B10-,". However 00x00x000x may not be combined with other masking parameters.


##### Calculation

Various calculations are performed by DE.FORMAT.PRINT , it uses up to nine working fields. The contents of these working fields can be printed by specifying Field text of TOTAL.n, where n is 1 - 9. Calculation are performed by setting the this field to one of the following values:

| Value | Description |
|---|---|
| +,TOTAL.n | Add the contents of the field into TOTAL.n |
| -,TOTAL.n | Subtract the contents of the field from TOTAL.n |
| *,TOTAL.n | Multiply TOTAL.n by the contents of the field |
| /,TOTAL.n | Divide TOTAL.n by the contents of the field |
| ZERO | Zero the field after printing (may be used only if the FIELD/"TEXT" is set to TOTAL.n). |

> **⚠️ Note:** When multiplying or dividing, the first field determines the number of decimal places. This is not suitable for such purposes as calculating a local currency equivalent.


##### Dependent On

Specifies that the Field text is not to be printed if the field named in Dependent On field is blank or zero, or is only printed if the field named in Dependent On matches the condition specified in Dependent Operand and Dependent Cond fields . This field can contain any field in the message (it need not be one of the fields being printed) or the name of any field in the format record prefixed by '*' (that is, it must be a field being printed) or TOTAL.n. This field is generally used to prevent a heading from being printed when the associated data is not present.

| Value | Description |
|---|---|
| Field text | Payment Details |
| Dependent On | PAY DET |
| Field text | PAY DET |

In addition, a field or text can be printed depending on the value of the Dependent On field. The fields can only be compared to constants (and not to other fields).

| Field in DE.FORMAT.PRINT | Description |
|---|---|
| Line S | .10 |
| Indent | .35 |
| Field text | .AMOUNT |
| Dependent On | .AMOUNT |
| Depend Operand | .LT |
| Depend Cond | .0 |
| Line S | .10 |
| Indent | .50 |
| Field text | .AMOUNT |
| Dependent On | .AMOUNT |
| Depend Operand | .GE |
| Depend Cond | .0 |


##### Depend Operand

This field is used to specify how the Dependent On field is to be compared against the Depend Cond field in determining whether to print the Field text or not. This field contains the following values:

- Eq (Equal)
- Ne (Not equal)
- Lt (Less than)
- Le (Less than or equal)
- Gt (Greater than)
- Ge (Greater than or equal)


##### Depend Cond

This field specifies the constant value that the Dependent On field is to be compared against in determining whether to print the Field text or not.


##### Page Overflow

This field specifies whether a field is allowed to overflow onto the next page. If a field overflows a page and Page Overflow field is set to NO, the message is placed in the repair queue.


#### 📋 Tasks

There are no Tasks available for Defining Print Format feature.


#### 📊 Outputs

There are no Outputs available for Defining Print Format feature.


> **Related Applications:** `,`, `CUSTOMER`, `DE`, `DE.ADDRESS`, `DE.FORM.TYPE`, `DE.FORMAT.PRINT`, `DE.I.HEADER`, `DE.MESSAGE`, `DE.O.HEADER`, `DE.PARM`, `DE.TRANSLATION`, `LANGUAGE`, `PGM.FILE`, `PRINTER.ATTRIBUTES`, `PRINTER.ID`, `PRODUCT`, `TSA.SERVICE`, `USER`, `theDE.FORMAT.PRINT`

---


### 2.5  DeliveryasMicroserviceEvents


> **📇 Quick Reference Card**
> 
> **Purpose:** *Delivery (DE) module in Transact is enhanced with the ability to emit delivery messages or events to the Event Store microservice, which then can be consumed by Infinity or other external systems by configuring a dedicated delivery interface to the delivery carrier.*
> 
> **Key Fields:** *Ext Cust Id*, *Ext User Id*, *Out If Routine*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Delivery (DE) module in Transact is enhanced with the ability to emit delivery messages or events to the Event Store microservice, which then can be consumed by Infinity or other external systems by configuring a dedicated delivery interface to the delivery carrier.

This feature enables the bank administrator who may or may not have CUSTOMER record in Transact to raise an alert request the account/arrangement to which he is not associated at the Transact level.


#### ⚙️ Configuration

Transact provides a placeholder ( Ext User Id ) in EB.ALERT.REQUEST for the bank to specify the user id in the alert request. This is a free text field and the validations are done by the Infinity system when a subscription request is raised to Transact.

The alert engine should identify whether the alert has been subscribed by the user or customer based on the Ext User Id field. The following configurations are required to enable the DE module in Transact to pass the delivery message to the Event Store microservice.

The DE.INTERFACE application contains the details of the protocols for all interfaces which use the Generic Delivery interface. You need to configure a separate DE.INTERFACE as shown below to route the delivery message to event store.

The Out If Routine field should have the DE.EVENTSTORE.JSON.INTERFACE value, which is the routine released from the product for converting the delivery message into JSON format and push the event to Event Store microservice through the queue.

IF.OUT.ROUTINE receives the alert payload and uses the MS.BUILD.EVENT.JSON to form the json format. The following script shows the intern calling MS.BUILD.EVENT.JSON to form the json format and assign the constructed value to SYSTEM(5005).

The following JSON string is stored in Event store, which will be processed in microservices.

The delivery framework will pass the payload as key value pair of arrays. IF.OUT.ROUTINE will receive the alert payload and use MS.BUILD.EVENT.JSON to form the json format.


#### 🔧 Working With

When the alert is requested by the user, the alert message should be raised only to USER and not CUSTOMER of the arrangement. Hence, the system must pass Ext User Id and Ext Cust Id instead of customer with specific keyword EXT.USER.ID! EXT.CUST.ID to DE.PROCESS.ALERT, which is the subscription routine.

The delivery framework will pass the payload as key value pair of arrays. The system receives the alert payload from delivery system and use the MS.BUILD.EVENT.JSON to form the json format. The workflow is as follows:

OFS Request:

OFS Response:

The EVENT.LOG file is updated after posting Funds Transfer (FT).

The TEC.PROCESS.SUBSCRIPTION routine passes the external user value in the 8th argument position in the EXT.USER.ID! EXT.CUST.ID format.

1st event ALERT.REQUEST.ID : (-1) EBAR2010806143

In the DE.PROCESS.ALERTS routine, the 8th argument has external user values.


#### 📋 Tasks

There are no Tasks available for Delivery as Microservice Events feature.


#### 📊 Outputs

There are no Outputs available for Delivery as Microservice Events feature.

---


### 2.6  Detailed workflow Outward Delivery Messages


> **📇 Quick Reference Card**
> 
> **Purpose:** *The outward delivery messages generated by the Temenos Transact applications follow the flow shown below.*
> 
> **Applications:** `BATCH`, `DE`, `DE.ADDRESS`, `DE.BATCH.GROUP`, `DE.CARRIER`, `DE.FORMAT.PRINT`, `DE.FORMAT.SWIFT`, `DE.FORMAT.TELEXF` ... +26 more
> 
> **Key Fields:** *Ack*, *Application Format*, *Assoc*, *Basic header (1)-*, *Batching Req*, *Block*, *C*, *Carrier* ... +43 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The outward delivery messages generated by the Temenos Transact applications follow the flow shown below.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 🔧 Working With

This topic covers the detailed workflow of outward delivery messages.


##### Application Handoff

When an online transaction or overnight process requires to send messages, the APPLICATION.HANDOFF delivery process is invoked. This process simply puts the raw message data in the application without reformatting it. APPLICATION.HANDOFF gives each message a delivery message ID and passes this ID to the calling application, which places it in the application to provide an audit trail.

When a banking application needs to send a message, it passes the following data to APPLICATION.HANDOFF :

1. The ID (for example, 103.FT.1) to the required DE.MAPPING application: Message type Application Mapping sub-classification Sub-classification is used when a particular application calls the APPLICATION.HANDOFF for the same message type from different programs and supplies different record layouts to map the data from.
2. Between 1 - 9 records containing the data that are later mapped into the message detail and the DE.O.HEADER applications.
3. A field in which the delivery message reference generated by the delivery system is updated. This reference is passed back to the banking application, as an acknowledgement that the message was received by the delivery system.

The delivery message ID is composed in the XYYYYMMDDNNNNNSSSSSQQ format, where:

- X is the D message to be delivered (outward message).
- YYYYMMDD is the date.
- QQQQQ is the system user number of the inputter.
- SSSSS is the time in seconds, since midnight.
- QQ is the sequence number of the transactions within a second.

If a single transaction must send three different messages, then it has to make three calls to APPLICATION.HANDOFF , which provides three records of raw message data. Each of these records has the date and time it was created in the ID (as described above), and contains the mapping key followed by blocks of data (between 1 and 9).

A user-defined subroutine can be called within APPLICATION.HANDOFF , to enable the modification to the records to make additional information available to delivery. For example, to add fields to a record, to perform calculation for new fields. The routine is specified in the DE.MAPPING application in the Routine field.

The routine is passed in all nine APPLICATION.HANDOFF records in a dimensioned (DIM) array, as the first argument and a null in the second argument, which is used as a return error message. If there is a value in the second argument, on return from the routine the mapping does not proceed and the error message is handed back to the calling application.

If all the records are blanked by the call to the user routine, then the mapping process does not proceed and an error is returned to the calling application. The routine should be specified as EXAMPLE.ROUTINE (MAT EXAMPLE.REC, ERR.MSG).


##### Mapping

The mapping process, which is part of the interaction between the transaction and delivery, extracts the fields required in the message from the raw data that was passed to APPLICATION.HANDOFF by the banking applications. The message information is stored in the DE.MESSAGE application. Additionally, for each message, a DE.O.HEADER record is created for holding and controlling the information about the message. The messages are placed in the unformatted queue.

The raw data in a message contains up to nine blocks of data dumped from a program in the layout defined in that program. Different programs generating the same message type will produce different raw data, so each require a different record in the DE.MAPPING application for converting the data into the standard message detail and DE.I.HEADER or DE.O.HEADER records. The ID to be used for the mapping record is passed from the banking application.

The mapping process updates the fields in the DE.MESSAGE application in the positions that correspond to their definition in the DE.MESSAGE application.

The mapping ID is 103.FT.1. Therefore, the ID to the

application is 103. On the

application, the fifth value of field name is

. This means that, in the

record generated by the mapping process, the fifth field should be

. This does not normally concern the user, because the message contents cannot be viewed until they have been formatted for output.

The DE. MAPPING record also specifies which fields are used to update the DE.I.HEADER and DE.O.HEADER records created by this process. Fields in the header can be examined using DE.O.HEADER . Once the DE. MESSAGE and the DE.I.HEADER or DE.O.HEADER records are processed, the message is placed in the unformatted queue.

If there is a field in the originating contract that contains multiple customer numbers or addresses, then a copy of the message can be sent to each. If this is required, then the appropriate field has its Header Name field in DE.MAPPING updated with the value Multi Cust and any associated fields have the value Assoc Fld in their Header Name field.


##### Formatting

This section details the formatting options in the delivery system.

In the upgrade process, there may be a residue of messages in the older style to be transitioned through the various carriers until completed. For these the legacy system has been left in place. The new messages will go through the new Temenos Transact services path and then it becomes the standard method once the legacy queues have been cleared.

The DE.O.SELECT.NEXT.MESSAGE outward formatting message selects the messages for formatting in the order of priority. At this stage, the priority can only be specified within the banking application that generated the message or by a user amending the priority in the DE.O.HEADER record.

All Urgent (U) messages are processed first, followed by a set of Priority (P) messages, as specified in the Read Priority field in the SYSTEM.STATUS record of DE.PARM . Then the U queue is processed again, followed by the set of P messages. Once all U and P messages have been processed, a set number of Normal (N) priority messages are processed, as specified in the Read Normal field in the SYSTEM.STATUS record (in the DE.PARAM ). This order of processing the messages ensures that U messages do not spend longer time than necessary in the unformatted queue.

If the Read Priority field is set to 10 and the Read Normal field is set to 5, the messages are processed as follows:

- All U messages are processed, then up to 10 P messages are processed.
- Any U messages which may have been added to the queue would then be processed, followed by up to 10 more P messages.
- If there are no more U or P messages, then 5 N messages would be processed, before the urgent and priority queues are re-examined.

At this stage, the messages are mapped and the carrier method is selected. Then, the Temenos Transact service for the carrier(s) are started and as the TSA . SERVICE is started the carrier queues are processed. If a DE.I.HEADER or DE.O.HEADER record contains an override carrier, this determines the formatting required and the DE. PRODUCT application is not read. This override carrier is the only carrier used with the following attributes:

- There is only one copy of the message
- The format is version 1
- The status, priority and language values are picked up during mapping.

However, normally a DE.I.HEADER or DE.O.HEADER record does not contain an override carrier, so the DE.PRODUCT application is read. If the relevant DE. PRODUCT record specifies that a message is to be sent by SWIFT, but the format record does not exist in the DE.FORMAT.SWIFT application, then the message is sent by TELEX. If the format record does not exist in the DE.FORMAT.TELEXF or DE.FORMAT.TELEXP applications, then the message is sent by print. If the print format record does not exist in the DE.FORMAT.PRINT application and a special language was requested, the print format in the base language is used. If a print format does not exist, the message is placed in the repair queue.

If a message is routed by a company level DE. PRODUCT record, the language of the customer is used in formatting, rather than the language on the DE. PRODUCT record, as the language of the customer is more relevant.

Although, a record may exist in the DE. PRODUCT application to send all messages to a particular customer by telex and print. If copies are not allowed for a particular message type, the C opies field in the DE.MESSAGE application is set to NO. The first carrier specified in the DE. PRODUCT record is used when the message is formatted.

After the DE. PRODUCT record is read (or override carrier is determined), the DE.I.HEADER or DE.O.HEADER records is expanded to include a multi-value set of data for each copy of the message. The D isposition field is set to FORMATTED and the individual message D isposition fields are now used to control the disposition of the message. The copy number of the message (that is, the offset in the multi-value set) is appended to the delivery ID, so that when the message copy is placed in a queue, it is apparent which message copy is being referred to. The format of delivery ID is XYYYYMMDDNNNNNSSSSSQQ.C, where C is the copy number.

Each message copy is processed in turn, before the next message is processed. For each message copy, the DE.ADDRESS application is accessed to determine the address to which the message should be sent.

> **⚠️ Note:** The DE. PRODUCT application and the DE.I.HEADER or DE.O.HEADER records can specify the carriers of TELEX, TELEXF and TELEXP which refers to the different ways of formatting. TELEX uses the DE.FORMAT.SWIFT application. TELEXF uses the DE.FORMAT.TELEXF application. TELEXP uses the DE.FORMAT.TELEXP application.

However, when the DE.ADDRESS application is looked up, the TELEX carrier is used, regardless of the way the message is formatted. All telex messages for a particular customer should be sent to the same telex number (different telex numbers can be specified by using different address numbers).

The appropriate formatting application is accessed to determine the formatting rules. The ID to the application are as follows:

- ID is NNNN.1.1, where NNNN is the message type.
- For example, if the message type is 320, the key is 320.1.1.

- ID is NNNN, where NNNN is the message type.
- For example, if the message type is 320, the key is 320.

- ID is NNNN.AANNNN.NNN.AA, where: NNNN is the message type. AANNNN is the application format, which is either application code or numeric or application code, followed by four (up to) numeric characters. NNN is the format version number. AA is the language.
- For example, if the message type is 320, the application format is MM1030, the format version 20 and the language FR. The key is 320.MM1030.20.FR.

The field attributes held in DE.I.HEADER or DE.O.HEADER records are:

- The message type is held in the Message Type field in the DE.I.HEADER or DE.O.HEADER records and is part of the mapping key passed in APPLICATION.HANDOFF .
- The application format is held in the Application Format field in the DE.I.HEADER or DE.O.HEADER records and is passed from the banking application during mapping using the APP.FORMAT value, which defined in the Header Name field in the DE.MAPPING application.
- The format version number is held in Format field in the DE.I.HEADER or DE.O.HEADER record and is passed from the DE. PRODUCT application.
- The language is held in the Msg Language field in the DE.I.HEADER or DE.O.HEADER records and is either passed by the banking application or from the DE. PRODUCT application.
- If any errors occur during formatting, the message is placed in the repair queue, with the error message in the Msg Error Code field.
- If formatting is successful, the formatted message is placed in the formatted carrier application. For example, formatted SWIFT and formatted PRINT. However, there can be various exceptions, as follows: If a message is to be held. For example, if the message need not be sent out until business reopens in Tokyo and until the start of the next working day, the message can be placed in the HOLD queue. If the message is being sent by TELEX, the message might be specified as suitable for batching, in which case it is placed in the batching queue. Once a batch is complete, it is removed from the batching queue.


##### Batching

Telex messages for the same customer may (if desired) be grouped into batched messages. By batching the messages, the system reduces the cost of sending messages (by removing duplication of data) and also reduces the work of the customer to whom the messages are sent. If the telex messages needs to be batched, the Batching Req field in the SYSTEM.STATUS record in DE.PARAM must be set to Y. The messages are only batched as follows:

- Only messages of normal priority (N) are batched.
- Messages are batched in groups of the same addressee, the same currency, whether a test key is required or not and the same batch group.
- Only TELEXP messages (free format telex messages) are batched,

The batch groups are specified in the DE.BATCH.GROUP application. A batch group may contain more than one message type, but each message type may only exist in one batch group. If a message type does not exist in any batch group, then the messages of that message type are be batched.

If a message is to be batched, the batching queue is examined to check if there is a batch to which the message can be added. If there is a batch satisfying all the above criteria, the message is added to that batch. If there is not a batch, a new batch will be created, assigning the next available batch number. When there are ten messages in the batch, the batch is completed and removed from the batching queue and the messages are added to the formatted TELEX queue.

Batches may be completed manually (if desired), for example, just before COB in a particular country. In this case, there may be less than 10 messages in the batch and there may only be one message in the batch. To complete a batch manually, the DE.MM.DISPLAY application is used to display the batching queue. To complete a batch, enter C (complete) beside the batch. The batch is removed from the batching queue and placed in the formatted TELEX queue.


##### Outward Carrier Control Processes

Although messages can be sent by different carriers, part of the processing of these messages are always the same. This process is explained in the below section to avoid repetition in the following carrier control sections. Once the messages have been correctly sent (that is, the acknowledgement is received), the following process is performed:

- The Msg Disposition field is updated as ACK.
- The message is removed from the awaiting acknowledgement queue (or formatted queue for print).
- A copy of the DE.I.HEADER or DE.O.HEADER records are written to the DE.O.HEADER.ARCH application.
- A copy of the formatted message is written to the HISTORY tables.

> **⚠️ Note:** The messages are stored in the HISTORY tables, so that a copy of the message is always accessible.

Some interfaces use the generic carrier service, rather than customised carrier control programs. All carriers are defined in the DE.CARRIER application, whether the generic interface is used ( Carrier Module field is set to GENERIC) or not ( Carrier Module field is set to SWIFT).

Although the generic carrier service can be used to process many different carriers, a separate service can be launched for each carrier.

The generic carrier control service processes the messages for the carrier specified. Each message processed placed to the interface routine specified in the INTERFACE record in the DE.INTERFACE application, and is handled accordingly. If ACKs are required ( Ack Required field is set to Y in DE.INTERFACE ), the message is placed in the awaiting acknowledgement queue. When the ACK is received (from the inward routine) or if ACKs are not required, the message is flagged as having been sent correctly and a copy of the formatted message is placed in the HISTORY tables.

If a NAK is received, the message is removed from the awaiting acknowledgement queue and placed in the repair queue. Incoming messages received from the inward interface routines are placed in the unformatted inward queue. When an acknowledgement received from SWIFT for outward messages, their output sequence number (OSN) is updated in the Osn No field in the DE.SENT.SWIFT application. The OSN is in the message header, it is a six digit number as available in Basic header (1)- field with position from 23 to 28.

Each carrier should have a TSA.SERVICE record, a BATCH record for outward, inward or both directions. For example, the system may have PRINT.OUT and SWIFT.OUT or SWIFT.IN records.

While sending the message out of the Temenos Transact system, there is a possibility that the communication with the interface goes down or some other abnormal termination occurs. In those cases, when generic processing is restarted, the message that was in the process of being sent during the previous process has to be re-sent first before normal processing starts. This is also handled by the CONTROL.LIST variable in batch process.

It has become a standard practice to use generic delivery for SWIFT processing, so where DE.O.CC.SWIFT is used for older systems, the Temenos Transact services will use the user-defined carrier names, for example, the SWIFT.OUT carrier control process if the DE.CARRIER has been called SWIFT.

SWIFT messages are sent to the SWIFT network from Temenos Transact through a SWIFT mainframe, such as an ST400 or SWIFT alliance systems. The SWIFT.OUT carrier control process, sends the SWIFT messages from Temenos Transact to the SWIFT mainframe and monitors the responses received from it.

Messages are sent by the SWIFT carrier control process. When the SWIFT mainframe receives the message, it performs integrity checking on the message, to ensure that the message is received correctly. If the message fails the integrity checking, an attempt is made to resend the message. If the integrity checking fails again, it is assumed that there is something wrong in the communication between Temenos Transact and the SWIFT mainframe, and the SWIFT carrier control process is terminated. The termination message is written to the Syslog file.

If the message is received by the SWIFT mainframe correctly, then the SWIFT mainframe user may be required to input and authorise a test key. Once the message is ready to send, the SWIFT mainframe sends the message to the SWIFT network. The SWIFT mainframe either receives an acknowledgement or a time out message after a standard period of time. The resulting ACK or NAK is sent to Temenos Transact through the DE.I.CC.SWIFT . Therefore, if the inward SWIFT messages are not processed by Temenos Transact , the DE.I.CC.SWIFT must always be run to receive the ACKs and NAKs for outward messages.

If DE.I.CC.SWIFT receives an ACK, the message is removed from the awaiting acknowledgement queue and the Msg Disposition field is updated to ACK. If a NAK is received, the message is removed from the awaiting acknowledgement queue and placed in the repair queue with the Msg Disposition field set to REPAIR.

SWIFT messages can be sent to/from, either the ST400 or alliance using the CASmf protocol. This is achieved using the generic delivery service agent.

The DE.PRINT carrier control process, send print formatted messages into the appropriate printer spool queues , which is controlled by the computer's operating system.

Messages are printed in company, customer and account sequence. Therefore, it may be possible to put adjacent messages into the same envelope. However, if both formatting and print carrier control are running simultaneously, the print carrier control process the messages faster than formatting. So, the messages could be printed in the same sequence as they were formatted in, which is usually date or time within priority. If the order of company, customer and account is required, the print carrier control could be started after formatting is completed. However, if large volumes of printout are expected, it is worth considering how long it will take to print all the messages, if print carrier control is only run once the formatting carrier control is completed.

The print carrier control is run as a service. Once the messages are placed in the spool queues, the Msg Disposition field is updated to ACK and the message is removed from the formatted queue.

> **⚠️ Note:** If the Hold Output in the DE.ADDRESS is set to Y, that is, all printed output for a customer for a particular address is to be held (for example, if the customer has no contact address but just comes into the bank on a regular basis to collect all correspondence). The messages are not spooled but instead are written to HOLD.CONTROL . The message is acknowledged (ACK) by delivery at this stage. When the customer comes in, all the messages and reports can be printed using PRINT.CUST.OUTPUT .


##### Summary of Outward Dispositions

The following is the list of outward message queue. It can be found depending on the value of D isposition and Msg D isposition field . The system does not take into account the unauthorised changes to these fields.

| Disposition | Msg Disposition | Queue |
|---|---|---|
| UNFORMATTED |  | Unformatted |
| SELECTED |  | Unformatted (being processed) |
| REPAIR |  | Repair |
| DELETED |  | Not in queue (History) |
| FORMATTED | REPAIR | Repair |
| FORMATTED | FORMATTED | Outward carrier control or Hold if status is resent |
| FORMATTED | BATCHING | Telex batching |
| FORMATTED | WACK | Awaiting acknowledgement |
| FORMATTED | WACK – REROUTED | Awaiting acknowledgement |
| FORMATTED | WACK – RESUBMITTED | Awaiting acknowledgement |
| FORMATTED | ACK | Not on a queue (History) |
| FORMATTED | ACK – REROUTED | Not on a queue (History) |
| FORMATTED | ACK – RESUBMITTED | Not on a queue (History) |
| FORMATTED | DELETED | Not on a queue (History) |
| FORMATTED | REROUTED | Not on a queue (History) |
| FORMATTED | RESUBMITTED | Not on a queue (History) |


##### User fields inDE.MESSAGEandDE.MAPPING

The user fields in DE.MESSAGE and DE.MAPPING applications, wherein the user can define their local setting in DE.MESSAGE and map them in the user fields of DE.MAPPING , and it can be used in the DE.FORMAT.SWIFT or DE.FORMAT.PRINT to generate the messages with their local setting.

When the records are changed in DE.MESSAGE and DE.MAPPING is copied during upgrading or installing a fix, it overwrites the system fields only and retains the existing user field details.

In DE.MAPPING , the system fields can also be mapped to user input position and the details are mapped to user position has the precedence over the system fields, and same is used in APPLICATION.HANDOFF .

If a bank wants to generate the MT103s from the FUNDS.TRANSFER (FT) application with tag 23B (bank operation code) using their local reference field and to achieve this, the following setup is done.

Step 1:

In DE.MESSAGE for record 103, add the user field as OPERATION.CODE and give the required field values like Length , Single or Multi and Mandatory . If it is mandatory, then the field should have a value in the APPLICATION.HANDOFF , otherwise message will go into repair.

Step 2:

In DE.MAPPING for record 103.FT.1, map the local reference field position of FT for Usr Fld Name field with value as OPERATION.CODE. Like the system fields, the mapping can be done directly from the application or from the application hand off position. If the user field is mandatory for message type, then the record will not be allowed to commit without a mapping for that field in DE.MAPPING .

In this example, the Local Ref field in FT (field 1.67.2) is mapped to Usr Fld Name field with value as OPERATION CODE.

Step 3:

In DE.FORMAT.SWIFT update the field name along with the tag detail for record 103.1.1.

The tag 23B is mapped to Field Name as OPERATION CODE that is defined in DE.MESSAGE and mapped in DE.MAPPING .

Step 4:

Now, enter the FT transaction with the local reference details for tag 23B. In this example, CRTS has been given in FT Local Ref field for tag 23B.

Step 5:

When MT103 message is generated, it has the tag 23B with the details as given in FT.

The user fields in DE.MESSAGE and DE.MAPPING are protected, any amended record released (as part of a patch or upgrade of Temenos Transact ) can overwrite the system fields but not the user ones. This means that local changes are not lost due to a small change to a system field.


##### User Header – Block 3 Details in Outward Swift Message

In outgoing swift messages the User Header - Block 3 may contain the user reference for a message. It is optional on user-to-user messages. In the User Header - Block 3 of SWIFT FIN message the following details can be given (optional):

| User Header Fields/Tags | Description | Content/Options |
|---|---|---|
| User Header Fields/Tags | Description | Content/Options |
| 103 | Fin Copy Service Code | 3!a |
| 113 | Banking Priority | 4!x |
| 108 | Message User Reference | 16x |
| 119 | Validation Flag | 8!c |
| 115 | Payment-Release-Information-Receiver | 32x |

Outgoing SWIFT messages that utilise the User Header - Block 3 details are generated using the below steps:

1. This is done by adding new fields names in DE.MESSAGE .
2. Mapping them in DE.MAPPING (perhaps to a Local Ref field).
3. Updating the User Block and User Field fields in the DE.FORMAT.SWIFT with the field required to update the appropriate SWIFT User Header Block field.
4. In DE.FORMAT.SWIFT application the User Block field accepts the following block names to correspond to the above SWIFT User Header - Block 3 fields. SERVICE.ID BNK.PRIORITY MUR VALID.FLAG PAY.REL.INF

That is, the system can automatically populate the value in Validation Flag field 119 in MT103 message-STP for 'MT103+' and REMIT in '103 Extend'. Read the Funds Transfer User Guide for more information on MT103 type.

While generating the SWIFT message, based on the modified mapping, the APPLICATION.HANDOFF is populated with the block details, which is then used while generating the outward swift message. For example, while generating an MT103, the bank wants to send payment release information receiver field 115 details. The details are captured in FUNDS.TRANSFER in a Local Ref field and in this case, it is Pay Rel Inf field. The setup required for the above example is as follows:

- Add a field name such as Pay Rel Inf Data in DE.MESSAGE for the message type 103.

- Map the field name with FT Local Ref field in DE.MAPPING for record 103.FT.1.

- In DE.FORMAT.SWIFT application for 103.1.1, add the User Block field as PAY.REL.INF and User Field as PAY.REL.INF.DATA.

- Now, input the FT with the local reference details and outward SWIFT message MT103’s. The User block header 3 has the details as given in FT Local Ref field.

- In the same way for other user block fields in user header, the details can be mapped and generated in outgoing MT103.

As explained above the result of the mapping of a Local Ref field has produced an update to the header block of the SWIFT message, in this case field 115.

> **⚠️ Note:** Although it is possible to update these fields, any validations performed by SWIFT on them must be observed, as they are not validated by Temenos Transact .


#### 📋 Tasks

There are no Tasks available for Outward Delivery Messages feature.


#### 📊 Outputs

There are no Outputs available for Outward Delivery Messages feature.


> **Related Applications:** `BATCH`, `DE`, `DE.ADDRESS`, `DE.BATCH.GROUP`, `DE.CARRIER`, `DE.FORMAT.PRINT`, `DE.FORMAT.SWIFT`, `DE.FORMAT.TELEXF`, `DE.FORMAT.TELEXP`, `DE.I.HEADER`, `DE.I.HEADERorDE.O.HEADER`, `DE.INTERFACE`, `DE.MAPPING`, `DE.MESSAGE`, `DE.MM.DISPLAY`, `DE.O.HEADER`, `DE.O.HEADER.ARCH`, `DE.PARAM`, `DE.PARM`, `DE.PRODUCT`, `DE.SENT.SWIFT`, `FUNDS.TRANSFER`, `HOLD.CONTROL`, `INTERFACE`, `MAPPING`, `MESSAGE`, `PRINT.CUST.OUTPUT`, `PRINT.OUT`, `PRODUCT`, `SERVICE`, `SWIFT.IN`, `SWIFT.OUT`, `TSA`, `TSA.SERVICE`

---


### 2.7  DetailedWorkflow InwardDeliveryMessages


> **📇 Quick Reference Card**
> 
> **Purpose:** *Inward messages can be processed by Temenos Transact , if they are in a format that Temenos Transact can decode. Inward messages can be the messages sent by other banks. SWIFT and telex messages can be decoded, if the format is described in the DE.FORMAT.TELEXF application. The DE.FORMAT.TELEXF appl...*
> 
> **Applications:** `BATCH`, `DE.CARRIER`, `DE.FORMAT.SWIFT`, `DE.FORMAT.TELEXF`, `DE.INTERFACE`, `DE.INWARD.ROUTING`, `DE.MESSAGE`, `DE.SENT.SWIFT` ... +2 more
> 
> **Key Fields:** *Basic Header (1)-*, *Carrier*, *Disposition*, *Module*, *Msg Disposition*, *No*, *Osn*, *field*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Inward messages can be processed by Temenos Transact , if they are in a format that Temenos Transact can decode. Inward messages can be the messages sent by other banks. SWIFT and telex messages can be decoded, if the format is described in the DE.FORMAT.TELEXF application. The DE.FORMAT.TELEXF application can be used to describe the inter-branch messages.


##### Flow of Incoming SWIFT Messages

The incoming SWIFT messages follow the flow shown below.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 🔧 Working With

This topic covers the detailed workflow of inward delivery messages.


##### Generic Carrier Control

Some interfaces use the generic carrier service, rather than customised carrier control programs. All carriers are defined in the DE.CARRIER application, whether the generic interface is used (the Carrier Module field is set to GENERIC OFS User Guide ) or not (the Carrier Module field is set to SWIFT).

Although, the generic carrier service can be used to process many different carriers, a separate service can be launched for each carrier.

The generic carrier control service processes the messages for the carrier specified. Each message processed is placed in the interface routine specified in the DE.INTERFACE record, and is handled accordingly. Incoming messages received from the inward interface routines are placed in the unformatted inward queue. When an acknowledgement received from SWIFT for outward messages, their output sequence number (OSN) is updated in the Osn No field in the DE.SENT.SWIFT application. The OSN is in the message header, it is a six digit number as available in Basic Header (1)- field with position from 23 to 28.

The DE.CC.GENERIC.OUT and DE.CC.GENERIC.IN services, for outward and inward messages, can be run online or automatically during the Close of Business (COB). If the user wants to segregate each carrier and have a service for each one, then new BATCH , TSA.SERVICE and TSA.WORKLOAD.PROFILE records must be created. The inward generic service works on the messages which are fed into the Temenos Transact system, by the interface. There are two sources in which the Temenos Transact system can receive messages for inward processing:

The first one is from the IN.IF.ROUTINE attached in the DE.INTERFACE application. This routine passes one message at a time in DE.CC.GENERIC, which runs in a loop until messages are not received. If this routine is attached in the service, the routine is called in a loop for about 20 items with some pause. So, there are 20 messages (approximately) received by the system. The information passed by IN.IF.ROUTINE is written into the DE.GEN.IN.WORK work file. The information includes the:

- Reference to the message.
- Actual message.
- DE.I.HEADER or DE.O.HEADER records.
- Code.
- Error message (if any).

The actual process routine reads all this information with the reference passed into the routine and processes the message normally. After the message is processed, the details in the work file are deleted.


##### SWIFT Carrier Control

Messages can be received in the SWIFT mainframe (for example, ST400) from the SWIFT network. In the SWIFT mainframe, it is possible to specify that particular message types should be directed to the mainframe on which Temenos Transact is running. If any message is received which should be sent to Temenos Transact , it is processed by the SWIFT.IN carrier control module. Since this module is required for processing the ACKs and NAKs to outward messages, it is always running if outward messages are sent.

When messages are sent from the SWIFT mainframe, integrity checking is performed to ensure that the message is correctly received by Temenos Transact . If the message fails the integrity checking, an attempt is made to resend the message. If the integrity checking fails again, it is assumed that there is something wrong in the communication between Temenos Transact and the SWIFT mainframe, and the SWIFT carrier control process is terminated. The termination message is written to the Syslog file.

> **⚠️ Note:** If a message is received from the SWIFT mainframe, it is placed in the inward unformatted queue.


##### Formatting

The DE.I.SELECT.NEXT.MESSAGE inward formatting process, takes the messages from the inward unformatted queue and uses the DE.FORMAT.SWIFT and DE.FORMAT.TELEXF applications to decode the messages. If there is a problem with the decoding, the message is placed on the inward repair queue. If the decoding is successful, the message is placed in the inward message queue for the appropriate banking application, as specified in the DE.MESSAGE record. The default application is Funds Transfer (FT). The DE.INWARD.ROUTING application is used to mark the messages for the attention of particular departments, depending on the values of selected fields in the DE.I.HEADER or DE.O.HEADER records.


##### Summary of Inward Dispositions

The following is the list of inward message queue. It can be found depending on the value of Disposition and Msg Disposition field s. The system does not take into account the unauthorised changes to these fields.

| Disposition | Queue |
|---|---|
| ATK | Awaiting test key verification |
| UNFORMATTED | Unformatted |
| SELECTED | Unformatted (being processed) |
| REPAIR | Repair |
| DELETED | Not on queue (history) |
| FORMATTED | Passed to the banking application and on history |


#### 📋 Tasks

There are no Tasks available for Inward Delivery Message feature.


#### 📊 Outputs

There are no Outputs available for Inward Delivery Message feature.


> **Related Applications:** `BATCH`, `DE.CARRIER`, `DE.FORMAT.SWIFT`, `DE.FORMAT.TELEXF`, `DE.INTERFACE`, `DE.INWARD.ROUTING`, `DE.MESSAGE`, `DE.SENT.SWIFT`, `TSA.SERVICE`, `TSA.WORKLOAD.PROFILE`

---


### 2.8  Diverting SWIFT MT Messages


> **📇 Quick Reference Card**
> 
> **Purpose:** *The bank may decide to send all the SWIFT statements (for example, for Nostro reconciliation). This functionality is achieved by using the SWIFT diversion processing.*
> 
> **Applications:** `DE`, `DE.PRODUCT`, `DE.SWIFT.DIVERSION`, `PRODUCT`
> 
> **Key Fields:** *Address*, *Allow*, *Carrier Addr No*, *Cust*, *Pass*, *Thru*, *Use*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The bank may decide to send all the SWIFT statements (for example, for Nostro reconciliation). This functionality is achieved by using the SWIFT diversion processing.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 🔧 Working With

Messages to be diverted are processed as normal SWIFT messages through to the carrier control stage. However, in the SWIFT carrier control program (SWIFT.OUT), instead sending the message to MT400, it is written to an application which can then be transferred by some other means, like, sent by tape or accessed by a program.

Messages to be diverted are defined in DE.SWIFT.DIVERSION . For each message type, the user can specify that messages for a particular SWIFT address which is to be diverted. The outgoing and incoming messages can be diverted. Incoming messages can be copied by setting the Allow Pass Thru field to YES.

To divert all statements to a nostro reconciliation package, the user can set up records for each of the message types concerned in the DE.SWIFT.DIVERSION application as shown below.

In the above example, all 950 messages for SWIFT address are to be diverted to NOSTRECS address. NOSTRECS is a dummy SWIFT address, which is used to control the diversion of the required messages.

For each customer for whom the messages are to be diverted has two SWIFT addresses:

- SWIFT.1 for normal SWIFT messages
- SWIFT.2 for diverted messages

When the SWIFT messages are diverted, the dummy SWIFT address are replaced with the real SWIFT address, if the Use Cust Address field is set to Y in the DE.SWIFT.DIVERSION application.

The DE. PRODUCT records should be set up to route 950 messages to SWIFT.2 in the Carrier Addr No field. All other messages should be sent to the SWIFT.1 address.

Alternatively, the DE.PRODUCT records can be created to generate two copies for 950 messages. The first copy to address SWIFT.1 and the second copy to address SWIFT.2 which is to be diverted.


#### 📋 Tasks

There are no Tasks available for Diverting SWIFT MT Messages feature.


#### 📊 Outputs

There are no Outputs available for Diverting SWIFT MT Messages feature.


> **Related Applications:** `DE`, `DE.PRODUCT`, `DE.SWIFT.DIVERSION`, `PRODUCT`

---


### 2.9  Email SMS Secure Messaging


> **📇 Quick Reference Card**
> 
> **Purpose:** *Temenos Transact allows Email and SMS as message carriers within the Delivery module, so that any existing message supported by the Delivery module can be additionally or singularly sent through Email and/or SMS. In addition, the secure messaging functionality integrated with the Delivery module can...*
> 
> **Applications:** `CUSTOMER`, `DE.ADDRESS`, `DE.CUSTOMER.PREFERENCES`, `DE.FORMAT.XML`, `DE.PARAM`, `DE.PARM`
> 
> **Key Fields:** *Customer No*, *Offset*, *Outward Carriers*, *Produce Schema*, *Secure Msg*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Temenos Transact allows Email and SMS as message carriers within the Delivery module, so that any existing message supported by the Delivery module can be additionally or singularly sent through Email and/or SMS. In addition, the secure messaging functionality integrated with the Delivery module can be linked. This enables the usage of standard message routing facilities to generate a secure message thereby ensuring that all customer messaging is configured and sent through a central utility.

For sending Email, SMS and secure messages, an extensible markup language (xml) format of the message should be generated and sent to the customer using the interface.


#### ⚙️ Configuration

The below topic covers the configuration required in Temenos Transact for generating and sending messages to the customer through Email, SMS, and Secure Messaging.


##### CUSTOMER

The Secure Msg field can be set to Y or N in the CUSTOMER application. If the Secure Msg field is set to Y in the CUSTOMER record, then a record is created or updated in the DE.ADDRESS application.


##### DE.ADDRESS

Although input is not allowed in DE.ADDRESS for Email, SMS and Secure Message, the records can be created or amended or deleted through the CUSTOMER application. The Customer No field holds the customer reference which is used to get the address for a secure message.

The option to give a start and end date for hold mail period is available in the DE.ADDRESS application, where the setup can be made if a customer wishes to stop receiving correspondences for a particular period. Also, options are provided for what needs to be done with the held correspondences after the end date is reached.

> **⚠️ Note:** DE.ADDRESS is automatically maintained if the DE.CUSTOMER.PREFERENCES application is used. It is recommended that DE.CUSTOMER.PREFERENCES application is used for capturing customer preferences and not DE.ADDRESS directly.


##### DE.PARAM

The carriers like EMAIL, SMS and SECUREMSG must be added in the Outward Carriers field in the DE.PARAM application.

The Offset field in DE.PARM is used to enter any offset period from Universal Standard Time (UST).


#### 🔧 Working With

This section explains the message carriers within the Delivery module.


##### Formatting XML Schema

The Produce Schema field in the DE.FORMAT.XML application is used to create schema. After reversing the created record, the corresponding schema produced is deleted.


##### Displaying the Product Schema

The Display De Schema (DISPLAY.DE.SCHEMA) enquiry is used to display the schema that is produced.


#### 📋 Tasks

There are no Tasks available for Email, SMS and Secure Messaging feature.


#### 📊 Outputs

There are no Outputs available for Email, SMS and Secure Messaging feature.


> **Related Applications:** `CUSTOMER`, `DE.ADDRESS`, `DE.CUSTOMER.PREFERENCES`, `DE.FORMAT.XML`, `DE.PARAM`, `DE.PARM`

---


### 2.10  Emitting Delivery Messages to Event Store


> **📇 Quick Reference Card**
> 
> **Purpose:** *Delivery messages or events can be sent to the Event Store microservice. These events can be consumed by Infinity products or any other external systems. This feature is supported only for generic delivery interfaces (Generic Carrier module) and Delivery Carrier with formatting module as XML.*
> 
> **Key Fields:** *Carrier Module*, *Format Module*, *Job Name*, *Out If Routine*, *Xml Transform Req*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Delivery messages or events can be sent to the Event Store microservice. These events can be consumed by Infinity products or any other external systems. This feature is supported only for generic delivery interfaces (Generic Carrier module) and Delivery Carrier with formatting module as XML.


#### ⚙️ Configuration

This section details the configuration required to enable the Delivery module in Temenos Transact to pass the delivery message to the Event Store microservice.


##### Configuring Delivery Interface

The DE.INTERFACE application contains the details of the protocols for all interfaces. To route the delivery message to the Event Store microservice, the bank must configure a dedicated DE.INTERFACE as shown in the following screenshot.

> **⚠️ Note:** The Out If Routine field must be configured with the DE.EVENTSTORE.JSON.INTERFACE routine, which is the routine released by the product for converting the delivery message into JSON format and pushing the events to the Event Store microservice through a queue.


##### Configuring Delivery Carrier

The DE.CARRIER application contains the details of all carriers available in the Delivery module. Configure a separate DE.CARRIER , as shown in the following screenshot, by linking the delivery interface.

> **⚠️ Note:** The Format Module field must be set to XML; the Carrier Module field must be to GENERIC; and the Xml Transform Req field must be set to Neutral. The user can also link the delivery interface EVENTSTOREINTERFACE to the existing Delivery Carriers like EMAIL, SMS or SECUREMSG. With this configuration, the system pushes the formatted EMAIL, SMS or SECUREMSG to the Event Store microservice.


##### Configuring Delivery Parameter

The DE.PARM application holds a number of parameters to control the processing of messages in the Delivery module. The SYSTEM.STATUS is the only record in this application. To enable the delivery carrier EVENTSTORE, the bank must add this to the list of carriers defined in DE.PARAM .

As applicable for any generic delivery interfaces, for the EVENTSTORE carrier, a TSA.SERVICE record and a BATCH record must be configured for outward processing as shown in the following screenshot. The Job Name field in the BATCH record must be set to DE.OUTWARD.


#### 🔧 Working With

The processing through the EVENTSTORE delivery carrier defined in the Configuring Emitting Delivery Messages to Event Store section is similar to any other generic carrier interfaces. For delivery carriers that are using the XML Formatting module, with the Xml Transform Req field set to Neutral (Read the Configuring Emitting Delivery Messages to Event Store section for more information), the messages are generated in a dynamic array format, that is, as name-value pairs rather than the standard XML format.

The formatted message holds three types of data:

- Event Details – Event details are similar to message headers. These details are available as a part of the message irrespective of the message type.
- Message Data – The message data section holds the data along with the field names as configured for the respective message type in the DE.FORMAT.XML record. For example, account number and available balance. This information can differ based on message types.
- Formatted Message – This section of data is applicable only for delivery carriers EMAIL, SMS or SECUREMSG, when the carriers are configured with delivery interface EVENTSTOREINTERFACE. In such case, the formatted message is passed as a BLOB of information to the event store.

| Parameter Name | Value |
|---|---|
| FROM | modelbank@temenos.com |
| TO | alertherman@gmail.com |
| REPLY-TO | modelbank@temenos.com |
| SUBJECT | "Alert notification - Account Overdrawn" |
| MESSAGE | "Message from Model Bank Dear MR. Retail User We have the following Alert notification for you : Account Overdrawn Account Number : *9737 Transaction Amount : USD10,000.00DR Transaction Date : 20 APR 2020 Account Balance : -35,749.38 " |

The EVENTSTOREINTERFACE delivery interface converts the above explained formatted message from dynamic array format to JSON format and posts this into the queue to be passed to the Event Store microservice.

The following screenshot shows a sample output of the message sent to the Event Store in JSON format for Carrier EVENTSTORE.

The following screenshot shows a sample output of the message sent to the Event Store in JSON format for Carrier EMAIL.

Read the Event Store Microservice section for more information.


#### 📋 Tasks

There are no Tasks available for Emitting Delivery Messages to Event Store feature.


#### 📊 Outputs

There are no Outputs available for Emitting Delivery Messages to Event Store feature.

---


### 2.11  EndPeriodProcessing


> **📇 Quick Reference Card**
> 
> **Purpose:** *The delivery end of period processing consolidates all statistical data. It clears the application of deleted, acknowledged and printed messages. The delivery end of period processing is independent of the Temenos Transact close of business (COB) and is run whenever required by the user.*
> 
> **Applications:** `BATCH`, `DE.MM.I.END.OF.PERIOD`, `DE.MM.O.END.OF.PERIOD`, `DE.MM.SYS.CLEAR`, `DE.O.HEADER`, `DE.PARM`
> 
> **Key Fields:** *Awack*, *Data*, *Disposition*, *Eop*, *Error Code*, *History*, *Maintain*, *Msg* ... +1 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The delivery end of period processing consolidates all statistical data. It clears the application of deleted, acknowledged and printed messages. The delivery end of period processing is independent of the Temenos Transact close of business (COB) and is run whenever required by the user.

> **⚠️ Note:** It is suggested to run the processing weekly. However, it is up to the user to decide when they find it best to run and how often to process.

Running the delivery end of period removes the messages, for which processing is complete and places them in the HISTORY tables. Therefore, regular running of end of period keeps the LIVE tables in a reasonable size and therefore improves the processing time within delivery.


#### ⚙️ Configuration

The end of period service means that the process can be run multi-threaded. The two services used are:

- DE.EOP.OUTWARD for outward messages
- DE.EOP.INWARD for inward messages

The Data field in the BATCH record for the DE.EOP.OUTWARD and DE.EOP.INWARD services can be used to give the purge date before which the archiving of records is required. The date format is YYYYMMDD. If this field is empty in the respective BATCH record, then the archiving is not performed.

> **⚠️ Note:** It is recommended to run both the services. However, if no inward messages are received by Temenos Transact , it is not necessary to run the inward end of period service.


#### 🔧 Working With

When the DE.EOP.OUTWARD and DE.EOP.INWARD services are run, the records older than the specified date in the Data field, and those records that are completed with the Msg Disposition values (as detailed below), are cleared from the relevant applications. The records are copied to the HISTORY tables, if Maintain History field is set in DE.PARM :

- DELETED
- REROUTED
- RESUBMITTED
- ACK
- ACK – RESUBMITTED
- ACK – REROUTED
- ACK – MANUALLY SENT

A report is generated listing any messages that are awaiting acknowledgement and still outstanding from the previous period if it is set to run. The Eop Awack Report field in DE.PARM indicates whether this report has to be generated or not. If it is left blank, the report is generated. If it is set to NO, it indicates that the report need not be generated.

The DE.AWAITING.ACKNOWLEDGEMENT report is produced by the DE.PRODUCE.AWACK.REPORT job.

Similar to the outward processing, for inward processing the DE.EOP.INWARD service is run to delete the completed records from the relevant applications. The DE.MM.O.END.OF.PERIOD and DE.MM.I.END.OF.PERIOD applications for end of period processing are obsolete.


##### Displaying History

The DE.MM.HISTORY.DISPLAY is used to view the messages that was removed from the LIVE tables and copied to the HISTORY tables. This can also be done using the Outgoing Message (OUTGOING.MSG) enquiry. The selection criteria is used as desired to drill down to display the individual message.

The results fetched based on the input criteria are displayed. To view the record, click the OUTGOING.MSG.DETS option.


##### Updating the Delivery Syslog

When an error occurs in any of the delivery processes, it is handled in either of the following ways:

- If the error is associated with a particular message, the error is reported in the Error Code or Msg Error Code fields in the DE.O.HEADER record and the message is placed in the repair queue.
- If the error is not associated with a particular message and since the error cannot be reported immediately to the application, the error is written to the delivery Syslog file.

The Log of Delivery System (DE.MM.SYS.DISP) enquiry lists the events in the log.

If the log is getting big in size and needs to be reduced, the user can delete the older entries using the DE.MM.SYS.CLEAR application in input mode to select a date before which any records are deleted.

Use the Verify function in the record, to run the log clearance.


##### Clear Handoff – DE.MM.CLEAR.HANDOFF

The DE.O.HANDOFF is an internal table which contains the raw message data passed from the applications to delivery.

The DE.MM.CLEAR.HANDOFF job is run under the Temenos Transact batch program control, from the batch process CUS.FILE.TIDY.UP during the start of day. The DE.MM.CLEAR.HANDOFF clear the IDs of the messages whose processing has been completed from the DE.O.HANDOFF table . It only clears the ID of the messages that have been removed from the LIVE tables by the end of period processing. The DE.MM.CLEAR.HANDOFF should be run as an ad hoc job and since the DE.O.HANDOFF table is used for recovery, this program should be run only after backups and once the end of period processing is successful.


#### 📋 Tasks

There are no Tasks available for End of Period Processing feature.


#### 📊 Outputs

There are no Outputs available for End of Period Processing feature.


> **Related Applications:** `BATCH`, `DE.MM.I.END.OF.PERIOD`, `DE.MM.O.END.OF.PERIOD`, `DE.MM.SYS.CLEAR`, `DE.O.HEADER`, `DE.PARM`

---


### 2.12  Financial Messaging


> **📇 Quick Reference Card**
> 
> **Purpose:** *Delivery supports the processing of inward and outward messages when an underlying transact application is involved. These can be MT or MX messages. A framework is built to support third-party API requests through the Financial Messaging system. These API requests can be in the form of MT or MX mess...*
> 
> **Key Fields:** *In Msg Post Method*, *In Msg Queue*, *Inward Ofs Rtn*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Delivery supports the processing of inward and outward messages when an underlying transact application is involved. These can be MT or MX messages. A framework is built to support third-party API requests through the Financial Messaging system. These API requests can be in the form of MT or MX messages (inward messages) or can result in the generation of MX or MT messages (outward messages).


#### ⚙️ Configuration

There are two types of messages in Temenos Transact:

- Inward messages – Messages that Temenos Transact receives.
- Outward messages – Messages that Temenos Transact generates.

If the message received is from a non-Temenos Transact system (an external bank or a third-party application) or the message generated is for a non-Temenos Transact system, no transaction occurs. The message is posted in the JMS queue until further action takes place.

> **⚠️ Note:** The JMS queue handles those Temenos Transact messages for which related applications are not involved.

| Column 1 | Column 2 |
|---|---|
| Field | Description |
| In Msg Post Method | This field specifies whether the inward message needs to be posted in the JMS queue or a Temenos Transact application. The allowed values are: • Internal – Each incoming inward message processes its respective transaction in Temenos Transact. For example, an incoming MT102 creates the related DE.I.HEADER and FUNDS.TRANSFER applications. • External – Inward messages are not processed and the related application is not created in Temenos Transact, but the messages are pushed into the JMS queue. Only a DE.I.HEADER record is generated for such messages. The default value for In Msg Post Method is Internal. |
| In Msg Queue | This field specifies the JMS queue to which the inward message is to be posted and is required when the post method is specified as External. It is not a mandatory field. |

| Column 1 | Column 2 |
|---|---|
| Records in Temenos Transact | SETR Message |
| EB.TABLE.DEFINITION | SETR01200104 |
| DE.MESSAGE | SETR01200104 |
| DE.MAPPING | SETR01200104.DE.1 |
| IF.EXIT.POINTS | SETR01200104.DE.1 |
| IF.INTEGRATION.FLOW.CATALOG | SubsOrdConf-SubsOrdConf |


#### 🔧 Working With

The delivery framework for both inward and outward messages has been improved to provide a supporting framework to the API requests. This is valid for both MT and MX messages.


##### Financial Messaging for Inward Messages

When a SWIFT or ISOMX request for a transaction (with inward message) is received by the Temenos Transact system, the system checks the value in the In Msg Post Method and In Msg Queue fields in the DE.MESSAGE application.

The workflow below is explained in the following table:

| Column 1 | Column 2 |
|---|---|
| Scenario | Result |
| Inward Ofs Rtn – Defined In Msg Post Method – Internal | DE.I.HEADER is generated. Transaction is processed. |
| Inward Ofs Rtn – Not Defined In Msg Post Method – Internal | DE.I.HEADER is generated with Repair status. Transaction is not processed. |
| In Msg Queue – Defined In Msg Post Method – External | DE.I.HEADER is generated. Message is pushed into the JMS queue defined in In Msg Queue . |
| In Msg Queue – Not Defined In Msg Post Method – External | DE.I.HEADER is generated with Repair Status. Message is not pushed anywhere since the JMS queue is not defined. |

When the In Msg Post Method field is set to Internal, the Temenos Transact system processes the inward message based on the routine defined in the Inward Ofs Rtn field and the related record is generated in DE.I.HEADER . The transaction for the inward message occurs and the related application is generated.

The In Msg Post Method is defined as Internal and an inward MT102 message is received by the delivery system. DE.MESSAGE processes this message by creating a record in DE.I.HEADER and a FUNDS.TRANSFER record is generated, thereby crediting the related account.

> **⚠️ Note:** If Inward Ofs Rtn is not defined, the record in DE.I.HEADER moves to Repair status and no transaction occurs and a FUNDS.TRANSFER record is not generated.

For message requests not formatted to Temenos Transact request format, the In Msg Post Method field in DE.MESSAGE is set to External. When the system receives a message request, the request is pushed into the JMS queue. These queues are defined in the In Msg Queue field in DE.MESSAGE .

A message request (MT or MX message) is received by the delivery system. The post method specified in DE.MESSAGE is External. The inward message is not processed and no transaction record is generated in Temenos Transact. Only a DE.I.HEADER record is generated for the message. The system sends the inward message to a queue defined in the In Msg Queue field.

> **⚠️ Note:** The name of the JMS queue must be defined in the In Msg Queue field, if the In Msg Post Method field is set to External. Otherwise, the record generated in DE.I.HEADER moves to Repair status.


##### Financial Messaging for Outward Messages

When the system needs to generate an outward message, Temenos Transact receives an API request for the corresponding application and the delivery system generates an MX message based on the MX framework configuration.


#### 📋 Tasks

There are no Tasks available for Financial Messaging feature.


#### 📊 Outputs

There are no Outputs available for Financial Messaging feature.

---


### 2.13  Free Format Messages


> **📇 Quick Reference Card**
> 
> **Purpose:** *Free format messages are created through the EB.FREE.MESSAGE application. The application also generates appropriate delivery messages. This applies to outward and inward messages, and it is possible to preview the message before sending it.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Free format messages are created through the EB.FREE.MESSAGE application. The application also generates appropriate delivery messages. This applies to outward and inward messages, and it is possible to preview the message before sending it.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

Miscellaneous Swift Messages helps to send, receive queries, answers, free format messages and cancellation requests.


##### Workflow

This section allows the user to perform the below activities:

This Screen allows the user to send the Free text messages for the inward or outward messages exchanged.

1. Send Free Format Messages MT199/ MT299/ MT999 .
2. In the Free Format Message tab, enter or select values in the below fields: Free message Type Receiver Customer Id Message Text
3. Click Validate icon to check for errors and overrides.
4. Click Commit icon to submit the record.

| SCREENS | WORKFLOW |
|---|---|
|  | Authorise/Delete MT199/MT299/MT999 . |
| Authorisation of Free messages | Click the Authorise icon of a corresponding record. |
| Free Format Messages | Click the Authorise icon to authorise the record. |


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to Free Format Messages in the core banking system.


##### Enquiries and Reports

Enquiries displays the authorised free messages, cancel messages, query messages and answer messages.

Free Messages

This enquiry displays the authorised free messages sent or received. Users can View Transaction and View Delivery reference for the respective records using drilldowns.

Queries/Answers

This enquiry displays the authorised Query or Answer and cancel the messages sent or received. Users can View Transaction and View Delivery reference for the respective records using drilldowns.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA

---


### 2.14  Generation of MX Message using ISOMX Carrier


> **📇 Quick Reference Card**
> 
> **Purpose:** *This functionality provides Business Applications a framework to forms the business message. The Business Applications hands off the message data to Delivery, Delivery maps the message and issues the details to the Integration Framework which applies the transformation to the final formal. The Deliv...*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

This functionality provides Business Applications a framework to forms the business message. The Business Applications hands off the message data to Delivery, Delivery maps the message and issues the details to the Integration Framework which applies the transformation to the final formal. The Delivery Carrier associated to this processing is ISOMX.

To use the full benefits of the Delivery Transformation layer and the capabilities to handle headers please consult the Support MX messages through SWIFTNet Interact services section.

ISO 20022 MX is a new message type expressed in XML syntax, which is more flexible and easier to implement than the previous generation of message types (MT). These message types are developed in accordance with the ISO 20022 standard.

The current syntax format is xxxx.nnn.aaa.bb, where:

- xxxx is an alphabetic code in four positions (fixed length) identifying the business process.
- nnn is an alphanumeric code in three positions (fixed length) identifying the message functionality.
- aaa is a numeric code in three positions (fixed length) identifying a particular flavour (variant) of message functionality.
- bb is a numeric code in two positions (fixed length) identifying the version.

TREA.001.001.02, where:

- TREA refers to Treasury.
- 001 refers to NDF opening (notification).
- 001 refers to the variant.
- 02 refers to the version message format, in this case, version 2 of NDF opening type.


##### SWIFT Standards for MX Messages

| MX Identifier | Description |
|---|---|
| acmt.xxx.xxx.xx | Account Management |
| admi.xxx.xxx.xx | Administration |
| camt.xxx.xxx.xx | Cash Management |
| defp.xxx.xxx.xx | Derivatives |
| pacs.xxx.xxx.xx | Payments Clearing and Settlement |
| pain.xxx.xxx.xx | Payments Initiation |
| reda.xxx.xxx.xx | Reference Data |
| seev.xxx.xxx.xx | Securities Events |
| semt.xxx.xxx.xx | Securities Management |
| sese.xxx.xxx.xx | Securities Settlement |
| setr.xxx.xxx.xx | Securities Trade |
| trea.xxx.xxx.xx | Treasury |
| tsmt.xxx.xxx.xx | Trade Services Management |


#### ⚙️ Configuration

The following applications enable the configuration and use of MX messages in Temenos Transact :


##### Delivery Carrier

If the ISOMX formatting module is defined as a carrier in DE.CARRIER , then it requires the MX product to be installed as a prerequisite in SPF.


##### Delivery Header

- The If Event Table Link and Mapping Key fields in the HEADER applications (such as DE.O.HEADER , DE.I.HEADER , DE.O.HEADER.ARCH and DE.I.HEADER.ARCH ) are used to store the ‘Link to IF.EVENT.INTERFACE.TABLE for the message’ and ‘Mapping key related to the message’, respectively.
- A mapping key is passed by business applications, which is used later for resubmissions and rerouting of MX messages.
- The ‘IF’ reference is stored to track the status of the message for MX carriers through enquiries.


##### Delivery Message

The V, VL and ML options in the Single Multi field (in DE.MESSAGE ) are used for MX type of messages in addition to S and M:

- V (multi-value)
- ML (M option with language support)
- VL (V option with language support)
- S (single value)
- M (combination of normal, multi and sub-value field possible)

> **⚠️ Note:** VL and ML options allow the translation of messages.


##### Delivery Product

- If the carrier address is ISOMX, the user can enter a value in the Copies field (in DE.PRODUCT ).
- Users can capture the Mdr Customer details for ISOMX carrier.
- The same carrier message is sent to multiple customers for the ISOMX carrier.


#### 🔧 Working With

This section explains the processing of MX messages and the MX delivery framework.


##### Runtime Processing of MX Messages

The runtime processing of MX messages occurs in two stages:

The data for MX messages is updated by the respective business application to the Application Handoff.

After the static delivery processing (based on the configurations for MX message), the data is built, formatted and emitted to the Integration Framework (IF) module for further processing. The dataflow diagram is shown below.

The data emitted to IF event is converted to IF extensible markup language (XML) format and pushed to external eXtensible stylesheet language transformations (XSLT) for the transformation to the target MX XML format. The dataflow diagram is shown below.


##### Understanding MX Delivery Framework

The configuration of parameter and the examples given in the following section helps to understand the MX delivery framework.

Follow the below steps to set up the parameters required to enable MX messages using delivery framework:

1. Set up the SYSTEM.STATUS record in DE.PARM to enable ISOMX. Update the details as shown in the following screenshot.
2. Setup the ISOMX record in DE.CARRIER with the following details.
3. Setup the address records for customer and company in DE.ADDRESS , where required (as shown in the screenshot below).
4. Setup DE.MESSAGE and DE.MAPPING . The DE.MESSAGE application is used to define variable names, which are allocated to data in data storage. These variables are mapped through DE.MAPPING , where each variable defined in the DE.MESSAGE record is allocated a position in DE.O.HANDOFF . Examples for these parameters are shown below: If any changes are required in the mandatory or non-mandatory tags in the above message (preceding screenshot), the DE.MESSAGE and DE.MAPPING records must be updated.
5. After this, catalog needs to be rebuilt to update the IF.INTEGRATION.FLOW.CATALOG application.

The DE.PRODUCT record can be created for a company, a customer or an account, which is used to select the carrier such as PRINT, SWIFT, or any other channel. Below is an example for parameter at the Customer level for ISO MX, where 100112 is the Customer ID.

- Update the value of Mx Instruction field to SESE in CUSTOMMER.SECURITY (Depository).
- Enter a transaction in the SEC.TRADE application for depository as shown in the following screenshot.
- The If Event Table Lin field in DE.O.HEADER has been updated. This is the reference ID for IF.EVENT.INTERFACE.TABLE.
- IF.EVENTS.INTERFACE.TABLE is updated with values to be passed in XML.
- Run INTEGRATION.SERVICE in TAFJEE or Execute Servlet.
- Transformation and Delivery status are updated in the IF.EVENTS.INTERFACE.TABLE .

> **⚠️ Note:** Event Data is truncated in the screenshot.

- Run the ISOMX.OUT service.
- The transformed XML is updated in DE.O.MSG.ISOMX. The view of the XML message from DBTOOLS is shown in the below screenshot.

- Validate the XML against the schema, as shown in the below screenshot.
- After the validation, the XML is generated as shown in the below screenshot.

- The system updates the Msg Disposition field (in DE.O.HEADER) to Ack, after the XML message is generated successfully. The DE.O.HEADER) to Ack, after the XML message is generated successfully. The DE.O.HEADER) application of the delivery message D20170919-59554-18620-02, is shown in the below screenshot

In this scenario, the user creates a position (a Security Trade ) for outward messages to be generated with Cash Hold Settle or sec hold set to YES, Broker to be on SEL Side and Broker Deliver Instruction set to FOP.

- Update the Process Mt548 In field to Yes for the company record (GB-001-0001) (COMPANY ID) in SC.PARAMETER .
- Create the MtchgSts/Mtchd record in SC.MT548.MATCH.CODE .
- Incoming setup in DE.MESSAGE is required for highlighted fields.
- Enter a SEC.TRADE as shown in the below screenshot.
- In SC.MT548.MATCH.QUEUE , a record is created with the ID of SEC.TRADE in IHLD status.
- Run the ISOMX service and ensure that MT540 is generated.
- Build an Inward XML message by entering in the necessary trade details.

- Ensure that the status shows ‘Validation of XML was SUCCESSFUL’.
- Retrieve the 'DE.I.HEADER - ID' by entering the specified commands (for admin or super users)

(or), use the View Delivery Messages enquiry to check the delivery message.

- Run the XML.IN service or run the ISO MX routine.

> **⚠️ Note:** The launching company should always be the Master Company for MX service, however, transactions can be routed to different companies according to the Inward OFS Routine attached in DE.MESSAGE .


#### 📋 Tasks

There are no Tasks available for Generation of MX Message using ISOMX Carrier feature.


#### 📊 Outputs

There are no Outputs available for Generation of MX Message using ISOMX Carrier feature.

---


### 2.15  Generic Delivery Interface


> **📇 Quick Reference Card**
> 
> **Purpose:** *Messages sent and received using the generic delivery interface follow the normal flow of messages in delivery. The sending and receiving of the messages is performed by the generic carrier control which determines whether the message should simply be written to a table or should be updated to a rou...*
> 
> **Applications:** `,`, `CREATE.FILES`, `DE.ADDRESS`, `DE.CARRIER`, `DE.CC.GENERIC`, `DE.FORMAT.SWIFT`, `DE.FORMAT.format.carrier`, `DE.INTERFACE` ... +5 more
> 
> **Key Fields:** *Ack Required*, *Audit Seq Checking*, *File Pathname*, *Out If Routine and In If Routine*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Messages sent and received using the generic delivery interface follow the normal flow of messages in delivery. The sending and receiving of the messages is performed by the generic carrier control which determines whether the message should simply be written to a table or should be updated to a routine.

The generic delivery interface is used to add a new interface. The DE.CARRIER application determines the number of messages formatted, which address records should be used and the interface required.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 🔧 Working With

This section details the necessary steps for adding a new interface through the generic delivery interface.


##### Adding a New Interface

If the bank wants to create an interface called GLOBUSTLX and if the messages should be sent to telex addresses in standard SWIFT format, the below steps must be followed:

Create a record named GLOBUSTLX in the DE.INTERFACE application. This application contains the details of the protocols used for the interface. If possible, these should be stored on the interface record, rather than being hard-coded in the program, so that options can be amended by the user (for example, line speed) and that the programming changes are not required if the protocol requirements change. The following fields are set as explained below.

All messages sent through the generic delivery interface are written to DE.O.MSG.GLOBUSTLX , which is an the interface message table (DE.O.MSG ). By default, this resides in the data area. However, it is possible to have this table residing on a different disk, or even on a disk mounted from a network server or PC, by specifying the pathname in the File Pathname field. This field is multi-valued, so that the pathname of the table for outward messages (DE.O.MSG ) can be specified and the pathname for the table for incoming messages (DE.O.MSG ) can be specified.

The interface routines can be written depending on whether the interface is to be interactive or batched. If the interface is to be interactive, then the interface routines are required. If the interface is to be batched, then the interface routines are not required.

An outward routine can be specified without an inward routine and vice versa.

Some interfaces do not send ACKs (positive acknowledgement) and NAKs (negative acknowledgement). Therefore, it is assumed that if the message was sent to the interface, the recipient received it correctly. If ACKs are not required, set the Ack Required field to N. As soon as the message is correctly handed to the interface routine or simply written to the interface application and if no interface routine is specified, then the message is updated as ACK and a copy of the formatted message is written to history. If ACKs are required, then the message is written to the awaiting acknowledgement queue. When the ACK is received, the message is removed from the awaiting acknowledgement queue and a copy of the formatted message is written to history. If a NAK is received, the message is removed from the awaiting acknowledgement queue and placed in the repair queue.

Normally for both outward and inward messages, the sequence number assigned to the message is checked by both Temenos Transact and the interface. This number is a five digit, sequential number. However, some interfaces may have their own numbering mechanism. For outward messages, Temenos Transact always assign the message sequence number. This number must be used if ACK or NAKs are sent by the interface back to delivery. For inward messages, the user can decide whether to use the six digit number or any numbering system of the user’s choice.

If the Audit Seq Checking field is set to Y, the delivery checks the sequence numbers in the normal way (that is, the number assigned is the next number expected, there is no un-archived message on the audit table). If this field is set to N, the delivery uses the number passed to it from the interface without any validation of the number or checking the audit table.

The LOCKING table normally contains the next expected number. However, for inward messages where the Audit Seq Checking field is set to N, the LOCKING record contains the last reference received, as the format of the IDs are unknown and it is not possible to increment it. The ID of the LOCKING record for the outward sequence number is OUT-carrier, where carrier is the ID of the DE.CARRIER record (for example, OUT-TELEX). For inward messages, the ID of the LOCKING record is IN-CARRIER (for example, IN-TELEX).

Specify two routines in the GLOBUSTLX.OUT interface record, to send outward messages. The GLOBUSTLX.IN receives the incoming messages and the ACKs and NAKs to the outward messages.

> **⚠️ Note:** If ACKs and NAKs cannot be received from the interface being used, Ack Required field can be set to N in the interface record, then the messages are marked as ACK as soon as they are handed to the outward routine. These routines does not update any delivery tables, as all of this processing is done in DE.CC.GENERIC carrier control program.

The interface to which the messages are to be sent are already decided. Now, the format of the body messages needs to be decided and the addresses to which they should be sent. This is done by defining a carrier record in DE.CARRIER . In the below example, although telex messages are sent, they are sent in standard SWIFT format. That is, the messages are formatted using the rules defined in DE.FORMAT.SWIFT . The messages are sent to telex addresses, that is, the carrier used to look-up addresses from DE.ADDRESS is TELEX (for example, US0010001.C-100017.TELEX.1).

When the record is authorised, the following file control records and files are created if it does not exist already:

- F.DE.O.MSG.Carrier
- F.DE.O.PRI.Carrier
- F.DE.O.MSG.Interface
- F.DE.I.MSG.Interface
- F.DE.SENT.Carrier

In this example, the following files are created:

- F.DE.O.MSG.TELEX
- F.DE.O.PRI.TELEX
- F.DE.O.MSG.GLOBUSTLX
- F.DE.I.MSG.GLOBUSTLX
- F.DE.SENT.TELEX

Setup telex address records for any customers to whom telex messages are to be sent.

Add the carrier to the list of valid carriers (OUT.CARRIERS) in DE.PARM , if it is not present already. Inward carriers need not be defined, as the same process handles both the inward and outward messages.

The messages to be sent through the new interface (GLOBUSTLX) are defined using the delivery system. The records in DE.PRODUCT are setup to route the messages for the required message types, for any customers who wish to receive telex messages.

The system is now setup to send messages through GLOBUSTLX.


##### Interactive Processing – Routine Specified

If a routine is specified, it is called from DE.CC.GENERIC when a message is ready to be sent. The program should be a data or basic routine with four arguments:

- Message sequence number
- Formatted message
- Dynamic array containing miscellaneous data
- Error message

GLOBUSTLX.OUT (MSG.NO,R.MSG,GENERIC.DATA,ERR.MSG):

- MSG.NO (message sequence number) - The message sequence number is a six digit sequence number used to identify the message. It is also used to check that the message received was the next one expected, if sequence number checking is required the set the Audit Seq Checking field to Y in DE.INTERFACE .
- R.MSG (formatted message) - The formatted message is the message as formatted by the formatting routine. The (DE.O.MSG ) is not updated, if OUT.IF.ROUTINE is specified. This application is reserved for the routine to control and use.
- GENERIC.DATA (dynamic array containing miscellaneous data) - This array contains additional information that can be passed between DE.CC.GENERIC and the outward routine. The layout of the array is described in the insert I_DE.GENERIC.DATA.
- ERR.MSG (error message) - The error message is null, when the interface routine is called. If an error message is passed back to DE.CC.GENERIC , the message is written to the repair queue and the error message is used to update the header record.

The interface program should add a header or trailer as required, convert the message (if necessary) and physically send the message, handling all the communications protocol. This can either be done in the data or basic routine. The routine can be a very simple data or basic program, executing a C program or VOC entry or shell script depending on the skill of the person developing the interface.

If an error message is not passed back to DE.CC.GENERIC , the message is placed in the awaiting acknowledgement queue. If ACKs are required (ACK.REQUIRED set to Y on DE.INTERFACE) and the MSG.DISPOSITION is set to WACK (awaiting acknowledgement) or history if ACKs are not required and the MSG.DISPOSITION set to ACK.

The inward routine, as specified in IN.IF.ROUTINE is called to check if there are any incoming messages or ACKs or NAKs to the outward messages. The inward routine is called with six arguments:

- Dynamic array containing miscellaneous data
- Message sequence number
- Type of message (ACK, NAK, MSG)
- Formatted message
- Delivery header record
- Error message

GLOBUSTLX.IN (GENERIC.DATA,MSG.NO,MSG.TYPE,R.MSG,MAT R.DE.HEADER,ERR.MSG):

- GENERIC DATA (dynamic array containing miscellaneous data) - This array contains additional information that can be passed between DE.CC.GENERIC and the inward routine. The layout of the array is described in the insert I_DE.GENERIC.DATA.
- MSG.NO (message sequence number) - The message sequence number is a six digit sequence number used to identify the message. It is also used to check that the message received was the next one expected, if sequence number checking is required (if Audit Seq Checking field is set to Y in DE.INTERFACE ). For ACKs or NAKs, it is the sequence number of the message, which the ACK or NAK relates to.
- MSG.TYPE (type of message) - The message type is ACK, NAK, or MSG, if the message is an incoming message.
- R.MSG (formatted message) - Message to be formatted by the inward formatting routine. This has to be in a format, which the inward formatting routine understands, which normally means that the header and trailer are removed.
- R.DE.HEADER (delivery header record) - Update any fields on the header record with any known information, that is, retrieved from the header or trailer (for example, FROM.ADDRESS).
- ERR.MSG (error message) - If the error message begins with STOP (regardless of the type of the message), the program will terminate. Apart from this, the error message is only used for NAKs, to indicate why a message was rejected.

If errors are not found in the message, it is placed in the inward delivery queue. If an error is found, the message is placed in the inward repair queue. For outward and inward routines, if the error message begins with STOP, the generic delivery carrier control program is terminated.


##### Batched Processing – No Routine Specified

If outward interface routine is not specified, the messages are simple placed in the (DE.O.MSG ) application. The ID of the message is the message sequence number, that is, a six digit sequential number. Depending on whether ACKs are required or not, the messages are either added to the awaiting acknowledgement queue or written to history.

To process the messages in (DE.O.MSG ) a procedure must be established. This can be as simple as a manual process to save the file to tape (for example, in tar format), an automated process to save the file to tape, which can either be run on-line from within Temenos Transact (for example, from a menu) or from within the Close of Business (COB), that is, a program called from within COB to batch the messages before sending them.

> **⚠️ Note:** Delivery does not delete the messages from (DE.O.MSG ). The messages should be deleted by the procedure handling these messages once they have been processed successfully, or by a routine called from the COB.

If an inward routine is not specified, messages in (DE.O.MSG ) are processed in sequential order. The ID of the record must be ACK.nnnnnn or NAK.nnnnnn for ACKs or NAKs to outward messages (where, nnnnnn is the message sequence number of the outward message); for inward message, if sequence number checking is required, the id must be a 6 digit sequential number or any characters if sequence checking is not required. For NAKs, the record should contain the reason why the message was unsuccessful.


##### Adding a New Formatting Routine

A new formatting routine might be added to send messages to a clearing interface, for example, BGC. In addition to the steps included in “Adding a new interface”, the user must perform the following steps

1. Specify the formatting rules by writing a program, DE.FORMAT.FORMAT.CARRIER, for example, DE.FORMAT.BGC, based on TEMPLATE. This program allows the user to input the formatting rules and validate them.
2. Create a PGM.FILE record for the program, a file control record for DE.FORMAT.format.carrier (specifying that $HIS and $NAU files are required) and run CREATE.FILES to create the new files.
3. Write the formatting program DE.O.FORMAT.format.carrier.MESSAGE, for example, DE.O.FORMAT.BGC.MESSAGE, to format the message based on the formatting rules specified in DE.FORMAT.format.carrier.


##### Adding a New Address Carrier

Special steps are not required to add addresses to DE.ADDRESS for a new carrier, apart from the fact that the carrier must be a valid carrier specified in DE.CARRIER . For example, the user can enter addresses for BGC without any additional code. The ID of the records are in the format of US0010001.C-100017.BGC.1. However, the user has to create a version of DE.ADDRESS , so that access is restricted to certain fields and additional validations are performed.


#### 📋 Tasks

There are no Tasks available for Generic Delivery Interface feature.


#### 📊 Outputs

There are no Outputs available for Generic Delivery Interface feature.


> **Related Applications:** `,`, `CREATE.FILES`, `DE.ADDRESS`, `DE.CARRIER`, `DE.CC.GENERIC`, `DE.FORMAT.SWIFT`, `DE.FORMAT.format.carrier`, `DE.INTERFACE`, `DE.O.MSG.GLOBUSTLX`, `DE.PARM`, `DE.PRODUCT`, `LOCKING`, `PGM.FILE`

---


### 2.16  Hold OutputDelivery Carriers


> **📇 Quick Reference Card**
> 
> **Purpose:** *The hold mail output is enabled for a carrier for the corresponding address.*
> 
> **Applications:** `DE.ADDRESS`, `DE.CARRIER`, `DE.CUSTOMER.PREFERENCES`, `DE.O.HEADER`
> 
> **Key Fields:** *Allow Hold*, *Hold End Date*, *Hold Mail End*, *Hold Mail Opt*, *Hold Mail Start*, *Hold Option*, *Hold Options*, *Hold Output* ... +2 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The hold mail output is enabled for a carrier for the corresponding address.


#### ⚙️ Configuration

The Allow Hold field in the DE.CARRIER application allows the bank to indicate if the hold output related fields can be manually entered or can be setup in DE.CUSTOMER.PREFERENCES and DE.ADDRESS records which are linked to the respective carrier. The possible options are Yes or NULL and the default option is NULL.


#### 🔧 Working With

The existing validations apply to the hold output related fields irrespective of the carrier:

- Hold Output – Allows the bank to indicate Yes or No.
- Hold Mail Start – This is optional and can only be set if Hold Output is Yes. A warning is displayed when the Hold Start Date is in the past.
- Hold Mail End – This is optional and can only be set if Hold Output is Yes. A warning is displayed when the Hold End Date is in the past. The Hold Start Date is mandatory when the Hold End Date is supplied. The Hold End Date must be greater or equal to the Hold Start Date .
- Hold Mail Opt – This field holds the following values: No mail – Indicates that the customer output should not be generated (no delivery message to the address). Held – Indicates that the delivery message to the address is generated on a hold status. This is the default option.

For each message a delivery header record is created with high level details for the respective message including the carrier addresses to which the correspondence is to be sent. If the following setup is done for a DE.ADDRESS record, then the correspondence sent to the address will be deleted.

- If the Hold Output field is set to Yes
- If the Hold Mail Start and Hold Mail End fields are blank
- If the Hold Mail Opt field is set to No mail.

As result of the above setup, the Msg Disposition field associated with the address is updated as Delete in the DE.O.HEADER application.

> **⚠️ Note:** This option is recommended to stop the output from being sent to a deleted address.

Alternately, if the following setup is done for a DE.ADDRESS record, then the correspondence sent to the address is put on hold and the message status for that particular carrier address in the DE.O.HEADER record is set to HOLD.

- If the Hold Mail Start and Hold Mail End fields are blank.
- If the Hold Option field is set to Held.

The HOLD status allows the copy for that particular carrier address to be manually deleted or resubmitted. This can also be used in some future cases, when there is a doubt that the customer might require the output later. However, this requires a manual decision to release or resubmit and it should not be used for large volumes of output as the system does not archive the output which is in hold till this is not deleted or released (sent).

The Hold List enquiry is launched to resubmit or delete the generated messages.

The applications used for resubmitting and deleting the listed hold records are shown in the below screenshots.

- If Hold Mail Start is less than the current business date and Hold End Date is greater than the current business date then: The correspondence to that address is deleted, if the Hold Mail Opt is set to No Mail in the DE.ADDRESS . That is, in DE.O.HEADER the Msg Disposition field associated with the address is set as Delete. The correspondence to that address is put on hold if the Hold Option is set to HOLD. That is, the message status for the particular carrier address in the DE.O.HEADER record is set as HOLD.
- If Hold Mail Start is greater than the current business date or the Hold Mail End is lesser than the current business date, then the delivery message follows the normal flow.

The Hold Options , that is, Clear and Send are available only for PRINT carriers and not for non-PRINT carriers.

The system evaluates all the DE.ADDRESS records which have the Hold Option set to Yes during close of business. If the Hold Mail End is less or equal to the closing business date, then the Hold Output is automatically set to No and Hold Mail Start , Hold Mail End and Hold Option are cleared.

The customer has requested to receive every communication, including the changes in the interest conditions to XML.1 and EMAIL.1 address.

Later on, the customer requests to delete the current correspondence address A as that property has been sold, however the customer does not provide a new physical address. The address A is stored in the DE.ADDRESS record named XML.1 where the Hold Output field is set as Yes and the Hold Mail Opt field is set to No mail. The customer EMAIL.1 address is still valid and is not changed.

The default Interest Condition Changes Advice product is setup to send a copy of the letter to the XML.1 address and another copy to the EMAIL.1 address.

The bank changes the interest conditions and this impacts one of the customer’s savings account. An advice message is triggered and a DE.O.HEADER record is created. This indicates that the copy of the letter which is for the XML.1 address is deleted but the copy sent to the EMAIL.1 address is sent.


#### 📋 Tasks

There are no Tasks available for Hold Output for Delivery Carriers feature.


#### 📊 Outputs

There are no Outputs available for Hold Output for Delivery Carriers feature.


> **Related Applications:** `DE.ADDRESS`, `DE.CARRIER`, `DE.CUSTOMER.PREFERENCES`, `DE.O.HEADER`

---


### 2.17  Interbank Statement Request


> **📇 Quick Reference Card**
> 
> **Purpose:** *Banks send a request message to their correspondent requesting information related to their accounts (or accounts maintained for their customers, where a prior agreement is in place).*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Banks send a request message to their correspondent requesting information related to their accounts (or accounts maintained for their customers, where a prior agreement is in place).

Incidentally an MT920 request message is sent to the account servicing institution to transmit one or more MT940 Customer Statements, MT941 Balance Report(s), MT942 Interim Transaction Report(s), or MT950 Statement Message(s) containing the latest information available for the account as identified in the message. This message has a multiple sequence consisting of account(s) for which the information and required message type(s) is requested. The MT920 message requires implementation of special procedures and its use is governed by bilateral agreements between correspondents.


#### ⚙️ Configuration

Covered as part of module configuration and there is no specific configuration for this feature.


#### 📋 Tasks

There are no Tasks available for Interbank Statement Requests feature.


#### 📊 Outputs

There are no Outputs available for Interbank Statement Requests feature.

---


### 2.18  Interim Intraday Transaction Report


> **📇 Quick Reference Card**
> 
> **Purpose:** *The interim transaction report (MT942) should contain detailed and summary information about the entries debited or credited to the account since:*
> 
> **Applications:** `DE.MT941.SENT.ENTRIES`, `DE.MT942.REQUEST`, `DE.MT942.SENT.ENTRIES`
> 
> **Key Fields:** *Cr Floor Limit*, *Gen942 Independently*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The interim transaction report (MT942) should contain detailed and summary information about the entries debited or credited to the account since:

- The last statement (MT940 or 950) or balance report (MT941) or
- The last interim transaction (MT942) report (sent in the period since the last statement or balance report).

The interim report can be generated manually on an ad hoc basis or automatically through the Temenos Transact service.

MT942 is an intra-day transaction report, which is used to transmit detailed information about entries debited or credited to the account since:

- The last statement or balance report.
- The last interim transaction report (sent in the period since the last statement or balance report).

MT941 and MT942 message types are not linked and therefore the statement for these message types is generated independently, that is, the entries to be reported in the statement for the message type 942 do not depend on the last MT941 statement.


#### ⚙️ Configuration

The ACCOUNT.STATEMENT application allows the production of SWIFT MT942 messages. The following fields in the ACCOUNT.STATEMENT record control the MT942s:

| Column 1 | Column 2 |
|---|---|
| Field Name | Description |
| Message Time | A multi-valued field indicating the time during the day when the message is to be produced. This is required for automatic production of MT942 messages. The value needs to be defined in hh:mm format, where, hh is the hours in 24 hour format mm is the minutes past that hour |
| Dr Floor Limit | The minimum value of a debit transaction that is to appear on the statement. Any transaction below this amount, is not included in the statement. |
| Cr Floor Limit | The minimum value of a credit transaction that is to appear on the statement. Any transaction below this amount, is n |
| Message Type | The MT942 message type to be defined. |
| Send Msg Type | Allows the values Yes, No, STP or MOV, where: Yes generates through DE.MT942.REQUEST . No stops or does not allow the generation of the MT942 message. STP generates the MT942 after receiving an inward MT920 message. MOV ignores generation of the message if there is no movement to the account since the last statement. |
| Intra Day Start | Defines the date from when the first MT942 and MT941 statement generation starts. |

The AC.STMT.PARAMETER application contains the Intra Ent Date field. The value defined in this field indicates whether the MT942 statement includes only the entries booked on the current bank date, or holds entries raised after the last statement.

- When the field is set as Today, and if it is the first MT942 statement for that business day, then it holds entries with the booking date equal to Today, which is the current bank date. For a subsequent statement on the same day, it holds the entries posted for that account after the last statement.
- If the field is left blank, it holds the entries posted for that account after the last statement date. It is not confined to entries raised for the current bank date.

The following parameterisation is used to generate the statement for the MT941 and MT942 message types independently at the system level.

The MT942 message type entries are selected based on the parameterisation of the Gen942 Independently field. If it is set to Yes, then during the statement generation for the message type MT942, the system performs filter only based on the previous MT942 statement (that is, based on DE.MT942.SENT.ENTRIES . Core filter process does not perform check on DE.MT941.SENT.ENTRIES ).

This parameterisation is available only at the system level and cannot be modified at the account level.


#### 📋 Tasks

There are no Tasks available for Interim or Intra-day Transaction Report feature.


#### 📊 Outputs

There are no Outputs available for Interim or Intra-day Transaction Report feature.


> **Related Applications:** `DE.MT941.SENT.ENTRIES`, `DE.MT942.REQUEST`, `DE.MT942.SENT.ENTRIES`

---


### 2.19  InwardDeliveryMessageProcessing


> **📇 Quick Reference Card**
> 
> **Purpose:** *Certain SWIFT payment messages are processed using the inward delivery OFS.GLOBUS.MANAGER method. This generic method relies on the following attributes to improve the functionality and maintainability:*
> 
> **Applications:** `DE.I.SUBROUTINE.TABLE`, `DE.MESSAGE`, `FUNDS.TRANSFER`, `INWARD.OFS.RTN`, `OFS`, `OFS.SOURCE`, `PGM.FILE`, `VERSION`
> 
> **Key Fields:** *Application*, *Control*, *Det*, *Detail*, *Dets*, *Dir*, *Err*, *File* ... +20 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Certain SWIFT payment messages are processed using the inward delivery OFS.GLOBUS.MANAGER method. This generic method relies on the following attributes to improve the functionality and maintainability:

- OFS.GLOBUS.MANAGER
- Message specific processing
- Tag field specific subroutines.

It allows the flexibility of locally developed subroutine messages. This has been developed largely in response to the increased Straight Through Processing (STP) requirements.


#### ⚙️ Configuration

This topic covers the configuration required for processing the inward deliver message.


##### SWIFT Inward Message Subroutines and Local Development Templates

The messages supported by Temenos Transact are:

- MT101
- MT103
- MT200
- MT205
- MT210

A subroutine is provided for each of these messages, although this may be replaced by a locally developed routine (if required), for example, a template subroutine, TEMPLATE.S.

> **⚠️ Note:** Similar processing is done for Securities (SC), Miscellaneous Deals (MD) and Letters of Credit (LC) messages, although these may not use the same template program style.


##### Processing of SWIFT Inward Tag Routines -DE.I.SUBROUTINE.TABLE

The DE.I.TAGxx application is used for inward tag processing routines (where, xx is the SWIFT tag field number) which are supplied for all supported SWIFT tag fields. The local type subroutines (S type set in PGM.FILE ) may be substituted. The DE.I.SUBROUTINE.TABLE indicates which tag subroutine is to be used for each tag field number supported (default routines are supplied).

> **⚠️ Note:** The tag field subroutine listed in Subroutine field will be used for all occurrences of the field tag, regardless of the SWIFT message type or the application the data will be passed to.


##### Setting up OFS.GLOBUS.MANAGER Processing for a SWIFT Message

The steps for setting up the OFS.GLOBUS.MANAGER are as follows:

1. Create an OFS.SOURCE record. This defines an OFS interface for OFS.GLOBUS.MANAGER. The field usage of this application are:

| Field | Value | Description |
|---|---|---|
| Source Type | GLOBUS | Holds the interface called from a subroutine. |
| Log File Dir | LOGDIR | Specifies the name of the OFS log directory. |
| Log Detail Level | FULL | Lists the full history of each OFS message maintained. |
| Maint Msg Dets | Y | Creates an audit record for each OFS message. |
| Det Prefix | INW | Specifies the audit record prefix. |
| Syntax Type | OFS | Specifies the OFS syntax type for messages. |

1. Create a VERSION record for the application to be called. This is used by OFS to add a record to the required application. For example, a zero authoriser version of FUNDS.TRANSFER .

> **⚠️ Note:** The Gts Control field is set to 1, as it places the error message contracts on hold and automatically accept the overrides.

1. Set the DE.MESSAGE application for OFS.GLOBUS.MANAGER processing and to use the subroutine. The following fields are set in DE.MESSAGE for OFS inward delivery processing:

| Field | Value | Description |
|---|---|---|
| Application Queue | NULL | Specifies the application which should receive an inward message of this type. |
| Inward Ofs Rtn | ROUTINE NAME | Specifies the supplied or local subroutine, which should be called to process this message type. |
| In Ofs Version | VERSION | Indicates to OFS, which version of an application should be used to create the records. |
| Ofs Source | SOURCE | Indicates the OFS source interface to be used when processing this message. |


#### 🔧 Working With

Inward SWIFT messages are received from the SWIFT interface (for example, alliance) and then the inward formatting services process the messages.

The OFS SWIFT inward message processing subroutine indicated in INWARD.OFS.RTN in DE.MESSAGE (when the Application Queue is NUL) is executed using tag subroutines indicated in DE.I.SUBROUTINE.TABLE . The subroutine creates an OFS record populating the fields for the target application from information in the SWIFT message and then calls OFS.GLOBUS.MANAGER.

A history log is generated for each message, as per the setup in OFS.GLOBUS.MANAGER. The transactions appear successfully in the application or they may be placed in IHLD, if there are any errors. While processing the inward messages (which creates the FUNDS.TRANSFER records) the In Process Err field is updated with the processing information (with tag which is not mapped or errors encountered in FT) and In Swift Msg field is updated with the incoming SWIFT message details.


#### 📋 Tasks

There are no Tasks available for Processing of Inward Delivery Message feature.


#### 📊 Outputs

There are no Outputs available for Processing of Inward Delivery Message feature.


> **Related Applications:** `DE.I.SUBROUTINE.TABLE`, `DE.MESSAGE`, `FUNDS.TRANSFER`, `INWARD.OFS.RTN`, `OFS`, `OFS.SOURCE`, `PGM.FILE`, `VERSION`

---


### 2.20  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *This topic explains the Delivery (DE) module that manages the flow of all messages from Temenos Transact , such as confirmations, payments and advices which gives full control over formatting and language of presentation to the users. Messages are generated automatically, as soon as the transaction ...*
> 
> **Applications:** `ADDRESS`, `ARCHIVE`, `ASCII.VAL.TABLE`, `ASCII.VALUES`, `CARRIER`, `CONTROL`, `CUSTOMER`, `DE` ... +33 more
> 
> **Key Fields:** *Address*, *Address Purpose*, *Address Type*, *Address Validated By*, *Apply Address Rules*, *Arc Filename*, *Archive Data*, *Building Name* ... +23 more
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- APIs
- Temenos Transact Services

This topic explains the Delivery (DE) module that manages the flow of all messages from Temenos Transact , such as confirmations, payments and advices which gives full control over formatting and language of presentation to the users. Messages are generated automatically, as soon as the transaction is complete or when a scheduled event occurs.

All messages may be either printed or sent through electronic carrier systems, such as SWIFT, Telex and the like.

Messages from external carrier systems are received by the delivery system and formats (if necessary) according to the user-determined requirements. Then, printed output containing the incoming information is produced. For example, after authorisation the payment messages are passed in the Funds Transfer (FT) module, which updates the accounts and it's related information.

The delivery process is fully automated, but the users may take control over many aspects of message management. Temenos Transact has the facility to inspect, control the message queues and use graphical enquiries to view the queue status. Once the messages are in queue, the individual messages may be displayed, amended or re-routed.

> **⚠️ Note:** The DE module can create messages, which are not explicitly linked to any other Temenos Transact business application.

Product Features

The DE module is classified as:

- Base functionality – Covers the setup and usage of delivery across the business applications in Temenos Transact .
- Message creation functionality – Covers the setup and usage of applications under the DE module, which are not explicitly linked to any other Temenos Transact application that generate the delivery messages for various purposes.

Base Functionality

Static Processing of Messages Outward Delivery Messages Inward Delivery Messages End Period Processing Translation Delivery Messages Recovery Delivery Tables Defining Print Format Defining Template Format for Printing Outside Delivery Module Diverting SWIFT MT Messages Generic Delivery Interface Email, SMS and Messaging Hold Output for Delivery Carriers BIC Database Upload Straight Through Processing Customer Address in Delivery Output Generation of MX Message using ISOMX Carrier SWIFT MT Stop Delivery Service SWIFT Security Program - Local Authentication Delivery as Microservice Events Message Creation Functionality Request for Transfer of Funds Soft Delivery Free Format Messages Interbank Statement Request Interim or Intraday Transaction Report


##### Product Configuration

This section details the configuration setup required for the DE module.

SF is the product code for SWIFT messages (available from R13). With this product code, SWIFT messages are formatted only if the SF product is installed. If SF is not installed, then the messages will go to repair status. This is applicable for incoming and outgoing SWIFT messages.

The DE.PARM application holds a number of parameters to control the processing of messages in the DE module. This application contains a single record (SYSTEM.STATUS). With the replacement of formatting and ad hoc processing accompanied by the new delivery services, the settings in DE.PARM may not be applicable.

The following are the types of data on DE.PARM :

- Parameters that allow the operator to shut down the carrier control modules, the inward and outward formatting modules. The shut down can be: Urgent (after the message being processed). Normal (when all queues have been processed).
- Parameters that can be used to optimise the performance of all carrier control, inward and outward formatting modules. The options are: After processing all urgent messages, a specified number of priority messages and a specified number of normal messages are processed, before returning to check whether there are any other urgent messages to be processed. Making these numbers larger increases the efficiency of the system, but causes slight delays in the processing of urgent messages. A wait time can be specified. This is the time that the carrier control and formatting modules will wait, between finishing the processing of all their queues and searching them again for input. A longer wait time gives other users a faster response, but causes slight delays to messages.
- Fields are defined in the way the delivery system is installed.
- The Cet Time Diff field defines the local time difference from the Central European Time (CET). This is used in the conversion of SWIFT messages and added after the time.

> **⚠️ Note:** Shut down of services using DE.PARM affects only the remaining phantom services, the newer services are controlled using the TSA.SERVICE records.

The DE.CARRIER application contains the details of all carriers available in the DE module. The bank need not amend this application, unless new interfaces are required to be linked to the delivery system. The user must specify the carrier in the DE.PARM application, to enable the carriers specified in DE.CARRIER . The ID of DE. CARRIER is the name of the carrier, as used in DE.PRODUCT .

Each record contains:

- The address type to be used for the carrier (that is, when accessing DE.ADDRESS ).
- The formatting rules (defined in DE.FORMAT.CARRIER ).
- The carrier module (for example, SWIFT).

If the carrier module is GENERIC, the interface must be specified. The interface must reference a record in DE.INTERFACE , which contains the details of the protocol for all generic interfaces (non-generic interface details are stored in DE.PARM ). When the record is authorised, formatting and carrier applications are created (if they are not existing already).

The Apply Address Rules field in DE.CARRIER enables the bank to define for each carrier if that carrier is allowed for validation of the address rules or not. The available options in this field are Yes or Null and the default value is Null.

The DE.ALTERNATE application contains the alternative carriers or addresses to be used, if a message is to be rerouted. For example, a customer may normally have all their messages sent to a particular telex number, but that telex number might be out of order, so all their messages are to be sent to an alternative telex number.

The DE.ALTERNATE application is accessed, if the Msg Disposition field in the inward and outward DE.I.HEADER and DE.O.HEADER applications are set to REROUTE.

When a message is passed through formatting and if the Msg Disposition field is set to REROUTE, the DE.ALTERNATE application is accessed for the carrier, address number, language and format. It then copies the message which is to be sent. The ID of this application is as follows:

- Company code followed by ’.’
- C-customer number followed by ’.’ or A-account number followed by ’.’
- Carrier followed by ’.’
- Address number (that is, nnnnn as per DE.ADDRESS )

For example, US0010001.C-1026.SWIFT.1

When this application is accessed, only a record at the same level as the DE.PRODUCT record originally read will be accessed. Therefore, if the DE.PRODUCT record originally read was at customer level, then the DE.ALTERNATE application will be accessed at customer level. If an appropriate record cannot be found, the message will go into repair with a corresponding error message.

The DE.ALT.CHARS application holds the character mappings for the replacement of language specific characters to SWIFT acceptable characters.

If a field is defined as a language based field and the data captured is in the French, the system allows standard French characters such as á,è,é,Ç, if the date captured is in the German characters, then it allows ü,ß. When the system uses such information in the SWIFT messages, it converts it to SWIFT acceptable characters.

The system provides a default set of known characters and the alternative replacements. In addition, it provides an option to amend the application, if the user wants to add more characters.

The ID of this application must be a meaningful ID that must be relevant to any validation or conversion and used in carrier’s formatting of the message. A single language specific character may be replaced by null, one or more characters.

The ASCII.VALUES application must be configured to ensure that the character sets are allowed. It is possible to define invalid characters and their replacement values by message format types.

- SWIFT message types - ‘è’ is not allowed for this message type and should be replaced with ‘e’.
- CAMT message types - ‘è’ is not allowed for this message type and need not be replaced, whereas ‘â’ is not allowed and should be replaced with ‘a’.

Conversion is achieved by attaching CONV* DE.ALT.CHARS to the field as shown in the below screenshots.

The product information in the DE.PRODUCT application is used by formatting process when expanding the DE.I.HEADER and DE.O.HEADER records for the copies required for the message. Product information consists of status (normal, hold or delete), carrier or delivery address, version of the format to be used and how many copies should be made.

After the DE.I.HEADER and DE.O.HEADER records has been expanded, the DE.PRODUCT record is not read again for this message, even if the message is resubmitted and is placed again on the dun-formatted queue. Therefore, if language, format or copies are to be changed after the DE.I.HEADER and DE.O.HEADER records has been expanded, the message must be re-routed.

The DE.PRODUCT records may be specified for:

- A particular company.
- A customer.
- An account.

> **⚠️ Note:** Account is applicable only for statement type messages.

And each of the DE.PRODUCT records may be specified for:

- All message types.
- Specific message types.
- All banking applications.
- A specific application.

During formatting, the DE.PRODUCT is read for the most specific record, matching the details on the DE.I.HEADER and DE.O.HEADER records. If the most specific record is not found, the DE.PRODUCT is read again until a more general record is found. The ID of the DE. P RODUCT application consist of one or more following components in the sequence given below:

- Company code followed by ’.’
- C-customer number followed by ’.’ or A-account number followed by ’.’ (this is not present for company level records)
- Message type or ALL followed by ’.’
- Application or ’ALL’ or xxyy, where xx is the Application code and yy is the Funds Transfer (FT) product code.

A portfolio specific

for

related applications are shown in the below screenshots. A sample list of

records:.

A sample of portfolio specific DE.PRODUCT records:

The records in the DE.PRODUCT application is searched in the following order:

- All fields used to find the records in the DE.PRODUCT are stored in the DE.I.HEADER and DE.O.HEADER records. Therefore, by using the fields available and by searching the DE.PRODUCT (in the above order), it is possible to find out which DE.PRODUCT record has been used to expand the multi-value set in the DE.I.HEADER and DE.O.HEADER records.
- The multi-value set on the DE.I.HEADER and DE.O.HEADER records are expanded according to the fields in the DE.PRODUCT record. For example, if the DE.PRODUCT record says that, one copy should be sent by SWIFT and one by print. The DE.I.HEADER and DE.O.HEADER records are updated accordingly. The following fields in the DE.I.HEADER and DE.O.HEADER are updated from the DE.PRODUCT record: Carrier Addr No Format Msg Language Msg Priority Msg Status Msg Disposition
- If the DE.PRODUCT record says that a particular carrier should send two copies, these copies are split on the DE.I.HEADER and DE.O.HEADER records into two multi-value sets.
- If a single message should be sent to multiple customers, the Mdr Customer field in the DE.PRODUCT application (a multi-value set) can be used to specify additional customers to whom the copies of the message needs to be sent. This can be specified for customer or account level records and for print carrier only.
- The language on the DE.PRODUCT record is not used to update the DE.I.HEADER and DE.O.HEADER records, if the DE.PRODUCT record used was a company level record, since the language passed from the application is more specific.
- For a particular message type, if copies are not allowed, that is, copies is set to NO in the DE.MESSAGE , then only the first copy of the message specified in the DE.PRODUCT record is used to update the DE.I.HEADER and DE.O.HEADER records.
- The DE.PRODUCT record can also be used to hold the messages or to delete the messages, using the Status field.

The DE.ADDRESS application contains the names and addresses of a bank customers, and also the details of each company within the banking organisation. The basic postal address of each customer is automatically updated, when the address is changed through customer maintenance ( CUSTOMER application). A record is created in the DE. ADDRESS application with ID as COMPANY ’.C-’ CUSTOMER ’.PRINT.00001’

The address on this record cannot be updated through the DE.ADDRESS application, but must be updated through CUSTOMER application. The SWIFT IDs, telex numbers and alternative print addresses are also held in DE.ADDRESS . These records may be input and amended through the DE.ADDRESS . The ID of this records is COMPANY ’.C-’ CUSTOMER ’.XXXXXX.N’, where, XXXXXX is a valid carrier defined in DE.CARRIER (for example, SWIFT, TELEX) and N is the address number. The address number is in the range 00001 to 99999.

> **⚠️ Note:** If the carrier is TELEXF or TELEXP, a carrier of TELEX is used when looking up the DE. ADDRESS application.

During formatting, after the DE.PRODUCT record has been read, DE. ADDRESS is read for each copy of the message in the multi-value set in the DE.I.HEADER and DE.O.HEADER records. The ID of DE.ADDRESS application consists of the fields in the DE.I.HEADER and DE.O.HEADER records, using the carrier address from the DE.CARRIER and the address number held in the Carrier Addr No field. If the ADDRESS record is not found in DE. ADDRESS , the message will go into repair.

The address in the DE.ADDRESS is appropriate to the carrier ID used to update the To Address field in the DE.I.HEADER and DE.O.HEADER records. It is possible to hold all printed output for this address by setting the Hold Output field to Yes.

The message goes through delivery process in the normal way, but instead of being printed, it is written to the HOLD.CONTROL table. When up to date messages are required for the customer, it can be printed using the PRINT.CUST.OUTPUT application.

A multi-value Address field is available in DE.ADDRESS . When the customer’s main address is updated, the DE.ADDRESS PRINT.1 record is updated by copying the address lines from the CUSTOMER record to the DE.ADDRESS PRINT.1 record. For all other DE.ADDRESS records, the Address multi-value field is manually inputted.

Additional address line details are added using the following fields:

- The Address Type field identifies the nature of the postal address (that is, the postal office (PO) box, home). These values are defined in the EB.LOOKUP application.
- The Address Purpose field represents the purpose of an address (that is, communication to customer, communication to in care of party)
- The Building Number field represents the number that identifies the position of a building in the street.
- The Building Name field identifies the name of the building and entrance.
- The Flat Number field represents the number that identifies the apartment and unit that have other dwellings above or below, often with shared access and common areas.
- The Po Box Number field identifies PO box number.
- The Country Subdivision field identifies a subdivision of a country, such as, state, region or county.
- The Title field holds the title for the customer name.
- The Salutation field represents the greeting used for communication with the customer.
- The Address Validated By field represents the party or service, which confirms that it is a valid or real address.
- The Idd Prefix Phone field represents an international call prefix or dial out code.

> **⚠️ Note:** The main delivery address (PRINT.1) is automatically updated by changing the address of a customer. For all the other delivery addresses, rather than PRINT1, the above field values are inputted.

As the priority of a message can only be N, the DE.DISP.CONTROL application is used to change the status of a message. Disposition checks are done after the carrier is identified at the transaction level itself. If the messages are marked as HOLD or DELETE or REROUTE, the appropriate applications are updated as mentioned below:

- If HOLD, the DE.O.HOLD.KEY application is updated.
- If DELETE, the DE.O.HEADER is deleted.
- If REROUTE, the message is put into the DE.ALTERNATE application.

On releasing the DE.O.HEADER from HOLD, the held records are moved into the appropriate carrier activation applications. The DE.DISP.TIMECHECK service process the messages marked as HOLD until a particular time.

The DE.DISP.CONTROL application is used to specify special conditions for which particular processing is required. If the conditions are satisfied, the requirements specified in DE.DISP.CONTROL overrides all other the requirements. The only condition is that, it cannot override restrictions such as deleting messages for message types, which cannot be deleted (that is, Delete field in DE.MESSAGE application is set to NO) or the copies of messages being generated for message types that do not allow copies ( Copies field in the DE.MESSAGE application is set to NO).

The DE.DISP.CONTROL application can be used in the following scenarios:

- All messages for a particular carrier must be rerouted (the DE.ALTERNATE application is accessed to find the new carrier).
- Print a copy of all messages, which have a message type of 100 and for Customer 254 or 256.

The above is achieved by setting up the conditions on which the message status is set. Alternatively, a user-defined routine can be specified to check complex conditions, the routine passes back whether the conditions were matched or not. The routine name is placed in the Field Name field and must be prefixed by @ character. The routine is passed with the current DE.O.HEADER record in argument one, the OPERAND in argument two and the CONDITION in argument three.

The return argument is argument four and should evaluate to true (1) or false (0 or null). The routine should be specified as EXAMPLE.NAME (HEADER.REC, OPERAND, CONDITION, RETURN.FLAG).

Records are added to the DE.DISP.CONTROL application with a numeric ID. When the transaction is entered and passes the formatting stage, DE.DISP. CONTROL application is examined in numerical order until a record is found with satisfying conditions or until no further records are found in the DE.DISP.CONTROL application. Thus, if a message matches the conditions specified in DE.DISP.CONTROL records 10 and 50, only record 10 will be applied to the message. Therefore, it is important to be cautious when entering records in the DE.DISP.CONTROL application, to assign the ID according to the importance of the record.

Conditions can be specified in the DE.DISP.CONTROL record to compare the fields in the DE.I.HEADER and DE.O.HEADER records to certain values.

CARRIER EQ SWIFT or AMOUNT GT 1000000. The condition fields are multi-value and assumes a condition of AND. Therefore, complex conditions can be built by setting up several simple conditions in a multi-value set. For example, AMOUNT GT 1000000 AND CURRENCY EQ GBP. All the conditions must be true before the status is applied. If OR is required, separate records must be entered.

In the DE.DISP.CONTROL application, the messages that match the conditions specified can be updated with specific status. This is entered in the Status field and the field can be set as:

- HOLD
- HOLD hh:mm
- WAIT hh:mm
- RELEASE
- DELETE
- RESUBMIT
- REROUTE or
- PRINT

The HOLD status can also be used with the Hold Until Date field, by either specifying an exact date or entering VAL to set the hold date according the days’ delivery for the currency.

When a new or amended DE.DISP.CONTROL record is authorised, the Msg Disposition or Msg Status field in the DE.I.HEADER and DE.O.HEADER records for each message that has been successfully formatted but not sent (messages not in the repair queue) is amended, if the information in the DE.I.HEADER and DE.O.HEADER records match the conditions defined in that DE.DISP.CONTROL record. This involves examining numerous queues and application in the delivery system and could take some considerable time.

However, if the Delivery Operator does not require the DE.DISP.CONTROL record to be applied to messages already formatted, but only requires them to be applied to newly generated messages, the Disposition Control field in the DE.PARM application can be set to N before the DE.DISP.CONTROL record is authorised, then it must be reset to Y after the record is authorised.

> **⚠️ Note:** The Disposition Control field in DE.PARM refers to all records in the DE.DISP.CONTROL application. Therefore, care should be taken in resetting it, as messages currently being processed by delivery might not have action taken by relevant records because the Disposition Control field was not set. It is recommended to stop all the delivery processes before changing this field.

The DE.DISP.CONTROL records are also applied to messages that are created by the delivery system during formatting, unless the Disposition Control field in DE.PARM is set to N. The following status affects the records with a disposition of Formatted:

- HOLD
- WAIT
- DELETE
- RESUBMIT
- REROUTE

They operate subsequently while formatting the records that are set to Formatted. The WAIT hh:mm status is translated to HOLD hh:mm, when the DE.DISP.CONTROL record is applied.

The RELEASE status affects the records in HOLD status and operates subsequently during formatting. The PRINT status prints an image of the formatted messages, regardless of the carrier used to send the message. It produces a printed copy of a SWIFT message (if the message was originally sent by SWIFT). If the original message was sent out by print, the image has ’** COPY ** COPY ** COPY **’ printed at the bottom of each.

Each DE.I.HEADER and DE.O.HEADER records that is changed has the ID of the DE.DISP.CONTROL record, placed in the appropriate Disposition No field in the each copy of message affected. This ensures a less important DE.DISP.CONTROL record which does not subsequently change it. Records with lower IDs take precedence over higher IDs, for example, 10 takes precedence over 100.

The record should be reversed when the conditions no longer apply. Run the DE.DISP.CONTROL application using the DE.DISP.TIMECHECK record in TSA.SERVICE .

The DE.INTERFACE application contains the details of the protocols for all interfaces which use the Generic Delivery interface. The protocols for interfaces written prior to the introduction of the Generic Delivery interface are either stored in DE.PARM or are hard-coded in the program. The sequence numbers for existing interfaces are stored in the F.LOCKING application. This application need not be amended unless a new interface is being developed.

Minimum validations are done in the fields of the DE.INTERFACE application. This is to allow maximum flexibility when new interfaces are written. The ID of the application is the interface, as defined in the Interface field in the DE.CARRIER application.


##### Archival of Delivery Messages

The Delivery messages can be archived using the Transact Standard archival or Data Lifecycle Management (DLM) archival.

The DL module must be installed for the user to initiate the archival service to archive the delivery messages to a Read-only (RO) database. Otherwise, the user moves the data records to the $ARC file using the Standard archival method. The user defines Retention Period in ARCHIVE for the DELIVERY.IN and DELIVERY.OUT records for the inward delivery messages and outward delivery messages, respectively. If the delivery message date in DE.I.HEADER (for Inward message) and DE.O.HEADER (for Outward message) cross Retention Period , it is archived.

The user must execute the following services as a pre-requisite for initiating the generic archival service to archive the delivery message in the Transact Standard archival process.

| Services | Description |
|---|---|
| DE.EOP.INWARD and DE.EOP.OUTWARD | These services analyse the DE.O.HEADER and DE.I.HEADER entries respectively to identify the records that are processed completely. These services select the DE.I.HEADER and DE.O.HEADER records, moving the records from DE.I.HEADER to DE.I.HEADER.ARCH and DE.O.HEADER to DE.O.HEADER.ARCH respectively. |
| DE.MM.CLEAR.HANDOFF | This service deletes the DE.O.HANDOFF records where DE.O.HEADER is previously removed. This service selects all the DE.O.HANDOFF records to identify the records to be deleted. |
| Delivery Inward and Delivery Outward Archiving | These services archive the records from DE.I.HEADER.ARCH and DE.O.HEADER.ARCH respectively along with related table records. |

However, when the DL module is installed, the DLM archival processing logic consolidates the processing performed by the pre-requisite services mentioned above. The generic archival service execution is sufficient to perform the delivery archival based on the DELIVERY.IN and DELIVERY.OUT records configured in ARCHIVE .

Sample screenshots of the ARCHIVE application for the delivery messages are shown below.

- DELIVERY.IN
- DELIVERY.OUT

When Retention Period ends and the user runs the archival service, the files mentioned in Arc Filename are archived.

> **⚠️ Note:** The user must set Archive Data as Y to archive the record. If the user sets it as N, the record is deleted instead of archiving, which results in loss of data.

Read Archiving for more details regarding Transact Standard archival process. Read Data Life Cycle Management for more details regarding DLM Archiving process.


##### Illustration Model Parameters

This section covers the Model Parameters required for the Delivery module.

| S.No | Parameters | Description |
|---|---|---|
| 1. | Tracker Status Reason | Allows users to define the status code and status reason which is used to update the status of the incoming MT103 payment in the SWIFT Confirmation tracker. |
| 2. | DE.MESSAGE.HEADER | Allows users to define the message headers, which are used for various type of messages. For each header, it stores the version, set of Business and Generic Metadata, which must be pushed as part of the data event with the payload. |
| 3. | DE.BUSINESS.SERVICE.RULES | Allows users to create business service rules for delivery messages based on domain, message name id, business application, application context field, application context value, start date, end date, business service and status. When a Delivery Message is handed off to Delivery, it considers the supplied value if the Business Application supplies the Business Service. Otherwise, it determines the Business Service based on the DE.BUSINESS.SERVICE.RULES application setup. |
| 4. | DE.DELIVERY.RESPONSES | Stores the incoming replies received for the outward interact MX messages (Ack/Nack/DLN) sent through delivery. It is possible to store other replies sent by other bank systems, which are acting as an intermediary systems before the messages sent to SWIFT network. |
| 5. | DE.DLN.REQUIREMENTS | Allows the bank to define the rules to request a positive or overdue delivery notification. In this way, the bank has the option to request a positive delivery notification and overdue warning (Optional). It is not possible to request only overdue warning. |
| 6. | DE.ALT.CHARS | This table helps to parameterise the alternate characters (defined in ASCII.VAL.TABLE ) for the local unsupported characters. Various rules are defined to replace the alt chars based on the position of the unsupported character in the message string. A default alternate character is defined if alternate character is not defined for an unsupported character. |
| 7. | DE.MSG.CHARS.RULE | This parameter table defines the character set rules for each carrier and message type. |


##### Illustration Model Products

Model Products are not applicable for this module.


> **Related Applications:** `ADDRESS`, `ARCHIVE`, `ASCII.VAL.TABLE`, `ASCII.VALUES`, `CARRIER`, `CONTROL`, `CUSTOMER`, `DE`, `DE.ADDRESS`, `DE.ADDRESS PRINT.1`, `DE.ALT.CHARS`, `DE.ALTERNATE`, `DE.BUSINESS.SERVICE.RULES`, `DE.CARRIER`, `DE.DELIVERY.RESPONSES`, `DE.DISP`, `DE.DISP.CONTROL`, `DE.DISP.TIMECHECK`, `DE.DLN.REQUIREMENTS`, `DE.FORMAT.CARRIER`, `DE.I.HEADER`, `DE.I.HEADER.ARCH`, `DE.INTERFACE`, `DE.MESSAGE`, `DE.MESSAGE.HEADER`, `DE.MSG.CHARS.RULE`, `DE.O.HANDOFF`, `DE.O.HEADER`, `DE.O.HEADER.ARCH`, `DE.O.HOLD.KEY`, `DE.PARM`, `DE.PRODUCT`, `EB.LOOKUP`, `F.LOCKING`, `HOLD.CONTROL`, `P`, `PRINT.CUST.OUTPUT`, `RODUCT`, `SEC.ACC.MASTER`, `TSA.SERVICE`, `Tracker Status Reason`

---


### 2.21  Mx Message FW


> **📇 Quick Reference Card**
> 
> **Purpose:** *During annual maintenance, SWIFT CBPR+, National RTGS, and other SWIFT Interact based solutions undergo modifications that could potentially affect the Temenos Transact modules.*
> 
> **Applications:** `DE.BUSINESS.SERVICE.RULES`, `DE.CARRIER`, `DE.DISTINGUISH.NAME.RULES`, `DE.MESSAGE`, `DE.PRODUCT`, `SWIFT.PARAMETER`
> 
> **Key Fields:** *Curr Swift Rel*, *Current Release*, *Format Module*, *Manual Prev Swift Rel*, *Prev Swift Rel*, *Prev Swift Rel.1*, *Prev Swift Rel.2*, *Release* ... +2 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

During annual maintenance, SWIFT CBPR+, National RTGS, and other SWIFT Interact based solutions undergo modifications that could potentially affect the Temenos Transact modules.

The modifications can include:

- Message Headers - Addition of new or removal of existing fields, changes in fields, and addition of new versions of header elements such as Business Service and Message Name.
- Message Payloads - Addition or removal of tags, changes to tag status (mandatory or optional), and modifications to Message Name IDs.
- Messages - Creation of new messages or obsolescence of existing messages.

A part of these changes must be controlled by the respective business module. For example, new mandatory payload fields usage rules, decision to emit the MT or MX message, and so on. The Delivery framework controls the general changes such as modifications to parameter setups maintained through configurations (distinguish names, business service, carrier, and so on).

> **⚠️ Note:** Verticals must adhere to strict guidelines while releasing configurations for their solutions in the Delivery module.


##### Licensing Annual Change

The Delivery module contains a framework to control the parameterisation and the activation of the annual rulebook changes across the Temenos Transact modules that use the Delivery XMLISO formatting modules such as CBPR, TGT, SIC, and so on. The Delivery Carrier stores the details of the SWIFT interact service used for each solution (service name, message name, and so on).

For example, CBPRPLUS Delivery Carrier is used for CBPR+ messages, TGT is used for Target2 messages, SIC is used for SIC RTGS messages, FUNDS is used for Funds messages, and so on. Each services’ rulebook calendars are independent of one another, and the Delivery module handles them separately.

> **⚠️ Note:** For backpatch clients, annual rulebook changes are released under specific license codes.


#### ⚙️ Configuration

This topic describes the configurations of MX Messages Framework.


##### Activating MX Messages

The user configures the annual release for MT messages through SWIFT.PARAMETER . The user configures the ISO20022 messages processed by the solutions that use the Delivery XMLISO in which case, the user activates the rulebook per solution or payment scheme level such as CBPRPLUS, FUNDS, SIC, CHAPS, and so on.

The user can use the SYSTEM record in SWIFT.PARAMETER for the annual SWIFT MT rulebooks. The user enables the annual SWIFT MX rulebooks using the record in SWIFT.PARAMETER with a valid DE.CARRIER ID, provided the respective carrier uses Format Module as XMLISO.

The user enables the latest rulebook by configuring Curr Swift Rel in SWIFT.PARAMETER . Manual Prev Swift Rel is used to update previous releases. If Manual Prev Swift Rel is defined, the system updates its value to Prev Swift Rel multi-value during authorisation.

The user activates a rulebook by configuring the corresponding rulebook year in Curr Swift Rel in SWIFT.PARAMETER , giving them flexibility to install the software in the production environment before the rulebook activation date.

For example, if the SWIFT CBPR+ 2023 changes are published on 19th November 2023, the user must activate the changes on that date. Therefore, Curr Swift Rel in the CBPRPLUS record in SWIFT.PARAMETER is updated to 2023 on the date when the new rule book changes take effect.

Whenever the user modifies Curr Swift Rel , the system updates its previous value in Prev Swift Rel multi-value. However, the user may skip certain annual changes if it does not process messages that are impacted by the changes in the respective annual release.

The user activates the changes when it is ready to be published based on the calendar imposed by SWIFT or at a later stage, if the changes are optional. The users manually update the previous release using Manual Prev Swift Rel . However, this option is available only for the parameterisation solutions that use the XMLISO Delivery framework and not the SYSTEM record for MT.

| SWIFT.PARAMETER | @ID=CBPRPLUS |
|---|---|
| Curr Swift Rel | 2025 |
| Prev Swift Rel | 2023 |


##### Handling Modifications to Delivery Configuration for Rulebooks

The Delivery framework can manage the rulebook-specific configurations by enabling the activation of configuration changes and the expiration of outdated or replaced configurations.

The system refers to DE.MESSAGE for the messages routed through the Delivery framework. If the business module hands-off the data to Delivery to form the payload, DE.MESSAGE stores the definition of all the tags.

If the existing messages are affected by the annual rule book changes, the definitions in DE.MESSAGE are updated to reflect those changes. However, certain changes such as making a field mandatory or adding calculation logic for enrichment are not addressed by the Delivery message definition. The system incorporates changes to the applications responsible for generating the messages based on the rulebook for the corresponding feature.

The definition of the CAMT054 message is changed in 2025, whereby a previously optional field or tag becomes mandatory.

- This change has no impact on the DE.MESSAGE definition.
- The payment applications generating CAMT054 handle the logic to make the field or tag mandatory only if Curr Swift Rel in SWIFT.PARAMETER for the respective channel (Delivery carrier) is equal to or greater than 2025.

If the payload is formed by the business module, the application handles the payload based on the current rulebook as DE.MESSAGE stores only a minimum set of details.

DE.PRODUCT contains the information about the routing carrier, message format, and the number of copies to be generated. To handle new message types, Temenos Transact releases new delivery product definition. Hence, the impact of annual rulebook changes on the existing Delivery Product definition is minimal.

The new product definition activation does not require any specific logic from a delivery perspective since the respective business modules handle the emission of these new messages.

DE.CARRIER contains information about the SWIFT Interact channels that are used by various business applications to send and receive messages.

As part of the annual maintenance license code, the Delivery carrier configurations applicable for the rulebook are available and the user manages carrier-specific customisation in the delivery carrier that corresponds to the rulebook year. Hence, if customisation is required for a particular carrier, the user must configure the rulebook-specific delivery carrier and such customisation takes effect when the rulebook year is activated.

The Release field in the DE.DISTINGUISH.NAME.RULES and DE.BUSINESS.SERVICE.RULES tables decide the rule that is active at some point in time. A rule is considered active and applicable if the Release field is either blank or matches the value in the Current Release field in SWIFT.PARAMETER .

While processing a message, the delivery framework determines the distinguish name and business service rule using the following logic:

- Use the rule defined for the respective message type and carrier, where the Release and Current Release fields defined in SWIFT.PARAMETER are the same for the respective carrier.
- If no rule is defined, the Delivery framework refers the rule for the respective message type and carrier that has the Release field left blank.
- If not found, Delivery refers the generic rule defined for that Delivery Carrier, irrespective of the message type.

Whenever there is a rule book change, the respective business modules deliver the following records:

- The existing records that are affected by the upcoming release are updated with the current release value in the Release field. This ensures that they become obsolete after the new standard release is activated.
- New records are released for the new or modified rules, the Release field is left blank since the timing of when this rule will be changed in future is unknown.

Following are examples for Business Service and Distinguish Name:

When a new rule book is activated in SWIFT.PARAMETER , the Delivery framework moves any records in the DE.DISTINGUISH.NAME.RULES and DE.BUSINESS.SERVICE.RULES tables with a Release less than the new rule book year to history.

The Delivery Transformation Layer covers the property files containing information on queues, file paths, and routing logic. The new MX messages could impact these property files.

Therefore, any necessary changes to the property files for those new messages are released as part of the pack and are referred to, only when those new messages are routed through the delivery framework.

The XML schema definition (XSD) is a framework document that defines the rules and constraints for XML documents. XSDs are provided to formally define the structure of all ISO 20022 XML messages.

In the event of any changes to the ISO20022 message as part of the CBPR+ rule book changes, a new schema version is issued by SWIFT resulting in potential modifications in the payload. Temenos releases new XSDs and XSLTs under a dedicated license code to handle these modifications.

The Schema Path and Stylesheet Path fields in the DE.CARRIER application can be used to allow the delivery framework to access the latest XSD and XSLT version when generating XMLISO messages. When generating the XML message, the delivery framework accesses the required XSDs and the XSLTs from the file path defined in the DE.CARRIER application.

It is mandatory that banks place the necessary artefacts in the file paths configured in DE.CARRIER when a new rulebook is activated. If the file path is not defined in the Delivery carrier or if the required artefacts are not available in the respective file path, the Delivery framework refers to the necessary from the default folders.

• The

and

fields apply exclusively to the outbound messages generated by the Delivery framework.

• To ensure schema validation of incoming messages, banks must manually update the latest schema in the default folder.


#### 🔧 Working With

The Delivery module supports the implementation of annual rulebook updates for CBPR+ messages and other ISO20022 solutions. The business verticals use the message framework to send and receive CBPR+ messages and other ISO20022 messages.


##### Activating Delivery Carrier for Each Rulebook

The annual maintenance license code includes the Delivery carrier configuration that applies to the rulebook, which will be activated when the user enables the corresponding rulebook year in SWIFT.PARAMETER .

Until the new rulebook is activated, both the regular carrier configuration and the rulebook specific carrier configuration will be available in DE.CARRIER and the Delivery framework will refer to the regular carrier configuration to send and receive messages. Therefore, to differentiate between the regular carrier configuration and the rulebook-specific carrier configuration, the ID of the rulebook-specific carrier will indicate the rulebook year to which the configuration applies.

Once the new rulebook is activated in SWIFT.PARAMETER , the system replaces contents of the regular carrier record with the rulebook-specific carrier record that corresponds to the relevant rulebook, thus enabling the carrier configuration for that rulebook. Subsequently, the carrier record that is specific to the rulebook will be deleted.

1. The bank is currently operating on the 23 AMR release and the rulebook 2023 is already enabled in SWIFT.PARAMETER .
2. The user installs the CBPR24 module resulting in the release of a Delivery Carrier with CBPRPLUS-2024 record.
3. The user creates the CBPRPLUS record in SWIFT.PARAMETER and sets Curr Swift Rel to 2024.
4. The system replaces the contents of the CBPRPLUS record with the CBPRPLUS-2024 record and deletes the latter record.
5. The user acquires and installs the CBPR25 module, resulting in the release of CBPRPLUS-2025 record.
6. The user then activates Curr Swift Rel 2025 in the CBPRPLUS record of SWIFT.PARAMETER .


#### 📋 Tasks

There are no Tasks available for MX Messages Framework feature.


#### 📊 Outputs

There are no Outputs available for MX Messages Framework feature.


> **Related Applications:** `DE.BUSINESS.SERVICE.RULES`, `DE.CARRIER`, `DE.DISTINGUISH.NAME.RULES`, `DE.MESSAGE`, `DE.PRODUCT`, `SWIFT.PARAMETER`

---


### 2.22  Recovery DeliveryTables


> **📇 Quick Reference Card**
> 
> **Purpose:** *After a system failure, the Temenos Transact database is restored and if possible it is rolled back to shortly before the system failure occurred.*
> 
> **Applications:** `DE.DISP.CONTROL`, `DE.I.HEADER`, `DE.INWARD.ROUTING`, `DE.O.HEADER`, `DE.SENT.SWIFT`, `DE.SENT.TELEX`, `SPF`
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

After a system failure, the Temenos Transact database is restored and if possible it is rolled back to shortly before the system failure occurred.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 🔧 Working With

The SPF application is updated with the crash time. At this stage, the delivery messages which may have been processed and sent out before the crash, is in the unmapped queue. Due to the recovery system, the messages have the same delivery ID, as it was when they were created before the system failure. The delivery ID of messages has the date time stamp, which is the date and time the messages were originally created.

In the event of a system failure, the DE.DISP.CONTROL and DE.INWARD.ROUTING applications are not recovered. Records are input to the DE.DISP.CONTROL and DE.INWARD.ROUTING applications, to deal with current circumstances. As a result, neither of these applications are recovered, as the circumstances may have changed and recovery of these applications have become irrelevant.

When the delivery system receives an acknowledgement from a SWIFT or telex device, that a message has reached its destination, it records the message ID (either in the DE.SENT.SWIFT application or in the DE.SENT.TELEX application, as appropriate). In the event of a system failure, neither of these applications are restored. If the applications are still readable they are used, otherwise, they are cleared.

All other applications in the delivery system uses the standard Temenos Transact recovery techniques. The applications which contain the messages, message headers and indices to the messages have a recovery system of their own.

The delivery services should be started as normal. Each message passes through mapping and formatting as normal. As each message is processed by the appropriate carrier control module, the date timestamp of each SWIFT or telex message is compared to the crash time in the SPF application. The messages created after the system failure (that is, messages with IDs after the crash time) are sent out as normal. The messages created before the system failure (that is, messages with IDs before the crash time) are not sent if their IDs are in the DE.SENT.SWIFT or DE.SENT.TELEX applications, as appropriate.

If a message was created before the system failure but is not in the appropriate sent application, the message is sent out as possible duplicate entry (PDE). If the DE.SENT.SWIFT or DE.SENT.TELEX applications are unreadable after a system failure they are cleared, so all messages subsequently processed which were created before the system failure are sent out as PDEs.

The same reason that neither DE.DISP.CONTROL nor DE.INWARD.ROUTING application can be restored also applies to DE.O.HEADER and DE.I.HEADER applications. When the DE.FORMAT.PRINT application is recovered, the sample print layouts are not reproduced.

> **⚠️ Note:** If the input function is used to change the fields in the DE.O.HEADER and DE.I.HEADER applications, as these changes may have to be re-applied after a recovery, if the conditions for the original changes still apply.


#### 📋 Tasks

There are no Tasks available for Recovery of Delivery Applications feature.


#### 📊 Outputs

There are no Outputs available for Recovery of Delivery Applications feature.


> **Related Applications:** `DE.DISP.CONTROL`, `DE.I.HEADER`, `DE.INWARD.ROUTING`, `DE.O.HEADER`, `DE.SENT.SWIFT`, `DE.SENT.TELEX`, `SPF`

---


### 2.23  Relationship Management Authorisations


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Central Relationship Management (CRM) portal allows banks to define and manage the authorisations to exchange SWIFT messages. The platform enables SWIFT to validate the authorisations centrally, when the banks exchange messages through either SWIFT FIN or SWIFT FINPlus service.*
> 
> **Applications:** `EB.FREE.MESSAGE`, `EB.QUERIES.ANSWERS`, `POR.TRANSACTION`, `PP.NO.RMA`, `PP.RMA`, `RMA.FILE.UPLOAD.DETAILS`, `RMA.PARAMETER`, `RMA.PARAMTER`
> 
> **Key Fields:** *MessageTypInclude*, *MessageTypeExcluded*, *MessageTypeInclude*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The Central Relationship Management (CRM) portal allows banks to define and manage the authorisations to exchange SWIFT messages. The platform enables SWIFT to validate the authorisations centrally, when the banks exchange messages through either SWIFT FIN or SWIFT FINPlus service.

RMA authorisations are of two types - Authorisation to receive and authorisation to send.

Temenos bank, as RMA receiver bank, initiates the authorisation to receive as an indicator to its counterparty that Temenos bank allows them to send messages. The counterparty, which is now the RMA receiver bank, can accept or reject the authorisations.

Temenos bank counterparty, as an RMA sender bank, initiates the authorisation to send as an indicator to the RMA receiver bank that counterparties are allowed to send messages. Temenos bank can accept or reject the authorisation.

The RMA sender bank can indicate a future start date, from which the authorisation will be enabled, provided that is accepted by the RMA receiver bank. If the RMA sender bank does not specify a start date, the authorisation is enabled when the RMA receiver bank accepts authorisation.

The RMA sender bank can also specify a future end date. An active authorisation which has future end date expires when it reaches the end date. The RMA sender and receiver banks have the option to stop this authorisation, where the RMA sender bank can revoke the authorisation and the RMA receiver bank can delete it.

The actions of the RMA party and how it impacts the status of the RMA authorisation are shown below.

- RMA Authorization (SWIFT Central platform) – Happy Path
- RMA Authorization (SWIFT Central Platform) – Unhappy Path

The authorisation process takes place in the RMA central platform. The portal provides an option that allows banks to manually or automatically download RMA distribution files, which contain all the authorisations and the changes occurred during a certain period or after the last download. Banks can import and use the files in their systems while processing transactions.

> **⚠️ Note:** At any point in time, only one received authorisation can be active (enabled) for a counterparty and a SWIFT service.

If the sender or receiver bank changes an existing authorisation in the central RMA platform, the RMA record in the next complete or partial file contains all the authorisation details including the updated ones. The issue date and time of the authorisation indicate when the authorisation has been modified. If an existing authorisation is revoked or deleted, the RMA record in the next complete or partial file specifies the issue date and time of the authorisation, but not the time when it was revoked.

As the SWIFT RMA portal validates the RMA authorisations centrally for the SWIFT services that have the RMA feature enabled, for example, FIN and FINPlus, the banks do not need to perform an RMA check for the inward messages.

However, in order to reduce the exceptions and avoid the possibility that SWIFT will reject the outward messages, the banks can check the RMA authorization before they send messages to SWIFT. Banks can consider the 'Authorisations to Receive' issued by their counterparties to send them messages. The Temenos RMA directory stores the 'Authorisation to Receive' records of the counterparties and is referred by TPH as well as other modules during transaction processing.

The Temenos No RMA directory maintains the message type for which no authorization is required. With the adoption of the ISO 20022 for cross border payments, banks can establish separate authorisations for SWIFT FIN messages versus the ISO20022 messages exchanged over SWIFT Finplus service. If the user enables the RMA feature, the Temenos RMA and No RMA directories allow the bank to maintain the authorisation per service. If the RMA is not enabled, the bank can specify the allowed or excluded message types irrespective of the service.

Banks can manually capture the authorisations in the directories, or upload the RMA distribution files sent or downloaded by the SWIFT central RMA portal. To upload the RMA files, the bank must install and obtain license for the Temenos RMA Adapter.

Read the Temenos RMA Adapter user guide for more information.


#### ⚙️ Configuration

RMAs can be parameterised in the following applications that are part of the Delivery module.


##### ConfiguringRMA.PARAMETER

This application allows the bank to define the main characteristics of the RMA check.

The ID of the record is ‘System’ as the characteristics set here affects all the companies. The Enhanced Directory field indicates if the authorisations are maintained per service type, if enabled or not.

> **⚠️ Note:** The system supports the RMA distribution file only when the Enhanced Directory field is enabled

If the Enhanced Directory field is enabled and the business application which invokes the RMA check supplies the correspondent BIC and the message type, but not a service, the system uses either the Default MT Service (when the supplied message type starts with a digit) or the Default MX Service (when the supplied message type does not start with a digit) to determine the appropriate authorisation for the respective message type and service.

The Default MT Service field indicates the default SWIFT service for MT messages and the Default MX Service field indicates the default SWIFT service for MX messages.

Once the Enhanced Directory enabled, it cannot be disabled.


##### ConfiguringPP.NO.RMA

The bank can configure the FIN and ISO20022 message types that do not require authorisation in the PP.NO.RMA application. These message types can be exchanged with any counterparty.

The ID of the record is formed as below:

- 'MessageType-service-StartDate' if the Enhanced Directory is enabled in the RMA.PARAMETER application
- 'MessageType-StartDate' if the Enhanced Directory is disabled or blank or no record is configured in the RMA.PARAMETER application. (MT and ISO20022 message type can be used).

Start Date is the date from which the system doesn’t require an authorisation for the respective message type or the respective message type of the SWIFT service. Refer to sample the screenshot below.


##### ConfiguringPP.RMA

This application allows the bank to define the received authorisations issued by their counterparties.

The ID of the record is formed as below:

- If the Enhanced Directory field is enabled in the RMA.PARAMETER application, the PP.RMA record ID follows the pattern BIC8-service-StartDate.
- If the Enhanced Directory field is disabled or blank, or there is no record configured in the RMA.PARAMETER application, the record ID follows the pattern BIC8-Start Date.

The fields in PP.RMA application are given below:

- StartDate - The issue date of the authorisation
- CompanyID - The company ID for which the RMA record has been created
- SwiftService - The SWIFT service for which the RMA applies if the Enhanced Directory is enabled (If the Enhanced Directory is not enabled, it is ignored)
- MessageTypeInclude - The message types which can be exchanged to counterparty For MessageTypeInclude , the bank can specify three character message types. For example, 103 or they can use '*' as a wildcard character, like 1* to represent any message type in Category 1.
- MessageTypeExclude - The message types which cannot be exchanged with the counterparty For MessageTypeExclude , the bank must use the first two elements that are part of the ISO20022 message name, pacs.008, or they can use '*' as a wildcard character, like pacs* to represent any pacs message type. Comma must be used as a separator between the message types.

- IssueDateTime - The date and time when the authorisation has been issued
- ValidFrom - The date from when the authorisation can be used

> **⚠️ Note:** If not specified, the authorisation can be used from the issue date.

- EndDate - The date up to which the authorisation can be used
- AuthType - The type of the relationship authorisation Only the Received authorisations are captured.
- Issuer - BIC8 of the correspondent who issued the authorisation to receive messages from the Temenos Bank
- UploadType - Type of the authorisation how it has been created or amended The valid options of this field are: Blank - Indicates that the relationship authorisation record has been created manually Partial - Indicates this has been created or updated by a partial file upload Complete - Indicates this has been created or updated by a complete file upload
- UpldFileName - The name of the uploaded file through which the record has been created or amended
- UpldFileCreateDateTime - The create date and the time of the file through which the record has been created or amended

> **⚠️ Note:** If the RMA record is created based on the automated upload of the RMA distribution file using the Temenos RMA Adapter, the PP.RMA application also stores the file name.

If Enhanced Directory is blank in the RMA.PARAMETER application, the bank should define the authorisations to send them in the following ways:

- To send all the FIN category 1 messages to the counterparty, 1* must be indicated in the MessageTypeInclude field.
- To send all the FIN category 1 messages to the counterparty, except for MT104 and MT107, 1* must be indicated in the MessageTypeInclude field and 104, 107 must be set in the MessageTypeExclude field.
- To define an entry that excludes the authorisation to send any category 2 messages except for the MT202, 202 must be captured in the MessageTypeInclude field. A specific entry takes precedence over the wildcard entries. For example, the included 202 takes precedence over the excluded 2*.

If Enhanced Directory is enabled in the RMA.PARAMTER application (manual entries), the bank should define the authorisations to send in the following ways:

- To send all the FIN Category 1 messages to the counterparty, the counterparty BIC, swift.fin, and the start date must be indicated in the record ID and 1* must be indicated in the MessageTypeInclude field. The swift.fin value is default in SwiftService field.
- To define the authorisation with pacs.008 and pacs.009 messages to the counterparty, the counterparty BIC, swift.finplus, and the start date must be indicated in the record ID, and pacs.008, pacs.009 must be indicated in the MessageTypeInclude field. The swift.finplus value is available in the SwiftService field.
- To send all the FIN Category 1 messages to the counterparty, with the exception of MT104 and MT107, the counterparty BIC, swift.fin, and the start date must be indicated in the record ID. 1* must be indicated in the MessageTypeInclude field and 104, 107 must be set in the MessageTypeExclude field. The swift.fin value is available in SwiftService field.

If the bank uses the Temenos RMA adapter to automatically upload the RMA distribution files, the PP.RMA records are created or updated automatically based on the details available in the file.


##### ConfiguringRMA.FILE.UPLOAD.DETAILS

This application stores the details of the RMA distribution files uploaded to Temenos RMA directory. The distribution file can contain authorisations for multiple companies (identified by the BIC8 of the crsp tag in the RMA records for which the type is “Received”) and multiple service.

Each time a distribution file is received, if there is at least one authorisation received for the company BIC, the Temenos RMA Adapter creates or updates a record with the ID formed as CompanyId-Service with the below fields:

- Part File Create Dt - The create date and time from the last partial RMA distribution file uploaded in the PP.RMA which had received authorisations for the respective company and service
- Part File Name - The name of the latest partial file uploaded in PP.RMA
- Part File Upld Datetime - The date and time when the latest partial file has been uploaded
- Comp File Create Dt - The create date and time indicated in the last complete RMA distribution file uploaded in the PP.RMA
- Comp File Name - The name of the last complete file uploaded in PP.RMA
- Comp File Upld Datetime - The date and time when the latest complete file has been uploaded
- Initial Archival Run - Updated by the system with the date when the first complete file has been uploaded


#### 🔧 Working With

The Delivery module allows the Temenos Infrastructure based modules to validate if there is an active (enabled) authorisation to permit the bank to send the respective message type to a certain counterparty identified by its BIC8.

By default, the RMA check doesn’t consider the SWIFT service when it validates the RMA authorisation. The RMA.PARAMETER application allows the bank to indicate that the authorisations are maintained per service and that the service is considered when it performs the RMA check.

Read the Configuration section for more information.


##### RMA Check

When a Temenos infrastructure based module invokes the RMA check, it supplies the corresponding BIC, message type and the optional SWIFT service. In this case, the Delivery module ignores the SWIFT service and checks the setup in the PP.NO.RMA application. If a record is found for that message type and the start date is either the current business date or a date in the past and the end date is a date in the future, the Delivery module considers the authorisation is for the respective message type. The bank can configure the message types for which the SWIFT does not require any authorisations to send such messages (for example, 99n message types).

If there is no record in PP.NO.RMA for the respective message type, the Delivery module checks the PP.RMA application if there is an authorisation for the respective counterparty with:

- The valid from date (or start date).
- The issue date of the authorisation if no valid from date is defined.
- The current business date or a date in the past and the end date in the future (if the end date is defined).

If the PP.RMA record is either not found or found, but its Status field is not enabled or left blank, then the RMA check does not pass.

If the PP.RMA record is found, the Delivery module verifies both the MessageTypeInclude and MessageTypeExclude fields. The most specific parameterisation for the message types in the fields take precedence, for example, 202 included takes precedence over 2* excluded, and the 103 excluded takes precedence over 1* included.

Temenos Payments Hub (TPH) is using the Delivery framework to perform RMA Check for cross border payments over SWIFT network.

The following screenshot shows the RMA setup for the counterparty identified by the BOFAUS30 BIC. The message types that can be sent to this counterparty are defined in the MessageTypeInclude field.

A credit transfer is initiated in TPH, the channel for the payment is SWIFT MX, which implies that ISO20022 messages are sent. The instructed agent (receiver of the pacs.008 message) is BOFAUS30. TPH invokes the RMA Check for the message type pacs.008 and receiver BOFAUS30.

The Delivery module performs the RMA Check – there is no PP.RMA for message type pacs.008 and therefore it checks if there is a PP.RMA record for the receiver (BOFAUS30). As the record exists and the message type pacs.008 is specified in the MessageTypeInclude , the Delivery module indicates to TPH that the RMA Check is passed. TPH does not raise any error.

The following screenshot shows the configuration of PP.RMA for the receiver BOFAUS30. This indicates that the bank can send to this receiver any message from Category 3, 4, 5 and the pacs.008, pac.004 and pacs.002 are specifically excluded.

A user initiates a credit transfer in TPH, the channel for the payment is SWIFT MX, which implies ISO20022 messages. The instructed agent (receiver of the pacs.008 message) is BOFAUS30. TPH invokes the RMA Check for the message type pacs.008 and receiver BOFAUS30.

The Delivery module performs the RMA Check – there is no PP.NO.RMA for message type pacs.008 and therefore it checks PP.RMA for the receiver (BOFAUS30). A PP.RMA record is found for the receiver in which the message type pacs.008 is specified in the MessageTypeExcluded field. The Delivery module indicates TPH that the RMA Check has failed and therefore TPH raises an error.

The EB.QUERIES.ANSWERS and EB.FREE.MESSAGE are using Delivery framework to perform RMA Check for the MT messages they are generating.

The following screenshot shows the configuration of the PP.RMA application for the counterparty KKMTUSBN. This indicates that the bank can send to this receiver any message from Category 1, 2 and 9 with the exception of the 195 message for which the authorisation is excluded.

In the following screenshot, the user creates a cancellation request for the receiver BIC KKMTUSBN using the EB.QUERIES.ANSWERS application, and the message type is 192.

Considering the above RMA setup, the authorisation for the receiver KKMTUSBN counterparty for the message type 192 is present ( as the parameterisation of 1* in the MessageTypInclude field covers the 192 message type as well as any other message in Category 1 apart than 195) and valid (the processing date for the cancellation request is 28 Dec 2009) and therefore EB.QUERIES.ANSWERS does not raise an override when the cancellation request is committed.

Consider the following setup for the receiver BIC KKMTUSFN.

A free message is initiated to the receiver SW-KKMTUSFN for message type 199. As this message type is configured as an excluded message type for the receiver, an override message is prompted for this free message, as shown in the following screenshot.

The RMA is not configured for the receiver, SW-KKMTUSGN.

When a cancellation request is raised through the EB.QUERIES.ANSWERS application for this receiver BIC, the system prompts an override message as there is no authorisation for this counterparty and message type.


##### Enhanced RMA Check

When a Temenos Infrastructure based module invokes the RMA check, it supplies the correspondent BIC, message type and the optional SWIFT service. If the service is not supplied, the Delivery module refers the setup in the RMA.PARAMETER . If the message type starts with a digit, it considers the value defined in the Default MT Service field else the value populated in the Default MX Service field. The Delivery module then checks the setup in the PP.NO.RMA application. If a record is found for that message type service and the start date is either the current business date or a date in the past and the end date is either not defined or a date in the future, then RMA skips the check and the system does not require an authorisation.

If there is no PP.NO.RMA record for the respective message type and service, the Delivery module checks whether the business application has supplied the date, then it considers the PP.RMA record which has the ID equal to the correspondent BIC8, service, message type, and the supplied date. If not found, then it considers the latest PP.RMA record for that BIC and service which has the start date (issue date) valid from the date less than or equal to the supplied date.

If the business application has not supplied a date, then the Delivery module considers the latest PP.RMA record for that BIC and service which has the start date (issue date) valid from the date less than or equal to the current calendar date.

If the PP.RMA record is either not found or found, but its Status field is not set as Enabled or is left blank, then RMA check does not pass. Similarly, with the regular RMA check, if the PP.RMA record is found, the Delivery module verifies both the MessageTypeInclude and MessageTypeExclude fields. The most specific parameterisation for the message types in these fields take precedence. For example, 202 included takes precedence over 2* excluded, and the 103 excluded takes precedence over 1* included.

Consider an example where valid authorisation exists for the receiver (both message and service is included)

The following screenshot shows the RMA setup for the counterparty identified by the BIC, CITIFRPP. The message types that can be sent to this counterparty are defined in the MessageTypeInclude field and service type is included in SwiftService .

The user can initiate a credit transfer in TPH. The channel for the payment is SWIFT MX, which implies that ISO20022 messages are sent. The instructed agent (receiver of the pacs.008 message) is CITIFRPP. TPH invokes the RMA Check for the message type as pacs.008, swift service as swift.finplus and receiver CITIFRPP.

The Delivery module performs the RMA Check. If there is no PP.NO.RMA record for message type pacs.008, it checks if there is a PP.RMA record for the receiver (CITIFRPP) and SWIFT service as SWIFT.finplus. As the record exists and the message type pacs.008 is specified in the MessageTypeInclude , the Delivery module indicates to TPH that the RMA check is passed. So, the TPH does not raise any error.

A sample order entry is shown in the below screenshot.

A sample for POR.TRANSACTION is show below.

The following screenshot shows the configuration of PP.RMA for the receiver CITIUS33. This indicates that the bank can send to this receiver ALL 2 series messages and MT 195 message is specifically excluded. The service type swift.fin is included in SwiftService .

A user initiates a credit transfer in TPH. The channel for the payment is SWIFT MT and the instructed agent (receiver of the MT 103 message) is CITIUS33. TPH invokes the RMA Check for the MT 103, swift service as swift.fin and receiver CITIUS33.

The Delivery module performs the RMA Check. There is no PP.NO.RMA for MT 103 and so it checks PP.RMA record for the receiver (CITIUS33).

A PP.RMA record is found for the receiver in which 2* is specified in the MessageTypeIncluded field and 194 is specified in the MessageTypeExcluded field.

The Delivery module indicates TPH that the RMA check is failed. So, the TPH raises an error.

A sample screenshot for order entry is show below.


##### Archival Process

A housekeeping process that allows the bank to move the obsolete records in history. The process covers the following scenarios:

- The existing RMA records, created before the bank enabled the enhanced feature for the RMA Directory, must be removed after the initial file upload.
- Regular archive of records that are made obsolete by new or complete or partial file uploads.

> **⚠️ Note:** The Initial Archive Run field is set to blank when a PP.RMA.FILE.UPLOAD record is created by the SWIFT RMA Adapter.

The DE.RMA.MOVE.TO.HIS service automatically moves the following cases to history:

- Any PP.RMA record which has been created before the file upload (the PP.RMA key formed by the BIC8-date) and then changes the Initial Archive Run field to Yes in the respective RMA.FILE.UPLOAD.DETAILS record.
- Any PP.RMA record which has the UploadFileDateTime field less than the CompleteFileDateTime field in the RMA.FILE.UPLOAD.DETAILS application. This ensures all the records created by complete or partial upload, older than the latest complete file are archived.
- Any PP.RMA record which has the Status field either not enabled or blank or has the EndDate field in the past. This ensures any revoked or deleted or expired authorisation is moved to history.


#### 📋 Tasks

There are no Tasks available for Relationship Management Authorisations feature.


#### 📊 Outputs

There are no Outputs available for Relationship Management Authorisations feature.


> **Related Applications:** `EB.FREE.MESSAGE`, `EB.QUERIES.ANSWERS`, `POR.TRANSACTION`, `PP.NO.RMA`, `PP.RMA`, `RMA.FILE.UPLOAD.DETAILS`, `RMA.PARAMETER`, `RMA.PARAMTER`

---


### 2.24  Request for Transfer of Funds


> **📇 Quick Reference Card**
> 
> **Purpose:** *Swift message MT101 (Request for Transfer) is sent by a financial institution on behalf of a non-financial institution account owner, that is, the ordering customer or instructing party. It is subsequently received by the receiving financial institution and processed by the receiving financial insti...*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Swift message MT101 (Request for Transfer) is sent by a financial institution on behalf of a non-financial institution account owner, that is, the ordering customer or instructing party. It is subsequently received by the receiving financial institution and processed by the receiving financial institution or the account servicing financial institution.

The MT101 message is used to order the movement of funds:

- Between ordering customer accounts , or
- In favour of a third party, either domestically or internationally.

The MT01 consists of two sequences:

- Sequence A – General Information is a single occurrence mandatory sequence and contains information to be applied to all individual transactions detailed in sequence B.
- Sequence B – Transaction Details is a repetitive sequence; each occurrence provides details of one individual transaction. Fields which appear in both sequences are mutually exclusive.


#### ⚙️ Configuration

Covered as part of module configuration and there is no specific configuration for this feature.


#### 📋 Tasks

There are no Tasks available for Request for Transfer of Funds feature.


#### 📊 Outputs

There are no Outputs available for Request for Transfer of Funds feature.

---


### 2.25  Soft Delivery


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Soft Delivery mechanism enables the user to control the creation of the delivery messages, whether in the form of SWIFT messages or PRINT output. This is achieved by defining activities that can generate a specific message type at each stage of a contract life cycle.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The Soft Delivery mechanism enables the user to control the creation of the delivery messages, whether in the form of SWIFT messages or PRINT output. This is achieved by defining activities that can generate a specific message type at each stage of a contract life cycle.


#### ⚙️ Configuration

This section explains the configuration of the Soft Delivery mechanism. The main concept of Soft Delivery is to define every stage in the life cycle of a contract as a discrete event, by means of defining activities on the EB.ACTIVITY application. Each of these events are unique to the business application.

The delivery messages relating to each of these events may, if required, can be produced prior to the event. The number of days in advance of the event that the messages are produced is defined in the Days Prior Event field in the EB.ACTIVITY application.


##### EB.MESSAGE.CLASS

This application is used to classify SWIFT message types into different message classes such as CONFIRMATION, ADVICE and PAYMENT. The users have the flexibility to classify SWIFT message types in the EB.ADVICES application and can control the production of the eventual messages from the main contract.

For example, a contract amendment activity has been defined to produce a confirmation and payment advice. If, for some reason, the production of the payment advice for a particular contract is to be suppressed, a user can set NO to send advice on that contract instead of changing the EB.ADVICES record to stop the payment advice and change back afterwards.


#### 📋 Tasks

There are no Tasks available for Soft Delivery feature.


#### 📊 Outputs

There are no Outputs available for Soft Delivery feature.

---


### 2.26  StaticProcessing Messages


> **📇 Quick Reference Card**
> 
> **Purpose:** *Most of the online transactions in Temenos Transact send messages. For example, when a Funds Transfer (FT) transaction is entered and approved, it usually requires to send a credit advice to one address and a debit advice to another, together with one or more payment cables. In addition, some overni...*
> 
> **Applications:** `)`, `,`, `.HEADER`, `ADDRESS`, `BATCH`, `DE`, `DE.ADDRESS`, `DE.ALTERNATE` ... +14 more
> 
> **Key Fields:** *Ack*, *C*, *Code*, *Copies*, *D*, *Data*, *Disposition*, *Error* ... +7 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Most of the online transactions in Temenos Transact send messages. For example, when a Funds Transfer (FT) transaction is entered and approved, it usually requires to send a credit advice to one address and a debit advice to another, together with one or more payment cables. In addition, some overnight processing, such as the processing of standing orders, requires the payment messages to be sent.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 🔧 Working With

When an online transaction or overnight process requires the sending of a message, the delivery process APPLICATION.HANDOFF is invoked. This passes all the details of the message to the delivery system, while passing back a unique identifier to the application, the delivery message ID and the message is mapped.

The main processes within delivery, that is, formatting and the carrier control processes are run as Temenos Transact services ( TSA.SERVICE ) which are continuously running throughout the day and during the Close of Business (COB) processing.

The mapping stage examines the raw data created by the Delivery Header applications ( DE.I.HEADER or DE.O.HEADER ) and a Message Detail record is created using the mapping rules described in the DE.MAPPING application. Then the message is placed in the unformatted queue identified by the carrier type.

The appropriate DE.PRODUCT record is read, which determines:

- To whom the message should be sent.
- How many copies to be sent.
- Which carrier should be used.

The formatting services examine the unformatted queue for the carrier concerned and process the messages using one or more agents. The carrier (as specified in DE. PRODUCT ) is used to access the DE.CARRIER application. The DE.CARRIER application contains the carrier to be used for formatting, address lookups, the carrier module and the interface to be used.

The DE. PRODUCT application specifies a carrier of TELEX. The carrier record specifies for telex that TELEX record should be used for the address record lookups, SWIFT should be used for formatting, the GENERIC carrier control program should be used and the interface should be TELEXBOX. The DE.ADDRESS application is accessed to determine the address to which the message should be sent, for example, the print address, the SWIFT ID, the telex number, and the like. The appropriate format applications (for example, DE.FORMAT.PRINT, DE.FORMAT.SWIFT ) are read to determine how the message should be formatted, how to generate a formatted print and SWIFT message.

However, there can be various exceptions, as follows:

- If a message is to be held, for example, it is not required to send the message out until business reopens in Tokyo at the start of the next working day, the message can be placed on the HOLD queue.
- If the message is being sent by TELEX, the message might be specified as being suitable for batching, in which case it is placed in the batching queue. Once a batch is complete, it is removed from the batching queue.
- If the message is being sent by TELEX, the message might require the input of a test key, in which case the message is placed in the awaiting test key queue (this may include batched messages). Once the test key has been input and authorised, the message is placed on the formatted telex queue.
- If an error is detected during the formatting of the message, the message is placed in the repair queue. The message stays in the repair queue until the Delivery Operator corrects the problem and resubmits the message. Messages can also be placed in the repair queue at any stage during the processing of the messages within delivery. It is the responsibility of the Delivery Operator to examine the contents of the repair queue regularly and correct any problems highlighted.

The DE.MM.TIMECHECK service, continuously examines the HOLD queue to check if there are any messages that should be released. For example, if a message was to be held until 16:00 and it is now past that time, the message should be released. Released messages are removed from the HOLD queue and placed in the appropriate formatted queue.

> **⚠️ Note:** For telex messages, the messages are placed in the batching queue, awaiting test key queue or the formatted telex queue.

The DE.PRINT control process sends the printed formatted messages to the appropriate spool queues, placing a copy of the formatted message on the HISTORY table.

The SWIFT.OUT carrier control process sends the SWIFT formatted messages to the SWIFT device, for example, ST400. Integrity checking exists within the ST400. If this fails, the message will be rejected immediately, but normally the message will be sent to the SWIFT network. Then the message is placed in the awaiting acknowledgement queue.

The SWIFT.IN carrier control process receives the resulting acknowledgement (ACK) or negative acknowledgement (NAK) from the ST400 for the messages sent out by the outward SWIFT carrier control process (SWIFT.OUT). If an ACK is received, the message will be removed from the awaiting acknowledgement queue, is flagged as having been sent correctly and a copy of the formatted message placed in the HISTORY table. If a NAK is received, the message will be removed from the awaiting acknowledgement queue and placed in the repair queue. The inward SWIFT carrier control process (SWIFT.IN) can also receive messages from the SWIFT network destined for Temenos Transact . The messages are placed in the unformatted inward queue. The SWIFT messages can be sent to or from, either the ST400 or alliance using the CASmf protocol. This is achieved using the DE.CC.GENERIC generic service.

The generic carrier control service processes the messages for any carrier using the generic interface (that is, the CARRIER.MODULE in DE.CARRIER is specified as GENERIC). Each message processed is handed to the interface routine specified in the interface record in DE.INTERFACE , and is handled accordingly. If ACKs are required (the Ack Required field is set to Y in DE.INTERFACE ), the messages are placed in the awaiting acknowledgement queue. When the ACK is received (from the inward routine) or if ACKs are not required, the message are set as having been sent correctly and a copy of the formatted message is placed in the HISTORY table. If a NAK is received, the message is removed from the awaiting acknowledgement queue and placed in the repair queue. For each generic carrier, the incoming messages received from the inward interface routines are placed in the unformatted inward queue.

The inward formatting services take formatted SWIFT and telex messages, and reformats them into the raw message details (similar to how the message would have been produced by the Temenos Transact applications). If an error is detected in the reformatting of a message, it is placed in the inward repair queue, for the Delivery Operator to correct.


##### Starting the Queues and Services

Formatting is controlled by a service for each carrier, so there are records such as SWIFT.OUT and TELEX.OUT in TSA.SERVICE , this allows the formatting to be scaled up to larger workflows. Each service can be run separately and the appropriate number of agents can be given to deal with the volume for that carrier.

Generic delivery has records for DE.CC.GENERIC.IN and DE.CC.GENERIC.OUT services, and has the user defined carriers to run specified in the BATCH records using the Data field.

TSA.SERVICE management controls these services either on a start/stop basis or automatically. The processing is common and the same concept is used for running the Close of Business processes (COB).


##### Displaying the State of Messages

Messages can be passed to delivery:

- From an application.
- From the COB processor.
- Received from an external device, such as SWIFT or telex.

Each message is given a unique identifier as the message ID. The message ID is composed as XYYYYMMDDNNNNNSSSSSSQQ, where:

- X is the D-message which is to be delivered (outward message) or R-message which are received (inward message).
- NNNNN is the system user number of the inputter.
- YYYYMMDD is the format of the date.
- SSSSSSS is the time in seconds, since midnight.
- QQ is the sequence number of transactions within a second.

This unique ID is used throughout the life of the message, regardless of which queue the message is currently in. Once the message has been through mapping, a record is created in the DE.O.HEADER with this ID. To check the current status of the message, the user can find the record in the DE. I .HEADER or DE.O.HEADER applications. The Disposition and Message Disposition are the status fields in the DE. I .HEADER or DE.O.HEADER applications.

When the message has been through mapping, but has not been formatted, the DE.O.HEADER record is created with the Disposition field set to UNFORMATTED. If mapping fails, the Disposition field is set to REPAIR. During formatting, the Disposition field is temporarily set to SELECTED before being reset to FORMATTED. This Disposition field refers to the message as a whole and is set to FORMATTED, even though individual copies of a message may be in repair.

Formatting causes the DE. I .HEADER or DE.O.HEADER records to expand to include a multi-value set of data for each copy of message, and each is set with its own Msg Disposition field. If a problem prevents the expansion of a message, such as, a missing DE.PRODUCT record, then the Disposition field is set to REPAIR.

However, problems that relate to the detailed formatting of message fields, result in the Disposition field being set to FORMATTED and the Msg Disposition field with REPAIR, being set in the appropriate place in the multi-value fields at the end of the record. From this point on, the individual copies of each message are dealt separately and can be placed in separate queues. So that it is apparent which copy of the message is on which queue, the message ID is appended with the copy number as XYYYYMMDDNNNNNSSSSSQQ.C, where C is the copy number.

Once a message has been formatted, each copy of the message is put in the formatted queue appropriate to the carrier with the Msg Disposition field set to FORMATTED. However, if the carrier is TELEXP and the message is of normal priority, then the message is placed in the batching queue, if batching is required for this message. The messages to be batched are placed in the batching queue with Msg Disposition field set to BATCHING until the batch is complete. The completed batches and individual telex messages which do not require batching are placed in the awaiting test key queue (if a test key is required) with the Msg Disposition field set to ATK (awaiting test key). Once the test key has been entered successfully, the message is placed in the formatted queue, with the Msg Disposition field set to FORMATTED.

The carrier control modules for SWIFT and TELEX, passes the message to the carrier device and sets the Msg Disposition field to WACK (awaiting acknowledgement). If the message is successfully received by the recipient (the carrier device receives an acknowledgement), the Msg Disposition field is set to ACK (acknowledged). The Msg Disposition field can also have the value of RESUBMITTED and REROUTED.

The business applications map the messages and the service agent deals with each carrier type individually, the need for different queue displays is not required any longer. Appropriate users can create customised enquiries, which are suitable for their business than using a generic one.

- DE.O.HEADER is basis to use for outward messages.
- DE.I.HEADER is equivalent for inward messages.

The users may want to create enquiries for the purpose such as:

- Inward messages in repair requiring intervention.
- Outward messages in repair requiring intervention.
- Message awaiting acknowledgement.


##### Reprinting messages

Printed messages can be accessed either using the RESUBMIT option in the Msg Disposition field in DE.O.HEADER or it can be accessed using the copy of the message in the HOLD.CONTROL application.

If a printed copy of a message which was sent by means other than print is required (for example, a SWIFT message), then the message can be viewed in the Outgoing Message Details (OUTGOING.MSG.DETS) enquiry and the message can be printed through this enquiry.


##### Repairing Messages

There are number of reasons for the messages being placed in repair, that is, if there is something wrong with the message and which the Delivery Operator should investigate and is able to correct. However, once all the delivery applications are setup, the messages should rarely go into repair.

As already described in the section Displaying the State of Messages , there are two Disposition fields in the DE.I.HEADER or DE.O.HEADER records. Either of these record could contain a disposition of repair. Associated with each of the disposition fields is an error code field. If the Disposition field is set to REPAIR, the message is in the repair queue and the associated error code field has a description of the error that occurred.

Errors occurring in mapping are quite unusual. If an error has occurred in mapping, it indicates that there is an error in the application, which produced the message.

There are two areas in which formatting errors occur. The first area is before the DE. PRODUCT record is read. Any errors occurring during this stage of formatting is reported in disposition with the associated error message in the Error C ode field. Then the message is placed in the repair queue.

The message is corrected by first investigating the cause of the error, for example, a missing DE. PRODUCT record. Once the cause of the error has been corrected, for example, by adding the DE. PRODUCT record to the DE. PRODUCT application, the message can be resubmitted.

To correct the message, amend the Disposition field to RESUBMIT in the DE.I.HEADER and DE.O.HEADER records and authorise the record. The Disposition field is changed to RESUBMIT, the error message is removed from the repair queue and added to the unformatted queue, for a further attempt of formatting.

The other type of error, which can occur during formatting, is after the DE. PRODUCT record has been read. Once the DE. PRODUCT record is read, the multi-value message set at the end of the DE.I.HEADER and DE.O.HEADER records is expanded with details of all the copies of the messages to be produced. For example, two copies of a message may be required, one to be sent by telex and one to be printed. Therefore, the multi-value set has the details of the two copies of the message. Once the multi-value set has been added to the DE.I.HEADER and DE.O.HEADER records, the Disposition field is set to FORMATTED and the user should refer the Msg Disposition field and the associated Msg Error Code field to determine the status of the message. From this point onwards of the delivery, the copies of the message are treated separately. When a copy of the message appears in a queue, the delivery ID has the copy number added to the ID, so the user can determine which message copy is being processed.

Here, the system has picked up that an advice is to be sent by SWIFT and PRINT, and that the SWIFT address is not held.

Most errors which occur during formatting, is normally because of missing DE. ADDRESS record. The error is corrected by adding the DE. ADDRESS record to DE.ADDRESS application. The DE.O.HEADER record is amended by changing the Msg Disposition field to RESUBMIT and the record is authorised. The Msg Disposition field is changed to RESUBMITTED and a new multi-value set is added to the end of the record with the same details as the message being resubmitted. The Msg Disposition field in the new multi-value set is set to RESUBMIT. Thus the history of the message is available, with the fact that the first time an attempt was made to format the message an error occurred, the error message still being set on the original copy of the message. When the message is resubmitted, the message is added to the unformatted queue for another attempt at formatting and removed from the repair queue. The message sequence number of the new message is included in the ID of the record in the unformatted queue.

In the above scenario, if copy number 1 was resubmitted, then the message DYYYYMMDDNNNNNSSSSSQQ.3 would be added to the unformatted queue.


##### Resubmitting Messages at Other Stages

Messages may be resubmitted not only from the repair queue, but also when they are successfully formatted. However, if copies are not allowed ( Copies field in the DE.MESSAGE record is set to NO) for the message type being processed and the Msg Disposition field is set to ACK (acknowledged, which means that the message has been successfully sent) or WACK (awaiting acknowledgement, which means that the message has been sent but the acknowledgement that it has been received successfully by the recipient has not been received yet), the message cannot be resubmitted.

If a message in the Msg Disposition field, that is set to ACK or WACK, is resubmitted, its Msg Disposition field becomes ACK - RESUBMITTED or WACK - RESUBMITTED and a new copy is generated (as described above). Once the DE. PRODUCT record has been read successfully (that is, the multi-value set has been expanded), the subsequent attempts of formatting will not read the DE. PRODUCT record again.

Messages in the test key queue and the batching queue may also have their D isposition field changed to RESUBMIT. Also, the Msg Disposition field is changed to RESUBMIT, a new message copy is generated (as described above) and the new copy is placed in the unformatted queue. The completed batches of telex messages, which has a message removed from them, is re-completed and placed back on the test key queue.

The completed telex batches elsewhere in the delivery system, in which the messages removed from them are re-completed. Then the changed batch is placed back in the carrier queue in which it was originally located in or returned to the test key queue, if a test key is required for it. The individual message removed is processed in similar method as a resubmitted message.


##### Holding or Releasing the Messages

Within delivery, it is possible to hold the messages indefinitely, for a period of time or until a certain time. To hold a message means, that the message go through formatting normally, but are not placed in the appropriate carrier control queue until:

- The wait time is elapsed or
- The message hold time is elapsed or
- The message has been released.

Instead of being placed on a carrier control queue, the message is placed in the HOLD queue. The DE.DISP.TIMECHECK service continuously examines this queue to determine if there are any messages to be released. If a message is found which should be released, it is removed from the HOLD queue and added to the appropriate carrier control queue. However, if the message is to be sent by telex and batching is required, the message will be added to the batching queue. Similarly, if the message is to be sent by telex and batching is not required but a test key is required, the message is added to the test key queue.

An application may pass a message to delivery as Hold, Wait hh:mm or Hold hh:mm as already specified. If a hold requirement is passed to delivery, during mapping the hold details are used to update the Status field in the DE.I.HEADER and DE.O.HEADER records. Wait time is always added to the current time to produce a status of Hold hh:mm.

During formatting, when the DE. PRODUCT record is read, the status on the DE.I.HEADER and DE.O.HEADER records may be updated with the status details in the DE. PRODUCT record. The status details in the DE. PRODUCT does not override any status details passed from the banking application.

The status can be amended in the DE.I.HEADER and DE.O.HEADER records before the multi-value set has been expanded, that is, when the message is unformatted or in repair before the DE. PRODUCT record is read. The status can be changed to Hold, Hold hh:mm, Wait hh:mm or Release (Release can only be entered if the status is currently Hold or Hold hh:mm). When the record is authorised, the Release removes a status of Hold or Hold hh:mm, Wait hh:mm is translated to Hold hh:mm.

Before formatting, the Status field is not used and the record is processed during formatting as normal. However, when the multi-value set at the end of the DE.I.HEADER and DE.O.HEADER records are added, the value of Status field is used to update each value of the Msg Status fields. Once each copy of the message is formatted, the copies are added to the HOLD queue (if appropriate).

If a message has been formatted but has not yet been sent by a carrier (that is, the Msg Disposition field is not set to WACK or ACK), the Msg Status field can be amended in the DE.I.HEADER and DE.O.HEADER records. As for status, the Msg Status field can be changed to:

- Hold
- Hold hh:mm
- Wait hh:mm
- Release

Once the record is authorised and if the message is to be held, the message is removed from the current queue and added to the HOLD queue. If the message is to be released, it is removed from the HOLD queue and added to the carrier control queue, test key queue or batching queue as appropriate. In addition, the messages can be held by specifying the particular requirements on the DE.DISP.CONTROL application. This application is read during formatting to check, if any of the conditions match.


##### Re-routing Messages

There may be circumstances when messages should be sent either to a different address from usual or through a different carrier. For example, if a customer's telex is out of order, the customer may want all their telex messages to be sent to a different number. Alternatively, if the bank's connection to SWIFT is not working, the customer may want to send everything out by print.

If a message is to be rerouted, the DE.ALTERNATE application is accessed for the carrier, address number, language and format. Then it copies the message which should be sent. There are different ways thorough which the messages may be rerouted. The customer can decide which method best suits the current situation.

The simplest method of re-routing messages is to update the header records ( DE. I .HEADER and DE.O.HEADER ). This method can be used:

- When the delivery ID of the message is known and only a few messages are to be re-routed or
- When a message has gone into repair because of an error in the carrier or the carrier address.

The Msg Disposition field in the DE.I.HEADER or DE.O.HEADER records should be updated to REROUTE and must be authorised. Then the Msg Disposition field is updated to REROUTE, the message is removed from the current queue, the multi-value set is expanded according to the details in the DE.ALTERNATE application and the new message (or messages) is added to the unformatted queue.

> **⚠️ Note:** More than one copy of message may be generated from one message being rerouted. For example, a SWIFT message being rerouted may be replaced by a telex message and a print message.

Messages can be rerouted by specifying particular conditions, which must be updated in the DE.DISP.CONTROL . This application is read during formatting to check, if any of the conditions match.


#### 📋 Tasks

There are no Tasks available for Static Processing of Messages feature.


#### 📊 Outputs

There are no Outputs available for Static Processing of Messages feature.


> **Related Applications:** `)`, `,`, `.HEADER`, `ADDRESS`, `BATCH`, `DE`, `DE.ADDRESS`, `DE.ALTERNATE`, `DE.CARRIER`, `DE.DISP.CONTROL`, `DE.FORMAT.PRINT, DE.FORMAT.SWIFT`, `DE.I.HEADER`, `DE.INTERFACE`, `DE.MAPPING`, `DE.MESSAGE`, `DE.O.HEADER`, `DE.PRINT`, `DE.PRODUCT`, `HOLD.CONTROL`, `I`, `PRODUCT`, `TSA.SERVICE`

---


### 2.27  Straight Through Processing


> **📇 Quick Reference Card**
> 
> **Purpose:** *Straight Through Processing (STP) is used by companies in the financial world to optimise the speed at which transactions are processed. This is performed by allowing information that has been electronically entered to be transferred from one party to another in the settlement process without manual...*
> 
> **Key Fields:** *Direction*, *Stp Status*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Straight Through Processing (STP) is used by companies in the financial world to optimise the speed at which transactions are processed. This is performed by allowing information that has been electronically entered to be transferred from one party to another in the settlement process without manually re-entering the same pieces of information repeatedly over the entire sequence of events.

The generated SWIFT messages are not supported for STP. Processing of SWIFT messages happens faster when BIC codes are used. The SWIFT messages generated mostly uses the name and addresses which need manual intervention to convert to BIC codes. This delays the settlement time and increases the transaction cost for the bank.

STP product (VS) integrates with Integration Framework (IF) for SWIFT messages. They are enhanced by an external STP processing software for better STP compliance. It reduces the time of settlement and transaction costs for the bank.


#### ⚙️ Configuration

The DE.STP.REPAIR.PARM application defines the SWIFT message types for STP processing. The Direction field defines if the messages are INWARD or OUTWARD or of BOTH directions.


#### 🔧 Working With

The workflow of an incoming SWIFT message is shown below.

The STP scans the SWIFT message for names and addresses that can be converted to BIC codes and it populate the related tags.

It can be seen that where ever names and addresses were provided, they have been converted to BIC codes. The account number given at a different location in tag 59 has also been placed correctly within the tag.

A SWIFT message before and after the processing of STP is shown in the screenshots below.

The names and address provided have been converted to BIC codes. The account number given at a different location in Tag 59 has also been placed correctly within the Tag.

The SWIFT messages are forwarded to STP through IF. Until a response is received the Stp Status field in the DE.O.HEADER and DE.I.HEADER records are updated as WAITING-STP. Once the response is received, this field is updated to FORMATTED-STP.

The workflow for an outgoing message is shown below.

> **⚠️ Note:** MDINT is the SWIFT interface. The F.DE.O.AWAK , F.DE.O.MSG.MDINT and F.DE.O.HISTORY.QUEUE are system maintained internal files used in processing.


#### 📋 Tasks

There are no Tasks available for Straight Through Processing feature.


#### 📊 Outputs

There are no Outputs available for Straight Through Processing feature.

---


### 2.28  SWIFT2024 Rulebook Changes


> **📇 Quick Reference Card**
> 
> **Purpose:** *As part of the CBPR+ SR2024 Release, camt.109 has undergone the following changes given in the table below.*
> 
> **Applications:** `SWIFT.PARAMETER`
> 
> **Key Fields:** *Curr Swift Rel*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

As part of the CBPR+ SR2024 Release, camt.109 has undergone the following changes given in the table below.

| Tags | Path in SWIFT Portal | Description |
|---|---|---|
| Business Service Tag | /AppHdr/BizSvc | Populated as swift.cbprplus.02 |
| Payee Address Line | /Pyee/PstlAdr/AdrLine | Limited to three lines with a maximum of 35 characters per line |
| Stop Request Status Code | /ChqCxlOrStopSts/Sts/Cd | Changed to RJCR and ACCR for ‘Rejected’ and ‘Accepted’ respectively |
| Province Of Birth | /ChqCxlOrStopRpt/Chq/Pyee/Id/PrvtId/DtAndPlcOfBirth/PrvcOfBirth | Updated character type as ISOEXTENDED for payee |
| City Of Birth | /ChqCxlOrStopRpt/Chq/Pyee/Id/PrvtId/DtAndPlcOfBirth/CityOfBirth | Updated character type as ISOEXTENDED for payee |


#### ⚙️ Configuration

This section explains the configurations required to enable SWIFT 2024 rule book changes.

To enable SWIFT 2024 rule book changes, the Curr Swift Rel field in the SWIFT.PARAMETER application for CBPRPLUS record is set to 2024.

Update CBPRPLUS


#### 📋 Tasks

There are no Tasks available for the SWIFT 2024 Rulebook Changes feature.


#### 📊 Outputs

There are no Outputs available for the SWIFT 2024 Rulebook Changes feature.


> **Related Applications:** `SWIFT.PARAMETER`

---


### 2.29  SWIFT 2017 Rulebook Changes


> **📇 Quick Reference Card**
> 
> **Purpose:** *The SWIFT 2017 Rulebook enables the following features:*
> 
> **Applications:** `DE.I.HEADER`, `DE.MESSAGE`, `FUNDS.TRANSFER`, `SWIFT.PARAMETER`, `SWIFT.PARMETER`
> 
> **Key Fields:** *Ben Address*, *Ben Country*, *Ben Customer*, *Ben Name*, *Ben Town*, *Bk To Bk Out*, *Curr Swift Rel*, *In Bk To Bk* ... +6 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The SWIFT 2017 Rulebook enables the following features:

- The incoming MT103 or MT103REMIT, with the CODE words INS or ACC in Sender to Receiver Information in Tag 72, is updated automatically in Tag 72 of the outgoing message in the payment chin, without being modified. However, additional Sender to Receiver Information is given using the Bk To Bk Out and Send To Party fields in the outgoing message.
- The incoming MT103STP, with the CODE word INS in Sender to Receiver Information is updated automatically in Tag 72 of the outgoing message in the payment chain, without being modified. However, additional Sender to Receiver information is given using the Bk To Bk Out and Send To Party fields in the outgoing message.
- The incoming messages such as MT202, MT202COV, MT203, MT205 and MT205COV that have Sender to Receiver Information in Tag 72, with CODE words INS, ACC or BNF, are updated automatically in Tag 72 of the outgoing message in the payment chain, without being modified. However, additional Sender to Receiver Information is given using the Bk To Bk Out and Send To Party fields in the outgoing message.
- In the MT110 ‘Advice of Cheques’ message, Tag 59 is replaced with Tag 59a. This supports the ‘No Letter Option’ and Option F.
- The Invalid Msg Type multi-value field in SWIFT.PARAMETER is used to define the message types that are invalid and not supported by SWIFT. It should be a valid message type in the DE.MESSAGE application. If the SWIFT message is the same type as defined in this field, the system writes the message in Repair stating the Invalid SWIFT Message Type .
- The incoming Tags 111 and 121 in Header block 3 are stored in the Inw Head Trail field in DE.I.HEADER . These values can be viewed by the user using appropriate screen configuration.


#### ⚙️ Configuration


##### Updating theCurr Swift Relfield in theSWIFT.PARAMETERapplication

The SWIFT 2017 Rulebook changes are effective only from the time the Curr Swift Rel field in SWIFT.PARAMETER is updated as 2017. The Prev Swift Rel field is updated automatically with the old value of the Curr Swift Rel field.


#### 🔧 Working With

This section explains the process of the SWIFT 2017 Rulebook Changes.


##### Processing of Tag 72 (Sender to Receiver Information)

This section explains the processing of the Sender to Receiver Information.

- The Sender to Receiver Information (Tag 72) with CODE words INS or ACC, in the incoming MT103 or MT103REMIT, are updated in Tag 72 of the subsequent message in the payment chain. Additional Sender to Receiver Information is provided through the Send To Party and Bk To Bk Out fields in the FUNDS.TRANSFER record that is generated to process the subsequent message. The maximum lines in the outgoing Sender to Receiver Information Tag 72 (Including incoming details of Tag 72) is 6 rows with a maximum of 35 characters in each row (6*35x), as stipulated by SWIFT.

The example below shows an MT103 message with Incoming Tag 72 with Code ACC.

> **⚠️ Note:** The outgoing MT103 message contains the Sender to Receiver Information from the incoming message In Bk To Bk ) as well as the additional information given in the Bk To Bk Out field in FUNDS.TRANSFER .

- Similarly, for the Incoming MT103STP, if the Sender to Receiver Information in Tag 72 contains the CODE word INS, it is updated in Tag 72 of the subsequent message in the payment chain. Additional Sender to Receiver Information is provided through the Send To Party and Bk To Bk Out fields in the FUNDS.TRANSFER record that is generated to process the subsequent message.
- The incoming messages such as MT202, MT202COV, MT203, MT205 and MT205COV that have the Sender to Receiver Information in Tag 72 (updated in the In Bk To Bk field) and CODE words INS, ACC or BNF, are updated automatically in Tag 72 of the outgoing message in the payment chain, without being modified. However, additional Sender to Receiver Information is provided using in the Bk To Bk Out and Send To Party fields in the outgoing message. The maximum lines in the outgoing Sender to Receiver Information Tag 72 (Including incoming details of Tag 72) is 6 rows with 35 characters in each row (6*35x), as stipulated by SWIFT regulation.

> **⚠️ Note:** Cover messages in the incoming Sender to Receiver Information are stored in the In C Bk T Bk In field in FUNDS.TRANSFER .

The example below shows an MT 202 cover message with incoming Tag 72 with CODE word ACC and no additional Sender to Receiver Information.

> **⚠️ Note:** In the above example, there is no additional Sender to Receiver Information in the Bk To Bk Out field. Hence, the outgoing message contains only the incoming value of Tag 72.


##### Payee Information in MT110

The MT110 message is an Advice of Cheques. The existing Tag 59 of this message is replaced with 59a, to identify the Beneficiary (Payee) of the cheque. This is a Mandatory Tag that supports the No Letter Option and Option F, in the following format:

| Column 1 | Column 2 | Column 3 |
|---|---|---|
| NO LETTER OPTION | [/34X] 4*35X | (Account) (Name And Address) |
| Option F | [/34x] 4*(1!n/33x) | (Account) (Number/Name and Address Details) |

In Option F, the Number, Name and Address Details must contain one of the following codes:

- The first line must start with number 1.
- Numbers must appear in numerical order.
- Number 2 must not be used without number 3.
- The first occurrence of number 3 must be followed by a valid ISO country code.

Payee Information such as Account Number and Name and Address are given in the Ben Customer fields as shown below.

Payee Information, such as, Account Number and Name and Address are given in the associated multi-value fields such as Ben Name , Ben Address , Ben Country and Ben Town as shown below.


##### Invalid Message Types

The following messages are removed from the FIN Network as there is no FIN traffic for them. Hence, they are not supported by SWIFT MT from 2017.

- MT207, MT256, MT303, MT307, MT574, MT577, MT579, MT609, MT643, MT644, MT646 and MT649.

However, the removal of the above messages from the FIN network has no impact on messages that are used on proprietary networks or any other non-FIN network or messaging service.

The system prevents the message from being sent to SWIFT. The user can define these invalid message types in the Invalid Msg Type field in SWIFT.PARMETER . If a message appears in the formatting queue with the invalid message type defined in SWIFT.PARAMETER , the system sends it to REPAIR with the ‘Message Type xxx is Invalid’ message, thereby preventing the message from being sent to SWIFT.

The above-mentioned Invalid Message Types are not supported by SWIFT but still exists in the DE.MESSAGE for use in any non-FIN network or messaging service.

SWIFT gpi participants can include the header fields such as Service Type Identifier (STI) – Tag 111 and Unique End-to-End Transaction Reference (UETR) – Tag 121, in all MT 03, MT103STP and MT103REMIT that they send including to banks that are not in the CUG (Closed User Group). This allows the service to track a payment up to the first bank outside the SWIFT gpi CUG. Banks that are not in the CUG can receive these header fields but are not allowed to send or forward messages containing the 111 or 121 fields.

Temenos Core Banking can receive and store these header tags for the specified message types. It does not allow these fields to be sent or forwarded to subsequent messages in the payment chain. These tag values are stored in the Inw Head Trail field in DE.I.HEADER , where the other header fields are stored. The user views these details using the appropriate inward Delivery Reference.


#### 📋 Tasks

There are no Tasks available for SWIFT 2017 Rule Book Changes feature.


#### 📊 Outputs

There are no Outputs available for SWIFT 2017 Rule Book Changes feature.


> **Related Applications:** `DE.I.HEADER`, `DE.MESSAGE`, `FUNDS.TRANSFER`, `SWIFT.PARAMETER`, `SWIFT.PARMETER`

---


### 2.30  SWIFT 2018 Rulebook Changes


> **📇 Quick Reference Card**
> 
> **Purpose:** *The SWIFT 2018 Rulebook enables the following features:*
> 
> **Applications:** `DE.BIC`, `DE.I.HEADER`, `DE.O.HEADER`, `EB.QUERIES.ANSWERS`, `FUNDS.TRANSFER`, `SWIFT.CODE.WORDS`, `SWIFT.PARAMETER`
> 
> **Key Fields:** *Cancellation Code*, *Curr Swift Rel*, *Hdr 3 Uetr*, *ISO Cancel Reason Code*, *In Hdr 3 Uetr*, *Inw Head Trail*, *Prev Swift Rel*, *Uetr   Reference* ... +2 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The SWIFT 2018 Rulebook enables the following features:

1. For the supported incoming messages in Category 1 and 2, the system stores the supported incoming messages from Category 1 and Category 2, tags 111 (Service Type Identifier) and 121 (Unique End-to-End Transaction Reference - UETR) received in Header block 3 in the following fields: Tag 121 is stored in a Uetr Reference field in DE.I.HEADER and in the In Hdr 3 Uetr field in FUNDS.TRANSFER . Tag 111 is updated by the system in the Inw Head Trail field in DE.I.HEADER .

1. The system generates a UETR and maps this reference in Tag 121 for the following outgoing messages: MT103 MT103+ MT103REMIT MT202 MT202COV MT205 MT205COV The outgoing messages that require a UETR reference to be generated are configured in the SWIFT.PARAMETER table, in the Uetr Msg Type field. This generated UETR reference is mapped in the outgoing SWIFT message in Tag 121 from Header block 3.

- Bank as Intermediary

- MT103 and MT202COV

1. When an inward MT202COV message processed by the system results in an onward MT202COV, the same UETR reference is used to generate the outgoing message, as the one received in the incoming message When an inward MT205COV message processed by the system results in an onward MT205COV, the same UETR reference is used to generate the outgoing message, as the one received in the incoming message.

1. For the n92 messages, the mapping is changed for tag 79 (Narrative description of the original message) to accommodate the ISO cancellation reason codes added by SWIFT for this tag. A Cancellation Code field is available in the EB.QUERIES.ANSWERS , 192 and EB.QUERIES.ANSWERS , 292 versions, where the information from this field is mapped to the ISO Cancel Reason Code field in the EB.QUERIES.ANSWERS application. For the n92 messages, ISO cancellation codes such as AGNT, CURR, CUST, CUTA, DUPL, FRAD, TECH and UPAY are added in the SWIFT.CODE.WORDS table to be used in tag 79, which is the narrative description of the original message.
2. For the n96 messages , ISO reason codes such as CNCL, PDCR, RJCR, AC04, AGNT, AM04, ARDT, ARPL, CUST, INDM, LEGL, NOAS, NOOR, PTNA and RQDA are added in the SWIFT.CODE.WORDS table, to be used in tag 76 (Answers)
3. For the BIC codes that are added or entered in the DE.BIC application, the first four characters from the BIC code are alpha-numeric.


#### ⚙️ Configuration

This section explains the configuration of the SWIFT 2018 Rulebook Changes.

- Updating the Curr Swift Rel field in SWIFT.PARAMETER .

- Storing the Uetr Reference in the Uetr Reference field in the DE.O.HEADER application.

- Updating DE.I.HEADER with the Uetr Reference field.

- Updating FUNDS.TRANSFER with the In Hdr 3 Uetr field.

- Updating SWIFT.PARAMETER with the Uetr Msg Type field.


#### 🔧 Working With

This section explains the process of the SWIFT 2018 Rulebook Changes.


##### Receive Tag 111 and 121 in Header Block 3 for the Supported Category 1 and Category 2 Incoming Messages

Temenos Transact can receive and store these header tags (tag 111 and tag 121) for the supported Category 1 and Category 2 incoming messages.

- Tag 121 is stored in: The Uetr Reference field in DE.I.HEADER The In Hdr 3 Uetr field in FUNDS.TRANSFER
- Tag 111 is updated by the system in the Inw Head Trail field in DE.I.HEADER .

Below is the list of Category 1 and Category 2 messages supported by the system, for which these tags are stored:

Category 1xx – Supports Customer Payments and Cheques.

| Column 1 | Column 2 | Column 3 |
|---|---|---|
| Message | Description |  |
| MT101 | Request For Transfer | Requests to debit a customer's account held at another institution |
| MT102 | Multiple Customer Credit Transfer | Conveys multiple instructions between financial institutions. |
| MT103 | Single Customer Credit Transfer | Instructs a funds transfer |
| MT103+ | Single Customer Credit Transfer | Instructs a funds transfer (STP) |
| MT103 REMIT | Single Customer Credit Transfer | Instructs a funds transfer (REMIT) |
| MT192 | Request for Cancellation | Requests the Receiver to consider cancellation of the message identified in the request. |
| MT195 | Queries | Responds to an MT n95 Queries message or MT n92 Request for Cancellation or other messages where no specific message type has been provided for the response. |
| MT196 | Answers | Responds to a MT n95 Queries message or MT n92 Request for Cancellation or other messages where no specific message type has been provided for the response. |
| MT199 | Free-Format | Contains information for which no other message type has been defined. |

Category 2xx – Supports Financial Institution Transfers.

| Column 1 | Column 2 | Column 3 |
|---|---|---|
| Message | Description |  |
| MT 200 | Financial Institution Transfer for its Own Account | Requests the movement of the sender’s funds to its account at another financial institution. |
| MT 202 | General Financial Institution Transfer | Requests the movement of funds between financial institutions. |
| MT202COV | General Financial Institution Transfer | Requests the movement of funds between financial institutions. |
| MT 203 | Multiple General Financial Institution Transfer | Multiple of the MT 202 |
| MT 205 | Financial Institution Transfer Execution | Further transmits a transfer request domestically. |
| MT 210 | Notice to Receive | Notifies the receiver that it will receive funds for the Sender’s account. |
| MT292 | Request for Cancellation | Requests the Receiver to consider cancellation of the message identified in the request. |
| MT295 | Queries | Responds to a MT n95 Queries message or MT n92 Request for Cancellation or other messages where no specific message type has been provided for the response. |
| MT296 | Answers | Responds to a MT n95 Queries message or MT n92 Request for Cancellation or other messages where no specific message type has been provided for the response. |
| MT299 | Free-Format | Contains information for which no other message type has been defined |

- The received Tag 121 is stored in the Uetr Reference field in DE.I.HEADER .
- The received Tag 111 is stored in the Inw Head Trail field in DE.I.HEADER .


##### Generate a UETR and Map this Reference in Tag 121 of the following Outgoing Messages

MT103, MT103+, MT103REMIT, MT202, MT202COV, MT205, MT205COV

The outgoing messages that require a UETR reference (Tag 121) to be generated are configured in the Uetr Msg Type field in the SWIFT.PARAMETER table. The generated UETR is stored in the Uetr Reference field in DE.O.HEADER .

Below is a generated Uetr Reference from DE.O.HEADER .

- MT103 and MT202COV The system generates the same Uetr reference for the transactions (like MT103 + MT202COV) that generate multiple messages. The same UETR reference is used for both MT103 and MT202COV messages. This value is mapped in Tag 121 of both the MT103 and MT202COV messages. The screenshot below shows the Uetr Reference from DE.O.HEADER for MT103. The screenshot below shows the Uetr Reference from DE.O.HEADER for MT202COV (same value).
- Bank as Intermediary The UETR received in the incoming message is passed unchanged in the outgoing message when the bank acts as an intermediary, receiving and sending a message from the chain. The value of Tag 121 from the incoming message is stored in the In Hdr 3 Uetr field in Funds Transfer and in the Uetr Reference field in DE.I.HEADER . When the outward message is generated for the same FUNDS TRANSFER, the same value from Uetr Reference is used and is mapped in the Uetr Reference field in DE.O.HEADER . This is how the value from field 121 is passed on unchanged in the outgoing message. The screenshot below shows the Uetr Reference in DE.I.HEADER for the incoming MT103 message. The created Funds Transfer contains the incoming UETR (stored in the In Hdr 3 Uetr field in FUNDS.TRANSFER ), which is used when generating the outgoing message.


##### Support Tag 121 that must be Passed Unchanged in Header block 3 for Category 2 Cover Messages

Temenos Transact can,

- Forward or Copy the content of field 121 from Header block 3 of the inward MT202COV message and pass it unchanged to field 121 from Header block 3 of the onward MT202COV.
- Forward or Copy the content of field 121 from Header block 3 of the inward MT205COV message and pass it unchanged to field 121 from Header block 3 of the onward MT202COV.

The screen shot below shows a received MT202COV, stored in the Uetr Reference (Tag 121) field stored in DE.I.HEADER .

The screenshot below shows an outgoing MT205COV, containing the same UETR, stored in the Uetr Reference field in DE.O.HEADER .


##### Adding Tag 79 for n92 Messages

Temenos Transact supports the codes (Cancellation Reason codes) that are added for field 79, for inward and outward n92 messages:

> **⚠️ Note:** Field 79 is a Narrative Description of the Original Message

FORMAT:

The following ISO Cancellation Reason codes are available for n92 messages, in the SWIFT.CODE.WORDS table:

- AGNT, CURR, CUST,CUTA, DUPL, FRAD, TECH, UPAY

These cancellation codes are stored in the ISO Cancel Reason Code field in the EB.QUERIES.ANSWERS application.


##### Adding Tag 76 for n96 Messages

Temenos Transact supports the codes (Response and Reason codes added for field 76, for inward and outward n96 messages:

The following ISO reason codes are available for n96 messages, in the SWIFT.CODE.WORDS table:

- CNCL, PDCR, RJCR, AC04, AGNT, AM04, ARDT, ARPL, CUST, INDM, LEGL, NOAS, NOOR, PTNA, RQDA


##### Business Identifier Code (BIC) fromDE.BIC

The system supports or allows the first four characters from a BIC code that is entered in DE.BIC , to be alphanumeric.


#### 📋 Tasks

There are no Tasks available for SWIFT 2018 Rulebook Changes feature.


#### 📊 Outputs

There are no Outputs available for SWIFT 2018 Rulebook Changes feature.


> **Related Applications:** `DE.BIC`, `DE.I.HEADER`, `DE.O.HEADER`, `EB.QUERIES.ANSWERS`, `FUNDS.TRANSFER`, `SWIFT.CODE.WORDS`, `SWIFT.PARAMETER`

---


### 2.31  SWIFT 2019 Rulebook Changes


> **📇 Quick Reference Card**
> 
> **Purpose:** *The SWIFT 2019 Rulebook changes enables the following features:*
> 
> **Key Fields:** *Curr Swift Rel*, *Delivery Reference*, *Fwd Uetr Message Type*, *Org.De.I.Header*, *Org.De.O.Header*, *Prev Swift Rel*, *Sender Address*, *Service Type Id* ... +6 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The SWIFT 2019 Rulebook changes enables the following features:

- For category 1, 2 and 9 outward queries, answers and cancellation messages (MT190, MT191, MT192, MT195, MT196, MT199, MT292, MT295, MT296, MT299, MT992, MT995, MT996 and MT999), forward the same UETR (Unique End to End Transaction Reference) as in the original payment message.
- For Category 1 and Category 2, the code word REC from field 72 (Sender to Receiver information) is removed.
- For n92 messages, two optional cancellation codes (AM09 and COVR) are added for Tag 79.


#### ⚙️ Configuration

Temenos Transact allows the Fwd Uetr Message Type field in the SWIFT.PARAMETER application to specify the message types that require a UETR reference to be forwarded in the outgoing message.

The Fwd Uetr Message Type field can be configured in the SWIFT.PARAMETER application only when the license for the SWIFT 2019 changes is available in the system. This is done by updating the Curr Swift Rel field as 2019 in the SWIFT.PARAMETER application. The Prev Swift Rel field is updated automatically with the old value of the Curr Swift Rel field.


#### 🔧 Working With

This section explains the process of the SWIFT 2019 Rulebook Changes.


##### Forward the UETR in the Category 1, 2 and 9 Outward Queries, Answers and Cancellation Messages

In 2018, SWIFT introduced the UETR (Unique End to End Transaction Reference), which is a Globally Unique Transaction Reference that must be mapped in field 121 of Header Block 3 of the following outgoing messages:

- MT103, MT103 STP, MT103REMIT, MT202, MT202COV, MT205 and MT205COV

The SWIFT 2019 Rulebook changes enables banks to forward the UETR received in the original payment message in the subsequent queries, answers and cancellation messages in categories 1, 2 and 9 messages.

The forwarding and mapping of field 121 in Block 3 is now applicable in Temenos Transact for the following outgoing messages:

| Message | Description |
|---|---|
| MT190 | Advice of Charges, Interest and Other Adjustments |
| MT191 | Request for Payment of Charges, Interest and Other Expenses |
| MT192 | Request for Cancellation |
| MT195 | Queries |
| MT196 | Answers |
| MT199 | Free-Format |
| MT292 | Request for Cancellation |
| MT295 | Queries |
| MT296 | Answers |
| MT299 | Free-Format |
| MT992 | Request for Cancellation |
| MT995 | Queries |
| MT996 | Answers |
| MT999 | Free-Format |

The following three applications from Temenos Transact generate the above-mentioned outgoing messages:

- The AC.CHARGE.REQUEST application generates the MT190 and MT191 messages.
- The EB.FREE.MESSAGES application generates the MT199, MT299 and MT999 messages.
- The EB.QUERIES.ANSWERS application generates the MT192, MT195, MT196, MT292, MT295, MT296, MT992, MT995 and MT996 messages.

The Transaction Ref field in the AC.CHARGE.REQUEST application captures the Temenos Transact reference of the original or related message (for example, T103, MT202, MT202COV) to which the new AC.CHARGE.REQUEST transaction (MT190 or MT191) refers.

The following screenshot is an example of an incoming MT103 message that is received by the system with the following UETR in field 121: eb6305c9-1f7f-49de-aed0-16487c27b42d.

The system assigns the BNK19107MK0GMLDK transaction reference to the MT103 message.

After the MT103 is processed, an MT191 message is sent to the correspondent bank to request for the charges from the beneficiary bank.

The outgoing MT191 message is captured in the AC.CHARGE.REQUEST application where the user captures the Transaction Reference of the original MT103 message (BNK19107MK0GMLDK) in the Txn Reference field.

Based on the captured Transaction Ref , the system retrieves the UETR from the original MT103 and forwards it in the generated outgoing MT191 message. The forwarded UETR is stored in the Uetr Reference field in DE.O.HEADER (for the MT191 generated record).

The forwarded UETR is mapped in field 121 of Header Block 3 of the outgoing MT191 message.

The EB.FREE.MESSAGE application processes the MT199, MT299 and MT999 messages.

This application contains the Transaction Ref field that captures the Temenos Transact transaction reference of the original or related message (for example, MT103, MT202 and MT202COV), to which the new transaction generated by EB.FREE.MESSAGE refers (MT199, MT299 and MT999).

The following screen shot is an example of an outgoing MT103 message that is sent by the system with the UETR mapped in field 121.

An outgoing MT199 message is sent to the correspondent bank to investigate if the funds were applied by the beneficiary bank.

The outgoing MT199 message is captured in the EB.FREE.MESSAGE application where the user captures the Transaction Reference of the original outgoing MT103 message in the Transaction Ref field.

Based on the captured Transaction Ref , the system retrieves the UETR from the original MT103 and forwards the same in the generated outgoing MT199 message. The forwarded UETR is stored in the Uetr Reference field in DE.O.HEADER (for the MT199 generated record).

The forwarded UETR is mapped in field 121 of Header Block 3 of the outgoing MT199 message.

The EB.QUERIES.ANSWERS application generates the following messages:

MT192, MT195, MT196, MT292, MT295, MT296, MT992, MT995 and MT996.

To forward the same UETR as in the original message, the Org.De.I.Header and Org.De.O.Header fields (which contain the Delivery Reference ) in the EB.QUERIES.ANSWERS application, allows the user to capture the delivery reference of the original or related message (incoming or outgoing) to which the new EB.QUERIES.ANSWERS transaction refers.

The following screen shot is an example of an outgoing MT103 message that is sent by the bank with the following UETR mapped in field 121: ed0cfb32-0137-44d7-9652-53cdc66963ad

The bank sends an MT192 outgoing message to cancel the outgoing MT103 message. The outgoing MT192 message is captured in the EB.QUERIES.ANSWERS application, where the user captures the Delivery Reference of the original outgoing MT103 message.

Based on the captured Delivery Reference , the system retrieves the UETR from the original MT103 and forwards the same in the generated outgoing MT192 cancellation message. The forwarded UETR (with the same value as ed0cfb32-0137-44d7-9652-53cdc66963ad) is stored in the Uetr Reference field in DE.O.HEADER (for the MT192 generated record).

The forwarded UETR is mapped in field 121 of Header Block 3 of the outgoing MT192 message.


##### Remove Code Word REC from Field 72 for Messages from Category 1 and Category 2

SWIFT has removed the code word REC from their User Handbooks in the Standard Release 2019, because the use of this code word almost always stops at Straight Through Processing. Instead of using this code word, the correspondent banks must either agree on a more appropriate code or cover the usage of this code in bilateral agreements.

As a result, the code word REC is removed from the SWIFT.CODE.WORDS application, thus aligning the system to the new SWIFT Standards.

The removal of the code word REC from tag 72 (Sender to Receiver Information) is applicable for the below messages:

- MT103 – Single Customer Credit Transfer
- MT103 REMIT – Single Customer Credit Transfer
- MT110 – Advice of Cheque
- MT200 – Financial Institution Transfer for its Own Account
- MT201 – Multiple Financial Institution Transfer for its Own Account
- MT202 – General Financial Institution Transfer
- MT202 COV – General Financial Institution Transfer
- MT203 – Multiple General Financial Institution Transfer
- MT204 – Financial Markets Direct Debit Message
- MT205 – Financial Institution Transfer Execution
- MT205 COV – Financial Institution Transfer Execution

When capturing and processing an outgoing MT103, the system displays an error message when the code word REC is used in field 72.


##### Changes for n92 Messages for Field 79

SWIFT has introduced two new cancellation reason codes (AM09 and COVR) that are to be used in field 79 of the n92 messages.

These two cancellation reason codes, AM09 and COVR, are available in the SWIFT.CODE.WORDS application for Message Type ’n92’.


##### Process Inward MT199 and MT299 gpi Confirmation

This functionality enables to receive MT199 and MT299 confirmation and alert messages from the gpi tracker service (identified by the BIC code TRCKCHZZ orTRCKCHZZVA), confirming that a payment was credited on the beneficiary’s account, or in case of alerts notifying a validation failure.

The functionality for processing inward MT199 and MT299 gpi confirmations is a functionality specific to gpi participant banks.

In Temenos Transact , the EB.FREE.MESSAGE application is responsible for storing the details of the received MT199 and MT299 SWIFT messages.

When an incoming MT199 and MT299 is received by the bank and is updated in EB.FREE.MESSAGE , the application checks if the gpi license or module is available in the system.

If the gpi license or module is available, the system checks if the message is received by the gpi service, which confirms if the Service Type Identifier (field 111) is present in the header of the received MT199 and MT299 messages.

The EB.FREE.MESSAGE application is improved to store all the information received in an MT199 and MT299 from the gpi tracker. The following three fields are added in the EB.FREE.MESSAGE application:

- Sender Address – This field stores the Sender BIC code which is received in the incoming message.
- UETR Reference – This field contains the Unique End to End Transaction Reference (UETR)
- Service Type Id – This field holds the Service Type Identifier (Tag 111 from Block 3). The value 001 in this field indicates the gpi service.

The following screenshot is an example of an MT199 message received that contains the Unique End to End Transaction Number and the Service Type Identifier as 001, indicating that the message was sent under the SWIFT gpi service.

The following screenshot is an example of an MT299 message received that contains the Unique End to End Transaction Number and the Service Type Identifier as 001, indicating that the message was sent under the SWIFT gpi service.

After the message is received by the system, it is stored by the EB.FREE.MESSAGE application and validations are done. The details of the received MT199 and MT299 are passed to TPH (Temenos Payment Hub), which is responsible for updating the payment status, based on the status code received in the MT199 and MT299. All the details that are stored in the EB.FREE.MESSAGE application are passed to TPH.

If the MT199 and MT299 are not received from the gpi tracker (and instead is received from a correspondent bank), in this case, no details of the MT199 and MT299 messages are passed from the EB.FREE.MESSAGE application to TPH (Temenos Payment Hub).

The gpi functionality for generating (MT199 and MT299) messages and sending them to the gpi tracker to report the status of the payment (credited on the beneficiary account or rejected), represents a functionality in TPH (Temenos Payment Hub) and does not involve the usage of the EB.FREE.MESSAGE application.


##### Enquiries and Reports

Find UETR References

The Find UETR References enquiry is available as a context enquiry for the applications from Temenos Transact that capture or forward the UETR in the Category 1, 2 and 9 queries, answers and cancellation messages : AC.CHARGE.REQUEST , EB.FREE.MESSAGE and EB.QUERIES.ANSWERS .

This enquiry allows the user to view the messages that contain a UETR (Unique End to End Transaction Reference). If multiple messages share the same UETR, then all the messages with that UETR are displayed.

The following information related to the UETR is displayed in the enquiry, based on the search that is performed using the Transaction Reference :

- UETR
- Temenos Transact Transaction Reference
- Message Type
- Delivery Reference

The example below shows Find UETR References as the context enquiry of the EB.QUERIES.ANSWERS application:

The user can search for a transaction that contains a UETR using the Transaction Reference.

In this example, the displayed result of the enquiry contains the MT103 and MT192 messages that have the same UETR, because the UETR of the original MT103 is sent in the MT192 message.


#### 📋 Tasks

There are no Tasks available for SWIFT 2019 Rulebook Changes feature.


#### 📊 Outputs

There are no Outputs available for SWIFT 2019 Rulebook Changes feature.

---


### 2.32  SWIFT 2020 Rulebook Changes


> **📇 Quick Reference Card**
> 
> **Purpose:** *As part of the Standards MT Release 2020, universal confirmation is mandatory for all the FIN users and is no longer confined to GPI member banks.*
> 
> **Applications:** `COMPANY`, `DE.I.HEADER`, `DE.O.HEADER`, `DE.PARM`, `FT.APPL.DEFAULT`, `FUNDS.TRANSFER`, `SFCONF.CONFIRMATION.TRACKER`, `SFCONF.TRACKER.STATUS.REASON` ... +1 more
> 
> **Key Fields:** *Amount Credited*, *Application*, *Confirmed Amount*, *Confirmed Amt*, *Confirmed Ccy*, *Confirmed Currency*, *Credit Amount*, *Credit Currency* ... +16 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

As part of the Standards MT Release 2020, universal confirmation is mandatory for all the FIN users and is no longer confined to GPI member banks.

Universal confirmations are basically payment confirmations which provide certainty that a particular payment from the ordering customer has been duly received by the beneficiary customer. Each financial institution that receives MT103, MT103 STP and MT103 REMIT will confirm the processing status of the payment to the SWIFT (Society for Worldwide Interbank Financial Telecommunication) tracker (BIC code: TRCKCHZZ), within two business days following the payment value date.

Universal confirmations are categorised follows:

It is mandatory to send a confirmation to the SWIFT tracker in the following situations:

- When an incoming MT103 payment is credited to the account of the beneficiary customer.
- When an incoming MT103 payment is rejected.

It is recommended (optional) to send a confirmation to the SWIFT tracker in the following situations:

- When the settlement is in progress for a transferred payment (when payment has been transferred outside of the FIN service). In this case, the Settlement in Progress status code must be used to indicate that the transaction still requires further processing before it can be considered completed. The bank need not send further updates.
- When the settlement is in progress for a pending payment and the receiver is unable to send a final confirmation within two business days. In this case, the Settlement in Progress status code must be used.


#### ⚙️ Configuration

The incoming MT103 payments for universal confirmations are processed through the Funds Transfer (FT) module. To enable SWIFT 2020 for universal confirmations, set the Curr Swift Rel field in the SWIFT.PARAMETER application to 2020.

The Swift Tracker Bic code (TRCKCHZZ) is stored in the DE.PARM application, which is used for universal confirmation. Each financial institution that receives an MT103, MT103 STP or MT103 REMIT message must confirm the processing status of the payment to the SWIFT tracker within two business days following the payment value date.

The SFCONF.TRACKER.STATUS.REASON application stores the universal confirmation status codes along with the status reasons. The Status Code in this application is defined in the FUNDS.TRANSFER application and from FT, it is mapped to the Status Code field in the SFCONF.CONFIRMATION.TRACKER application.

The record ID for SFCONF.TRACKER.STATUS.REASON is status code or status code/status reason (for example, ACCC or ACSP/G002). The ACCC record in SFCONF.TRACKER.STATUS.REASON is shown in the below screenshot.

The following combination of status code and status reason is used for universal confirmation:

| ID | Description | Tracker Status | Status Code | Status Reason | Confirmed Amount and Currency |
|---|---|---|---|---|---|
| ACCC | Accepted; settlement confirmed | Settled | ACCC |  | Yes |
| ACSP/G001 | Payment transferred | Transferred | ACSP | G001 | Yes |
| ACSP/G002 | Credit might not be confirmed in the required two days | Pending | ACSP | G002 |  |
| ACSP/G003 | Credit not confirmed due to pending required documents | Pending | ACSP | G003 |  |
| ACSP/G004 | Pending funds | Pending | ACSP | G004 |  |
| RJCT/AC01 | Incorrect account number | Rejected | RJCT | AC01 |  |
| RJCT/AC04 | Closed account number | Rejected | RJCT | AC04 |  |
| RJCT/AC06 | Blocked account | Rejected | RJCT | AC06 |  |
| RJCT/BE01 | Inconsistent with end customer | Rejected | RJCT | BE01 |  |
| RJCT/NOAS | No answer from customer | Rejected | RJCT | NOAS |  |
| RJCT/RR03 | Missing creditor name or address | Rejected | RJCT | RR03 |  |
| RJCT/FF07 | Invalid purpose | Rejected | RJCT | FF07 |  |
| RJCT/RC01 | Bank identifier incorrect | Rejected | RJCT | RC01 |  |
| RJCT/RC08 | Invalid clearing system member identifier | Rejected | RJCT | RC08 |  |
| RJCT/FOCR | Following cancellation request | Rejected | RJCT | FOCR |  |
| RJCT/DUPL | Duplication | Rejected | RJCT | DUPL |  |
| RJCT/RR05 | Regulatory information invalid | Rejected | RJCT | RR05 |  |
| RJCT/AM06 | Amount too low | Rejected | RJCT | AM06 |  |
| RJCT/CUST | Requested by customer | Rejected | RJCT | CUST |  |
| RJCT/MS03 | Not specified reason agent generated | Rejected | RJCT | MS03 |  |

In case of offline confirmations, the Off Pend Track Status field in the FT.APPL.DEFAULT application stores the offline pending tracker status code.


#### 🔧 Working With

The required setups are done in SWIFT.PARAMETER and DE.PARM and the reason code records are created in SFCONF.TRACKER.STATUS.REASON .

An incoming MT103 message is received and the DE.I.HEADER application is generated in unformatted status. After the BNK/SWIFT.IN service is run, DE.I.HEADER is formatted and the records in FUNDS.TRANSFER and SFCONF.CONFIRMATION.TRACKER are generated for the same.

The SFCONF.CONFIRMATION.TRACKER application stores the main details of all the incoming SWIFT MT103 messages received through delivery.

The confirmation tracker is updated only when the Payment System field in DE.PARM is left blank. Also, a record is generated in SFCONF.CONFIRMATION.TRACKER only if this field is left blank.

The Status Reason Code and the In Hdr 3 Uetr fields are updated in FUNDS.TRANSFER . The In Hdr 3 Uetr reference generated in FT is the record ID for SFCONF.CONFIRMATION.TRACKER .

The following fields in SFCONF.CONFIRMATION.TRACKER are mapped from FUNDS.TRANSFER .

| Fields | Mapping |
|---|---|
| Status | Tracker status corresponding to the tracker status reason captured in FT, based on the parameterisation in SFCONF.TRACKER.STATUS.REASON |
| Status Code | Status code corresponding to the tracker status reason captured in FT, based on the parameterisation in SFCONF.TRACKER.STATUS.REASON |
| Reason Code | Reason code corresponding to the tracker status reason captured in FT, based on the parameterisation in SFCONF.TRACKER.STATUS.REASON |
| Confirmed Amount | Amount Credited from FUNDS.TRANSFER , if the Confirmed Amount and Currency fields are set to Yes in SFCONF.TRACKER.STATUS.REASON for the tracker status reason captured in FT |
| Confirmed Currency | Credit Currency from FUNDS.TRANSFER , if the Confirmed Amount and Currency fields are set to Yes in SFCONF.TRACKER.STATUS.REASON for the tracker status reason captured in FT |
| Status Transaction ID | The FT ID |

> **⚠️ Note:** For offline confirmations, the Status Transaction ID is CF plus FT ID.

The record in FUNDS.TRANSFER is created in INAU status. The user creates another FT and authorises it with fields as defined in the previous unauthorised FT and also mentions the Status Reason Code . The value in the In Hdr 3 Uetr field in FUNDS.TRANSFER is also copied from the original transaction to the new FT transaction.

The following screenshots show the records in DE.I.HEADER , FUNDS.TRANSFER and SFCONF.CONFIRMATION.TRACKER applications created through an incoming MT103.

When a record in FT is generated in INAU status, the following two scenarios are possible:

1. The corresponding SFCONF.CONFIRMATION.TRACKER for the unauthorised FT is generated with Status as blank. The user authorises the FT and does not update the Status Reason Code field. After the user runs the BNK/OFS.MESSAGE.SERVICE, the SFCONF.CONFIRMATION.TRACKER for this FT is directly updated with Status as Settled.
2. The corresponding SFCONF.CONFIRMATION.TRACKER for the unauthorised FT is generated with Status as blank. The user creates a second FT with the same values as defined in the unauthorised FT. The user updates the Status Reason Code field in the new FT and authorises the record. After the user runs the BNK/OFS.MESSAGE.SERVICE, SFCONF.CONFIRMATION.TRACKER is updated with Status as Settled or Rejected (depending upon the Status Reason Code defined in the new FT). The other fields like Status Code are updated as defined in the FT’s Status Reason Code field. The Orig Amt and Orig Ccy fields in SFCONF.CONFIRMATION.TRACKER are mapped from the Amount Credited and Credit Currency fields in FT.

The following screenshot shows a record in SFCONF.CONFIRMATION.TRACKER with the updated Status .

The BNK/OFS.MESSAGE.SERVICE also creates the DE.O.HEADER for the outgoing MT199 message with Status as Unformatted, Transaction Ref as the FT ID and Message Type as 199 and Application as SFCONF.

The user runs the BNK/SWIFT.OUT service to format the MT199 message. The following tags are updated in the MT199 message:

| MT199 Tag | Mapping | Description |
|---|---|---|
| Sender | The SWIFT address of the bank |  |
| Receiver | The BIC of the SWIFT tracker from DE.PARM |  |
| Tag 121 | The ID of the confirmation tracker | The UETR of the following MT103 |
| Tag 20 | Status Transaction ID | The ID of the FT which as updated the confirmation tracker status |
| Tag 21 | Inward Message Reference | The original tag 20 of the incoming MT103 |
| Tag 79 Line 1 | //yymmHHMM ± the offset of the local time server against UTC | The current date and time of the system when the confirmation tracker is updated |
| Tag 79 Line 2 | // / |  |
| Tag 79 Line 3 | //The SWIFT address of the bank |  |
| Tag 79 Line 4 | If Confirmed Ccy is blank, use Orig Ccy If Confirmed Amt is blank, use Orig Amt // |  |

> **⚠️ Note:** The offset time in the MT199 message will be displayed only when a value is set in Timezone in the record in the COMPANY application.

The following screenshot shows a record in DE.O.HEADER for MT199 and the related SWIFT MT199 message.

The screenshot below shows the MT199 message for View Delivery Messages (DE.MSG.SUM) enquiry.

> **⚠️ Note:** The above screenshots are pertaining to universal confirmation with the Settled status. The same can be done for the Rejected status.

The status in the confirmation tracker is updated as follows:

- If the FT transaction type is IT, inward message type is MT103 and the credit account is the account or alternate account identified in tag 59, then the status code is updated as Settled. The confirmed amount and confirmed currency will be updated with the Credit Amount and Credit Currency .
- If the FT transaction type is OT, the status is updated as Routed (the incoming MT103 message is routed to the next agent), irrespective of the Status Reason Code captured in FT.
- Apart from Pending and blank, all other confirmation tracker statuses are final, and no further updates are accepted for the confirmation tracker record.

In case, the status is Pending, the user creates a third FT and updates the Status Reason Code (Rejected or Settled). This will move the SFCONF.CONFIRMATION.TRACKER from Pending to Settled or Rejected.

The Pending status is also updated in case of offline confirmations. The Off Pend Track Status field in FT.APPL.DEFAULT stores the offline pending tracker status code. The offline pending tracker status is parametrised with ACSC/G002 so that these confirmation messages indicate to the SWIFT tracker that the credit to the beneficiary might not be confirmed in the required two business days.

In case of offline confirmations, the Status field in SFCONF.CONFIRMATION.TRACKER is blank for two business days. The user runs BNK/SFCONF.OFFLINE.CONFIRMATION (an independent service), which moves the Confirmation tracker status to Pending.

The user can change the status from Pending to Settled or Rejected through the following methods:

- Run the BNK/OFS.MESSAGE.SERVICE and authorise the same FT. The Status moves to Settled.
- Run the BNK/OFS.MESSAGE.SERVICE, create another FT and update the Status Reason Code field in the new FT. The SFCONF.CONFIRMATION.TRACKER is updated with a new Status – Settled or Rejected. Once the Status and Status Reason Code fields are updated in the confirmation tracker, the MT199 message and a record in DE.O.HEADER are generated as described above. Any confirmation tracker record with a Status other than blank or Pending is moved to history.


#### 📋 Tasks

The SWIFT 2020 Rulebook changes enables the following features:

- Solution for Universal confirmation for MT103, MT103 STP and MT103 REMIT for Funds Transfer.
- New Validation of the optional format option F in field 50 and 59 for all the Group 1, Group 2 and Group 9 messages.


##### Workflow

In this feature, the user can perform the below activities:

| SCREENS | WORKFLOW |
|---|---|
|  | Tracker Status Reason . |
| Confirmation Tracker Records | Click the Edit Details icon of a corresponding record. The individual record is opened in edit mode. |
| Tracker Status Reason | Enter values in the fields that require amendment. Click the Validate icon to check for errors and overrides. Click the Commit icon. |


#### 📊 Outputs

The SWIFT 2020 Rulebook changes enables the following features:

- Solution for Universal confirmation for MT103, MT103 STP and MT103 REMIT for Funds Transfer.
- New Validation of the optional format option F in field 50 and 59 for all the Group 1, Group 2 and Group 9 messages.


##### Enquiry and Reports

This section allows the user to view the below enquiries and reports,

Miscellaneous Payment Message

This enquiry displays all the live records in the Confirmation Tracker application. User have options to drilldown and view the following records:

- View Incoming Payment - This displays the inward delivery message
- View Incoming Payment Transaction – This displays the FT linked to the inward delivery message
- View Outward Confirmation Messages – This displays the list of the outward SWIFT confirmation messages sent for the respective Confirmation Tracker record for the current status as well as for previous status(es).
- View Linked Transactions – This displays the Funds Transfers indicated in the Status Transaction ID for the current status as well as for previous statuses.
- Update Confirmation Status – This updates the status, status code and reason code.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA


> **Related Applications:** `COMPANY`, `DE.I.HEADER`, `DE.O.HEADER`, `DE.PARM`, `FT.APPL.DEFAULT`, `FUNDS.TRANSFER`, `SFCONF.CONFIRMATION.TRACKER`, `SFCONF.TRACKER.STATUS.REASON`, `SWIFT.PARAMETER`

---


### 2.33  SWIFT 2021 Rulebook Changes


> **📇 Quick Reference Card**
> 
> **Purpose:** *The format of Ordering Customer and Beneficiary Customer is structured in the SWIFT 2021 rule book changes.*
> 
> **Key Fields:** *Ben Address*, *Ben Country*, *Ben Country Ben Town*, *Ben Name*, *Ben Name 1*, *Ben Name 2*, *Ben Name 3*, *Curr Swift Rel* ... +4 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The format of Ordering Customer and Beneficiary Customer is structured in the SWIFT 2021 rule book changes.

The Ordering Customer (tag50F) and Beneficiary Customer (tag59F) tags have the following structure:

[/34x] (Account)

4*(1!n/33x) (Number/Name and Address)

The four lines denoting the number and name and address of the Ordering or Beneficiary Customer have the following implication:

| Column 1 | Column 2 | Column 3 |
|---|---|---|
| 1 | Name of beneficiary customer | The number followed by a slash, '/', must be followed by the name of the Beneficiary Customer. |
| 2 | Address line | The number followed by a slash, '/', must be followed by an address line (address line can be used to provide, for example, street name and number, building name or post office box number). |
| 3 | Country and town | The first occurrence of number 3 must be followed by a slash, '/', the ISO country code and, optionally, additional details that are preceded by a slash, '/'. Other occurrences of number 3 must be followed by a slash, '/', and the continuation of additional details. Additional details can contain the town, which can be complemented by the postal code (for example, zip code) and country subdivision (for example, state, province or county). The country code and town should preferably indicate the country and town of residence, as provided by the Ordering Customer. |

The SWIFT 2021 Rulebook changes allows the following format changes in tag50F and tag59F for several messages in Group 1 and Group 2 MT messages and Group 9 messages:

- A line starting with number 3 must be present.
- Number lines 1, 2 and 3 may be repeated. The same number must not occur more than two times.


#### ⚙️ Configuration

To enable SWIFT 2021 rule book changes, set the Curr Swift Rel field in the SWIFT.PARAMETER application to 2021.


#### 🔧 Working With

To align with the format changes as per SWIFT 2021 Rulebook, for tag50F (Ordering Customer) and tag59F (Beneficiary Customer), Temenos Transact has allowed mapping of various application fields to these tags.


##### Tag 50F for Group 1, Group 2 and Group 9 Messages

If the Ordering Customer details are not specified in the FUNDS.TRANSFER application, the details for tag50F are populated in the SWIFT messages based on the details captured in the CUSTOMER application for the Debit Account in FUNDS.TRANSFER .

The mapping is done from the CUSTOMER record using the Name.1 and Name.2 fields for line 1/, the Street field for line 2/ and the Residence/Town field for line 3/.

The mapping also ensures that only the first 66 characters of Name.1 and Name.2 (including spaces) are considered. The maximum number of line 1/, 2/ and 3/, which can appear in the SWIFT message for tag50F, is two lines.

The formatted tag50F is applicable to SWIFT messages MT103, MT103 REMIT, MT103 STP, MT102, MT202COV and MT910.

The following screenshot shows tag50F for SWIFT MT103 updated for the customer with only 66 characters for name, address and country or town and two lines for each.


##### Tag 59F for Group 1 and Group 2 Messages

Tag59F is updated with details pertaining to the Beneficiary Customer. In tag 59F, the following lines are populated through the corresponding fields in FUNDS.TRANSFER :

- Line 1/ – The name of the beneficiary – Ben Name
- Line 2/ – Address of the beneficiary, if defined – Ben Address
- Line 3/ – Country and town – Ben Country Ben Town

Because, as per SWIFT 2021 Rulebook, line 3/, which represents the ISO country followed by the town information, must be present, the Ben Country field in FUNDS.TRANSFER is mandatory when Ben Name is given. The formatted tag59F is applicable for SWIFT messages MT103, MT103 REMIT, MT103 STP, MT101, MT110, MT102 and MT202COV.

The mapping for 1/ corresponding to the beneficiary name includes only the first 66 characters of Ben Name 1 , Ben Name 2 and Ben Name 3 . The maximum number of line 1/ that can appear in the SWIFT message for tag59F is 2. Similarly, the mapping for the Ben Address field for line 2/ is limited to two lines.

The DE.MT101.REQUEST application, which generates the MT101 messages and supports tag59F also complies with the SWIFT 2021 Rulebook. The Ben Country field in DE.MT101.REQUEST is mandatory when Ben Name is given and the mapping for 1/ corresponding to the Beneficiary Name includes only the first 66 characters of Ben Name 1 , Ben Name 2 and Ben Name 3 .

The following screenshot shows only two lines for the beneficiary names, whereas three lines are mentioned in the application for a SWIFT MT103 message:


#### 📋 Tasks

There are no Tasks available for SWIFT 2021 Rulebook Changes feature.


#### 📊 Outputs

There are no Outputs available for SWIFT 2021 Rulebook Changes feature.

---


### 2.34  SWIFT MT Stop Delivery Service


> **📇 Quick Reference Card**
> 
> **Purpose:** *This feature provides the ability to stop the SWIFT messages processing (both inward and outward) when the company is offline. This can be done company wise, company group wise or as a whole.*
> 
> **Key Fields:** *Msg Status*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

This feature provides the ability to stop the SWIFT messages processing (both inward and outward) when the company is offline. This can be done company wise, company group wise or as a whole.


#### ⚙️ Configuration

The stop delivery service is configured in the DE.CARRIER application, where either company ID or company group ID or ALL (SWIFT processing is held for all the companies that are offline) is specified.

The inward message with SWIFT carrier for all companies where the offline processing is restricted is shown in the below screenshot. For US0010001 company and for company group 1, the outward SWIFT processing during the offline stage is restricted.


#### 🔧 Working With

Whenever the SWIFT delivery message is generated and if the configuration restricts the generated messages in DE.CARRIER for SWIFT, then the messages are put on HOLD only when the company is offline.

During the start of day (when the date is cycled) the held messages are automatically released in the batch DE.HOLD.KEY.RELEASE .

Messages are processed even when the company is offline and configured as HOLD in DE.CARRIER by setting the Msg Status field in the corresponding DE.O.HEADER to RELEASE to manually release the message from HOLD.

The references of the held messages are stored in the tables DE.O.HOLD.KEY for outward messages and DE.I.HOLD.KEY for inward messages.

Once the messages are released, it is deleted from the DE.I.HOLD.KEY or DE.O.HOLD.KEY and written to the corresponding .OUT.LIST for outward messages and .IN.LIST for inward messages.

> **⚠️ Note:** The ACK and NAK messages are not put on HOLD. This functionality is supported for carriers like ISOMX. However, it supports only the outward and not the inward ISOMX.


##### Enquiry and Reports

These enquiries list the outward messages which are kept on hold when the respective companies are offline.

This enquiry will list the outward messages which are kept on hold when the respective companies are offline.

This enquiry lists the inward messages, which are kept on hold when the respective companies are offline.


#### 📋 Tasks

There are no Tasks available for SWIFT MT Stop Delivery Service feature.


#### 📊 Outputs

There are no Outputs available for SWIFT MT Stop Delivery Service feature.

---


### 2.35  Swift Security Program-Local Authentication


> **📇 Quick Reference Card**
> 
> **Purpose:** *The SWIFT Security Program ensures the security of the data flows that are exchanged between Temenos Core System and the connected SWIFT infrastructure component (for example, SWIFT Alliance Access).*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The SWIFT Security Program ensures the security of the data flows that are exchanged between Temenos Core System and the connected SWIFT infrastructure component (for example, SWIFT Alliance Access).

The Local Authentication (LAU) principle ensures the integrity and authentication of the files that are exchanged between the Temenos Core System and SWIFT infrastructure.

It secures the inward and outward messages exchanged between the Temenos Core System and SWIFT, using bilateral security keys, which are kept securely in a keystore, outside the Temenos Core System.

Local Authentication:

The principle behind LAU is that the sending and receiving systems (SWIFT Alliance Access and Temenos Core System) use the same bilateral keys to calculate the Hash-Based Message Authentication Code (HMAC).

> **⚠️ Note:** The HMAC is a digital signature, which is calculated, based on an algorithm (HMAC-SHA-256) and is appended to the SWIFT FIN message, in the S: block as MDG tag.

The entity that produces a message calculates the HMAC and includes it within the message. The receiving entity recalculates the HMAC based on the received message and verifies it against the HMAC included in the message.

Successful verification indicates that both entities (Temenos Core System and SWFT infrastructure) recognize each other and that the message is not tampered with.

LAU functionality implemented by Temenos Core System covers the calculation of the digital signature for FIN Messages in the RJE format. This functionality includes the following:

- Securely holds the bilateral left and right LAU keys in a keystore.
- Outgoing messages – Generate a digital signature, which is added in the outgoing message.
- Incoming messages – Receive and decrypt the digital signature added by SWIFT in the incoming message.


#### ⚙️ Configuration

This section explains the configuration of the SWIFT Security Program.


##### Capturing and Securely Storing Bilateral Security Keys in a Keystore

A keystore is used to securely store bilateral security keys (Left and Right keys), that are used for the calculation of the digital signature (HMAC).

The Temenos Core System and SWIFT application share the Left and Right Keys, which are used for the calculation of the digital signature (HMAC) that is added or appended to the SWIFT message.

To comply with security protocols, the bilateral security keys are stored in this keystore and not in the Temenos Core System.

The keystore interface to capture the bilateral security keys and their related details is displayed below:

Users can capture the following information in the Keystore interface:

- Keystore Name - Identifies the name of the Keystore, where the bilateral security keys are stored. The keystore allows the user to capture and store multiple and different bilateral security keys, in situations where the organization uses different keys for multiple message flows.

- One pair of keys for RTGS messages.
- One pair of keys for cross border SWIFT payments.

Using the value from this field, a corresponding record needs to be created in the Key configuration table from Temenos Transact , where the configuration details of the keys from this keystore are stored (SWIFT Security Key configuration – EB.SEC.KEY.CONFIGURATION).

- Keystore Password – Identifies the password used to secure the keystore.
- Keystore Location – Identifies the location of the keystore.
- Enter Organization Name – Identifies the name of the organization for the keystore.
- Key Type – Contains two values: Asymmetric Key – uses two different keys: one to authenticate the outgoing messages and one to authenticate the incoming messages. Symmetric Key – uses the same key to authenticate both incoming and outgoing messages.
- Enter Entry Name – Identifies the entry name. The keystore allows the user to define and store multiple bilateral keys, in situations where the organization uses different keys for multiple message flows. This field is linked to the Temenos Transact configuration table named EB.SEC.KEY.CONFIGURATION.
- Enter Entry Password – Identifies the password for the entry (Entry Name)
- Enter Left Key – Identifies the Left Key (or first part of the key). For LAU, these are the first 16 characters of the key. The two parts together form a 32- character string, which is used for the calculation of the LAU digital signature.
- Enter Right Key – Identifies the Right Key (or second part of the key). For LAU,, these are the second 16 characters of the key. The two parts together form a 32-character string, which is used for the calculation of the LAU digital signature.
- Validity Start Date – Identifies the date on which the bilateral security keys become active.
- Validity End Date – Identifies the date on which the bilateral security keys reach their end date (expire).
- Grace Days – Identifies the grace period which represents the duration (in days) in which, both the new and the previous bilateral keys are valid at reception. This can range from 0 days to 90 days.

The left and right bilateral security keys are captured and stored in the Keystore. From the Keystore, the bilateral keys are used whenever the system has to calculate the LAU digital signature (either for incoming or for outgoing SWIFT FIN messages).

The configurations for the keystore and keys are done in the Temenos Core System in the following tables ( EB.SEC.KEY.CONFIGURATION and EB.SEC.INTEGRITY.MSG.CONF) .


##### Configuring the SWIFT Security Key Table (EB.SEC.KEY.CONFIGURATION)

This table defines the security details necessary in the Temenos Core System to access the keys from the keystore. It contains the following fields:

- Keystore Name – Identifies the name of the Keystore where the security keys are stored. The keystore allows the user to define and store multiple bilateral keys, in situations where the organization uses different keys for multiple message flows. This field is linked to the Keystore (with the name), where the bilateral security keys are stored.
- Keystore Encrypted password – Identifies the encrypted password used for the keystore (defined in Keystore Name).
- Entry Name – Identifies the entry name. The keystore allows the user to define and store multiple and different bilateral keys in situations where the organization uses different keys for multiple message flows. This field is linked to the keystore, where the bilateral security keys are stored.
- Entry Generated Password – Identifies the generated password for the entry.
- Operation – Comprises of two values: Sign – Used for outward messages when the system needs to calculate the digital signature. This signature is added to the outgoing message. Verify – Used for incoming messages when the system needs to check the signature in the message received from the SWIFT infrastructure, and recalculate the digital signature to match it with the received one.
- Grace – Identifies whether the grace period is applicable for the bilateral keys. The grace period represents the duration (in days) during which both the new and the previous bilateral keys are valid at reception.


##### Configuring the SWIFT Integrity Message

The EB.SEC.INTEGRITY.MSG.CONF table configures the algorithm to be used for security validations. The configuration is not only be used for SWIFT LAU, but also for other generic types such as the validations applicable in PSD2.

The table contains the following fields:

- Algorithm – Indicates the algorithm used by the system to calculate the digital signature (LAU signature). The algorithm for SWIFT LAU is HMAC-SHA-256.
- Key Configuration – Indicates the key configurations defined in the SWIFT Security Key Configuration table ( EB.SEC.KEY.CONFIGURATION ). It represents an existing record from EB.SEC.KEY.CONFIGURATION .
- Compliance Attribute – Indicates the compliance attribute (SWIFT Config).


#### 🔧 Working With

This section explains the working of the SWIFT Security Program.


##### Calculating Local Authentication (LAU) for Outward FIN Messages

This functionality allows the generation of the LAU digital signature for the Outgoing SWIFT FIN messages securing the messages sent by the Temenos Core System to the SWIFT infrastructure.

The system allows the configuration of the LAU digital signature to be calculated and applied to the outward FIN messages, which are sent to the SWIFT infrastructure.

In the DE.CARRIER application, the user can configure the LAU calculation that needs to be applied for outward SWIFT messages (using the Outgoing LAU field), If a record from the EB.SEC.INTEGRITY.MSG.CONF table is indicated in this configuration, then the LAU calculation is applicable for outward messages. The calculation is made using the indicated Algorithm and Key Configuration from that table. If the value of the Outgoing LAU field is none (blank), then the LAU calculation is not applied for the Outward FIN messages.

The example below shows that the LAU calculation for outward messages is applicable, with the value indicating the record that corresponds from the SWIFT Integrity Message configuration table:

After the system calculates the LAU signature, it is added or appended to the message before the message is sent to the SWIFT infrastructure.

The system allows the parametrization of the signature algorithm, which is used for the LAU signature calculation in the EB.SEC.INTEGRITY.MSG.CONF table.

The signature algorithm that is used for LAU is HMAC-SHA-256 is in combination with the bilateral keys that are retrieved from the keystore when the calculation of the LAU digital signature needs to take place.

The outgoing FUNDS.TRANSFER message (as shown below), which is processed by Temenos Transact is generated with the LAU digital signature, using the calculation algorithm and the key configurations.

After the Delivery module processes the message, it is generated with the digital signature that is added by the system in the S: block for Alliance Access as MDG tag:

{S:{MDG:D1D5BC71023DFAFA69F18D1CB2B53477163E1D4CBC62942478FBC68CDCAEBD6}}


##### Calculating the LAU Signature for Inward FIN Messages

This functionality receives and decrypts the LAU digital signature added by SWIFT in the inward messages that are received from the SWIFT infrastructure.

The system decrypts the digital signature received in the incoming SWIFT message if the Incoming LAU field in DE.CARRIER indicates if a record is configured in the LAU field. If the field is none (blank), then the LAU calculation is not applied for the Inward FIN messages.

The system recalculates the value of the LAU signature (using the bilateral security keys from the keystore and the content of the received SWIFT message) based on the configuration in DE.CARRIER , and compares this signature with the one that is attached by SWIFT in the incoming SWIFT message.

The signature algorithm that is used for the LAU calculation is retrieved by the EB.SEC.INTEGRITY.MSG.CONF table for the record key that is used in the In Lau Conf field .

- If these two digital signatures match, then authentication is successful and the message is further processed on the incoming flow. All the details of the transaction are accepted and are mapped in DE.I.HEADER . The Status of the message is Ofs formatted. Example of an MT103 message (the LAU digital signature attached to it) with a successful authentication and message mapped in DE.I.HEADER (with the status Ofs formatted) is displayed below.
- If the two LAU digital signatures do not match (the one received in the incoming SWIFT messages and the one calculated by the system), then the message is placed in the Repair queue and the user can resubmit the incoming message.

This scenario is applicable if the LAU keys are wrongly captured in the keystore. The user can enter the correct key and resubmit the transaction.

The transaction is displayed below after the user resubmits the transaction.


#### 📋 Tasks

There are no Tasks available for SWIFT Security Program – Local Authentication feature.


#### 📊 Outputs

There are no Outputs available for SWIFT Security Program – Local Authentication feature.

---


### 2.36  SwiftNet Interact MX Services


> **📇 Quick Reference Card**
> 
> **Purpose:** *Various High Value Payment Systems (HVPS) referred also as Real Time Gross Settlement systems have adopted or are in progress of adopting ISO20022 messaging standards. The majority of these HVPS (SIC, CHAPS, T2, and so on) use the SWIFTNet as a network provider.*
> 
> **Applications:** `ASCII.VAL.TABLE`, `DE.ALT.CHARS`, `DE.BUSINESS.SERVICE.RULES`, `DE.CARRIER`, `DE.DISTINGUISH.NAME.RULES`, `DE.DLN.REQUIREMENTS`, `DE.FORMAT.SWIFT`, `DE.I.HEADER` ... +17 more
> 
> **Key Fields:** *Ack Required*, *AckNackTemenosFormatXsd*, *Alter Char Code*, *App Context Field*, *App Context Field.*, *App Context Value*, *Business Application*, *Business Service* ... +39 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Various High Value Payment Systems (HVPS) referred also as Real Time Gross Settlement systems have adopted or are in progress of adopting ISO20022 messaging standards. The majority of these HVPS (SIC, CHAPS, T2, and so on) use the SWIFTNet as a network provider.

Moreover SWIFT is also migrating to the ISO20022 cross border payments. The main difference is that SWIFT supports a co-existence period, allowing its members to make the full switch by the end of 2025.

Interact is a SWIFTNet messaging service that is used to send and receive financial messages in XML format. The majority of the new messaging solutions defined by the HVPS owners are using SWIFTNet Interact services. For the ISO20022 cross border payments, SWIFT also decided to use a SWIFTNet Interact based service.

A key element of the new services is the presence of the Business Application Header (BAH) as part of the exchanged message. The use of BAH, the version and the usage guidelines are decided by each payment scheme owner or administrator.

Temenos Delivery module offers Temenos Business modules a framework to exchange the ISO20022 messages with a SWIFT messaging interface, supporting the main elements of the SWIFTNet Interact message structure and providing the following capabilities

- Define the distinguish name rules for the bank itself as well as for its counterparties.
- Define the rules for the business service used by various HVPS and CBPR+.
- Define Delivery Message Headers, indicating the schema, its version and the header elements, and associated them with a channel/service (Delivery Carrier).
- Apply a transformation to the business payload, if a transformation rule is indicated.
- Generate SAA technical header (XMLv2).
- Generate BAH specific to each service.
- Process Network acknowledgements (Ack/Nack).
- Process Delivery Notifications (positive, negative andoverdue warning).
- Calculate and attach the local authentication code (LAU), if enabled.
- Provide option to add locally a digital signature.
- Store the final outward message.
- Determine the channel for the inward messages based on the service name specified in the technical header.
- Validate the local authentication, if enabled.
- Validate the header details, based on the supplied schema.
- Route the inward messages to the Business Applications.
- Store the original inward message.

> **⚠️ Note:** The Delivery module generates the outward Interact ISO20022 messages in XMLv2 fomat. The Delivery module processes the inward Interact ISO20022 messages, Ack/Nack and Delivery notifications received in XMLV2 envelope.

The Temenos business modules like TPH and Account Statement can use the Delivery capabilities to send or receive Interact messages to SWIFT Alliance.

The Temenos SWIFT Interact Connector acts as an interface between the Transact Delivery Transformation Layer queues and the SWIFT Alliance messaging interface.

The following diagrams provide an overview on how various modules are linked to Delivery:


##### SWIFTNet Interact

SWIFT provides multiple messaging services like Interact, FIN, FileAct, etc. The Interact messaging service can be deployed in various modes :

- Real Time - Where both parties must be active.
- Store and Forward - Where the message sent by the sender is stored centrally by SWIFT until the receiver connects.
- Query and Answer - Where the sender sends the request in real time, and either receives the response from receiver or an error.

A SWIFTNet service uses a SWIFT messaging service, configured in the context of specific messaging solution. The messaging solution has a service administrator which decides the rules and policies around that solution.

> **⚠️ Note:** Delivery currently supports SWIFT Interact store and forward services – for example, SWIFTNet Funds, FINPlus service used by CBPR+, ESMIG T2 used by T2 RTGS consolidation, etc.


##### Interact Message Structure

The SWIFTNet Interact message structure is presented in the screenshot below:

- Request Header - It is used by the SWIFT Messaging Interface/ SWIFTNet network to determine the service to which the message must be sent, to distinguish name of the sender institution (also referred as Requestor), to distinguish name of the receiver institution ( also referred as Responder), the message type, etc.
- Request Payload - It is used by the Receiver Institution. The BAH is optional, it’s presence is the decision of the service owner/administrator. The BAH can be used by the Receiver to decide on the route flow for the respective message. The business document provides the required details of the respective transaction.
- Security - It allows the bank to include security features to the exchanged messages. For example, to include a local authentication code to ensure the message is not tampered between the Source Application and the Messaging Interface.

Delivery supports XMLv2 message format (also known as DataPDU) which is used by the SWIFT Alliance interfaces to exchange Interact messages with Application Systems like Transact.


##### Interact Terminology

Service Name - It is the name communicated by the service administrator to its members representing a service defined for a specific business purpose. It usually follows this pattern: “service administrator”.”service identifier” ”operational environment”

swift.finplus!p

Where,

- swift – Indicates the name of the service administrator
- FINPlufinplus service -– Indicates the name of the service communicated to the users
- .!p– Indicates the test and training environment,

If the “operational environment” is blank, this denotes the live environment.

Distinguish name - It is the logical name through which a user or system is identified in a domain. In the SWIFT world, the financial institutions are identified by their BICs, the Distinguish Names help to identify entities at a more specific level.

For example, the messages must be addressed to a specific entity of a financial institution, like, functional units and geographical locations.

T2 is the European real-time gross settlement (RTGS) system called which will be launched in Nov 2022. The name of the SWIFT Interact store and forward service used by T2 is esmig.t2.iast. The BIC assigned to T2 is TRGTXEPM but different distinguish names identify the RTGS (cn=rtgs,o=trgtxepm,o=swift) and CLM (cn=clm,o=trgtxepm,o=swift) components of the T2 system. The T2 ESMIG layer routes the messages received by T2 to the RTGS or CLM components based on the responder distinguish name indicated in the request.

The distinguish name definition follows this rule:

Level 4 (Common Name), Level 3 (Organisation Unit), Level 2(Organisation), Level 1 (Registration Authority)

Where,

- Level 3 and Level 4 are optional,
- Level 2 and Level 1 are mandatory.

cn=payments, ou=ho, o=bankbebb, o=swift denotes the traffic is addressed to institution BIC BANKBEBB – and more specifically to its payments entity/system, part of organisation unit ho.

Each institution which is using SWIFT network must register their Distinguish Names with SWIFT.

- Requestor Distinguish Name represents the distinguish name of the sending institution.
- Responder Distinguish Name represents the distinguish name of the receiving institution to which the message is addressed.
- Request Type represents the name of the message ISO message, for example, pacs.008.001.08.

SenderReference – Uniquely identifies the message being sent out

UserReference – The reference allocated to the message which will be also present in the responses


##### Business Application Header

The purpose of the Business Application Header(BAH) is to provide a consistent way to supply the basic details of the business message, regardless of the network and interfaces through the message is processed. The BAH has been designed by the ISO20022 community, its definition (head.001.01.0x) can be combined with any other ISO20022 message to form the business message.

The owner of a service decides the use of the BAH as part of the exchanged messages, its versions (for example, Target2 uses head.001.001.01, CBPR and CHAPS uses head.001.001.02) and rules (the mandatory/optional elements, their values, which elements take precedence – the elements in the BAH or the elements in the body of the message).


###### BAH Elements

- From element - Identifies the entity which has created the business message and it could be different from the sending address (Requestor Distinguish Name) in the technical header. For example in case of T2, the From element identifies the T2 member who sent the Business message but the Requestor Distinguish Name identifies the T2 ESMIG DN (T2 is implemented using a SWIFT V Copy architecture - messages are sent by the Instructing members to the central system which validates and then forwards the messages to the Instructed members).
- To element - Identifies the entity which has been indicated by the sender of the Business Message as the recipient of the message. Could be different from the receiving address (Responder Distinguish Name) in the technical header, for example, in the messages sent to T2 the Responder Distinguish Name is the T2 DN but the To Address identifies the Instructed Agent.
- Business Message Identifier - Indicates a reference allocated to the business message by the entity which is initiated the message to identify the message.
- Message Definition Identifier - Identifies the type of the message, for example, camt.053.001.08.
- Business Service - Identifies the service agreed between the entities exchanging the message.
- Market Practice - Identifies the market practice to which the message is aligned with.
- Creation Date - Indicates the date when the business message has been created.
- Possible Duplicate - Indicates if the exchanged message is a possible duplicate.

The example below shows an Business Application Header for a CBPR+ pacs.008 message:


##### SWIFT Multi-format MT MX Messages

The FINPlus service used by CBRP+ allows banks to exchange payment and payment-related MX messages. Until November 2025, banks will have the option to choose between MT and MX formats.

For CBPR+, SWIFT provides a translation from MT to MX and vice versa either at the Transaction Management Platform (for MT103/ MT202 COV, MT205 COV and pacs.002 reject, pacs.004, pacs.008, pacs.009 and COV messages) or as part of the FINPlus service (from CAMT to MT).

SWIFT allows banks to decide if they want to receive MT or MX messages for each of their BIC8 or BIC11. The bank can refine this decision based on the message type and/or currency.

Until November 2025, the SWIFT MX messages sent by financial institutions that have already adopted ISO20022 standards will be translated by SWIFT to MT before being sent to receiving institutions that are still using MT formats. In such cases, SWIFT sends a multi-format message to the receiving institutions representing the original ISO20022 message, which embeds the MT message as a comment.

The following is a (edited) sample of a multi-format MT MX message.

The receiving institutions can configure their SWIFT interface to send either the original message received from SWIFT or just the translated MT to the business application.

The following scenarios are possible from November 2022:

- Bank A is subscribed to the platform as an MT recipient and bank B as MX: Bank A sends to bank B MT and bank B receives MX translated from MT.
- Bank A is subscribed to the platform as an MT recipient and bank B as MT: Banks exchange MTs.
- Bank A is subscribed to the platform as an MX recipient and bank B as MX: Banks exchange MXs.
- Bank A is subscribed to the platform as an MX recipient and bank B as MT: Bank B receives MT translated from MX (as a multi-format message).

The Delivery Transformation Layer can receive multi-format messages and, depending on the parameterisation set up by the bank, either route the MX message (the default option) or the MT message to Temenos Payments Hub (TPH) or the Delivery module. In both cases, the original MX message is stored in the Delivery module.


##### Support for Allowed Character Set

SWIFT defined the basic character set for the CBPR+ messages and indicated that an extended character set is permitted for few ISO20022 elements. Real Time Gross Settlement systems like T2, CHAPS have also defined their allowed character sets.

Delivery allows the bank to define the supported characters for the XMLISO based channels.

For outward business messages formatted by Delivery, the character set rules are validated during the XMLISO formatting process. If there are any rules configured for the delivery carrier and the message type, Delivery identifies the message elements for which conversion rules are defined, applies the conversion rules and validates the resulted string with the allowed character set. The message is then emitted to the Delivery Transformation Layer.

Temenos business modules that generate the business messages directly (for example, TPH) use the Delivery configuration and invoke its conversion capabilities for each of the defined elements. Once the business payload is formatted the TPH emits the message to Delivery Transformation layer.

The Delivery Transformation Layer applies the payload transformation, if indicated in the message, adds the header details, appends the LAU, if configured and emits the final message to the integration queue. Please read the Message Data Handed off to Delivery for more details.

The inward messages are not validated with the allowed character set because SWIFT or the central RTGS system rejects the messages that do not comply with the allowed character set.


##### Support for Currency Transformation in Inward and Outward Messages

The Delivery module allows the bank to configure currency transformation between offshore and onshore bank currencies for both inward and outward messages.

Consider the onshore yuan as an illustrative example, identified by the ISO currency code, CNY. The onshore yuan is exclusively traded within Mainland China under stringent government control. In contrast, the offshore yuan, known as CNH operates beyond the confines of Mainland China. Notably, CNH does not have an official ISO 4217 currency code, reflecting its distinct status as an offshore currency.

The Delivery module facilitates the seamless exchange of SWIFT MX messages and helps the financial institutions the capability to transform the offshore to onshore currency and vice versa.

This functionality applies to the messages which are transformed through the delivery transformation layer. Read CNY to CNH currency conversion for more information on messages transformed by Temenos Payments .


#### ⚙️ Configuration

This section describes the configuration of the Delivery framework to process MX messages through SWIFTNet Interact services.


##### Delivery Message

The DE.MESSAGE application stores the definition of the message. The DE.MESSAGE records with the definition of ISO20022 messages are released by core - the Id of the DE.MESSAGE is given by the first 2 parts of the ISO message, without the ‘.’. This is optionally followed by ‘.’ and then by the message subtype, if any.

PACS009 is released for the financial institution’s credit transfers message and the PACS009.COV is released for financial institution’s credit transfer cover message.

If the message is not handed off to Delivery, the definition stored in DE.MESSAGE is very simple, indicating the Msg Name Id .

However, if the message is handed off and emitted through Delivery, it stores the definition of the tags.

The Message Name Id field in DE.MESSAGE stores the full message name of the default variant for the respective message, for example, pacs.008.001.08.

The preference for the Message Name Id can be also specified in DE.PRODUCT . This can be used to capture the preference for a specific variant for a given customer/account, if this differs from the default variant.

The preference for the Message Name Id is overridden by the setup in DE.CARRIER , where the bank can indicate the version which is used for a given message type. The DE.CARRIER can represent the channel to an RTGS system, for example, T2 ( Target2, the European settlement system) or another service in which the rules are enforced by a service administrator, in which case the variant is imposed by the rules of the administrator and not be the preference of a given participant.


##### Delivery Message Header

The DE.MESSAGE.HEADER application allows the bank to define technical and business headers which can be then added to the ISO20022 messages processed through Delivery (XMLISO processing). The following characteristics of the header can be specified in this application:

- The schema identifier - specifies the namespace of the header.

urn:iso:std:iso:20022:tech:xsd:head.001.001.02

- The type of the header - technical or business.
- Version of the header - 2.0.8.
- The list of the generic and business metadata that is part of the header.
- The format of the Create Date Time - Zulu ( also known as UTC format) or Local time with UTC offset.

The list of the metadata covers the header elements which are supported by Temenos and are required either by the SWIFT Alliance technical header (XMLv2) for Interact messages or by the ISO20022 Business Application Header.

The Business Metadata are supplied by the business application, the Generic Metadata are determined by Delivery but can be imposed by the business applications.

The following Business Metadata are currently supported by Delivery:

- Transaction Reference
- From Address
- To Address
- Instruction Priority

Currently Delivery supports the following generic metadata:

- Format
- Business Service
- Message Name Id
- SenderReference
- MemberId
- CreateDateTime
- DLNOverdueTime
- DLNRequested
- RequestorName
- ResponderName
- ServiceName

> **⚠️ Note:** The system evaluates and determines the metadata in the order in which they are defined; this is important as some of the metadata are used to determine the others, for example, the Business Service Rules depend on the Message Name Id. Implementations can still define and use headers for local channels as long as the messages are processed through Delivery using XMLISO formatting module.

The screenshot below shows the setup of the XMLv2 technical header

The screenshot below shows the setup of the BAH applicable to CBPR+ messages:

The screenshot below shows the setup of the BAH applicable to T2 messages. It can be noticed that a different schema and a different version is indicated in the setup for the T2 BAH comparing to the CBPR BAH and the metadata are slightly different as T2 doesn’t allow the Business Service as part of the BAH.

The Lcl Hdr Element Api field allows the bank to define a local routine which can handle local headers. This routine receives the following arguments:

- The Delivery Outward Header record linked with the current message.
- The Delivery Message Header record to which the routine is attached.
- The list of the Generic Metadata calculated by core, as name:value pairs, delimited by @SM.
- The list of the Business Metadata calculated by core (for the messages handed off via Delivery), as name:value pairs, delimited by @SM.

The output of this routine is:

- The list of the Generic Metadata updated by the local logic – which can update the values calculated for the core metadata and supplied as input argument but can also add local metadata and their values, using the same delimiter.
- Business meta data cannot be updated by the local routine.


##### Delivery Carrier

A dedicated Delivery Carrier has to be setup for each SWIFT Interact service/channel. The headers applicable to each service are defined using the DE.MESSAGE.HEADER and attached to the DE.CARRIER , the Formatting Module has to be set to XMLISO, Carrier Module as GENERIC.

The CBPRPLUS Delivery Carrier is released as part of the Delivery module. Delivery carriers for various RTGS systems are released by the verticals as part of their solution (TGT for T(arget)2, STG as part of CHAPS, etc.) For local channels, the implementation must setup the Delivery Carrier locally. Few other attributes must be set in the Delivery Carrier:

- The name of the SWIFTNet service through which the messages are processed, for example, swift.finplus in the CBPRPLUS Delivery Carrier.
- The format is MX.

If the Unique End To End Transaction Reference (UETR) must be generated/retrieved for certain messages types processed through the respective Delivery Carrier, the name of the respective message types has to be configured in the UETR Message field. Masking can be used, for example, pacs.008 means for any pacs.008 message.

If the service imposes rules regarding the variant(s) for the message types that can be exchanged, the specific variant(s) must be defined in the Delivery Carrier in the Message Name Id field associated with the respective Delivery Message .

If the Requestor DN (the Distinguish Name assigned to the bank) is the same for all messages sent through that service, this can be defined in the Overriding Requestor DN in DE.CARRIER . This overrides the setup in the DE.DISTINGUISH.NAME.RULES application. For performance reasons, it is recommended to use this setup where possible, rather than defining this in the DE.DISTINGUISH.NAME.RULES application.

If the Responder DN (the Distinguish Name assigned to the receiver) is the same for all messages sent through that service, this can be defined in the Overriding Responder DN in DE.CARRIER . For example, if an RTGS like T2 RTGS follows the SWIFT V copy architecture ( all messages are sent to the RTGS which forwards them to the destination, after the RTGS validations are passed) then all messages must be sent to the distinguish name assigned to the RTGS as the Responder DN. This overrides the setup in the DE.DISTINGUISH.NAME.RULES application. For performance reasons, it is recommended to use this setup where possible, rather than defining this in the DE.DISTINGUISH.NAME.RULES application.

Member Id can be used to capture the Member Id of the bank – this is currently not used by core but can be used by implementations..

The Format of the message must be set to MX.

The following screenshot shows the setup for the CBRPLUS DE.CARRIER which is used to process CBPR+ messages. The XMLV2 technical header as well as the CBPR+ Business Application Header are linked to this. No Overriding Responder DN is indicated in the Delivery Carrier. The Responder DN varies and is a direct translation of the Receiver BIC – a rule must be set for CBPRPLUS domain in the DE.DISTINGUISH.NAME.RULES application.

The screenshots below show the setup for TGT DE.CARRIER which is used to process T2 messages. The XMLV2 technical header as well as the T2 Business Application Header (BAH) are linked to the TGT carrier. The Overriding Responder DN indicates the distinguished name ( Responder DN) assigned to the RTGS system (ESMIG), as all messages are sent directly to ESMIG and not to the instructed banks (identified by the To Address in the BAH).

The offshore companies maintain the Nostro/Vostro accounts in offshore currency (CNH), hence the outward messages require transformation of the Chinese currency (that is, CNH to CNY) into the ISO currency to avoid the messages being rejected by SWIFT or local RTGS. The currency transformation (CNH to CNY) must be enabled for services/channels that send outward messages in offshore currency (CNH).

The Replace Currency field in the DE.CARRIER application configures the currency transformation for outward MX messages. This configuration explicitly instructs the delivery transformation layer to change the currency in the ‘From currency’ to the ‘To currency’ in the outward MX messages processed through the respective Delivery Carrier and this configuration is applicable only for the carriers that have Format Module set as XMLISO. The format for this configuration is ‘FromCurrency/ToCurrency’.

The following screenshots provide the configuration for the outward SWIFT MX Messages.


##### Delivery Interface

The DE.INTERFACE application stores the name of the Integration Queue where the final outward message is released. This is linked to the DE.CARRIER defined for the respective channel.

The outward Interact messages are picked from this queue by the Temenos SWIFT Connector and is sent to SWIFT Alliance queue/folder. Alternatively, the bank can use their own adapters to consume the messages from this queue.

The Ack Required field indicates if a SWIFT Ack/Nack is expected for the messages sent through this channel/service. Read Handle responses section in the Working with MX Interact messaging for more information.


##### Delivery Product

The bank can customise the preference for a certain customer or account by indicating the Message Name Id and the Transformation Rule that must be applied to the payload before sending the message out.


##### Distinguish Name Rules

The Requestor (Sender) and Responder (Receiver) Distinguish Name are mandatory elements for the Interact header.

The DE.DISTINGUISH.NAME.RULES application allows the bank to capture the rules based on which Delivery can determine the distinguish name for the bank itself as well as for the receiving counterparty. The following attributes are mandatory in the DE.DISTINGUISH.NAME.RULES :

- Scope - Specifies if the rule applies is for the Requestor DN or for the Responder DN.
- Domain - Indicates the Delivery Carrier for which the rule is used.
- Status - Determines if the rule is Active, Expired or Cancelled.
- Distinguish Name or a Distinguish Name Rule - The user can specify either of them. This is the value which is assigned to the Responder/Requestor Name metadata if all other conditions are met. Two different Distinguish Name rules are supported by core: DefaultDnLevel3 - Determines the DN based on the supplied (To/From)Address, assuming the To/From Address is a BIC, using the following logic: ou=last 3 chars from BIC11 or xxx if a BIC8 or 9 is supplied, converted to smalls, o=BIC8(converted to small cases), o=swift DefaultDnLevel2 - Determines the DN based on the supplied (To/From)Address, assuming the To/From Address is a BIC, using the following logic: o=BIC8(converted to small cases), o=swift
- Start Date and End Date - Specify if a certain rule becomes effective at a future date (Start Date) or it stops being effective at a certain date (End Date).
- Customer, Address, Message Type and Currency - Define rules specific to a customer, address, message type, currency. If not specified, it means the rules apply to any customer, address, message type, currency.
- Message Type - Identifies a specific DE.MESSAGE .
- App Context Field and App Context Field - Define rules based on the content supplied by the Business Application. ORIGINATING.SOURCE and SUB.TYPE.INDICATOR are currently supported for App Context Field .

The above screenshot shows the rule released as part of the Model Bank setup – for all CBPRPLUS messages, irrespective of the receiver’s customer number, address, message type, ccy, or other values supplied by the Business Applications generating the message, the Responder DN is decided based on the To Address supplied in the message (and stored in the DE.O.HEADER created for the respective outward message), using the DefaultDNLevel3 rule.

- If the To address indicates the BNABFRPP BIC, then the Requestor DN is set to ou=xxx,o=bnabfrpp,o=swift.
- If the To Address indicates BNABFRPPABC, then the Requestor DN is set to ou=abc,o=bnabfrpp,o=swift.

The following screenshot shows how the Responder DN is defined for all messages sent through FUNDS Delivery Carrier to the BBHCUS3I address, irrespective of the message type, currency or other values supplied by the Business Application.


##### Business Service Rules

The Business Service is an optional attribute of the ISO20022 Business Application Header and is used by CBPR+ as well as certain national RTGS which have adopted ISO20022 messages.

The DE.BUSINESS.SERVICE.RULES application captures the rules for the Business Service. Delivery uses this application to determine the rules applicable to the Business Service metadata, when this metadata is parameterised in the DE.MESSAGE.HEADER linked to the Delivery Carrier through which the outward message are processed.

- Domain, Business Service and the Status - Fields of the rule are mandatory elements in the DE.BUSINESS.SERVICE.RULES application.
- Message Name Id - Allows the bank to define the message type to which the Business Service Rule applies. The Business Application is the system Id of the module generating the message.
- App Context Field and App Context Field - Define rules based on the content supplied by the Business Application. The SUB.TYPE.INDICATOR is currently supported for App Context Field.
- Business Service - It is the actual value assigned to the Business Service metadata, if the outgoing message satisfies all the other conditions.

The screenshot below shows the setup for the PACS.008.STP messages processed through CBPRPLUS Delivery Module, initiated by TPH, which has the Sub Type Indicator (supplied to Delivery in the App Context Field ) as STP(supplied to Delivery in the App Context Value ).


##### Delivery Notification Requirements

The bank can indicate in the DE.CARRIER if they want to request a positive Delivery Notification message ( Dln Requested set to Yes) for all the outward messages processed through that carrier as well as the Overdue Time Interval , after which the bank expects to receive an overdue delivery notification.

Alternatively, if the positive DLN is required only for certain message types, the bank can define these requirements in the DE.DLN.REQUIREMENTS application.

The ID of this record is the combination of the ID of the Delivery Carrier followed by ‘-‘ (dash) and the ID of the Delivery Message. See below an example to request a positive delivery notification for CBPR+ pacs.008 messages – for EUR messages, the delivery notification is requested only for messages which have the amount bigger than 100,000 and the overdue notification is expected if the message was not successfully delivered in the next 15 minutes. For any other currency the minimum amount for which the delivery notification is requested is 10,000, the overdue notification interval is 1 hour.


##### Delivery Parameter

The DE.PARM application is used to define the Transact Business Modules to which the responses ( Ack/Nack/DLN) must be notified.

Currently only TPH is able to process responses for the outward messages, the configuration below enables Delivery to send the responses received for messages initiated by TPH ( Reply to Appln ) to the queue indicated in the Response Queue Name field.

The Exclude Message Type field defines the message initiated by TPH, for which Delivery does not forward the responses to TPH.


##### IF Exit Point Setup

For messages handed off to the Delivery Transformation Layer by the Delivery module, the XMLISO service, after it determines the header metadata, emits the message through the Integration Framework using the OutwardMessageService.emitOutwardMessage exit point- the configuration for this exitpoint is released in the IF.EXIT.POINTS and IF.INTEGRATION.FLOW.CATALOG applications.

> **⚠️ Note:** The Integration Framework uses the setup in the IF.INTEGRATION.SERVICE.PARAM application to define the queue where the message is emitted. This must be parameterised by the bank to point to the queue identified by the attribute defined in DEHandoffQueue in the QueueConfigMXOutward.properties file used by the Delivery Transformation Layer.


##### Delivery Transformation Layer – Inward Processing Parameterisation

The Delivery Transformation layer processes the inward messages based on the setup in the DE_SWIFTInward_QueueConfig.properties file. The file specifies the queues through which the messages are moved during processing, the rules to determine the source channel as well as the routing decision to the internal/destination channel that identifies the business application to which the message must be forwarded and the transformations that are applied to the message. Each of these sections are described below.

- SWIFTInputQueue - The inward message queue, where the integration layer (Temenos SWIFT Connector) passes the Interact message received from SWIFT Alliance. Delivery Transformation Layer picks up the message from this queue and processes this further.
- RouteChannel=ACTIVEMQ - Indicates the internal processing of the message is done using queues (ActiveMq); Possible values are ACTIVEMQ or FILESYSTEM;

> **⚠️ Note:** FILESYSTEM is only for testing purpose.

- DEBackupQueue - The queue where Delivery Transformation Layer writes a copy of the inward messages, once the message is picked from SWIFTInputQueue queue, for audit purpose.
- MXInputQueue - The intermediary queue where the inward MX messages is routed .
- MXRejectQueue - The queue where the message is moved in case of any failure during MX processing, for example, xsd validation failure or the failures related to local authentication.
- T24DeliveryQueue - The queue to which the messages are sent to Delivery sub system to create the Delivery Inward Header and store the original message.
- OFSRequestQueue - The queue to which the messages are sent for timeout polling.
- T24AppQueue - The queue which stores the copy of the message sent to the OFSRequestQueue. After the response is received from Delivery confirming the DE.I.HEADER is created successfully, the copy of the message is picked from this queue and is sent to the queue decided based by the routing decision .
- IntervalTime - The polling interval to wait for the response from Transact Delivery Subsystem that the Delivery Inward Header for the inward message has been created.
- DeliveryResponseQueue - The queue where Delivery Subsystem returns the response indicating if the Delivery Inward Header has been created and the original message stored.
- AdmiInputQueue - The admi inward messages are moved directly to TPH queue, overpassing Delivery.
- SwiftDataProtectRequestQueue – The queue to which the Delivery framework directs SWIFT messages for data pseudonymization when the user sets the ‘IsAppDataProtected’ property as TRUE. The Temenos exchange adapter encrypts user-classified data in XML messages by consuming them from this queue to enable data privacy before they reach Temenos Transact.
- SwiftDataProtectReplyQueue – The queue to which the Temenos exchange adapter transmits the pseudonymized message responses upon successful encryption.
- SwiftDataProtectErrorQueue - The queue to which the Temenos exchange adapter transmits error responses for the pseudonymized messages during encryption failures.

The environment variable XSD_ROOT_DIR decides the location of the properties files as well as the location of the schemas validation folders.

As shown in the screenshot below, the properties files used by the Delivery Transformation Layer are located under the folder indicated in the XSD_ROOT_DIR environment variable.

The service name in the technical header (XMLV2 envelope) determines the source channel which is used to identify the name of the folder where the XSDs for the respective channels are stored.

SWIFT frequently changes the technical header schema (XMLv2) to introduce new features in the Alliance Access, SWIFTNet, and other systems. The bank uses different versions of the schema. Temenos currently supports the XMLv2 schema version 2.0.12. The bank can use another schema version if that does not have additional mandatory elements.

To use a different XMLv2 version, Temenos cannot access to SWIFT saa schemas. The bank must copy the schema from their Alliance Access product and place it in the folder structure mentioned above. For example, if the bank needs to use the 2.0.13 version schema, the user must place this in the XSD folder under PP_HOME path and rename as saa.2.0.13.

> **⚠️ Note:** If the schema version the bank wants to use introduces mandatory elements, the bank must contact Temenos.

For example, considering the following setup in the inward properties file:

esmig.t2.iast=T2

swift.finplus=CBPRIN

swift.chaps=STGIN

Three different folders namely CBPRIN, STGIN and T2 are defined under the main folder identified by the XSD_ROOT_DIR .

The Delivery Transformation Layer validates the message is received in the XMLV2 envelope as well as BAH, if present.

The name of the schemas in this folder must match the namespace of the XMLv2 envelope (saa.2.0) as well as the namespace of the BAH (head.001.001.02 in case of CBPRPLUS).

The saa.2.0 contains a simplified XMLv2 schema defined by SWIFT, with the main elements expected by the Delivery Transformation Layer.

The AckNackTemenosFormatXsd attribute identifies the name of the schema that is used to validate the inward Ack/Nack/Delivery Notifications, once they have been transformed into Temenos Standard Response format. This is located on the main XSD folder.

The XSLT are located in the folder identified by the XSLT_ROOT_DIR variable.

- The InwardGenericOfsConversion.xslt file stores the transformation which extract the details required to create the Delivery Inward Header and send the original message to Delivery.
- The TransmissionReportXslt and DeliveryReportXslt attributes identifies the files that stores the transformations which are applied to TransmissionReport (Ack/Nack) and DeliveryReport (Delivery Notifications) to transform them in Temenos Standard Response Format before sending them to Delivery.

For LAU validation and Digital Signature validations the Delivery Transformation Layer consults the DE_SWIFTInward_InwardIntegrity.properties file.

The setup in this file is based on the Source Channel which is used as a prefix.

- -LAU-IntegrityCheckRequired - If this is set to TRUE, indicates LAU must be checked for all messages received from the respective source channel; if FALSE then LAU is not checked
- -LAU-Compliance - Indicates the keystore where the bilateral keys used to validate the LAU code supplied in the inward message are stored. Read Working with Swift Security Program for more details on LAU and how the bilateral keys are stored.
- -BAH-IntegrityCheckRequired - Is currently not used.
- -BAH-Compliance - Indicates the keystore.
- -APIName - The Local API which is used to check the BAH signature. The following screenshot shows an example of the setup configured in the DE_SWIFTInward_InwardIntegrity.properties file

The decision to route the inward messages to various Business Applications are based on combining several criteria:

- MessageType
- Sender
- ResponderDN
- Receiver
- RequestorDN
- ServiceIdentifier

The ‘*’ can be used as a wildcard, to replace any value. For Message Type, the first two parts of the ISO20022 Message Name Id should be used, without the ‘.’.

The routing criteria identifies an internal channel to which the message is forwarded, for example:

Considering the above setup:

- All inward messages from ESMIG are sent to the internal channel T2.
- All inward camt.054 messages from CBRPLUS are sent to internal CAMT54 channel.
- All inward camt.057 messages from CBRPLUS are sent to internal CAMT57 channel.
- All other messages from CBRPLUS are sent to CBPRIN channel.
- All inward messages from CHAPS are sent to STGIN channel.

Once the internal Channel is established, the following attributes decide the processing further, each of them being prefixed by the Channel:

- -ACTIVEMQ - Indicates the name of the queue where the message is placed.
- -FILESYSTEM - Indicates the name of the folder where the message is placed ( used by Temenos for internal purposes).
- -Carrier - Indicates the name of the Delivery Carrier through which the message is processed.
- -SkipRouting -Indicates if the message is sent directly to the Business Application or is routed by the Delivery which and processes this based on the inward routine indicated in the DE.MESSAGE.
- -Carrier must have the Formatting Module field set to SWIFT.
- -Carrier must have Formatting Module set to XMLISO.
- -Xslt - Indicates the name of the xslt that is applied to the payload message before being routed to the Business Application.

For example, consider the following setup:

After the Delivery Transformation Layer has determined the internal channel is CBPRIN, it routes the message directly to the business application queue indicated above. No specific transformation is applied to the original payload message. The Delivery Inward Header created for this message indicates the CBPRPLUS Delivery Carrier.

The setup below corresponds to the messages processed through the internal ChannelCAMT57:

These messages are routed by Delivery, the XSLT indicated is applied to the business payload before the message is sent to Delivery. The CBPRPLUS Delivery Carrier is indicated in the Delivery Inward Header for these messages.

| Attribute | Description |
|---|---|
| ReplaceCurencyForReceivingBICS | Indicates the delivery transformation layer to perform currency transformation from a specific currency to another, with the option to exclude this for specific receiving BICs (BICs separated by a comma,","). Format: FromCurrency/ToCurrency/[ReceiverBIC1,ReceiverBIC2, and so on] |


##### Delivery Transformation Layer – Outward Properties Parameterisation

The Delivery Transformation layer processes the outward messages based on the setup in the DE_SWIFTOutward_QueueConfig file, which describes the queues through which the messages are moved during processing, the identification of the destination, the transformations that are applied to form the headers, the setup related to local authentication and digital signatures. Each of these sections are described below.

- RouteChannel - Indicates the internal processing of the message is done using queues (ActiveMq) and the possible values are ACTIVEMQ or FILESYSTEM.

> **⚠️ Note:** FILESYSTEM is only for testing purpose

Queues to Delivery Transformation Layer

- DeliveryPollingQueue - The queue where the Business Applications sends messages to Delivery Transformation Layer.
- SwiftPollingQueue and ChapsPollingQueue - Additional queues where TPH sends the SWIFT and Chaps related messages.
- DEHandoffQueue - The queue where Transact Delivery sends the messages mapped and emitted by Delivery via Integration Queue and this is used when the Business application handoffs the data to Delivery to map the messages.

Validation and Transformations Related Setup

The environment variable XSD_ROOT_DIR decides the location of the properties files as well as the location of the schemas validation folders.

As shown in the screenshot below, the properties files used by the Delivery Transformation Layer are located under the folder indicated in the XSD_ROOT_DIR environment variable.

folder, created under the folder structured identified by the XSD_ROOT_DIR variable.

SWIFT frequently changes the technical header schema (XMLv2) to introduce new features in the Alliance Access, SWIFTNet, and other systems. These changes happen more often than the annual standard changes and the bank uses different versions of the schema. Temenos currently supports the XMLv2 schema version 2.0.12. The bank can use another schema version if that does not have additional mandatory elements.

To use a different XMLv2 version,

- The bank must configure the version of the schema they want to use in the in the Header Version field of DE.MESSAGE.HEADER .
- Temenos cannot access the SWIFT saa schemas. The bank must copy the schema from Alliance Access product and place it in the folder structure mentioned above. For example, if the bank needs to use the version 2.0.13 schema, the user must place this in the XSD folder under PP_HOME path and rename as saa.2.0.13.

> **⚠️ Note:** If the schema version the bank wants to use mandatory elements, the bank must contact Temenos.

- T24DeliveryQueue - The queue through which the Delivery Transformation Layer notifies Transact Delivery about the final message being sent out and/or the processing result based on which the disposition of the Delivery Outward Header is updated.
- T24BackUpQueue - The queue where Delivery Transformation Layer sends a copy of the message sent to Transact Delivery.
- IntegrationOutputQueue - The default queue to the integration layer. Temenos SWIFT Connector should pick the messages from this queue.
- IntegrationErrorQueue - The queue where the rejected messages are moved (for example failures with the XSD validation).
- SwiftDataProtectRequestQueue – The queue to which the Delivery framework directs SWIFT messages for data reconstruction when the user sets the ‘IsAppDataProtected’ property to TRUE. The Temenos exchange adapter decrypts user-classified data in XML messages by consuming them from this queue to enable data reconstruction before they reach the IntegrationOutput Queue.
- SwiftDataProtectReplyQueue – The queue to which the Temenos exchange adapter transmits responses for the reconstructed messages upon successful decryption.
- SwiftDataProtectErrorQueue - The queue to which the Temenos exchange adapter transmits error responses for the reconstructed messages during decryption failures.

For LAU validation and Digital Signature check Delivery Transformation Layer consults the the DE_SWIFTOutward_OutwardIntegrity.properties file.

The setup in this file is based on the outward Channel which is used as a prefix – this is determined based on the OutCarrier specified in the messages received by the Delivery Transformation Layer.

- -LAU-Required - If this is set to TRUE, indicates LAU must be calculated and added to all messages sent to this channel; if FALSE then LAU is not calculated for these messages.
- -LAU-Compliance - Indicates the keystore where the bilateral keys used to calculate the LAU code are stored. Read Working with Swift Security Program for more details on LAU and how the bilateral keys are stored.
- -APIName - Indicates the Local API which is used to calculate and add the BAH signature; if blank then no digital signature is added.
- -BAH-Compliance - Indicates the keystore.
- -IntegrityRequired – Currently not used.


##### Support for Allowed Character Set

The ASCII.VAL.TABLE application allows the bank to define the characters sets used for various purposes, for example, the ISO basic character set used by CBPR, the SWIFT character set used for SWIFT MT messages exchanged across the SWIFT FIN service and so on.

The DE.ALT.CHARS application defines the conversion rules for the characters which are not part of the allowed char set indicated by the Valid Ascii Table field.

For each unsupported character specified in the Local Char Code field, the alternate character(s) to which it must be converted is defined in the Alter Char Code field. Alternate characters are defined based on the position of the unsupported character. For example, if the local character code is the first character in a string, the associated Char Position field must be set to First. For any other position, Char Position field is set to Other or left blank.

The extended character set ISOEXTENDED is available in the Model Bank and defined in DE.ALT.CHARS record.

The Def Alt Char Code field is used to define the default character to which the unsupported characters are converted without specific setup. Space can be specified as a default character using its ASCII value.

The DE.MSG.CHARS.RULE parameterisation table provides the option to specify the message element tags that must be validated for each channel and message type. For each of these tags, the corresponding DE.ALT.CHARS record indicates the conversion rules that apply.


###### Example

This section demonstrates the translation of unsupported characters in an MT942 message based on different configurations.

CONV* is already configured for Tag61 in DE.FORMAT.SWIFT for MT942 as shown below.

Configure the DE.ALT.CHARS ID in DE.CARRIER . This is referred from the Delivery layer, during MT message generation to replace the special characters with alternate characters as configured in DE.ALT.CHARS .

A TPH transaction posted with a special character in the sender’s reference which is not a valid swift character is shown below.

A default character is not defined.

When a MT942 message is generated, since the special character (@) has no alternate character configured in DE.ALT.CHARS , it is not replaced.

A default character is defined.

When a MT942 message is generated, since the special character (@) has no alternate character configured in DE.ALT.CHARS , it is replaced with the default character defined in DE.ALT.CHARS as shown below.

An alternate character for @ is defined as “:”.

When a MT942 message is generated, since the special character (@) has an alternate character configured in DE.ALT.CHARS as “:”, it is replaced with the alternate character as shown below.


#### 📋 Tasks

Interact is a SWIFTNet messaging service, which is used to send and receive financial messages in XML format. SWIFTNet Interact based services are designed to exchange the ISO20022 payments and payments related messages.

Temenos delivery module enables the exchange of the ISO20022 messages with a SWIFT messaging interface.


##### Workflow

In the SWIFTNet Interact MX Services, the user can perform the following activities:

Users can able to resubmit a message, which has the message disposition WaikAck/WaitDLN/DLNOverdue by changing the message disposition to Resubmit.

To amend an in progress outward header record, follow the below steps:

1. Delivery Response Details .
2. In the In Progress Outward Header tab, search records with delivery carrier name.
3. Click the Amend icon.
4. Select Resubmit or Delete option from Message Disposition field and save the record.
5. Click the Validate icon to check for errors and overrides.
6. Click the Commit icon.

Users can able to change the response status from Unmatched to Manually Matched or Completed.

To change an unmatched delivery response, follow the below steps:

1. Delivery Response Details .
2. Click the Delivery Responses tab.
3. Click the Edit icon corresponding to a record and then change the status from Unmatched to Manually Matched or Completed.
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon.

Users can authorise all the unauthorised delivery response records.

To authorise a delivery response record, follow the below steps:

1. Delivery Response Details .
2. Click the Unauthorised Delivery Responses tab.
3. Choose the record and click the Authorise icon.
4. Click the Validate icon to check for errors or overrides.
5. Click the Commit icon.

Users can define the rules to request a positive or overdue delivery notification.

To create a new DLN requirement record, follow the below steps:

1. DLN Requirements .
2. Click the New deal icon.
3. Enter the values in below fields: Currency Min Amt Overdue Time Interval Default Min Amt Def overdue Time Interval
4. Click the Validate icon to check for errors and overrides.
5. Click the Commit icon.


#### 📊 Outputs

The user can view the below list of enquiries and reports pertaining to SWIFTNet Interact MX Services in the Temenos Transact .


##### Enquiries and Reports

The user can view the below list of enquiries and reports:

Delivery Response Details

- Outward Header Details – It shows all the outward header records with drill-downs to outward header details, view message details and related response details.
- Inward Header Details – It shows all the inward header records with drill-downs to inward header details and view SWIFT message.
- Archived Outward Headers – Users can view all the archived outward header records with drill-down to view delivery outward header details and delivery response details.
- Archived Inward Headers – Users can view all the archived inward header records with drill-down to view inward header details and view SWIFT messages.


##### SWIFT Messages

NA


##### Advices

NA


##### Alerts

NA


> **Related Applications:** `ASCII.VAL.TABLE`, `DE.ALT.CHARS`, `DE.BUSINESS.SERVICE.RULES`, `DE.CARRIER`, `DE.DISTINGUISH.NAME.RULES`, `DE.DLN.REQUIREMENTS`, `DE.FORMAT.SWIFT`, `DE.I.HEADER`, `DE.INTERFACE`, `DE.MESSAGE`, `DE.MESSAGE.HEADER`, `DE.MSG.CHARS.RULE`, `DE.O.HEADER`, `DE.PARM`, `DE_SWIFTInward_InwardIntegrity.properties`, `DE_SWIFTInward_QueueConfig.properties`, `DE_SWIFTOutward_OutwardIntegrity.properties`, `DE_SWIFTOutward_QueueConfig`, `IF.EXIT.POINTS`, `IF.INTEGRATION.FLOW.CATALOG`, `IF.INTEGRATION.SERVICE.PARAM`, `InwardGenericOfsConversion.xslt`, `QueueConfigMXOutward.properties`, `XSD_ROOT_DIR`, `XSLT_ROOT_DIR`

---


### 2.37  TemplateFormat Printing


> **📇 Quick Reference Card**
> 
> **Purpose:** *Temenos Transact Delivery can hand over message data to a Windows application (such as Word), so that the formatting and printing of the document is done outside the delivery system. This means that all the functionality of Word is available, giving a enhanced formatting capabilities, for example, m...*
> 
> **Applications:** `DE.FORMAT.TEMPLATE`
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Temenos Transact Delivery can hand over message data to a Windows application (such as Word), so that the formatting and printing of the document is done outside the delivery system. This means that all the functionality of Word is available, giving a enhanced formatting capabilities, for example, multiple fonts and styles, headers and trailers, watermarks, inclusion of graphics and pictures. This is achieved through the DE.FORMAT.TEMPLATE application.


> **Related Applications:** `DE.FORMAT.TEMPLATE`

---


### 2.38  Translation DeliveryMessages


> **📇 Quick Reference Card**
> 
> **Purpose:** *The DE.TRANSLATION application is used to convert codes passed in the messages into descriptive text (in various languages). It is also used to enter all the SWIFT field codes. This serves two purposes:*
> 
> **Applications:** `DE.AUTO.TRANSLATION`, `DE.FORMAT.PRINT`, `DE.FORMAT.SWIFT`, `DE.MM.SETUP.TRANSLATION`, `DE.TRANSLATION`
> 
> **Key Fields:** *Conversion*, *Last Run*, *OT*, *Update*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The DE.TRANSLATION application is used to convert codes passed in the messages into descriptive text (in various languages). It is also used to enter all the SWIFT field codes. This serves two purposes:

- To validate codes entered in DE.FORMAT.SWIFT .
- To put meaningful descriptions against the fields in SWIFT messages, if they need to be displayed for inspection.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 🔧 Working With

Codes to be translated by the formatting modules have a prefix (defined in the appropriate format application) inserted before accessing the DE.TRANSLATION application. If a prefix is not specified, SW (the default) is used. The field tags use this prefix.

The SWIFT field tag 50 means that the ordering customer is in the

application with the ID of SW50. If a different description of a tag is required when it occurs in a particular message type, then the description should be entered in

in the format SWtt-mmm. For example, SW50-900 for tag 50 in MT900.

These records can be entered manually or automatically created from the database using a load or update application.

- DE.AUTO.TRANSLATION – A browser compliant record for each auto update required.
- DE.MM.SETUP.TRANSLATION – A legacy application which works on classic display terminals.

For print formatting, a special prefix can be specified in the Conversion field of the DE.FORMAT.PRINT record. Then the required text is placed in the DE.TRANSLATION application with the prefix and code as the ID. This technique allows the applications to use the same code for different types of data or to translate the same code differently in various sorts of messages.

| Field | Conversion |
|---|---|
| Commiss | TABLE COM |
| Tax | TABLE TAX |


##### Setting up Frequent Tables for Translation

The DE.AUTO.TRANSLATION application is used for applications used as a source of translation text that are updated more frequently. The input selections are stored and can be re-run easily.

As this is a W type application, the user can input the criteria to build the DE.TRANSLATION records and save the criteria for updates or rebuilds as required. The V function is used to run the build process. The DE.AUTO.TRANSLATION application is used to setup the DE.TRANSLATION application, but it is also used to update the DE.TRANSLATION application from time to time.

The DE.TRANSLATION application is delivered with various records, which should not be deleted. In addition, there are records required by formats, which are file dependent and must be added to the DE.TRANSLATION application after the files have been updated. For example, category codes are passed to delivery for translation in printed messages.

The DE.AUTO.TRANSLATION application allows the user to choose the application, prefix, separator, as well as the field name to be used for the text. When this application is run with Update field settings, it can be for New (create new records only) or ALL (update all records). The Last Run field specifies the date to display the last activity.

If a field is specified in the format tables as requiring translation, the field with the appropriate prefix is looked up in the DE.TRANSLATION application. If the record is not found in the DE.TRANSLATION application, the message is placed in the repair queue. Therefore, it is important always to keep the DE.TRANSLATION application up to date. If new records have been added to any of the above applications, the DE.TRANSLATION application must be updated accordingly. It is updated either by running the setup translation or by entering the records directly into the DE.TRANSLATION application.


##### Legacy setup for Translation

The DE.MM.SETUP.TRANSLATION application enables the user to copy the description from all records in a particular file to the DE.TRANSLATION application, prefixing the codes with the prefix required in formatting.

Initially, the user is prompted to confirm if he wants the records in the DE.TRANSLATION application to be overwritten. If Y is entered, the existing records are updated (but never deleted). If N is entered, the records that do not exist alone is created. The user is required to enter the file name (without company mnemonic) from which the records are to be copied and the prefix to be used when updating the DE.TRANSLATION application.

> **⚠️ Note:** This setup in the DE.TRANSLATION application always copies the description from the first field in the record being copied from. Therefore, for records copied from the DE.TRANSLATION application, where a short description is required (TXNS), the description in the DE.TRANSLATION application must be amended to the required length.


#### 📋 Tasks

There are no Tasks available for Translation of Delivery Messages feature.


#### 📊 Outputs

There are no Outputs available for Translation of Delivery Messages feature.


> **Related Applications:** `DE.AUTO.TRANSLATION`, `DE.FORMAT.PRINT`, `DE.FORMAT.SWIFT`, `DE.MM.SETUP.TRANSLATION`, `DE.TRANSLATION`

---


### 2.39  Unique End-to-End Transaction Reference


> **📇 Quick Reference Card**
> 
> **Purpose:** *A Unique End-to-End Transaction Reference (UETR) is a string of thirty-six unique characters featured in all payment instruction messages carried over SWIFT FIN and FINPlus services. The UETR identifies a payment transaction, where all SWIFT users originating payments must provide a UETR as standard...*
> 
> **Applications:** `DE.CARRIER`, `DE.O.HEADER`, `DE.UETR.CATALOG.LIST`, `DE.UETR.REF.FILE`, `FUNDS.TRANSFER`, `MD.DEAL`, `SWIFT.PARAMETER`
> 
> **Key Fields:** *Fwd Msg Type*, *Uetr Message*, *Uetr Msg Type*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

A Unique End-to-End Transaction Reference (UETR) is a string of thirty-six unique characters featured in all payment instruction messages carried over SWIFT FIN and FINPlus services. The UETR identifies a payment transaction, where all SWIFT users originating payments must provide a UETR as standard for each of the MT 103, MT 103 STP, MT 103 REMIT, MT 202, MT 205, MT 202 COV, MT 205 COV, pacs.008, pacs.008 STP, pacs.009, pacs.009.COV and pacs.009.ADV message types. As the UETR is uniquely assigned to a payment transaction, the payment message and its related cover payment message must have the same UETR.

All other parties involved in the respective payment transaction must use the supplied UETR when they forward the payment message to the subsequent parties.

SWIFT Tracker is a central solution developed by SWIFT which monitors the UETR sent in the payment messages. Using UETR, banks can locate the latest counterparty that received the payment. It provides a very strong tool in case of delays or payment not reaching beneficiaries.

Charge request or advice messages, free messages, queries and answers must indicate the UETR of the original transaction. The Delivery module generates the UETRs unless instructed otherwise by a business module.

- If the business module can generate and impose the UETR, the Delivery module uses the UETR.
- If the UETR is not imposed: For Payment modules - The Delivery module assigns the UETR to the first message received with a specific Transaction Reference. For the next message with the same Transaction Reference, the Delivery module uses the same UETR. The Temenos Payments Hub (TPH) and Funds Transfer (FT) modules do not re-cycle the UETR. For non-payment modules - The Delivery module assigns a new UETR for each message, irrespective if a UETR was already assigned for the respective Transaction Reference. Non-payment modules can generate multiple SWIFT MT payment messages and pass the same Transaction Reference that identifies the contract number. Modules that generate payment and cover messages must impose the UETR in both messages.

For Non-payment modules that generate payment orders, the UETR is assigned when TPH hands off the data for the payment message. The Transaction Reference in this case identifies the reference assigned by TPH to the transaction.


#### ⚙️ Configuration

The fields to be configured in the SWIFT.PARAMETER application for SWIFT MT messages are listed in the below table.

| Field | Description |
|---|---|
| Uetr Msg Type | A multi-valued field in the SWIFT.PARAMETER application that holds the message types that require a UETR reference to be mapped in the outgoing message. |
| Fwd Msg Type | A multi-valued field that holds the message types that require a UETR reference to be forwarded in the outgoing message. |

The screenshot below shows the Uetr Msg Type and Fwd Msg Type fields in the SWIFT.PARAMETER application.

The field to be configured in the CBPRPULS record of the DE.CARRIER application for SWIFT CBPR messages is listed in the below table.

| Field | Description |
|---|---|
| Uetr Message | A multi-valued field in the CBPRPULS record of the DE.CARRIER application that holds the message types that require a UETR reference to be mapped in the outgoing message. |

The screenshot below shows the Uetr Message field in the DE.CARRIER application.

Use the below reference links to know more about UETR:

- Refer SWIFT 2018 Rulebook Changes for more information on the usage of UETR.
- Refer SWIFT 2019 Rulebook Changes for more information on the usage of forwarding UETR.
- Refer UETR Recycling Validation - Principles and Use Cases by SWIFT for more information on UETR.


#### 🔧 Working With

The Delivery module generates a Unique End-to-End Transaction Reference (UETR) unless instructed otherwise by the business module. The files used in UETR are listed below:


###### DE.UETR.REF.FILE

Serves as a cross-reference between the transaction reference of the contract and the corresponding UETRs. This file allows more than one UETR to be stored for the same transaction reference and header record ( DE.O.HEADER reference), for which the UETR was generated or allocated for a specific transaction reference delimited by pipe (I). The ID of the application is the transaction reference of the contract.


###### DE.UETR.CATALOG

Provides the transaction reference of the contract and delivery reference for each UETR available in the system. The ID of the application is the UETR ref.


##### Imposing the Received UETR for Outward Messages

If the Temenos non-payment business module has already created a UETR and given it to the Delivery module, the Delivery module can use the same UETR for the transaction, even if it has already been linked to an existing transaction reference. This means, the Delivery module does not generate a new UETR but uses the one provided by the business module.

The Delivery module incorporates the UETR populated in header element of the data received from the business modules to the Uetr Reference field of the header record ( DE.O.HEADER ).

The Delivery module checks whether there is an existing record in DE.UETR.REF.FILE for the given transaction reference.

- If no record is found, a new record in DE.UETR.REF.FILE is created with the received UETR along with the header reference ( DE.O.HEADER ).
- If a record is found, the existing record is updated by appending the received UETR as an additional value and the header reference ( DE.O.HEADER ) for which the UETR is included.


##### Generating a New UETR If Not Imposed for Outward Messages

Temenos non-payment business module generates more than one SWIFT MT message with the same transaction reference which identifies the contract. In this case, if the business module has not imposed a UETR, then the Delivery module generates a new UETR, irrespective if the system has already assigned a UETR for the same transaction reference.

The Delivery module checks whether there is an existing record in DE.UETR.REF.FILE for the given transaction reference.

- If no record exists, a new record in DE.UETR.REF.FILE is created with the generated UETR along with the header reference ( DE.O.HEADER ).
- If a record is found, the existing record is updated by appending the generated UETR and the header reference ( DE.O.HEADER ) for which the UETR is generated.

Scenario 1 - Generating a UETR in the FT Module

In this scenario, the user creates a record in the the

application that generated both MT103 and MT202 COV messages.

As the MT202 COV belongs to the same transaction where the MT103 was also generated, the Delivery module re-uses the same UETR for both the message types. The screenshot below is an example of the transaction in DE.UETR.REF.FILE showing the UETR delimited with delivery reference.

> **⚠️ Note:** If multiple messages are generated and a single UETR is used, then only one header record is delimited with UETR in DE.UETR.REF.FILE .

The screenshot below is an example of DE.UETR.CATALOG.LIST enquiry for the generated UETR which shows the transaction reference, payment message types and their respective delivery references.

end of accordion body

Scenario 2 - Generating a UETR in the MD Module

In this scenario, the user creates a contract in the

application for which a partial claim is registered.

The screenshot below shows a payment initiation claim of the MD deal generated for MT103 and MT202C messages.

As the MT202 COV belongs to the same transaction where the MT103 was also generated, the Delivery module re-uses the same UETR for both the message types.

The screenshot below is an example of DE.UETR.REF.FILE for the contract which shows the UETR delimited by delivery reference.

> **⚠️ Note:** If multiple messages are generated and a single UETR is used, then only one header record is delimited with UETR in DE.UETR.REF.FILE . Another partial claim is registered later for the same contact.

The screenshot below shows a payment initiation claim of the MD deal generated for MT103 and MT202C messages.

On the day of the claim, as the MT202 COV belongs to the same transaction where the MT103 was also generated, the Delivery module re-uses the same UETR (different from the initial UETR) for both the message types.

The screenshot below is an example of DE.UETR.REF.FILE for the MD contract showing the two UETRs (one UETR for every claim transaction) delimited with delivery reference.

> **⚠️ Note:** If multiple messages are generated and a single UETR is used, then only one header record is delimited with UETR in DE.UETR.REF.FILE .


#### 📋 Tasks

There are no Tasks available for the Unique End-to-End Transaction Reference feature.


#### 📊 Outputs

There are no Outputs available for the Unique End-to-End Transaction Reference feature.


> **Related Applications:** `DE.CARRIER`, `DE.O.HEADER`, `DE.UETR.CATALOG.LIST`, `DE.UETR.REF.FILE`, `FUNDS.TRANSFER`, `MD.DEAL`, `SWIFT.PARAMETER`

---


### 2.40  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Funds Transfer functionality is split in two different modules:*
> 
> **Applications:** `ARCHIVE`, `BENEFICIARY`, `FUNDS.TRANSFER`, `STANDING.ORDER`
> 
> **Key Fields:** *Account With Bank*, *Address*, *Arc Filename*, *Archive Data*, *Auto Process Limit*, *Autoroute Agrd*, *Back Value Max*, *Ben Acct No* ... +36 more
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- APIs
- Temenos Transact Services

The Funds Transfer functionality is split in two different modules:

- The Booking and Finance Adjustments (license code:FT) module covers the basic functionality to perform bookings and finance adjustments and direct postings. It is used by finance and operations teams to perform adjustments to accounts and profit and loss (limited to use of account transaction types only). Temenos Payments is the strategic solutions for customer payments and transfers.
- The Legacy Payment Processing using Funds Transfer (FTFULL) module provides the Temenos legacy payments functionality through Funds Transfer and supports cheques, international and local clearing payment types. Temenos customers upgrading from a release before 202009 already having the FT license code, automatically receive the FTFULL license code if they have not licensed LEAP. The functionality of the existing module is supported and maintained, but will not be enhanced to provide any new functions. Temenos Payments is Temenos standard payments solution and provides full payment capabilities including support for new payment schemes and standards (For example, CBPR+) and FTFULL will not be offered to new customers. Refer the Payments module for more information on Temenos Payments functionalities.

Temenos reiterates the recommendation to use Generic Accounting Interface (ACCCSM) as the solution to integrate Transact with third parties’ payment systems or other bank solutions involved in payment initiation, payment execution flows and any other interface which require cover check, funds reservations or bookings.

> **⚠️ Note:** The field length of the Name and Address fields in the STANDING.ORDER and BENEFICIARY applications is increased to support ISO20022. The FTFULL module is not modified to support ISO20022. While mapping the above details in FUNDS.TRANSFER , the system truncates them to the maximum length allowed by the FTFULL module.

The FUNDS.TRANSFER application handles internal transfer (under the license code FT) and external payment transfers (under the license code FTFULL). The FUNDS.TRANSFER application is integrated with the following modules:

- Accounting
- Central liability
- Delivery (Outgoing)
- Delivery (Incoming)
- Position management

Real-time updates are applied to:

- Balances
- Positions
- Cash flows
- Limits

Charges and commissions can be taken based on a variety of conditions or entered directly.


##### Configuring Funds Transfer

This section covers the configuration of Funds Transfer.

The FT.APPL.DEFAULT application contains application-level default values, which will be used while processing FUNDS.TRANSFER or STANDING.ORDER instructions. These values will be applicable irrespective of the transaction type, and the user must create one record for each company on the system.

The default values defined in this application can be summarised as follows:

- Limit Amounts:

- The Auto Process Limit field defines the amount in local currency, below which incoming transactions received direct from delivery can be processed automatically.
- The Less Charges Limit field defines the amount in local currency, below which instructions for outgoing payments should not be accepted to pay on a less charges basis. For example, when charges exceed the amount of the payment.
- The Min Sto Amt field defines a minimum transfer amount, below which balance maintenance instructions will not be processed for specified currency.

- Suspense Accounts: The Claim Charges Acct field contains the account to be debited when charges are claimed from the ordering bank.

- General Information: The Secondary Tlx Chg field indicates the FT.CHARGE.TYPE record to be used when a telex charge is to be applied for cover and free format telex messages. The Centralised Ft field defines whether or not the funds transfer function in the bank is centralised in one department.
- Commission or Charge on Error: When Funds Transfer applications are entered with commission or charge related fields, and any error is encountered while committing, all the commission or charges related fields are nullified and need to be entered once again or defaulted from FT.TXN.TYPE.CONDITION .

An OT transaction type is entered with commission and charges but without mandatory beneficiary details. So, the system clears the commission or charge field details after raising an Input Missing error and defaults the value again from the

. To retain the commission or charges entered after encountering an error, the

field can be specified as Retain in

or Null to clear the fields.

- MT103 Control: SWIFT message MT103+ which is processed straight through can be generated through FUNDS.TRANSFER by giving Mt103 Type as Mt103+ and filling Account With Bank , Receiver Bank , Receiver’s Correspondent (Tag 54) , Intermediary Institution (Tag 56) (Tag 52,54,55,56 & 57) with either a number of a customer who has a valid record in DE.ADDRESS for carrier as SWIFT, or a valid BIC code prefixed with 'SW-' along with the Ben Acct No field. When the above case is not satisfied, the system raises an error if the Mt103 Control is specified as System. When Mt103 Control is NULL, it generates an MT103 instead of an MT103+ with an override.
- Default Receiver Bank Charges: To default receiver charges for outgoing or incoming MT103 messages based on the CORR.BANK.CHARGES application in Funds Transfer, Def Corr Bank Chgs field can be set to Yes.
- Rounding: Rounding rule can be applied in FUNDS.TRANSFER application when The default in Temenos Transact is Natural rounding (NATURAL). Round Type field in FT.APPL.DEFAULT record can be used to setup new rounding rules. The rounding rule is set in the EB.ROUNDING.RULE application and is then entered into Round Type . A rounding rule entered in the FUNDS.TRANSFER transaction will override the rounding rule defined in FT.APPL.DEFAULT parameter application.

| Debit Value Date | Cut off time | Debit or Credit currency | Credit value date default |
|---|---|---|---|
| Debit value date prior or equal to date of receipt | Time of receipt prior or equal to cut off time | Debit currency equal to credit currency | Credit value date equal to date of receipt |
| As above | As above | Debit currency not equal to credit currency | Credit value date equal to date of receipt +1 working day |
| As above | Time of receipt after cut off time | Debit currency equal to credit currency | Credit value date equal to date of receipt +1 working day |
| As above | As above | Debit currency not equal to credit currency | Credit value date equal to date of receipt +2 working days |
| Debit value date after day of receipt | Time of receipt prior or equal to cut off time | Debit currency equal to credit currency | Credit value date equal to debit value date |
| As above | As above | Debit currency not equal to credit currency | Credit value date equal to debit value date +1 working day |
| As above | Time of receipt after cut off time | Debit currency equal to credit currency | Credit value date equal to debit value date +1 working day |
| As above | As above | Debit currency not equal credit currency | Credit value date equal to debit value date +2 working days |

The main objective of the AGENCY application is to keep the default delivery instructions for a customer or for a BIC address and the details of operation of the NOSTRO.ACCOUNT . It provides settlement information, which otherwise must be entered repeatedly on each transaction.

The key to the AGENCY application is the customer number or the BIC address prefixed by SW. The customer number should be a valid Temenos Transact customer number and should exist on the CUSTOMER application.

The SWIFT address is prefixed by 'SW-' and must contain 11 characters for a valid SWIFT ID (without prefix) and must be present on the DE.BIC application. The DE.BIC application is loaded from SWIFT and contains the BIC codes, addresses and other details.

The Autoroute Agrd field in the AGENCY record is used where there is an agreement in place with the correspondent bank (to which the Agency record corresponds to), regarding reimbursement on payments sent to other banks. This can be used to suppress cover payment messages where they are not required.

Read AGENCY table in the System Tables User Guide for more details.


##### Archival of Funds Transfer

The user can archive the matured or reversed transaction records in Funds Transfer (FT) using the Transact Standard or Data Lifecycle Management (DLM) archival.

The DL module must be installed for the user to initiate the archival service to archive the matured or reversed FT records in history to a Read-only (RO) database. Otherwise, the user moves the data records to the $ARC file using the Standard archival method.

The user defines Retention Period in ARCHIVE for the FUNDS.TRANSFER (FT) record. When the matured or reversed transaction data in FUNDS.TRANSFER crosses the retention period, it is selected for archival. Retention Period is calculated from the processing date of the FT transaction. A sample screenshot of ARCHIVE for the FUNDS.TRANSFER record is shown below.

When Retention Period ends and the user runs the archival service, the files mentioned in Arc Filename are archived.

> **⚠️ Note:** The user must set Archive Data as Y to archive the record. If the user sets it as N, the record is deleted instead of archiving, which results in loss of data.

Read Archiving for more details regarding Transact Standard archival process. Read Data Life Cycle Management for more details regarding DLM Archiving process.


##### Illustrating Model Parameters

This section covers the high-level parametrization, which describes the design, setup, charges, commissions, inward and outward delivery interfaces.

| S.No. | Parameters | Description |
|---|---|---|
| 1. | FT.APPL.DEFAULT | This application allows the user to define application-level default values, which is used when processing FUNDS.TRANSFER or STANDING.ORDER instructions. These values will be applicable irrespective of the transaction type, and the user must create one record for each COMPANY (that is, in case of multi-company setup) on the system. |
| 2. | FT.TXN.TYPE.CONDITION | This application allows the user to define the default conditions for each transaction type, which can be processed by the FUNDS.TRANSFER and STANDING.ORDER applications. User can define Transaction Code Credit , Transaction Code Debit , Comm Types , Charge Types , Forw Value Max and Back Value Max for each transaction type. |
| 3. | FT.CHARGE.TYPE | This application allows the user to define the conditions related to various types of standard flat charges used by Temenos Transact . In addition, charge types can be linked to allow different charge structures, tax codes and so on to be applied depending on the residence of the ordering customer. |
| 4. | FT.COMMISSION.TYPE | This application allows the user to define the conditions related to all types of commission used in applications. Each commission type can be defined as a Flat Amount or variable amount, proportionate to the amount transferred. In the latter case, different percentages can be defined for different Bands or Levels of transfer amounts. Minimum and maximum commissions can be specified for each Band or Level together with overall minimum or maximum commission charges. |
| 5. | CORR.BANK.CHARGES | This application allows the user to define correspondent bank charges or commission, which will default in FT when Def Corr Bank Chgs field in FT.APPL.DEFAULT is set to Yes. |
| 6. | FT.GEN.CONDITION | This application allows the user to identify a specific group of customers, using a user-defined Funds Transfer General Condition number. , This will then be cross-related to the Group Condition table to define Funds Transfers conditions applicable to that group. The FT General Condition record must exist before any associated group condition is specified. The key to this table is also the key to the associated FT Group Condition record. |
| 7. | FT.GROUP.CONDITION | This application allows the user to define special conditions applicable to specific groups of customers or individual customers which overrides the normal conditions, used by the Funds Transfer application. A customer subjected to these conditions must first meet the selection criteria defined in FT.GEN.CONDITION and accessed using an identical key. |
| 8. | EB.DUPLICATE.TYPE | This application allows the user to define selected fields to check for any duplicate contracts for the given application. This application also allows the user to define duplicate check criteria for linked applications, which can be defined in the Linked Application field. It allows the user to select the following: Application for which the duplicate check criteria is defined. The fields from that application which will be part of the duplicate check. The number of purge days, which will ensure that the duplicate criteria check will be applied only for contracts raised in the past n days (number of days defined in the Purge Days field in this application). |


##### Illustrating Model Products

The following Model Bank products are released as part of the FTFULL module:

| S.No. | Product Name | Product Attributes |
|---|---|---|
| 1. | OC- Outward by Cheque | Refers to the issuance (by the bank) of a Manager Cheque or a Bank Cheque in local currency in favor of the beneficiary who does not maintain an account with the bank. |
| 2. | OD – Outward By Draft | Refers to the issuance (by the bank) of a Bank Draft (usually in foreign currency), in favor of the beneficiary who does not maintain an account with the bank. |
| 3. | OT –Outward by Telex | Refers to the issuance (by the bank) of a payment via Swift or Telex. The instructions are usually sent to the correspondent bank for processing. This transaction type will produce both pay and cover cables automatically where required. |
| 4. | OB – Outward by bankers payment | Refers to the issuance (by the bank) of a banker's payment in local currency. This method of payment is used extensively in the UK to perform local currency payment. |
| 5. | BC – Outward by BACS | This transaction type is only applicable for Sterling and within the UK and refers to outward transfers by BACS (Bankers Automatic Clearing System). Currently BACS payments are not generated by the system. If it is required, it must be added as a local enhancement. Other host countries may have similar systems to which this may be adapted. |
| 6. | IC – Inward payment by cheque or draft | Refers to the receipt of a cheque or a draft by the bank, to be credited to a customer account. |
| 7. | IT – Inward by Telex | Refers to the receipt of a Swift or Telex payment by bank in favor of bank's customers, where the proceeds have to be credited to an account in bank’s books. |
| 8. | IB – Inward by banker's payment | Refers to the receipt (by the bank) of a banker's payment in favor of an account in our books (UK only). |


> **Related Applications:** `ARCHIVE`, `BENEFICIARY`, `FUNDS.TRANSFER`, `STANDING.ORDER`

---


### 2.41  Treasury Settlement


> **📇 Quick Reference Card**
> 
> **Key Fields:** *Application*, *Autoroute Bank*, *BROKER*, *Bic Code*, *Effective Date*, *GB Notes*, *Last Eff Change*, *Nostro Acct No* ... +3 more
> 
> **Sections:** 🔧 Working With


#### 🔧 Working With

This topic explains the workflow of the treasury and settlement related reference applications in Temenos Transact .


##### Nostro Account

The NOSTRO.ACCOUNT application defines the nostro account records by currency and identifies, which account is the default nostro for each function of each application within the specified currency.

FT OT transactions use account 20753, FX uses 23752 and all others transactions use account 20656.

The various NOSTRO.ACCOUNT records can be recorded for each application. The definition of NOSTRO.ACCOUNT records within this application eliminates the need to enter the same details each time for each transaction processed by various applications of Temenos Transact .

> **⚠️ Note:** FOREX allows fast input of alternate nostro account values by entering A, B and C and so on. These relate directly to the first, second, third and so on, values entered.

- Future Dated Nostro Account Details Banks change their Nostro correspondents periodically. They are notified in advance when these changes happen and it is possible to capture these changes within the system, allowing the system to provide the correct nostro account details based on a settlement date. Once the effective date of a record is reached, the system makes this the current record and writes previous records to history during the online phase of COB. A record is entered into the system with the ID as effective date added as a suffix to the record (as shown in the below screenshot). The Effective Date field is used to hold a list of effective dated records within the system on the current record. GB Notes field is used to add comments. The last date and time, an effective date record updated is held in Last Eff Change field. The Effective Date and GB Notes fields are updated in the current record (as shown in the below screenshot), when effective and future dated records are created:


##### Agency

The AGENCY application contains the settlement details for major customers and all banks irrespective of whether there is any business connection. The details include any arrangements, account relationships and where possible, the agent’s correspondent bankers for specific currencies. This information is entered centrally to supply automatic routing instructions for remittances or cover to all banks and customers with whom the bank has numerous dealings. This eliminates the need to re-enter the details at transaction level. It allows full advantage to be taken of electronic delivery facilities by providing automatically, the settlement agents for remittances or cover involved in outward payments.

The absence of agent's correspondent banker’s information in this application forces the user to enter these details each time at the time of transaction. Any nostro account defined in this application is for information only and is not used as a default nostro by the transaction processing, which always uses the details from the NOSTRO.ACCOUNT application.

Record details can be setup on this application using two different ID formats, either the customer number or the Bic Code field prefixed with SW- in DE.BIC application.

- Customer Number The basic details of these banks and major customers must first be defined in the CUSTOMER application before the creation of the AGENCY details is allowed. Having created a CUSTOMER record, which is a bank, it is advisable to create an AGENCY record with the same ID and all available auto routing details.
- Bic Code The AGENCY records can be created for the BIC code with all the auto routing details. The input of this record is similar to that of the record created by using the customer number ID. The exceptions being that the input are not allowed for Nostro Acct No , Our Ext Acc No and Their Acct No fields. In the AGENCY application, the BIC codes are pre-fixed by ‘SW-’ and should have 14 characters (including ‘SW-’). The Bic Code should be a valid SWIFT code and can exist in the DE.BIC application. The DE.BIC application is loaded from the BIC address directory file and this is supplied by SWIFT. Refer the DE.BIC section, for more details. If the Validate Bic field in the DE.BIC.PARAMETER application must be set to YES, then upon inputting a BIC code (an SW- record) Temenos Transact validates the ID against the DE.BIC records. If the field is set to NO, then AGENCY accepts any SW- codes as long as they are in the correct format.
- Multiple Agency Records for Settlement

> **⚠️ Note:** There is an informal linkage between records, which comes into effect when the system is working out the full settlement path for a customer.

The auto routing bank ( Autoroute Bank field) is defined for the counterparty in the AGENCY application. The auto routing bank must exist in the AGENCY application and the input can be in BIC or customer number. If the Application field is FX or FT, the Autoroute Bank field is defined as a BIC.

The below screenshot shows SWIFT BIC codes used in AGENCY for the Autoroute Bank field.

The AGENCY for a counterparty has the Autoroute Bank field value as the correspondent bank BIC for a specific currency. If the correspondent bank has the payment routing arrangement with another intermediary bank for the currency, then the BIC or customer number of the intermediary bank can be set as correspondent bank BIC in Autoroute Bank.

An example of auto routing arrangement is shown in the following screenshots:

- The counterparty record (100129) in AGENCY has Autoroute Bank as SW-BFWTES01 (correspondent bank BIC).
- The correspondent bank BIC (SW-BFWTES01) has the routing arrangement through the intermediary bank (Autoroute Bank) as SW-BFWTES02.
- The Intermediary bank has the Autoroute Bank defined as the same BIC, indicating that there is no further routing.

Future Dated Settlement Instructions

Temenos Transact can capture future dated standard settlement instructions, if required. This allows the bank to update the correspondent banking details in advance of the effective date, allowing the system to provide the correct settlement instructions based on a settlement date.

Once the effective date of a record is reached, the system makes this the current record and writes the previous records to HISTORY table during the online phase of COB.

A record is entered into the system with the effective date added as a suffix to the record’s ID. For example, 140048-20091224 (as shown below) or SW-CITIUS33-20091224’.

The future dated record for customer is shown in the below screenshot.

The future dated record for BIC is shown in the below screenshot.

The Effective Date field is used to hold a list of effective dated records within the system on the current record. The GB Notes field is used to add comments. The last date and time, an effective dated record was updated, is held in Last Eff Change field in the current record.

The below screenshots demonstrate the Effective Date and GB Notes are updated in the current record, when effective and future dated records are created:

The current record with the Effective Date and GB Notes fields are shown in the below screenshot.

The future dated record with the Effective Date and GB Notes fields are shown in the below screenshot.


##### Broker

The BROKER application is used to define the banks' authorised brokers. The following screenshot shows the field details in BROKER application:

- Payment Instructions

The first section of the BROKER application is used to specify the broker's payment instructions as follows:

- Currencies in which the broker accepts payment
- The default transaction code for brokerage entries
- The account to which the brokerage funds are to be transferred.

This account may be defined in two ways:

1. The default specifies an internal account number, which consists of: The payment currency The category specified in the ACCOUNT.CLASS record The BROKER and the sub-division code specified in the BROKER record. The actual internal account number is not shown on the record.
2. The second method of account definition is the specification of a Temenos Transact account, which must be a customer account that belongs to the BROKER . One account may be defined for each payment currency. Calculation Parameters

The second section of BROKER application is used to determine the different brokerage rates applicable to specific deal types. During the deal input stages for the valid applications, if a broker code is entered, then the details of this application are obtained to default and the brokerage amount for the deal. Certain aspects of the deal are matched to the parameters on this application to define a deal type. Each deal type is defined using the following parameters:

- System ID
- Category
- Time

The System ID is used to define the application. At present, valid products are Money Market, Loans and Deposits, Letter of Credit, Drawings, Fiduciaries and Forward Rate Agreements. Category is used to match the product category of the deal. Time is defined as the number of days from the start date to the maturity date. Once a match has been found for the deal type, the currency of the deal is matched with a list of currencies on the BROKER record. Then, whether the customer of the deal is a bank or a non-bank, a rate or FT.CHARGE.TYPE or FT.COMMISSION.TYPE is returned on which the brokerage calculation is based.


##### Position Type

The FX.POS.TYPE application is used to split the position and accounting of the bank into logical divisions. In particular, the usage of this application is mandatory when using a GAAP or IFRS financial reporting. Although prefixed by FX, this application is commonly used in Temenos Transact and is referred to by CATEGORY, ACCOUNT and many accounting or position parameter files.

When used for GAAP reporting, it is recommended that the two digit ID is set to the same ID used by the country (that is, IN for India, GB for the UK, CH for Switzerland and so on). The TR record is the original and default record used by Temenos Transact must be present. The IF record is used for IFRS reporting and must be present, if IFRS reporting is required.

In normal usage, the ID of the application is used but for contingent and self-balancing, an extended ID identifier is needed.

> **⚠️ Note:** It is recommended that the following style of values is followed:

- For P/L add the PL prefix to the position type. For example, PLIF.
- For Contingent P/L add CP prefix to the position type. For example, CPIF.
- For self-balancing P/L add CB prefix to the position type. For example, CBIF.

Otherwise, by default it is achieved, by taking the first character of the ID and adding 'P' for contingents and 'B' for self-balancing. Alternatively, the user can define their own values of up to four digits for each of these.

> **⚠️ Note:** There is a system control RE.PL.PREFIXES table, which stores a cross-reference of all the prefixes that prevents the duplication of any user or system defined values.


##### Deal Method

The FX.DEAL.METHOD application is used by the main dealing or lending applications to record how the deal was booked. It is used mainly for advices and reports, and is entered in the BROKER field on the relevant applications.

---


---


## Chapter 3: Customer_Output - DEMXTR


Customer_Output - DEMXTR module of Temenos Transact


### Features in Customer_Output - DEMXTR


| # | Feature | Sections |
|---|---------|----------|
| 3.1 | SwiftNet Interact MX Services | Intro, Confi |
| 3.2 | Generating Message Flow | Intro, Confi, Worki, Tasks, Outpu |
| 3.3 | Misc | Intro |
| 3.4 | Transform messages to Payment | Intro, Confi, Worki, Tasks, Outpu |
| 3.5 | Translating Messages | Intro, Confi, Worki, Tasks, Outpu |


### 3.1  SwiftNet Interact MX Services


> **📇 Quick Reference Card**
> 
> **Purpose:** *Various High Value Payment Systems (HVPS) referred also as Real Time Gross Settlement systems have adopted or are in progress of adopting ISO20022 messaging standards. The majority of these HVPS (SIC, CHAPS, T2, and so on) use the SWIFTNet as a network provider.*
> 
> **Applications:** `ASCII.VAL.TABLE`, `DE.ALT.CHARS`, `DE.BUSINESS.SERVICE.RULES`, `DE.CARRIER`, `DE.DISTINGUISH.NAME.RULES`, `DE.DLN.REQUIREMENTS`, `DE.FORMAT.SWIFT`, `DE.I.HEADER` ... +17 more
> 
> **Key Fields:** *Ack Required*, *AckNackTemenosFormatXsd*, *Alter Char Code*, *App Context Field*, *App Context Field.*, *App Context Value*, *Business Application*, *Business Service* ... +38 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration


#### 📖 Introduction

Various High Value Payment Systems (HVPS) referred also as Real Time Gross Settlement systems have adopted or are in progress of adopting ISO20022 messaging standards. The majority of these HVPS (SIC, CHAPS, T2, and so on) use the SWIFTNet as a network provider.

Moreover SWIFT is also migrating to the ISO20022 cross border payments. The main difference is that SWIFT supports a co-existence period, allowing its members to make the full switch by the end of 2025.

Interact is a SWIFTNet messaging service that is used to send and receive financial messages in XML format. The majority of the new messaging solutions defined by the HVPS owners are using SWIFTNet Interact services. For the ISO20022 cross border payments, SWIFT also decided to use a SWIFTNet Interact based service.

A key element of the new services is the presence of the Business Application Header (BAH) as part of the exchanged message. The use of BAH, the version and the usage guidelines are decided by each payment scheme owner or administrator.

Temenos Delivery module offers Temenos Business modules a framework to exchange the ISO20022 messages with a SWIFT messaging interface, supporting the main elements of the SWIFTNet Interact message structure and providing the following capabilities

- Define the distinguish name rules for the bank itself as well as for its counterparties.
- Define the rules for the business service used by various HVPS and CBPR+.
- Define Delivery Message Headers, indicating the schema, its version and the header elements, and associated them with a channel/service (Delivery Carrier).
- Apply a transformation to the business payload, if a transformation rule is indicated.
- Generate SAA technical header (XMLv2).
- Generate BAH specific to each service.
- Process Network acknowledgements (Ack/Nack).
- Process Delivery Notifications (positive, negative andoverdue warning).
- Calculate and attach the local authentication code (LAU), if enabled.
- Provide option to add locally a digital signature.
- Store the final outward message.
- Determine the channel for the inward messages based on the service name specified in the technical header.
- Validate the local authentication, if enabled.
- Validate the header details, based on the supplied schema.
- Route the inward messages to the Business Applications.
- Store the original inward message.

> **⚠️ Note:** The Delivery module generates the outward Interact ISO20022 messages in XMLv2 fomat. The Delivery module processes the inward Interact ISO20022 messages, Ack/Nack and Delivery notifications received in XMLV2 envelope.

The Temenos business modules like TPH and Account Statement can use the Delivery capabilities to send or receive Interact messages to SWIFT Alliance.

The Temenos SWIFT Interact Connector acts as an interface between the Transact Delivery Transformation Layer queues and the SWIFT Alliance messaging interface.

The following diagrams provide an overview on how various modules are linked to Delivery:


##### SWIFTNet Interact

SWIFT provides multiple messaging services like Interact, FIN, FileAct, etc. The Interact messaging service can be deployed in various modes :

- Real Time - Where both parties must be active.
- Store and Forward - Where the message sent by the sender is stored centrally by SWIFT until the receiver connects.
- Query and Answer - Where the sender sends the request in real time, and either receives the response from receiver or an error.

A SWIFTNet service uses a SWIFT messaging service, configured in the context of specific messaging solution. The messaging solution has a service administrator which decides the rules and policies around that solution.

> **⚠️ Note:** Delivery currently supports SWIFT Interact store and forward services – for example, SWIFTNet Funds, FINPlus service used by CBPR+, ESMIG T2 used by T2 RTGS consolidation, etc.


##### Interact Message Structure

The SWIFTNet Interact message structure is presented in the screenshot below:

- Request Header - It is used by the SWIFT Messaging Interface/ SWIFTNet network to determine the service to which the message must be sent, to distinguish name of the sender institution (also referred as Requestor), to distinguish name of the receiver institution ( also referred as Responder), the message type, etc.
- Request Payload - It is used by the Receiver Institution. The BAH is optional, it’s presence is the decision of the service owner/administrator. The BAH can be used by the Receiver to decide on the route flow for the respective message. The business document provides the required details of the respective transaction.
- Security - It allows the bank to include security features to the exchanged messages. For example, to include a local authentication code to ensure the message is not tampered between the Source Application and the Messaging Interface.

Delivery supports XMLv2 message format (also known as DataPDU) which is used by the SWIFT Alliance interfaces to exchange Interact messages with Application Systems like Transact.


##### Interact Terminology

Service Name - It is the name communicated by the service administrator to its members representing a service defined for a specific business purpose. It usually follows this pattern: “service administrator”.”service identifier” ”operational environment”

swift.finplus!p

Where,

- swift – Indicates the name of the service administrator
- FINPlufinplus service -– Indicates the name of the service communicated to the users
- .!p– Indicates the test and training environment,

If the “operational environment” is blank, this denotes the live environment.

Distinguish name - It is the logical name through which a user or system is identified in a domain. In the SWIFT world, the financial institutions are identified by their BICs, the Distinguish Names help to identify entities at a more specific level.

For example, the messages must be addressed to a specific entity of a financial institution, like, functional units and geographical locations.

T2 is the European real-time gross settlement (RTGS) system called which will be launched in Nov 2022. The name of the SWIFT Interact store and forward service used by T2 is esmig.t2.iast. The BIC assigned to T2 is TRGTXEPM but different distinguish names identify the RTGS (cn=rtgs,o=trgtxepm,o=swift) and CLM (cn=clm,o=trgtxepm,o=swift) components of the T2 system. The T2 ESMIG layer routes the messages received by T2 to the RTGS or CLM components based on the responder distinguish name indicated in the request.

The distinguish name definition follows this rule:

Level 4 (Common Name), Level 3 (Organisation Unit), Level 2(Organisation), Level 1 (Registration Authority)

Where,

- Level 3 and Level 4 are optional,
- Level 2 and Level 1 are mandatory.

cn=payments, ou=ho, o=bankbebb, o=swift denotes the traffic is addressed to institution BIC BANKBEBB – and more specifically to its payments entity/system, part of organisation unit ho.

Each institution which is using SWIFT network must register their Distinguish Names with SWIFT.

- Requestor Distinguish Name represents the distinguish name of the sending institution.
- Responder Distinguish Name represents the distinguish name of the receiving institution to which the message is addressed.
- Request Type represents the name of the message ISO message, for example, pacs.008.001.08.

SenderReference – Uniquely identifies the message being sent out

UserReference – The reference allocated to the message which will be also present in the responses


##### Business Application Header

The purpose of the Business Application Header(BAH) is to provide a consistent way to supply the basic details of the business message, regardless of the network and interfaces through the message is processed. The BAH has been designed by the ISO20022 community, its definition (head.001.01.0x) can be combined with any other ISO20022 message to form the business message.

The owner of a service decides the use of the BAH as part of the exchanged messages, its versions (for example, Target2 uses head.001.001.01, CBPR and CHAPS uses head.001.001.02) and rules (the mandatory/optional elements, their values, which elements take precedence – the elements in the BAH or the elements in the body of the message).


###### BAH Elements

- From element - Identifies the entity which has created the business message and it could be different from the sending address (Requestor Distinguish Name) in the technical header. For example in case of T2, the From element identifies the T2 member who sent the Business message but the Requestor Distinguish Name identifies the T2 ESMIG DN (T2 is implemented using a SWIFT V Copy architecture - messages are sent by the Instructing members to the central system which validates and then forwards the messages to the Instructed members).
- To element - Identifies the entity which has been indicated by the sender of the Business Message as the recipient of the message. Could be different from the receiving address (Responder Distinguish Name) in the technical header, for example, in the messages sent to T2 the Responder Distinguish Name is the T2 DN but the To Address identifies the Instructed Agent.
- Business Message Identifier - Indicates a reference allocated to the business message by the entity which is initiated the message to identify the message.
- Message Definition Identifier - Identifies the type of the message, for example, camt.053.001.08.
- Business Service - Identifies the service agreed between the entities exchanging the message.
- Market Practice - Identifies the market practice to which the message is aligned with.
- Creation Date - Indicates the date when the business message has been created.
- Possible Duplicate - Indicates if the exchanged message is a possible duplicate.

The example below shows an Business Application Header for a CBPR+ pacs.008 message:


##### SWIFT Multi-format MT MX Messages

The FINPlus service used by CBRP+ allows banks to exchange payment and payment-related MX messages. Until November 2025, banks will have the option to choose between MT and MX formats.

For CBPR+, SWIFT provides a translation from MT to MX and vice versa either at the Transaction Management Platform (for MT103/ MT202 COV, MT205 COV and pacs.002 reject, pacs.004, pacs.008, pacs.009 and COV messages) or as part of the FINPlus service (from CAMT to MT).

SWIFT allows banks to decide if they want to receive MT or MX messages for each of their BIC8 or BIC11. The bank can refine this decision based on the message type and/or currency.

Until November 2025, the SWIFT MX messages sent by financial institutions that have already adopted ISO20022 standards will be translated by SWIFT to MT before being sent to receiving institutions that are still using MT formats. In such cases, SWIFT sends a multi-format message to the receiving institutions representing the original ISO20022 message, which embeds the MT message as a comment.

The following is a (edited) sample of a multi-format MT MX message.

The receiving institutions can configure their SWIFT interface to send either the original message received from SWIFT or just the translated MT to the business application.

The following scenarios are possible from November 2022:

- Bank A is subscribed to the platform as an MT recipient and bank B as MX: Bank A sends to bank B MT and bank B receives MX translated from MT.
- Bank A is subscribed to the platform as an MT recipient and bank B as MT: Banks exchange MTs.
- Bank A is subscribed to the platform as an MX recipient and bank B as MX: Banks exchange MXs.
- Bank A is subscribed to the platform as an MX recipient and bank B as MT: Bank B receives MT translated from MX (as a multi-format message).

The Delivery Transformation Layer can receive multi-format messages and, depending on the parameterisation set up by the bank, either route the MX message (the default option) or the MT message to Temenos Payments Hub (TPH) or the Delivery module. In both cases, the original MX message is stored in the Delivery module.


##### Support for Allowed Character Set

SWIFT defined the basic character set for the CBPR+ messages and indicated that an extended character set is permitted for few ISO20022 elements. Real Time Gross Settlement systems like T2, CHAPS have also defined their allowed character sets.

Delivery allows the bank to define the supported characters for the XMLISO based channels.

For outward business messages formatted by Delivery, the character set rules are validated during the XMLISO formatting process. If there are any rules configured for the delivery carrier and the message type, Delivery identifies the message elements for which conversion rules are defined, applies the conversion rules and validates the resulted string with the allowed character set. The message is then emitted to the Delivery Transformation Layer.

Temenos business modules that generate the business messages directly (for example, TPH) use the Delivery configuration and invoke its conversion capabilities for each of the defined elements. Once the business payload is formatted the TPH emits the message to Delivery Transformation layer.

The Delivery Transformation Layer applies the payload transformation, if indicated in the message, adds the header details, appends the LAU, if configured and emits the final message to the integration queue. Please read the Message Data Handed off to Delivery for more details.

The inward messages are not validated with the allowed character set because SWIFT or the central RTGS system rejects the messages that do not comply with the allowed character set.


##### Support for Currency Transformation in Inward and Outward Messages

The Delivery module allows the bank to configure currency transformation between offshore and onshore bank currencies for both inward and outward messages.

Consider the onshore yuan as an illustrative example, identified by the ISO currency code, CNY. The onshore yuan is exclusively traded within Mainland China under stringent government control. In contrast, the offshore yuan, known as CNH operates beyond the confines of Mainland China. Notably, CNH does not have an official ISO 4217 currency code, reflecting its distinct status as an offshore currency.

The Delivery module facilitates the seamless exchange of SWIFT MX messages and helps the financial institutions the capability to transform the offshore to onshore currency and vice versa.

This functionality applies to the messages which are transformed through the delivery transformation layer. Read CNY to CNH currency conversion for more information on messages transformed by Temenos Payments .


#### ⚙️ Configuration

This section describes the configuration of the Delivery framework to process MX messages through SWIFTNet Interact services.


##### Delivery Message

The DE.MESSAGE application stores the definition of the message. The DE.MESSAGE records with the definition of ISO20022 messages are released by core - the Id of the DE.MESSAGE is given by the first 2 parts of the ISO message, without the ‘.’. This is optionally followed by ‘.’ and then by the message subtype, if any.

PACS009 is released for the financial institution’s credit transfers message and the PACS009.COV is released for financial institution’s credit transfer cover message.

If the message is not handed off to Delivery, the definition stored in DE.MESSAGE is very simple, indicating the Msg Name Id .

However, if the message is handed off and emitted through Delivery, it stores the definition of the tags.

The Message Name Id field in DE.MESSAGE stores the full message name of the default variant for the respective message, for example, pacs.008.001.08.

The preference for the Message Name Id can be also specified in DE.PRODUCT . This can be used to capture the preference for a specific variant for a given customer/account, if this differs from the default variant.

The preference for the Message Name Id is overridden by the setup in DE.CARRIER , where the bank can indicate the version which is used for a given message type. The DE.CARRIER can represent the channel to an RTGS system, for example, T2 ( Target2, the European settlement system) or another service in which the rules are enforced by a service administrator, in which case the variant is imposed by the rules of the administrator and not be the preference of a given participant.


##### Delivery Message Header

The DE.MESSAGE.HEADER application allows the bank to define technical and business headers which can be then added to the ISO20022 messages processed through Delivery (XMLISO processing). The following characteristics of the header can be specified in this application:

- The schema identifier - specifies the namespace of the header.

urn:iso:std:iso:20022:tech:xsd:head.001.001.02

- The type of the header - technical or business.
- Version of the header - 2.0.8.
- The list of the generic and business metadata that is part of the header.
- The format of the Create Date Time - Zulu ( also known as UTC format) or Local time with UTC offset.

The list of the metadata covers the header elements which are supported by Temenos and are required either by the SWIFT Alliance technical header (XMLv2) for Interact messages or by the ISO20022 Business Application Header.

The Business Metadata are supplied by the business application, the Generic Metadata are determined by Delivery but can be imposed by the business applications.

The following Business Metadata are currently supported by Delivery:

- Transaction Reference
- From Address
- To Address
- Instruction Priority

Currently Delivery supports the following generic metadata:

- Format
- Business Service
- Message Name Id
- SenderReference
- MemberId
- CreateDateTime
- DLNOverdueTime
- DLNRequested
- RequestorName
- ResponderName
- ServiceName

> **⚠️ Note:** The system evaluates and determines the metadata in the order in which they are defined; this is important as some of the metadata are used to determine the others, for example, the Business Service Rules depend on the Message Name Id. Implementations can still define and use headers for local channels as long as the messages are processed through Delivery using XMLISO formatting module.

The screenshot below shows the setup of the XMLv2 technical header

The screenshot below shows the setup of the BAH applicable to CBPR+ messages:

The screenshot below shows the setup of the BAH applicable to T2 messages. It can be noticed that a different schema and a different version is indicated in the setup for the T2 BAH comparing to the CBPR BAH and the metadata are slightly different as T2 doesn’t allow the Business Service as part of the BAH.

The Lcl Hdr Element Api field allows the bank to define a local routine which can handle local headers. This routine receives the following arguments:

- The Delivery Outward Header record linked with the current message.
- The Delivery Message Header record to which the routine is attached.
- The list of the Generic Metadata calculated by core, as name:value pairs, delimited by @SM.
- The list of the Business Metadata calculated by core (for the messages handed off via Delivery), as name:value pairs, delimited by @SM.

The output of this routine is:

- The list of the Generic Metadata updated by the local logic – which can update the values calculated for the core metadata and supplied as input argument but can also add local metadata and their values, using the same delimiter.
- Business meta data cannot be updated by the local routine.


##### Delivery Carrier

A dedicated Delivery Carrier has to be setup for each SWIFT Interact service/channel. The headers applicable to each service are defined using the DE.MESSAGE.HEADER and attached to the DE.CARRIER , the Formatting Module has to be set to XMLISO, Carrier Module as GENERIC.

The CBPRPLUS Delivery Carrier is released as part of the Delivery module. Delivery carriers for various RTGS systems are released by the verticals as part of their solution (TGT for T(arget)2, STG as part of CHAPS, etc.) For local channels, the implementation must setup the Delivery Carrier locally. Few other attributes must be set in the Delivery Carrier:

- The name of the SWIFTNet service through which the messages are processed, for example, swift.finplus in the CBPRPLUS Delivery Carrier.
- The format is MX.

If the Unique End To End Transaction Reference (UETR) must be generated/retrieved for certain messages types processed through the respective Delivery Carrier, the name of the respective message types has to be configured in the UETR Message field. Masking can be used, for example, pacs.008 means for any pacs.008 message.

If the service imposes rules regarding the variant(s) for the message types that can be exchanged, the specific variant(s) must be defined in the Delivery Carrier in the Message Name Id field associated with the respective Delivery Message .

If the Requestor DN (the Distinguish Name assigned to the bank) is the same for all messages sent through that service, this can be defined in the Overriding Requestor DN in DE.CARRIER . This overrides the setup in the DE.DISTINGUISH.NAME.RULES application. For performance reasons, it is recommended to use this setup where possible, rather than defining this in the DE.DISTINGUISH.NAME.RULES application.

If the Responder DN (the Distinguish Name assigned to the receiver) is the same for all messages sent through that service, this can be defined in the Overriding Responder DN in DE.CARRIER . For example, if an RTGS like T2 RTGS follows the SWIFT V copy architecture ( all messages are sent to the RTGS which forwards them to the destination, after the RTGS validations are passed) then all messages must be sent to the distinguish name assigned to the RTGS as the Responder DN. This overrides the setup in the DE.DISTINGUISH.NAME.RULES application. For performance reasons, it is recommended to use this setup where possible, rather than defining this in the DE.DISTINGUISH.NAME.RULES application.

Member Id can be used to capture the Member Id of the bank – this is currently not used by core but can be used by implementations..

The Format of the message must be set to MX.

The following screenshot shows the setup for the CBRPLUS DE.CARRIER which is used to process CBPR+ messages. The XMLV2 technical header as well as the CBPR+ Business Application Header are linked to this. No Overriding Responder DN is indicated in the Delivery Carrier. The Responder DN varies and is a direct translation of the Receiver BIC – a rule must be set for CBPRPLUS domain in the DE.DISTINGUISH.NAME.RULES application.

The screenshots below show the setup for TGT DE.CARRIER which is used to process T2 messages. The XMLV2 technical header as well as the T2 Business Application Header (BAH) are linked to the TGT carrier. The Overriding Responder DN indicates the distinguished name ( Responder DN) assigned to the RTGS system (ESMIG), as all messages are sent directly to ESMIG and not to the instructed banks (identified by the To Address in the BAH).

The offshore companies maintain the Nostro/Vostro accounts in offshore currency (CNH), hence the outward messages require transformation of the Chinese currency (that is, CNH to CNY) into the ISO currency to avoid the messages being rejected by SWIFT or local RTGS. The currency transformation (CNH to CNY) must be enabled for services/channels that send outward messages in offshore currency (CNH).

The Replace Currency field in the DE.CARRIER application configures the currency transformation for outward MX messages. This configuration explicitly instructs the delivery transformation layer to change the currency in the ‘From currency’ to the ‘To currency’ in the outward MX messages processed through the respective Delivery Carrier and this configuration is applicable only for the carriers that have Format Module set as XMLISO. The format for this configuration is ‘FromCurrency/ToCurrency’.

The following screenshots provide the configuration for the outward SWIFT MX Messages.


##### Delivery Interface

The DE.INTERFACE application stores the name of the Integration Queue where the final outward message is released. This is linked to the DE.CARRIER defined for the respective channel.

The outward Interact messages are picked from this queue by the Temenos SWIFT Connector and is sent to SWIFT Alliance queue/folder. Alternatively, the bank can use their own adapters to consume the messages from this queue.

The Ack Required field indicates if a SWIFT Ack/Nack is expected for the messages sent through this channel/service. Read Handle responses section in the Working with MX Interact messaging for more information.


##### Delivery Product

The bank can customise the preference for a certain customer or account by indicating the Message Name Id and the Transformation Rule that must be applied to the payload before sending the message out.


##### Distinguish Name Rules

The Requestor (Sender) and Responder (Receiver) Distinguish Name are mandatory elements for the Interact header.

The DE.DISTINGUISH.NAME.RULES application allows the bank to capture the rules based on which Delivery can determine the distinguish name for the bank itself as well as for the receiving counterparty. The following attributes are mandatory in the DE.DISTINGUISH.NAME.RULES :

- Scope - Specifies if the rule applies is for the Requestor DN or for the Responder DN.
- Domain - Indicates the Delivery Carrier for which the rule is used.
- Status - Determines if the rule is Active, Expired or Cancelled.
- Distinguish Name or a Distinguish Name Rule - The user can specify either of them. This is the value which is assigned to the Responder/Requestor Name metadata if all other conditions are met. Two different Distinguish Name rules are supported by core: DefaultDnLevel3 - Determines the DN based on the supplied (To/From)Address, assuming the To/From Address is a BIC, using the following logic: ou=last 3 chars from BIC11 or xxx if a BIC8 or 9 is supplied, converted to smalls, o=BIC8(converted to small cases), o=swift DefaultDnLevel2 - Determines the DN based on the supplied (To/From)Address, assuming the To/From Address is a BIC, using the following logic: o=BIC8(converted to small cases), o=swift
- Start Date and End Date - Specify if a certain rule becomes effective at a future date (Start Date) or it stops being effective at a certain date (End Date).
- Customer, Address, Message Type and Currency - Define rules specific to a customer, address, message type, currency. If not specified, it means the rules apply to any customer, address, message type, currency.
- Message Type - Identifies a specific DE.MESSAGE .
- App Context Field and App Context Field - Define rules based on the content supplied by the Business Application. ORIGINATING.SOURCE and SUB.TYPE.INDICATOR are currently supported for App Context Field .

The above screenshot shows the rule released as part of the Model Bank setup – for all CBPRPLUS messages, irrespective of the receiver’s customer number, address, message type, ccy, or other values supplied by the Business Applications generating the message, the Responder DN is decided based on the To Address supplied in the message (and stored in the DE.O.HEADER created for the respective outward message), using the DefaultDNLevel3 rule.

- If the To address indicates the BNABFRPP BIC, then the Requestor DN is set to ou=xxx,o=bnabfrpp,o=swift.
- If the To Address indicates BNABFRPPABC, then the Requestor DN is set to ou=abc,o=bnabfrpp,o=swift.

The following screenshot shows how the Responder DN is defined for all messages sent through FUNDS Delivery Carrier to the BBHCUS3I address, irrespective of the message type, currency or other values supplied by the Business Application.


##### Business Service Rules

The Business Service is an optional attribute of the ISO20022 Business Application Header and is used by CBPR+ as well as certain national RTGS which have adopted ISO20022 messages.

The DE.BUSINESS.SERVICE.RULES application captures the rules for the Business Service. Delivery uses this application to determine the rules applicable to the Business Service metadata, when this metadata is parameterised in the DE.MESSAGE.HEADER linked to the Delivery Carrier through which the outward message are processed.

- Domain, Business Service and the Status - Fields of the rule are mandatory elements in the DE.BUSINESS.SERVICE.RULES application.
- Message Name Id - Allows the bank to define the message type to which the Business Service Rule applies. The Business Application is the system Id of the module generating the message.
- App Context Field and App Context Field - Define rules based on the content supplied by the Business Application. The SUB.TYPE.INDICATOR is currently supported for App Context Field.
- Business Service - It is the actual value assigned to the Business Service metadata, if the outgoing message satisfies all the other conditions.

The screenshot below shows the setup for the PACS.008.STP messages processed through CBPRPLUS Delivery Module, initiated by TPH, which has the Sub Type Indicator (supplied to Delivery in the App Context Field ) as STP(supplied to Delivery in the App Context Value ).


##### Delivery Notification Requirements

The bank can indicate in the DE.CARRIER if they want to request a positive Delivery Notification message ( Dln Requested set to Yes) for all the outward messages processed through that carrier as well as the Overdue Time Interval , after which the bank expects to receive an overdue delivery notification.

Alternatively, if the positive DLN is required only for certain message types, the bank can define these requirements in the DE.DLN.REQUIREMENTS application.

The ID of this record is the combination of the ID of the Delivery Carrier followed by ‘-‘ (dash) and the ID of the Delivery Message. See below an example to request a positive delivery notification for CBPR+ pacs.008 messages – for EUR messages, the delivery notification is requested only for messages which have the amount bigger than 100,000 and the overdue notification is expected if the message was not successfully delivered in the next 15 minutes. For any other currency the minimum amount for which the delivery notification is requested is 10,000, the overdue notification interval is 1 hour.


##### Delivery Parameter

The DE.PARM application is used to define the Transact Business Modules to which the responses ( Ack/Nack/DLN) must be notified.

Currently only TPH is able to process responses for the outward messages, the configuration below enables Delivery to send the responses received for messages initiated by TPH ( Reply to Appln ) to the queue indicated in the Response Queue Name field.

The Exclude Message Type field defines the message initiated by TPH, for which Delivery does not forward the responses to TPH.


##### IF Exit Point Setup

For messages handed off to the Delivery Transformation Layer by the Delivery module, the XMLISO service, after it determines the header metadata, emits the message through the Integration Framework using the OutwardMessageService.emitOutwardMessage exit point- the configuration for this exitpoint is released in the IF.EXIT.POINTS and IF.INTEGRATION.FLOW.CATALOG applications.

> **⚠️ Note:** The Integration Framework uses the setup in the IF.INTEGRATION.SERVICE.PARAM application to define the queue where the message is emitted. This must be parameterised by the bank to point to the queue identified by the attribute defined in DEHandoffQueue in the QueueConfigMXOutward.properties file used by the Delivery Transformation Layer.


##### Delivery Transformation Layer – Inward Processing Parameterisation

The Delivery Transformation layer processes the inward messages based on the setup in the DE_SWIFTInward_QueueConfig.properties file. The file specifies the queues through which the messages are moved during processing, the rules to determine the source channel as well as the routing decision to the internal/destination channel that identifies the business application to which the message must be forwarded and the transformations that are applied to the message. Each of these sections are described below.

- SWIFTInputQueue - The inward message queue, where the integration layer (Temenos SWIFT Connector) passes the Interact message received from SWIFT Alliance. Delivery Transformation Layer picks up the message from this queue and processes this further.
- RouteChannel=ACTIVEMQ - Indicates the internal processing of the message is done using queues (ActiveMq); Possible values are ACTIVEMQ or FILESYSTEM;

> **⚠️ Note:** FILESYSTEM is only for testing purpose.

- DEBackupQueue - The queue where Delivery Transformation Layer writes a copy of the inward messages, once the message is picked from SWIFTInputQueue queue, for audit purpose.
- MXInputQueue - The intermediary queue where the inward MX messages is routed .
- MXRejectQueue - The queue where the message is moved in case of any failure during MX processing, for example, xsd validation failure or the failures related to local authentication.
- T24DeliveryQueue - The queue to which the messages are sent to Delivery sub system to create the Delivery Inward Header and store the original message.
- OFSRequestQueue - The queue to which the messages are sent for timeout polling.
- T24AppQueue - The queue which stores the copy of the message sent to the OFSRequestQueue. After the response is received from Delivery confirming the DE.I.HEADER is created successfully, the copy of the message is picked from this queue and is sent to the queue decided based by the routing decision .
- IntervalTime - The polling interval to wait for the response from Transact Delivery Subsystem that the Delivery Inward Header for the inward message has been created.
- DeliveryResponseQueue - The queue where Delivery Subsystem returns the response indicating if the Delivery Inward Header has been created and the original message stored.
- AdmiInputQueue - The admi inward messages are moved directly to TPH queue, overpassing Delivery.
- SwiftDataProtectRequestQueue – The queue to which the Delivery framework directs SWIFT messages for data pseudonymization when the user sets the ‘IsAppDataProtected’ property as TRUE. The Temenos exchange adapter encrypts user-classified data in XML messages by consuming them from this queue to enable data privacy before they reach Temenos Transact.
- SwiftDataProtectReplyQueue – The queue to which the Temenos exchange adapter transmits the pseudonymized message responses upon successful encryption.
- SwiftDataProtectErrorQueue - The queue to which the Temenos exchange adapter transmits error responses for the pseudonymized messages during encryption failures.

The environment variable XSD_ROOT_DIR decides the location of the properties files as well as the location of the schemas validation folders.

As shown in the screenshot below, the properties files used by the Delivery Transformation Layer are located under the folder indicated in the XSD_ROOT_DIR environment variable.

The service name in the technical header (XMLV2 envelope) determines the source channel which is used to identify the name of the folder where the XSDs for the respective channels are stored.

SWIFT frequently changes the technical header schema (XMLv2) to introduce new features in the Alliance Access, SWIFTNet, and other systems. The bank uses different versions of the schema. Temenos currently supports the XMLv2 schema version 2.0.12. The bank can use another schema version if that does not have additional mandatory elements.

To use a different XMLv2 version, Temenos cannot access to SWIFT saa schemas. The bank must copy the schema from their Alliance Access product and place it in the folder structure mentioned above. For example, if the bank needs to use the 2.0.13 version schema, the user must place this in the XSD folder under PP_HOME path and rename as saa.2.0.13.

> **⚠️ Note:** If the schema version the bank wants to use introduces mandatory elements, the bank must contact Temenos.

For example, considering the following setup in the inward properties file:

esmig.t2.iast=T2

swift.finplus=CBPRIN

swift.chaps=STGIN

Three different folders namely CBPRIN, STGIN and T2 are defined under the main folder identified by the XSD_ROOT_DIR .

The Delivery Transformation Layer validates the message is received in the XMLV2 envelope as well as BAH, if present.

The name of the schemas in this folder must match the namespace of the XMLv2 envelope (saa.2.0) as well as the namespace of the BAH (head.001.001.02 in case of CBPRPLUS).

The saa.2.0 contains a simplified XMLv2 schema defined by SWIFT, with the main elements expected by the Delivery Transformation Layer.

The AckNackTemenosFormatXsd attribute identifies the name of the schema that is used to validate the inward Ack/Nack/Delivery Notifications, once they have been transformed into Temenos Standard Response format. This is located on the main XSD folder.

The XSLT are located in the folder identified by the XSLT_ROOT_DIR variable.

- The InwardGenericOfsConversion.xslt file stores the transformation which extract the details required to create the Delivery Inward Header and send the original message to Delivery.
- The TransmissionReportXslt and DeliveryReportXslt attributes identifies the files that stores the transformations which are applied to TransmissionReport (Ack/Nack) and DeliveryReport (Delivery Notifications) to transform them in Temenos Standard Response Format before sending them to Delivery.

For LAU validation and Digital Signature validations the Delivery Transformation Layer consults the DE_SWIFTInward_InwardIntegrity.properties file.

The setup in this file is based on the Source Channel which is used as a prefix.

- -LAU-IntegrityCheckRequired - If this is set to TRUE, indicates LAU must be checked for all messages received from the respective source channel; if FALSE then LAU is not checked
- -LAU-Compliance - Indicates the keystore where the bilateral keys used to validate the LAU code supplied in the inward message are stored. Read Working with Swift Security Program for more details on LAU and how the bilateral keys are stored.
- -BAH-IntegrityCheckRequired - Is currently not used.
- -BAH-Compliance - Indicates the keystore.
- -APIName - The Local API which is used to check the BAH signature. The following screenshot shows an example of the setup configured in the DE_SWIFTInward_InwardIntegrity.properties file

The decision to route the inward messages to various Business Applications are based on combining several criteria:

- MessageType
- Sender
- ResponderDN
- Receiver
- RequestorDN
- ServiceIdentifier

The ‘*’ can be used as a wildcard, to replace any value. For Message Type, the first two parts of the ISO20022 Message Name Id should be used, without the ‘.’.

The routing criteria identifies an internal channel to which the message is forwarded, for example:

Considering the above setup:

- All inward messages from ESMIG are sent to the internal channel T2.
- All inward camt.054 messages from CBRPLUS are sent to internal CAMT54 channel.
- All inward camt.057 messages from CBRPLUS are sent to internal CAMT57 channel.
- All other messages from CBRPLUS are sent to CBPRIN channel.
- All inward messages from CHAPS are sent to STGIN channel.

Once the internal Channel is established, the following attributes decide the processing further, each of them being prefixed by the Channel:

- -ACTIVEMQ - Indicates the name of the queue where the message is placed.
- -FILESYSTEM - Indicates the name of the folder where the message is placed ( used by Temenos for internal purposes).
- -Carrier - Indicates the name of the Delivery Carrier through which the message is processed.
- -SkipRouting -Indicates if the message is sent directly to the Business Application or is routed by the Delivery which and processes this based on the inward routine indicated in the DE.MESSAGE.
- -Carrier must have the Formatting Module field set to SWIFT.
- -Carrier must have Formatting Module set to XMLISO.
- -Xslt - Indicates the name of the xslt that is applied to the payload message before being routed to the Business Application.

For example, consider the following setup:

After the Delivery Transformation Layer has determined the internal channel is CBPRIN, it routes the message directly to the business application queue indicated above. No specific transformation is applied to the original payload message. The Delivery Inward Header created for this message indicates the CBPRPLUS Delivery Carrier.

The setup below corresponds to the messages processed through the internal ChannelCAMT57:

These messages are routed by Delivery, the XSLT indicated is applied to the business payload before the message is sent to Delivery. The CBPRPLUS Delivery Carrier is indicated in the Delivery Inward Header for these messages.

| Attribute | Description |
|---|---|
| ReplaceCurencyForReceivingBICS | Indicates the delivery transformation layer to perform currency transformation from a specific currency to another, with the option to exclude this for specific receiving BICs (BICs separated by a comma,","). Format: FromCurrency/ToCurrency/[ReceiverBIC1,ReceiverBIC2, and so on] |


##### Delivery Transformation Layer – Outward Properties Parameterisation

The Delivery Transformation layer processes the outward messages based on the setup in the DE_SWIFTOutward_QueueConfig file, which describes the queues through which the messages are moved during processing, the identification of the destination, the transformations that are applied to form the headers, the setup related to local authentication and digital signatures. Each of these sections are described below.

- RouteChannel - Indicates the internal processing of the message is done using queues (ActiveMq) and the possible values are ACTIVEMQ or FILESYSTEM.

> **⚠️ Note:** FILESYSTEM is only for testing purpose

Queues to Delivery Transformation Layer

- DeliveryPollingQueue - The queue where the Business Applications sends messages to Delivery Transformation Layer.
- SwiftPollingQueue and ChapsPollingQueue - Additional queues where TPH sends the SWIFT and Chaps related messages.
- DEHandoffQueue - The queue where Transact Delivery sends the messages mapped and emitted by Delivery via Integration Queue and this is used when the Business application handoffs the data to Delivery to map the messages.

Validation and Transformations Related Setup

The environment variable XSD_ROOT_DIR decides the location of the properties files as well as the location of the schemas validation folders.

As shown in the screenshot below, the properties files used by the Delivery Transformation Layer are located under the folder indicated in the XSD_ROOT_DIR environment variable.

folder, created under the folder structured identified by the XSD_ROOT_DIR variable.

SWIFT frequently changes the technical header schema (XMLv2) to introduce new features in the Alliance Access, SWIFTNet, and other systems. These changes happen more often than the annual standard changes and the bank uses different versions of the schema. Temenos currently supports the XMLv2 schema version 2.0.12. The bank can use another schema version if that does not have additional mandatory elements.

To use a different XMLv2 version,

- The bank must configure the version of the schema they want to use in the in the Header Version field of DE.MESSAGE.HEADER .
- Temenos cannot access the SWIFT saa schemas. The bank must copy the schema from Alliance Access product and place it in the folder structure mentioned above. For example, if the bank needs to use the version 2.0.13 schema, the user must place this in the XSD folder under PP_HOME path and rename as saa.2.0.13.

> **⚠️ Note:** If the schema version the bank wants to use mandatory elements, the bank must contact Temenos.

- T24DeliveryQueue - The queue through which the Delivery Transformation Layer notifies Transact Delivery about the final message being sent out and/or the processing result based on which the disposition of the Delivery Outward Header is updated.
- T24BackUpQueue - The queue where Delivery Transformation Layer sends a copy of the message sent to Transact Delivery.
- IntegrationOutputQueue - The default queue to the integration layer. Temenos SWIFT Connector should pick the messages from this queue.
- IntegrationErrorQueue - The queue where the rejected messages are moved (for example failures with the XSD validation).
- SwiftDataProtectRequestQueue – The queue to which the Delivery framework directs SWIFT messages for data reconstruction when the user sets the ‘IsAppDataProtected’ property to TRUE. The Temenos exchange adapter decrypts user-classified data in XML messages by consuming them from this queue to enable data reconstruction before they reach the IntegrationOutput Queue.
- SwiftDataProtectReplyQueue – The queue to which the Temenos exchange adapter transmits responses for the reconstructed messages upon successful decryption.
- SwiftDataProtectErrorQueue - The queue to which the Temenos exchange adapter transmits error responses for the reconstructed messages during decryption failures.

For LAU validation and Digital Signature check Delivery Transformation Layer consults the the DE_SWIFTOutward_OutwardIntegrity.properties file.

The setup in this file is based on the outward Channel which is used as a prefix – this is determined based on the OutCarrier specified in the messages received by the Delivery Transformation Layer.

- -LAU-Required - If this is set to TRUE, indicates LAU must be calculated and added to all messages sent to this channel; if FALSE then LAU is not calculated for these messages.
- -LAU-Compliance - Indicates the keystore where the bilateral keys used to calculate the LAU code are stored. Read Working with Swift Security Program for more details on LAU and how the bilateral keys are stored.
- -APIName - Indicates the Local API which is used to calculate and add the BAH signature; if blank then no digital signature is added.
- -BAH-Compliance - Indicates the keystore.
- -IntegrityRequired – Currently not used.


##### Support for Allowed Character Set

The ASCII.VAL.TABLE application allows the bank to define the characters sets used for various purposes, for example, the ISO basic character set used by CBPR, the SWIFT character set used for SWIFT MT messages exchanged across the SWIFT FIN service and so on.

The DE.ALT.CHARS application defines the conversion rules for the characters which are not part of the allowed char set indicated by the Valid Ascii Table field.

For each unsupported character specified in the Local Char Code field, the alternate character(s) to which it must be converted is defined in the Alter Char Code field. Alternate characters are defined based on the position of the unsupported character. For example, if the local character code is the first character in a string, the associated Char Position field must be set to First. For any other position, Char Position field is set to Other or left blank.

The extended character set ISOEXTENDED is available in the Model Bank and defined in DE.ALT.CHARS record.

The Def Alt Char Code field is used to define the default character to which the unsupported characters are converted without specific setup. Space can be specified as a default character using its ASCII value.

The DE.MSG.CHARS.RULE parameterisation table provides the option to specify the message element tags that must be validated for each channel and message type. For each of these tags, the corresponding DE.ALT.CHARS record indicates the conversion rules that apply.


###### Example

This section demonstrates the translation of unsupported characters in an MT942 message based on different configurations.

CONV* is already configured for Tag61 in DE.FORMAT.SWIFT for MT942 as shown below.

Configure the DE.ALT.CHARS ID in DE.CARRIER . This is referred from the Delivery layer, during MT message generation to replace the special characters with alternate characters as configured in DE.ALT.CHARS .

A TPH transaction posted with a special character in the sender’s reference which is not a valid swift character is shown below.

A default character is not defined.

When a MT942 message is generated, since the special character (@) has no alternate character configured in DE.ALT.CHARS , it is not replaced.

A default character is defined.

When a MT942 message is generated, since the special character (@) has no alternate character configured in DE.ALT.CHARS , it is replaced with the default character defined in DE.ALT.CHARS as shown below.

An alternate character for @ is defined as “:”.

When a MT942 message is generated, since the special character (@) has an alternate character configured in DE.ALT.CHARS as “:”, it is replaced with the alternate character as shown below.


> **Related Applications:** `ASCII.VAL.TABLE`, `DE.ALT.CHARS`, `DE.BUSINESS.SERVICE.RULES`, `DE.CARRIER`, `DE.DISTINGUISH.NAME.RULES`, `DE.DLN.REQUIREMENTS`, `DE.FORMAT.SWIFT`, `DE.I.HEADER`, `DE.INTERFACE`, `DE.MESSAGE`, `DE.MESSAGE.HEADER`, `DE.MSG.CHARS.RULE`, `DE.O.HEADER`, `DE.PARM`, `DE_SWIFTInward_InwardIntegrity.properties`, `DE_SWIFTInward_QueueConfig.properties`, `DE_SWIFTOutward_OutwardIntegrity.properties`, `DE_SWIFTOutward_QueueConfig`, `IF.EXIT.POINTS`, `IF.INTEGRATION.FLOW.CATALOG`, `IF.INTEGRATION.SERVICE.PARAM`, `InwardGenericOfsConversion.xslt`, `QueueConfigMXOutward.properties`, `XSD_ROOT_DIR`, `XSLT_ROOT_DIR`

---


### 3.2  Generating Message Flow


> **📇 Quick Reference Card**
> 
> **Purpose:** *SWIFT is migrating to ISO 20022 message standard for Cross Border Payments from Nov 2022 and therefore, the existing SWIFT MT messages will be replaced with ISO 20022 and CBPR+ formats. The Delivery MX Translation (DEMXTR) module transforms the messages MT900, MT910, MT940, MT941, MT942, MT950, MT20...*
> 
> **Applications:** `BATCH`, `DE.BUSINESS.SERVICE.RULES`, `DE.CARRIER`, `DE.DELIVER.REQUEST.LISTENER`, `DE.DELIVERY.REQUEST.LISTENER`, `DE.DISTINGUISH.NAME.RULES`, `DE.INTERFACE`, `DE.MESSAGE` ... +7 more
> 
> **Key Fields:** *Disposition*, *Event Dest*, *Message Type*, *Msg Name Id*, *Send Msg Type*, *Status*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

SWIFT is migrating to ISO 20022 message standard for Cross Border Payments from Nov 2022 and therefore, the existing SWIFT MT messages will be replaced with ISO 20022 and CBPR+ formats. The Delivery MX Translation (DEMXTR) module transforms the messages MT900, MT910, MT940, MT941, MT942, MT950, MT202, MT210 and MT103 messages into its equivalent CBPR+ compliant CAMT messages.

When the DEMXTR module is installed in Temenos Transact prior to the R21 release, then Standalone Temenos Payments (TPH) implementation must be deployed on R21 or R22 releases. The following are the configuration details.

- The delivery customer preferences are held in Transact release.
- The delivery carrier for extended MT is configured in Transact release.
- The ISO channel characteristics are configured in the Delivery module installed in the Standalone TPH platform.
- The DE.DELIVERY.REQUEST.LISTENER application is configured in the Standalone TPH platform.

The below table defines the updates installed for generating ISO20022 CBPR+ equivalent messages for MT900, 910, 940, 950, 941 and 942.

| Product | Updates |
|---|---|
| DE | XX _ DE_OutwardMessageService XX _ DE_Outward XX _ DE_Config DE_SWIFTOutward-0.0.x.war |
| DEMXTR | DEMXTR_MTMXOutward-0.0.x.war |

> **⚠️ Note:** XX - Denotes the release number.


#### ⚙️ Configuration

This section defines the configuration steps required for generating ISO20022 CBPR+ camt053, camt052 and camt054 as an MT to MX translation of MT940, 950, 941, 942, 900 and 910 through Delivery MX Translation (DEMXTR) module.

> **⚠️ Note:** Perform the instructions given below only when the DE and DEMXTR modules are licensed and installed.


##### Deploying War File

To deploy the war file,

1. Set environment variables.
2. Place the stylesheets in the path mentioned in the XSLT_ROOT_DIR system variable.
3. deployments folder.

The war files are deployed successfully.


##### Configuring Transact

To configure Transact for DEMXTR to generate messages, follow the below steps.

1. SWIFTXMLINT
2. Create records in TSA.SERVICE and BATCH applications to emit extended MT messages.
3. Configure the destination queue, in the IF.INTEGRATION.SERVICE.PARAM application, through which the SWIFTXML.OUT service routes the MT messages to the delivery translation layer.


##### Configuring Standalone TPH Platform

Perform the following steps to configure the standalone TPH platform.

1. DEMXTR_ESBOutward
2. Enter the below value in the Msg Name Id field in DE.MESSAGE . Record Respective value in Msg Name Id CAMT053 camt.053.001.08 CAMT052 camt.052.001.08 CAMT054 camt.054.001.08 .
3. Authorise the CAMT053, CAMT052, and CAMT054 message type records for creating a record in the DE.MESSAGE.CONCAT live table.
4. Configure the destination queue ( Event Dest ) in the IF.INTEGRATION.SERVICE.PARAM application, through which the DE.DELIVERY.REQUEST.LISTENER application routes the MTXML message to the delivery transformation layer.
5. To configure delivery transformation layer, parameterise the routing rules for the MT900, 910, 940, 950, 941 and 942 message types in the DEMXTR_MTMXOutward_QueueConfig property file.
6. Configure TPS.INTERNAL.CONFIGS as shown below for the additional TPH enriched tags to be mapped.
7. Post installation, copy the delivered XSLT’s and XSD’s to PP Home folders.


#### 🔧 Working With

This sections defines the workflow for the DEMXTR module which generates an ISO20022 CBPR+ message by translating its equivalent MT message.

> **⚠️ Note:** The below screenshots are the sample steps to generate the CBPR+ CAMT054 and CAMT052 from its equivalent MT900 and MT942 respectively.


##### Generating CAMT054 - ISO2022 CBPR+ Equivalent for MT900

Perform the following steps to generate CAMT054 using the new MT carrier SWIFTXML.

1. Create a record in DE.PRODUCT .
2. Initiate a transaction to create an MT900 message. For example, creating Letter of Credit transaction generate 900 debit advice. The Disposition field in DE.O.HEADER generates Unformatted status for the message type 900.
3. Run BNK/SWITFXML.OUT service to emit IF event and the status in the Disposition field is updated as Formatted.
4. Run BNK/INTEGRATION.SERVICE in servlet mode to create a record in DE.DELIVERY.REQUEST.LISTENER .
5. Run BNK/XMLISO.OUT service to update the Status field as Routed. For the CAMT054 message type a DE.O.HEADER is created with the Disposition field updated as Unformatted and IF event emitted.
6. Run BNK/INTEGRATION.SERVICE in servlet mode to update the Disposition field as Ofs Formatted for MX messages.

CAMT message is generated successfully by translating MT900 with the business application and technical header.


##### Generating CAMT052- ISO2022 CBPR+ Equivalent for MT942

Perform the following steps to generate CAMT052 using the existing MT carrier SWIFT.

1. Enter the required values for the Message Type and Send Msg Type fields in ACCOUNT.STATEMENT .
2. Create a record in DE.PRODUCT and DE.ADDRESS .
3. Create a request for the MT942 message in DE.STATEMENT.REQUEST . The MT942 with status as Unformatted is generated in DE.O.HEADER . Generated MT942 message.
4. Run BNK/SWIFT.OUT service to update the status of the Disposition field as formatted and to emit the IF event.
5. Run BNK/INTEGRATION.SERVICE in servlet mode to update the Status field as Awaiting.Enrichment and emit the IF event.
6. Run BNK/DE.GET.ADDITIONAL.ENRICHMENT and BNK/XMLISO.OUT service to: Calculate the transaction summary Determine additional enrichment for the payment transaction Update the status of the record in the Status field as Routed. Create a record in DE.O.HEADER and emit IF Events.
7. Run BNK/INTEGRATION.SERVICE in servlet mode to update the status of the Disposition field as Ofs Formatted in the record.

CAMT message is generated successfully by translating MT942 with the business application and technical header.


##### Updating Deployment Details

| War or Jar | Standalone TPH Platform | Transact Instance |
|---|---|---|
| DE_OutwardMessageService | Yes | Yes |
| DE_Outward | Yes | Yes |
| DE_Config | Yes | Yes |
| DE_SWIFTOutward-0.0.x.war | Yes | No |
| DEMXTR_MTMXOutward-0.0.x.war | Yes | No |


#### 📋 Tasks

There are no Tasks for the Generating Message Flow feature.


#### 📊 Outputs

There are no Outputs available for the Generating Message Flow feature.


> **Related Applications:** `BATCH`, `DE.BUSINESS.SERVICE.RULES`, `DE.CARRIER`, `DE.DELIVER.REQUEST.LISTENER`, `DE.DELIVERY.REQUEST.LISTENER`, `DE.DISTINGUISH.NAME.RULES`, `DE.INTERFACE`, `DE.MESSAGE`, `DE.MESSAGE.CONCAT`, `EB.COMPONENT`, `EB.PRODUCT`, `IF.INTEGRATION.SERVICE.PARAM`, `TPS.INTERNAL.CONFIGS`, `TSA.SERVICE`, `VERSION`

---


### 3.3  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *Temenos contract-based financial applications can generate SWIFT MT103/202 payment messages. Temenos strategic business modules generate Payment Orders and Temenos Payment solution decides the payment channel and the format of the messages that must be exchanged. Temenos legacy modules (for example,...*
> 
> **Key Fields:** *Ack Required*, *Carrier Address No*, *Format Module*, *Interface*, *SystemId*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Temenos contract-based financial applications can generate SWIFT MT103/202 payment messages. Temenos strategic business modules generate Payment Orders and Temenos Payment solution decides the payment channel and the format of the messages that must be exchanged. Temenos legacy modules (for example, LD) which do not have the capability to generate payment orders will not be enhanced to provide this feature.

Temenos contract-based financial applications are designed to generate MT900/910 (debit and credit advice) messages. Some of these applications can also send MT210 (notice to receive) messages to their counterparties.

The Delivery MX Translation module enables banks to send ‘like for like’ (the tags populated in the ISO20022 outward messages are populated based on the fields supplied in the outward MT messages) ISO20022 CBPR compliant camt.054 and camt.057 messages to their counterparties based on the MT210/900/910 messages generated by the business modules. The Delivery MX Translation module also enables banks to generate Payment Order based on the MT103/202 messages generated by legacy modules like Loan and Deposit (LD) module.

The Delivery MX Translation Module does not handle the MT103 and MT202 generated by the Funds Transfer module. Banks must initiate their payments using Payment Order.

Transact clients who are in releases prior to R22 AMR can implement a standalone Temenos Payments platform to process the ISO20022 SWIFT payments. Delivery MX Translation module, installed as part of standalone Temenos Payments platform, receives the MT103/202 generated by Transact business modules and transforms them to payment order. Temenos Payments executes the payment orders and generates the final ISO20022 message. Temenos Transact business modules that generate the MT210/900/910 messages can run in the same platform with Temenos Payments or can be implemented on a different platform (possibly on a lower release).

IZCAMT module is a Temenos strategic module that produces customer statements and account reporting messages. It offers ‘out of the box’ pre-configured enriched events and provides the flexibility to further customise and enrich the content of the transaction details. Delivery MX Translation module, available as part of Standalone Payments platform, generates ‘like for like’ ISO20022 statement and account report messages based on the MT940/950/941/942 messages generated from Temenos Transact .

> **⚠️ Note:** If the Temenos Transact business modules and Temenos Payments are deployed on different platforms, the Delivery module must run on both platforms. In the Temenos Transact the Delivery module is used to generate SWIFT MT messages (SWIFT formatting) and on the Temenos Payment platform the Delivery module is used to generate the ISO20022 messages.

The SWIFTXML Delivery Carrier is released as part of Delivery (DE) module to be used for SWIFT MT messages that must be translated to ISO20022 standards. Though the SWIFTXML Delivery Carrier uses the SWIFT formatting module to generate MT messages, it has a dedicated interface which emits an extended MT message into a queue. The extended MT message includes the main details from the delivery message header along with the MT message.


##### Product Configuration

This section covers the setup required by the Delivery MX Translation module.

The Delivery module uses the SWIFT Delivery Carrier and SWIFT Formatting modules to generate MT messages. For the MT messages which must be translated to ISO20022, the bank must use a different Delivery Carrier. The SWIFTXML Delivery Carrier has been released for this purpose.

The setup of the SWIFTXML DE.CARRIER indicates:

- The Format Module is SWIFT.
- A dedicated DE.INTERFACE is assigned to this Delivery Carrier (referred by the Interface field in DE.CARRIER ) which emits messages through the Integration Framework and generates messages in the Temenos Extended MT format (the message includes the MT message along with the main details of the delivery header).

- The Ack Required field is set to No in the DE.INTERFACE application.

- The DE.PRODUCT application decides the delivery preferences for the delivery messages. The default setup for the MT messages is to generate them using the SWIFT Delivery Carrier (the Carrier Address No field in DE.PRODUCT is set to SWIFT.1). Implementations must change this setup to refer the SWIFTXML Delivery Carrier addresses when they want the MT messages to be translated to ISO20022 CBPR+ standards.

> **⚠️ Note:** Implementations can set up local Delivery Carriers if they need to route the translated ISO20022 messages to other channels than CBPRPLUS.

For each DE.CARRIER which has the Format Module field set to SWIFT, the bank must run its dedicated service – the naming convention is .OUT.

> **⚠️ Note:** The bank must set up the SWIFTXML.OUT TSA.SERVICE and its SWIFTXML.OUT BATCH on the platform where the business applications which are generating the MT messages are implemented. If Temenos Transact and TPH are running on different platforms, the records must be created in Temenos Transact.

The bank must run the SWIFTXML.OUT and INTEGRATION.SERVICE services to generate the messages in the extended MT format.

The integration queue where the SWIFTXMLINT DE.INTERFACE emits the extended MT message to the Delivery Translation layer must be defined in the IF.INTEGRATION.SERVICE.PARAM application:

- Event type destination: Outwardmessageservice-mtmessageflow
- Event destination: queue/t24MtMessageQueue

The name of the Delivery MX Translation component is DEMXTR_MTMXOutward-0.0.1-SNAPSHOT.war, which must be deployed in the Temenos\jboss\standalone\deployments path. The technical characteristics for the Delivery MX Translation processing are defined in the DEMXTR_MTMXOutward property file. For example, the queue mechanism connectivity, ip, max connections and number of concurrent consumers.

The Delivery MX Translation layer processes the extended MT messages based on the setup in the DEMXTR_MTMXOutward_QueueConfig property file. The file describes the various queues through which the messages are moved during processing and the routing rules based on which the Delivery MX Translation layer determines the processing rule and the processing characteristics.

> **⚠️ Note:** The transformations which are applied to the outward messages are located in the folder identified by the XSLT_ROOT_DIR variable.

The configurations defined in this file are described below:

- RouteChannel attribute – Indicates the internal processing of the message is done using queues (ActiveMq) or folders. The values are ACTIVEMQ or FILESYSTEM; however, FILESYSTEM is used for Temenos internal purposes.
- DEMXTRHandoffQueue attribute – Defines the queue where the MT messages generated by the business applications are emitted through the Delivery module in the extended MT format. Delivery MX Translation picks the messages from this queue and starts the processing, applying the DEMXTR-MTXML.xslt to transform the message into MTXML format.

- MtXmlTransPostQueue attribute – Indicates the queue where DEMXTR places the message if the transformation into MTXML format is successful. This message is evaluated using the routing rules to decide the target processing.

- transformationFailQueue attribute – Indicates the queue where DEMXTR places the message in the Extended MT format, if the transformation to MTXML format fails.

- DefaultQueue attribute – Indicates the queue where DEMXTR places the MTXML format, if no routing rule is matched and no processing rule is found.
- T24DeliveryQueue attribute – Identifies the queue where DEMXTR sends the messages to the target application in the target application format (the Delivery Request Listener application installed on the same platform with TPH). The messages are processed using XMLOFS OFS.SOURCE.

- extTransFailQueue attribute – Specifies the queue where DEMXTR places the message if transformation to the target application format fails. The message is in MTXML format.

- DLQError attribute – Specifies the folder where DEMXTR places the message if the queues become unavailable during processing.

The routing rules which are used to determine the processing rules are defined in the following manner:

MessageType-ServiceIdentifier-Application-SenderBic-SourceCarrier=Channel

The ‘*’ can be used as a wildcard character to indicate any value. For example, considering the following setup:

- 900-*-*-*-SWIFTXML=ROUTECBPR
- 910-*-*-*-SWIFTXML=ROUTECBPR
- 210-*-*-*-SWIFTXML=ROUTECBPR
- 103-*-*-*-*=103ROUTE
- 202-*-*-*-*=202ROUTE

According to this setup, the MT210, 900, 910 messages are processed based on the characteristics defined for the ROUTECBPR channel, irrespective of the service identifier, application generating them, sender BIC or source carrier.

-attributeName. The following attributes are supported:

- SystemId attribute — Identifies the target module to which the message is routed.
- Carrier attribute — Specifies the carrier which is to be used if the message is sent to the Delivery module.
- Xslt attribute — Specifies the name of the XSLT that is applied to the MTXML message before sending the message to the target module.
- Company attribute — Specifies the company to which the message is re-routed (in an implementation which involves Temenos Transact and standalone TPH, the companies in Temenos Transact could be different from those defined in Standalone TPH). If this is blank, the target company for the ISO20022 message is the same as the source company of the MT message.
- POProduct — Used for MT103/202 routing and indicates the Payment Order product.

For example, the following setup indicates the processing attributes for the ROUTECBRP channel:

- ROUTECBPR-SystemId=DE
- ROUTECBPR-Carrier=CBPRPLUS
- ROUTECBPR-Xslt=transformToDeliveryRequest.xslt
- ROUTECBPR-Company=

According to this setup, the Delivery MX Translation module applies the transformToDeliveryRequest.xslt transformation to the MTXML message processed through the ROUTECBPR channel, set the target Delivery Carrier to CBPRPLUS and then routes the message to the Delivery module (identified by SystemId attribute).

- The target company where the MTXML message is processed is the same as company for the source MT message (Company is blank).
- The properties file can be amended to suit the implementations. However, the attributes must not be removed. The implementation can remove the value defined for the respective attribute rather than remove or comment the attribute itself.


##### Illustrating Model Parameters

Model Parameters are not applicable for this module.


##### Illustrating Model Products

The SWIFTXML DE.CARRIER and SWIFTXMLINT DE.INTERFACE have been released to generate the MT messages that must be translated into ISO20022.

---


### 3.4  Transform messages to Payment


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Delivery MX Translation module enables bank to generate Payment Order based on the MT103/202 messages generated by legacy modules like Loan and Deposit (LD) module.*
> 
> **Key Fields:** *Auto Pay Acct*, *Company*, *DEMXTRHandoffQueue*, *Debit account*, *Def Funds Diversion*, *DefaultQueue*, *MtXmlTransPostQueue*, *Sign* ... +6 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The Delivery MX Translation module enables bank to generate Payment Order based on the MT103/202 messages generated by legacy modules like Loan and Deposit (LD) module.

Transact clients that are in releases prior to R21 AMR can implement a standalone Temenos Payments platform (R21 or R22 AMR+) to process the ISO20022 SWIFT payments. Delivery MX Translation module, installed as part of standalone Temenos Payments platform, receives the MT103/202 generated by Transact business modules and transform them to payment order. Temenos Payments executes the payment orders and generates the final ISO20022 message.

In the past the MT103/202 payment messages have been generated directly by the contract based modules, through the Delivery. The contract raised the accounting entries and credited the Nostro or Vostro account used in the payment.

However, if the MT103/202 messages are not sent to SWIFT directly but they are translated to payment orders the entries raised by the contract on the Nostro or Vostro account must be diverted to a wash (suspense) account. When the payment order is executed, Temenos payments raises the booking entries and clears (debit) the wash account and credits the Nostro or Vostro account involved in the transaction. Auto-pay accounts must be setup for the Nostro or Vostro accounts used by the business modules and the funds diversion must be parameterised for the respective business modules.

The MT103, 202 messages are emitted through the Delivery Framework using the SWIFT formatting functionality and a dedicated interface. The messages are generated into a Temenos extended format.

The Delivery Translation module picks these messages, transforms them into XML (Temenos MTXML format), identifies the target carrier and sends them to the Payment Order application on the same platform with Temenos Payments (in case of a Transact and Standalone Temenos Payments implementation, Payment Order is implemented in the Standalone Payments platform). The debit account in the Payment Order indicates the auto-pay account used by the funds diversion.

The Payment Order hands-off the message to Temenos Payments which executes the message, determines the channel and sends the payment out. If cover method is used, Temenos Payments also generates the cover message.

Once the payment is successfully executed, Temenos Payments raises the booking entries and clears the wash account set as auto-account and credits the Nostro or Vostro account.

> **⚠️ Note:** Bank must include the Auto-Pay Accounts as part of their account reconciliation process.

The following flowchart explains how the Delivery MX Translation module works when the business modules generating the messages are on a different Temenos Transact platform (and potentially on a different Temenos Transact release version) than Temenos Payments.

The flowchart below explains how the Delivery MX Translation works when the business modules and TPH are on the same platform.


#### ⚙️ Configuration

In addition to the product configuration, the following setup is specific to the MT103,202 translation to payment orders.


##### Auto pay account configuration

For all the Nostro or Vostro accounts used by the contract based applications for which the MT103/202 must be routed through payment order, the Auto Pay Acct field in the ACCOUNT application must be set to indicate the wash account to which the funds will be diverted.


##### Funds diversion configuration

The AC.FUNDS.DIVERSION.PARAM must be used to redirect the accounting entry raised by the business module from the Nostro/Vostro account to the auto pay account.

The Def Funds Diversion field indicates the default behaviour for the entries raised on the auto-pay account. If the bank sets this to No, it means that by default the accounting entries are not diverted to the auto-pay accounts.

The Sys Txn Code field and its associated subfields, Sys Id Sign and Sys Txn Code fields allow the bank to indicate the modules, sign, and transaction codes for which the entries must be diverted to the auto-pay accounts. If the Sys Id Sign is not specified, the accounting entries will be diverted to the auto-pay accounts, irrespective of the sign.

The bank must use this setup to indicate the business modules for which the MT103, 202 are translated to payment orders. For each module, bank must define the transaction codes which are used to debit or credit the Nostro or Vostro accounts to ensure the funds are diverted to the wash accounts.


#### 🔧 Working With

The transformation of the MT103, 202 messages into payment orders involve the following steps:

1. Divert the accounting entries raised by the contract-based module to the auto pay account set for the counter party account, when the payment event is generated – this is performed by the AC module, part of Transact.
2. Emit the MT message in the extended format – performed by the Delivery module, installed on Transact platform.
3. The Delivery MX Translation module, installed on Temenos Payments platform, to performs the following steps: Translate the extended MT message into XML format Assign the payment order product Apply the transformation to payment order expected format and route the message to the payment order.
4. Processing the Payment Order – performed by Payment Order and Temenos Payments.

The following diagram explains a high-level view of the Delivery MX Translation workflow when Transact and Temenos Payments are on the same platform.

The following diagram explains a high-level view of the of the Delivery MX Translation workflow when Temenos Payments is implemented as a standalone, on a separate platform.


##### Diverting the Funds

The system diverts the accounting entry raised by the contract when it generates the payment event from the Nostro or Vostro account to the wash account, using the setup for auto-pay account diversion

Considering the setup explained in Configuration, the principal and commission entries raised by the LD contract are diverted to the wash account specified in the Auto Pay Acct field of the counterparty account involved in the payment.


##### Emitting the MT Message in the Extended Format

As explained in the product configuration section, the DE.PRODUCT for the MT103,202 messages that is transformed to payment must be changed to indicate the SWIFTXML delivery addresses.

Based on this setup, the Delivery module uses the SWIFTXML DE.CARRIER to emit the MT103, 202 messages generated by the contract based modules.

The SWIFTXMLINT DE.INTERFACE indicated in the SWIFTXML DE.CARRIER emits the message in an extended MT format, which includes the MT message and the main details from the DE.O.HEADER .

> **⚠️ Note:** The MT202COV for these messages must be stopped using the DE.DISP.CONTROL . The cover payment messages are generated by the Temenos Payments while executing the payment order.


##### Transforming the Extended MT Message to MTXML and Routing to Payment Order

The Delivery MX Translation module picks the message from the queue identified by the DEMXTRHandoffQueue property attribute (specified in the DEMXTR_MTMXOutward_QueueConfig properties file) and processes the message as follows:

- It applies a transformation to the Temenos generic MTXML format (using the DEMXTR-MTXML.xslt located in the stylesheet folder identified by the XSLT_ROOT_DIR variable).
- In case of errors during the transformation, the message is moved to the queue identified by the transformationFailQueue property attribute and the processing of that message is stopped.
- The message successfully transformed into the generic MTXML is moved to the queue identified by the MtXmlTransPostQueue properties attribute and evaluated based on the routing rules defined in the properties file to determine the processing rule.
- If routing rule is not matched, the message is moved to the queue identified by the DefaultQueue attribute and the processing of that message is stopped.
- If a routing rule is matched, then the processing rule is identified.

For example, consider the following parameterisation in the properties file for the routing rules:

Based on the above configuration, the MTXML messages corresponding to the MT103 messages generated through the SWIFTXML Delivery Carrier are processed according to the 103ROUTE processing rule. The ‘*’ indicates that the processing is done irrespective of the message service identifier, the application which generates the respective message or the sender BIC.

Read the Product Configuration – Delivery MX Translation Parameterisation section for more information.

The MTXML message is processed based on the parameters of the processing rule attributes (the attributes are prefixed with the processing rule), which define the payment order product and the target transformation.

For example, considering the above parameterisation of the processing attributes for the 103ROUTE processing rule:

- The POProduct attribute defines the payment order product.
- If the Company attribute is not specified in the property file, the message is sent to the target module using the company indicated in the MTXML message. Alternatively, the bank can specify a different company. For example, if the TPH Standalone has a different company structure than the Temenos Transact platform where the business module generating the MT message is implemented, the Company attribute allows the bank to indicate the Target Company to which the message must be sent.
- Finally, the transformation indicated by the Xslt attribute is applied to the MTXML message to transform it to the Payment Order format.
- If the transformation to the target format (Payment Order, in this case) fails, the message is moved to the queue identified by the extTransFailQueue property attribute and the processing of that message stops. The format of the message is MTXML.
- The message transformed into the target application format is moved to the queue identified by the T24DeliveryQueue property attribute. The message is in the DE.DELIVERY.REQUEST.LISTENER format.


##### Payment Processing

The OFS layer picks the MTXML messages and routes them to the corresponding application based on the setup in the XMLOFS OFS.SOURCE .

The MT103,202 messages are routed to the PAYMENT.ORDER application, which is part of the Delivery module. The Debit account field of the PAYMENT.ORDER record indicates the auto-pay account.

The payment order is processed by Temenos Payments and once the payment is executed, the auto-pay account is debited.


#### 📋 Tasks

There are no Tasks for the Transforming MT103, MT202 messages to Payment Order feature.


#### 📊 Outputs

There are no Outputs available for the Transforming MT103, MT202 messages to Payment Order feature.

---


### 3.5  Translating Messages


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Delivery MX Translation module enables the bank to send to their counterparties the ISO20022 CBPR compliant camt.054 and camt.057 messages based on the MT210/900/910 messages generated by the business modules. The business modules which generate the MT210/900/910 messages can be deployed on the ...*
> 
> **Key Fields:** *Carrier Address No*, *DeRequestListenerQueue*, *Delivery Out Header Id*, *Event Dest*, *Event Type*, *Format Module*, *Last Page Indicator*, *Message Name Id* ... +13 more
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The Delivery MX Translation module enables the bank to send to their counterparties the ISO20022 CBPR compliant camt.054 and camt.057 messages based on the MT210/900/910 messages generated by the business modules. The business modules which generate the MT210/900/910 messages can be deployed on the same instance with TPH and the Delivery Module or can run on a different instance.

The Delivery MX Translation can also be used to send the following ISO20022 CBPR+ compliant Account reporting messages based on the corresponding MT messages:

- camt.053( Bank to Customer Statement) : translated from MT940 and MT950
- camt.052 (Bank to Customer Account Report): translated from MT942 and MT941
- camt.054 (Bank to Customer Debit Credit Notification): translated from MT900 and MT910
- camt.060 (Account Reporting Request): translated from outward MT920

The MT210/900/910/920/940/950 messages are emitted through the Delivery Framework using the SWIFT formatting functionality and a dedicated interface. The messages are generated into a Temenos extended format.

The Delivery MX Translation module picks these messages, transforms them into XML (Temenos MTXML format), identifies the target carrier and sends them to the Delivery Request Listener application.

> **⚠️ Note:** The Delivery Request Listener application is part of the Delivery module implemented on the same platform with Temenos Payments. (In case of a Transact and Standalone Temenos Payments implementation, Delivery Request Listener is implemented in the Standalone Payments platform).

The Delivery Request Listener handoffs the messages to Delivery which generates the final ISO20022 messages.

- The following flowchart explains how the Delivery MX Translation module works when the business modules generating the messages are on a different Temenos Transact platform (potentially on a different Temenos Transact release version) than Temenos Payments.
- The delivery customer preferences are held in the Transact.
- The delivery carrier ‘SWIFTXML’ for ‘extended MT’ must be configured in Transact.
- The ISO channel characteristics are managed by the Delivery modules installed in the Standalone TPH.
- The flowchart below explains the Delivery MX Translation works when the business modules and TPH are on the same platform.


#### ⚙️ Configuration

In addition to the product configuration, the following setup is specific to the MT210, 900, 910, 920, 940, 941, 942, 950 translation.


##### Delivery Carrier Configuration

The message name variant ( Message Name Id field) and the payload transformation ( Transformation Rule field) to CBPR+ ISO20022 messages are set up for the Delivery messages 210, 900, 910, 920, 940, 941, 950 in the CBRPPLUS DE.CARRIER . This configuration must be done on the platform where Temenos Payments is implemented.

> **⚠️ Note:** The payload transformations are located in the stylesheet folder identified by the XSLT_ROOT_DIR variable.


##### MTXML Delivery Requests – Integration Framework Queue Parameterisation

The local implementations must configure in the IF.INTEGRATIONS.SERVICE.PARAM application the name of the queue where the DE.REQUEST.LISTENER application emits the message to the Delivery Transformation layer.

- Event Type must be set to Outwardmessageservice-mtxmlmessageflow.
- Event Dest stores the queue name where the message is emitted.

This configuration must be done on the platform where Temenos Payments is implemented.


##### Delivery Transformation Layer Configuration

The DeRequestListenerQueue attribute of the DE_SWIFTOutward_QueueConfig properties file indicates the queue from where the Delivery Transformation Layer picks the messages which have the payload in the MTXML format. It applies the payload and header transformation, validates the message and emits them to the integration queue from where they are processed by the Temenos SWIFT Interact connector and sent to SWIFT Alliance interface.

This configuration is be done on the platform where Temenos Payments is implemented.


#### 🔧 Working With

The translation of the MT210, 900, 910, 920, 940, 941, 942, 950 messages to ISO20022 messages involves the following four main steps:

- Emitting the MT message in extended format – performed by the Delivery module.
- Translating the extended MT message into XML format, assigning target carrier and routing the message to the Delivery Request Listener – performed by the Delivery MX Translation module.
- Processing the delivery requests, determining the characteristics of the target carrier and emitting the message to the Delivery Translation Layer – performed by the Delivery module.
- Transforming the payload and headers, generating LAU and emitting the message to the integration layer – performed by the Delivery Transformation Layer, which is part of the Delivery module.

The following diagram presents a high-level view of the workflow and the details are presented in the following sections.


##### Emitting the MT Message in the Extended Format

As explained in the product configuration section, the DE.PRODUCT application decides the delivery preferences for the delivery messages. The default setup for the MT messages is to generate them using the SWIFT DE.CARRIER (the Carrier Address No field in DE.PRODUCT is set to SWIFT.1). Implementations must change this setup to refer the SWIFTXML DE.CARRIER addresses when they want the MT messages to be translated to ISO20022 CBPR+ standards or payment orders.

The SWIFTXMLINT DE.INTERFACE indicated in the SWIFTXML DE.CARRIER emits the message in an extended MT format, which includes the MT message as well as the main details from its DE.O.HEADER .

The SWIFTXML.OUT TSA.SERVICE must run to emit the MT messages generated by the business applications in the Extended MT format.


##### Translating the Extended MT Message to MTXML and Routing to Delivery Request Listener

The Delivery MX Translation module picks the message from the queue identified by the DEMXTRHandoffQueue property attribute (specified in the DEMXTR_MTMXOutward_QueueConfig properties file) and processes the message as follows:

- The Delivery MX Translation module applies a transformation to the Temenos generic MTXML format (using the DEMXTR-MTXML.xslt located in the stylesheet folder identified by the XSLT_ROOT_DIR variable).
- In case of errors during the transformation, the message is moved to the queue identified by the transformationFailQueue property attribute and the processing of that message is stopped.
- The message successfully transformed into the generic MTXML is moved to the queue identified by the MtXmlTransPostQueue properties attribute and evaluated based on the routing rules defined in the properties file to determine the processing rule.
- If no routing rule is matched, the message is moved to the queue identified by the DefaultQueue attribute and the processing of that message is stopped.
- If a routing rule is matched, then the processing rule is identified.

For example, considering the following parameterisation in the properties file for the routing rules, the 210, 900, 910 messages generated through the SWIFTXML Delivery Carrier are processed according to the ROUTECBPR rules, irrespective of message service identifier, the application which generated the respective MT message or the sender BIC.

According to this setup the 210, 900, 910 messages generated through the SWIFTXML Delivery Carrier are processed according to the ROUTECBPR rules, irrespective of message service identifier and the application that generateds the respective MT message or the sender BIC.

Read the Delivery MX Translation Parameterisation section for more information.

The MTXML message is processed based on the parameters of the processing rule attributes (the attributes are prefixed with the processing rule) which define the target module to which the message is sent, the target carrier, the target company and the target transformation.

- ROUTECBPR-SystemId=DE
- ROUTECBPR-Carrier=CBPRPLUS
- ROUTECBPR-Xslt=transformToDeliveryRequest.xslt
- ROUTECBPR-Company=

For example, considering the above parameterisation of the processing attributes for the ROUTECBPR processing rule:

- The SystemId attribute defines the target processing module. The Delivery MX Translation module sends the MT210, 900, 910 messages to DE which handles their transformation to the ISO20022 standards.
- The target carrier of the message is identified based on the Carrier attribute.
- If the Company attribute is not specified in the property file, the message is sent to the target module, using the company indicated in the MTXML message. Alternatively, the bank can specify a different company, for example, if the TPH Standalone has a different company structure than the Temenos Transact platform where the business module generating the MT message is implemented.
- Finally, the transformation indicated by the XSLT attribute is applied to the MTXML message to transform this into the Delivery Request Listener format.

- If the transformation to the target module format fails, the message is moved to the queue identified by the extTransFailQueue property attribute and the processing of that message stops. The format of the message is MTXML.

- The message successfully transformed into the target application format is moved to the queue identified by the T24DeliveryQueue property attribute. The message is in the DE.DELIVERY.REQUEST.LISTENER format.


##### Processing the MTXML Delivery Request

The OFS layer picks the MTXML messages and routes them to the corresponding application based on the setup in the XMLOFS OFS.SOURCE.

The MT210, 900 ,910, 920, 940, 950, 941, 942 messages are routed to the DE.DELIVERY.REQUEST.LISTENER application, which is part of the Delivery module:

- Org Payload — Stores the original MT message (new line is represented by the ~ separator)
- Payload — Stores the message in the MTXML format, encoded in base64.
- Source Application — Indicates the business application which generated the MT message.
- Source Trans ref — Stores the transaction ID.
- Source Common Ref — Stores the ID of the DE.O.HEADER for the MT message.
- Source Unique Id — Indiactes the carrier sequence of the MT message.
- Target Carrier — Indicates the DE.CARRIER through which is to be used to transform the message to the ISO20022 format.
- Target Msg Type — Indicates the delivery messages associated with the transformed message.
- Delivery Out Header Id — Keeps the ID of the Delivery Outward Header for the transformed ISO20022 message.

The following fields are populated for the account report messages:

- Page Number — Page number of the MT message.
- Statement Id — Unique value of a statement. This value is common for all the pages of the statement (applicable only for the message types MT940/950/941/942), in case of paginated statements.
- Last Page Indicator — Indicates the last page of the MT message (applicable only for the message types MT940/950/941/942).

The following is an MTXML sample message – the content of the Org Payload field stores the message in this format, but encoded in base64.

Additional processing is required for the MT940,950,941,942 messages as the transaction summary must be populated in the message representing the first page of the statement.

The Status field is set to Awaiting Enrichment in the DE.REQUEST.LISTENER records created based on the MT940, 950, 941, 942 messages.

The DE.GET.ADDITIONAL.ENRICHMENT TSA.SERVICE must run in the background to process the DE.DELIVERY.REQUEST.LISTENER records with Status as Awaiting Enrichment. Once the service determines that all pages are available,

- It calculates the Transaction Summary for the whole statement and updates this in the record representing the first page of the statement.
- Get the additional enrichment for TPH related transactions and updates them in the corresponding records.
- Once the processing is done, it changes the Status field of the DE.REQUEST.LISTENER records to blank.

If the Status field is blank, the message can be processed further and the DE.DELIVERY.REQUEST.LISTENER checks the characteristics of the DE.CARRIER identified by the Target Carrier field in DE.DELIVERY.REQUEST.LISTENER .

If the target carrier is an XMLISO carrier (the Format Module field in DE.CARRIER is XMLISO), the DE.DELIVERY.REQUEST.LISTENER updates the XMLISO.OUT.LIST file. Once the XMLISO.OUT service runs, it checks the corresponding DE.DELIVERY.REQUEST.LISTENER record and considers the technical and business headers configured for the respective carrier, the message name variant and payload transformation that is setup for the respective source message type and emits the payload message along with the header details through Integration Framework.

The following screenshot shows the DE.O.HEADER associated with the ISO20022 message generated by the DE.DELIVERY.REQUEST.LISTENER. The Message Type indicates CAMT054.

The INTEGRATION.SERVICE TSA.SERVICE must run to emit the messages through Integration Framework to the Delivery Transformation Layer.

Read the Configuring MX Messages through SWIFT Interact Services section for more information on the technical and business header configuration, message name variants and payload transformation.

After the message is emitted through Integration Framework, the Status field in DE.DELIVERY.REQUEST.LISTENER is changed to Routed. If the target carrier is not an XMLISO carrier, the Status field in DE.DELIVERY.REQUEST.LISTENER is changed to Repair and the message is not processed further.

> **⚠️ Note:** Standard archiving is used for the messages with the Routed or Repair status.


##### Transforming the MTXML Message into the Final Format

The Delivery Transformation Layer picks the message from the queue identified by the DeRequestListenerQueue property attribute (configured in the DE_SWIFTOutward_QueueConfig Delivery Transformation property file), where DE.DELIVERY.REQUEST.LISTENER has emitted the message.

The Delivery Transformation Layer applies the transformation rule indicated in the header of the message transforming the payload from the generic MTXML format to the ISO20022 format. Read the Delivery Carrier Configuration section for more information regarding the CBPRPLUS Delivery Carrier configuration.

The Delivery module applies the header transformations, generates the local authentication code (LAU) and appends them to the final ISO20022 message. Read the Outward Processing section for information on this processing.


##### Emitting the ISO20022 Message to the Final Integration Queue

Delivery emits the ISO20022 message to the integration queue. Read the Configuring MX Messages through SWIFT Interact Services section to understand the configuration of the integration queue. Temenos SWIFT Interact Connector picks the message from the integration queue and sends that to the SWIFT Alliance queues and folders.


#### 📋 Tasks

There are no Tasks for the Translate Advices and Account Reporting MT Messages to CBPR+ feature.


#### 📊 Outputs

There are no Outputs available for the Translate Advices and Account Reporting MT Messages to CBPR+ feature.

---


---


## Chapter 4: Customer_Output - IX


Customer_Output - IX module of Temenos Transact


### Features in Customer_Output - IX


| # | Feature | Sections |
|---|---------|----------|
| 4.1 | Archiving XML Statement Related Tables | Intro, Confi, Tasks, Outpu |
| 4.2 | Camt.53 and Camt.54 Statement Summary | Intro, Confi, Tasks, Outpu |
| 4.3 | Camt Generation Process | Intro, Confi, Tasks, Outpu |
| 4.4 | Camt XML Message Production | Intro, Confi, Tasks, Outpu |
| 4.5 | Changes in Camt Processing to Improve Performance | Intro, Confi, Tasks, Outpu |
| 4.6 | Exception Handling of Camt Messages | Intro, Confi, Tasks, Outpu |
| 4.7 | Generation of a Camt Message to Multiple Recipients | Intro, Confi, Tasks, Outpu |
| 4.8 | Misc | Intro |
| 4.9 | User-Definable Content of the Camt Message | Intro, Confi, Tasks, Outpu |


### 4.1  Archiving XML Statement Related Tables


> **📇 Quick Reference Card**
> 
> **Purpose:** *The T24 archiving process supports the following XML statement related tables:*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The T24 archiving process supports the following XML statement related tables:

- XML.OUTPUT.MSG
- AC.XML.STMT.DATA
- AC.XML.STMT.EXCEPTION
- EXTERNAL.SEPA.DETAILS


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

There are no Tasks available for Archiving of XML Statement Related Tables feature.


#### 📊 Outputs

There are no Outputs available for Archiving of XML Statement Related Tables feature.

---


### 4.2  Camt.53 and Camt.54 Statement Summary


> **📇 Quick Reference Card**
> 
> **Purpose:** *Both the Camt.053 and Camt.054 are ISO20022 standard account reports based on movements across the account over a specified period of time. They are produced in regular frequencies agreed with the customer.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Both the Camt.053 and Camt.054 are ISO20022 standard account reports based on movements across the account over a specified period of time. They are produced in regular frequencies agreed with the customer.

Camt.053 – This is an account statement that contains all movements (entries may be consolidated into a single entry) for the statement period and includes the opening and closing balance.

Camt.054 – This is a report of the selected transactions processed across the account during the requested period, and does not include the account balances.

The client provides two distinct variations of camt.054 for their customers:

- Payment list report
- Incoming reference report

The option to show complete or partial details of the bulk transactions is based on the message type. The level of reporting detail required, either complete or detailed, is requested as part of the transaction.

Since both the types of reports are generated for an account based on the movement over a period to the same message schema, the mechanism already available in Temenos Transact to produce a camt.053 is used to generate a camt.054 also.

SEPA details mapping in camt statements is essential–

- For banks that participate in SEPA, C2B and other payments (substituting for the ordering party or the beneficiary), are required to generate camt.054, 053 or 052 electronic statements, if requested by the account holding customer or bank.
- From February 1 2014, this capability is mandatory in many European countries.
- Temenos Transact provides the ability to generate a camt.054, camt.053 or camt.052 statement message for accounts.


#### ⚙️ Configuration


##### Configuration to get Entry Information from External SEPA System through an API

To link the STMT.ENTRY record to the EXTERNAL.SEPA.DETAILS , a hook is available to attach a local API with the logic for the link. The API returns the ID to the EXTERNAL.SEPA.DETAILS application.

The External SEPA Link API field in AC.STMT.PARAMETER is the hook that gets the link from the entry to the EXTERNAL.SEPA.DETAILS application. It is a valid ID of EB.API to hold the API that returns the link ID to the EXTERNAL.SEPA.DETAILS application.


##### Configuration to get SEPA details fromTemenos TransactSEPA system

The following configurations are required to get the SEPA details from Temenos Transact SEPA entries:

INWARD.110 INWARD.210 and INWARD.213. The layout record is modified to map the payment participant’s additional information to SEPA.PAYM.PARTICIPANTS application, for the PAIN message. This functionality is available for PACS message.

| FIELD | VALUE |
|---|---|
| Validation Rtn | @SEPA.WRITE.PAYM.PARTICIPANTS |

- OUTWARD.111, OUTWARD.221 and OUTWARD.222

The layout is modified to map the data correctly to the outward xml message.

The following screenshot shows an example of the XML.TAG.DEFINITION with the Transaction Ref as EntryDetails.Batch.Details.

The following screenshot shows an example of the XML.TAG.DEFINITION with ID as TxnDet.Details.

The following screenshot shows an example of ACCOUNT.STATEMENT application.

The following screenshot shows an example of FUNDS.TRANSFER application.

The XML.TRANSFORMATION service is run to produce the output.


#### 📋 Tasks

There are no Tasks available for Camt.53 and Camt.54 Statement Summary – SEPA Details Mapping feature.


#### 📊 Outputs

There are no Outputs available for Camt.53 and Camt.54 Statement Summary – SEPA Details Mapping feature.

---


### 4.3  Camt Generation Process


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Camt Generation Process involves the following sequence:*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The Camt Generation Process involves the following sequence:

1. Request and Trigger for camt statement
2. Assembling Statement content
3. Transformation of Data


#### ⚙️ Configuration

Covered as part of module configuration and there is no specific configuration for this feature.


#### 📋 Tasks

There are no Tasks available for Camt Genration Process feature.


#### 📊 Outputs

There are no Outputs available for Camt Genration Process feature.

---


### 4.4  Camt XML Message Production


> **📇 Quick Reference Card**
> 
> **Purpose:** *Temenos has provided a standard transformation (XSLT) of the Temenos Transact schema to ISO20022 camt schema.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Temenos has provided a standard transformation (XSLT) of the Temenos Transact schema to ISO20022 camt schema.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

There are no Tasks available for Camt XML Message Production feature.


#### 📊 Outputs

There are no Outputs available for Camt XML Message Production feature.

---


### 4.5  Changes in Camt Processing to Improve Performance


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Cash Management Messages (camt) such as camt.052 (intraday message), camt.053 and camt.054 are produced in Temenos Transact :*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The Cash Management Messages (camt) such as camt.052 (intraday message), camt.053 and camt.054 are produced in Temenos Transact :

- Camt.052 can be generated online.
- Camt.053 and camt.054 are generated during COB.

This functionality improves system performance during the generation of these messages, by de-linking IF and using the concept of segmentation.


#### ⚙️ Configuration

The following setup is required to enable this functionality:

1. The DE.ADDRESS record must be created for the carrier named ISOREPORT.
2. The DE.PRODUCT must be created.
3. In ACCOUNT.STATEMENT , the message type that must be produced must be given.
4. In AC.STMT.PARAMETER , additional parameterisation can be done for each message type, like adding local API to filter certain entries. The local API consolidates the entries. Also, there is a field to attach the local APIs which add local tags.


#### 📋 Tasks

There are no Tasks available for Changes in Camt Processing to Improve Performance feature.


#### 📊 Outputs

There are no Outputs available for Changes in Camt Processing to Improve Performance feature.

---


### 4.6  Exception Handling of Camt Messages


> **📇 Quick Reference Card**
> 
> **Purpose:** *The transformation process updates the AC.XML.STMT.EXCEPTION exception table for the messages that have failed. This table holds the details of the unsuccessful camt xml messages, and provides the reasons for the message failure. It is possible to resubmit a failed message for which the Temenos Tran...*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

The transformation process updates the AC.XML.STMT.EXCEPTION exception table for the messages that have failed. This table holds the details of the unsuccessful camt xml messages, and provides the reasons for the message failure. It is possible to resubmit a failed message for which the Temenos Transact xml format is produced.


#### ⚙️ Configuration

This is covered as part of module configuration. There is no specific configuration for this feature.


#### 📋 Tasks

There are no Tasks available for Exception Handling of CAMT Messages feature.


#### 📊 Outputs

There are no Outputs available for Exception Handling of CAMT Messages feature.

---


### 4.7  Generation of a Camt Message to Multiple Recipients


> **📇 Quick Reference Card**
> 
> **Purpose:** *A camt message is sent to the account owner and it can also be sent to a third party authorised by the account owner to receive the message. On request from the account owner, a copy of the camt.053 message can be sent to multiple recipients.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

A camt message is sent to the account owner and it can also be sent to a third party authorised by the account owner to receive the message. On request from the account owner, a copy of the camt.053 message can be sent to multiple recipients.


#### ⚙️ Configuration

The recipients of a camt message can be defined using the carrier functionality in Temenos Transact . The carrier used for the camt messages is ISOREPORT.

DE.ADDRESS application is used to define recipient’s addresses. For camt statements, it is possible to provide the correct identifier for the customer as the destination (carrier) for the camt message, without having to define additional customer records for Temenos Transact .

Temenos Transact uses the DE.CUSTOMER.PREFERENCES and DE.PRODUCT applications to define the recipients of a particular message.

For account statements, it is possible to specify the recipient for a particular statement cycle and message type. This functionality allows multiple recipients to be specified based on the type of message and cycle for all types of statements.

The DE.PRODUCT application is used to define any additional recipients for the camt message using the Additional Recipient field for the SWIFT carrier.

> **⚠️ Note:** Defining additional recipients does not change any functionality to the SWIFT statement processing.

The following screenshot shows how an additional recipient is added in the DE.PRODUCT record for the camt message under the ISOREPORT carrier, using the account owner’s customer identifier and the customer identifier of another customer.


#### 📋 Tasks

There are no Tasks available for Generation of a Camt Message to Multiple Recipients feature.


#### 📊 Outputs

There are no Outputs available for Generation of a Camt Message to Multiple Recipients feature.

---


### 4.8  Misc


> **📇 Quick Reference Card**
> 
> **Purpose:** *The camt.053 (Bank to Customer Statement) message is a statement of account(s) sent by the bank to account holding customer (or nominated representative) on a periodic basis. The message format is one of the family of cash management messages (camt) of the ISO20022 (also known as UNIFI) standard. Th...*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Related topics:

- Temenos Transact Services

The camt.053 (Bank to Customer Statement) message is a statement of account(s) sent by the bank to account holding customer (or nominated representative) on a periodic basis. The message format is one of the family of cash management messages (camt) of the ISO20022 (also known as UNIFI) standard. The camt.052 message is an intraday version of the camt.053, only showing movements generated since the last generation of camt.052 or camt.053.

Banks that participate in Single Euro Payments Area (SEPA) payments (either credit transfer or direct debit) acting for the ordering party or the beneficiary must be able to generate the camt.053 or camt.052 electronic statement if requested by the account holding customer or bank. The format must include complete details of the SEPA payment in the statement detail and details of other non-SEPA financial transactions.

This capability is mandatory in many European countries from February 1, 2014.

- The camt.053 and camt.052 are part of the cash management messages set by ISO20022 using an XML based schema.
- The camt.053 (Bank to Customer Statement) is sent by the bank to an account owner or a party authorised by the account owner on a periodic basis.
- The camt.052 (Bank to Customer Account report) is used for intra-day account reporting upon request by the account owner.

The CAMT messages are the ISO20022 equivalent of the MT9nn series:

- Camt.053 is the ISO20022 equivalent of MT940, which is sent by the bank to the account holder on a periodic basis.
- Camt.052 is the IS020022 equivalent of MT942 or MT941, which is an intraday version of the camt.053.


##### Product Configuration

The camt solution is packaged into the Temenos Transact ISO20022 XML Account Statement Module (IX - ISO20022 Statement). The IX product must be installed to use the camt statement functionality.

The camt message produced by Temenos Transact is aligned with the Dutch-specific usage rules, as set by the Dutch Banking Association (NVB).

The NVB guidelines include the usage rules for the reporting of SEPA credit transfers and Single Euro Payments Area (SEPA) direct debits. The SEPA details required under NVB are reported in the camt statement if the required information is available in Temenos Transact .

> **⚠️ Note:** Other country-specific regulations need to be requested with requirements to evaluate if those usage rules can be accommodated.

A camt message has a nested structure with the building blocks as shown in the image below. The Temenos Transact Camt module is responsible to assemble the data necessary to produce a camt message for each statement triggered.

The camt.053 and the camt.052 messages both have the same structure, except that the header name is different.

- Camt.053 message has the following structure:

Bank to Customer Statements:

- Camt.052 has the following structure:

Bank to Customer Account Report:

- Group Header Report Entry Transaction details

The following image shows the structure of a camt.053 message.

- Group Header (Statement Level Information):

The Group Header block of the camt message provides the information related to the statement and is specified for the camt message. This section of the message is mandatory.

It contains information like Message Identification, Pagination, Message Recipients and so on.

> **⚠️ Note:** Group Header block is mandatory and is specified only once for the camt message.

- Statement or Report (Account Level Information):

The Statement section of the camt message provides the details of the account(s) for which the statement(s) is being produced.

The camt message may contain information related to more than one account statement. However, Temenos Transact is producing one camt message for a single account statement.

Details required at this level are built from the Temenos Transact account and related statement production details. This includes details of the statement period, account identification, opening, closing and other account balances.

> **⚠️ Note:** Statement section is mandatory and may occur multiple times in the camt message.

- Entry-Level Information:

One account statement can contain multiple account movements (a statement may have zero entries during the period). Information at this level is derived from the individual account movement from the Temenos Transact statement entry table.

> **⚠️ Note:** Entry Level section is optional and may occur multiple times in the camt message.

Transaction-Level Information:

This section provides additional information for each entry displayed in the Entry Level section. The additional information may include:

- Additional details for an individual entry.
- Additional details for SEPA related transactions.
- Underlying entries of a netted entry which represents multiple debits and credits or a batch entry (this will be supported at a later stage).

> **⚠️ Note:** Transaction Level information section is optional and may occur multiple times in the camt message.

The following screenshot shows the xml view of the camt.053 message.

This table is used to define the default details for an account statement when opening new accounts. It also holds the high-level parameter that is applicable to account statement at the system level.

The AC.STMT.PARAMETER application is also used to define the following:

- Provide the link between an entry and the EXTERNAL.SEPA.DETAILS table, which would hold the SEPA details from an external SEPA system.
- Provide a hook to plug-in APIs to filter and consolidate the list of entries for a specific camt message.

Link between the Entry and the EXTERNAL.SEPA.DETAILS table:

To identify the corresponding EXTERNAL.SEPA.DETAILS record that holds the SEPA details for a STMT.ENTRY , the STMT.ENTRY and the EXTERNAL.SEPA.DETAILS record should be linked.

A hook is available based on each implementation to attach a local API with the logic to link the STMT.ENTRY record to the EXTERNAL.SEPA.DETAILS . The API returns the key to the EXTERNAL.SEPA.DETAILS table.

The External SEPA Link API field in AC.STMT.PARAMETER application is the hook that gets the link from the entry to the EXTERNAL.SEPA.DETAILS table. It is a valid key to EB.API to hold the API that returns the link key to the EXTERNAL.SEPA.DETAILS table.

Different variations of the camt.054 message are generated by filtering the list of entries to be reported. A filter API is invoked to exclude entry details based on the criteria the bank requires.

Entries for the statement or report period are combined into consolidated entries for the statement. The criteria and consolidation method used is determined by message types and decisions made through an API routine. This consolidates entries together according to the required rules and ensures that the consolidated entry is shown in the statement.

The following screenshot shows the hook in AC.STMT.PARAMETER to plug-in an API to return the link between the entry and the EXTERNAL.SEPA.DETAILS table.

The camt account statements and reports are generated using the standard account statement functionality.

ACCOUNT.STATEMENT table is used to specify the dates and frequencies for producing account statements. A record is automatically created with the default settings when an account is set-up. It can then be defined specifically for each account based on the customer’s requirements. User can define up to nine statement cycles, and within each cycle, a combination of different types of messages can be generated.

The Xml Stmt Type field in the ACCOUNT.STATEMENT application is used to request a camt or MT type message for the first cycle for an account.

The Swift Statement-2 Type field is used to define the message types for the additional statement cycles.

The following screenshot shows the set-up for camt and MT type messages for two statement cycles.

| Camt Index | Description | User Configurable |
|---|---|---|
|  | Group Header |  |
| 1.1 | Message Identification | Y |
| 1.2 | CreationDateTime |  |
|  | Statement |  |
| 2.1 | Identification | Y |
| 2.4 | CreationDateTime |  |
| 1.2.1 | IBAN |  |
| 1.2.2 | OtherId | Y |
| 2.24 | Code |  |
| 2.34 | Amount |  |
| 2.35 | CreditDebitIndicator |  |
| 2.36 | Date |  |
| 2.78 | Amount |  |
| 2.79 | CreditDebit Indicator |  |
| 2.81 | Status |  |
| 2.91 | Proprietary | Y |
| 2.99 | Issuer | Y |

---


### 4.9  User-Definable Content of the Camt Message


> **📇 Quick Reference Card**
> 
> **Purpose:** *To facilitate the banks to adhere to local regulation and practice, a flexible mechanism is available to configure the content of the camt message. The following locally defined logic is used to configure the camt message:*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

To facilitate the banks to adhere to local regulation and practice, a flexible mechanism is available to configure the content of the camt message. The following locally defined logic is used to configure the camt message:

- Ability to filter the list of entries for a specific camt message type.
- Ability to consolidate a list of selected entries to be reported as one entry.
- Ability to suppress a data tag or a group of data tags.
- Ability to configure the content of a data tag or a group of data tags.


#### ⚙️ Configuration


##### Filtering Entry Content

The Filter Routine field in AC.STMT.PARAMETER allows the entry list for the report cycle to be filtered. A filter API can be invoked by the statement processor that will be able to exclude entry detail based on the criteria required by the bank. This will allow the inclusion and exclusion of information based on the recipient receiving the report. It is typically used to restrict the list of entries reported under camt.054 (Debit or Credit notification).

The API is passed at the entry, and it returns a flag to indicate if the entry can be included in the account report. A test API, IX.TEST.FILTER.RTN, has been released as an example of how the API should be built.

The following screenshot shows the set-up to plug-in an API to filter the entries for camt.054 account report.


##### Consolidating Selected Entries

Entries for the period under consideration can be combined into consolidated entries for the statement. The criteria and consolidation method used is determined by message type and the decision is made through an API routine. The Consolidate Routine field in AC.STMT.PARAMETER provides the hook to plug in the API. This will consolidate entries together according to the required rules and ensure that the consolidated entry is shown in the statement.

The default consolidation grouping uses the following elements from the entry:

- System ID
- Transaction Code
- Booking Date
- Reversal Marker

The API is passed to the entry and the consolidation group. The API can alter or clear the consolidation group. It can also change the transaction code, if a specific transaction code is preferred for a consolidated entry. This allows the system to show a specific transaction description in the camt message.

While the statement shows the consolidated entry in the statement, the actual entries are held in detail in the system. This is typically used when an account report is generated for a selected list of entries with all the details, but in the statement, the entries are reported as one consolidated entry. A test API, IX.TEST.CONSOLIDATE.RTN, is released as an example of how the API is built.

The following screenshot shows how an API may be plugged in to consolidate entries for a camt.053 account statement:


##### Suppressing Information

The XML.TAG.DEFINITION application allows an individual tag or group of tags defined as Optional under camt, to be suppressed for a specific message type or entry from a specific application. Additionally, it is possible to make more complex suppression decisions through a developed API routine to handle specific bank’s criteria.

The following screenshot shows the suppression set-up for a group tag for batch details. The suppression can be set by default for the group, or by message type as shown here, or under the application or transaction type for the message type. The following image shows the suppression for camt.053 by setting the Suppress Flag as Yes and for camt.054a, the suppression is based on a logic defined in SUPP.BATCH.DTLS API.

The following screenshot shows how the suppression set-up for a data tag can be defined.


##### Configuring the content of Data Tags

The content of a tag group or individual data tags may be required to meet local regulation or banks’ requirements.

Users can configure either a group tag or an individual data tag as explained below.

| Group.Tag | Child.Group | Child Tag |
|---|---|---|
| Header.Recipient.Details |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
| Balance.Details | Balance.Amt.Details |  |
|  |  |  |
|  |  |  |
|  |  |  |
| Balance.CredLine.Details |  |  |
|  |  |  |
| Entry.Details | Batch.Details |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  | Transaction.Details | All Txn.Det tags |

| Data Source | Source Value |
|---|---|
| API | @XXXX, where XXXX is a valid API and recorded in EB.API. |
| VALUE | It is a fixed value |


#### 📋 Tasks

There are no Tasks available for User-Definable Content of the Camt Message feature.


#### 📊 Outputs

There are no Outputs available for User-Definable Content of the Camt Message feature.

---


---


## Appendix A: Glossary of T24 Applications & Fields


This glossary lists all T24/Transact application names and field names referenced throughout this document, with descriptions where available.


### Applications


| Application | Description |
|------------|-------------|
| `)` | T24 application: ) |
| `,` | T24 application: , |
| `.HEADER` | T24 application: .HEADER |
| `ADDRESS` | T24 application: ADDRESS |
| `ARCHIVE` | T24 application: ARCHIVE |
| `ASCII.VAL.TABLE` | T24 application: ASCII.VAL.TABLE |
| `ASCII.VALUES` | T24 application: ASCII.VALUES |
| `BATCH` | T24 application: BATCH |
| `BENEFICIARY` | T24 application: BENEFICIARY |
| `CARRIER` | T24 application: CARRIER |
| `COMPANY` | T24 application: COMPANY |
| `CONTROL` | T24 application: CONTROL |
| `CREATE.FILES` | T24 application: CREATE.FILES |
| `CUSTOMER` | T24 application: CUSTOMER |
| `DE` | T24 application: DE |
| `DE.ADDRESS` | T24 application: DE.ADDRESS |
| `DE.ADDRESS PRINT.1` | T24 application: DE.ADDRESS PRINT.1 |
| `DE.ALT.CHARS` | T24 application: DE.ALT.CHARS |
| `DE.ALTERNATE` | T24 application: DE.ALTERNATE |
| `DE.AUTO.TRANSLATION` | T24 application: DE.AUTO.TRANSLATION |
| `DE.BATCH.GROUP` | T24 application: DE.BATCH.GROUP |
| `DE.BIC` | T24 application: DE.BIC |
| `DE.BUSINESS.SERVICE.RULES` | T24 application: DE.BUSINESS.SERVICE.RULES |
| `DE.CARRIER` | T24 application: DE.CARRIER |
| `DE.CC.GENERIC` | T24 application: DE.CC.GENERIC |
| `DE.CUSTOMER.PREFERENCES` | T24 application: DE.CUSTOMER.PREFERENCES |
| `DE.DELIVER.REQUEST.LISTENER` | T24 application: DE.DELIVER.REQUEST.LISTENER |
| `DE.DELIVERY.REQUEST.LISTENER` | T24 application: DE.DELIVERY.REQUEST.LISTENER |
| `DE.DELIVERY.RESPONSES` | T24 application: DE.DELIVERY.RESPONSES |
| `DE.DISP` | T24 application: DE.DISP |
| `DE.DISP.CONTROL` | T24 application: DE.DISP.CONTROL |
| `DE.DISP.TIMECHECK` | T24 application: DE.DISP.TIMECHECK |
| `DE.DISTINGUISH.NAME.RULES` | T24 application: DE.DISTINGUISH.NAME.RULES |
| `DE.DLN.REQUIREMENTS` | T24 application: DE.DLN.REQUIREMENTS |
| `DE.FORM.TYPE` | T24 application: DE.FORM.TYPE |
| `DE.FORMAT.CARRIER` | T24 application: DE.FORMAT.CARRIER |
| `DE.FORMAT.PRINT` | T24 application: DE.FORMAT.PRINT |
| `DE.FORMAT.PRINT, DE.FORMAT.SWIFT` | T24 application: DE.FORMAT.PRINT, DE.FORMAT.SWIFT |
| `DE.FORMAT.SWIFT` | T24 application: DE.FORMAT.SWIFT |
| `DE.FORMAT.TELEXF` | T24 application: DE.FORMAT.TELEXF |
| `DE.FORMAT.TELEXP` | T24 application: DE.FORMAT.TELEXP |
| `DE.FORMAT.TEMPLATE` | T24 application: DE.FORMAT.TEMPLATE |
| `DE.FORMAT.XML` | T24 application: DE.FORMAT.XML |
| `DE.FORMAT.format.carrier` | T24 application: DE.FORMAT.format.carrier |
| `DE.I.HEADER` | T24 application: DE.I.HEADER |
| `DE.I.HEADER.ARCH` | T24 application: DE.I.HEADER.ARCH |
| `DE.I.HEADERorDE.O.HEADER` | T24 application: DE.I.HEADERorDE.O.HEADER |
| `DE.I.SUBROUTINE.TABLE` | T24 application: DE.I.SUBROUTINE.TABLE |
| `DE.INTERFACE` | T24 application: DE.INTERFACE |
| `DE.INWARD.ROUTING` | T24 application: DE.INWARD.ROUTING |
| `DE.MAPPING` | T24 application: DE.MAPPING |
| `DE.MESSAGE` | T24 application: DE.MESSAGE |
| `DE.MESSAGE.CONCAT` | T24 application: DE.MESSAGE.CONCAT |
| `DE.MESSAGE.HEADER` | T24 application: DE.MESSAGE.HEADER |
| `DE.MM.DISPLAY` | T24 application: DE.MM.DISPLAY |
| `DE.MM.I.END.OF.PERIOD` | T24 application: DE.MM.I.END.OF.PERIOD |
| `DE.MM.O.END.OF.PERIOD` | T24 application: DE.MM.O.END.OF.PERIOD |
| `DE.MM.SETUP.TRANSLATION` | T24 application: DE.MM.SETUP.TRANSLATION |
| `DE.MM.SYS.CLEAR` | T24 application: DE.MM.SYS.CLEAR |
| `DE.MSG.CHARS.RULE` | T24 application: DE.MSG.CHARS.RULE |
| `DE.MT941.SENT.ENTRIES` | T24 application: DE.MT941.SENT.ENTRIES |
| `DE.MT942.REQUEST` | T24 application: DE.MT942.REQUEST |
| `DE.MT942.SENT.ENTRIES` | T24 application: DE.MT942.SENT.ENTRIES |
| `DE.O.HANDOFF` | T24 application: DE.O.HANDOFF |
| `DE.O.HEADER` | T24 application: DE.O.HEADER |
| `DE.O.HEADER.ARCH` | T24 application: DE.O.HEADER.ARCH |
| `DE.O.HOLD.KEY` | T24 application: DE.O.HOLD.KEY |
| `DE.O.MSG.GLOBUSTLX` | T24 application: DE.O.MSG.GLOBUSTLX |
| `DE.PARAM` | T24 application: DE.PARAM |
| `DE.PARM` | T24 application: DE.PARM |
| `DE.PRINT` | T24 application: DE.PRINT |
| `DE.PRODUCT` | T24 application: DE.PRODUCT |
| `DE.SENT.SWIFT` | T24 application: DE.SENT.SWIFT |
| `DE.SENT.TELEX` | T24 application: DE.SENT.TELEX |
| `DE.SWIFT.DIVERSION` | T24 application: DE.SWIFT.DIVERSION |
| `DE.TRANSLATION` | T24 application: DE.TRANSLATION |
| `DE.UETR.CATALOG.LIST` | T24 application: DE.UETR.CATALOG.LIST |
| `DE.UETR.REF.FILE` | T24 application: DE.UETR.REF.FILE |
| `DE_SWIFTInward_InwardIntegrity.properties` | T24 application: DE_SWIFTInward_InwardIntegrity.properties |
| `DE_SWIFTInward_QueueConfig.properties` | T24 application: DE_SWIFTInward_QueueConfig.properties |
| `DE_SWIFTOutward_OutwardIntegrity.properties` | T24 application: DE_SWIFTOutward_OutwardIntegrity.properties |
| `DE_SWIFTOutward_QueueConfig` | T24 application: DE_SWIFTOutward_QueueConfig |
| `EB.COMPONENT` | T24 application: EB.COMPONENT |
| `EB.FREE.MESSAGE` | T24 application: EB.FREE.MESSAGE |
| `EB.LOOKUP` | T24 application: EB.LOOKUP |
| `EB.PRODUCT` | T24 application: EB.PRODUCT |
| `EB.QUERIES.ANSWERS` | T24 application: EB.QUERIES.ANSWERS |
| `F.LOCKING` | T24 application: F.LOCKING |
| `FT.APPL.DEFAULT` | T24 application: FT.APPL.DEFAULT |
| `FUNDS.TRANSFER` | T24 application: FUNDS.TRANSFER |
| `HOLD.CONTROL` | T24 application: HOLD.CONTROL |
| `I` | T24 application: I |
| `IF.EXIT.POINTS` | T24 application: IF.EXIT.POINTS |
| `IF.INTEGRATION.FLOW.CATALOG` | T24 application: IF.INTEGRATION.FLOW.CATALOG |
| `IF.INTEGRATION.SERVICE.PARAM` | T24 application: IF.INTEGRATION.SERVICE.PARAM |
| `INTERFACE` | T24 application: INTERFACE |
| `INWARD.OFS.RTN` | T24 application: INWARD.OFS.RTN |
| `InwardGenericOfsConversion.xslt` | T24 application: InwardGenericOfsConversion.xslt |
| `LANGUAGE` | T24 application: LANGUAGE |
| `LOCKING` | T24 application: LOCKING |
| `MAPPING` | T24 application: MAPPING |
| `MD.DEAL` | T24 application: MD.DEAL |
| `MESSAGE` | T24 application: MESSAGE |
| `OFS` | T24 application: OFS |
| `OFS.SOURCE` | T24 application: OFS.SOURCE |
| `P` | T24 application: P |
| `PGM.FILE` | T24 application: PGM.FILE |
| `POR.TRANSACTION` | T24 application: POR.TRANSACTION |
| `PP.NO.RMA` | T24 application: PP.NO.RMA |
| `PP.RMA` | T24 application: PP.RMA |
| `PRINT.CUST.OUTPUT` | T24 application: PRINT.CUST.OUTPUT |
| `PRINT.OUT` | T24 application: PRINT.OUT |
| `PRINTER.ATTRIBUTES` | T24 application: PRINTER.ATTRIBUTES |
| `PRINTER.ID` | T24 application: PRINTER.ID |
| `PRODUCT` | T24 application: PRODUCT |
| `QueueConfigMXOutward.properties` | T24 application: QueueConfigMXOutward.properties |
| `RMA.FILE.UPLOAD.DETAILS` | T24 application: RMA.FILE.UPLOAD.DETAILS |
| `RMA.PARAMETER` | T24 application: RMA.PARAMETER |
| `RMA.PARAMTER` | T24 application: RMA.PARAMTER |
| `RODUCT` | T24 application: RODUCT |
| `SEC.ACC.MASTER` | T24 application: SEC.ACC.MASTER |
| `SERVICE` | T24 application: SERVICE |
| `SFCONF.CONFIRMATION.TRACKER` | T24 application: SFCONF.CONFIRMATION.TRACKER |
| `SFCONF.TRACKER.STATUS.REASON` | T24 application: SFCONF.TRACKER.STATUS.REASON |
| `SPF` | T24 application: SPF |
| `STANDING.ORDER` | T24 application: STANDING.ORDER |
| `SWIFT.CODE.WORDS` | T24 application: SWIFT.CODE.WORDS |
| `SWIFT.IN` | T24 application: SWIFT.IN |
| `SWIFT.OUT` | T24 application: SWIFT.OUT |
| `SWIFT.PARAMETER` | T24 application: SWIFT.PARAMETER |
| `SWIFT.PARMETER` | T24 application: SWIFT.PARMETER |
| `TPS.INTERNAL.CONFIGS` | T24 application: TPS.INTERNAL.CONFIGS |
| `TSA` | T24 application: TSA |
| `TSA.SERVICE` | T24 application: TSA.SERVICE |
| `TSA.WORKLOAD.PROFILE` | T24 application: TSA.WORKLOAD.PROFILE |
| `Tracker Status Reason` | T24 application: Tracker Status Reason |
| `USER` | T24 application: USER |
| `VERSION` | T24 application: VERSION |
| `XSD_ROOT_DIR` | T24 application: XSD_ROOT_DIR |
| `XSLT_ROOT_DIR` | T24 application: XSLT_ROOT_DIR |
| `theDE.FORMAT.PRINT` | T24 application: theDE.FORMAT.PRINT |


### Fields Referenced


| Field | Field | Field |
|-------|-------|-------|
| `).` | `320.MM1030.20.FR` | `Account With Bank` |
| `Ack` | `Ack Required` | `AckNackTemenosFormatXsd` |
| `Address` | `Address Attribute` | `Address Country` |
| `Address Purpose` | `Address Type` | `Address Validated By` |
| `Allow` | `Allow Hold` | `Alter Char Code` |
| `Amount Credited` | `Api Output Format` | `App Context Field` |
| `App Context Field.` | `App Context Value` | `App Pde` |
| `Application` | `Application Format` | `Apply Address Rules` |
| `Arc Filename` | `Archive Data` | `Assoc` |
| `Audit Seq Checking` | `Auto Pay Acct` | `Auto Process Limit` |
| `Autoroute Agrd` | `Autoroute Bank` | `Awack` |
| `BROKER` | `Back Value Max` | `Basic Header (1)-` |
| `Basic header (1)-` | `Batching Req` | `Ben Acct No` |
| `Ben Address` | `Ben Country` | `Ben Country Ben Town` |
| `Ben Customer` | `Ben Name` | `Ben Name 1` |
| `Ben Name 2` | `Ben Name 3` | `Ben Town` |
| `Beneficiary Bank` | `Bic Code` | `Bk To Bk Out` |
| `Block` | `Building Name` | `Building Number` |
| `Business Application` | `Business Service` | `C` |
| `Calculation` | `Cancellation Code` | `Carrier` |
| `Carrier Addr No` | `Carrier Address No` | `Carrier Module` |
| `Carrier Type` | `Centralised Ft` | `Cet` |
| `Cet Time Diff` | `Char Position` | `Charge Types` |
| `Chg Com On Err` | `Claim Charges Acct` | `Code` |
| `Coll Rem Bk` | `Comm Types` | `Company` |
| `Complete` | `Cond` | `Confid` |
| `Confirmed Amount` | `Confirmed Amt` | `Confirmed Ccy` |
| `Confirmed Currency` | `Control` | `Conversion` |
| `Copies` | `Country` | `Country Subdivision` |
| `Cr Floor Limit` | `Credit Amount` | `Credit Currency` |
| `Curr Swift Rel` | `Currency fields` | `Current Release` |
| `Cust` | `Customer` | `Customer No` |
| `Customer Number` | `Customer, Address, Message Type and Currency` | `Customer/Account Number` |
| `Cut Off Rule` | `Cut Off Time` | `D` |
| `DEHandoffQueue` | `DEMXTRHandoffQueue` | `Data` |
| `Date` | `Db A Cr Max Days` | `Db After Cr` |
| `De Format Conversion` | `DeRequestListenerQueue` | `Debit account` |
| `Def Alt Char Code` | `Def Corr Bank Chgs` | `Def Funds Diversion` |
| `Default Output Fmt` | `Default To Addr Out Fmt` | `DefaultQueue` |
| `Delete` | `Delivery Message` | `Delivery Out Header Id` |
| `Delivery Reference` | `DeliveryReportXslt` | `Department` |
| `Depend` | `Depend Cond` | `Depend Operand` |
| `Dependent` | `Dependent On` | `Description` |
| `Det` | `Detail` | `Dets` |
| `Diff` | `Dir` | `Direction` |
| `Disposition` | `Disposition Control` | `Disposition No` |
| `Distinguish Name` | `Distinguish Name Rule -` | `District Name` |
| `Dln Requested` | `Domain` | `Domain, Business Service` |
| `Effective Date` | `End Date` | `Eop` |
| `Err` | `Error` | `Error Code` |
| `Event Dest` | `Event Type` | `Exclude Message Type` |
| `Expected Recs` | `Ext Cust Id` | `Ext User Id` |
| `F` | `FIELD/"TEXT"` | `Field` |
| `Field Name` | `Field Text` | `Field text` |
| `File` | `File Pathname` | `Flat` |
| `Flat Amount` | `Flat Number` | `Fld` |
| `Floor` | `Form` | `Form Type` |
| `Format` | `Format Module` | `Formatting Module` |
| `Forw Value Max` | `Fwd Msg Type` | `Fwd Uetr Message Type` |
| `GB Notes` | `Gen942 Independently` | `Gts` |
| `Hdr 3 Uetr` | `Header` | `Header Name` |
| `Header Version` | `Heading` | `His Reversal` |
| `History` | `Hold` | `Hold End Date` |
| `Hold Mail End` | `Hold Mail Opt` | `Hold Mail Start` |
| `Hold Option` | `Hold Options` | `Hold Output` |
| `Hold Start Date` | `Hold Until Date` | `IN Account With Bank` |
| `ISO Cancel Reason Code` | `Idd Prefix Phone` | `In` |
| `In Bk To Bk` | `In C Bk T Bk In` | `In Chg Code` |
| `In Hdr 3 Uetr` | `In Msg Post Method` | `In Msg Queue` |
| `Indent` | `Inf` | `Integration Queue` |
| `Interface` | `Intermediary Institution (Tag 56)` | `Invalid Msg Type` |
| `Invalid SWIFT Message Type` | `Inw Head Trail` | `Inward` |
| `Inward Ofs Rtn` | `Job Name` | `LINE(S)` |
| `Language` | `Last Eff Change` | `Last Page Indicator` |
| `Last Run` | `Lcl Hdr Element Api` | `Length` |
| `Less Charges Limit` | `Level` | `Line S` |
| `Line S)` | `Local Char Code` | `Local Ref` |
| `Log` | `Maint` | `Maintain` |
| `Mandatory` | `Manual Prev Swift Rel` | `Mapping Api` |
| `Mask` | `Max Length` | `Maximum Lines` |
| `Mdr Customer` | `Member Id` | `Message` |
| `Message Disposition` | `Message Name Id` | `Message Type` |
| `MessageTypInclude` | `MessageTypeExcluded` | `MessageTypeInclude` |
| `Min Sto Amt` | `Module` | `Msg` |
| `Msg Disposition` | `Msg Error Code` | `Msg Name Id` |
| `Msg Pde` | `Msg Status` | `Mt103 Control` |
| `Mt103 Type` | `MtXmlTransPostQueue` | `Multi` |
| `Name` | `Name.1` | `Name.2` |
| `No` | `No Lines Per Output Item` | `Nostro Acct No` |
| `Null Lines Allowed` | `OT` | `Off Pend Track Status` |
| `Offset` | `Ofs` | `On` |
| `Operand` | `Ordering Bank` | `Ordering Customer` |
| `Org Payload` | `Org.De.I.Header` | `Org.De.O.Header` |
| `Orig Amt` | `Orig Ccy` | `Osn` |
| `Our Ext Acc No` | `Out If Routine` | `Out If Routine and In If Routine` |
| `Output` | `Output Format` | `Output Item` |
| `Outward Carriers` | `Overdue Time Interval` | `Overflow` |
| `Overriding Requestor DN` | `Overriding Responder DN` | `Page` |
| `Page Number` | `Page Overflow` | `Pass` |
| `Pay` | `Payload` | `Payment System` |
| `Pgm Autom Id` | `Po Box Number` | `Post Code` |
| `Prefix` | `Prefix Text` | `Prev Swift Rel` |
| `Prev Swift Rel.1` | `Prev Swift Rel.2` | `Process` |
| `Produce Schema` | `Queue` | `Read Normal` |
| `Read Priority` | `Reason Code` | `Receiver Bank` |
| `Receiver's Correspondent (Tag 54)` | `Receiver’s Correspondent (Tag 54)` | `Rel` |
| `Release` | `Replace Currency` | `Reply to Appln` |
| `Report` | `Required` | `Residence/Town` |
| `Response Queue Name` | `Retention Period` | `Round Type` |
| `RouteChannel` | `Routine` | `Rtn` |
| `Salutation` | `Schema Path` | `Scope` |
| `Secondary Tlx Chg` | `Secure Msg` | `Send Msg Type` |
| `Send To Party` | `Sender Address` | `Service Type Id` |
| `Sign` | `Single` | `Sort Code` |
| `Source` | `Source Application` | `Source Common Ref` |
| `Source Trans ref` | `Source Type` | `Source Unique Id` |
| `Start Date` | `Statement Id` | `Status` |
| `Status Code` | `Status Reason Code` | `Status Transaction ID` |
| `Stp Status` | `Street` | `Street Name` |
| `Stylesheet Path` | `Sub Department` | `Subroutine` |
| `Suffix Text` | `Swift` | `Swift Address` |
| `Swift Auth Key` | `Swift Tracker Bic` | `Syntax` |
| `Sys Id` | `Sys Txn Code` | `SystemId` |
| `T` | `T24DeliveryQueue` | `TYPE` |
| `Tag` | `Target Carrier` | `Target Msg Type` |
| `Text` | `Their Acct No` | `Thru` |
| `Time` | `Timezone` | `Title` |
| `To Addr Output Fmt` | `To Address` | `Town Location Name` |
| `Town Name` | `Transaction Code Credit` | `Transaction Code Debit` |
| `Transaction Ref` | `Transaction Reference` | `Transaction Reference.` |
| `Transaction Type` | `Transformation Rule` | `TransmissionReportXslt` |
| `Txn Reference` | `Txt` | `Type` |
| `UETR Message` | `UETR Reference` | `Uetr Reference` |
| `Uetr Message` | `Uetr Msg Type` | `Uetr Reference` |
| `Unstruct Addr Default Format` | `Upd Addr Hold Opt` | `Update` |
| `Use` | `User` | `Usr` |
| `Valid Ascii Table` | `Validate Bic` | `Validate Sak` |
| `Validation Flag` | `Version` | `Xml Transform Req` |
| `Xslt` | `extTransFailQueue` | `field` |
| `fields` | `isposition` | `ode` |
| `opies` | `or` | `orm` |
| `transformationFailQueue` | `value as` | `with` |
| `ype` | `ypes` |  |


---


## Appendix B: Consolidated Field Reference


This appendix consolidates all field description tables from across the documentation, grouped by sub-module. This provides a single reference for all field definitions.


### Customer_Output - DE (DE)


**Customer Address in Delivery Output**

| Field | Description |  |  |  |  |  |  |
|---|---|---|---|---|---|---|---|
| ID | Represents the identification ID of the address output format. |  |  |  |  |  |  |
| Description | Specifies the description of address output format. |  |  |  |  |  |  |
| Output Item | Identifies an output component and it can have one or more lines. This is a multi-value field and has sub values. The logic applied (rules) on how the system handles the output item is described below: By giving the same name to the Output Item field to different output items, the system evaluates the first output line and if this is null it continues with the next one. Different output item names implies that each output item is included in the address output. The output item number/value given by the bank user does not reflect the position a line has in the address. The position of a line in an address output is implied by the order in which the output items are defined into the address output format. The output items must be described top-down, in the order in which they must appear in the output. Example The below table shows the position of a line in the address output display. Attributes Address Output Display Length=15 Number of Lines Per Output Item=1 Address Attribute.1.1=BUILDINGNO=50 Address Attribute.1.2=STREET=Luliu Maniu Address Attribute.1.3=FLAT NO=502 50 Luliu Maniu Length=15 Number of Lines Per Output Item =2 Address Attribute.1.1=BUILDINGNO=50 Address Attribute.1.2=STREET=Luliu Maniu Address Attribute.1.3=FLAT NO=502 50 Luliu Maniu 502 | Attributes | Address Output Display | Length=15 Number of Lines Per Output Item=1 Address Attribute.1.1=BUILDINGNO=50 Address Attribute.1.2=STREET=Luliu Maniu Address Attribute.1.3=FLAT NO=502 | 50 Luliu Maniu | Length=15 Number of Lines Per Output Item =2 Address Attribute.1.1=BUILDINGNO=50 Address Attribute.1.2=STREET=Luliu Maniu Address Attribute.1.3=FLAT NO=502 | 50 Luliu Maniu 502 |
| Attributes | Address Output Display |  |  |  |  |  |  |
| Length=15 Number of Lines Per Output Item=1 Address Attribute.1.1=BUILDINGNO=50 Address Attribute.1.2=STREET=Luliu Maniu Address Attribute.1.3=FLAT NO=502 | 50 Luliu Maniu |  |  |  |  |  |  |
| Length=15 Number of Lines Per Output Item =2 Address Attribute.1.1=BUILDINGNO=50 Address Attribute.1.2=STREET=Luliu Maniu Address Attribute.1.3=FLAT NO=502 | 50 Luliu Maniu 502 |  |  |  |  |  |  |
| Address Attribute | Identifies a name or address attribute that is included in the Output Item field and is part of the output item group. This field is multi-value field allowing the user to include one or more name and address fields in the output. The logic applied (rules) on how the system handles the output item is described below: The DE.ADDRESS fields alone can be specified. Adding multiple address attributes within the same output item, implies that all the address attributes are combined together within the same output item (it applies the and logic) in the order specified by the user. Attributes that are combined together are separated by a space. |  |  |  |  |  |  |
| Prefix Text | Associated with the value given in Address Attribute and identifies the text to precede the address attribute. If the Address Attribute field is blank, then its prefix is not considered in the output. |  |  |  |  |  |  |
| Suffix Text | Associated with the value given in Address Attribute . It identifies the text to follow the address attribute. If the Address Attribute field is blank then its prefix is not considered in the output. |  |  |  |  |  |  |
| Max Length | 1, the system returns the first character up to max length for the first line and then continues with the output for the next lines. If the max line is exceeded the next chars are ignored. |  |  |  |  |  |  |
| No Lines Per Output Item | Represents the maximum number of lines to use for an output item (Output Item). The maximum number of lines per output item combined with the maximum number of characters per output item gives an indication of the name or address attributes to be displayed on each line in the output. If this field is left blank, the default value is 1. |  |  |  |  |  |  |
| Maximum Lines | Indicates the maximum lines to be entered for the respective address output, including all the output items. When applying this format to an address, if the system determines the output has more lines than the maximum lines defined here, then the system considers only the first maximum lines and the remaining lines are ignored. |  |  |  |  |  |  |
| Null Lines Allowed | Indicates if the system should include an output item which is evaluated as blank in the address output. The logic applied (rules) on how the system handles the output item is described below: If set to YES, the system does not remove the null output items. If set to NO or left blank, the system removes the null output items. |  |  |  |  |  |  |
| Api Output Format | Identifies the routine to be called by the system. It attaches a routine to implement more complex output format rules. |  |  |  |  |  |  |

**Customer Address in Delivery Output**

| Field | Description |
|---|---|
| ID | Indicates the country code. |
| Description | Specifies the description of the address country output rule for a specific country for various carriers. |
| Carrier Type | Indicates the name of the carrier for which these rules are applied. It must be a defined carrier. This is a multi-value field and has sub values. The existing conversion can be mapped differently depending on the carrier type. |
| To Addr Output Fmt | Indicates the name and address output format applied to the address when the output is sent. It is part of the carrier group and refers to the ADDRESS.OUTPUT.FORMAT record. At least one of the To Addr Output Fmt and De Format Conversion fields must be populated. |
| De Format Conversion | Indicates a CUS conversion used in the delivery format. It is part of the carrier group and sub group with associated values. The CUS conversions are notations, which are used in the delivery formats to indicate that the customer’s address should be included in the output. The system provides a set of CUS conversions, which are hard coded rules and are carrier specific. For example, CUS*FULL. |
| Output Format | Specifies the name of the address output format, which is to be used by the delivery when the associated CUS conversion is indicated in a delivery format. It refers to a record in ADDRESS.OUTPUT.FORMAT . |
| Unstruct Addr Default Format | Identifies an unstructured address output format. |

**Customer Address in Delivery Output**

| Field | Description |
|---|---|
| Carrier Type | Indicates the name of the carrier for which the default output rules are defined. |
| Default To Addr Out Fmt | Indicates the default address output format, which is applied to the address where the output is sent. |
| De Format Conversion | This field is part of the carrier group, sub-group with the associated values. It identifies the output format that is used when a conversion is indicated in the delivery format for the defined carrier. |
| Default Output Fmt | Indicates the default address output format, which is used by delivery when this conversion is indicated in a delivery format. It refers to a record in ADDRESS.OUTPUT.FORMAT . |
| Unstruct Addr Default Format | Identifies an unstructured address output format. |

**DefiningPrintFormat**

| Line number | Description |
|---|---|
| 02 | Print on line two |
| +2 | Print two lines down from the last item printed (miss one line) |
| +0 | Print on the same line as the last item |
| 1-10 | Start printing on line one, put the next multi-value on line two and put the 10th value on line 10 .If more than 10 values exist, page overflow*** occurs |
| +2-55 | Start printing two lines down from the last item printed and do not print past line 55. If the previous item was printed on line 54 or more, this item overflows*** immediately to the next page |
| +4-+2 | Start printing four lines down from the last item printed and do not print more than two lines |

**DefiningPrintFormat**

| Field in DE.FORMAT.PRINT | Value |
|---|---|
| Line S | 3-55 |
| Field Text | AMOUNT |
| Line S | +2 |
| Field Text | TOTAL |

**DefiningPrintFormat**

| Field in DE.FORMAT.PRINT | Value |
|---|---|
| Line S | 2 |
| Indent | 10 |
| Field Text | CUSTOMER NAME: |
| Line S | +0 |
| Indent | 25 |
| Field Text | CUSNAME |

**DefiningPrintFormat**

| Field in DE.FORMAT.PRINT | Value |
|---|---|
| Line S | +2-+4 |
| Indent | 10 |
| Field Text | ADDRESS |
| Line S | +0-+4 |
| Indent | 60 |
| Field Text | DATE |

**DefiningPrintFormat**

| Field in DE.FORMAT.PRINT | Value |
|---|---|
| Line S | +2-+4 |
| Indent | 1 |
| Field Text | ADDRESS |
| Multi | M |
| Line S | +0-+4 |
| Indent | 10 |
| Field Text | ADDRESS |
| Multi | M |

**DefiningPrintFormat**

| Value | Format | Description |
|---|---|---|
| DATE | DD MMM YYYY | Three letter month |
| DATE/F | DD MMMMMMMMM YYYY | Full month name |
| DATE/S | DD MM YY | Two digit month |
| DATE/US | MMM DD YYYY | Three letter month |
| DATE/F/US | MMMMMMMMM DD YYYY | Full month name |
| DATE/S/US | MM DD YY | Two digit month |
| DATE/U | Defaults from the value of the USER definition held on the DE.FORMAT.PRINT record in TSA.SERVICE . | As per USER or LANGUAGE , the definition of the Date Format field. |

**DefiningPrintFormat**

| Value | Description |
|---|---|
| Bn | Right adjust into a length of n by inserting blanks on the left |
| *n | Right adjust into a length of n by inserting asterisks (*) on the left |
| Zn | Right adjust into a length of n by inserting zeros (0) on the left |
| , | Insert commas (,) to separate thousands |
| . | Change decimal points (.) to commas (,) |
| . , | Insert points (.) to separate thousands and use a comma for decimals |
| , . | As above |
| - | Put the sign after the amount (the sign normally precedes the amount) |
| A | Print the absolute value (that is, without a sign) |
| D | Print DR after the amount, if it is negative |
| C | Print CR after the amount, if it is positive and DR if negative |
| % | Print % after the data |
| 00x00x000x | Digits are substituted for the zeros. Any other characters are printed in the non-zero representations of the mask (that is, x represents 1 or more characters). For example, Field contains 123456, mask is 00-(00-00), the field is output as 12-(34-56) |

**DefiningPrintFormat**

| Value | Description |
|---|---|
| +,TOTAL.n | Add the contents of the field into TOTAL.n |
| -,TOTAL.n | Subtract the contents of the field from TOTAL.n |
| *,TOTAL.n | Multiply TOTAL.n by the contents of the field |
| /,TOTAL.n | Divide TOTAL.n by the contents of the field |
| ZERO | Zero the field after printing (may be used only if the FIELD/"TEXT" is set to TOTAL.n). |

**DefiningPrintFormat**

| Value | Description |
|---|---|
| Field text | Payment Details |
| Dependent On | PAY DET |
| Field text | PAY DET |

**DefiningPrintFormat**

| Field in DE.FORMAT.PRINT | Description |
|---|---|
| Line S | .10 |
| Indent | .35 |
| Field text | .AMOUNT |
| Dependent On | .AMOUNT |
| Depend Operand | .LT |
| Depend Cond | .0 |
| Line S | .10 |
| Indent | .50 |
| Field text | .AMOUNT |
| Dependent On | .AMOUNT |
| Depend Operand | .GE |
| Depend Cond | .0 |

**Detailed workflow Outward Delivery Messages**

| User Header Fields/Tags | Description | Content/Options |
|---|---|---|
| User Header Fields/Tags | Description | Content/Options |
| 103 | Fin Copy Service Code | 3!a |
| 113 | Banking Priority | 4!x |
| 108 | Message User Reference | 16x |
| 119 | Validation Flag | 8!c |
| 115 | Payment-Release-Information-Receiver | 32x |

**Emitting Delivery Messages to Event Store**

| Parameter Name | Value |
|---|---|
| FROM | modelbank@temenos.com |
| TO | alertherman@gmail.com |
| REPLY-TO | modelbank@temenos.com |
| SUBJECT | "Alert notification - Account Overdrawn" |
| MESSAGE | "Message from Model Bank Dear MR. Retail User We have the following Alert notification for you : Account Overdrawn Account Number : *9737 Transaction Amount : USD10,000.00DR Transaction Date : 20 APR 2020 Account Balance : -35,749.38 " |

**Generation of MX Message using ISOMX Carrier**

| MX Identifier | Description |
|---|---|
| acmt.xxx.xxx.xx | Account Management |
| admi.xxx.xxx.xx | Administration |
| camt.xxx.xxx.xx | Cash Management |
| defp.xxx.xxx.xx | Derivatives |
| pacs.xxx.xxx.xx | Payments Clearing and Settlement |
| pain.xxx.xxx.xx | Payments Initiation |
| reda.xxx.xxx.xx | Reference Data |
| seev.xxx.xxx.xx | Securities Events |
| semt.xxx.xxx.xx | Securities Management |
| sese.xxx.xxx.xx | Securities Settlement |
| setr.xxx.xxx.xx | Securities Trade |
| trea.xxx.xxx.xx | Treasury |
| tsmt.xxx.xxx.xx | Trade Services Management |

**InwardDeliveryMessageProcessing**

| Field | Value | Description |
|---|---|---|
| Source Type | GLOBUS | Holds the interface called from a subroutine. |
| Log File Dir | LOGDIR | Specifies the name of the OFS log directory. |
| Log Detail Level | FULL | Lists the full history of each OFS message maintained. |
| Maint Msg Dets | Y | Creates an audit record for each OFS message. |
| Det Prefix | INW | Specifies the audit record prefix. |
| Syntax Type | OFS | Specifies the OFS syntax type for messages. |

**InwardDeliveryMessageProcessing**

| Field | Value | Description |
|---|---|---|
| Application Queue | NULL | Specifies the application which should receive an inward message of this type. |
| Inward Ofs Rtn | ROUTINE NAME | Specifies the supplied or local subroutine, which should be called to process this message type. |
| In Ofs Version | VERSION | Indicates to OFS, which version of an application should be used to create the records. |
| Ofs Source | SOURCE | Indicates the OFS source interface to be used when processing this message. |

**Misc**

| Services | Description |
|---|---|
| DE.EOP.INWARD and DE.EOP.OUTWARD | These services analyse the DE.O.HEADER and DE.I.HEADER entries respectively to identify the records that are processed completely. These services select the DE.I.HEADER and DE.O.HEADER records, moving the records from DE.I.HEADER to DE.I.HEADER.ARCH and DE.O.HEADER to DE.O.HEADER.ARCH respectively. |
| DE.MM.CLEAR.HANDOFF | This service deletes the DE.O.HANDOFF records where DE.O.HEADER is previously removed. This service selects all the DE.O.HANDOFF records to identify the records to be deleted. |
| Delivery Inward and Delivery Outward Archiving | These services archive the records from DE.I.HEADER.ARCH and DE.O.HEADER.ARCH respectively along with related table records. |

**Misc**

| S.No | Parameters | Description |
|---|---|---|
| 1. | Tracker Status Reason | Allows users to define the status code and status reason which is used to update the status of the incoming MT103 payment in the SWIFT Confirmation tracker. |
| 2. | DE.MESSAGE.HEADER | Allows users to define the message headers, which are used for various type of messages. For each header, it stores the version, set of Business and Generic Metadata, which must be pushed as part of the data event with the payload. |
| 3. | DE.BUSINESS.SERVICE.RULES | Allows users to create business service rules for delivery messages based on domain, message name id, business application, application context field, application context value, start date, end date, business service and status. When a Delivery Message is handed off to Delivery, it considers the supplied value if the Business Application supplies the Business Service. Otherwise, it determines the Business Service based on the DE.BUSINESS.SERVICE.RULES application setup. |
| 4. | DE.DELIVERY.RESPONSES | Stores the incoming replies received for the outward interact MX messages (Ack/Nack/DLN) sent through delivery. It is possible to store other replies sent by other bank systems, which are acting as an intermediary systems before the messages sent to SWIFT network. |
| 5. | DE.DLN.REQUIREMENTS | Allows the bank to define the rules to request a positive or overdue delivery notification. In this way, the bank has the option to request a positive delivery notification and overdue warning (Optional). It is not possible to request only overdue warning. |
| 6. | DE.ALT.CHARS | This table helps to parameterise the alternate characters (defined in ASCII.VAL.TABLE ) for the local unsupported characters. Various rules are defined to replace the alt chars based on the position of the unsupported character in the message string. A default alternate character is defined if alternate character is not defined for an unsupported character. |
| 7. | DE.MSG.CHARS.RULE | This parameter table defines the character set rules for each carrier and message type. |

**SWIFT2024 Rulebook Changes**

| Tags | Path in SWIFT Portal | Description |
|---|---|---|
| Business Service Tag | /AppHdr/BizSvc | Populated as swift.cbprplus.02 |
| Payee Address Line | /Pyee/PstlAdr/AdrLine | Limited to three lines with a maximum of 35 characters per line |
| Stop Request Status Code | /ChqCxlOrStopSts/Sts/Cd | Changed to RJCR and ACCR for ‘Rejected’ and ‘Accepted’ respectively |
| Province Of Birth | /ChqCxlOrStopRpt/Chq/Pyee/Id/PrvtId/DtAndPlcOfBirth/PrvcOfBirth | Updated character type as ISOEXTENDED for payee |
| City Of Birth | /ChqCxlOrStopRpt/Chq/Pyee/Id/PrvtId/DtAndPlcOfBirth/CityOfBirth | Updated character type as ISOEXTENDED for payee |

**SWIFT 2019 Rulebook Changes**

| Message | Description |
|---|---|
| MT190 | Advice of Charges, Interest and Other Adjustments |
| MT191 | Request for Payment of Charges, Interest and Other Expenses |
| MT192 | Request for Cancellation |
| MT195 | Queries |
| MT196 | Answers |
| MT199 | Free-Format |
| MT292 | Request for Cancellation |
| MT295 | Queries |
| MT296 | Answers |
| MT299 | Free-Format |
| MT992 | Request for Cancellation |
| MT995 | Queries |
| MT996 | Answers |
| MT999 | Free-Format |

**SWIFT 2020 Rulebook Changes**

| ID | Description | Tracker Status | Status Code | Status Reason | Confirmed Amount and Currency |
|---|---|---|---|---|---|
| ACCC | Accepted; settlement confirmed | Settled | ACCC |  | Yes |
| ACSP/G001 | Payment transferred | Transferred | ACSP | G001 | Yes |
| ACSP/G002 | Credit might not be confirmed in the required two days | Pending | ACSP | G002 |  |
| ACSP/G003 | Credit not confirmed due to pending required documents | Pending | ACSP | G003 |  |
| ACSP/G004 | Pending funds | Pending | ACSP | G004 |  |
| RJCT/AC01 | Incorrect account number | Rejected | RJCT | AC01 |  |
| RJCT/AC04 | Closed account number | Rejected | RJCT | AC04 |  |
| RJCT/AC06 | Blocked account | Rejected | RJCT | AC06 |  |
| RJCT/BE01 | Inconsistent with end customer | Rejected | RJCT | BE01 |  |
| RJCT/NOAS | No answer from customer | Rejected | RJCT | NOAS |  |
| RJCT/RR03 | Missing creditor name or address | Rejected | RJCT | RR03 |  |
| RJCT/FF07 | Invalid purpose | Rejected | RJCT | FF07 |  |
| RJCT/RC01 | Bank identifier incorrect | Rejected | RJCT | RC01 |  |
| RJCT/RC08 | Invalid clearing system member identifier | Rejected | RJCT | RC08 |  |
| RJCT/FOCR | Following cancellation request | Rejected | RJCT | FOCR |  |
| RJCT/DUPL | Duplication | Rejected | RJCT | DUPL |  |
| RJCT/RR05 | Regulatory information invalid | Rejected | RJCT | RR05 |  |
| RJCT/AM06 | Amount too low | Rejected | RJCT | AM06 |  |
| RJCT/CUST | Requested by customer | Rejected | RJCT | CUST |  |
| RJCT/MS03 | Not specified reason agent generated | Rejected | RJCT | MS03 |  |

**SWIFT 2020 Rulebook Changes**

| Fields | Mapping |
|---|---|
| Status | Tracker status corresponding to the tracker status reason captured in FT, based on the parameterisation in SFCONF.TRACKER.STATUS.REASON |
| Status Code | Status code corresponding to the tracker status reason captured in FT, based on the parameterisation in SFCONF.TRACKER.STATUS.REASON |
| Reason Code | Reason code corresponding to the tracker status reason captured in FT, based on the parameterisation in SFCONF.TRACKER.STATUS.REASON |
| Confirmed Amount | Amount Credited from FUNDS.TRANSFER , if the Confirmed Amount and Currency fields are set to Yes in SFCONF.TRACKER.STATUS.REASON for the tracker status reason captured in FT |
| Confirmed Currency | Credit Currency from FUNDS.TRANSFER , if the Confirmed Amount and Currency fields are set to Yes in SFCONF.TRACKER.STATUS.REASON for the tracker status reason captured in FT |
| Status Transaction ID | The FT ID |

**SWIFT 2020 Rulebook Changes**

| MT199 Tag | Mapping | Description |
|---|---|---|
| Sender | The SWIFT address of the bank |  |
| Receiver | The BIC of the SWIFT tracker from DE.PARM |  |
| Tag 121 | The ID of the confirmation tracker | The UETR of the following MT103 |
| Tag 20 | Status Transaction ID | The ID of the FT which as updated the confirmation tracker status |
| Tag 21 | Inward Message Reference | The original tag 20 of the incoming MT103 |
| Tag 79 Line 1 | //yymmHHMM ± the offset of the local time server against UTC | The current date and time of the system when the confirmation tracker is updated |
| Tag 79 Line 2 | // / |  |
| Tag 79 Line 3 | //The SWIFT address of the bank |  |
| Tag 79 Line 4 | If Confirmed Ccy is blank, use Orig Ccy If Confirmed Amt is blank, use Orig Amt // |  |

**SwiftNet Interact MX Services**

| Attribute | Description |
|---|---|
| ReplaceCurencyForReceivingBICS | Indicates the delivery transformation layer to perform currency transformation from a specific currency to another, with the option to exclude this for specific receiving BICs (BICs separated by a comma,","). Format: FromCurrency/ToCurrency/[ReceiverBIC1,ReceiverBIC2, and so on] |

**Translation DeliveryMessages**

| Field | Conversion |
|---|---|
| Commiss | TABLE COM |
| Tax | TABLE TAX |

**Unique End-to-End Transaction Reference**

| Field | Description |
|---|---|
| Uetr Msg Type | A multi-valued field in the SWIFT.PARAMETER application that holds the message types that require a UETR reference to be mapped in the outgoing message. |
| Fwd Msg Type | A multi-valued field that holds the message types that require a UETR reference to be forwarded in the outgoing message. |

**Unique End-to-End Transaction Reference**

| Field | Description |
|---|---|
| Uetr Message | A multi-valued field in the CBPRPULS record of the DE.CARRIER application that holds the message types that require a UETR reference to be mapped in the outgoing message. |

**Misc**

| S.No. | Parameters | Description |
|---|---|---|
| 1. | FT.APPL.DEFAULT | This application allows the user to define application-level default values, which is used when processing FUNDS.TRANSFER or STANDING.ORDER instructions. These values will be applicable irrespective of the transaction type, and the user must create one record for each COMPANY (that is, in case of multi-company setup) on the system. |
| 2. | FT.TXN.TYPE.CONDITION | This application allows the user to define the default conditions for each transaction type, which can be processed by the FUNDS.TRANSFER and STANDING.ORDER applications. User can define Transaction Code Credit , Transaction Code Debit , Comm Types , Charge Types , Forw Value Max and Back Value Max for each transaction type. |
| 3. | FT.CHARGE.TYPE | This application allows the user to define the conditions related to various types of standard flat charges used by Temenos Transact . In addition, charge types can be linked to allow different charge structures, tax codes and so on to be applied depending on the residence of the ordering customer. |
| 4. | FT.COMMISSION.TYPE | This application allows the user to define the conditions related to all types of commission used in applications. Each commission type can be defined as a Flat Amount or variable amount, proportionate to the amount transferred. In the latter case, different percentages can be defined for different Bands or Levels of transfer amounts. Minimum and maximum commissions can be specified for each Band or Level together with overall minimum or maximum commission charges. |
| 5. | CORR.BANK.CHARGES | This application allows the user to define correspondent bank charges or commission, which will default in FT when Def Corr Bank Chgs field in FT.APPL.DEFAULT is set to Yes. |
| 6. | FT.GEN.CONDITION | This application allows the user to identify a specific group of customers, using a user-defined Funds Transfer General Condition number. , This will then be cross-related to the Group Condition table to define Funds Transfers conditions applicable to that group. The FT General Condition record must exist before any associated group condition is specified. The key to this table is also the key to the associated FT Group Condition record. |
| 7. | FT.GROUP.CONDITION | This application allows the user to define special conditions applicable to specific groups of customers or individual customers which overrides the normal conditions, used by the Funds Transfer application. A customer subjected to these conditions must first meet the selection criteria defined in FT.GEN.CONDITION and accessed using an identical key. |
| 8. | EB.DUPLICATE.TYPE | This application allows the user to define selected fields to check for any duplicate contracts for the given application. This application also allows the user to define duplicate check criteria for linked applications, which can be defined in the Linked Application field. It allows the user to select the following: Application for which the duplicate check criteria is defined. The fields from that application which will be part of the duplicate check. The number of purge days, which will ensure that the duplicate criteria check will be applied only for contracts raised in the past n days (number of days defined in the Purge Days field in this application). |

**Misc**

| S.No. | Product Name | Product Attributes |
|---|---|---|
| 1. | OC- Outward by Cheque | Refers to the issuance (by the bank) of a Manager Cheque or a Bank Cheque in local currency in favor of the beneficiary who does not maintain an account with the bank. |
| 2. | OD – Outward By Draft | Refers to the issuance (by the bank) of a Bank Draft (usually in foreign currency), in favor of the beneficiary who does not maintain an account with the bank. |
| 3. | OT –Outward by Telex | Refers to the issuance (by the bank) of a payment via Swift or Telex. The instructions are usually sent to the correspondent bank for processing. This transaction type will produce both pay and cover cables automatically where required. |
| 4. | OB – Outward by bankers payment | Refers to the issuance (by the bank) of a banker's payment in local currency. This method of payment is used extensively in the UK to perform local currency payment. |
| 5. | BC – Outward by BACS | This transaction type is only applicable for Sterling and within the UK and refers to outward transfers by BACS (Bankers Automatic Clearing System). Currently BACS payments are not generated by the system. If it is required, it must be added as a local enhancement. Other host countries may have similar systems to which this may be adapted. |
| 6. | IC – Inward payment by cheque or draft | Refers to the receipt of a cheque or a draft by the bank, to be credited to a customer account. |
| 7. | IT – Inward by Telex | Refers to the receipt of a Swift or Telex payment by bank in favor of bank's customers, where the proceeds have to be credited to an account in bank’s books. |
| 8. | IB – Inward by banker's payment | Refers to the receipt (by the bank) of a banker's payment in favor of an account in our books (UK only). |


### Customer_Output - DEMXTR (DEMXTR)


**SwiftNet Interact MX Services**

| Attribute | Description |
|---|---|
| ReplaceCurencyForReceivingBICS | Indicates the delivery transformation layer to perform currency transformation from a specific currency to another, with the option to exclude this for specific receiving BICs (BICs separated by a comma,","). Format: FromCurrency/ToCurrency/[ReceiverBIC1,ReceiverBIC2, and so on] |


### Customer_Output - IX (IX)


**Camt.53 and Camt.54 Statement Summary**

| FIELD | VALUE |
|---|---|
| Validation Rtn | @SEPA.WRITE.PAYM.PARTICIPANTS |

**Misc**

| Camt Index | Description | User Configurable |
|---|---|---|
|  | Group Header |  |
| 1.1 | Message Identification | Y |
| 1.2 | CreationDateTime |  |
|  | Statement |  |
| 2.1 | Identification | Y |
| 2.4 | CreationDateTime |  |
| 1.2.1 | IBAN |  |
| 1.2.2 | OtherId | Y |
| 2.24 | Code |  |
| 2.34 | Amount |  |
| 2.35 | CreditDebitIndicator |  |
| 2.36 | Date |  |
| 2.78 | Amount |  |
| 2.79 | CreditDebit Indicator |  |
| 2.81 | Status |  |
| 2.91 | Proprietary | Y |
| 2.99 | Issuer | Y |


---
