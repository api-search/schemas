---
description: ''
layout: schema
name: InvokeRequest
properties_list:
- description: ''
  name: datasetLinkName
  type: string
- description: ''
  name: conditions
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-invoke-request-schema.json
slug: salesforce-invoke-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"datasetLinkName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"conditions\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"conditionsList\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"fieldName\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                },\n                \"value\": {\n                  \"type\": \"object\",\n                  \"example\": \"example_value\"\n                },\n                \"operator\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n             \
  \   }\n              },\n              \"required\": [\n                \"fieldName\",\n                \"value\",\n                \"operator\"\n              ]\n            }\n          }\n        },\n        \"required\": [\n          \"conditionsList\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"datasetLinkName\",\n    \"conditions\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InvokeRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-invoke-request-schema.json
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
title: InvokeRequest
---
