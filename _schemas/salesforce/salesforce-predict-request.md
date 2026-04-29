---
description: ''
layout: schema
name: PredictRequest
properties_list:
- description: ''
  name: predictionDefinition
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: columnNames
  type: array
- description: ''
  name: rows
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-predict-request-schema.json
slug: salesforce-predict-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"predictionDefinition\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"columnNames\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"rows\": {\n      \"type\": \"array\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"predictionDefinition\",\n    \"type\",\n    \"columnNames\",\n    \"rows\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PredictRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-predict-request-schema.json
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
title: PredictRequest
---
