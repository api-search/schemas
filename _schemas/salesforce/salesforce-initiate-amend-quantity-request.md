---
description: ''
layout: schema
name: InitiateAmendQuantityRequest
properties_list:
- description: ''
  name: assetIds
  type: object
- description: ''
  name: startDate
  type: string
- description: ''
  name: quantityChange
  type: integer
- description: ''
  name: amendmentOutputType
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-initiate-amend-quantity-request-schema.json
slug: salesforce-initiate-amend-quantity-request
source_filename: salesforce-initiate-amend-quantity-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetIds\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"assetIdArray\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"required\": [\n        \"assetIdArray\"\n      ]\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"quantityChange\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"amendmentOutputType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"assetIds\",\n    \"startDate\",\n    \"quantityChange\",\n    \"amendmentOutputType\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InitiateAmendQuantityRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-initiate-amend-quantity-request-schema.json
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
title: InitiateAmendQuantityRequest
---
