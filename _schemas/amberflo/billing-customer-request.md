---
description: Request body for creating or updating a customer
layout: schema
name: CustomerRequest
properties_list:
- description: Unique customer identifier
  name: customerId
  type: string
- description: Customer display name
  name: customerName
  type: string
- description: Customer email address
  name: customerEmail
  type: string
- description: Customer description
  name: description
  type: string
- description: Marks customer as test
  name: test
  type: boolean
- description: Lifecycle stage
  name: lifecycleStage
  type: string
- description: Custom metadata
  name: traits
  type: object
- description: ''
  name: address
  type: object
provider_name: Amberflo
provider_slug: amberflo
schema_file: json-schema/billing-customer-request-schema.json
slug: billing-customer-request
source_filename: billing-customer-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/json-schema/billing-customer-request-schema.json\",\n  \"title\": \"CustomerRequest\",\n  \"description\": \"Request body for creating or updating a customer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique customer identifier\",\n      \"example\": \"customer-123456\"\n    },\n    \"customerName\": {\n      \"type\": \"string\",\n      \"description\": \"Customer display name\",\n      \"example\": \"Acme Corp\"\n    },\n    \"customerEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Customer email address\",\n      \"example\": \"billing@acme.com\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Customer description\"\n    },\n    \"test\": {\n      \"\
  type\": \"boolean\",\n      \"description\": \"Marks customer as test\",\n      \"example\": false\n    },\n    \"lifecycleStage\": {\n      \"type\": \"string\",\n      \"description\": \"Lifecycle stage\",\n      \"enum\": [\n        \"ONBOARDING\",\n        \"TRAIL\",\n        \"ACTIVE\",\n        \"OFFBOARDED\"\n      ],\n      \"example\": \"ACTIVE\"\n    },\n    \"traits\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Custom metadata\"\n    },\n    \"address\": {\n      \"$ref\": \"#/components/schemas/Address\"\n    }\n  },\n  \"required\": [\n    \"customerId\",\n    \"customerName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/json-schema/billing-customer-request-schema.json
tags:
- Usage-Based Billing
- Metering
- FinOps
- AI Cost Management
- Billing
- Monetization
title: CustomerRequest
---
