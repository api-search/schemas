---
description: ''
layout: schema
name: Context
properties_list:
- description: ''
  name: masterContractId
  type: '[''string'', ''null'']'
- description: ''
  name: renewedContracts
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-context-schema.json
slug: salesforce-context
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"masterContractId\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"500123\"\n    },\n    \"renewedContracts\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"attributes\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              }\n            },\n            \"required\": [\n              \"type\"\n            ]\n          },\n          \"Id\": {\n            \"type\": \"string\",\n            \"example\": \"abc123\"\n          }\n        },\n        \"required\": [\n          \"attributes\",\n          \"Id\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"masterContractId\",\n    \"renewedContracts\"\n  ],\n  \"$schema\": \"\
  https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Context\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-context-schema.json
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
title: Context
---
