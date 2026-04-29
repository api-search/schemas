---
description: ''
layout: schema
name: RequestProductInformationBundledComponentsRequest
properties_list:
- description: ''
  name: productContexts
  type: array
- description: ''
  name: retrievalType
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-request-product-information-bundled-components-request-schema.json
slug: salesforce-request-product-information-bundled-components-request
source_filename: salesforce-request-product-information-bundled-components-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"productContexts\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"product2Id\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          }\n        },\n        \"required\": [\n          \"product2Id\"\n        ]\n      }\n    },\n    \"retrievalType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"productContexts\",\n    \"retrievalType\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RequestProductInformationBundledComponentsRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-request-product-information-bundled-components-request-schema.json
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
title: RequestProductInformationBundledComponentsRequest
---
