---
description: ''
layout: schema
name: CompositeBatchRequest
properties_list:
- description: ''
  name: haltOnError
  type: boolean
- description: ''
  name: batchRequests
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-composite-batch-request-schema.json
slug: salesforce-composite-batch-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"haltOnError\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"batchRequests\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"method\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"url\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com\"\n          }\n        },\n        \"required\": [\n          \"method\",\n          \"url\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"haltOnError\",\n    \"batchRequests\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompositeBatchRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-composite-batch-request-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: CompositeBatchRequest
---
