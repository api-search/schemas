---
description: ''
layout: schema
name: Status201-Success
properties_list:
- description: ''
  name: aggregationResults
  type: object
- description: ''
  name: executionId
  type: string
- description: ''
  name: outputs
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-status201-success-schema.json
slug: salesforce-status201-success
source_filename: salesforce-status201-success-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"aggregationResults\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"results\": {\n          \"type\": \"object\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"results\"\n      ]\n    },\n    \"executionId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"outputs\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"results\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"output\": {\n                \"type\": \"integer\",\n                \"example\": 10\n              }\n            },\n            \"required\": [\n              \"output\"\n            ]\n          }\n        },\n        \"required\": [\n          \"results\"\n        ]\n      }\n    }\n  },\n\
  \  \"required\": [\n    \"aggregationResults\",\n    \"executionId\",\n    \"outputs\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Status201-Success\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-status201-success-schema.json
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
title: Status201-Success
---
