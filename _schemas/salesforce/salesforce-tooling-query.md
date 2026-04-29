---
description: ''
layout: schema
name: ToolingQuery
properties_list:
- description: ''
  name: size
  type: integer
- description: ''
  name: totalSize
  type: integer
- description: ''
  name: done
  type: boolean
- description: ''
  name: queryLocator
  type: '[''string'', ''null'']'
- description: ''
  name: entityTypeName
  type: string
- description: ''
  name: records
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-tooling-query-schema.json
slug: salesforce-tooling-query
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"size\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"totalSize\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"done\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"queryLocator\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"entityTypeName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"records\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"attributes\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"url\": {\n                \"type\": \"string\",\n           \
  \     \"example\": \"https://www.example.com\"\n              }\n            },\n            \"required\": [\n              \"type\",\n              \"url\"\n            ]\n          },\n          \"Name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          }\n        },\n        \"required\": [\n          \"attributes\",\n          \"Name\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"size\",\n    \"totalSize\",\n    \"done\",\n    \"queryLocator\",\n    \"entityTypeName\",\n    \"records\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ToolingQuery\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-tooling-query-schema.json
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
title: ToolingQuery
---
