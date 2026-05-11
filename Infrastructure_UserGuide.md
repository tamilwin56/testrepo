
# Temenos Transact — Infrastructure Module Documentation


> **Comprehensive User Guide**
> Generated: 13 April 2026
> Content: Configuration | Reference | Field Descriptions | Glossary


## Table of Contents

  - [Infrastructure Module Overview](#infrastructure-module-overview)
    - [Sub-Module Summary](#sub-module-summary)
    - [How to Use This Guide](#how-to-use-this-guide)
  - [Chapter 1: Infrastructure - EB](#chapter-1-infrastructure---eb)
    - [Features in Infrastructure - EB](#features-in-infrastructure---eb)
    - [1.1  Dynamic-applications](#11-dynamic-applications)
    - [1.2  Component Framework](#12-component-framework)
    - [1.3  Connection Management](#13-connection-management)
    - [1.4  Database Schema Separation](#14-database-schema-separation)
    - [1.5  Document Management](#15-document-management)
    - [1.6  Enquiry](#16-enquiry)
    - [1.7  Enterprise Deployment Pattern](#17-enterprise-deployment-pattern)
    - [1.8  FileUpload](#18-fileupload)
    - [1.9  Multi-language](#19-multi-language)
    - [1.10  Protocol](#110-protocol)
    - [1.11  Report Control](#111-report-control)
    - [1.12  System Core](#112-system-core)
    - [1.13  COB](#113-cob)
    - [1.14  Service Automation](#114-service-automation)
    - [1.15  Warmup](#115-warmup)
    - [1.16  Mass-changes](#116-mass-changes)
    - [1.17  Neighbor](#117-neighbor)
    - [1.18  Archiving](#118-archiving)
    - [1.19  Businessdayfrequencyforservice](#119-businessdayfrequencyforservice)
    - [1.20  Cache Resetting](#120-cache-resetting)
    - [1.21  Cloud Operation Efficiency](#121-cloud-operation-efficiency)
    - [1.22  COB](#122-cob)
    - [1.23  Exit-API](#123-exit-api)
    - [1.24  Queues](#124-queues)
    - [1.25  Company Local Content](#125-company-local-content)
    - [1.26  Constraints](#126-constraints)
    - [1.27  Data Events](#127-data-events)
    - [1.28  Grouping Events](#128-grouping-events)
    - [1.29  LocalReference AlternateKeys](#129-localreference-alternatekeys)
    - [1.30  Multi-time zone](#130-multi-time-zone)
    - [1.31  Service Automation](#131-service-automation)
    - [1.32  Standards Restrictions](#132-standards-restrictions)
    - [1.33  SupportingOtherDateFormat](#133-supportingotherdateformat)
    - [1.34  Traceability](#134-traceability)
    - [1.35  Transact Monitoring Using Grafana](#135-transact-monitoring-using-grafana)
  - [Chapter 2: Infrastructure - GP](#chapter-2-infrastructure---gp)
    - [2.1  Global Processing](#21-global-processing)
  - [Chapter 3: Infrastructure - NS](#chapter-3-infrastructure---ns)
    - [3.1  Non-Stop Processing](#31-non-stop-processing)
  - [Chapter 4: Infrastructure - OF](#chapter-4-infrastructure---of)
    - [4.1  OFS features](#41-ofs-features)
  - [Chapter 5: Infrastructure - PW](#chapter-5-infrastructure---pw)
    - [5.1  Process Orchestration](#51-process-orchestration)
  - [Chapter 6: Infrastructure - SM](#chapter-6-infrastructure---sm)
    - [Features in Infrastructure - SM](#features-in-infrastructure---sm)
    - [6.1  ExternalAuthorisation](#61-externalauthorisation)
    - [6.2  Sms](#62-sms)
  - [Appendix A: Glossary of T24 Applications & Fields](#appendix-a-glossary-of-t24-applications-fields)
    - [Applications](#applications)
    - [Fields Referenced](#fields-referenced)
  - [Appendix B: Consolidated Field Reference](#appendix-b-consolidated-field-reference)
    - [Infrastructure - EB (EB)](#infrastructure---eb-eb)
    - [Infrastructure - NS (NS)](#infrastructure---ns-ns)
    - [Infrastructure - OF (OF)](#infrastructure---of-of)
    - [Infrastructure - SM (SM)](#infrastructure---sm-sm)

---


## Infrastructure Module Overview


This document provides comprehensive documentation for the **Infrastructure** module of Temenos Transact. It covers **6 sub-modules** with a total of **41 feature areas**.


### Sub-Module Summary


| # | Sub-Module | Code | Features | Description |
|---|-----------|------|----------|-------------|
| 1 | **Infrastructure - EB** | `EB` | 35 | Infrastructure - EB module of Temenos Transact |
| 2 | **Infrastructure - GP** | `GP` | 1 | Infrastructure - GP module of Temenos Transact |
| 3 | **Infrastructure - NS** | `NS` | 1 | Infrastructure - NS module of Temenos Transact |
| 4 | **Infrastructure - OF** | `OF` | 1 | Infrastructure - OF module of Temenos Transact |
| 5 | **Infrastructure - PW** | `PW` | 1 | Infrastructure - PW module of Temenos Transact |
| 6 | **Infrastructure - SM** | `SM` | 2 | Infrastructure - SM module of Temenos Transact |


### How to Use This Guide


Each feature in this document is organized into the following sections:

- 📖 **Introduction** — Overview and purpose of the feature
- ⚙️ **Configuration** — How to set up and configure the feature
- 🔧 **Working With** — Operational usage and field descriptions
- 📋 **Tasks** — Step-by-step procedures
- 📊 **Outputs** — Reports, enquiries, and generated outputs

Each feature includes a **Quick Reference Card** at the top with application names, key fields, prerequisites, and a summary. Appendices provide a full glossary, consolidated field tables, and end-to-end use-case scenarios.

---


## Chapter 1: Infrastructure - EB


Infrastructure - EB module of Temenos Transact


### Features in Infrastructure - EB


| # | Feature | Sections |
|---|---------|----------|
| 1.1 | Dynamic-applications | Intro, Confi, Tasks |
| 1.2 | Component Framework | Confi |
| 1.3 | Connection Management | Confi, Tasks |
| 1.4 | Database Schema Separation | Confi, Tasks |
| 1.5 | Document Management | Confi |
| 1.6 | Enquiry | Intro, Confi, Tasks |
| 1.7 | Enterprise Deployment Pattern | Tasks |
| 1.8 | FileUpload | Intro |
| 1.9 | Multi-language | Intro, Confi, Tasks |
| 1.10 | Protocol | Intro, Confi, Outpu |
| 1.11 | Report Control | Confi |
| 1.12 | System Core | Intro |
| 1.13 | COB | Intro, Confi, Tasks |
| 1.14 | Service Automation | Confi |
| 1.15 | Warmup | Confi, Tasks |
| 1.16 | Mass-changes | Intro, Confi, Tasks |
| 1.17 | Neighbor | Confi, Tasks |
| 1.18 | Archiving | Intro, Confi, Tasks |
| 1.19 | Businessdayfrequencyforservice | Tasks |
| 1.20 | Cache Resetting | Intro, Confi, Tasks |
| 1.21 | Cloud Operation Efficiency | Tasks |
| 1.22 | COB | Confi, Tasks |
| 1.23 | Exit-API | Confi |
| 1.24 | Queues | Intro |
| 1.25 | Company Local Content | Confi, Tasks |
| 1.26 | Constraints | Confi |
| 1.27 | Data Events | Intro, Confi, Worki, Tasks |
| 1.28 | Grouping Events | Intro |
| 1.29 | LocalReference AlternateKeys | Confi |
| 1.30 | Multi-time zone | Confi, Tasks, Outpu |
| 1.31 | Service Automation | Tasks |
| 1.32 | Standards Restrictions | Tasks |
| 1.33 | SupportingOtherDateFormat | Confi, Tasks |
| 1.34 | Traceability | Confi |
| 1.35 | Transact Monitoring Using Grafana | Confi, Tasks |


### 1.1  Dynamic-applications


> **📇 Quick Reference Card**
> 
> **Purpose:** *Banks uses T24 to create their applications without any code. Such applications are called as Dynamic applications. They are created locally using the Temenos Transact template but do not possess the full capabilities of a T24 application.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks


#### 📖 Introduction

Banks uses T24 to create their applications without any code. Such applications are called as Dynamic applications. They are created locally using the Temenos Transact template but do not possess the full capabilities of a T24 application.

In this user guide, you will learn about the following Temenos Transact applications:

- EB.TABLE.DEFINITION - It helps you to create Dynamic applications.
- EB.TABLE.PROCEDURES - It helps you to trigger user-defined routines during the Dynamic application life cycle.

Designing Dynamic applications

This section explains you the concept of EB.TABLE.DEFINITION application and various field level configurations that are required to create a Dynamic application.

User-defined subroutines

You can trigger user-defined subroutines at specific points during the Dynamic application life cycle. This section lists the scenarios where you can trigger user-defined subroutines.

Enabling GDPR support for Dynamic applications

This section shows the configuration and procedure to apply General Data Protection Regulation (GDPR) support on the EB.TABLE.DEFINITION and AA.CLASS.DEFINITION applications.


#### ⚙️ Configuration

This section explains you the concept of EB.TABLE.DEFINITION application and various field level configurations that are required to create a Dynamic application.

The EB.TABLE.DEFINITION application allows you to design a new application without using the template programming. This application can define a table by simply defining the fields.


##### Field value calculations in a table

In Dynamic applications, you need to define the fields based on certain calculations. A value of a field is determined based on the contents of the other fields present in the table.

If you want to store a calculation in a field, then you need to define that field as a numeric field. For example, an AMOUNT or a NOINPUT field.

The field calculations are defined using a subset of the ECMAScript language, which allows certain formulas to be defined using the following numeric operators:

- Addition operator ( + )
- Subtraction operator ( - )
- Multiplication operator ( * )
- Division operator ( / )
- Exponential operator ( ** )

The below table shows the examples of the formulas that are used in field calculations.

| Formula | Result |
|---|---|
| 1 + 2 | 3 |
| 4 - 2 | 2 |
| 2 * 4 | 8 |
| 6 / 2 | 3 |
| 2 ** 5 | 32 |


###### Order of precedence

The order of precedence defines the order in which mathematical operators are evaluated. It specifies in which direction the evaluation should be performed when operators of the same order are encountered.

The below table shows how to evaluate the calculations when there are no brackets.

| Operator | Order | Direction | Example | Evaluation | Result |
|---|---|---|---|---|---|
| ** | 1 | R to L (where, R - Right and L - Left) | 2 ** 2 ** 3 | 2 ** (2 ** 3) | 256 |
| 2 ** 3 ** 2 | 2 ** (3 ** 2) | 512 |  |  |  |
| 3 ** 2 ** 2 | 3 ** (2 ** 2) | 81 |  |  |  |
| * or / | 2 | L to R | 3 * 4 / 2 | (3 * 4) / 2 | 6 |
| 4 / 2 * 3 | (4 / 2) * 3 |  |  |  |  |
| + or - | 3 | L to R | 1 + 2 - 3 | (1 + 2) - 3 | 0 |
| 2 - 3 + 1 | (2 - 3) + 1 |  |  |  |  |

The below examples show how you can evaluate expressions.

| Expression | Evaluation |
|---|---|
| 2 ** 3 + 3 ** 2 | (2 ** 3) + (3 ** 2) = 8 + 9 = 17 |
| 1 + 2 * 3 + 4 | 1 + (2 * 3) + 4 = 1 + 6 + 4 = 7 + 4 = 11 |
| 2 + 3 * 4 / 2 + 6 | 2 + ((3 * 4) / 2) + 6 = 2 + (12 / 2) + 6 = 2 + 6 + 6 = 8 + 6 = 14 |


###### Field relationships

You can define calculations only on those fields that have direct relationship.

The below example defines two multivalued groups. The first group is shown in red and green color. The second group is shown in blue color.

The below table shows how to calculate a value for different field types using the above example.

| Field type | Calculation |
|---|---|
| Single valued | You can calculate the value of a single valued field using: The other single valued fields The fixed values For example, Field8 |
| Multivalued | You can calculate the value of a multivalued field using: The other multi-values within the same multivalued set The single valued fields The fixed values For example, Field6 |
| Subvalued | You can calculate the value of a subvalued field using: The other sub-values within the same subvalued set The other multi-values within the same multivalued set The single valued fields The fixed values For example, Field3 |


##### Field availability rules

You can add availability rules to a field. These rules determine whether the field should be displayed or not.

A rule is an expression that evaluates to either true or false . You can define a rule by using a subset of the ECMAScript language, which allows the expressions to be defined using the following operators:

- Addition operator ( + )
- Subtraction operator ( - )
- Multiplication operator ( * )
- Division operator ( / )
- Exponential operator ( ** )
- Equality operator ( == )
- Inequality operator ( != )
- Less than operator (
- )
- Less than or equal operator (
- = )
- Logical OR operator ( || )
- Logical AND operator ( && )

You can define rules only on those fields that have direct relationship. When a field has an availability rule assigned to it and the rule evaluates to false , then

- Any value entered in that field is cleared
- Any calculations defined for that field is ignored


#### 📋 Tasks

This section shows the configuration and procedure to apply General Data Protection Regulation (GDPR) support on the EB.TABLE.DEFINITION and AA.CLASS.DEFINITION applications.

Procedure

1. In the EB.TABLE.DEFINITION application, configure the below highlighted fields as shown in the below screenshot.
2. Authorise the EB.TABLE.DEFINITION application. The STANDARD.SELECTION table is updated as below.
3. In the AA.CLASS.DEFINITION application, configure the below highlighted fields as shown in the below screenshot. The STANDARD.SELECTION table is updated as below.

---


### 1.2  Component Framework


> **📇 Quick Reference Card**
> 
> **Sections:** ⚙️ Configuration


#### ⚙️ Configuration

Catalog Service is available as a Temenos Transact component. This section provides details about the APIs used to invoke this service, various flow methods and flow types.

You can invoke the catalog service using the following APIs.

| Interface API | Used By |
|---|---|
| JBC API | Other Temenos Transact components |
| C++ API | Third party systems with C++ supported technologies |
| Java API | Third party systems with Java supported technologies. |
| .NET API | Third party systems with C++ supported technologies |


##### Catalog Service Methods

This section provides details of the parameters used, their corresponding type, description and direction of flow for the various flow service methods.

| Parameter Name | Type | Description | Direction | Format |
|---|---|---|---|---|
| metaDataXML | MetaDataXML | Indicates the metadata XML for all available Temenos Transact services | OUT | For example, ServicesMetaData.xsd |

| Parameter Name | Type | Description | Direction | Format |
|---|---|---|---|---|
| serviceName | String | Indicates the Temenos Transact service name | IN | For example, Customer |
| metaDataXML | MetaDataXML | Indicates the metadata XML for the selected Temenos Transact services | OUT | For example, ServicesMetaData.xsd |

| Parameter Name | Type | Description | Direction | Format |
|---|---|---|---|---|
| serviceName | String | Indicates the Temenos Transact service name | IN | For example, Customer |
| metaDataXML | MetaDataXML | Indicates the operations metadata XML for the selected Temenos Transact service | OUT | For example, OperationsMetaData.xsd |

| Parameter Name | Type | Description | Direction | Format |
|---|---|---|---|---|
| serviceName | String | Indicates the Temenos Transact service name. | IN | For example, Customer |
| operationName | String | Indicates the service operation name. | IN | For example, getLanguage |
| metaDataXML | MetaDataXML | Indicates the metadata XML of a single operation present under the selected Temenos Transact service. | OUT | For example, OperationsMetaData.xsd |

| Parameter Name | Type | Description | Direction | Format |
|---|---|---|---|---|
| serviceName | String | Indicates the Temenos Transact service name | IN | For example, Customer |
| operationName | String | Indicates the service operation name | IN | For example, getLanguage |
| metaDataXML | MetaDataXML | Indicates the metadata XML of all the parameters available under the selected Temenos Transact service operation | OUT | For example, ParametersMetaData.xsd |

| Parameter Name | Type | Description | Direction | Format |
|---|---|---|---|---|
| serviceName | String | Indicates the Temenos Transact service name | IN | For example, Customer |
| operationName | String | Indicates the service operation name | IN | For example, getLanguage |
| parameterName | String | Indicates the parameter name | IN | For example, customerKey |
| metaDataXML | MetaDataXML | Indicates the metadata XML of a single parameter available under the selected Temenos Transact service operation | OUT | For example, ParametersMetaData.xsd |

| Parameter Name | Type | Description | Direction | Format |
|---|---|---|---|---|
| serviceName | String | Indicates the Temenos Transact service name | IN | For example, Customer |
| customizedTypeName | String | Indicates the service operation name | IN | For example, Language |
| metaDataXML | MetaDataXML | Indicates the metadata XML of a customizedType available in the selected Temenos Transact service. | OUT | For example, CustomizedTypeMetaData.xsd |

This method gets the details about the resources specified, in which Name is the input parameter and can have the values APPLICATION, VERSION or ENQUIRY.

This method gets the details about the resource type, product and component mentioned, in which the resource type can be APPLICATION, VERSION or ENQUIRY.

This method returns a list of non-obsolete applications in Temenos Transact .

This method returns an XML string containing metadata of a Temenos Transact application. The name of the application must be the input parameter to this method.

This method returns an XML string containing metadata of a Temenos Transact version. The name of the version must be the input parameter to this method.

This method returns an XML string containing metadata of a Temenos Transact enquiry. The name of the enquiry must be the input parameter to this method.

| Parameter Name | Type | Description | Direction | Format |
|---|---|---|---|---|
| serviceName | String | Indicates the Temenos Transact service name | IN | For example, Customer |
| exists | Boolean | Indicates the exists | OUT | For example, 0 or 1 |

| Parameter Name | Type | Description | Direction | Format |
|---|---|---|---|---|
| serviceName | String | Indicates the Temenos Transact service name | IN | For example, Customer |
| operationName | String | Indicates the service operation name | IN | For example, getLanguage |
| exists | boolean | Indicates the exists | OUT | For example, 0 or 1 |

| Parameter Name | Type | Description | Direction | Format |
|---|---|---|---|---|
| serviceName | String | Indicates the Temenos Transact service name | IN | For example, Customer |
| operationName | String | Indicates the service operation name | IN | For example, getLanguage |
| parameterName | String | Indicates the operation parameter name | IN | For example, customerKey |
| exists | Boolean | Indicates the exists | OUT | For example, 0 or 1 |

| Parameter Name | Type | Description | Direction | Format |
|---|---|---|---|---|
| serviceName | String | Indicates the Temenos Transact service name | IN | For example, Customer |
| customizedTypeName | String | Indicates the service customised type name | IN | For example, Language |
| exists | boolean | Indicates the exists | OUT | For example, 0 or 1 |

---


### 1.3  Connection Management


> **📇 Quick Reference Card**
> 
> **Sections:** ⚙️ Configuration | 📋 Tasks


#### ⚙️ Configuration

Connection and resource management is available for the Temenos Transact Oracle database.

This can be used to display the entity or company, the running mode for the current session and details of the COMPANY, ACTION and batch processes.


#### 📋 Tasks

Connect to the Oracle database using TAFJ runtime.

Please refer to TAFj Documentation for setting up the connection to Oracle.

---


### 1.4  Database Schema Separation


> **📇 Quick Reference Card**
> 
> **Sections:** ⚙️ Configuration | 📋 Tasks


#### ⚙️ Configuration

Database schema separation gives customers better control over their data.

Temenos Transact uses a lot of tables to hold its data. These tables are created in Temenos Transact during upgrades, updates, company creation and COB. Database Schema Separation allows you to store tables with respect to the company, or categorise them according to their functionality. This gives clients better control of the tables at database level. Schemas are enabled for any Temenos Transact table at company level and table functionality level.


#### 📋 Tasks

Database Schema Separation allows you to have schemas at company and table level for any Temenos Transact table.

Overview

Database schema separation gives customers better control over their data.

Configuring Database Schema Separation

This section details the actions required to configure Database Schema Separation.

Using Database Schema Separation

There are a number of ways in which you can create files in the schema.

---


### 1.5  Document Management


> **📇 Quick Reference Card**
> 
> **Sections:** ⚙️ Configuration


#### ⚙️ Configuration

The TRANS.DOCUMENT record stores details of contract specific documents tracked for customers in all applications other than CUSTOMER . This section provides details about the fields in TRANS.DOCUMENT and their corresponding descriptions.

You cannot reverse the records of this application. When a transaction is reversed in an application, Temenos Transact reverses all the related documents for that application in this record.

| Field | Description |
|---|---|
| ID | Indicates the ID of this application. The ID format is customer ID.* application mnemonic * transaction ID * document type ID , in which, First part - ID of the customer for whom the document is tracked Second part - Mnemonic defined for an application Third part - ID of the record for which the document is tracked Fourth part - ID of the document type |
| Reference No | Indicates the reference for the document, if any |
| Begin Date | Indicates the date from which the document is tracked in Temenos Transact |
| Status | Indicates the status of the document. |
| Status Date | Indicates the date from which the status applies to the document |
| XX LL Stat Details | Indicates the remarks on the status of the document, if any |
| Sig Date | Indicates the date on which the document is signed |
| End Date | Indicates the expiry date of the document |
| Doc Sequence | Indicates the sequence number of a document, to distinguish the new document obtained on the expiry of an old document |
| Last Upd Date | Indicates the date on which the record was last updated |
| Last Upd Appln | Indicates the application from which Temenos Transact updates the document record |
| Appln Txn Ref | Indicates the transaction reference number of the application, from which Temenos Transact updates the document record |
| Update By | Indicates if the record is updated by the user or Temenos Transact |
| Next Status | Indicates the status of the next document |
| XX LL Next Details | Indicates the remarks on the status of the next document, if any |
| Next Eff Date | Indicates the date on which the next valid document becomes effective, for tracking purposes. |
| Next Status Date | Indicates the date from which the specified status ( Next Status field value) applies to the next document. |
| Next Sig Date | Indicates the date on which signature is obtained on the next document |
| Next End Date | Indicates the expiry date of the next document |

---


### 1.6  Enquiry


> **📇 Quick Reference Card**
> 
> **Purpose:** *This document explains the ways to query and view the Temenos Transact database records and the various facilities available including Enquiry designing, data selection and generating reports.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks


#### 📖 Introduction

This document explains the ways to query and view the Temenos Transact database records and the various facilities available including Enquiry designing, data selection and generating reports.

Overview

You can seek information in the Temenos Transact database using enquires. Enquiries are statements that extract the database records based on the specified criteria.

Enquiry Facilities

This section describes about the features in Enquiry, Enquiry Selection Screen, and Enquiry Command Buttons and Sample Select.

Formatting Existing Enquiries for Browser

The layout of enquiries in browser and desktop mode are different. This section details on how the enquiries appear in desktop and browser modes and solutions to resolve the discrepancies in the appearance between these modes.

Architectural Design

This section details on how the Enquiry system is constructed in Temenos Transact . The architectural design includes the creation and modification of enquiries, data selection, modifying field data, display of enquiries in desktop and browser modes and sections displayed on screen.

Creating Report Enquiry

You can define Enquiries as a report and print on-line or at the end of day. This section details on creating report enquiries.

Setting-up Security Management System

This section details on the implementation of Security Management System (SMS) for an Enquiry at Enquiry, data, and company level and setting-up of user SMS Applications for NOFILE Enquiries.

Enquiry Extension for API

This feature enables you to define common fields to include with all API (enquiry) requests without modifying individual enquiries. The required new fields are exclusive to API requests and will be part of the OFS responses.

Nofile Enquiry Extension for API

This section details the configurations required to get the extension field or data in the OFS API response for the nofile enquiries.


#### ⚙️ Configuration

This section details on how the Enquiry system is constructed in Temenos Transact . The architectural design includes the creation and modification of enquiries, data selection, modifying field data, display of enquiries in desktop and browser modes and sections displayed on screen.


##### Creating and Modifying Enquiries

The Enquiry Wizard (toolbox plug in) and Enquiry Designer are used to create simple and complex enquiries, respectively.

> **⚠️ Note:** See Temenos Transact Toolbox User Guide for more details on Enquiry Wizard.

The Enquiry record holds the following:

- Enquiry definition
- File for selection
- Fixed selection or sort criteria
- Header details
- Display data
- Next linking Enquiry (if required).

The activated ENQUIRY.DESIGNER auto-launches the Designer Form where all settings take place. The different field parameters are summarised in the table below:

| Section | Elements | Description |
|---|---|---|
| Selection | File Name | Indicates the main file of the extracted |
|  | Enquiry Title | Indicates the title of the Enquiry appearing on the window caption |
|  | Product | Indicates the product of the Enquiry used when the Enquiry list is generated |
|  | Predefined Selection / Sort | Indicates the default selection and sort criteria applied when Enquiry is run |
|  | Selection Fields | Indicates the fields displayed in the selection panel |
|  | Op (errand) | Indicates the operand applied for predefined default selection |
|  | Mandatory | Indicates if the predefined selection is mandatory |
| Data/Column | Name | Indicates the name of the field to be processed |
|  | Heading | Indicates the field heading. This can be different from the default heading. |
|  | Col(um) | Indicates the column (order number) of the field display |
|  | Operation | Indicates the comparison, logical, arithmetic or other operators applied on field data |
|  | Type | Indicates the type for formatting (date, amount, currency, and so on) |
|  | Mask | Indicates the output length or mask for display (35L, ###, -~, and so on) |
|  | Conversion | Indicates the conversion for manipulating data prior to display |
|  | S/M | Indicates if the instruction must be processed for every multi/sub-value occurrence) |
|  | Break | Indicates if the field is processed during break conditions |
| Drill-down | Enquiry Name | Indicates the Enquiry to be linked |
|  | Selection Criteria | Indicates the selection criteria passed to the linked Enquiry, which may include data from the parent Enquiry |
|  | Label Field | Indicates the field to highlight for drill-down options |
|  | Next Level Disc. | Indicates the text to be displayed for drill-down options on pop-up menus |
| Advanced | Miscellaneous | Indicates the miscellaneous instructions (like specifying field number instead of field name, and so on) |
|  | Report Options | Indicates the report options for spooling purpose |
|  | SMS Settings | Indicates the security conditions at application, field, and Enquiry level |
| Audit |  | Indicates the system generated fields |
| Full View |  | Indicates the full view of all Enquiry fields |


##### Data Selection

The data selection can be done based on various criteria as explained in this section.

The Enquiry system is designed for single file access–all related data extracted using the data in the main file. The system reads the main file sequentially and presents data from the source record and/or associated check-files.

You can make the Enquiry run with pre-set conditions, if required. This section provides a scenario based explanation on how to specify default records selection and sorting mode.

The Enquiry in the example screen capture below selects accounts that:

- Are overdrawn—'WORKING.BALANCE LT 0'.
- Have a working balance—'WORKING.BALANCE NE NULL'.
- Have an owner (CUSTOMER)—'CUSTOMER NE NULL'.

The Predefined Sort field is set to CUSTOMER , for the records to be sorted according to the customers.

You can view the sort result in the below screen capture.

You can limit the usage of selection fields using the criteria panel. This feature is different from the fixed selection conditions discussed above.

The 'Op' and Mandatory columns indicate the operators and if the field selection is mandatory, respectively. You can modify the selection criteria by selecting the fields at design time.


##### Modifying Fields and Data

You can modify the data to be extracted from the main record, any conversions or calculations to be performed and the column for display. The Operation column indicates the instruction for the Enquiry system.

The Name defines a name for the Enquiry field and is used as a reference by other Enquiry instructions for the current value, for example, a break or total field.

If the value in Name equals any of the field names defined in the File Names field in STANDARD.SELECTION , the Operation field is defaulted to the name of that field.

You can define the column heading in this column.

| Instruction | Action |
|---|---|
| Field Name | Returns the field name and data for the current record |
| IDESC XXX | Executes the I-descriptor defined in STANDARD.SELECTION of the file, as Type I or J, with the FIELD.NAME.XXX. The result is as if the field is taken from the record. |
| SELECTION XXX | Returns the value of the SELECTION.FIELD XXX entered in the selection criteria |
| FIELD XXX | Extracts the current value of Enquiry field XXX |
|  |  |
| IF AA GT BB XXX YYY | Indicates the decision process. If Enquiry field AA is greater than BB, then process Enquiry field XXX or YYY and return the value to this Enquiry field. The valid operands are EQ, NE, GT, LT, GE, LE, RG, NR, LK, UL. This field is sub-valued to allow the decision criteria to span more than a single line for clarity. |
|  |  |
| TOTAL XXX | Totals the Enquiry field XXX |
| CALC XXX + YYY | Adds the Enquiry fields XXX and YYY |
| CALC XXX / YYY | Divides the Enquiry field XXX by YYY |
| CALC XXX * YYY | Multiplies two Enquiry fields |
| CALC XXX _ YYY | Divides two Enquiry fields |
| CALC XXX : YYY | Concatenates two Enquiry fields |
| “zzzzzz” | Uses the constant contained in quotes |
|  |  |
| !USER | Extracts the current user ID |
| !TODAY | Extracts the current date |
| !COMPANY | Extracts the current company ID |
| !LANGUAGE | Extracts the user’s language code |
| !LOCAL.CCY | Extracts the local currency code |
| !LAST.WORKING.DAY | Extracts the last working day |
| !NEXT.WORKING.DAY | Extracts the next working day |


##### Enquiry Display

You can define the format in which the Enquiry fields are displayed.

| Type | Action | Comments |
|---|---|---|
| IMAGE | Displays images | Accepts three forms of data as its argument: It can accept path. It can accept ID of the IM.DOCUMENT.IMAGE. It can accept ID of the table. |
| BAR | Displays numeric values as a self-scaling bar. Supports negative values as well. | Multiple BAR fields are allowed. |
| PIE | Displays data as a pie chart or bar graph. Holds the value to be added for the row. | Only one PIE display type is allowed per Enquiry. |
| PIELABEL | Displays data as a pie chart or bar graph. Holds the value to be added for the row. | Only one PIELABEL display type is allowed per Enquiry. |
| PROGRESSBAR | Displays numeric information as a horizontal bar, but with a fixed maximum. Negative values are not supported | Multiple PROGRESSBAR display type fields are allowed and they use the same PROGRESSAX. |
| PROGRESSMAX | Displays the maximum value of the progress bar. | Only one PROGRESSMAX display type is allowed per Enquiry |
| EDIT | Displays editable enquiries | Edits and updates the enquiry values. |
| NO-EDIT | Displays non-editable enquiries | Corresponding Target Field must be present. |
| GRAPHX | Defines the X axis values in the data as a graph | Multiple GRAPHX items are allowed – one for each series. |
| GRAPHY | Defines the Y axis values in the data as a graph | Multiple GRAPHY items are allowed – one for each series. |
| CLASS-POSNEG | Displays numeric values as a bar chart. Negative values are supported | Positive and negative bars are displayed. |
| LEGENDS | Displays a legend in the form of a coloured icon square. | Indicates data key and shows clear differences by colouring different values. |

You must set Field Disp Type to BAR to display a numeric value as a bar. These bars self-scale and show negative values. PROGRESSMAX and PROGRESSBAR display progress information and values respectively. PROGRESSBAR displays do not support negative values.

You must set Field Disp Type to CLASS-POSNEG to display positive and negative bars.

Auto scaling can be any configurable value and not just percentages. A tool tip displays the values when the mouse is hovered on the associated bar. The following example illustrates the display of bars with positive and negative values.

You must set Field Disp Type to LEGEND to display a legend as a coloured icon square.

The following example shows the Field Name and Field Disp Type fields set to BOX and LEGEND, respectively. These represent icon squares in the bar chart and a cycling palette of colours for each bar based on the stylesheet.

The GB Field Label field sets the header definition. In the below screen capture, the client labelling is set with open and close brackets.

The following example displays the legend in the left column:

If you set Field Disp Type to IMAGE , it allows direct interaction among Browser, Enquiry and Image Management. There are two uses of the image management module with browser and Enquiry. If you specify a key to IM.DOCUMENT.IMAGE , the system includes the image in that column of the Enquiry.

You can also define the display type of IMAGE for any data; for example, the cross reference tables in the IM module are used to attempt to retrieve an image. If multiple images are found, only the first is shown. For example, if you use the Customer Number field and set Field Disp Type as IMAGE , the Enquiry processing attempts to find any images for that customer number.

You must ensure that the full path specified is accessible by the client PC, or if a relative path is used, it must be accessible from the web server for the correct display of images in the browser.

In the above example Enquiry, the Info column is displayed as icons instead of text. In this case, a relative path is created as a text manipulation, and the final Enquiry field set to IMAGE. For example, a relative path used could be plaf/tec/warning.gif.

You can experiment with HTML pages first, if required.

The PIELABEL and PIE display types define the text labels and values for the items, respectively. The browser adjusts the display based on the percentage of the overall total. The pie chart ignores any negative values available.

The below screen captures show a simple balance Enquiry with two columns and result.

The below screen captures display the Enquiry with modified field display types:

You can also use the drill-down function, which can be modified using the combo box.

The setup for both bar and pie charts are the same. At present, the pie chart is the default display type, but you can modify the display during runtime.

The default setting in browserParameters.xml is to display charts and graphs in Structured Vector Graphics (SVG) format. You need to install a SVG viewer in your browser to view these items. You can also display charts and graphs in PNG format, which is configured in 'browserParameters.xml' and 'web.xml'.

> **⚠️ Note:** Refer to the Browser Installation and Configuration User Guide for further information.

In both the formats, you must ensure that the numeric values returned from enquiries are not masked with currency information or thousand separators. Masking results in error messages.

Differences between SVG and PNG

SVG offers better functionality and many features like multi-pie charts, drill-downs and other interactive features available in SVG are unavailable with PNG images. The other disadvantages of PNG images are:

- Colour of different bars in the same series are the same
- Cannot specify margin widths, legend and title locations
- Grid lines are dashed and more numerous
- Pie chart segments labelled with a text box attached by a string

The below screen captures displays a chart in SVG and PNG formats, respectively.

You must certainly define GRAPHX and/or GRAPHY display type to represent the data as a graph. The graph display handles multiple series display, and if only one GRAPHX is used, each series uses the first graph X series.

The below screen captures display the Enquiry screen and the definition of data for graphical display.

The graphical representation of the above example is shown in the below screen capture.

The values of Avg Balance , Cr Avg Bal and Dr Avg Bal use the 'X' series data. The below screen capture displays the graphical representation of the Enquiry.

The EB.ENQUIRY.GRAPH application allows you to create various types of graphs.

If you want to create a graph using EB.ENQUIRY.GRAPH , you must trigger SEARCH.LIVE.FILE and set attributes to ALLDATA . You can then open EB.ENQUIRY.GRAPH , select the respective Enquiry, set axes and legends (if any) and run the Enquiry.

> **⚠️ Note:** You must set all the required fields to ALLDATA in the respective Enquiry for the system to build the graph accurately.

In the above example screen captures, the Attributes.1 field in ENQUIRY is set to ALLDATA for the Enquiry account to be included in the ALLDATA based enquires.

Now using EB.ENQUIRY.GRAPH , you can build a graph based on the selection criteria for the above Enquiry.

The below screen capture shows a LINE.ORDINAL graph generated for the above Enquiry.

The other graph options available are BAR.ORDINAL, BAR.LINE.ORDINAL and PIE.CHART, which are displayed in the following screen captures.

You also have an option to use a current pie enquire like AM.VAL.MULTIPIE and map it to EB.GRAPH.TYPE, to allow amendments for the layout of the graph.

| Attribute | Functionality |
|---|---|
| ALLDATA | Forces the retrieval of all data before the Enquiry is displayed. |
| APPLICATION.ENQUIRY | Displays an Enquiry screen in editable mode, which becomes a record for a specific application when committed. Displays a contract screen in case of any errors. Each row in the Enquiry normally becomes a multi-value in the application record. |
| FASTPATH | Allows a user to select various records on an Enquiry and does Authorise, Delete, Verify or Reverse function of all the selected items consecutively in a single click. |
| INCREMENTAL | Indicates that the Enquiry shows all pages from 'page 1' up to the current page. Applicable for browser only. |
| MULTI.DOWNLOAD | Enables merging of multiple PDF documents prior downloading. |
| NO.BREADCRUMBS | Deletes the list of previously viewed Enquiry navigation links from the top of the screen. Used only for drilled-down enquiries. |
| NO.COLUMN.HEADER | Displays Enquiry without a header for the selected column |
| NO.ENQUIRY.FAVOURITE | Disables the access to view favourites function in an Enquiry. |
| NO.MOREOPTIONS | Disables the ’More Options’ function in an Enquiry |
| NO.SELECTION | Hides the selection criteria found at the bottom of browser fields. Applicable for browser only. |
| NO.TOOLBAR | Hides the tool bar at the top of a browser Enquiry. Applicable for browser only. |
| NORMALISE - DESKTOP | Reserved for future use |
| PAGE | Not Available in Browser |
| REALTIME | Not Available in Browser |
| REMOVE | Deletes an entry if pick operation is performed on an Enquiry grid. Applicable for desktop only. |
| SELECTION.ABOVE.DATA | Displays the selection criteria above data. |
| SELECTION.HORIZONTAL | Displays the selection criteria horizontally along screen. |
| SELECTION.SORT.ONLY | Displays selection sort only criteria. |
| SHOWTREE | Displays the first value only when an Enquiry has expanded multi-values for one field. Clicking '+' button displays all the values. |
| SINGLE.BACKGROUND.COLOUR | Displays all Enquiry backgrounds in a single colour. The default colour is white but other colours can be defined in the 'general.css' file by editing the following elements. .colour0 .hidden0 .dispaly_box .columnHeader. .caption element. |
| STATIC.PAGING.TOOL | Places the paging toolbar inside the Enquiry header at the top left of the Enquiry page |
| UNDERLINE.ALL.ROWS | Underlines all data rows in the Enquiry except the header row. The default is colour is black but other colours and thickness of the ruler can be defined in '.enq-underlineAllRow' in the 'general.css' file. |
| UNDERLINE.DRILL.ROW | Underlines all the Enquiry rows with drill-downs. The rows nominated with view and fast path checkboxes are defined as drill rows for this purpose. The default is colour is black but other colours and thickness of the ruler can be defined in '.enq-underlineAllRow' in the 'general.css' file. |
| UNDERLINE.HEADER.ROW | Underlines all the headers in the selected Enquiry record The default is colour is black but other colours and thickness of the ruler can be defined in '.enq-underlineAllRow' in the 'general.css' file. |
| VIEWLARGEICONS | Converts grid Enquiry to display records as large icons as per windows standard. Applicable for desktop only. |
| VIEWLIST - DESKTOP | Converts grid Enquiry to display records in list format as per windows standard. Applicable for desktop only. |
| VIEWSMALLICONS | Converts grid Enquiry to display records as small icons as per windows standard. Applicable for desktop only. |
| ZERORECORDDISPLAY | Indicates the unavailability of records matching the Enquiry selection criteria with a pop up message. If this attribute is active, the message pop up is suppressed and Enquiry is launched blank. Applicable for desktop only. |

The Toolbar field lists the tool IDs as a dropdown list. Based on the option selected from the dropdown, the default Enquiry toolbar is replaced with a preset toolbar configuration.

The Toolbar configuration is set in BROWSER.TOOLBAR where various tool IDs can be arranged.

The preset configuration is applied to an Enquiry record that can be reused.

When you click a dropdown in an Enquiry, a list of results are displayed. The list can have only a maximum of 200 records. You must enter the field names in the Popup Dropdown multi-valued field in ENQUIRY .

You can collapse data displayed by setting the Attribs field in ENQUIRY to HIDDEN as shown in the below screen capture.

The columns collapsible are indicated by a ‘

The below screen capture displays the Enquiry with the CUST MNEMONIC column collapsed. On collapse, the icon ‘ ’ indicating that the column is hidden. If you hover over the collapsed column header, the tooltip shows the column header.

The expand and collapse buttons in Browser Composite screens are universal and appear in the top left corner as shown in the below screen captures.

The below screen capture indicates the setup for a Composite to enable this functionality:

The TOOLBAR setup in Content Type in the above record and the ATTRIBUTE field is set to NO.FRAMES .

You can use the Col Width field in ENQUIRY to line up and word wrap screens used in Composite Enquiries.

The below screen capture shows the usage of Col Width field.

You can specify the column width (in pixels) in the Col Width field, which is applicable only for browser mode. The column width adjust to accommodate the length (short of long) of the entry and fit to the display size of the window. Fields in the same column are restricted to have the same Col Width .

> **⚠️ Note:** At present, this functionality is not operational completely with editable enquiries.


##### Display Sections

You can add footers and captions in the Enquiry reports, to display certain details.

You can add a new section to the Enquiry as a separate footer table to allow totals and so on.

You can add captions, which adds data to the title of the Enquiry. For example, you can set the window title as ‘Account Balances for Richard Branson’ instead of ‘Account Balances.

> **⚠️ Note:** Defining a caption does not save the window position information.


#### 📋 Tasks

You can define Enquiries as a report and print on-line or at the end of day. This section details on creating report enquiries.

You must set the PAGE.SIZE in Enquiry to the size of the report page for report enquires.

> **⚠️ Note:** There is no restriction on width or depth of report. All other aspects of the definition are the same.

You must enter a record in ENQUIRY.REPORT to define selection criteria, the REPORT.CONTROL ID for printer routing, default header definitions and so on to run the report.

> **⚠️ Note:** For more information, see ENQUIRY.REPORT in Temenos Transact model bank.

If you want to run the report during the end of day, you must enter the ENQUIRY.REPORT record ID in the Data field of the BATCH record for the EB.PRIN job preceded by ENQ (ENQ EB.PRIN).

This set up is explained with the ACCOUNT-LIST Enquiry record. You need not make any changes to the ENQUIRY record for XML reporting.

The set-up is as follows:

Procedure:

1. Create two files in the account '.run' directory.

1. Create XML.TRANSFORM (user-defined record name) record in REPORT.TRANSFORM for which a REPORT.CONTROL record is created.

1. Check if the Form Name field in REPORT.CONTROL displays XML ( DE.FORM.TYPE )
2. Set the Printer Id field in DE.FORM.TYPE to HOLD

> **⚠️ Note:** If this field is left blank, the system defaults the value of the Printer Id field from USER . In case of incorrect values, the browser throws the 'Unable to write banner' FATAL.ERROR)

1. Set the Form Depth field in DE.FORM.TYPE to a higher value to avoid hidden characters in the XML report. The page breaks shown as hidden characters are automatically inserted according to the form depth set in this field.
2. Set the Options field in DE.FORM.TYPE to NHEAD to suppress the header in the XML record.

1. Create and authorise the ACCOUNT-LIST record in ENQUIRY.REPORT , which details the Enquiry record to access, applicable reporting rules and output format.
2. Generate an XML report from this record using the Verify function. A new record is created in the '&HOLD&' file.

1. Open the new file in the '&HOLD&' file with Word pad to view the Enquiry in XML format.

Multi-values (not sub-values) are supported in the generated XML and are indicated in the field definitions. In the above example, the repeatable label set to TRUE indicates it. The actual fields are repeated in the data.

The application of the Enquiry report must have the STANDARD.SELECTION record rebuilt to use the new functionality. To rebuild a STANDARD.SELECTION record, open the relevant record, set the Rebuild Sys Flds field to Y , and authorise the record.


##### XML Enquiry Reports in Browser Mode

You can view XML generated reports in Browser mode as well. For this mode, you must create a style sheet for the respective Enquiry report and place it on the Web Server. For the above example, the XML style sheet in placed in the C:\Program Files\Apache Group\Tomcat 4.1\webapps\BrowserWeb\transforms\custom directory .

The Additional Data and Output Format fields in ENQUIRY.REPORT must display the location of the style sheet and output format (XML), respectively.

> **⚠️ Note:** The path specified in Additional Data is short as BrowserWeb is considered to be the top-level directory.

If you verify the record in Browser, you can an XML record in the '&HOLD&' file launched with the appropriate stylesheet.

---


### 1.7  Enterprise Deployment Pattern


> **📇 Quick Reference Card**
> 
> **Sections:** 📋 Tasks


#### 📋 Tasks

You can deploy T24PackageInstaller through an application server. This section provides the prerequisites and procedural steps to deploy the package installer in the Temenos Transact environment.


##### Prerequisites

A DSPackageInstaller.war file must be created using Design Studio, with the package that needs to be deployed into the target environment.

Show Contextual Help in the Design Studio show screen.

You can deploy the package installer using the following steps.

1. Deploy the package into the application server and ensure that the deployment is successful.

1. Create a DS.PARAMETER record, with the Force Deployment Failure field set as per the requirement. This field is set to Yes , by default.

1. Create a staging area, which will create the TAFJ.PACKAGE and TAFJ.PACKAGE.RECORD tables.

1. Write the package content into the staging area, which will feed records in the TAFJ.PACKAGE and TAFJ.PACKAGE.RECORD tables. The deployment is complete and package is available for use.

---


### 1.8  FileUpload


> **📇 Quick Reference Card**
> 
> **Purpose:** *The file upload functionality allows simple delimited files to create records in Temenos Transact .*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

The file upload functionality allows simple delimited files to create records in Temenos Transact .

Overview

This section gives a detailed description of the file upload functionality.

Using File Upload

This section provides information on how to use the file upload functionality.

---


### 1.9  Multi-language


> **📇 Quick Reference Card**
> 
> **Purpose:** *This user guide describes about the multi-lingual support feature. You can learn more about the character sets, multi-lingual definition, and translation of text.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks


#### 📖 Introduction

This user guide describes about the multi-lingual support feature. You can learn more about the character sets, multi-lingual definition, and translation of text.

Overview

Temenos Transact provides full multi-lingual translation capabilities. This section provides an overview of this feature.

Features in Multi-language

This section details the various multi-language features like application text, static and dynamic text, international character set and so on available in Temenos Transact .

Setting up Language on PC for International Mode

This section details on how to setup an additional language in the Microsoft Windows 2000 operating system.

Definition of Available Languages and Character Sets

This section details the definition of available languages and character sets in Temenos Transact .

Dictionary

This section details the usage of EB.DICTIONARY and languages supported for translation in Temenos Transact .

Layering

This section explains the system core layering and switch parameter and how layering happens for Version, Enquiry, Menu, Composite screen, and Tabbed screens with illustrations.


#### ⚙️ Configuration

This section details the definition of available languages and character sets in Temenos Transact .


##### Available Languages

Languages supported by the system are defined in the LANGUAGE application. The language code 1 is reserved for English.

The universally standard two letter language codes as defined by ISO 639-1 (standardised nomenclature to classify all known languages) to identify the locale are defined in the Iso Code field in LANGUAGE .

The values of the Iso Code field are:

- en (English)
- fr (French)
- de (German)
- es (Spanish)

A Locale is a set of parameters that define the user’s language, country and the special preferences (if any) the user wants to see in their user interface. The Amount Format field in LANGUAGE defines the locale specific number format preferences in the format.

For example, the number 12345.67 is displayed as:

| Language | Number Format | Remarks |
|---|---|---|
| French | 12.345,67 | French users prefer comma (,) as decimal symbol and period (.) as digit grouping symbol. |
| English | 12,345.67 | English users prefer the reverse format. |

> **⚠️ Note:** The number format preference set for a language can be overridden with the Amount Format value in the USER record.

You can specify the locale specific date format in the Date Format field in the USER or LANGUAGE records. However, the precedence is given for the Date Format value in the USER record.

The minimum length for the description fields in an application is three characters, considering English as the default language. This restriction is not applicable for other languages. The minimum characters restriction for description fields is defined in Min Mand Length in LANGUAGE for other chosen languages.

You can change the screen layout (right to left) using the Attributes field in LANGUAGE as shown in the below screen capture.


##### Character Sets

Some languages use additional characters to the standard Latin alphabet that are not allowed with English input. These characters have specific ASCII values, defined in the Terminal/PC character set.

You must configure the ASCII.VALUES and ASCII.VAL.TABLE applications to use these characters in Temenos Transact . You can define the acceptable characters at language, application or field type level.

Temenos Transact performs initial edit checks according to the field to ensure that only valid characters are entered. You can define a set of valid characters in ASCII.VAL.TABLE and the ASCII value of the allowed range of characters. Multiple ranges and individual characters can also be specified.

The standard record character sets for each Temenos Transact character type are released with the STANDARD.XXX key in which XXX denotes the character type. You cannot modify these records directly, but can copy and then modify as required.

The below screen capture shows a sample record TEST.A, which allows additional ASCII characters 200–220.

The ASCII.VAL.TABLE application links a type of character validation to the character set defined in ASCII.VALUES . This can be defined for

- Individual applications
- Specific language fields either at an application level or any language field level
- All fields of the specified type by default

You must view the STANDARD.SELECTION record for the application to identify the validation type for a specific field available in the associated SYS.VAL.PROG . The type for the CUSTOMER fields Short Name and Name.1 is IN2SWI as shown in the below screen capture.

The below screen capture is an example of an amended alphanumeric ( IN2SWI ) ASCII.VALUES record to allow the character set TEST.A for German ( DE ).


#### 📋 Tasks

This section details on how to setup an additional language in the Microsoft Windows 2000 operating system.

This section details on how to setup an additional language in the Microsoft Windows 2000 operating system.

This setup may differ for other operating systems. Refer to the documentation supplied with your operating system.

Procedure:

1. Regional Options . The Regional Options dialog box appears.

1. Select the languages you want to configure for the system from the Regional Options dialog box and click Set Default . The Select System Locale dialog box appears.

1. Select the required language from the Select System Locale dialog box and click Apply .

1. Click OK in the Insert Disk dialog box (as shown in the below illustration) to install languages from Windows 2000 language pack CD, the supplement with Windows 2000.

> **⚠️ Note:** You must restart the PC for the change of system Locale to take effect.

1. Input Locales. Check if the languages selected earlier appear.

1. Install Temenos Transact Browser.

> **⚠️ Note:** UTF-8 is supported from browser on jBASE 4.1. The Jbase_Code page should be set to UTF-8 field in the 'environment.vars' file of the conf directory in the TCServer must be set by default. Refer to the TC Server User Guide, for more information.

---


### 1.10  Protocol


> **📇 Quick Reference Card**
> 
> **Purpose:** *PROTOCOL is a Temenos Transact table that stores data pertaining to the activities performed by the user with additional rights. You can view these user activities in the user records. This table is available only to certain users such as security administrators.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📊 Outputs


#### 📖 Introduction

PROTOCOL is a Temenos Transact table that stores data pertaining to the activities performed by the user with additional rights. You can view these user activities in the user records. This table is available only to certain users such as security administrators.

Overview

The PROTOCOL table is updated with the transaction details of all the successful transactions that are processed through Web Browser, ARC-IB, ARC-Mobile or UXP browsers.

Protocol Log Classification

The Protocol log updates are classified into three types based on the nature of log data.

User Role Information

This section shows the functionality of the EB.USER.ROLES table, which creates logical groups and specifies the group directly in a user profile, to avoid repetition of related applications, in different user profiles.

International Resource Identifier

This functionality enables the external requests in Temenos Transact to generate an International Resource Identifier (IRI) that accompanies the transaction during its entire lifecycle. This section provides you information about the generation of an IRI and how to associate it with a transaction.

Customer Data Access Logging

Transact and TPH have a structured logging mechanism of all user activities. This mechanism is configurable in a USER profile, which ensures that all activities of the user are logged for audit purposes. This information is also available for extracts and reports, if required. The logging is now extended for every CUSTOMER involved in a transaction or Enquiry. The feature to log additional (customised) information for each of those CUSTOMER s is also available for L3 customisation.

Enquiries and Reports

This section lists the various enquiries that are triggered based on the values in the Remark and User Role Details fields.


#### ⚙️ Configuration

Transact and TPH have a structured logging mechanism of all user activities. This mechanism is configurable in a USER profile, which ensures that all activities of the user are logged for audit purposes. This information is also available for extracts and reports, if required. The logging is now extended for every CUSTOMER involved in a transaction or Enquiry. The feature to log additional (customised) information for each of those CUSTOMER s is also available for L3 customisation.

> **⚠️ Note:** This customising feature is currently available only for jBC and not for Java.

You can define a SYSTEM record using EB.PROTOCOL.PARAM . The Txn Log Required and Enq Log Required fields enable the CUSTOMER data logging for Transaction and Enquiry, respectively. You can also enable these features independently, if required. The following screen capture shows the logging enabled for both Transaction and Enquiry.

You cannot define the Customer field in the SYSTEM record and can define this field only in the specific Application or Enquiry records, if required. The Protocol Info API field allows you to attach an L3 API (jBC only) routine, which can provide additional information for each CUSTOMER involved in a transaction or enquiry request.

The Protocol Info API field accepts seven arguments as shown in the following screen capture (like any other field where an API can be attached) and must be a valid EB.API entry.

> **⚠️ Note:** This feature is currently available only for jBC and not available for Java.

The fifth argument can return key or value pairs of additional information with Tilde (~) symbol as the delimiter, to separate the key from its value. If more than one set of details must be updated, they can be returned as a multi-value set. This API, when attached to the SYSTEM record, will be invoked for all CUSTOMER s in the applications and enquiry results, if there is no other specific API defined.

You can also configure EB.PROTOCOL.PARAM for specific application and enquiry. The Customer field has any of the following values.

- A list of fields of the application which are not direct CUS fields but a customer number—one level of join to get CUSTOMER number from a field in the current application.
- A routine attached with @ symbol. This is a Temenos Transact API with one argument and must return a list of customer fields or joins.

> **⚠️ Note:** The Customer Field can contain a list of fields (definition with Joins are supported) or a routine but not both.

The CUST.FIELD.RTN routine can be with one argument returning a list of fields or joins. The following sample routine returns,

- A single field ( CUSTOMER ) for ACCOUNT
- CUSTOMER ) for FUNDS.TRANSFER .

On posting a transaction, the PROTOCOL log for application is as follows.

On launching %ACCOUNT enquiry, all CUSTOMER s involved in the enquiry (till the pages loaded per request posted) are loaded in one record.


#### 📊 Outputs

This section lists the various enquiries that are triggered based on the values in the Remark and User Role Details fields.

- USER.ACTIVITY.REPORT This enquiry is used to view the particular user activity. You can filter the specific user activity details from PROTOCOL table using the Remark field. If the Remark field is set to TRANSACTION.SUCCESSFUL.COMMIT, this enquiry displays the successfully committed files. If the Remark field is set to ENQUIRY.SELECTION.DETAILS, this enquiry displays the enquiries with selection criteria.
- USER.ACTIVITY.REPORT.ALL If the Remark field is left blank, the USER.ACTIVITY.REPORT.ALL enquiry is used to display all the activities of the user. The EB.CLEAR.FILES company wise COB job clears the PROTOCOL entries every day if the value in Process Date is less than the current day. Conversion is released to delete UAD file and other related table records in Temenos Transact , as UAD is made obsolete. Based on the value in the User Role Details field, the below enquiries are triggered by the system.
- ENQ SMS.SIGN.ON.VIOLATIONS
- SMS.USER.OPERATION.INFO

- ENQ USER.ACTIVITY.REPORT

- ENQ USER.ACTIVITY.REPORT.ALL

---


### 1.11  Report Control


> **📇 Quick Reference Card**
> 
> **Sections:** ⚙️ Configuration


#### ⚙️ Configuration

This section explains the close of business (COB) processing involved in the report control system.


##### Receive Batch Reports

It is possible to address the batch reports generated by the COB process to certain users by specifying the report names and number of copies requested in the Rpt To Receive and Rpt Copies fields of the USER records.

When the COB output is spooled, the USER record is evaluated for the details of the users who have requested reports and those details are printed on the banner page of each requested report.


##### Defer All Close of Business (Batch) output

The output of COB processing, can be held by setting the Hold Batch Output field in the SYSTEM record in the SPF application to Y . When the COB batch is run, all the output is written to the &HOLD& file on disk and not sent for spooling.

> **⚠️ Note:** When a process or job in the batch is rerun for any reason, the previous job (log) file for the process is spooled out to the printer.


##### Defer Output From Individual Batch Processes

When the output from the COB processing is not held but being spooled immediately, the output from the individual batch processes or jobs can be held by specifying a destination printer of HOLD in Default Printer and/or Printer Name fields of the BATCH record for the process.

When the COB is run, the output from the batch processes or jobs with a destination printer of HOLD is not printed.


##### Manual Spooling of Close of Business Output

The output from a previous batch run can be spooled by using the SPOOL.BATCH.OUTPUT application in V (verify) mode. This maintains a history of five batch processing start date and times with the most recent one held in record one.

The output is spooled to a single printer defined in the Dest Printer field in SPOOL.BATCH.OUTPUT in a sorted order (by department/user/report name) with a covering dispatch list.

The banner on the reports is addressed to those users defined in the USER record who have requested to receive the COB output. If any report is found with no destination user, they are addressed to the current user requesting the re-spool.

The unrequested reports can be suppressed by setting the Spool All Output field in SPOOL.BATCH.OUTPUT to N .

> **⚠️ Note:** The actual number of batch reports held in the disk depends on the report purge cycle.


##### Reports Listing Output

Two online reports are available to list the batch output to be received.

The following applications can be run online or as part of the batch.

| Application | Details |
|---|---|
| BATCH.USERS.AND.RPTS | Generates a report listing the requestors of End of Day (EOD) reports. |
| BATCH.RPTS.FOR.USERS | Generates a reports listing the End of Day (EOD) report names and receivers |


##### Report Purging

The reports are purged based on the retention period defined in the system.

The number of working days for which the report output is held on disk (&HOLD&) is specified in the Report Retention field in the SYSTEM record in SPF . The reports in the HOLD.CONTROL application for more than this period are deleted.

If the retention period for specific reports need to exceed the system wide retention period specified in SPF , it should be specified in the Report Retention field of the individual REPORT.CONTROL records.

The COB process PURGE.HOLD.RPTS, which is run in the Start of Day (SOD) batch stage purges the reports. This batch process is run daily and deletes any reports held in the HOLD.CONTROL record for more than the retention period specified in SPF and REPORT.CONTROL .


##### Interface to Microfiche System

Reports to be microfiched are specified in REPORT.CONTROL . The Microfiche Output field in REPORT.CONTROL must be set to Y .

If the microfiche system is enabled (refer SYSTEM record in SPF ), the reports are also copied to the microfiche files when created. These files are used to create output media (normally tapes) that can be sent to the microfiche producers.

---


### 1.12  System Core


> **📇 Quick Reference Card**
> 
> **Purpose:** *System Core (EB), the technical core module sometimes referred to as Application Framework, defines the key concept such as template workflow for any vertical by defining base rules for all the modes such as interactive, straight-through processing with transaction integrity.*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

System Core (EB), the technical core module sometimes referred to as Application Framework, defines the key concept such as template workflow for any vertical by defining base rules for all the modes such as interactive, straight-through processing with transaction integrity.

The software library of core module provides a fundamental structure to support the development of applications and the framework acts as the backbone structure to build any business application in Temenos Transact . It also provides common libraries that can be used by all the verticals for certain common functions.

System Core also contains all the non-banking tools (for archiving, alert generation, customizing an application, etc), and utilities (for report generation, repeated and mass level static changes, etc) that are required for core processing. EB supports Close of Business scheduling and monitoring and it also provides the framework to relevant applications to enable non-stop processing. EB provides the framework to set up user level security settings across the breadth of the software.

Close of Business and Services

This guide tells you how to set up, run and monitor Close of Business (COB) processes, using Temenos Transact , our core banking system.

Cache Reset Mechanism

The Temenos Transact system can be configured to reset the cache when operating in TAFJ runtime.

Company Local Content

This facility allows you to move data from local content into real fields and vice-versa in the Customer application.

Connection Management

To use Connection Management, you must connect to the Oracle database and set certain parameters. This feature is only available if an Oracle database is being used.

Constraints

Constraints prohibit or report certain types of activity on a portfolio or transaction, based on rules defined at the global and institutional levels.

Database Schema Separation

Database Schema Separation allows you to have schemas at company and table level for any Temenos Transact table.

Dynamic applications

Banks uses T24 to create their applications without any code. Such applications are called as Dynamic applications. They are created locally using the Temenos Transact template but do not possess the full capabilities of a T24 application.

Mass Changes

The Mass Change feature allows to effect a user driven change in a number of data records based on user-defined selection criteria. The nature of the change remains the same across all these data records.

Master Data Access Layer

Master Data Access Layer is a Temenos framework used to access the data required for a Transact application from an external system (like micro-services) using REST API.

Multi-language

This user guide describes about the multi-lingual support feature. You can learn more about the character sets, multi-lingual definition, and translation of text.

Multi-time zone

Multi-time Zone helps you to capture the banking operations according to the time zone of its geographical location.

Neighbor field

Temenos Transact framework offers a packaged methodology to define and maintain the tables. Temenos Transact acts as a master for such table definition and abstracts underlying artefacts that are created at the database layer. This methodology ensures that the definitions are in sync with the core banking application standards.

Traceability

The Traceability module generates a record of a series of actions.

Local Reference and Alternate Keys

Customised fields can be added to the existing applications.

Protocol

PROTOCOL is a Temenos Transact table that stores data pertaining to the activities performed by the user with additional rights. You can view these user activities in the user records. This table is available only to certain users such as security administrators.

Report Control

The Report Control user guide helps you to learn about the report controlling system especially on how to spool a report, how to hold a report, how to restrict viewing a report and how to purge a report.

Enquiry

This document explains the ways to query and view the Temenos Transact database records and the various facilities available including Enquiry designing, data selection and generating reports.

Catalog Service Component Framework

Catalog Service is an independent component and acts as a resource to support the Temenos Transact Integration Tooling and implementation teams of the client banks to develop the interfaces to Temenos Transact. This service contains a list of operations categorised by its parent service. For example, under CustomerService , the operations getPhysicalAddress , getAccountOfficer and so on are listed. This user guide explains the catalog flow service operations and their corresponding flow methods and types.

Enterprise Deployment Pattern

Enterprise Deployment Pattern (EDP) is an industry standard to indicate that any data artefact deployed to the system must be sent to the database instead of user directories. This guide describes the advanced deployment process of T24PackageInstaller and sample package content for both successful and unsuccessful deployment scenarios.

Document Management

Document Management (DM) enables bank to manage the documents received from customers for various purposes at transaction level. This guide explains the design and processing with examples.

File Upload

The file upload functionality allows simple delimited files to create records in Temenos Transact .

Auto Unique ID Generation

The Auto Unique ID Generation facility allows Transact to generate unique IDs for transactions using the underlying Platform (TAFj) Function, to improve the performance.

Transact Monitoring Using Grafana

This feature facilitates to log the information of transactions such as online and batch into Grafana , which is an external monitoring tool. For more information on Grafana, see Monitoring Solution .

Supporting Other Date Formats

Temenos Transact is based on Gregorian calendar, which is the standard business calendar used in the international banking markets. This section guides the banks to enter the date, based on its country specific calendar such as Hijri or Ethiopian for creating transaction.

Cloud Operation Efficiency

Temenos Transact provides utilities to perform the cloud operations more efficiently. This section describes how to improve the cloud operations effectively.

Standards and Restrictions in SaaS 2021 (SS2021)

When installing Transact through SS2021, certain restrictions are enforced during implementation. This section describes the restrictions in adding applications and new routines to various user exits, and amendment of existing routines and records in an application.

Support for JWT Based Login

This section helps you to configure JSON Web Token (JWT), which is a security token validation.

Warmup in Transact

Warmup functionality helps to reduce the time taken for the transactions to complete. This guide explains required configuration of the Warmup functionality and details of supported applications.

Data Events in Transact

Temenos Transact can emit the Data Event Streaming (DES) as Data Events. This section explains the required configuration to emit Data Events for Temenos Transact application.

Grouping of Events

Transact can organise events into groups, each event belonging to a single group, though multiple events can be part of the same group.

---


### 1.13  COB


> **📇 Quick Reference Card**
> 
> **Purpose:** *This guide tells you how to set up, run and monitor Close of Business (COB) processes, using Temenos Transact , our core banking system.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks


#### 📖 Introduction

This guide tells you how to set up, run and monitor Close of Business (COB) processes, using Temenos Transact , our core banking system.

Overview

This topic provides an overview of Close of Business, the most important T24 activity. The COB process pulls together all the financial events of the day for the bank and processes them.

Configuring the COB

These topics show you how to set up the COB. They describe how to create the COB record, set timeouts and configure automation settings. There is also a reference to COB parameters.

Running the COB

These topics show you how to start the COB, run multiple COB processes or a COB for a specific company. It also shows you how to stop the COB gracefully on specific servers, and provides a reference to agent utilisation and list files.

Monitoring the COB

These topics describe how to monitor COB processes using both enquiries and tools. They also tell you about COB status information and the Write Cache facility.

Reporting

These topics describe the COMO and how to pull reports on the COB.

Handling Exceptions

This topic shows you how the system handles critical and non-critical errors in the COB.

Scheduler and Dynamic Profile

This feature allows a bank to be able to run specific jobs in the specific COB stages, but without adding the jobs to the COB related Batch records.

Service Processing using IRIS APIs

IRIS R18 is a lightweight, standalone component of Temenos Interaction Framework. Provider APIs are simple services that expose specific core capabilities as a proprietary API. These APIs are building blocks that expose Temenos business capabilities as RESTful APIs defined in Open API Specification (Swagger).

Scalability

This section describes the scalability mechanism used in COB.

Elastic Scaling of Agents

This feature allows you to have an option for services or COB to have dynamic agent allocation based on time, queue depth and job.

Services

This section details the features that enhances the processing of service framework's online services.

Tidying up the Jobs

This section describes how tidying up of an individual job is performed.

Verifying Pre-COB Services

This section explains the pre-checks performed for COB services.


#### ⚙️ Configuration

This topic provides an overview of Close of Business, the most important Temenos Transact activity. The COB process pulls together all the financial events of the day for the bank and processes them.

Those events can include everything from loan schedules, accruals and internal bank accounting to reports. They are always scheduled for processing on a specific day. The COB is a scalable, high performance mechanism for carrying out this process. It is also highly reliable in terms of recovery.


##### How the COB Works

Temenos Transact Batch Processing is handled by the COB. The COB is used to:

- Process events.
- Calculate and post interest.
- Roll the bank date forward.
- Produce reports.


##### COB Stages and Sequences

The COB triggers various activities based on the scheduled date and any specific conditions that are set. It consists of five stages:

The COB runs various processes, based on the above stages. The COB runs processes in a set order within each stage, based on the sequence number.

Each batch stage consists of a number of processes with the same or a different sequence number. Each number corresponds directly to records in the BATCH file and each process consists of a number of jobs. The jobs are routines defined in the PGM.FILE file as type B . Each batch process defines:

- The stage and sequence at which the process runs.
- The jobs that run.
- The frequency at which the process has to run.

The stage and the sequence of the batch process are never violated - this ensures data integrity and the proper processing of jobs, as some jobs are dependent on an earlier stage of the COB.


##### Non-Stop Processing and the COB

The Non-Stop (NS) processing and COB services complement each other. The COB does not allow the input and processing of records in applications, except for those supported by the NS service.

The applications that are available in NS stop service are available without any restrictions. They use the next working date for processing. This ensures that concurrent transactions are not picked up for processing by the COB, which runs in parallel.

To achieve this, the COB distinguishes the dates by two different records per company in the DATES application. At the start of the COB, the COB cycles the date record and restores the old dates record with the key as CO.CODE-COB. This means that:

- All COB processing happens based on the COB record in DATES.
- Online processing happens based on the cycled record in the DATES application.


##### Static Cache

The static cache is cleared only when the batch stage changes. To reset the static cache for each job in that batch, the CLEAR.STATIC.CACHE field in BATCH record is set as YES.


#### 📋 Tasks

This topic shows you how to configure the automation settings, including limits on start times and the number of COB runs.

Procedure

1. To make sure that the COB service starts after 18.30, the end of the banking day, and doesn't start after 24.00 (midnight), set the MIN.START.TIME and MAX.START.TIME fields in TSA.SERVICE.
2. To prevent unintended runs - so that the COB doesn't run more than 2 times a day, for example - set the NO.OF.RUNS.PER.DAY field in TSA.SERVICE.

> **⚠️ Note:** The automation settings also support the API's link with IRIS, our Interaction Framework.


##### Resolving EOD Errors Automatically

This feature allows you to automatically update the Date Resolved field in EB.EOD.ERROR .

Procedure

In TSA.SERVICE, set the following fields and then authorise the record:

- Attribute Type to UPDATE.EEE
- Attribute Value to Yes .

The following screen capture is a sample EB.EOD.ERROR available in the environment, after the completion of COB.

During authorisation of TSA.SERVICE, the system automatically updates the eligible EB.EOD.ERROR records in the Date Resolved field. The current Transact date (today) is updated in the Date Resolved field as shown in the following screen capture.

> **⚠️ Note:** The Date Resolved field is updated only for the multi-values, for which the Fix Required field is set to YES . These are blocker errors, without resolving these errors, COB cannot be initiated.

---


### 1.14  Service Automation


> **📇 Quick Reference Card**
> 
> **Sections:** ⚙️ Configuration


#### ⚙️ Configuration

This section describes the validations against the Feeder Queue field and the framework design of auto service process.

The service records EB.FEEDER.PREPARE and EB.FEEDER.EXECUTE should always be in AUTO operation.

The validations of the Feeder Queue field are given below:

- It does not allow the input when the operation is not AUTO or STOP.
- Validation in the BATCH and TSA.SERVICE reports error when there are verification jobs defined. Sample view of batch record with verification JOB is given below. Defining Feeder Queue is not allowed in TSA.SERVICE record since job in batch record is set with verification. Sample feeder queue enabled service is given below. Verification is not allowed in Batch when the service is feeder queue enabled.
- Validation in TSA.SERVICE and PGM.FILE reports an error when there is ACTIVIATION enabled in the job. Sample Batch record defined with activation enabled job is given below. Defining FEEDER.QUEUE is not allowed in TSA.SERVICE record, since job in batch record is activation enabled. Activation files enabled jobs are not allowed in Batch when the service record is feeder queue enabled.
- Validation in the TSA.SERVICE and BATCH, to report an error when the job is not multi-threaded. Sample Batch record defined with single threaded job Defining FEEDER.QUEUE is not allowed in TSA.SERVICE record, since job in batch record is single threaded. Single threaded jobs are not allowed in Batch when the service record is feeder queue enabled.

> **⚠️ Note:** tSM ignores feeder jobs. It does not start or include the services marked for feeder processing. The sample view of TSA.SERVICE records in START and AUTO status is given below. The FEEDER.QUEUE enabled services are not selected by tSM.


##### Auto service EB.FEEDER.PREPARE

It is a standalone service that runs in AUTO mode.

- It acts as the governing service for other services similar to the tSM.
- It selects all TSA.SERVICE with FEEDER.QUEUE defined and are set with the SERVICE.CONTROL as AUTO.
- It then populates each selected service name into the feeder queue.
- Each service is considered for processing and do the following: Invoke the .LOAD of the service, if it exists Invoke the .SELECT of the service Push the selected contract keys to the specific feeder queue configured for the service (in TSA.SERVICE) The content pushed to the feeder queue has the following information: Company Mnemonic Service name Actual contract key

The flow how EB.FEEDER.PREPARE works is shown below.

The FEEDER.QUEUE will be created if it does not exist already. Feeder queues are created during authorisation of TSA.SERVCIE record; Else, they are created during process time.

Sample TSA.SERVICE record is defined with FEEDER.QUEUE and the file does not exist. Hence it is created during process time of feeder service.

The individual services marked as FEEDER.QUEUE do not populate its own F.JOB.LIST. Instead each of them populates the keys into the specific FEEDER.QUEUE file.

Sample view of TSA.SERVICE records defined with FEEDER.QUEUE is given below.

You should run the EB.FEEDER.PREPARE service to enable the auto service.

For feeder services FBNK/OFS.MESSAGE.SERVICE and BNK/EB.ENTITLEMENT.SERVICE , the keys are updated in feeder queue F.FDR.Q.OFS.MSG as defined in TSA.SERVICE record.

The contract keys hold the feeder Service Company mnemonic and service name along with key.


##### Auto service EB.FEEDER.EXECUTE

It is a standalone service that acts as a wrapper service that serves a feeder queue.

Each feeder queue to be served must have one instance of the EB.FEEDER.EXECUTE running and the Data field of each batch specifies the queue name to serve. Only one feeder queue can be passed in this field and multi valuing it for feeder execution is invalid since feeder execute is supposed to serve only one queue at a time. If a queue name is not mentioned in the field, the execution skips this job without processing it and the information is logged in COMO to indicate the job is being skipped.

The flow how EB.FEEDER.EXECUTE works is shown below.

Sample view of Batch record to process the feeder queue F.FDR.Q.OFS.MSG is given below.

TSA.SERVICE record BNK/EB.FEEDER.EXECUTE.1 is given below.

The number of records in feeder queue F.FDR.Q.OFS.MSG are shown below.

You should run the BNK/EB.FEEDER.EXECUTE.1 service to enable the auto service.

---


### 1.15  Warmup


> **📇 Quick Reference Card**
> 
> **Key Fields:** *Application*, *Local Routine*, *Read Api*, *Read Api Info*, *Record Id*
> 
> **Sections:** ⚙️ Configuration | 📋 Tasks


#### ⚙️ Configuration

This section provides details about configuring the components involved in executing the warmup feature.


##### Configuring Platform Framework – TAFJ

To configure TAFJ for the warmup feature,

1. Go to ..\Temenos\jboss\standalone\deployments\TAFJJEE_EAR.ear\TAFJJEE_EJB.jar\META-INF\ .
2. Modify the ejb-jar.xml file as shown in the below screen captures.

TAFJ is configured successfully for the warmup feature.


##### Configuring REDIS External Cache

Redis is an external open source caching system, which temporarily stores information as key value structures. Transact loads into its internal cache bucket if REDIS mechanism is not used, thus making it optional.

To configure REDIS external cache for the warmup feature, go to .../TAFJ/Conf/tafj.property and set the below properties.

- Specify if you have to use external distributed cache for Transact temn.tafj.runtime.use.external.caching = true
- Specify the host name to access shared distributed cache temn.tafj.cache.host=127.0.0.1
- Specify the port to access shared distributed cache temn.tafj.cache.port=6379

REDIS is configured successfully for the warmup feature.


##### Configuring Transact

You need to configure warmup in Transact at the individual channel level. To configure Transact for the warmup feature,

1. Identify the channel ( OFS.SOURCE ) based on the nature of the channel’s business transaction
2. Add the attribute WARMUP to the identified channel ( OFS.SOURCE ) to indicate that the channel requires a warmup.


#### 📋 Tasks

This section details about the EB.WARMUP.GROUP and EB.WARMUP.SESSIONS applications that support Warmup functionality in Transact.


##### EB.WARMUP.GROUP

The EB.WARMUP.GROUP application stores the list of applications and their record IDs in an associated multi-valued set. You need to identify the list of applications and keys in the application, that must be preloaded (cached) as part of the warmup activity and define the same in EB.WARMUP.GROUP .

You can also do the following using this application:

- Define all keys, using the asterisk (*) symbol in the Record Id field.
- Attach local routine (API) for any custom definition for caching if the definition using direct names is difficult. This option is useful if the record to be cached is a derived key and not a direct key on the application.

The below sections offer the recommended best practices for defining the EB.WARMUP.GROUP .

You need to configure the list of applications and their corresponding record IDs in the Application and Record Id fields respectively for caching process. The Application field is an associated multi-value set and Record Id is a sub-value set for the Application field.

You can enter asterisk (*) in the Record Id field to cache all records of the application.

Local Routine is a multi-value field in which you can attach multiple jBC routines. Every routine must have a valid EB.API definition.The local routine which the client or any local development team is writing should restrict to use only cache read in the code as shown in the below coding snippet as part of the caching process. You need to use Local Routine judiciously and only when required. Application Framework does not impose any sort of restriction on what can be done within this user exit.

The below screen capture shows a sample subroutine for reference and signature purpose. The API does not take any arguments and does not return any value.

Temenos offers a common API— EB.PRE.LOAD.DATA , out-of-the-box, to the clients to cater to most common caching recommended by Temenos when required, as part of the Warmup procedures.

The following are some of the configurations that you should never do in local routines as part of Warmup. These are just recommended practices. However, application framework does not have any sort of restriction on the usage of these.

- Expensive IDESC calls or loading them as part of the warmup
- Call OFS.BULK. MANAGER to do warmup transactions
- Avoid the calls to core routines as part of warmup like CHECKFILE.VALIDATION or F. READ
- Judicious usage of core API - LOAD.COMPANY
- Avoid extensive READs on files/tables
- Many files/records warmed up in a session
- Many user routines The best practice is to have a maximum of three user routines
- Avoid writing complex user routines in the warmup
- Loading transactional (non-static) data as part of the warmup


###### CachingLOCAL.TABLE

To cache LOCAL.TABLE , you need to do the following:

- Define the keyword CACHE.LOCAL.TABLE in the Application field
- Configure the list of record keys in the Record Id field
- Enter the common API EB.PRE.LOAD.DATA in the Read Api field

The system also supports a custom savedlist in the definition along with the fixed list of IDs. For processing through Savedlist, the record ID must begin with SL - which is a valid definition. The system ignores missing and/or empty files and will not lead to any crash or errors being reported.


###### CachingEB.OBJECT

To cache EB.OBJECT , you need to do the following:

- Define the keyword CACHE.EB.OBJECT in the Application field
- Configure the list of record keys in the Record Id field
- Enter the common API EB.PRE.LOAD.DATA in the Read Api field

The system also supports a custom savedlist in the definition along with the fixed list of IDs. This is a valid definition and is duly processed from the &SAVEDLISTS& definition if it is available and accessible. The system ignores missing and/or empty files and will not lead to any crash or errors being reported.


###### CachingEB.LOOKUP

To cache EB.LOOKUP , you need to do the following:

- Define the keyword CACHE.EB.LOOKUP in the Application field
- Configure the list of record keys in the Record Id field
- Enter the common API EB.PRE.LOAD.DATA in the Read Api field

The system also supports a custom savedlist in the definition along with the fixed list of IDs. For processing through Savedlist, the record ID must begin with SL - which is a valid definition. The system ignores missing and/or empty files and will not lead to any crash or errors being reported.


###### Cache Classes

If there are a list of classes to preload instead of records, then the keyword CACHE.CLASSES can be defined. There are certain validations and checks, that are necessary for using this. These are explained below.

To cache classes, you need to do the following:

- Define the names of the classes in the Read Api Info field
- Set the Record Id field to null
- Enter the common API EB.PRE.LOAD.DATA in the Read Api field

The system also supports a custom savedlist in the definition along with the fixed list of IDs. For processing through Savedlist, the record ID must begin with SL - which is a valid definition. The system ignores missing and/or empty files and will not lead to any crash or errors being reported.


###### CachingSTANDARD.SELECTION

To cache STANDARD.SELECTION , you need to do the following:

- Define the keyword CACHE.STANDARD.SELECTION in the Application field
- Configure the list of record keys in the Record Id field
- Enter the common API EB.PRE.LOAD.DATA in the Read Api field

The system also supports a custom savedlist in the definition along with the fixed list of IDs. For processing through Savedlist, the record ID must begin with SL - which is a valid definition. The system ignores missing and/or empty files and will not lead to any crash or errors being reported.


###### Caching OPF

To cache OPF , you need to do the following:

- Define the keyword CACHE.FILE.OPEN in the Application field
- Configure the list of record keys in the Record Id field
- Enter the common API EB.PRE.LOAD.DATA in the Read Api field

For caching OPF, you can input four ways in the Record Id field. The following formats are supported for this configuration.

- filename
- filename
- filename
- 

This configuration supports any combination and order. However, you need to keep a check on the company switch if there is a change in the company, the company gets reloaded to open the file in that company. Care must however be taken with the company switch, as each change in company results in the company being reloaded to open the file in that company. So, Temenos recommends ordering the records by company as a preferred definition.

The below sample list file SL-MY.CUSTOMER.OPF.LLIST.txt displays the definitions that are permitted.


##### EB.WARMUP.SESSIONS

This application acts as the starting point for the warmup framework in Transact. The framework looks for a matching definition in this application for the Channel Name ( OFS.SOURCE ). This application allows to configure multiple EB.WARMUP.GROUP s, which will be referred during actual warmup, to understand the content to be cached.

The @ID of the application is the OFS.SOURCE for which the records are cached per session.

---


### 1.16  Mass-changes


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Mass Change feature allows to effect a user driven change in a number of data records based on user-defined selection criteria. The nature of the change remains the same across all these data records.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks


#### 📖 Introduction

The Mass Change feature allows to effect a user driven change in a number of data records based on user-defined selection criteria. The nature of the change remains the same across all these data records.

Overview

This section lets you get familiar with the key concepts in Mass Changes.

Mass Change Utility applications and services

This section describes the configurable Mass Change Utility applications and services.

Setting up Mass Change Instructions

This section details the working of various tasks available in Mass Change instruction.

Performing MCI tasks

This section shows you how to perform business operations such as change branch, change debit or credit interest, change product, etc.

Reversing Mass Changes

This section shows how to revert the Mass Changes.

Features in Mass Change Utility

This section helps you to perform various processes needed to execute a Mass Change Instruction.


#### ⚙️ Configuration

This section details about the source and target preview enquiries. It is possible to customize these enquiries and automatically incorporate them into the MCI workflow.

There are certain Mass Change business operations that could affect different Temenos Transact tables. In such cases, when you preview the source and target records, incorrect information may be displayed.

The Preview Monitor Enquiries in the Temenos Transact Model Bank for an MCI helps you to drill down these source and target preview enquiries. You can also customise these preview enquiries so that they can automatically be incorporated into the MCI workflow.

The Preview Monitor Enquiries has the following key points:

- The defaults A preview enquiry for source records is EB.MCI.S.P.DEFAULT A preview enquiry for target records is EB.MCI.T.P.DEFAULT
- The Preview Monitor determines which target preview enquiry to launch. It launches the enquiries in the following order: Enquiry named EB.MCI.T.P. Name of the business operation Enquiry named EB.MCI.T.P. Temenos Transact application of the business operation Enquiry named EB.MCI.T.P. AA Property Class of the business operation If none of the above enquires are launched, then it will launch the EB.MCI.T.P.DEFAULT. It is a default enquiry that displays upto the first four attributes of the target application, target attribute’s old value and new value.

> **⚠️ Note:** The Mass Change Instruction executes the instructions on the target record by invoking exactly the same target application and its business logic.

The Monitor Enquiries can become heavy for big execution size. It may be a good idea to index the fields TXN.REF and EXEC.STATUS in EB.MCI.EXECUTION.DETAILS.

It is recommended that the maximum execution size for especially AA Business Operations to be kept to 999 so that they are both controllable, observable and not affecting the system performance.

The Mass Change Instruction utility is not a ‘correction’ utility. Those requirements need to be addressed by IT or System Administrator with a purpose built procedure. The Mass Change Instruction is focused on effecting the changes required by either business managers or relationship managers, where the target changes are almost always driven by a Group of Customers or Customer Group.

Depending on the nature of such Mass Change requests and other transactional volumes, it is recommended to dedicate one application server just for Mass Change executions so that they don’t get in the way of actual user and channel transactions.


#### 📋 Tasks

This section shows you how to perform business operations such as change branch, change debit or credit interest, change product, etc.


##### Performing a change debit interest

To change debit interest,

1. Mass Change Instruction .
2. Click the New Instruction option.
3. In the Business Operation screen, click the Change Debit Interest option.
4. In the Preview screen, enter values in the following fields: Reason Processing Date Effective Date
5. In the Selection Criteria tab, enter a value in the following field: Target Field
6. Click the Validate icon to check for errors and overrides.
7. Click the Commit icon.


##### Performing a change customer static

To change customer static,

1. Mass Change Instruction .
2. Click the New Instruction option.
3. In the Business Operation screen, click the Change Customer Static option.
4. In the Preview screen, enter values in the following fields: Reason Processing Date Effective Date
5. In the Selection Criteria tab, enter a value in the below field: Target Field
6. Click the Attribute Changes tab and enter values in the following fields: Action Attribute MV SV Value Condition Lookup
7. Click the Validate icon to check for errors and overrides.
8. Click the Commit icon.

---


### 1.17  Neighbor


> **📇 Quick Reference Card**
> 
> **Sections:** ⚙️ Configuration | 📋 Tasks


#### ⚙️ Configuration

This section helps you to get familiar with the key concepts of neighbor field feature and how to add fields in an existing application.

The table definitions offered by Temenos Transact are called as templates. These templates are exposed through versions and queried through core banking enquiries. Core banking helps you to define templates through code and also through a code-less mechanism. The Neighbor field feature aims to improve the table definition mechanism, so that the maintenance of the existing applications or tables is more effective.

The following are the key concepts of Neighbor field feature:

- The Neighbor field feature facilitate the addition of new fields to an existing template without changing its layout.
- You can use this feature when there are no reserved fields available in the field definitions. In Temenos Transact , the applications are defined with maximum reserved fields to simplify the conversion process. You can add new fields by renaming these reserve fields in the existing application without changing the field position.
- You can avoid future conversion process to ensure that the field values are stored in its relative positions. This is done to ensure that new field definitions are added after audit fields upon record commit. This is called physical order data record in database. This happens according to the physical position defined for each added field. In this way you can avoid conversions as existing data in database does not require conversion. This Neighbor field feature gives you the ability to convert this physical order record into a logical order for display. Therefore, there is no change in the layout of the existing application.


##### Difference between framework and application

Frameworks and applications have a clear distinction on how to refer to a field position.


##### Framework

Framework provides the following features:

- It does not look for a value with physical position.
- Ensures that only logical position is maintained.
- They are generally not distinguished between applications and cannot use hard-coded position.
- Uses the definition of template to understand logical field position.
- Provides the record or the copy of record in physical order.


##### Application exit points

Applications provide the following features:

- Applications always refer to physical positions.
- Applications refer to records and any definition parameters in the physical order.
- Applications do not loop through a record and assume logical positions.


#### 📋 Tasks

This section shows the setup of adding an existing dynamic application with new fields using the neighbor field feature.

1. Use an existing dynamic application created through EB.TABLE.DEFINITION.
2. Specify the field name that you want to add in the FIELD.NAME field. This will auto-populate the PHYSICAL.POSITION field.
3. Authorize the application. This will update the following fields of STANDARD.SELECTION: SYS.FIELD.NO PHYSICAL.ORDER LOGICAL.ORDER


##### Example

The following example shows the addition of two neighboring fields JOINT.HOLDER.ADDRESS and MOBILE.NUMBER in an existing dynamic application.

- You can add special fields through ADD.SPECIAL.FIELDS available in EB.TABLE.DEFINITION. These special fields are XX.LOCAL.REF, XX.DELIVERY.REF and XX.STMT.NO.
- This special field can also adapt for neighbor feature when it is added in the corresponding application. Its PHYSICAL.POSITION stored in STANDARD.SELECTION is used by the system for any further processing of this application field.
- The PHYSICAL.POSITION value of a newly added field gets supplied to the 15 th position of this field’s T array and the same is updated in its STANDARD.SELECTION.
- The array conversion order gets updated in PHYSICAL.ORDER and LOGICAL.ORDER fields of STANDARD.SELECTION during authorization of record in EB.TABLE.DEFINITION.
- If AUDIT.DATE.TIME value is 25 in STANDARD.SELECTION of this dynamic application, then PHYSICAL.POSITION for first neighbor (new) field should be AUDIT.DATE.TIME + 1 = 25+1 = 26 and PHYSICAL.POSITION for second neighbor field should be Highest physical position used + 1 = 26+1 = 27
- Any neighbor field added to an application will have its corresponding details updated in STANDARD.SELECTION as shown below.
- The generated insert also contains the new neighbor fields with physical position pointed.

---


### 1.18  Archiving


> **📇 Quick Reference Card**
> 
> **Purpose:** *Temenos Transact archive reclaims the disk space by moving or removing historic data that is no longer required from the live database.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks


#### 📖 Introduction

Temenos Transact archive reclaims the disk space by moving or removing historic data that is no longer required from the live database.

The system performs the following to archive the historic data:

- Looks for records to be archived in the files.
- Writes the selected records (and related records, if specified) to a $ARC archive file—that ideally resides on a different disk, or a separate machine accessible through a network.
- Deletes these records from the live database.

> **⚠️ Note:** You may also simply delete the data without archiving them.

Configuration

This section explains the configuration steps and field settings pertaining to ARCHIVE and ARC.GENERIC.REQUEST applications in Temenos Transact.

Prerequisites

This section explains the conditions and processes to be followed before archiving the data.

Segmentation

Segmentation is the process of multi-threading the job processing by splitting the entries between available agents.

Illustrating Post Archiving Actions

This section explains the various actions that are performed after archiving the data.


#### ⚙️ Configuration

This section explains the configuration steps and field settings pertaining to ARCHIVE and ARC.GENERIC.REQUEST applications in Temenos Transact.


##### ARCHIVE

Create a record in ARCHIVE for the files to be archived, as the files to be archived must have an entry in ARCHIVE application.

The below table explains the required field settings in the ARCHIVE application.

| Field(s) | Description |
|---|---|
| Descriptn.1 , Descriptn.2 , Descriptn.3 and Descriptn.4 | Indicates the four distinct sections in this record |
| Purge Date and Retention Period | System selects the record to be archived, based on the dates specified in either the Purge Date or Retention Period field. The selected records are archived (or deleted). Purge date is automatically calculated from retention period, during runtime. If today's date is 23 May, 2012 and the retention period of three months is specified (03M), the three month period is calculated from the beginning of the current month. Therefore, records dated before 1 February, 2012 (purge date) are archived (or deleted). |
| Archive Data | Indicates whether the selected records need to be archived or deleted, with respect to the value in this field. Y – Archive N or None – Delete |
| Arc Pathname | Specifies the destination location of the $ARC archive files. If this field is blank, the $ARC files are created in the archive directory (BNK.arc). |
| Arc Filename | Indicates the names of all the $ARC files that are created based on the specified type and modulo. If the type and modulo specification are not present, the ARC files inherit these details from the corresponding live files. It is a multi-value field. |
| Company Run In, Time Started, User Id, Date Selected, Stop Requested, Recs Deleted, Recs Processed, Error Msg, Time Ended | Maintain a history of the archives. The system populates these multi-value fields after the contracts are archived. |
| Generic Method | Indicates whether the generic archival process may be executed or not, with respect to your input. Y – Executes generic archival process. This allows archival service (ARC.GENERIC service) to look after all selection and purging of records. FUNDS.TRANSFER , TELLER , STMT.ENTRY.DETAIL and so on are archived through the generic archival process, with respect to the values input in Main File , Field To Check or Filter Routine fields. No or None – Application specific archival routine specified in the Routine field is invoked. |
| Main File | Accepts the file name (for example, FUNDS.TRANSFER$HIS) input that has to be archived. If this field is multi-valued and populated with two or more applications, the date mentioned in Field To Check is applicable to the application specified in the first multi-value field. |
| Field To Check | Indicates the date field in the contract, which is compared with the Purge date for archiving. If this field is blank, the standard Date Time field is used for comparison. In order to archive the history records of the FUNDS.TRANSFER record, use the Processing Date of the contract. |
| Filter Rtn | It is a hook routine to select or ignore a contract for archiving. This field is an alternate to Field To Check field. The IN and OUT parameters of this routine are: IN Parameters Id Contract – Indicates the record key of the contract R Contract – Indicates the entire contract record OUT Parameters Contractarchive Date – Indicates the date against which the purge date set in the ARCHIVE record is compared. In FUNDS.TRANSFER, you may compare debit value and credit value date of the contract and return a final date as the OUT parameter, which is compared with purge date for archival. Skip Flag – Returns ‘1’ as the OUT parameter, which confirms that the current contract need not be archived. Logic to ignore the contract is available in the filter routine and the current contract is skipped from being archived. Two spare parameters for future expansion. |
| Related Files Rtn | It is a hook routine that returns the names of related files that have to be archived along with the main archival record in a dynamic array.The IN and OUT parameters of this routine are: IN Parameters Id Contract – Indicates the record key of the main contract that is ready to be archived R Contract – Indicates the entire contract record OUT Parameters Related Files – Indicates the information of related files to be archived in 'file name, file ID, archival flag separated by @VM' format. If there are multiple related files, each file information is delimited by @FM marker. Upon archiving LOANS.AND.DEPOSITS records, file records to be archived are balanced. So, pass the balances file name, its ID and a ‘Y’ to the Archival flag. Two spare parameters for future expansion. |
| Routine | Indicates a valid multi-threaded routine that is responsible for archiving the set of files specified in the ARCHIVE record. These are application specific routines that should not be changed unless a site specific program is written. For FOREX , the routine is ARC.FOREX. This record routine is responsible to decide the archival logic and perform the archival. Separate ARC.FOREX.LOAD and ARC.FOREX.SELECT routines must be available for opening and selecting all necessary files for archiving. However, it is not necessary to create a separate ARC.FOREX service. It is the responsibility of ARC.GENERIC service to simply invoke ARC.FOREX.LOAD, ARC.FOREX.SELECT, ARC.FOREX routines internally for archiving in the presence of Routine field. |


##### ARC.GENERIC.REQUEST

Create a SYSTEM record in ARC.GENERIC.REQUEST and specify the Archive Id for archival. Upon verification of this record, ARC.GENERIC service starts in the background and reads the ARCHIVE record. Based on the Generic Method set-up or the application specific Routine , the records are selected for archival. Ensure that TSM is already running.


#### 📋 Tasks

This section explains the various actions that are performed after archiving the data.


##### Review Process

Once the archiving process is complete, the size of all the files involved (both original and $ARC) are reviewed to predict the next number of records in the relevant files to be archived.


##### Report generation

The following details are stored in the respective ARCHIVE record for future reference:

- Total number of records selected for processing
- Total number of records archived or deleted

The above screenshot shows that, 780 contracts were selected for archival out of which 749 were removed from FUNDS.TRANSFER$HIS and archived in FUNDS.TRANSFER$ARC file.


##### Accessing the Archived Information

The archived information are written to the files with the suffix $ARC. The $ARC files use the same layout as the files from which they are created. For example, the layout of RE.CONSOL.SPEC.ENTRY$ARC is the same as RE.CONSOL.SPEC.ENTRY .

The archived files can be viewed using the Temenos Transact ENQUIRY utility, by creating an enquiry to view the archived files. This enquiry can be a copy of an enquiry on the archived file, upon setting the File Name to the name of the archived file.

For example, an enquiry to view the CATEG.ENTRY$ARC file is based on the List of PL entries (CATEG.ENTRY) enquiry, upon changing the File Name to CATEG.ENTRY$ARC.

The enquiry creation on FUNDS.TRANSFER$ARC is shown in the below screenshot.

---


### 1.19  Businessdayfrequencyforservice


> **📇 Quick Reference Card**
> 
> **Sections:** 📋 Tasks


#### 📋 Tasks

Banks can schedule the jobs to be executed as service. This section guides you to run jobs in a frequency at certain time on business days.


##### Executing Business Day

The following information guides you in executing business day, which enhances the processing architecture of service framework.

Procedure

In TSA.SERVICE, set Frequency for business day as shown in the following screen capture.

As per the frequency set in TSA.SERVICE, the service starts and the frequency is cycled to the next business day.

---


### 1.20  Cache Resetting


> **📇 Quick Reference Card**
> 
> **Purpose:** *You can configure the system to reset the cache in TAFJ runtime without restarting the application server. This allows the cache to be cleared down while the system is running, without losing any Temenos Transact common variables required to keep processing.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks


#### 📖 Introduction

You can configure the system to reset the cache in TAFJ runtime without restarting the application server. This allows the cache to be cleared down while the system is running, without losing any Temenos Transact common variables required to keep processing.

This also helps to keep the system running during installation of Temenos Transact updates. That is, there is no downtime required to refresh existing active sessions with newly released data items.

Cache reset can be enabled by entering a time in field Cache Reset Period of the SPF application.

This guide is intended for customers and Temenos staff.


#### ⚙️ Configuration

You must set the Cache Reset Period to configure the Cache Reset Mechanism.


##### Setting the Cache Reset Period

In the SPF application enter a time value in field Cache Reset Period .

You can enter a 24 hour UTC time in format HH:MM. For other options, see Other Cache Reset options .

The cache will be reset daily when this time is reached or exceeded. If there is no value in this field, there is no daily cache reset. Note the following:

- If the defined time is greater than or equal to the current UTC time, cache reset is allowed from today.
- If the defined time is less than the current UTC time, cache reset is allowed from tomorrow onwards.
- The Enrichment displays the time remaining until the next cache reset.

> **⚠️ Note:** When this field is changed, an override will be created to indicate to admin that cache reset has been set up.


##### When the cache can be reset

The time specified in Cache Reset Period is compared with the current UTC time and the cache will be reset according to that centralised time. This allows cache reset to work on a multi-application server model.


##### Temenos Transactonline request

At the start of each request, the Cache Reset Period is checked against the current UTC time. If the system time equals or exceeds the Cash Reset Period, a cache reset is performed for that session without interrupting production. Cache reset will only happen once per day, as and when the Cache Reset Period reaches or exceeds the current UTC time. Additional resets will only be performed if the Cache Reset Period has been changed.


##### TSA agents

Each time an agent makes a call to SERVICE.HEARTBEAT , the Cache Reset Period is checked against the current UTC time. If the system time equals or exceeds the Cash Reset Period, the agent will be stopped. The agent is relaunched subsequently by its active TSM agent. The cache reset is done only once per agent. The agent is not stopped when subsequent calls are made to the SERVICE.HEARTBEAT unless the Cache Reset Period has been changed in SPF. Any agent that was initiated after the Cache Reset Period will not be stopped for cache reset.


##### TSM

During each interaction of TSM, after sleeping for the specified review time, the Cache Reset Period is checked against the current UTC time. If it equals or exceeds the Cash Reset Period, a cache reset is performed. Then it continues its normal operations and also relaunches all required agents which were stopped for the cache reset. Additional resets will only be performed if the Cache Reset Period has been changed in SPF and its value is still less than the current UTC time. If the TSM was started after the Cache Reset Period, cache reset will not be performed.


#### 📋 Tasks

The Temenos Transact system can be configured to reset the cache when operating in TAFJ runtime.

Overview

You can configure the system to reset the cache in TAFJ runtime without restarting the application server. This allows the cache to be cleared down while the system is running, without losing any Temenos Transact common variables required to keep processing.

Configuring the Cache Reset Mechanism

You must set the Cache Reset Period to configure the Cache Reset Mechanism.

Using the Cache Reset Mechanism

You will need to understand how cache resetting works with Temenos Transact .

---


### 1.21  Cloud Operation Efficiency


> **📇 Quick Reference Card**
> 
> **Sections:** 📋 Tasks


#### 📋 Tasks

Temenos Transact provides utilities to perform the cloud operations more efficiently. This section describes how to improve the cloud operations effectively.

Removing References of Installed Updates

This feature facilitates to remove the reference of any Update from the SPF application and reinstall the Update without performing any manual operation at the backend. This section describes how the reference on the installed Updates can be removed using the front end application.

---


### 1.22  COB


> **📇 Quick Reference Card**
> 
> **Sections:** ⚙️ Configuration | 📋 Tasks


#### ⚙️ Configuration

This feature detects lock collision in a batch and diverts the allocated agents to the parallel batches that are running in the same stage during COB. This reduces lock collisions during a job processing.


##### Threshold Setup

A field Lock Retry Threshold is configured in TSA.PARAMETER . This is an editable field and can accept any valid numeric value greater than zero. It specifies the maximum number of times the batch can be retried and assigned to the agents, before it is skipped to the next batch in the same stage.


##### Example

The following example shows that the system can keep track of number of times a lock contention is encountered with the help of a field ( Lock Retry Count ) in the BATCH application. This is possible only if you configure the threshold in TSA.PARAMETER .

The latest value from Lock Retry Count in BATCH is compared to the threshold value setup in TSA.PARAMETER , before allocating agents to a batch. If the threshold is breached for a batch and if there are other incomplete batches in the same batch stage, then those batches are processed before allocating an agent to the batch encountering the locking contentions.

> **⚠️ Note:** We do not proceed to the next batch stage before all the batches in the current stage are completed and this feature does not override the current batch stage.


#### 📋 Tasks

This feature allows posting a message into an activation file or in a queue when a transaction is done through version.

When a transaction is processed through a version, the Link Activation field is enabled at version level or in VERSION.CONTROL . The activation file or queue is then updated based on the configuration maintained in the EB.VERSION.ACTIVATION.LINK application. This allows you to achieve communication through activation table and helps avoid writing the local code.

The EB.VERSION.ACTIVATION.LINK application contains the service name and job to be used for updating activation table. This application also allows you to configure ID and message to update activation file. If you do not configure ID, then a unique ID will be generated and updated in the activation file.


##### Enable Link Activation

Enabling link activation for a version or VERSION.CONTROL allows you to update the activation file. You cannot disable the link activation after enabling it and configuring the EB.VERSION.ACTIVATION.LINK application. However, you can disable the link activation by reversing the EB.VERSION.ACTIVATION.LINK record.


##### Setting up Services

You need to create an EB.VERSION.ACTIVATION.LINK record to specify the service and job required to update the activation file.

To setup Services, Specify Queue Service and Queue Name . These are mandatory fields. Set Emit Reversal to Yes in the EB.VERSION.ACTIVATION.LINK table. This is done to update the activation file for reversal transactions. Optional: You can set multiple queue services to update multiple activation files at the same time. Authorise the record.


##### Updating the Activation File

This section shows you how to update the activation file using version and EB.VERSION.ACTIVATION.LINK .

To update the activation file, Enable the Link Activation field in the VERSION.CONTROL record. Configure the EB.VERSION.ACTIVATION.LINK record as shown below. Message to the activation file is picked from the Queue Message field. Set Activation File to Yes in PGM.FILE . Perform a transaction using the version. The activation file is updated as below.


##### Updating a Priority File

To update a Priority File, Enable the Link Activation field in the VERSION.CONTROL record. Set Queue Priority to Yes in EB.VERSION.ACTIVATION.LINK . Set Priority File to Yes and specify the Priority Table Name field in PGM.FILE . The Activation file is updated as below.


##### Updating a Queue

Open TSA.PARAMETER and set Queue Jobs to ALL or the required job name.

The queue gets updated with the following details when a transaction is done through a version for which Link Activation is enabled and EB.VERSION.ACTIVATION.LINK is sent.

---


### 1.23  Exit-API


> **📇 Quick Reference Card**
> 
> **Sections:** ⚙️ Configuration


#### ⚙️ Configuration

This section explains the Exit API configuration introduced in PGM.FILE and allows you to perform certain activities (such as sending alert, updating a local table, etc.) after all the contracts of a job are completed.


##### PGM.FILEsetup

The Exit Api field is configured in PGM.FILE for processing an exit activity after job completion.

> **⚠️ Note:** Exit Api is allowed only if the current job is a multi-threaded batch job. If you enter a routine name in Exit Api , then it should have a valid entry in EB.API .


##### Triggering the Exit API

Procedure

1. Write the exit API and attach it to the job in PGM.FILE.
2. Start TSM and run the service. The exit API is triggered by the job after the contracts are processed and the information is recorded in COMO. The test file given in exit API is updated as shown below.

---


### 1.24  Queues


> **📇 Quick Reference Card**
> 
> **Purpose:** *This section explains how queues can improve the processing time for large select jobs.*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

This section explains how queues can improve the processing time for large select jobs.

When a service is run, agents allocated to it need not wait for the selected agent to complete the service. Instead, processing of request happens in parallel when initial set of IDs are available in a queue. The IDs are flushed to the queue once 10 records are available or based on the commit size. The commit size is calculated based on the TSA.PARAMETER or PGM.FILE configuration. This reduces the processing time taken for jobs with larger select.

Dynamic bulking is done internally for queue jobs and is excluded when:

- Total writes exceeds 500.
- Count of lock time out exceeds the value configured in the F.LOCKING record ( TIMEOUT.COUNT ).
- Last commit time exceeds review time interval.
- There are activation or online services.
- There are jobs with fixed bulk number.


##### Prerequisites

Before you begin, you should have the following components available in your system:

- TAFJ
- All application servers
- Active MQ broker attached to database


##### Setting up Application Server

Procedure

1. Deploy the following WAR files in the deployments folder. TAFJEE.war , TAFJJEE_Micro and TAFJConfiguration.war are available in TAFJ\appserver\micro . You can use this location to copy and deploy in standalone.
2. Add the following system properties in T24.xml .
3. Add the connection definition and transaction support properties for active MQ setup as shown below:


##### Setting up AMQ

Procedure

1. Set the java path in \apache-activemq-5.15.10\bin\win64\wrapper.conf . # Java Application wrapper.java.command=C:\WorkArea\DEV\Temenos\java\jdk
2. Run InstallService.bat from bin. This starts the service.
3. Add the following properties in the activemq.xml file ( AMQ_HOME/conf ) and restart the broker service.
4. services.msc and open the ActiveMQ service properties.
5. Verify that Startup type is set to Automatic .
6. Start the service.
7. Use the http://localhost:8161/admin/ URL to verify if ActiveMQ is running. Log in using account admin and password admin .


##### Configuring TAFJ Properties

Add the following properties in the TAFJ properties file:

temn.tafj.runtime.use.jmsqueues.for.services=true

temn.tafj.runtime.services.queue.pull.timeout=100


##### Setting up Transact

Procedure

- Specify ALL in the QUEUE.JOBS field to enable queue processing for all jobs.
- Specify batch name to enable queue processing for all jobs in the batch. For example, BNK/SYSTEM.END.OF.DAY3 .
- Specify batch job to enable queue processing for a particular job in the batch. For example, BNK/SYSTEM.END.OF.DAY3-IC.COB . The Active MQ screen shows the list of queues allocated and the number of messages yet to be consumed. It also shows the total number of messages enqueued and dequeued so far. As per the above Transact setup, the jobs in batch record BNK/PR.EOD.PROCESS have used TAFJ_QUEUE_0 for processing. Below como shows the queue in progress and the select agent populating the records. Below como shows that the other agents have started the processing before the completion of the select agent.

---


### 1.25  Company Local Content


> **📇 Quick Reference Card**
> 
> **Sections:** ⚙️ Configuration | 📋 Tasks


#### ⚙️ Configuration

Company Local Content is used when company-specific data needs to be captured for the same field for the same customer.

Temenos Transact provides this functionality such that, any bank can specify the required fields and positions in COMPANY and LOCAL.CONTENT.TABLE and Temenos Transact run time will understand the setup and use the right value for the field based on the current company in which the request is made.

For example, the correct value for field TAX.ID may be different when the record is viewed in company Denmark than when the record is viewed in company Spain.


#### 📋 Tasks

This facility allows you to move data from local content into real fields and vice-versa in the Customer application.

Overview

Company Local Content is used when company-specific data needs to be captured for the same field for the same customer.

Configuring Company Local Content

You must perform a number of steps to configure Local Content.

Using Company Local Content

Using Company Local Content is best illustrated by example.

Running reports and enquiries

When you run reports and enquiries the values obtained for local content fields will depend on the selected company. This is best illustrated by example.

---


### 1.26  Constraints


> **📇 Quick Reference Card**
> 
> **Sections:** ⚙️ Configuration


#### ⚙️ Configuration

This section allows you to define how the system gets the information, for each position type.

Modelling Analysis Portfolio positions on different views are based on basic data. This basic data (also named attribute) is defined in AM.ENTITY . Depending on the type of the Position (Security, Account, and so on), the basic information must be extracted from a different file using different fields.

The currency for an account is the

field in the

file; but the currency for a Security is the

field in the

application. Thus, the

application allows the user to define how the system gets the information, for each type of Position.

---


### 1.27  Data Events


> **📇 Quick Reference Card**
> 
> **Purpose:** *Temenos Transact can emit the Data Event Streaming (DES) as Data Events. This works in conjunction with the TAFJ runtime over the Outbox Libraries. The eligibility to emit Data Events are based on the applications defined in the RR.PARAM table. Read Event driven Architecture for more information on ...*
> 
> **Applications:** `ACCOUNT`, `EB.DES.PARAMETER`, `FUNDS.TRANSFER`, `FUNDS.TRANSFER$NAU`, `RR.INITIAL.LOAD.PARAMETER`, `RR.PARAM`, `SPF`, `STMT.ENTRY` ... +1 more
> 
> **Key Fields:** *Attribute Type*, *Data Stream*, *Ilp required*, *Record Status*, *Service Status*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 🔧 Working With | 📋 Tasks


#### 📖 Introduction

Temenos Transact can emit the Data Event Streaming (DES) as Data Events. This works in conjunction with the TAFJ runtime over the Outbox Libraries. The eligibility to emit Data Events are based on the applications defined in the RR.PARAM table. Read Event driven Architecture for more information on the Data Events. This feature is enabled for the following channels:

- Interface (OFS)
- Legacy Browser
- UXP Browser
- Batch or Services
- API request in Temenos Transact

> **⚠️ Note:** This feature is not applicable for the following: Classic mode and dynamic applications in Data Events. Classic mode in AVRO formatted Data Events.

Configuring Data Events

This section provides the details about configuring Temenos Transact to emit Data Events.

Working with Data Events

This section defines the contexts that are used to create the Data Events.

State Change Event

This section provides the details about the Data Events emitted for State Change in Temenos Transact.

Data Events in RAW Table Format

This section explains the required configuration to emit Data Events in the AVRO format.

Handling Event Delivery Failures

This section explains handling event delivery failures using catchup service.

Custom Eligibility Check

This section explains custom eligibility check for data events.


#### ⚙️ Configuration

This section provides the details about configuring Temenos Transact to emit Data Events.

To configure Data Events in Temenos Transact,

1. Enable SPF .
2. Enable EB.DES.PARAMETER . Enter EB.DES.PARAMETER, I SYSTEM in the command line. Set Data Stream as Outbox. Set Data Stream as Avro to emit Data Events in RAW table format.
3. in the command line. Commit the record.

> **⚠️ Note:** The application is eligible to emit Data Events only when it is defined in RR.PARAM .

Temenos Transact is configured successfully to emit Data Events.


#### 🔧 Working With

_DATA_EVENT. The following are the contexts used to create the event.

| Sub-Tag | Description |
|---|---|
| tableKey | . |
| tableName | Holds the file name (combination of application name and file mnemonics (for example, FBNK, FCO3, and so on)) for which the Data Events are emitted. The tableKey is the identifier of the corresponding table. The dot and dollar characters are replaced with underscore and hash characters respectively in the file name. |
| applicationData | Holds all the fields of the record in Temenos Transact. |

| Sub-Tag | Description |
|---|---|
| originatingApplication | Indicates the application name used for the transaction. Following are the application names used in the transaction types: Multi-Transaction - Parent application API requests - operationName non-API requests - the application (version) |
| bankingDate | Indicates the current business date in the Temenos Transact |
| transactionType | Indicates the posting type (ONLINE or BATCH mode) of the transaction |
| action | Indicates the actual operation (function) that is invoked for the transaction. Following are the actions in Temenos Transact: INPUT REVERSE APPROVED |
| channelType | Indicates the respective channel name (OFS$SOURCE.ID) that is common for both API and Non-API requests. |
| application | Indicates the actual file name (combination of application name and file mnemonics). The dot and dollar characters are replaced with underscore and hash characters respectively in the file name |
| operation | Indicates the actual operation (WRITE/DELETE) performed on the table |
| requestStatus | Indicates the status of the record in Temenos Transact based on the Record Status field. The following are the values of the field: Unauthorised Reversed Authorised |

| Sub-Tag | Description |
|---|---|
| key | Indicates the name of the local field which is a valid field in the local table application. |
| values | Indicates the value of the local field that is associated with the key. |


##### Use Case for Data Events

The FUNDS.TRANSFER$NAU , FUNDS.TRANSFER , ACCOUNT , and STMT.ENTRY applications are defined in RR.PARAM to emit Data Events in the INAU state before the transaction.

To emit the Data Events in Temenos Transact,

1. Enter FT, I F3 in the command line to create the Funds Transfer (FT) transaction.
2. Commit the transaction without authorizing (record status=INAU).
3. The Data Events are generated for FUNDS.TRANSFER$NAU by the system. The Data Events are also generated for ACCOUNT and STMT.ENTRY (defined in RR.PARAM ) as they are updated by FT. { "specversion": "1.0", "id": "bd49dbeb-75a5-4b30-b018-f6711565ce14", "source": "https://temenos.com/microservice/cloudevents/TransactTest", "type": "FUNDS.TRANSFER_DATA_EVENT", "datacontenttype": "application/json", "subject": "event", "time": "2022-12-13T00:13:09.312Z", "organizationid": "GB0010001", "sequenceno": -999, "businesskey": "TransactTest|GB0010001|FT22110TXFM1", "correlationid": "bd49dbeb-75a5-4b30-b018-f6711565ce14", "data": { "applicationContext": { "tableKey": "TransactTest|GB0010001|FT22110TXFM1", "applicationData": { "totRecChgCrccy": "0", "debitValueDate": "20220420", "debitCurrency": "USD", "positionType": "TR", "debitCustomer": "100335", "totRecComm": "0", "ibanCredit": "GB98DEMO60161300103837", "processingDate": "20220420", "chargedCustomer": "120198", "creditValueDate": "20220420", "totRecChg": "0", "fedFunds": "NO", "creditCompCode": "GB0010001", "locAmtCredited": "4500.00", "totRecCommLcl": "0", "currencyMktCr": "1", "creditCustomer": "120198", "chargeComDisplay": "NO", "drAdviceReqdYN": "NO", "totRecChgLcl": "0", "profitCentreCust": "100335", "debitCompCode": "GB0010001", "crAdviceReqdYN": "NO", "amountDebited": "USD4500.00", "commissionCode": "DEBIT PLUS CHARGES", "returnToDept": "NO", "rateFixing": "NO", "amountCredited": "USD4500.00", "locAmtDebited": "4500.00", "totSndChgCrccy": "0.00", "ibanDebit": "GB57DEMO60161300103799", "currencyMktDr": "1", "debitAmount": "4500.00", "transactionType": "AC", "creditAcctNo": "103837", "creditCurrency": "USD", "debitAcctNo": "103799", "regCompliance": "PSD.NON", "custGroupLevel": "99", "stmtNos": [ "VAL" ], "chargeCode": "DEBIT PLUS CHARGES" }, "tableName": "FBNK_FUNDS_TRANSFER" }, "extensionData": [ { "values": "PARRYS", "key": "TOWN.COUNTRY" }, { "values": "CHENNAI", "key": "CITY" }, { "values": "INDIA", "key": "COUNTRY" } ], "eventContext": [ { "originatingApplication": "FUNDS.TRANSFER,TEST", "bankingDate": "20220420", "transactionType": "ONLINE", "application": "FBNK_FUNDS_TRANSFER", "operation": "WRITE", "action": "INPUT", "channelType": "IRISPA", "requestStatus": "Unauthorised" } ] } } Given below is the Data Events generated for the ACCOUNT application (Debit Account). { "specversion": "1.0", "id": "99b339ed-4d0c-4269-8129-47efeb6dda1c", "source": "https://temenos.com/microservice/cloudevents/TransactTest", "type": "ACCOUNT_DATA_EVENT", "datacontenttype": "application/json", "subject": "event", "time": "2022-12-13T00:24:16.241Z", "organizationid": "GB0010001", "sequenceno": -999, "businesskey": "TransactTest|GB0010001|FT22110TXFM1", "correlationid": "99b339ed-4d0c-4269-8129-47efeb6dda1c", "data": { "applicationContext": { "tableKey": "TransactTest|GB0010001|103799", "applicationData": { "positionType": "TR", "onlineActualBal": "-4500", "conditionGroup": "1", "shortTitle": [ "LINDSAYUS" ], "capDateCrInt": [ "20220331" ], "tranLastDrCust": "213", "interestCcy": "USD", "dateLastUpdate": "20220420", "chargeMkt": "1", "interestMkt": "1", "chargeCcy": "USD", "workingBalance": "-4500", "mnemonic": "LINDSAYUS", "currency": "USD", "capDateDrInt": [ "20220331" ], "openingDate": "20220321", "onlineClearedBal": "-4500", "openClearedBal": "0", "dateLastDrCust": "20220420", "amntLastDrCust": "-4500.00", "capDateCharge": [ "20220331" ], "AltAcctType": [ { "altAcctType": "LEGACY" }, { "altAcctType": "T24.IBAN", "altAcctId": "GB57DEMO60161300103799" }, { "altAcctType": "PREV.IBAN" }, { "altAcctType": "HOLDER.REF" }, { "altAcctType": "CONN.REF" }, { "altAcctType": "CBU" }, { "altAcctType": "RIB" }, { "altAcctType": "ISIN" }, { "altAcctType": "CUSIP" } ], "capDateC2Int": [ "20220331" ], "accountOfficer": "2", "allowNetting": "NO", "accountTitle1": [ "LINDSAY USD" ], "passbook": "NO", "openCategory": "1001", "category": "1001", "openActualBal": "0", "currencyMarket": "1", "customer": "100335", "capDateD2Int": [ "20220331" ] }, "tableName": "FBNK_ACCOUNT" }, "eventContext": [ { "originatingApplication": "FUNDS.TRANSFER,TEST", "bankingDate": "20220420", "transactionType": "ONLINE", "application": "FBNK_ACCOUNT", "operation": "WRITE", "channelType": "IRISPA", "requestStatus": "APPROVED" } ] } }
4. Authorise the FT transaction. The Data Events are generated successfully with requestStatus as Approved for the following applications. FUNDS.TRANSFER { "specversion": "1.0", "id": "82f2ad2a-4299-43dc-a897-3d6fd677ce28", "source": "https://temenos.com/microservice/cloudevents/TransactTest", "type": "FUNDS.TRANSFER_DATA_EVENT", "datacontenttype": "application/json", "subject": "event", "time": "2022-12-13T00:24:16.634Z", "organizationid": "GB0010001", "sequenceno": -999, "businesskey": "TransactTest|GB0010001|FT22110TXFM1", "correlationid": "82f2ad2a-4299-43dc-a897-3d6fd677ce28", "data": { "applicationContext": { "tableKey": "TransactTest|GB0010001|FT22110TXFM1", "applicationData": { "totRecChgCrccy": "0", "debitValueDate": "20220420", "debitCurrency": "USD", "positionType": "TR", "debitCustomer": "100335", "totRecComm": "0", "ibanCredit": "GB98DEMO60161300103837", "processingDate": "20220420", "chargedCustomer": "120198", "creditValueDate": "20220420", "totRecChg": "0", "fedFunds": "NO", "creditCompCode": "GB0010001", "locAmtCredited": "4500.00", "totRecCommLcl": "0", "currencyMktCr": "1", "creditCustomer": "120198", "drAdviceReqdYN": "NO", "totRecChgLcl": "0", "profitCentreCust": "100335", "debitCompCode": "GB0010001", "crAdviceReqdYN": "NO", "amountDebited": "USD4500.00", "commissionCode": "DEBIT PLUS CHARGES", "returnToDept": "NO", "rateFixing": "NO", "amountCredited": "USD4500.00", "authDate": "20220420", "locAmtDebited": "4500.00", "totSndChgCrccy": "0.00", "ibanDebit": "GB57DEMO60161300103799", "currencyMktDr": "1", "debitAmount": "4500.00", "transactionType": "AC", "creditAcctNo": "103837", "creditCurrency": "USD", "debitAcctNo": "103799", "regCompliance": "PSD.NON", "custGroupLevel": "99", "stmtNos": [ "200713662221252.00", "1-2" ], "chargeCode": "DEBIT PLUS CHARGES" }, "tableName": "FBNK_FUNDS_TRANSFER" }, "extensionData": [ { "values": "PARRYS", "key": "TOWN.COUNTRY" }, { "values": "CHENNAI", "key": "CITY" }, { "values": "INDIA", "key": "COUNTRY" } ], "eventContext": [ { "originatingApplication": "FUNDS.TRANSFER,TEST", "bankingDate": "20220420", "transactionType": "ONLINE", "application": "FBNK_FUNDS_TRANSFER", "operation": "WRITE", "channelType": "IRISPA", "requestStatus": "APPROVED" } ] } } ACCOUNT – Debit Movement { "specversion": "1.0", "id": "99b339ed-4d0c-4269-8129-47efeb6dda1c", "source": "https://temenos.com/microservice/cloudevents/TransactTest", "type": "ACCOUNT_DATA_EVENT", "datacontenttype": "application/json", "subject": "event", "time": "2022-12-13T00:24:16.241Z", "organizationid": "GB0010001", "sequenceno": -999, "businesskey": "TransactTest|GB0010001|FT22110TXFM1", "correlationid": "99b339ed-4d0c-4269-8129-47efeb6dda1c", "data": { "applicationContext": { "tableKey": "TransactTest|GB0010001|103799", "applicationData": { "positionType": "TR", "onlineActualBal": "-4500", "conditionGroup": "1", "shortTitle": [ "LINDSAYUS" ], "capDateCrInt": [ "20220331" ], "tranLastDrCust": "213", "interestCcy": "USD", "dateLastUpdate": "20220420", "chargeMkt": "1", "interestMkt": "1", "chargeCcy": "USD", "workingBalance": "-4500", "mnemonic": "LINDSAYUS", "currency": "USD", "capDateDrInt": [ "20220331" ], "openingDate": "20220321", "onlineClearedBal": "-4500", "openClearedBal": "0", "dateLastDrCust": "20220420", "amntLastDrCust": "-4500.00", "capDateCharge": [ "20220331" ], "AltAcctType": [ { "altAcctType": "LEGACY" }, { "altAcctType": "T24.IBAN", "altAcctId": "GB57DEMO60161300103799" }, { "altAcctType": "PREV.IBAN" }, { "altAcctType": "HOLDER.REF" }, { "altAcctType": "CONN.REF" }, { "altAcctType": "CBU" }, { "altAcctType": "RIB" }, { "altAcctType": "ISIN" }, { "altAcctType": "CUSIP" } ], "capDateC2Int": [ "20220331" ], "accountOfficer": "2", "allowNetting": "NO", "accountTitle1": [ "LINDSAY USD" ], "passbook": "NO", "openCategory": "1001", "category": "1001", "openActualBal": "0", "currencyMarket": "1", "customer": "100335", "capDateD2Int": [ "20220331" ] }, "tableName": "FBNK_ACCOUNT" }, "eventContext": [ { "originatingApplication": "FUNDS.TRANSFER,TEST", "bankingDate": "20220420", "transactionType": "ONLINE", "application": "FBNK_ACCOUNT", "operation": "WRITE", "channelType": "IRISPA", "requestStatus": "APPROVED" } ] } } ACCOUNT – Credit Movement { "specversion": "1.0", "id": "13063fdb-5e94-42a0-8f2a-e31e40f13bcb", "source": "https://temenos.com/microservice/cloudevents/TransactTest", "type": "ACCOUNT_DATA_EVENT", "datacontenttype": "application/json", "subject": "event", "time": "2022-12-13T00:24:16.339Z", "organizationid": "GB0010001", "sequenceno": -999, "businesskey": "TransactTest|GB0010001|FT22110TXFM1", "correlationid": "13063fdb-5e94-42a0-8f2a-e31e40f13bcb", "data": { "applicationContext": { "tableKey": "TransactTest|GB0010001|103837", "applicationData": { "positionType": "TR", "onlineActualBal": "4500", "conditionGroup": "2", "shortTitle": [ "WILLNORUSD" ], "capDateCrInt": [ "20220331" ], "amntLastCrCust": "4500.00", "interestCcy": "USD", "dateLastUpdate": "20220420", "chargeMkt": "1", "interestMkt": "1", "dateLastCrCust": "20220420", "chargeCcy": "USD", "workingBalance": "4500", "mnemonic": "WILLNORUSD", "currency": "USD", "capDateDrInt": [ "20220331" ], "openingDate": "20220321", "onlineClearedBal": "4500", "openClearedBal": "0", "singleLimit": "Y", "capDateCharge": [ "20220331" ], "AltAcctType": [ { "altAcctType": "LEGACY" }, { "altAcctType": "T24.IBAN", "altAcctId": "GB98DEMO60161300103837" }, { "altAcctType": "PREV.IBAN" }, { "altAcctType": "HOLDER.REF" }, { "altAcctType": "CONN.REF" }, { "altAcctType": "CBU" }, { "altAcctType": "RIB" }, { "altAcctType": "ISIN" }, { "altAcctType": "CUSIP" } ], "capDateC2Int": [ "20220331" ], "accountOfficer": "5", "allowNetting": "NO", "accountTitle1": [ "WILLNORUSD" ], "passbook": "NO", "openCategory": "1001", "category": "1001", "openActualBal": "0", "currencyMarket": "1", "tranLastCrCust": "258", "customer": "120198", "capDateD2Int": [ "20220331" ] }, "tableName": "FBNK_ACCOUNT" }, "eventContext": [ { "originatingApplication": "FUNDS.TRANSFER,TEST", "bankingDate": "20220420", "transactionType": "ONLINE", "application ": "FBNK_ACCOUNT", "operation": "WRITE", "channelType": "IRISPA", "requestStatus": "APPROVED" } ] } } STMT.ENTRY – Credit Movement { "specversion": "1.0", "id": "85e2d323-d8c2-4f2a-8a6e-380c38476ec4", "source": "https://temenos.com/microservice/cloudevents/TransactTest", "type": "STMT.ENTRY_DATA_EVENT", "datacontenttype": "application/json", "subject": "event", "time": "2022-12-13T00:24:16.428Z", "organizationid": "GB0010001", "sequenceno": -999, "businesskey": "TransactTest|GB0010001|FT22110TXFM1", "correlationid": "85e2d323-d8c2-4f2a-8a6e-380c38476ec4", "data": { "applicationContext": { "tableKey": "TransactTest|GB0010001|200713662221252.000002", "applicationData": { "companyCode": "GB0010001", "systemId": "FT", "consolKey": "AC.1.TR.USD.1001.2001.NO.....2710.....GB0010001", "positionType": "TR", "exposureDate": "20220420", "amountLcy": "4500.00", "departmentCode": "1", "crfType": "CREDIT", "tdglDetails": [ "TD", "", "", "", "", "", "", "VALUE.DATE" ], "processingDate": "20220420", "transactionCode": "258", "valueDate": "20220420", "netParam": "CLDEFAULT", "productCategory": "1001", "ourReference": "FT22110TXFM1", "accountOfficer": "21", "origCcyMarket": "1", "transReference": "FT22110TXFM1", "customerId": "120198", "currency": "USD", "bookingDate": "20220420", "stmtNo": [ "200713662221252.00", "1-2" ], "currencyMarket": "1", "systemDateTimeRec": [ "20221213002413075" ] }, "tableName": "FBNK_STMT_ENTRY" }, "eventContext": [ { "originatingApplication": "FUNDS.TRANSFER,TEST", "bankingDate": "20220420", "transactionType": "ONLINE", "application": "FBNK_STMT_ENTRY", "operation": "WRITE", "channelType": "IRISPA", "requestStatus": "APPROVED" } ] } } STMT.ENTRY – Debit Movement { "specversion": "1.0", "id": "f0cfc8b6-1f73-4f51-a1d6-487c212505f2", "source": "https://temenos.com/microservice/cloudevents/TransactTest", "type": "STMT.ENTRY_DATA_EVENT", "datacontenttype": "application/json", "subject": "event", "time": "2022-12-13T00:24:16.529Z", "organizationid": "GB0010001", "sequenceno": -999, "businesskey": "TransactTest|GB0010001|FT22110TXFM1", "correlationid": "f0cfc8b6-1f73-4f51-a1d6-487c212505f2", "data": { "applicationContext": { "tableKey": "TransactTest|GB0010001|200713662221252.000001", "applicationData": { "companyCode": "GB0010001", "systemId": "FT", "consolKey": "AC.1.TR.USD.1001.1001.AU.....1000.....GB0010001", "positionType": "TR", "exposureDate": "20220420", "amountLcy": "-4500.00", "departmentCode": "1", "crfType": "DEBIT", "tdglDetails": [ "TD", "", "", "", "", "", "", "VALUE.DATE" ], "processingDate": "20220420", "transactionCode": "213", "valueDate": "20220420", "netParam": "CLDEFAULT", "productCategory": "1001", "ourReference": "FT22110TXFM1", "accountOfficer": "21", "origCcyMarket": "1", "transReference": "FT22110TXFM1", "customerId": "100335", "currency": "USD", "bookingDate": "20220420", "stmtNo": [ "200713662221252.00", "1-2" ], "currencyMarket": "1", "systemDateTimeRec": [ "20221213002412272" ] }, "tableName": "FBNK_STMT_ENTRY" }, "eventContext": [ { "originatingApplication": "FUNDS.TRANSFER,TEST", "bankingDate": "20220420", "transactionType": "ONLINE", "application": "FBNK_STMT_ENTRY", "operation": "WRITE", "channelType": "IRISPA", "requestStatus": "APPROVED" } ] } }


##### ILP Services

Temenos Transact tables defined in RR.PARAM are used to perform the Initial Load Processing (ILP) to emit Data Events through the following services:

To perform ILP,

1. Go to RR.PARAM in Temenos Transact.
2. Set Ilp required as Yes.
3. Run the RR.TAKEON service. Read Configuring TSA.SERVICE for RR.TAKEON to run the service. Given below is the sample Data Event emitted after the execution of the service. { "specversion": "1.0", "id": "637f0e3f-25aa-489e-b95d-d3a2dcd50102", "source": "https://temenos.com/microservice/cloudevents/ModelBank", "type": "CURRENCY_DATA_ILP_EVENT", "datacontenttype": "application/json", "subject": "event", "time": "2023-05-12T10:59:56.464Z", "organizationid": "GB0010001", "sequenceno": -999, "businesskey": "ModelBank|GB0010001|BNK/RR.TAKEON_RR.TAKEON_USD", "correlationid": "637f0e3f-25aa-489e-b95d-d3a2dcd50102", "data": { "applicationContext": { "tableKey": "ModelBank|GB0010001|USD", "applicationData": { "baseCcyRank": "25", "ccyName": [ "US Dollar", "Dollar US" ], "preciousMetal": "NO", "noOfDecimals": "2", "cashRoundType": "1", "daysForward": "0", "quotationPips": "4", "minRoundType": "1", "interestDayBasis": "B 366/360", "countryCode": "US", "CurrencyMarket": [ { "currencyMarket": "1", "negotiableAmt": "1000000.00" }, { "currencyMarket": "10", "negotiableAmt": "100000.00" } ], "numericCcyCode": "840", "rank": "0", "clsCcy": "NO", "daysDelivery": "1" }, "tableName": "FBNK_CURRENCY" }, "eventContext": [ { "jobName": "RR.TAKEON", "transactionType": "BATCH", "processName": "BNK/RR.TAKEON", "application ": "FBNK_CURRENCY", "operation": "WRITE", "cobDate": "20230419" } ] } }
4. Set Ilp required to “” (Null) after the ILP is performed. This avoids the table getting processed again in the next iteration of the service.

To perform ILP,

1. Go to RR.INITIAL.LOAD.PARAMETER .
2. Define the table record ID with either SYSTEM or COMPANY. RR.INITIAL.LOAD.PARAMETER, I SYSTEM RR.INITIAL.LOAD.PARAMETER, I GB0010001
3. Set the Service Status to Active.
4. Run RR.INITIAL.LOAD.SERVICE service. Read Configuring TSA.SERVICE for RR.INITIAL.LOAD.SERVICE to run the service. Given below is the sample Data Event emitted after the execution of the service. { "specversion": "1.0", "id": "825cf88b-bd9f-4d3b-a650-f8d3b5d0b7d7", "source": "https://temenos.com/microservice/cloudevents/ModelBank", "type": "CURRENCY_DATA_ILP_EVENT", "datacontenttype": "application/json", "subject": "event", "time": "2023-05-12T10:44:03.762Z", "organizationid": "GB0010001", "sequenceno": -999, "businesskey": "ModelBank|GB0010001|BNK/RR.INITIAL.LOAD.SERVICE_RR.INITIAL.LOAD.SERVICE_USD", "correlationid": "825cf88b-bd9f-4d3b-a650-f8d3b5d0b7d7", "data": { "applicationContext": { "tableKey": "ModelBank|GB0010001|USD", "applicationData": { "baseCcyRank": "25", "ccyName": [ "US Dollar", "Dollar US" ], "preciousMetal": "NO", "noOfDecimals": "2", "cashRoundType": "1", "daysForward": "0", "quotationPips": "4", "minRoundType": "1", "interestDayBasis": "B 366/360", "countryCode": "US", "CurrencyMarket": [ { "currencyMarket": "1", "negotiableAmt": "1000000.00" }, { "currencyMarket": "10", "negotiableAmt": "100000.00" } ], "numericCcyCode": "840", "rank": "0", "clsCcy": "NO", "daysDelivery": "1" }, "tableName": "FBNK_CURRENCY" }, "eventContext": [ { "jobName": "RR.INITIAL.LOAD.SERVICE", "transactionType": "BATCH", "processName": "BNK/RR.INITIAL.LOAD.SERVICE", "application ": "FBNK_CURRENCY", "operation": "WRITE", "cobDate": "20230419" } ] } }
5. Set Service Status to Inactive after the ILP is performed. This avoids the table getting processed again in the next iteration of the service.


#### 📋 Tasks

This section explains handling event delivery failures using catchup service.

When there are event delivery failures during KAFKA downtime environment, the system inserts the event records into the error table and then triggers a catch-up service to retrieve records from the error table, deliver them, and subsequently delete them.

It is possible that the KAFKA topics are not reachable due to a variety of reasons, the temporary network outage being the most prominent one. In such cases, delivery of some events likely fail to deliver to the required topic/s. The system has now rectified this by identifying any such failure to deliver events, and by moving them to the F_MS_OUTBOX_ERROR table within the Temenos Transact database.

A service MS.EVENTS.CATCH.UP is released which selects the failed events from the F_MS_OUTBOX_ERROR table and attempts a redelivery of those to the required topics. For this, a TAFj function MS.DELIVER.ERROR.EVENTS is also made available, which can deliver the requested event to the expected topic.

> **⚠️ Note:** The Topic names, where the delivery is made is not negotiable and remains the same as the original topic where the delivery would have been made but for the failure to deliver. Once the delivery is successful, the event is deleted from the ERROR table, to avoid a redelivery later.

You can start the BNK/MS.EVENTS.CATCH.UP service to deliver the failed events to the required topic once KAFKA has been re-established. If you set BULK.ID.SIZE in Attribute Type of the TSA.SERVICE application, it allows to group the eventIds and deliver the events. The default value of this attribute is 5 and you can set it to any integer or numeric value.

Once the service has been run successfully, the system delivers the events to the ms-eventstore-inbox-topic and then moves them to the consumer topic ( ModelBank-event-topic ).

Here, SPF site name is defined as ModelBank.


> **Related Applications:** `ACCOUNT`, `EB.DES.PARAMETER`, `FUNDS.TRANSFER`, `FUNDS.TRANSFER$NAU`, `RR.INITIAL.LOAD.PARAMETER`, `RR.PARAM`, `SPF`, `STMT.ENTRY`, `TSA.SERVICE`

---


### 1.28  Grouping Events


> **📇 Quick Reference Card**
> 
> **Purpose:** *Events are defined in MS.EVENT for First Class Business Events (FCBE) and in RR.PARAM for Data Events. Temenos Transact organises events into groups, based on the custom topic names along with the site name topic in SPF . Similar or related events can be grouped into a single category, allowing user...*
> 
> **Applications:** `MS.EVENT`, `MS.EVENT.GROUP`, `MS.PARAMETER`, `RR.PARAM`, `SPF`
> 
> **Key Fields:** *Allowed Topic Names*, *Attribute Type*, *Attribute Value*, *AttributeValue*, *Event Group*, *Topic Names*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

Events are defined in MS.EVENT for First Class Business Events (FCBE) and in RR.PARAM for Data Events. Temenos Transact organises events into groups, based on the custom topic names along with the site name topic in SPF . Similar or related events can be grouped into a single category, allowing users to subscribe only to the topics they need. This approach ensures users receive only the events relevant to them, significantly reducing their ingestion load. The MS.EVENT and RR.PARAM application defines a group name.


##### Workflow of FCBE and Data Events

The following is the workflow for a FCBE with custom topics.

1. Event Retrieval - Retrieve events from the MS.EVENT table.
2. Subscription Check and Status - Evaluate the SUBSCRIBED status in the MS.EVENT record. The following are the possible values: NO - Event is ineligible for delivery and is ignored. YES - Event is eligible for delivery, and group membership is checked.
3. Group Definition - Verify if the group name is defined for the event. No Group Defined - If no group is defined, the event is delivered to the topic specified by site name in SPF , contingent on the Subscribed status. Group Defined - If a group is defined, the Subscribed status within the group definition is checked. The following are the possible values: NO - Event is ineligible for delivery and is ignored. YES - Event is eligible for delivery, and group topic names are checked.
4. Topic Name Check - Check if any topic names are defined for the event's group. No Topic Names Defined - If no topic names are defined, the event is delivered to the topic specified by site name in SPF , contingent on the Subscribed status. Topic Names Defined - If one or more topic names are defined, the following actions are performed for each topic name: A new event is created with a unique key. The current topic name is set as the eventSourceId of the new event. The new event is emitted.

Define the following fields in RR.PARAM for Data Events.

- Attribute Type with EVENT.GROUP.NAME.
- Attribute Value with value for EVENT.GROUP.NAME. Ensure the value is a valid ID in the MS.EVENT.GROUP record.

> **⚠️ Note:** Data Events do not perform any additional subscription checks. The workflow for resolving topic names and delivering Data Events remains consistent with FCBE.


##### Configuring Applications

The following applications are configured for event grouping.

Define the topic name in the Allowed Topic Names field.

- Maximum of four topics can be defined, including SPF site name.
- Only the topics defined in MS.PARAMETER can be used in MS.EVENT.GROUP .

Define the topic in the Topic Names field that allows multiple topics already set in MS.PARAMETER .


##### Linking and Working of Event Group for FCBE

1. Link MS.EVENT.GROUP and MS.EVENT using the Event Group field.
2. Create or amend a country record that emits a FCBE event.


##### Linking and Working of Event Group for Data Events

1. Link MS.EVENT.GROUP and RR.PARAM using the fields Attribute Type and AttributeValue .
2. Create or amend a sector record that emits a Data Event.


> **Related Applications:** `MS.EVENT`, `MS.EVENT.GROUP`, `MS.PARAMETER`, `RR.PARAM`, `SPF`

---


### 1.29  LocalReference AlternateKeys


> **📇 Quick Reference Card**
> 
> **Sections:** ⚙️ Configuration


#### ⚙️ Configuration

This section allows you to configure the LOCAL.REF.TABLE application.

This application defines the names of Input applications to which the local fields defined are to be linked and the order in which they are to appear on the screen. It also controls the association between any local reference fields that the user has defined as a set of fields.

> **⚠️ Note:** Once the local fields are linked to the application, that is, LOCAL.REF.TABLE entry is Input and Authorised, it is not possible to delete or re-arrange the local fields. Only the descriptions or conditions defined on LOCAL.TABLE may be changed.

Once the LOCAL.REF.TABLE entry is authorized, the Temenos Transact system automatically updates the STANDARD.SELECTION with the new customised fields and hence build the corresponding dictionary items. Then it is also possible to use these fields in reports and enquiries, as well as adding HELPTEXT for the field to let the users know what the field is used for.

In few scenarios, the fields added using LOCAL.TABLE and LOCAL.REF.TABLE could consist of several single value fields, unrelated to each other and some multi-value fields (not related to any other fields) and to make it more complex, two sets of multi-valued fields, which are associated but not with each other as shown in the below example.

The '!' option from LOCAL.TABLE fields allows you to view the VETTING application or the LOCAL.REF record. The '_' option provides the valid options defined in the VETTING.TABLE application.

---


### 1.30  Multi-time zone


> **📇 Quick Reference Card**
> 
> **Sections:** ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### ⚙️ Configuration

This section shows the user level restrictions that are set to protect data against unauthorized access and to enforce stronger security for the application.


##### Permitted time of use

For each user account, valid log in days and hours are set so that you can log in at a specified day and time. When you login, the system checks your allowed login day and time, and validates with the local time zone. If it is valid, you can access the application. If it is invalid, log on to the network will be restricted.

In the below example, the user SEAT.AUTH is linked to the Asia or Singapore time zone.

Based on the following parameters of SEAT.AUTH, Temenos Transact will check if the user has logged in the application during the allowed login day and time:

- START.DATE.PROFILE
- END.DATE.PROFILE
- START.TIME
- END.TIME

If the validation is successfull, the user SEAT.AUTH logs in the application.

If the validation fails, the Temenos Transact system displays an error as shown below.


##### Allowed days

You can specify the number of days that the user can access the application in the ALLOWED.DAYS field. You can further specify the access time for a particular day in the DAY.ST.TIME and DAY.END.TIME fields. If you do not specify the DAY.ST.TIME and DAY.END.TIME fields, the system will use the START.TIME and END.TIME field values.

The ALLOWED.DAYS field is a multi-value field. The days of the week are numbered from '1-7', where Monday represents '1' and Sunday represents '7'.

For example, the ALLOWED.DAYS field is specified as 1 . The DAY.ST.TIME and DAY.END.TIME fields are specified as 17:00 and 24:00 respectively.

If the SEAT.AUTH user logs in on Monday, then the user can access the application from 5 pm to 12 am.

> **⚠️ Note:** When you check the duration of user's access, the ALLOWED.DAYS field is taken as precedence.


##### Sign on date and time

When the user successfully logs in the application, the system calculates the user's last sign on date and time with the country's local time zone. The final login date and time gets updated in the DATE.LAST.SIGN.ON and TIME.LAST.SIGN.ON fields.


##### Deactivating and reactivating user accounts

User profiles can be deactivated for a specific amount of time to cater periods of absence or holiday, and reactivated when the defined deactivation period expires.

The DEACTIVATION.DATE field holds the start date of deactivation period and the REACTIVATION.DATE field holds the end date of deactivation period.

When the deactivation and reactivation dates are updated successfully, the user profile defaults the deactivation and reactivation values.


#### 📋 Tasks

USER.SMS.GROUP enables additional functions to users for a temporary period of time.

To enable additional functions,

1. Open USER.SMS.GROUP with a relevant user record.
2. Specify the additional function in the TEMP.FUNCTION field. This makes the START.DATE and END.DATE fields as mandatory input fields.
3. Specify Start Date and End Date . These fields holds the local zone date and time. It specifies the duration of access to the additional function. In this case, Temenos Transact checks the Start Date and End Date field values to validate the login details with the local time zone. Below is the sample screen of the USG.ST.ED.D record. When the temporary function expires on 31 st JULY 2013, the system automatically removes the Temp Function , Start Date and End Date fields from the USER.SMS.GROUP record.


#### 📊 Outputs

This section deals with the audit reports that are involved in the multi-time zone feature.


##### OFS.REQUEST.DETAIL

OFS.REQUEST.DETAIL is a log file that maintains all the channel messages. It holds a record per message and maintains the details of the message in local time zone. It also maintains the server time details (time of the request and completion time).

The DATE.TIME.RECD and DATE.TIME.PROC fields show the transaction received and processed time in local time zone. The details are displayed in milliseconds.


##### Protocol

PROTOCOL is the main audit file for violations and breaches. It contains the local time information for audit purpose.

The LOCAL.DATE.TIME field updates the transactions that were committed in local time zone.


##### Enquiry

Coordinated Universal Time (UTC) is the primary time standard used across countries. Temenos Transact stores the UTC date and time in the database. Therefore, in the enquiry, you can view the local zone date and time automatically.

When you specify D in the TYPE field, it enables the USE.LOCAL.TIME field in SPF. This allows Temenos Transact to convert the given date and time to the specific local zone date and time in the enquiry record.

> **⚠️ Note:** If the USE.LOCAL.TIME field in SPF is disabled, then the local zone’s date and time is not displayed in the enquiry record.

---


### 1.31  Service Automation


> **📇 Quick Reference Card**
> 
> **Sections:** 📋 Tasks


#### 📋 Tasks

To configure Service Automation, you must set three fields in the TSA.SERVICE record.

Set the following fields as required:

| Column 1 | Column 2 |
|---|---|
| Max Start Time | The maximum start time. The service cannot be started after this time. |
| Min Start Time | The minimum start time. The service cannot be started before this time. |
| No Of Runs Per Day | The number of times the service can be started in one day. |

---


### 1.32  Standards Restrictions


> **📇 Quick Reference Card**
> 
> **Sections:** 📋 Tasks


#### 📋 Tasks

This section describes the restrictions in adding a new record and amending an existing record after installing Transact through SS2021.

After installing SS2021 in standard module, by default, following three applications given in the table can restrict the creation and amendment of records, as required.

| Application Name | New Record | Amendment of Record |
|---|---|---|
| EB.API | Not Allowed | Allowed |
| DFE.PARAMETER | Not Allowed | Not Allowed |
| EB.TABLE.DEFINITION | Allowed only when created through AA.CLASS.DEFINITION. Manual creation is not allowed. | Allowed only when created through AA.CLASS.DEFINITION. Manual amendment is not allowed. |

The following sections illustrate the system behavior for the above scenarios.


##### Adding or Creating Records

The below screen captures illustrate that the creation of a new record in EB.API , DFE.PARAMETER and EB.TABLE.DEFINITION is restricted.

However, these restrictions are not applicable for the EB.TABLE.DEFINITION applications that are created through AA.CLASS.DEFINITION , which are defined by the user. The screen captures below show the creation of AA.CLASS.DEFINITION .

The following screen capture shows the respective EB.TABLE.DEFINITION application with the ID of AA.CLASS.DEFINITION .


##### Modifying Records

The below screen captures show that the amendment is allowed in EB.API application. It is evident that the Protection Level field is changed from Partial to Full.

The following screen capture shows the amendment is restricted in DFE.PARAMETER .

The following screen captures show that the amendment is allowed in EB.TABLE.DEFINITION .

---


### 1.33  SupportingOtherDateFormat


> **📇 Quick Reference Card**
> 
> **Sections:** ⚙️ Configuration | 📋 Tasks


#### ⚙️ Configuration

Temenos Transact is based on Gregorian calendar, which is the standard business calendar used in the international banking markets. This section guides the banks to enter the date, based on its country specific calendar such as Hijri or Ethiopian for creating transaction.

Using Hijri or Ethiopian Calendar Format

This section guides you in using Hijri or Ethiopian calendar format.


#### 📋 Tasks

This section guides you in using Hijri or Ethiopian calendar format.

The prescribed format is to add H for Hijri and E for Ethiopian as prefix with the usual date format:

- HYYYYMMDD for Hijri
- EYYYYMMDD for Ethiopian

When you enter the Hijri or Ethiopian calendar format date, Temenos Transact automatically converts them to Gregorian format.

Consider a customer presents a cheque in Local Currency (LCY) for cash payment and the cheque date is written in Hijri calendar format, banks can enter the Hijri Date of Cheque in the Cheque Date field available in core. It is then converted into Gregorian Date and updated in the same field. The display is based on the date format option of the user.

The following screen capture shows the current logged in user date format is HYYYYMMDD and the options are 1 and 2 respectively. Option 1 date format is and option 2 date format is / / .

H14421007

The following shows an input FUNDS.TRANSFER transaction and validate screen capture.

On validating the record, the Hijri date (14421007) is converted to Gregorian date (19 MAY 2021) and is displayed in the same field.

The following shows an input PAYMENT.ORDER transaction and validate screen capture, which has Hijri date format.

The following screen capture shows that the Hijri date is converted to its equivalent Gregorian date and Hijri date is displayed as enrichment. The date display format is taken from the user level, which is / / .


##### Viewing Enquiry and Statements in Hijri Dates

For viewing enquiry and statements in Hijri date, you must use the common API provided by Temenos Transact . It converts the Gregorian date to Hijri date. Enquiries can use conversion routines. The following screen capture shows an enquiry with conversion routine attached with date field.

The following screen capture shows the enquiry output.

If required, conversion routine can be customised to display the output in required format and local language.

The following screen capture shows the enquiry output.

---


### 1.34  Traceability


> **📇 Quick Reference Card**
> 
> **Sections:** ⚙️ Configuration


#### ⚙️ Configuration

There are a number of reasons why a trace of actions may be required.

Financial institutions may have to provide information to regulatory auditors or customers when there is a deviation to normal procedures.

Banks may have to provide a trace when there property elements coming into a transaction request from multiple third parties.

The trace provided by the Traceability module is sent to a data repository called Micro services for further use. The information is transmitted asynchronously.

---


### 1.35  Transact Monitoring Using Grafana


> **📇 Quick Reference Card**
> 
> **Sections:** ⚙️ Configuration | 📋 Tasks


#### ⚙️ Configuration

This section guides you in configuring the triggering events from Temenos Transact to Grafana through TECEvent, which is a Platform Framework function.

In the SPF record, Ext is set for triggering the events to Grafana and list of events to trigger are taken from TEC.PROFILE . The Docker setup and configuration for sending the information from Temenos Transact to ElasticSearch and Logstash is added to display in Grafana.


##### Enabling Events to Grafana in the SPF Table

In the SPF table, Ext option in the Maint Tec Output field is used to enable the events to Grafana

You must set the Maint Tec Output field to Ext to trigger various events from Temenos Transact to Grafana.

The events are triggered from Temenos Transact and sent to TecEvent, which is a Platform Framework function.


##### Setting the List of Items in TEC.PROFILE

In the TEC.PROFILE table, you can set the list of items for which the events must be triggered in Grafana monitor.

> **⚠️ Note:** The list of items should have an entry in TEC.ITEMS table with defined threshold.

The following screen capture shows the list of events triggered from Temenos Transact system to Grafana.


##### Updating TAFJ

From TAFJ , go to conf and perform the following:

1. In the tafj.properties file, add the following property. temn.tafj.runtime.enable.jbc.meter=true
2. In TAFJTrace.properties , uncomment as shown in the following screen capture. Where, the host in appender.audit.host can be set to localhost or the system IP Address.
3. In TAFJTrace.properties , comment the properties mentioned in the following screen capture.
4. In TAFJTrace.properties , add the following line: log4j.logger.LOCKING=INFO,locking


##### Configuring Docker

This section guides you in configuring Docker.

As a prerequisite, you must install Docker in local system to run various containers, which sends the information from Temenos Transact to Grafana.

1. You can downloaded Docker from the Docker for Windows Released Notes link and install in the local system.
2. From TAFJ/TemnMonitor , execute the following commands: launch-monitoring.bat build launch-monitoring.bat up On successful execution of the commands, the Docker dashboard is displayed as follows:


##### Configuring Grafana

To configure Grafana,

1. Launch Grafana Dashboard from Web Browser by using the http://localhost:3000 link.
2. Login to Grafana using the default Username and Password admin/admin .
3. On the left pane, click the Data Sources , under Elasticsearch , set Version as 7.0+ .
4. Click Save and then Test . Message stating Index OK. Time field name OK is displayed. The elastic search is in-lined with Temenos Transact and data is sent from Temenos Transact .


#### 📋 Tasks

Temenos Transact allows external systems to monitor the progress of COB and the results can be viewed in T24 log, as a Data Event Streaming (DES) event, and in the Grafana dashboard. This section explains how Temenos Transact monitors the progress of COB.

Monitoring the COB Progress as DES Event and in Grafana Dashboard

This section explains how to monitor the COB progress as DES event and in Grafana dashboard.

Monitoring the COB Progress in T24 Log

This section explains how to monitor the COB progress in T24 log.

---


---


## Chapter 2: Infrastructure - GP


Infrastructure - GP module of Temenos Transact


### 2.1  Global Processing


> **📇 Quick Reference Card**
> 
> **Key Fields:** *Batch Holiday*, *Branch Holiday*, *Company Group*, *Global Process*, *Official Holiday*, *Relative Time*
> 
> **Sections:** ⚙️ Configuration | 📋 Tasks


#### ⚙️ Configuration

This section details the features available in Global Processing (GP), which support independent COB processing.


##### How to Group Companies?

The GP product allows you to group the companies using the Company Group field in the COMPANY record. This field identifies the group to which this company belongs. The values are 001–999, which indicate the first three numeric elements of the company ID.

COB runs separately for each company. However, it is recommended to run COB for group of companies.


##### Inter-company Group Accounting

The GP environment allows inter-company accounting within the same group of companies, which is defined in INTERCO.PARAMETER . This application restricts the usage of accounts from other companies belonging to different groups.


##### Company Holiday Definitions

In GP, you can maintain different calendars for each company at batch, official and branch level as explained below.

The Batch Holiday field in the COMPANY record defines the holiday table to control the Temenos Transact batch cycling. The value in this field has a two-character country code followed by two numeric characters from the HOLIDAY record. Each working day in this calendar is an operational day for Temenos Transact with a corresponding COB.

> **⚠️ Note:** For GP, the value of Batch Holiday can vary across companies. However, this value must be the same across companies belonging to the same group. In a non-GP environment, the values must be the same for all companies.

The Official Holiday field defines the official business holiday table for the local country related to the company. This field defaults the value from the Batch Holiday field, if left blank.

The Branch Holiday field defines the business holiday table used by the corresponding company or branch. The actual working days of the branch may be different from the official holidays, for example; a branch located in a shopping centre functioning on a Saturday. This field defaults the value from the Official Holiday field, if left blank. The value in this field is considered for the local country calendar in the default date calculations.


##### Time Difference Among Companies

The system records the date and time of a transaction based on the server date and time in the Date Time and Audit Date Time fields. You can also configure these fields to capture the local time of a transaction instead of the server time.

For the latter facility, the Relative Time field in the COMPANY record must have a value corresponding to the company related to the server. For example, a server running in Amsterdam on Central European Time (CET) with a UK based company should show -1:00 as the Relative Time in the UK Company.


#### 📋 Tasks

This section details how to install and activate the GP product in Temenos Transact .

> **⚠️ Note:** You must configure Temenos Transact Multi-company (MC) application and perform database backup (recommended).

Procedure:

1. Install the GP product in the SPF application. Contact Temenos for GP license key, if unavailable.
2. Set the Global Process field in SPF to Y . This will enable GP mode for independent COB.

---


---


## Chapter 3: Infrastructure - NS


Infrastructure - NS module of Temenos Transact


### 3.1  Non-Stop Processing


> **📇 Quick Reference Card**
> 
> **Sections:** ⚙️ Configuration | 📋 Tasks


#### ⚙️ Configuration

This section lists all the applications in Temenos Transact , which support NS completely for new and existing contracts and their corresponding business area.


##### New Contracts Only

The following applications allows only new contracts to be input during the COB .

| Application Name | Business Area |
|---|---|
| AZ.ACCOUNT | ALL IN ONE ACCOUNTS |
| FACILITY | SYNDICATED LOANS |
| FD.FID.ORDER | FIDUCIARIES |
| FD.FIDUCIARY | FIDUCIARIES |
| FOREX | FOREIGN EXCHANGE |
| FRA.DEAL | FWD RATE AGREEMENT |
| LD.LOANS.AND.DEPOSITS | LOANS AND DEPOSITS |
| LD.SCHEDULE.DEFINE | LOANS AND DEPOSITS |
| MG.MORTGAGE | MORTGAGES |
| MG.PAYMENT | MORTGAGES |
| MM.MONEY.MARKET | MONEY MARKET |
| PD.CAPTURE | PAST DUE |
| PD.PAYMENT.DUE | PAST DUE |
| PRE.SYNDICATION.FILE | SYNDICATED LOANS |
| SC.EXE.SEC.ORDERS | SECURITIES |
| SEC.OPEN.ORDER | SECURITIES |
| SEC.TRADE | SECURITIES |
| SECURITY.TRANSFER | SECURITIES |
| SC.SETTLEMENT | SECURITIES |
| SEC.ACC.MASTER | SECURITIES |
| SECURITY.MASTER | SECURITIES |
| SL.BUY.SELL | SYNDICATED LOANS |
| SL.CHARGE | SYNDICATED LOANS |
| SL.FACI.RATES | SYNDICATED LOANS |
| SL.LOANS | SYNDICATED LOANS |
| SL.RATES.PART | SYNDICATED LOANS |
| SL.REPAYMENT.SCHEDULES | SYNDICATED LOANS |
| SL.ROLLOVER | SYNDICATED LOANS |
| SWAP | SWAPS |


##### New and Existing Contracts

The following applications are fully non-stop enabled.

| Application Name | Business Area |
|---|---|
| AA.ARRANGEMENT.ACTIVITY | AA LOANS, DEPOSITS and ACCOUNTS |
| AC.LOCKED.EVENTS | ACCOUNTS |
| ACCOUNT | ACCOUNTS |
| ACCOUNT.CLOSURE | ACCOUNTS |
| ACCOUNT.CREDIT.INT | ACCOUNTS |
| ACCOUNT.DEBIT.INT | ACCOUNTS |
| ACCOUNT.DEBIT.LIMIT | ACCOUNTS |
| ACCT.CAPITALISATION | ACCOUNTS |
| ACCOUNT.STATEMENT | ACCOUNTS |
| ACCT.STATEMENT.CHARGE | ACCOUNTS |
| ACCT.INTERIM.CAP | ACCOUNTS |
| BALANCE.REQUIREMENT | BALANCES |
| CURRENCY | CURRENCY |
| CUSTOMER | CUSTOMER |
| CUSTOMER.SECURITY | CUSTOMER |
| DATA.CAPTURE | DATE CAPTURE |
| DEBIT.INT.ADDON | DEBIT INTEREST |
| DE.CUSTOMER.PREFERENCES | DELIVERY |
| ;DE.PRODUCT | DELIVERY |
| ENTITLEMENT | SECURITIES |
| FORWARD.RATES | FORWARD RATE AGREEMENTS |
| FUNDS.TRANSFER | FUNDS TRANSFER |
| GENERAL.CHARGE | CUSTOMER |
| GROUP.CAPITALISATION | CUSTOMER |
| GROUP.CREDIT.INT | CUSTOMER |
| GROUP.DEBIT.INT | CUSTOMER |
| HIGHEST.DEBIT | BALANCES |
| INTEREST.STATEMENT | INTEREST |
| NOTICE.WITHDRAWAL | ACCOUNTS |
| PAYMENT.STOP | CHEQUES |
| PERIODIC.INTEREST | INTEREST |
| STANDING.ORDER | STANDING ORDERS |
| TELLER | TELLER |
| TELLER.ID | TELLER |
| TRANSACTION.CHARGE | ACCOUNTS |
| TURNOVER.CREDIT | ACCOUNTS |
| TURNOVER.DEBIT | ACCOUNTS |

> **⚠️ Note:** See individual user guides of the respective application to understand the behaviour specific to NS processing.


#### 📋 Tasks

This section details how to install and activate the NS product in Temenos Transact .

Procedure:

1. Install the NS product in the SPF application. Contact Temenos for NS license key, if unavailable.
2. Include the NS product in the COMPANY records as required. For example, the bank can enable NS facility for specific branches, which handle critical operations.

---


---


## Chapter 4: Infrastructure - OF


Infrastructure - OF module of Temenos Transact


### 4.1  OFS features


> **📇 Quick Reference Card**
> 
> **Purpose:** *Open Financial Service (OFS) is an interface that allows our core banking software, Temenos Transact, to process transaction and query requests. This guide shows you how OFS works, and provides a reference to its features and syntax.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks | 📊 Outputs


#### 📖 Introduction

Open Financial Service (OFS) is an interface that allows our core banking software, Temenos Transact, to process transaction and query requests. This guide shows you how OFS works, and provides a reference to its features and syntax.

> **⚠️ Note:** This guide does not describe the available connectivity options for communicating with OFS. For more information, see the Transact Connectivity User Guides . You can find XML schema information at https://www.temenos.com

Overview of the Open Financial Service (OFS)

This topic provides an overview of OFS, the interface that provides a single point of entry to Temenos Transact. Every interaction with Transact takes place through OFS.

Configuring OFS.SOURCE

Before you can process OFS requests, you need to configure OFS.SOURCE. OFS.SOURCE contains the parameters for setting up an OFS connection with Transact.

OFS Requests and Responses

These topics describe the syntax of OFS requests and responses.

OFS Special Characters

Special characters can be used in OFS messages.

Other Features

These topics describe a variety of other OFS features, ranging from API features and security to message logging.


#### ⚙️ Configuration

This topic provides an overview of OFS, the interface that provides a single point of entry to Temenos Transact. Every interaction with Transact takes place through OFS.


##### Request Types

OFS offers the following distinct request types:

- Transactions.
- Enquiries.
- Clearing.
- TEC OFS Interface. The TEC OFS Interface is a subroutine which takes TEC.ITEMS such as ITEM.ID and processes the record data.
- XML report requests.
- Inward delivery messages (SWIFT).
- Routine requests.


##### Features

OFS offers the following features:

- An (optional) audit trail for messages.
- API hooks for pre and post processing.
- Fully multi company or multi book aware.
- Full support for hierarchical data (multi values, sub values).
- Full multi-lingual support.

> **⚠️ Note:** This guide does not describe the available connectivity options for communicating with OFS. For more information, see the Transact Connectivity User Guides . You can find XML schema information at https://www.temenos.com


#### 📋 Tasks

The following topic comprises example OFS requests.

OFS examples are shown with the following credentials.

| Column 1 | Column 2 |
|---|---|
| Username | TEST.USER |
| Password | 654321 |


##### Transactions

Example: Transaction OFS request

Example: FOREX swap transaction OFS request

The following example OFS request relates to a foreign exchange swap transaction, where information is required for both legs of the swap. The _ (underscore) character is used to delimit information for record 1 from record 2.


###### Example: AA Arrangement Activity update OFS request

The following example relates to an AA Arrangement Activity update. To populate a AA.ARR. within an arrangement, you need to follow the convention:

PROPERTY:N:1= ,FIELD.NAME:N:1= ,FIELD.VALUE:N:1=


##### Enquiries

Example: Enquiry OFS request


##### XML Reports

Example: XML report OFS request


##### TEC OFS Interface

Example: TEC OFS Interface OFS request


##### Clearing

Example: Clearing OFS request


##### Inward Delivery Message (SWIFT)

Example: Inward delivery message (SWIFT) OFS request


##### Routine Requests

Example: Routine request


#### 📊 Outputs

This topic describes the OFS request syntax of XML reports.

It references the following example message.

XML.REPORT,XML,TEST.USER/654321,PXML.CURRENCY.LIST


##### Operation

XML.REPORT

To run an xml report, you need to set the operation to XML.REPORT.


##### Options

The options are either XML or ID.

| Options | Description |
|---|---|
| ID | ID returns the HOLD.CONTROL key that was produced when the report was run. This means that the XML can be extracted asynchronously. |
| XML | XML returns the XML result. |


##### ID information

REPORT.CONTROLID

The key of the ENQUIRY.REPORT to run.


##### Data

Not required. It is possible to verify ENQUIRY records and have the '&HOLD&' ID or the entire XML message brought back in the return message.

The application title has changed from ENQUIRY.REPORT to 'XML.REPORT'. The OFS module translates the 'XML.REPORT' script and applies it to the ENQUIRY.REPORT application.


###### Configuring XML Reports

XML reports are configured through the ENQUIRY.REPORT, where:

- The OUTPUT.FORMAT must be set to XML.
- The corresponding REPORT.CONTROL record has the FORM.NAME set to 'HOLD'.

---


---


## Chapter 5: Infrastructure - PW


Infrastructure - PW module of Temenos Transact


### 5.1  Process Orchestration


> **📇 Quick Reference Card**
> 
> **Purpose:** *The TEMENOS Process Orchestration Group is responsible for the strategic direction, development and maintenance of the TEMENOS business process automation, management and monitoring solutions.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration | 📋 Tasks


#### 📖 Introduction

The TEMENOS Process Orchestration Group is responsible for the strategic direction, development and maintenance of the TEMENOS business process automation, management and monitoring solutions.

This includes the existing Process Workflow module and other functional micro workflows (override Override class, Dispo, approvals etc.), with a strategic goal to consolidate all within a unified industry standard business process management and business activity monitoring solution.

Introduction

You will need to understand some basic concepts, and set up some prerequisites, before you can use Process Orchestration.

Configuring PW module components

Some components need to be configured for Process Workflow.

Mapping

Mapping allows you to transfer information automatically from one activity to another.

Configuring process versioning

Process Workflow supports versioning, which allows an instance of a process to follow the (version of the) definition with which it was created.

Executing Process Workflow Activities

This section describes how you can execute process workflow activities by defining logical prerequisite conditions using parenthesis in the PW.PROCESS.DEFINITION application.

Using pattern-based workflows

In addition to sequential workflows, the PW module supports pattern-based workflows.

Special Features: Using variables

Process Workflow supports the concept of process variables which can be used in different stages of the process to govern the process flow logic.

Allocating tasks to external users

You can allocate tasks to external users using process variables.

Monitoring and reporting

You can monitor and report on Process Orchestration.

Glossary

There are some terms you need to understand when using Process Orchestration.

For more information about the Temenos Transact External BPM see T24 External BPM - User Guide .


#### ⚙️ Configuration

Automatic screen presentation takes place when the same USER or ACCOUNT.OFFICER defined in PW.PARICIPANT is part of the USER profile - in other words, the user who caused the activity to be launched is a member of the group. It also takes place when the PW.PROCESS.DEFINITION record has the field FOLLOW.ON.ACT set to Yes - in other words, when the next step is intended to be presented to the user automatically.

For more information, see PW.PROCESS.DEFINITION .

The USER or Account.Officer detailed in the PW.PARTICIPANT record must be the same as the USER profile executing the workflow.

Example: To use the functionality, the USER profile of CSAGENT whose Acc.Officer number will need to be used.


##### Adding the participant to an activity

Procedure

1. Include the PW.PARTICIPANT record in the Owner field in the PW.ACTIVITY record that you use.
2. The PW.PROCESS.DEFINITION record contains all the PW.ACTIVITY records that are included in the workflow. To allow the new automatic launch functionality, set the field FOLLOW.ON.ACT to YES . To control the order in which the flagged PW.ACTIVITY records are launched you need to use the PRE.REQ.ACT field. This will allow this functionality to operate.


##### Testing the functionality

The simplest way to test the Automatic Screen Presentation functionality is to perform the following steps.

1. Manually launch a PW.PROCESS record.
2. Specify the process to follow.
3. Provide the PW.PARTICIPANT in the owner field.
4. Commit the record. As soon as the PW.PROCESS record is committed and authorised the new functionality automatically launches the first activity flagged for automatic launch in the PW.PROCESS.DEFINITION record. Once the first activity has been committed, the process checks to see if any other activities can be launched. In this case, another activity is launched and as it also has Follow On Act set to YES and the user is in the appropriate group, the second activity is launched automatically. The ACCOUNT.OFFICER field has been populated showing that data mapping is operating in the new functionality.


#### 📋 Tasks

The PW process engine can loop back to a previous activity or repeat certain activities activities within a process.

The looping can be triggered with or without conditions. It is also possible to add a different construct in the workflow to control the flow of the process. You can configure which activity is to be executed next or executed more than one activity in parallel. PW.PROCESS.DEFINITION is used to set up the loops and constructs.

For example while creating a customer record, all available documents should have been supplied by the customer. You could potentially have a situation where a document is missing and it later supplied by the customer. In such a case, the transaction must be re-executed. This may happen after the next activity has completed.

Note that different patterns can only be defined in PW.PROCESS.DEFINITION, only if the field USE.WORKFLOW.PATTERNS in PW.PARAMETER is set to YES.

---


---


## Chapter 6: Infrastructure - SM


Infrastructure - SM module of Temenos Transact


### Features in Infrastructure - SM


| # | Feature | Sections |
|---|---------|----------|
| 6.1 | ExternalAuthorisation | Confi, Tasks |
| 6.2 | Sms | Intro, Confi |


### 6.1  ExternalAuthorisation


> **📇 Quick Reference Card**
> 
> **Sections:** ⚙️ Configuration | 📋 Tasks


#### ⚙️ Configuration

The design time section guides you to the UI layout and different intractable components or elements to create and model a policy.


##### Policy Editor

The Temenos Security Framework provides Policy Editor, which is an access control-authoring tool. It has a simplified graphical user interface and enables security administrator to author the access control policies.

The application layout is divided into two main sections:

- The left pane is a toolbar, which contains three core elements to interact when you use the application.
- The central or right pane is an editor, which allows you to configure a given policy inline (directly editing) by modifying the properties of the policy.

The left pane is called a toolbar.

It contains three core elements with which you can interact when using the application.

- The first element is the set of categories called as policy elements. You can either click on the categories or drag them into the editor (right pane) to create an element of this type in the policy.
- The second element is the elements section which shows the list of currently deployed or existing policy elements in the system. You can click the categories to filter them. Either you can drag and drop the elements or you can inspect using the controls located on the right of the element entry.
- The overview element, located below the elements, displays a simple overview of the policy. You can click the nodes of the policy to expand and examine the policies or you can just focus the clicked node in view in the editor.

The Editor pane consists of two major sections.

The top section of the editor pane allows you to:

- Manage and control the editor.
- Create new projects
- Download the current project
- Upload a new project
- Inspect and configure the application settings (such as font size and family, language, application theme and more).
- Change the name of the tab or project, when a new project or tab is created in the editor. The modified name of the tab or project eventually becomes the name of the file that is downloaded.

The top section lies the actual editor section, which shows the policy and enables you to configure and model the policy in place directly in the editor.

The editor section supports two main ways of interaction:

- Using drag and drop
- Using the controls of each policy element (add, delete, edit, etc.).

To use the drag and drop option, you can grab policy element from the list of elements on the left (toolbar pane) and drop it inside the policy editor. You can also grab a category from the list of four categories on the top of the toolbar pane to create an empty policy element of that type.

> **⚠️ Note:** You must be aware that elements have rules and you should drag and drop the elements as per the rules.

You can create or drop:

- Permissions in Role
- Rules and Obligations in Permissions

Each of the different policy elements in the editor can be collapsed by using the control on the left top of the element. This allows the editor to show more information and be more compact while at the same time it also gives more space for editing.

Roles and Permissions both have the ability to also filter their elements / contents by using the free text search on the right of the Roles or Permissions elements you can filter the contents by either the Identifier or Description of the contained element.

When editing a policy element it is important to note that some of the properties of a policy element can be required or constrained in some manner. For some of the properties, you cannot enter random values but you should comply to either the constraints applied to the property (such as being unique, required etc.) or select a value from a predefined list of values (such as product, resource, algorithm etc.). It is also important to notice that some properties depend on others. A prime example of that is the resource property which depends on the product and unless the user selects a product he would not be able to select a resource.

Roles and Obligations depend on the product and resource being selected or defined first before you use them.

When you drag an existing element from the elements pane on the left he creates what is called a reference. The reference means that the current policy which is using this dragged policy element is only refereeing to it but not copying it directly.

What this implies is that if the reference changes all of the policies referring to this policy element would immediately be affected. That is why referenced elements are not directly editable from policies which reference them but are only editable from the policy from which they originate (in other words only the policy inside of which they were initially created)

You can navigate to the original policy using the controls on the right of the policy element (using the edit action, you can either navigate to the original element being referenced or create a local copy of the referenced element).

> **⚠️ Note:** All intractable controls in the PAPUI have a tooltip associated with them.

You can hover over any intractable part of the UI and receive a tooltip, which describes control action and how it can be used in the current context.


##### Interaction APIs

IRIS APIs are used to provide input data for UI and to download policy files

IRIS R18 provider API’s are used to fetch data from Temenos Transact and the data fetched is then used by the UI to define and create policy files. This fetching of Temenos Transact data is a onetime process and the results are stored in a physical location/repository from where the UI picks it up for further processing of policy files.

There are two API’s:

- To retrieve all the resources from Temenos Transact , (here, resources refer to all the applications, versions and enquiries present in the system), you have to use the /system/resourceManagers/{resourceManagerId}/resources URI for the resource API:
- The second API fetches the attributes for a particular resource. The URI for the attribute API is /system/resources/{resourceType}/{resourceId}/attributes .

Apart from the two above provider APIs, there are provider meta APIs developed to initiate the above two APIs and to return static data for the Subject, Environment, operators, obligations, combined algorithms and actions.

All the above APIs are packed as a WAR file ( irf-provider-container.war ) in the JBoss deployments folder. To configure path for download or upload of the resource and attribute, navigate to the WAR file WEB-INF\classes\irf-config\ folder and edit the save-file-config file directory path:


##### Static Data for Editor

Different data types support specific operators as shown below.

| Action | Corresponding Action Id in Temenos Transact |
|---|---|
| authorize | A |
| secondLevelAuthorisation | A2 |
| backgroundValid | B |
| copy | C |
| delete | D |
| exception | E |
| fastInput | F |
| historyRestore | H |
| input | I |
| list | L |
| print | P |
| reverse | R |
| see | S |
| verify | V |
| audit | Q |

| Subject | Example |
|---|---|
| userId | Current User |
| roleId | User Roles |


##### Authorisation Extension

The Custom Data API and Link Data API fields in the EB.EXT.SMS.EXTENSION application are used to attach L3 API Implementation or JBC Implementation for user customised attribute names that can be used in XACML Policy Files.

You must create routines in accordance with the following definitions provided as support from the Temenos Security Framework.

| Definition | CUSTOM.DATA.API | LINK.DATA.API |
|---|---|---|
| Arguments | Argument 1: Application Name Argument 2: Record Id Argument 3: Record | Argument 1: Application Name Argument 2: Record Id Argument 3: Record Argument 4: External Attribute Name |
| Return Values for JBC | Argument 1: External Attribute Name Argument 2: Value for the attribute | Argument 1: Value for the attribute |
| L3 API Method Definition | List getAttributeValuePair (String application, String recordId, TStructure record){} | String getAttributeValue(String application, String recordId, TStructure record, String attributeName){} |

Snippets

CUSTOM.DATA.API

LINK.DATA.API


#### 📋 Tasks

This section helps you to create and download a policy from Policy Administration Point User Interface (PAPUI).

You can open the PAP UI from the Browser using the http:// : /papui (for example, http://localhost:9089/papui ) link.

A new untitled role is created by default when you open the PAP UI.

With the following requirements, this section helps you to create a role using the PAP UI:

- Create a role or policy named CSAGENTRole which has access to CUSTOMER application and allow access if nationality and residence is equals to GB and customer other officer is equals to 1 (Implementation) or 2 (Retail Banking Mgr).
- %CUSTOMER, CUSTOMER.SCV enquiry and lists only the records with nationality and residence is equals to GB.

The following steps helps you to create the CSAGENTRole role or policy using PAP UI.

1. Rename the role name to CSAGENTRole from Untitled as shown below.
2. Rename the role identifier (roleid) to CSAGENTRole and provide the description and the algorithm as deny-unless-permit as shown below.
3. Add a permission by providing the required details in the Permission section. Add the below details. Permission Id : Determines the identifier for the permission. It should be unique. For example, fill it as Access_Customer_Application Description : Descriptive text for the permission. For example, fill it as “Customer Application Access” Product : Product that this permission is applicable to. For example, select T24 from the dropdown. Algorithm : Algorithm that PDP applies to combine the decisions of the rules For example, select permit-unless-deny from the dropdown. Resource Type : Type of resource that the permission is applicable to. For example, select APPLICATION, since the CUSTOMER is an application in T24. Operator Type : The operator to apply between the resource type and the resource to select the list of resources that permission is applicable for. For example, select equal from the dropdown. Resource : Name of the resource that the policy/permission is applicable for.
4. For example, select CUSTOMER application.
5. To restrict creating the Customer records with Nationality or Residence as GB, add those as a rule as shown below. Add the below details. Identifier : Identifier for the rule. The value provided in this filed should be unique. For example, fill it as Allow_GB_Residence. Description : Descriptive text for the rule. For example, fill it as “Allow for only GB Residence Customers”. Effect : Effect of the rule when the condition inside the rule matches. Either Permit/Deny should be selected. For example, select Deny, since you are going to allow the access to the resource with Nationality and Residence as GB or Other Officer is equals to 1(Implementation) or 2(Retail Banking Mgr). Operator for condition groups : Operator to apply between the conditions For example, you can leave it to default, that is, OR. Attribute : Select the attribute that the condition should be evaluated against. For example, select resouce.Nationality, resource.Residence and resource.Other.Officer, since you are checking the Nationality and Residence of the Customer is GB and Other Officer is equals to 1(Implementation) or 2(Retail Banking Mgr). Operator : Operator to apply between the Attribute and the Attribute value. For example, select not-equal, since you are checking the Nationality and Residence of the Customer is GB and Other Officer is equals to 1(Implementation) or 2(Retail Banking Mgr). If the value is not equals to the specified values then the rule will be evaluated to Deny. Bag Type : It is used to specify the values for Multi Value Attributes. For Example: it is not applicable for Nationality and Residence, since they are single value attributes, but applicable to Other Officer, since it is a Multi Value attribute. The allowed values are: any-of-any :This expression is "True" if at least one of the elements from the specified values, is equal (Based on Operator specified like not-equal, greater-than, less-than, etc..) to at least one of the elements from the corresponding resource attribute values. If resource.OTHER.OFFICER Bag Type is specified as any-of-any (shown below), then only the records that contain OTHER.OFFICER as 1(Implementation) or 2(Retail Banking Mgr) are applicable. all-of-any :This expression is "True" if each of the elements from the specified values, is equal(Based on Operator specified ex: not-equal, greater-than, less-than, etc..) to at least one of the elements from the corresponding resource attribute values. any-of-all :This expression is "True" if at least one of the elements from the specified values, is greater-than(Based on Operator specified ex: not-equal, equal, less-than, etc..) to each of the elements from the corresponding resource attribute values. all-of-all :This expression is "True" if each of the elements from the specified values, is equal(Based on Operator specified ex: not-equal, greater-than, less-than, etc..) to each of the elements from the corresponding resource attribute values. bag-size :It counts the number of values for a particular Multi Value Attribute. Value : Attribute value that the condition should check for. Nationality and Residence of the Customer is GB and OTHER.OFFICER is equal to 1(Implementation) or 2(Retail Banking Mgr).
6. Create another Permission of OBLIGATION Type to specify the conditions to apply for executing the enquiry. Since the role can access %CUSTOMER and CUSTOMER.SCV enquires and those enquiries should list only the records of CUSTOMER with Residence and Nationality as GB.
7. To specify the filtering conditions for the enquiry, create a new permission with ResourceType as Obligation and Resource as Customer (since %CUSTOMER and CUSTOMER.SCV belongs to the CUSTOMER application) Add a Permission by clicking + adjacent to the Role as shown below. Permission Id : Determines the identifier for the permission. It should be unique. For example, fill it as Access_Customer_Obligation. Description : Descriptive text for the permission. For example, fill it as “Customer Obligation Access” Product : Product that this permission is applicable to. For example, select T24 from the dropdown. Algorithm : Algorithm that PDP applies to execute the permission on the resource. For example, select permit-unless-deny from the dropdown. Resource Type : Type of resource that the permission is applicable to. For example, select OBLIGATION. Operator Type : The operator to apply between the resource type and the resource to select the list of resources that permission is applicable for. For example, select equal from the dropdown. Resource : Name of the resource that the policy/permission is applicable for. For example, select CUSTOMER Obligation.
8. Add an obligation by clicking + adjacent to the permission as shown below, which lists only the customers with the Residence of the customer is GB. Provide the following details in the Obligation section. Identifier : Unique identifier for the obligation. For example, fill it as Allow_GB_Residence_Oblig. Description : Obligation to Filter to list only customers with Residence as GB For example, fill it as “Allow GB Residence” Type : Type of obligation to be applied in Policy Enforcement Point (PEP). For example, select Filter. Fulfillon : Determines when the obligation should be fulfilled/applied. Possible values are Permit or Deny. When permit is selected, Obligation will be applied when the permission evaluates to permit. When deny is selected, Obligation will be applied when the permission evaluates to deny. For example, select Permit. When the decision is permit, you can filter the records with RESIDENCE as GB. Attribute : Select the attribute that the obligation filter should be evaluated against in the PEP. For example, select resource. RESIDENCE, since you need to check if the RESIDENCE of the CUSTOMER is GB. Operator : Operator to apply between the Attribute and the Attribute value. For example, select equal, since you are checking if residence is equals to GB. Value : Attribute value that the filter should check for. For the purpose of this demo value select GB.
9. Add another obligation by clicking + adjacent to the permission as shown below, which lists only the customers with the Nationality of the customer is GB . Provide the following details in the Obligation section. Identifier : Unique identifier for the obligation. For example, fill it as Allow_GB_Nationality_Oblig. Description : Obligation to Filter to list only customers with Nationality as GB For example, fill it as “Allow GB Nationality” Type : Type of obligation to be applied in PEP. For example, select Filter. Fulfillon : Determines when the obligation should be fulfilled/applied. Possible values are Permit or Deny. When permit is selected, Obligation will be applied when the permission evaluates to permit. When deny is selected, Obligation will be applied when the permission evaluates to deny. For example, select Permit, since, when the decision is permit, you have to filter the records with NATIONALITY as GB. Attribute : Select the attribute that the obligation filter should be evaluated against in the PEP. For example, select resource. NATIONALITY, since you need to check if the NATIONALITY of the CUSTOMER is GB. Operator : Operator to apply between the Attribute and the Attribute value. For example, select equal, since you are checking if nationality is equals to GB. Value : Attribute value that the filter should check for. For the purpose of this demo value select GB. You have added another permission and obligation inside it.
10. Create a permission for giving access to %CUSTOMER and CUSTOMER.SCV enquiries and create rule, which holds allowed enquiries for this role. Add a permission by clicking + adjacent to the Role as shown below. Permission Id : Determines the identifier for the permission. It should be unique. For example, fill it as Access_Customer_Enquiry Description : Descriptive text for the permission. For example, fill it as “Customer Enquiry Access” Product : Product that this permission is applicable to. For example, select T24 from the dropdown. Algorithm : Algorithm that PDP applies to execute the permission on the resource. For example, select permit-unless-deny from the dropdown. Resource Type : Type of resource that the permission is applicable to. For the purpose of this demo resource type select ENQUIRY, since the %CUSTOMER and CUSTOMER.SCV are an enquiries in Temenos Transact . Operator Type : The operator to apply between the resource type and the resource to select the list of resources that permission is applicable for. For example, select equal from the dropdown. Resource : Name of the resource that the policy/permission is applicable for. For example, select %CUSTOMER enquiry initially and click on the + icon adjacent to the Permission Resource drop down as shown below.
11. Since the allowed Enquiries for this Role are %CUSTOMER and CUSTOMER.SCV, add it as a rule as shown below.
12. Add a rule clicking + adjacent to the permission as shown below.
13. The first attribute value of Rule is automatically set to %CUSTOMER.
14. You have to change the Enquiry Resource to %CUSTOMER.SCV and click the + icon adjacent to the Permission Resource drop down as shown below. The next attribute value of Rule is automatically set to CUSTOMER.SCV. Add the following details. Identifier : Identifier for the rule. The value provided in this filed should be unique. For example, fill it as Allowed_Enquiries. Description : Descriptive text for the rule. For example, fill it as “Allowed Enquiries for this Role”. Effect : Effect of the rule when the condition inside the rule matches. Either Permit/Deny should be selected. For example, select Deny to allow the Enquiries for this Role. Operator for condition groups : Operator to apply between the conditions For example, you can leave it to default, that is, OR. Attribute : Select the attribute that the condition should be evaluated against. For example, select resouce.resourceId. Operator : Operator to apply between the Attribute and the Attribute value. For example, select not-equal, since you are checking the resourceId of the Customer is %CUSTOMER or CUSTOMER.SCV. Bag Type : It is used to specify the values for multi-value attributes. For example, it is not applicable for resourceId, since they are single value attributes, so you can ignore it. Value : Attribute value that the condition should check for resourceId of the customer is %CUSTOMER or CUSTOMER.SCV. As shown above, you have given access to %CUSTOMER and CUSTOMER.SCV enquiries. When these enquiries are executed in Temenos Transact , the OBLIGATION attached to the CUSTOMER resource returns to Temenos Transact as filters. Then, these filters are added to the database query and the results contain only the GB customer records.


##### Creating Policy with Enhanced Obligations

Enhanced obligations provide a greater flexibility in designing the obligations. With this feature, the policy editor can:

- Create policies with multiple filter conditions inside a single obligation group.
- Define the grouping operator between the filter conditions.
- Define the grouping operator between the obligation groups

You can create a policy with enhanced single or multiple obligation groups.

To combine a group of filter conditions with a single operator (AND/OR), single obligation group is enough to create the policy.

As shown in the above example, single obligation group can be used when the combining operator (AND) is the same between the filter conditions.

To create a policy with single obligation group,

1. Create a policy and add permission
2. Add obligation for the permission
3. Add filter conditions in the obligations
4. Choose the combining operator The policy is created successfully with single obligation group.

The above policy has three filter conditions in a single obligations group with the combining operator as AND. PEP will apply the AND condition between the filter conditions that are present in the obligation group and frames the database query and extracts only the relevant records that satisfy the filter conditions.

The framed condition from the above obligation will look as shown below.

To combine a group of filter conditions with both the operators (AND/OR), multiple obligation groups are required to create the policy.

As shown in the above example, multiple obligation group needs to be used when there are a set of conditions that need to be combined with the AND operator and another set of conditions that needs to be combined with the OR operator

In the above example there are 3 obligation groups:

- Obligation Group 1: It contains 3 filter conditions with OR as the combining operator (Condition1 OR Condition2 OR Condition3)
- Obligation Group Combining Operator: This obligation group does not contain any filter conditions but contains only the Logical Combining Operator between the 2 obligation groups. AND
- Obligation Group 2: It contains 2 filter conditions with AND as the combining operator. (Condition4 AND Condition5)

> **⚠️ Note:** A maximum of only 3 obligation groups can be attached to a permission with the same fullfillOn decision. You need to group all the AND conditions inside a single obligation group, all OR conditions inside another obligation group and combine those 2 groups with the obligation group combining operator.

To create a policy with single obligation group,

1. Create a policy and add permission
2. Add obligation for the permission
3. Add the filter conditions in the obligations
4. Choose the combining operator The above policy has 3 filter conditions in a single obligations group with the combining operator as AND.
5. Add another obligation group that denotes the combining operator between the two obligation groups.
6. Choose the obligation type from the Type dropdown Logical_OR: When this option is chosen, the two obligation groups are grouped with the OR condition. Logical_AND: When this option is chosen, the two obligation groups are grouped with the AND condition. There should not be any filter conditions in this obligation group
7. Add another obligation and add the filter conditions.
8. Choose the combining operator The policy is created successfully with single obligation group.

In the above policy, the obligation group has two conditions with the combining operator as OR. The framed condition from the above obligations will look as shown below.


##### Saving a Policy

Saving a Policy involves the following steps.

1. Download the role by clicking the download button as shown below.
2. Downloaded role can be seen in the papRuntime\json and papRuntime\xacml directories as shown below.


##### Advanced Mode

In the default standard mode of the policy administrator, the policies are standardised on the role and provided with a simple user interface for defining RBAC and simple ABAC conditions.

In the advanced mode, the policy editor enables an effective control over policy selection criteria and condition definitions. It enables attributes selection and advanced conditions such as using a regular expression, etc. It also allows policy definition that caters to banks preferred approach.

| Target | Operator | Value | Description |
|---|---|---|---|
| subject:roleId | equal | CSAgentRole | Executes or targets the Policy if subject:roleId is equal to CSAgentRole . |
| subject:roleId | regexp-match | ADMIN.* | Executes or targets the Policy if subject:roleId starts with ADMIN . Similarly, any regular expression can be used. |
| subject:userId | equal | TOM | Executes or targets the Policy if subject:userId is equal to TOM . |
| subject:userId | regexp-match | .* | Targets the Policy to all the users, since .* regex means everything. |

This section details the Advanced mode features.

Advanced mode allows the policy author to target the policy or role to any of the subject attributes as shown below.

The policy author can choose any attribute as per the requirement. For example, if a role has to be designed to target a specific user, then subject:userId can be chosen as the attribute.

It is also possible to customise the Comparison Operator as shown below.

For example, if a role has to be designed to target all the users with any roleId, then Operator can be chosen as regexp-match with the value provided as .* to match everything.

Advanced mode allows the policy author to type a Resource value (instead of just choosing the Resource from the drop-down). This feature gives the control to the policy author to type a regular expression in the Resource field by choosing the regexp-match as the operator type.

As shown in the above image, the policy author can type regular expressions in the Resource field.

To type a value in the Resource field, click the drop-down and type a value in the filter field, and click return .

This section shows the sample cases of Advanced mode.

This case creates a role ADMIN , which provides access to all the APPLICATIONS, VERSIONS, and ENQUIRIES of Transact if the roleId is ADMIN .

Perform the following steps to create the role:

1. Launch the Policy Editor (http:// : /papui) and create a new role in advanced mode.
2. Provide the file name as ADMIN . The value provided in the above-shown image is used as the file name. It can be different from the role name or identifier. Since the value provided is ADMIN , the XACML file is saved as ADMIN.xml .
3. Provide the unique value in the Identifier field as shown below. The value provided in the Identifier field is used as the reference to the policy in the root-policy.xml at the runtime.
4. Provide the following values for the Target , Operator Type and Value fields. Target : subject:roleId Operator Type : equal Value : ADMIN Algorithm : deny-unless-permit
5. Provide the values for the Permission fields as shown below. Permission Identifier : Application_Access Description : Access to all applications Product : T24 Algorithm : deny-unless-permit Resource Type : APPLICATION Operator Type : regexp-match Resource : .* Since the algorithm is chosen as deny-unless-permit , a rule has been added with the effect as Permit to permit.
6. Similarly add new permissions to provide access to all VERSIONS and ENQUIRIES.
7. Download the policy. As shown below, the XACML policy is downloaded with the regexp-match as the operator with the value as .* .

This case creates a role named INPUTTER , which provides access to the user with userId as INPUTTER and allows access to ENQUIRIES that contains the word CUSTOMER in it (for example, %CUSTOMER.ACCOUNT, %CUSTOMER.SECURITY).

Perform the following steps to create the role:

1. Create a new policy in advanced mode.
2. Provide values for the role fields as shown below. Policy File name : INPUTTER Role Identifier : INPUTTER_USER_ROLE Description : Role for the INPUTTER user Target : subject:userId Operator Type : equal Value : INPUTTER Algorithm : deny-unless-permit As shown above, subject:userId is chosen instead of subject:roleId . This indicates that the userId is the target rather than the roleId .
3. Provide values for the permission fields as shown below. Permission Identifier : Customer_Enquiries_Access Description : Access to enquiries that contains the word CUSTOMER Product : T24 Algorithm : deny-unless-permit Resource Type : ENQUIRY Operator Type : regexp-match Resource : .*CUSTOMER.*
4. Download the policy. As shown below, the XACML policy is downloaded with the subject.userId as defined in the Target field.


##### Fetching Transact Resources and Attributes through System API Call

In PAP UI, Transact fetches the Resources and Attributes data using system API call from the Transact database instead of papRuntime folder. All the products other than Transact uses the meta API call to fetch the Resources and Attributes data from the papRuntime folder.

From the PAP UI, while creating a new policy file:

- In the Permission section, if you select the T24 product, then the resources corresponding to T24 application names are displayed in Resource .

- In the Permission section, if you select Resource from the drop-down list, then in the Rule section corresponding Attributes system API response list is displayed from the Transact database.

---


### 6.2  Sms


> **📇 Quick Reference Card**
> 
> **Purpose:** *Security Management System (SMS) controls the access of Temenos Transact and it can restrict the access to some parts of the system. It detects, stops and records any attempt at unauthorised use of the system. It can also, if required, record all the activities performed by the selected users.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration


#### 📖 Introduction

Security Management System (SMS) controls the access of Temenos Transact and it can restrict the access to some parts of the system. It detects, stops and records any attempt at unauthorised use of the system. It can also, if required, record all the activities performed by the selected users.

Overview

This section explains the functionality of Security Management System (SMS).

User Profile and Security

This section explains the basic identity settings in the user profile.

Overrides

This section explains the usage of overrides.

Dispo System

Dispo processing is the ability to direct overrides to the people whose attention the override requires, and is in addition to the functionality offered by OVERRIDE.

External Authorisation

This section explains the Policy Administration Point User Interface (PAP UI), which allows the security policy administrator to create the eXtensible Access Control Markup Language (XACML) policies with interactive GUI and gives the ability to create and download the XACML policy files.


#### ⚙️ Configuration

This section explains the various features of Dispo.

When an OVERRIDE is encountered which is flagged for Dispo processing for the application that raised the OVERRIDE (as defined in the OVERRIDE table), a DISPO.ITEM record will be produced for the contract. Whilst this item is in effect with a status of NEW, the contract may only be authorised by a USER whose DISPO.OFFICER (set on the USER profile) matches that of the item.

For example, a FUNDS.TRANSFER contract raised a DISPO override, after agreeing to the override the User was presented with a transaction conformation message letting them know they had raised a DISPO override and that it is not approved.

Also if you look at the FUNDS.TRANSFER contract the DISPO override has been raised against the audit information.

The DISPO.SUMMARY ENQUIRY displays, for each DISPO.OFFICER , the number of items pending both for today, and for previous days.

From this ENQUIRY, the USER may choose to show the details of today’s items for a particular officer, or for the previous days. This invokes the DISPO.DETAILS ENQUIRY with the appropriate selection criteria.

The ENQUIRYDISPO.DETAILS provides a USER with information regarding overrides that require their attention.

This is a real time enquiry. Refer to the ENQUIRY chapter of the System Administration User Guide for full details on installing and using real time enquiries.

To the user, this means that when an item becomes marked for their attention, the enquiry updates automatically.

From this ENQUIRY, you can

- Add a comment to the item and forward the item for the attention of another officer
- Approve the item
- View the item in full

| DispoOfficer*Operator*DateTimeStamp | Description |
|---|---|
| Dispo Officer | The Officer defined in the DISPO.OFFICER field on USER profile. |
| Operator | The user that performed the update. |
| DateTimeStamp | The date and time the update was made. |

There are two types of manual routing:

- Comment Routing
- Approval Routing

Comment routing allows multiple DISPO.OFFICER profilesto comment on an item before it is routed to the DISPO.OFFICER to carry out the approval. It is the DISPO.OFFICER of the DISPO.ITEMS and not the Comment Officer that controls which USER may approve an item.

Comment routing is achieved by entering a new DISPO.OFFICER into the Comment Officer field on DISPO.ITEMS .

Approval routing modifies the USER who may authorise the contract.

This is accomplished by modifying the Dispo Officer field on DISPO.ITEMS .

> **⚠️ Note:** The records of DISPO.ITEMS are updated only through a zero authoriser version.

| Officer Code | Officer Description | Disposition Amount | Overdraft Competence | Next Level of Disposition |
|---|---|---|---|---|
| 1100 | Account Office A | 15,000 | 10,000 | 1101 |
| 1101 | Account Officer B | 20,000 | 20,000 | 1105 |
| 1105 | Account Officer C | 999,999,999,999 | 24,000 |  |
| 2400 | Top Management | 0 | 999,999,999,999 |  |

Each record of DISPO.ITEMS has a pending status option, which is stored in the Pend Status field. This is used by Temenos Transact to determine which items are to be re-routed back to the officer that last had the item following overnight processing. If an item is held overnight, with this flag being set to NO or left empty, then the record DISPO.ITEMS is reset to the first Dispo officer as per the parameters for precedence processing, routing for unavailable Dispo officer and so on. If this field is set to Yes, then the record of DISPO.ITEMS is not altered.

Each time a record in DISPO.ITEMS is updated the, Gen Comment field is updated with the contents of the Comments field and the following details are appended:

- The Dispo Officer who made the update
- The User ID of the User that made the update
- The time and date when the update was made.

When the input of a record causes an OVERRIDE and that OVERRIDEis marked for DISPO then a DISPO.ITEMS record is created. The status of each DISPO item on the record must be marked “APPROVED” before the originating record can be fully authorised. Only a USER who has a DISPO.OFFICER record with the application and appropriate competence will be able to approve a disco item.

Only after all the items within a DISPO.ITEMS record are approved, can the contract record be finally Authorised. The normal rules for a USER’s applications and OVERRIDE.CLASS apply.

The DISPO.ITEMS record may be updated only after all related non-dispo authorisations have taken place on the originating record.

In a multi-company environment it is possible for one of two paths to be followed during authorisation of a Dispo.

Dispo can be configured to utilise OFS to perform final authorisation for all transactions that are created in remote Company accounts. The SYSTEM record in the DISPO.PARAMETER application contains a reference to an OFS.SOURCE record that has been set-up to run in BATCH mode. On approval of all Dispo Items within a DISPO.ITEMS record, an OFS message with an instruction to authorise the original contract is created.

The second path taken is when DISPO.PARAMETER application has not been configured and the original contract requiring authorisation is in a remote company. Temenos Transact displays a message requesting that the user changes company to approve the Dispo.


###### DISPO.ITEMS,COMMENTS – AUTH.ROUTINE field

The AUTH.ROUTINE field within the DISPO.ITEMS,COMMENTS version has been updated to action a BASIC subroutine called DISPO.NEXT.VERSION when a record has been committed using the DISPO.ITEMS,COMMENTS version.

The BASIC subroutine called DISPO.NEXT.VERSION has been supplied to:

- For multi company environments: You should check if original contract should be authorised in a different company. If so, is it possible to generate an OFS message to complete the Authorisation? If it is not possible to generate an OFS message – advise the user to change company to the company where the contract was originally created.
- For Single company environments: Calculate the command required to complete authorisation of the original contract. Store the command in R.VERSION(EB.VER.NEXT.VERSION). Temenos Transact performs the command stored in R.VERSION(EB.VER.NEXT.VERSION). If it is not possible to create the OFS message, or the Temenos Transact environment is set up for Single Company only, calculate the command required to complete authorisation of the original contract.

The subroutine DISPO.NEXT.VERSION performs the following calculation when calculating the name of the version that is required to complete the authorisation of the original contract.

Once the version name is known, a command is constructed. This command is comprised of VersionName A OriginalContractId .

- VersionName is the version that performs final authorisation of original contract
- A is the authorise function
- OriginalContractId is contract ID of the original contract

A COMMON variable, R.VERSION (EB.VER.NEXT.VERSION), is updated with the command to be performed. At this point no updates are made to the VERSION table.

Temenos Transact performs any command found in the COMMON variable R.VERSION (EB.VER.NEXT.VERSION).

Final authorisation can then be performed by viewing the original contract displayed, and committing the contract.

If the DISPO VERSION record has the Next Version field set to DISPO.ITEMS,COMMENTS , then once the contract is authorised and the DISPO.ITEMS, COMMENTS window appears ready for the next item.

---


---


## Appendix A: Glossary of T24 Applications & Fields


This glossary lists all T24/Transact application names and field names referenced throughout this document, with descriptions where available.


### Applications


| Application | Description |
|------------|-------------|
| `ACCOUNT` | T24 application: ACCOUNT |
| `EB.DES.PARAMETER` | T24 application: EB.DES.PARAMETER |
| `FUNDS.TRANSFER` | T24 application: FUNDS.TRANSFER |
| `FUNDS.TRANSFER$NAU` | T24 application: FUNDS.TRANSFER$NAU |
| `MS.EVENT` | T24 application: MS.EVENT |
| `MS.EVENT.GROUP` | T24 application: MS.EVENT.GROUP |
| `MS.PARAMETER` | T24 application: MS.PARAMETER |
| `RR.INITIAL.LOAD.PARAMETER` | T24 application: RR.INITIAL.LOAD.PARAMETER |
| `RR.PARAM` | T24 application: RR.PARAM |
| `SPF` | T24 application: SPF |
| `STMT.ENTRY` | T24 application: STMT.ENTRY |
| `TSA.SERVICE` | T24 application: TSA.SERVICE |


### Fields Referenced


| Field | Field | Field |
|-------|-------|-------|
| `Allowed Topic Names` | `Application` | `Attribute Type` |
| `Attribute Value` | `AttributeValue` | `Batch Holiday` |
| `Branch Holiday` | `Company Group` | `Data Stream` |
| `Event Group` | `Global Process` | `Ilp required` |
| `Local Routine` | `Official Holiday` | `Read Api` |
| `Read Api Info` | `Record Id` | `Record Status` |
| `Relative Time` | `Service Status` | `Topic Names` |


---


## Appendix B: Consolidated Field Reference


This appendix consolidates all field description tables from across the documentation, grouped by sub-module. This provides a single reference for all field definitions.


### Infrastructure - EB (EB)


**Dynamic-applications**

| Field type | Calculation |
|---|---|
| Single valued | You can calculate the value of a single valued field using: The other single valued fields The fixed values For example, Field8 |
| Multivalued | You can calculate the value of a multivalued field using: The other multi-values within the same multivalued set The single valued fields The fixed values For example, Field6 |
| Subvalued | You can calculate the value of a subvalued field using: The other sub-values within the same subvalued set The other multi-values within the same multivalued set The single valued fields The fixed values For example, Field3 |

**Component Framework**

| Parameter Name | Type | Description | Direction | Format |
|---|---|---|---|---|
| metaDataXML | MetaDataXML | Indicates the metadata XML for all available Temenos Transact services | OUT | For example, ServicesMetaData.xsd |

**Component Framework**

| Parameter Name | Type | Description | Direction | Format |
|---|---|---|---|---|
| serviceName | String | Indicates the Temenos Transact service name | IN | For example, Customer |
| metaDataXML | MetaDataXML | Indicates the metadata XML for the selected Temenos Transact services | OUT | For example, ServicesMetaData.xsd |

**Component Framework**

| Parameter Name | Type | Description | Direction | Format |
|---|---|---|---|---|
| serviceName | String | Indicates the Temenos Transact service name | IN | For example, Customer |
| metaDataXML | MetaDataXML | Indicates the operations metadata XML for the selected Temenos Transact service | OUT | For example, OperationsMetaData.xsd |

**Component Framework**

| Parameter Name | Type | Description | Direction | Format |
|---|---|---|---|---|
| serviceName | String | Indicates the Temenos Transact service name. | IN | For example, Customer |
| operationName | String | Indicates the service operation name. | IN | For example, getLanguage |
| metaDataXML | MetaDataXML | Indicates the metadata XML of a single operation present under the selected Temenos Transact service. | OUT | For example, OperationsMetaData.xsd |

**Component Framework**

| Parameter Name | Type | Description | Direction | Format |
|---|---|---|---|---|
| serviceName | String | Indicates the Temenos Transact service name | IN | For example, Customer |
| operationName | String | Indicates the service operation name | IN | For example, getLanguage |
| metaDataXML | MetaDataXML | Indicates the metadata XML of all the parameters available under the selected Temenos Transact service operation | OUT | For example, ParametersMetaData.xsd |

**Component Framework**

| Parameter Name | Type | Description | Direction | Format |
|---|---|---|---|---|
| serviceName | String | Indicates the Temenos Transact service name | IN | For example, Customer |
| operationName | String | Indicates the service operation name | IN | For example, getLanguage |
| parameterName | String | Indicates the parameter name | IN | For example, customerKey |
| metaDataXML | MetaDataXML | Indicates the metadata XML of a single parameter available under the selected Temenos Transact service operation | OUT | For example, ParametersMetaData.xsd |

**Component Framework**

| Parameter Name | Type | Description | Direction | Format |
|---|---|---|---|---|
| serviceName | String | Indicates the Temenos Transact service name | IN | For example, Customer |
| customizedTypeName | String | Indicates the service operation name | IN | For example, Language |
| metaDataXML | MetaDataXML | Indicates the metadata XML of a customizedType available in the selected Temenos Transact service. | OUT | For example, CustomizedTypeMetaData.xsd |

**Component Framework**

| Parameter Name | Type | Description | Direction | Format |
|---|---|---|---|---|
| serviceName | String | Indicates the Temenos Transact service name | IN | For example, Customer |
| exists | Boolean | Indicates the exists | OUT | For example, 0 or 1 |

**Component Framework**

| Parameter Name | Type | Description | Direction | Format |
|---|---|---|---|---|
| serviceName | String | Indicates the Temenos Transact service name | IN | For example, Customer |
| operationName | String | Indicates the service operation name | IN | For example, getLanguage |
| exists | boolean | Indicates the exists | OUT | For example, 0 or 1 |

**Component Framework**

| Parameter Name | Type | Description | Direction | Format |
|---|---|---|---|---|
| serviceName | String | Indicates the Temenos Transact service name | IN | For example, Customer |
| operationName | String | Indicates the service operation name | IN | For example, getLanguage |
| parameterName | String | Indicates the operation parameter name | IN | For example, customerKey |
| exists | Boolean | Indicates the exists | OUT | For example, 0 or 1 |

**Component Framework**

| Parameter Name | Type | Description | Direction | Format |
|---|---|---|---|---|
| serviceName | String | Indicates the Temenos Transact service name | IN | For example, Customer |
| customizedTypeName | String | Indicates the service customised type name | IN | For example, Language |
| exists | boolean | Indicates the exists | OUT | For example, 0 or 1 |

**Document Management**

| Field | Description |
|---|---|
| ID | Indicates the ID of this application. The ID format is customer ID.* application mnemonic * transaction ID * document type ID , in which, First part - ID of the customer for whom the document is tracked Second part - Mnemonic defined for an application Third part - ID of the record for which the document is tracked Fourth part - ID of the document type |
| Reference No | Indicates the reference for the document, if any |
| Begin Date | Indicates the date from which the document is tracked in Temenos Transact |
| Status | Indicates the status of the document. |
| Status Date | Indicates the date from which the status applies to the document |
| XX LL Stat Details | Indicates the remarks on the status of the document, if any |
| Sig Date | Indicates the date on which the document is signed |
| End Date | Indicates the expiry date of the document |
| Doc Sequence | Indicates the sequence number of a document, to distinguish the new document obtained on the expiry of an old document |
| Last Upd Date | Indicates the date on which the record was last updated |
| Last Upd Appln | Indicates the application from which Temenos Transact updates the document record |
| Appln Txn Ref | Indicates the transaction reference number of the application, from which Temenos Transact updates the document record |
| Update By | Indicates if the record is updated by the user or Temenos Transact |
| Next Status | Indicates the status of the next document |
| XX LL Next Details | Indicates the remarks on the status of the next document, if any |
| Next Eff Date | Indicates the date on which the next valid document becomes effective, for tracking purposes. |
| Next Status Date | Indicates the date from which the specified status ( Next Status field value) applies to the next document. |
| Next Sig Date | Indicates the date on which signature is obtained on the next document |
| Next End Date | Indicates the expiry date of the next document |

**Enquiry**

| Section | Elements | Description |
|---|---|---|
| Selection | File Name | Indicates the main file of the extracted |
|  | Enquiry Title | Indicates the title of the Enquiry appearing on the window caption |
|  | Product | Indicates the product of the Enquiry used when the Enquiry list is generated |
|  | Predefined Selection / Sort | Indicates the default selection and sort criteria applied when Enquiry is run |
|  | Selection Fields | Indicates the fields displayed in the selection panel |
|  | Op (errand) | Indicates the operand applied for predefined default selection |
|  | Mandatory | Indicates if the predefined selection is mandatory |
| Data/Column | Name | Indicates the name of the field to be processed |
|  | Heading | Indicates the field heading. This can be different from the default heading. |
|  | Col(um) | Indicates the column (order number) of the field display |
|  | Operation | Indicates the comparison, logical, arithmetic or other operators applied on field data |
|  | Type | Indicates the type for formatting (date, amount, currency, and so on) |
|  | Mask | Indicates the output length or mask for display (35L, ###, -~, and so on) |
|  | Conversion | Indicates the conversion for manipulating data prior to display |
|  | S/M | Indicates if the instruction must be processed for every multi/sub-value occurrence) |
|  | Break | Indicates if the field is processed during break conditions |
| Drill-down | Enquiry Name | Indicates the Enquiry to be linked |
|  | Selection Criteria | Indicates the selection criteria passed to the linked Enquiry, which may include data from the parent Enquiry |
|  | Label Field | Indicates the field to highlight for drill-down options |
|  | Next Level Disc. | Indicates the text to be displayed for drill-down options on pop-up menus |
| Advanced | Miscellaneous | Indicates the miscellaneous instructions (like specifying field number instead of field name, and so on) |
|  | Report Options | Indicates the report options for spooling purpose |
|  | SMS Settings | Indicates the security conditions at application, field, and Enquiry level |
| Audit |  | Indicates the system generated fields |
| Full View |  | Indicates the full view of all Enquiry fields |

**Enquiry**

| Attribute | Functionality |
|---|---|
| ALLDATA | Forces the retrieval of all data before the Enquiry is displayed. |
| APPLICATION.ENQUIRY | Displays an Enquiry screen in editable mode, which becomes a record for a specific application when committed. Displays a contract screen in case of any errors. Each row in the Enquiry normally becomes a multi-value in the application record. |
| FASTPATH | Allows a user to select various records on an Enquiry and does Authorise, Delete, Verify or Reverse function of all the selected items consecutively in a single click. |
| INCREMENTAL | Indicates that the Enquiry shows all pages from 'page 1' up to the current page. Applicable for browser only. |
| MULTI.DOWNLOAD | Enables merging of multiple PDF documents prior downloading. |
| NO.BREADCRUMBS | Deletes the list of previously viewed Enquiry navigation links from the top of the screen. Used only for drilled-down enquiries. |
| NO.COLUMN.HEADER | Displays Enquiry without a header for the selected column |
| NO.ENQUIRY.FAVOURITE | Disables the access to view favourites function in an Enquiry. |
| NO.MOREOPTIONS | Disables the ’More Options’ function in an Enquiry |
| NO.SELECTION | Hides the selection criteria found at the bottom of browser fields. Applicable for browser only. |
| NO.TOOLBAR | Hides the tool bar at the top of a browser Enquiry. Applicable for browser only. |
| NORMALISE - DESKTOP | Reserved for future use |
| PAGE | Not Available in Browser |
| REALTIME | Not Available in Browser |
| REMOVE | Deletes an entry if pick operation is performed on an Enquiry grid. Applicable for desktop only. |
| SELECTION.ABOVE.DATA | Displays the selection criteria above data. |
| SELECTION.HORIZONTAL | Displays the selection criteria horizontally along screen. |
| SELECTION.SORT.ONLY | Displays selection sort only criteria. |
| SHOWTREE | Displays the first value only when an Enquiry has expanded multi-values for one field. Clicking '+' button displays all the values. |
| SINGLE.BACKGROUND.COLOUR | Displays all Enquiry backgrounds in a single colour. The default colour is white but other colours can be defined in the 'general.css' file by editing the following elements. .colour0 .hidden0 .dispaly_box .columnHeader. .caption element. |
| STATIC.PAGING.TOOL | Places the paging toolbar inside the Enquiry header at the top left of the Enquiry page |
| UNDERLINE.ALL.ROWS | Underlines all data rows in the Enquiry except the header row. The default is colour is black but other colours and thickness of the ruler can be defined in '.enq-underlineAllRow' in the 'general.css' file. |
| UNDERLINE.DRILL.ROW | Underlines all the Enquiry rows with drill-downs. The rows nominated with view and fast path checkboxes are defined as drill rows for this purpose. The default is colour is black but other colours and thickness of the ruler can be defined in '.enq-underlineAllRow' in the 'general.css' file. |
| UNDERLINE.HEADER.ROW | Underlines all the headers in the selected Enquiry record The default is colour is black but other colours and thickness of the ruler can be defined in '.enq-underlineAllRow' in the 'general.css' file. |
| VIEWLARGEICONS | Converts grid Enquiry to display records as large icons as per windows standard. Applicable for desktop only. |
| VIEWLIST - DESKTOP | Converts grid Enquiry to display records in list format as per windows standard. Applicable for desktop only. |
| VIEWSMALLICONS | Converts grid Enquiry to display records as small icons as per windows standard. Applicable for desktop only. |
| ZERORECORDDISPLAY | Indicates the unavailability of records matching the Enquiry selection criteria with a pop up message. If this attribute is active, the message pop up is suppressed and Enquiry is launched blank. Applicable for desktop only. |

**Archiving**

| Field(s) | Description |
|---|---|
| Descriptn.1 , Descriptn.2 , Descriptn.3 and Descriptn.4 | Indicates the four distinct sections in this record |
| Purge Date and Retention Period | System selects the record to be archived, based on the dates specified in either the Purge Date or Retention Period field. The selected records are archived (or deleted). Purge date is automatically calculated from retention period, during runtime. If today's date is 23 May, 2012 and the retention period of three months is specified (03M), the three month period is calculated from the beginning of the current month. Therefore, records dated before 1 February, 2012 (purge date) are archived (or deleted). |
| Archive Data | Indicates whether the selected records need to be archived or deleted, with respect to the value in this field. Y – Archive N or None – Delete |
| Arc Pathname | Specifies the destination location of the $ARC archive files. If this field is blank, the $ARC files are created in the archive directory (BNK.arc). |
| Arc Filename | Indicates the names of all the $ARC files that are created based on the specified type and modulo. If the type and modulo specification are not present, the ARC files inherit these details from the corresponding live files. It is a multi-value field. |
| Company Run In, Time Started, User Id, Date Selected, Stop Requested, Recs Deleted, Recs Processed, Error Msg, Time Ended | Maintain a history of the archives. The system populates these multi-value fields after the contracts are archived. |
| Generic Method | Indicates whether the generic archival process may be executed or not, with respect to your input. Y – Executes generic archival process. This allows archival service (ARC.GENERIC service) to look after all selection and purging of records. FUNDS.TRANSFER , TELLER , STMT.ENTRY.DETAIL and so on are archived through the generic archival process, with respect to the values input in Main File , Field To Check or Filter Routine fields. No or None – Application specific archival routine specified in the Routine field is invoked. |
| Main File | Accepts the file name (for example, FUNDS.TRANSFER$HIS) input that has to be archived. If this field is multi-valued and populated with two or more applications, the date mentioned in Field To Check is applicable to the application specified in the first multi-value field. |
| Field To Check | Indicates the date field in the contract, which is compared with the Purge date for archiving. If this field is blank, the standard Date Time field is used for comparison. In order to archive the history records of the FUNDS.TRANSFER record, use the Processing Date of the contract. |
| Filter Rtn | It is a hook routine to select or ignore a contract for archiving. This field is an alternate to Field To Check field. The IN and OUT parameters of this routine are: IN Parameters Id Contract – Indicates the record key of the contract R Contract – Indicates the entire contract record OUT Parameters Contractarchive Date – Indicates the date against which the purge date set in the ARCHIVE record is compared. In FUNDS.TRANSFER, you may compare debit value and credit value date of the contract and return a final date as the OUT parameter, which is compared with purge date for archival. Skip Flag – Returns ‘1’ as the OUT parameter, which confirms that the current contract need not be archived. Logic to ignore the contract is available in the filter routine and the current contract is skipped from being archived. Two spare parameters for future expansion. |
| Related Files Rtn | It is a hook routine that returns the names of related files that have to be archived along with the main archival record in a dynamic array.The IN and OUT parameters of this routine are: IN Parameters Id Contract – Indicates the record key of the main contract that is ready to be archived R Contract – Indicates the entire contract record OUT Parameters Related Files – Indicates the information of related files to be archived in 'file name, file ID, archival flag separated by @VM' format. If there are multiple related files, each file information is delimited by @FM marker. Upon archiving LOANS.AND.DEPOSITS records, file records to be archived are balanced. So, pass the balances file name, its ID and a ‘Y’ to the Archival flag. Two spare parameters for future expansion. |
| Routine | Indicates a valid multi-threaded routine that is responsible for archiving the set of files specified in the ARCHIVE record. These are application specific routines that should not be changed unless a site specific program is written. For FOREX , the routine is ARC.FOREX. This record routine is responsible to decide the archival logic and perform the archival. Separate ARC.FOREX.LOAD and ARC.FOREX.SELECT routines must be available for opening and selecting all necessary files for archiving. However, it is not necessary to create a separate ARC.FOREX service. It is the responsibility of ARC.GENERIC service to simply invoke ARC.FOREX.LOAD, ARC.FOREX.SELECT, ARC.FOREX routines internally for archiving in the presence of Routine field. |

**Data Events**

| Sub-Tag | Description |
|---|---|
| tableKey | . |
| tableName | Holds the file name (combination of application name and file mnemonics (for example, FBNK, FCO3, and so on)) for which the Data Events are emitted. The tableKey is the identifier of the corresponding table. The dot and dollar characters are replaced with underscore and hash characters respectively in the file name. |
| applicationData | Holds all the fields of the record in Temenos Transact. |

**Data Events**

| Sub-Tag | Description |
|---|---|
| originatingApplication | Indicates the application name used for the transaction. Following are the application names used in the transaction types: Multi-Transaction - Parent application API requests - operationName non-API requests - the application (version) |
| bankingDate | Indicates the current business date in the Temenos Transact |
| transactionType | Indicates the posting type (ONLINE or BATCH mode) of the transaction |
| action | Indicates the actual operation (function) that is invoked for the transaction. Following are the actions in Temenos Transact: INPUT REVERSE APPROVED |
| channelType | Indicates the respective channel name (OFS$SOURCE.ID) that is common for both API and Non-API requests. |
| application | Indicates the actual file name (combination of application name and file mnemonics). The dot and dollar characters are replaced with underscore and hash characters respectively in the file name |
| operation | Indicates the actual operation (WRITE/DELETE) performed on the table |
| requestStatus | Indicates the status of the record in Temenos Transact based on the Record Status field. The following are the values of the field: Unauthorised Reversed Authorised |

**Data Events**

| Sub-Tag | Description |
|---|---|
| key | Indicates the name of the local field which is a valid field in the local table application. |
| values | Indicates the value of the local field that is associated with the key. |

**Standards Restrictions**

| Application Name | New Record | Amendment of Record |
|---|---|---|
| EB.API | Not Allowed | Allowed |
| DFE.PARAMETER | Not Allowed | Not Allowed |
| EB.TABLE.DEFINITION | Allowed only when created through AA.CLASS.DEFINITION. Manual creation is not allowed. | Allowed only when created through AA.CLASS.DEFINITION. Manual amendment is not allowed. |


### Infrastructure - NS (NS)


**Non-Stop Processing**

| Application Name | Business Area |
|---|---|
| AZ.ACCOUNT | ALL IN ONE ACCOUNTS |
| FACILITY | SYNDICATED LOANS |
| FD.FID.ORDER | FIDUCIARIES |
| FD.FIDUCIARY | FIDUCIARIES |
| FOREX | FOREIGN EXCHANGE |
| FRA.DEAL | FWD RATE AGREEMENT |
| LD.LOANS.AND.DEPOSITS | LOANS AND DEPOSITS |
| LD.SCHEDULE.DEFINE | LOANS AND DEPOSITS |
| MG.MORTGAGE | MORTGAGES |
| MG.PAYMENT | MORTGAGES |
| MM.MONEY.MARKET | MONEY MARKET |
| PD.CAPTURE | PAST DUE |
| PD.PAYMENT.DUE | PAST DUE |
| PRE.SYNDICATION.FILE | SYNDICATED LOANS |
| SC.EXE.SEC.ORDERS | SECURITIES |
| SEC.OPEN.ORDER | SECURITIES |
| SEC.TRADE | SECURITIES |
| SECURITY.TRANSFER | SECURITIES |
| SC.SETTLEMENT | SECURITIES |
| SEC.ACC.MASTER | SECURITIES |
| SECURITY.MASTER | SECURITIES |
| SL.BUY.SELL | SYNDICATED LOANS |
| SL.CHARGE | SYNDICATED LOANS |
| SL.FACI.RATES | SYNDICATED LOANS |
| SL.LOANS | SYNDICATED LOANS |
| SL.RATES.PART | SYNDICATED LOANS |
| SL.REPAYMENT.SCHEDULES | SYNDICATED LOANS |
| SL.ROLLOVER | SYNDICATED LOANS |
| SWAP | SWAPS |

**Non-Stop Processing**

| Application Name | Business Area |
|---|---|
| AA.ARRANGEMENT.ACTIVITY | AA LOANS, DEPOSITS and ACCOUNTS |
| AC.LOCKED.EVENTS | ACCOUNTS |
| ACCOUNT | ACCOUNTS |
| ACCOUNT.CLOSURE | ACCOUNTS |
| ACCOUNT.CREDIT.INT | ACCOUNTS |
| ACCOUNT.DEBIT.INT | ACCOUNTS |
| ACCOUNT.DEBIT.LIMIT | ACCOUNTS |
| ACCT.CAPITALISATION | ACCOUNTS |
| ACCOUNT.STATEMENT | ACCOUNTS |
| ACCT.STATEMENT.CHARGE | ACCOUNTS |
| ACCT.INTERIM.CAP | ACCOUNTS |
| BALANCE.REQUIREMENT | BALANCES |
| CURRENCY | CURRENCY |
| CUSTOMER | CUSTOMER |
| CUSTOMER.SECURITY | CUSTOMER |
| DATA.CAPTURE | DATE CAPTURE |
| DEBIT.INT.ADDON | DEBIT INTEREST |
| DE.CUSTOMER.PREFERENCES | DELIVERY |
| ;DE.PRODUCT | DELIVERY |
| ENTITLEMENT | SECURITIES |
| FORWARD.RATES | FORWARD RATE AGREEMENTS |
| FUNDS.TRANSFER | FUNDS TRANSFER |
| GENERAL.CHARGE | CUSTOMER |
| GROUP.CAPITALISATION | CUSTOMER |
| GROUP.CREDIT.INT | CUSTOMER |
| GROUP.DEBIT.INT | CUSTOMER |
| HIGHEST.DEBIT | BALANCES |
| INTEREST.STATEMENT | INTEREST |
| NOTICE.WITHDRAWAL | ACCOUNTS |
| PAYMENT.STOP | CHEQUES |
| PERIODIC.INTEREST | INTEREST |
| STANDING.ORDER | STANDING ORDERS |
| TELLER | TELLER |
| TELLER.ID | TELLER |
| TRANSACTION.CHARGE | ACCOUNTS |
| TURNOVER.CREDIT | ACCOUNTS |
| TURNOVER.DEBIT | ACCOUNTS |


### Infrastructure - OF (OF)


**OFS features**

| Options | Description |
|---|---|
| ID | ID returns the HOLD.CONTROL key that was produced when the report was run. This means that the XML can be extracted asynchronously. |
| XML | XML returns the XML result. |


### Infrastructure - SM (SM)


**ExternalAuthorisation**

| Target | Operator | Value | Description |
|---|---|---|---|
| subject:roleId | equal | CSAgentRole | Executes or targets the Policy if subject:roleId is equal to CSAgentRole . |
| subject:roleId | regexp-match | ADMIN.* | Executes or targets the Policy if subject:roleId starts with ADMIN . Similarly, any regular expression can be used. |
| subject:userId | equal | TOM | Executes or targets the Policy if subject:userId is equal to TOM . |
| subject:userId | regexp-match | .* | Targets the Policy to all the users, since .* regex means everything. |

**Sms**

| DispoOfficer*Operator*DateTimeStamp | Description |
|---|---|
| Dispo Officer | The Officer defined in the DISPO.OFFICER field on USER profile. |
| Operator | The user that performed the update. |
| DateTimeStamp | The date and time the update was made. |

**Sms**

| Officer Code | Officer Description | Disposition Amount | Overdraft Competence | Next Level of Disposition |
|---|---|---|---|---|
| 1100 | Account Office A | 15,000 | 10,000 | 1101 |
| 1101 | Account Officer B | 20,000 | 20,000 | 1105 |
| 1105 | Account Officer C | 999,999,999,999 | 24,000 |  |
| 2400 | Top Management | 0 | 999,999,999,999 |  |


---
