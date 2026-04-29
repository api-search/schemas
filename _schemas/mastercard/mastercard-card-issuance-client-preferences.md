---
description: ''
layout: schema
name: ClientPreferences
properties_list:
- description: Indicates whether registered in 'DNCR' (Do Not Call Register) or not. Default false. <BR/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.
  name: registerForDNCR
  type: boolean
- description: Indicates whether registered for sms alert notification facility or not. Default false. <BR/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.
  name: smsAlert
  type: boolean
- description: Indicates whether registered for email alert notification facility or not. Default false. <BR/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.
  name: emailAlert
  type: boolean
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-client-preferences-schema.json
slug: mastercard-card-issuance-client-preferences
source_filename: mastercard-card-issuance-client-preferences-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClientPreferences\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"registerForDNCR\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether registered in 'DNCR' (Do Not Call Register) or not. Default false. <BR/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.\"\n    },\n    \"smsAlert\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether registered for sms alert notification facility or not. Default false. <BR/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.\"\n    },\n    \"emailAlert\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether registered for email alert notification facility or not. Default false. <BR/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-client-preferences-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: ClientPreferences
---
