---
description: ''
layout: schema
name: Metadata9
properties_list:
- description: ''
  name: enrichedFields
  type: array
- description: ''
  name: eventChannel
  type: string
- description: ''
  name: filterExpression
  type: '[''string'', ''null'']'
- description: ''
  name: selectedEntity
  type: string
- description: ''
  name: urls
  type: '[''string'', ''null'']'
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-metadata9-schema.json
slug: salesforce-metadata9
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"enrichedFields\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"eventChannel\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"filterExpression\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"selectedEntity\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"urls\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"https://www.example.com\"\n    }\n  },\n  \"required\": [\n    \"enrichedFields\",\n    \"eventChannel\",\n    \"filterExpression\",\n    \"selectedEntity\",\n    \"urls\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Metadata9\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-metadata9-schema.json
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
title: Metadata9
---
