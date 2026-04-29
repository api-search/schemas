---
description: ''
layout: schema
name: ToolingSearch
properties_list:
- description: ''
  name: searchRecords
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-tooling-search-schema.json
slug: salesforce-tooling-search
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"searchRecords\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"attributes\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"url\": {\n                \"type\": \"string\",\n                \"example\": \"https://www.example.com\"\n              }\n            },\n            \"required\": [\n              \"type\",\n              \"url\"\n            ]\n          },\n          \"Name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          }\n        },\n        \"required\": [\n          \"attributes\",\n          \"Name\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"searchRecords\"\
  \n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ToolingSearch\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-tooling-search-schema.json
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
title: ToolingSearch
---
