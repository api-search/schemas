---
description: Currency exchange rate applied to an expense
layout: schema
name: ExchangeRate
properties_list:
- description: The exchange rate multiplier or divisor
  name: value
  type: number
- description: How to apply the rate to convert currencies
  name: operation
  type: string
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-exchange-rate-schema.json
slug: sap-concur-expense-exchange-rate
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExchangeRate\",\n  \"type\": \"object\",\n  \"description\": \"Currency exchange rate applied to an expense\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"number\",\n      \"description\": \"The exchange rate multiplier or divisor\"\n    },\n    \"operation\": {\n      \"type\": \"string\",\n      \"description\": \"How to apply the rate to convert currencies\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-exchange-rate-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: ExchangeRate
---
