---
description: ''
layout: schema
name: Type12
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: doc
  type: string
- description: ''
  name: fields
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-type12-schema.json
slug: salesforce-type12
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"doc\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"type\": {\n            \"type\": \"object\",\n            \"example\": \"example_value\"\n          },\n          \"doc\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"default\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          }\n       \
  \ },\n        \"required\": [\n          \"name\",\n          \"type\"\n        ]\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Type12\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-type12-schema.json
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
title: Type12
---
