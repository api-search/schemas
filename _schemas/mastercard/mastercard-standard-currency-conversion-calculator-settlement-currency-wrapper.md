---
description: ''
layout: schema
name: SettlementCurrencyWrapper
properties_list:
- description: The name of the service being requested.
  name: name
  type: string
- description: The description of the API being called.
  name: description
  type: string
- description: The date and time the API is being called in GMT.
  name: date
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-standard-currency-conversion-calculator-settlement-currency-wrapper-schema.json
slug: mastercard-standard-currency-conversion-calculator-settlement-currency-wrapper
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SettlementCurrencyWrapper\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the service being requested.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the API being called.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the API is being called in GMT.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-standard-currency-conversion-calculator-settlement-currency-wrapper-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: SettlementCurrencyWrapper
---
