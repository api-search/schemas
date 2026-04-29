---
description: ''
layout: schema
name: Predict
properties_list:
- description: ''
  name: predictionDefinition
  type: string
- description: ''
  name: predictions
  type: array
- description: ''
  name: settings
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-predict-schema.json
slug: salesforce-predict
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"predictionDefinition\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"predictions\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"model\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\",\n                \"example\": \"abc123\"\n              }\n            },\n            \"required\": [\n              \"id\"\n            ]\n          },\n          \"prediction\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"middleValues\": {\n                \"type\": \"array\",\n                \"description\": \"\",\n                \"example\": [],\n                \"items\": {\n                  \"type\": \"string\"\n                }\n       \
  \       },\n              \"total\": {\n                \"type\": \"number\",\n                \"example\": 42\n              }\n            },\n            \"required\": [\n              \"middleValues\",\n              \"total\"\n            ]\n          },\n          \"prescriptions\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"model\",\n          \"prediction\",\n          \"prescriptions\",\n          \"status\"\n        ]\n      }\n    },\n    \"settings\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"maxMiddleValues\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"maxPrescriptions\": {\n          \"type\":\
  \ \"integer\",\n          \"example\": 10\n        },\n        \"prescriptionImpactPercentage\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"maxMiddleValues\",\n        \"maxPrescriptions\",\n        \"prescriptionImpactPercentage\"\n      ]\n    }\n  },\n  \"required\": [\n    \"predictionDefinition\",\n    \"predictions\",\n    \"settings\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Predict\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-predict-schema.json
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
title: Predict
---
