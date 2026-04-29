---
description: ''
layout: schema
name: RequestProductInformationNoBundlesRequest
properties_list:
- description: ''
  name: productContexts
  type: array
- description: ''
  name: fields
  type: array
- description: ''
  name: retrievalType
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-request-product-information-no-bundles-request-schema.json
slug: salesforce-request-product-information-no-bundles-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"productContexts\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"product2Id\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"productSellingModelId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          }\n        },\n        \"required\": [\n          \"product2Id\"\n        ]\n      }\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"retrievalType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"productContexts\",\n    \"fields\",\n    \"retrievalType\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"RequestProductInformationNoBundlesRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-request-product-information-no-bundles-request-schema.json
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
title: RequestProductInformationNoBundlesRequest
---
