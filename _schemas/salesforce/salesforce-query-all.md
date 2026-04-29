---
description: ''
layout: schema
name: QueryAll
properties_list:
- description: ''
  name: totalSize
  type: integer
- description: ''
  name: done
  type: boolean
- description: ''
  name: records
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-query-all-schema.json
slug: salesforce-query-all
source_filename: salesforce-query-all-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalSize\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"done\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"records\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"attributes\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"url\": {\n                \"type\": \"string\",\n                \"example\": \"https://www.example.com\"\n              }\n            },\n            \"required\": [\n              \"type\",\n              \"url\"\n            ]\n          },\n          \"Name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n    \
  \      }\n        },\n        \"required\": [\n          \"attributes\",\n          \"Name\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"totalSize\",\n    \"done\",\n    \"records\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QueryAll\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-query-all-schema.json
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
title: QueryAll
---
