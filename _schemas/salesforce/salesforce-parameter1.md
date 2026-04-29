---
description: ''
layout: schema
name: Parameter1
properties_list:
- description: ''
  name: fieldName
  type: string
- description: ''
  name: isGroupByField
  type: boolean
- description: ''
  name: operator
  type: string
- description: ''
  name: sequence
  type: integer
- description: ''
  name: usage
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-parameter1-schema.json
slug: salesforce-parameter1
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"fieldName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"isGroupByField\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"operator\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"sequence\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"usage\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"fieldName\",\n    \"isGroupByField\",\n    \"usage\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Parameter1\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-parameter1-schema.json
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
title: Parameter1
---
