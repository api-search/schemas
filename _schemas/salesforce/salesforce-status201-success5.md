---
description: ''
layout: schema
name: Status201-Success5
properties_list:
- description: ''
  name: errorCode
  type: '[''string'', ''null'']'
- description: ''
  name: errorMessage
  type: '[''string'', ''null'']'
- description: ''
  name: outcomeList
  type: array
- description: ''
  name: outcomeType
  type: string
- description: ''
  name: successStatus
  type: boolean
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-status201-success5-schema.json
slug: salesforce-status201-success5
source_filename: salesforce-status201-success5-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorCode\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"errorMessage\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"outcomeList\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"outcomeType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"successStatus\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"errorCode\",\n    \"errorMessage\",\n    \"outcomeList\",\n    \"outcomeType\",\n    \"successStatus\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Status201-Success5\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-status201-success5-schema.json
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
title: Status201-Success5
---
