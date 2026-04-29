---
description: ''
layout: schema
name: Prediction
properties_list:
- description: ''
  name: model
  type: object
- description: ''
  name: prediction
  type: object
- description: ''
  name: prescriptions
  type: array
- description: ''
  name: status
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-prediction-schema.json
slug: salesforce-prediction
source_filename: salesforce-prediction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"model\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        }\n      },\n      \"required\": [\n        \"id\"\n      ]\n    },\n    \"prediction\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"middleValues\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"total\": {\n          \"type\": \"number\",\n          \"example\": 42\n        }\n      },\n      \"required\": [\n        \"middleValues\",\n        \"total\"\n      ]\n    },\n    \"prescriptions\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"\
  example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"model\",\n    \"prediction\",\n    \"prescriptions\",\n    \"status\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Prediction\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-prediction-schema.json
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
title: Prediction
---
