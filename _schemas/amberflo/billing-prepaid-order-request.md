---
description: Request body for creating a prepaid order
layout: schema
name: PrepaidOrderRequest
properties_list:
- description: Customer identifier
  name: customerId
  type: string
- description: Prepaid credit amount
  name: amount
  type: number
- description: Currency code
  name: currency
  type: string
- description: Expiration timestamp in Unix milliseconds
  name: expirationTime
  type: integer
provider_name: Amberflo
provider_slug: amberflo
schema_file: json-schema/billing-prepaid-order-request-schema.json
slug: billing-prepaid-order-request
source_filename: billing-prepaid-order-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/json-schema/billing-prepaid-order-request-schema.json\",\n  \"title\": \"PrepaidOrderRequest\",\n  \"description\": \"Request body for creating a prepaid order\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"Customer identifier\",\n      \"example\": \"customer-123456\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"Prepaid credit amount\",\n      \"example\": 500.0\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code\",\n      \"example\": \"USD\"\n    },\n    \"expirationTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Expiration timestamp in Unix milliseconds\",\n      \"example\": 1749686400000\n    }\n  },\n  \"required\"\
  : [\n    \"customerId\",\n    \"amount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/json-schema/billing-prepaid-order-request-schema.json
tags:
- Usage-Based Billing
- Metering
- FinOps
- AI Cost Management
- Billing
- Monetization
title: PrepaidOrderRequest
---
