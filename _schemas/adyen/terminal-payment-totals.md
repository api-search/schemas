---
description: Totals of the payment transaction during the reconciliation period.
layout: schema
name: PaymentTotals
properties_list:
- description: ''
  name: TransactionType
  type: object
- description: Number of processed transaction during the period.
  name: TransactionCount
  type: integer
- description: Sum of amount of processed transaction during the period.
  name: TransactionAmount
  type: number
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-payment-totals-schema.json
slug: terminal-payment-totals
source_filename: terminal-payment-totals-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-payment-totals-schema.json\",\n  \"title\": \"PaymentTotals\",\n  \"description\": \"Totals of the payment transaction during the reconciliation period.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TransactionType\": {\n      \"$ref\": \"#/components/schemas/TransactionType\"\n    },\n    \"TransactionCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of processed transaction during the period.\"\n    },\n    \"TransactionAmount\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0,\n      \"description\": \"Sum of amount of processed transaction during the period.\"\n    }\n  },\n  \"required\": [\n    \"TransactionType\",\n    \"TransactionCount\",\n    \"TransactionAmount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-payment-totals-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentTotals
---
