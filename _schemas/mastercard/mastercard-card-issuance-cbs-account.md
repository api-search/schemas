---
description: Core Banking System Account Info. Applicable for Debit Cards only
layout: schema
name: CbsAccount
properties_list:
- description: Primary Account number in CBS. <br/> **Conditional Mandatory**<font color='red'>* </font> field - Required while creating new client.
  name: number
  type: string
- description: Unique id/code/reference assigned to the client in CBS.
  name: clientId
  type: string
- description: '"The currency in which the amount is loaded. <br> Values - 3 letter alphabetic currency codes in `ISO 4217`" <br/> **Conditional Mandatory**<font color=''red''>* </font> field - Required while creating '
  name: currency
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-cbs-account-schema.json
slug: mastercard-card-issuance-cbs-account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CbsAccount\",\n  \"type\": \"object\",\n  \"description\": \"Core Banking System Account Info. Applicable for Debit Cards only\",\n  \"properties\": {\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"Primary Account number in CBS. <br/> **Conditional Mandatory**<font color='red'>* </font> field - Required while creating new client.\"\n    },\n    \"clientId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique id/code/reference assigned to the client in CBS.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"\\\"The currency in which the amount is loaded. <br> Values - 3 letter alphabetic currency codes in `ISO 4217`\\\" <br/> **Conditional Mandatory**<font color='red'>* </font> field - Required while creating new client.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-cbs-account-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: CbsAccount
---
