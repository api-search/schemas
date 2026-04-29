---
description: A payment method used for an expense
layout: schema
name: PaymentType
properties_list:
- description: The payment type identifier (e.g., CASH, CPAID)
  name: id
  type: string
- description: The localized display name
  name: name
  type: string
- description: The payment type code
  name: code
  type: string
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-payment-type-schema.json
slug: sap-concur-expense-payment-type
source_filename: sap-concur-expense-payment-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PaymentType\",\n  \"type\": \"object\",\n  \"description\": \"A payment method used for an expense\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The payment type identifier (e.g., CASH, CPAID)\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The localized display name\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"The payment type code\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-payment-type-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: PaymentType
---
