---
description: ''
layout: schema
name: Output4
properties_list:
- description: ''
  name: errorCode
  type: integer
- description: ''
  name: errorMessage
  type: string
- description: ''
  name: outcomeList
  type: array
- description: ''
  name: outcomeType
  type: '[''string'', ''null'']'
- description: ''
  name: successStatus
  type: boolean
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-output4-schema.json
slug: salesforce-output4
source_filename: salesforce-output4-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorCode\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"outcomeList\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"outcomeType\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"successStatus\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"errorCode\",\n    \"errorMessage\",\n    \"outcomeList\",\n    \"outcomeType\",\n    \"successStatus\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Output4\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-output4-schema.json
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
title: Output4
---
