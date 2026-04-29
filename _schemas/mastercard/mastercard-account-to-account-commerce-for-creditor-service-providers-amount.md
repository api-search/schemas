---
description: ''
layout: schema
name: Amount
properties_list:
- description: ISO 4217 code for Currency.
  name: currency
  type: string
- description: Amount value.
  name: value
  type: number
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-account-to-account-commerce-for-creditor-service-providers-amount-schema.json
slug: mastercard-account-to-account-commerce-for-creditor-service-providers-amount
source_filename: mastercard-account-to-account-commerce-for-creditor-service-providers-amount-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Amount\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 code for Currency.\"\n    },\n    \"value\": {\n      \"type\": \"number\",\n      \"description\": \"Amount value.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-account-to-account-commerce-for-creditor-service-providers-amount-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Amount
---
