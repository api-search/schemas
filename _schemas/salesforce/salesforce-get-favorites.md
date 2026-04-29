---
description: ''
layout: schema
name: GetFavorites
properties_list:
- description: ''
  name: favorites
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-get-favorites-schema.json
slug: salesforce-get-favorites
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"favorites\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"accessCount\": {\n            \"type\": \"integer\",\n            \"example\": 42\n          },\n          \"iconColor\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"iconUrl\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"abc123\"\n          },\n          \"lastAccessDate\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"objectType\": {\n            \"type\"\
  : \"string\",\n            \"example\": \"example_value\"\n          },\n          \"sortOrder\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          },\n          \"subtitle\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"target\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"targetType\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"accessCount\",\n          \"iconColor\",\n          \"iconUrl\",\n          \"id\",\n          \"lastAccessDate\",\n          \"name\",\n          \"objectType\",\n          \"sortOrder\",\n          \"subtitle\",\n          \"target\",\n          \"targetType\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"favorites\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"\
  title\": \"GetFavorites\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-get-favorites-schema.json
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
title: GetFavorites
---
