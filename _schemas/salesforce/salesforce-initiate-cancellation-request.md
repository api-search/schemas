---
description: ''
layout: schema
name: InitiateCancellationRequest
properties_list:
- description: ''
  name: assetIds
  type: object
- description: ''
  name: cancellationDate
  type: string
- description: ''
  name: cancellationOutputType
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-initiate-cancellation-request-schema.json
slug: salesforce-initiate-cancellation-request
source_filename: salesforce-initiate-cancellation-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetIds\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"assetIdArray\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"required\": [\n        \"assetIdArray\"\n      ]\n    },\n    \"cancellationDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"cancellationOutputType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"assetIds\",\n    \"cancellationDate\",\n    \"cancellationOutputType\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InitiateCancellationRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-initiate-cancellation-request-schema.json
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
title: InitiateCancellationRequest
---
