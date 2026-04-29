---
description: A monetary amount with its currency code
layout: schema
name: Amount
properties_list:
- description: The numeric monetary amount
  name: value
  type: number
- description: ISO 4217 three-letter currency code
  name: currencyCode
  type: string
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-amount-schema.json
slug: sap-concur-expense-amount
source_filename: sap-concur-expense-amount-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Amount\",\n  \"type\": \"object\",\n  \"description\": \"A monetary amount with its currency code\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"number\",\n      \"description\": \"The numeric monetary amount\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 three-letter currency code\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-amount-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: Amount
---
