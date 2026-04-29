---
description: A customer account in Amberflo
layout: schema
name: Customer
properties_list:
- description: Creation timestamp in Unix milliseconds
  name: createTime
  type: integer
- description: Last update timestamp in Unix milliseconds
  name: updateTime
  type: integer
- description: Deletion timestamp in Unix milliseconds
  name: deleteTime
  type: integer
- description: Unique customer identifier from your system
  name: customerId
  type: string
- description: Customer display name
  name: customerName
  type: string
- description: Customer contact email
  name: customerEmail
  type: string
- description: Customer description
  name: description
  type: string
- description: Deprecated — use lifecycleStage instead
  name: enabled
  type: boolean
- description: Whether this is a test customer account
  name: test
  type: boolean
- description: Customer lifecycle stage
  name: lifecycleStage
  type: string
- description: Last deactivation timestamp in Unix milliseconds
  name: deactivateTimeStamp
  type: integer
- description: Custom metadata for external system integration
  name: traits
  type: object
- description: ''
  name: address
  type: object
provider_name: Amberflo
provider_slug: amberflo
schema_file: json-schema/billing-customer-schema.json
slug: billing-customer
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/json-schema/billing-customer-schema.json\",\n  \"title\": \"Customer\",\n  \"description\": \"A customer account in Amberflo\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"createTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Creation timestamp in Unix milliseconds\",\n      \"example\": 1718153645993\n    },\n    \"updateTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Last update timestamp in Unix milliseconds\",\n      \"example\": 1718153645993\n    },\n    \"deleteTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Deletion timestamp in Unix milliseconds\",\n      \"example\": 1718153645993\n    },\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Unique customer identifier from your system\",\n      \"example\": \"customer-123456\"\n    },\n    \"customerName\": {\n      \"type\": \"string\",\n      \"description\": \"Customer display name\",\n      \"example\": \"Acme Corp\"\n    },\n    \"customerEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Customer contact email\",\n      \"example\": \"billing@acme.com\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Customer description\",\n      \"example\": \"Enterprise customer account for Acme Corporation\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Deprecated \\u2014 use lifecycleStage instead\",\n      \"deprecated\": true\n    },\n    \"test\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a test customer account\",\n      \"example\": false\n    },\n    \"lifecycleStage\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Customer lifecycle stage\",\n      \"enum\": [\n        \"ONBOARDING\",\n        \"TRAIL\",\n        \"ACTIVE\",\n        \"OFFBOARDED\"\n      ],\n      \"example\": \"ACTIVE\"\n    },\n    \"deactivateTimeStamp\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Last deactivation timestamp in Unix milliseconds\"\n    },\n    \"traits\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Custom metadata for external system integration\"\n    },\n    \"address\": {\n      \"$ref\": \"#/components/schemas/Address\"\n    }\n  },\n  \"required\": [\n    \"customerId\",\n    \"customerName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/json-schema/billing-customer-schema.json
tags:
- Usage-Based Billing
- Metering
- FinOps
- AI Cost Management
- Billing
- Monetization
title: Customer
---
