---
description: ''
layout: schema
name: InitiateRenewalRequest
properties_list:
- description: ''
  name: assetIds
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-initiate-renewal-request-schema.json
slug: salesforce-initiate-renewal-request
source_filename: salesforce-initiate-renewal-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetIds\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"assetIdArray\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"required\": [\n        \"assetIdArray\"\n      ]\n    }\n  },\n  \"required\": [\n    \"assetIds\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InitiateRenewalRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-initiate-renewal-request-schema.json
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
title: InitiateRenewalRequest
---
