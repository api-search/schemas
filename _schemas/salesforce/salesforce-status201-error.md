---
description: ''
layout: schema
name: Status201-Error
properties_list:
- description: ''
  name: outputs
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-status201-error-schema.json
slug: salesforce-status201-error
source_filename: salesforce-status201-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"outputs\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"errorCode\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          },\n          \"errorMessage\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"outcomeList\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"outcomeType\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"successStatus\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          }\n        },\n        \"required\": [\n          \"errorCode\"\
  ,\n          \"errorMessage\",\n          \"outcomeList\",\n          \"outcomeType\",\n          \"successStatus\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"outputs\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Status201-Error\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-status201-error-schema.json
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
title: Status201-Error
---
