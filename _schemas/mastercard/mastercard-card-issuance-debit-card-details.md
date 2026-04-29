---
description: ''
layout: schema
name: DebitCardDetails
properties_list:
- description: Branch Code. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required for **Primary** card issuance to new client. <BR> <BR/> For the following application types, if the value is se
  name: branchCode
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-debit-card-details-schema.json
slug: mastercard-card-issuance-debit-card-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DebitCardDetails\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"branchCode\": {\n      \"type\": \"string\",\n      \"description\": \"Branch Code. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Required for **Primary** card issuance to new client. <BR> <BR/> For the following application types, if the value is sent, then the branch code is changed for the client initiating the request along with the associated Primary, Supplementary and Add-On cards.: <BR/>\\n* Primary Card - Existing Client (New Program) <BR/>\\n* Supplementary Card - Existing Program <BR/> For the following application types, the value in the field should be empty or same as Primary client's branch code. If the branch code is received and does not match with Primary client's branch code, then the request is rejected: <BR/>\\n* Add On for new Client <BR/>\\n* Supplementary Existing Program for\
  \ Corporate Card\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-debit-card-details-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: DebitCardDetails
---
