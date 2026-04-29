---
description: A customer invoice
layout: schema
name: Invoice
properties_list:
- description: Unique invoice identifier
  name: invoiceId
  type: string
- description: Customer identifier
  name: customerId
  type: string
- description: Invoice period start in Unix seconds
  name: startTime
  type: integer
- description: Invoice period end in Unix seconds
  name: endTime
  type: integer
- description: Total invoice amount
  name: totalAmount
  type: number
- description: Invoice currency code
  name: currency
  type: string
- description: Invoice payment status
  name: status
  type: string
provider_name: Amberflo
provider_slug: amberflo
schema_file: json-schema/billing-invoice-schema.json
slug: billing-invoice
source_filename: billing-invoice-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/json-schema/billing-invoice-schema.json\",\n  \"title\": \"Invoice\",\n  \"description\": \"A customer invoice\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"invoiceId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique invoice identifier\",\n      \"example\": \"inv-500123\"\n    },\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"Customer identifier\",\n      \"example\": \"customer-123456\"\n    },\n    \"startTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Invoice period start in Unix seconds\",\n      \"example\": 1718100000\n    },\n    \"endTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Invoice period end in Unix seconds\",\n      \"example\": 1718186400\n    },\n    \"totalAmount\": {\n      \"type\": \"number\",\n      \"description\"\
  : \"Total invoice amount\",\n      \"example\": 99.5\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Invoice currency code\",\n      \"example\": \"USD\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Invoice payment status\",\n      \"enum\": [\n        \"DRAFT\",\n        \"PENDING\",\n        \"PAID\",\n        \"VOID\"\n      ],\n      \"example\": \"PAID\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/json-schema/billing-invoice-schema.json
tags:
- Usage-Based Billing
- Metering
- FinOps
- AI Cost Management
- Billing
- Monetization
title: Invoice
---
