
# Temenos Transact — User_Agents Module Documentation


> **Comprehensive User Guide**
> Generated: 13 April 2026
> Content: Configuration | Reference | Field Descriptions | Glossary


## Table of Contents

  - [User_Agents Module Overview](#user_agents-module-overview)
    - [Sub-Module Summary](#sub-module-summary)
    - [How to Use This Guide](#how-to-use-this-guide)
  - [Chapter 1: User_Agents - UserAgents](#chapter-1-user_agents---useragents)
    - [Features in User_Agents - UserAgents](#features-in-user_agents---useragents)
    - [1.1  CDM](#11-cdm)
    - [1.2  LiqOff](#12-liqoff)
    - [1.3  SettlementOfficer](#13-settlementofficer)
  - [Appendix A: Glossary of T24 Applications & Fields](#appendix-a-glossary-of-t24-applications-fields)
  - [Appendix B: Consolidated Field Reference](#appendix-b-consolidated-field-reference)

---


## User_Agents Module Overview


This document provides comprehensive documentation for the **User_Agents** module of Temenos Transact. It covers **1 sub-modules** with a total of **3 feature areas**.


### Sub-Module Summary


| # | Sub-Module | Code | Features | Description |
|---|-----------|------|----------|-------------|
| 1 | **User_Agents - UserAgents** | `UserAgents` | 3 | User_Agents - UserAgents module of Temenos Transact |


### How to Use This Guide


Each feature in this document is organized into the following sections:

- 📖 **Introduction** — Overview and purpose of the feature
- ⚙️ **Configuration** — How to set up and configure the feature
- 🔧 **Working With** — Operational usage and field descriptions
- 📋 **Tasks** — Step-by-step procedures
- 📊 **Outputs** — Reports, enquiries, and generated outputs

Each feature includes a **Quick Reference Card** at the top with application names, key fields, prerequisites, and a summary. Appendices provide a full glossary, consolidated field tables, and end-to-end use-case scenarios.

---


## Chapter 1: User_Agents - UserAgents


User_Agents - UserAgents module of Temenos Transact


### Features in User_Agents - UserAgents


| # | Feature | Sections |
|---|---------|----------|
| 1.1 | CDM | Intro |
| 1.2 | LiqOff | Intro, Confi |
| 1.3 | SettlementOfficer | Intro, Confi |


### 1.1  CDM


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Customer Information Manager for CDM (Customer Data Management) user agent is dedicated for branch use, within the financial institution. It provides the ability to store and view the contact history for a customer. Besides these, it helps the branch users to manage and record the content of a c...*
> 
> **Sections:** 📖 Introduction


#### 📖 Introduction

The Customer Information Manager for CDM (Customer Data Management) user agent is dedicated for branch use, within the financial institution. It provides the ability to store and view the contact history for a customer. Besides these, it helps the branch users to manage and record the content of a contact the bank establishes with a customer. This allows the agents to reduce the time spent on unnecessary tasks, navigating around multiple systems and enables them to spend more time listening to the customer and therefore improve customer experience.

With the use of the Customer Information Manager for CDM user agent, the user is able to quickly understand the following:

- Who the customer is.
- What is their current relationship with the bank.
- If there are any issues or have been any complaints that need immediate attention.
- If there are any opportunities to upsell new products to the customer.
- Access a loan arrangement from the customer's profile.
- Request a payoff for the denoted loan.

The Customer Information Manager for CDM user agent grants a streamlined customer search flow, a decluttered first view of the single customer view, providing a top-level overview of the customer’s profile, with the opportunity to dive deeper where relevant. The users will have a clearer and more considered hierarchy to all onscreen data.

---


### 1.2  LiqOff


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Liquidity Officer (LQUSER1) User Agent, developed using the Temenos Explorer framework, is designed to address the needs of international treasury operations in a modern banking environment.*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration


#### 📖 Introduction

The Liquidity Officer (LQUSER1) User Agent, developed using the Temenos Explorer framework, is designed to address the needs of international treasury operations in a modern banking environment.

Intraday liquidity management is a key element of a bank’s overall Liquidity management framework, designed to efficiently control and optimize the available funds throughout the trading day. Its primary goal is to ensure that the bank has adequate liquidity to meet short-term payment obligations and respond to unforeseen financial demands. This is essential for maintaining financial stability, regulatory compliance, and seamless transaction processing.

Regulatory frameworks such as the Basel Committee on Banking Supervision (BCBS), require banks to implement monitoring tools for intraday liquidity management. These tools provide quantitative measures and controls, including compliance with obligations such as:

- Monitoring the real-time cash position across accounts and currencies to meet payment and settlement obligations.
- Managing and reporting the liquidity position across branches, business units, and legal entities.
- Building historical information to support intraday liquidity modeling, liquidity forecasting, and liquidity risk analytics.

This monitoring tool ensures that the bank maintains sufficient liquidity positions for nostro accounts, enabling seamless customer services while minimising the costs, mitigating mitigating risks, and adhering to regulatory requirements. It enables the liquidity officer to eliminate unnecessary tasks, thereby reducing the time spent navigating multiple systems, allowing them to focus on strategic operations. Based on a combination of forecasts and external reporting, this tool provides enhanced intra-day liquidity management which helps to reduce the required liquidity buffer.

Using the Liquidity Officer User Agent, the user can:

- Consolidate the liquidity management across nostro accounts.
- Monitor the expected and actual cash positions of nostro accounts.
- Forecasting the liquidity position across nostro accounts.
- Set up rules to monitor intraday liquidity limits.
- Generate alerts and notifications based on the breach of limits or rules.
- Enable data availability of regulatory reporting.
- Reduce manual tasks and elevate accuracy.

Read the Temenos Explorer User Guide for more information on the usage of the general functions of Temenos Explorer.


#### ⚙️ Configuration

This section explains the configurations required for the Liquidity Officer UA.


##### Prerequisites

Following are the prerequisites for configuring the Liquidity Officer UA:

- Configure Transact Explorer with Keycloak.
- Deploy the following files in the jboss environment: LiquidityUA.war transact-explorer-wa.war tb-server.war irf-provider-container.war


##### Configuring Liquidity Officer User Agent

Following are the initial configurations required for the Liquidity Officer UA:

1. Execute the below Keycloak configuration in the TA_Config.js file ( ……\ \TemenosExplorer-SNAPSHOT\public\TA_config.js )
2. For the Liquidity Officer UA to work with APIs, deploy the irf-provider-container.war file and set PROVIDER_API_ROOT to have the corresponding IP in the TA_Config.js file as shown below.
3. Save the changes to TA_config.js within the WAR archive.
4. Define the following user information to work with Temenos Explorer-based Liquidity UA and Transact. Definition Keycloak Transact Liquidity Officer LQUSER1 Liquidity Officer (to be created manually using the sign-on name as LQUSER1)

Read Keycloak User Guide for more information on the Keycloak installation and configuration.

> **⚠️ Note:** Banks can create different users, however, for the single sign-on feature to work, the Keycloak username and Transact sign-on name must match. Read the User Profile and Security section for more information on user management in Transact.


##### Customisation

Following are the controls used for customising the browser:

- Preference Settings: Click and select the preferred settings for a browser session.
- Full View: Click to view the respective details in full screen. The below screenshot shows the full-screen view of the Intraday Position chart.
- Refresh Button: Click to refresh the values and update the screen. The below screenshot shows the refreshed view of the Projections screen.
- Visible Columns: The Visible Columns filter can be used to customise the columns to be displayed in the table.
- Filterable Columns: The Filterable Columns filter can be used to enter any text (for example, 24 in the below screenshot) and choose the columns in which the text needs to be searched. The corresponding records are displayed based on the selected columns.

---


### 1.3  SettlementOfficer


> **📇 Quick Reference Card**
> 
> **Purpose:** *The Settlement Officer User Agent is a plug-in that is part of Temenos Explorer. It allows the settlement officer to manage pending settlements. It provides detailed insights into outstanding settlements, grouped by various statuses and reasons which are listed below:*
> 
> **Sections:** 📖 Introduction | ⚙️ Configuration


#### 📖 Introduction

The Settlement Officer User Agent is a plug-in that is part of Temenos Explorer. It allows the settlement officer to manage pending settlements. It provides detailed insights into outstanding settlements, grouped by various statuses and reasons which are listed below:

- Settlements by status – Displays an overview of the count and value of outstanding settlements for each prioritised status such as matched, unmatched, pending, rejected, and so on. It displays the list of transactions based on status for the Settlement Officer to address.
- Settlements requiring immediate attention – Displays the count of outstanding settlements requiring immediate attention of the settlement officer. For example, unmatched, failing, repair, rejected, failed and cancellations initiated by the counterparty.
- Standard Settlement Instruction – Displays the Standard Settlement Instruction (SSI) details of the broker or counterparty involved in the securities transaction.
- Allegements – Displays the details of allegements received from the custodian with their corresponding status.
- Split Settlements – Displays settlements that are part of unilateral and bilateral split settlements. Split settlement involves requesting the replacement of an existing instruction with two or more instructions. It also allows the settlement officer to act on the settlement using single-sign on through Transact Explorer that is embedded into the User Agent.

Read the Temenos Explorer User Guide for more information on the usage of the general functions of Temenos Explorer.


#### ⚙️ Configuration

As a prerequisite, configure Transact Explorer with Keycloak. The initial configurations required for the Settlement Officer User Agent (UA) are:


##### Configuring Keycloak Instance with Temenos Explorer

To use the Settlement Officer UA plug-in, an authentication system must be integrated with Temenos Explorer. To integrate Keycloak with Temenos Explorer, update the config files as shown below:

Configure Keycloak in the TA_Config.js file in (……\ \TemenosExplorer-SNAPSHOT\public\TA_config.js) as shown below.

For the Settlement Officer UA war to work with the APIs,

1. Deploy irf-provider-container.war .
2. Set PROVIDER_API_ROOT in TA_config.js to have the corresponding IP for irf-provider-container.war .
3. To effect this change, modify the below line in TA_config.js and specify the IP address:top["PROVIDER_API_ROOT"] = "http:// :9089";
4. Save the changes to TA_config.js within the WAR archive.

> **⚠️ Note:** Any setting configured with ‘localhost’ in the URL can be replaced with the respective IP address to access the UA from various systems.

| Definition | Keycloak | Transact |
|---|---|---|
| Settlement Officer | SETT.OFF | Settlement Officer (to be created manually using the sign-on name as SETT.OFF) |
| Settlement Manager | SETT.MNGR | Settlement Manager (to be created manually using the sign-on name as SETT.MNGR) |

Read User Profile and Security for more information on user management in Transact.

The following are some controls used for customisation of the browser.

Preference Settings

Click to select the preferred settings for a browser session.

Full View

Click to view the details in the full screen. The following screen depicts the view of the Reason-wise chart in full-screen.

Visible Columns and Filterable Columns

- Visible Columns – The user can customise the display of fields. Only the selected columns appear in the table.
- Filterable Columns - The user can filter the display by entering any text (for example, ADEA in the screen below) and choose the columns in which this text needs to be searched. Based on the selected columns, the corresponding records are displayed.

---


---


## Appendix A: Glossary of T24 Applications & Fields


This glossary lists all T24/Transact application names and field names referenced throughout this document, with descriptions where available.


---


## Appendix B: Consolidated Field Reference


This appendix consolidates all field description tables from across the documentation, grouped by sub-module. This provides a single reference for all field definitions.

*No field description tables were found in the source documentation.*


---
