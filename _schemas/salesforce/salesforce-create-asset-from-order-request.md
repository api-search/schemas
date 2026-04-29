---
description: ''
layout: schema
name: CreateAssetFromOrderRequest
properties_list:
- description: ''
  name: inputs
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-create-asset-from-order-request-schema.json
slug: salesforce-create-asset-from-order-request
source_filename: salesforce-create-asset-from-order-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"orderId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          }\n        },\n        \"required\": [\n          \"orderId\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"inputs\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateAssetFromOrderRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-create-asset-from-order-request-schema.json
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
title: CreateAssetFromOrderRequest
---
