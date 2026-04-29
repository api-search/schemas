---
description: ''
layout: schema
name: ExpressionSetUpdateRequest
properties_list:
- description: ''
  name: apiName
  type: string
- description: ''
  name: contextDefinitions
  type: array
- description: ''
  name: name
  type: string
- description: ''
  name: usageType
  type: string
- description: ''
  name: versions
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-expression-set-update-request-schema.json
slug: salesforce-expression-set-update-request
source_filename: salesforce-expression-set-update-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"contextDefinitions\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"usageType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"versions\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"apiName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"enabled\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"id\": {\n            \"type\": \"string\",\n           \
  \ \"example\": \"abc123\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"showExplExternally\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"startDate\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"steps\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"variables\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"versionNumber\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          }\n        },\n        \"required\": [\n          \"apiName\",\n\
  \          \"enabled\",\n          \"id\",\n          \"name\",\n          \"showExplExternally\",\n          \"startDate\",\n          \"steps\",\n          \"variables\",\n          \"versionNumber\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"apiName\",\n    \"contextDefinitions\",\n    \"name\",\n    \"usageType\",\n    \"versions\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExpressionSetUpdateRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-expression-set-update-request-schema.json
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
title: ExpressionSetUpdateRequest
---
