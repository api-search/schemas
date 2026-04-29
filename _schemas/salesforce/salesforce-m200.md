---
description: ''
layout: schema
name: m200
properties_list:
- description: ''
  name: description
  type: string
- description: ''
  name: content
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-m200-schema.json
slug: salesforce-m200
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"A sample description.\"\n    },\n    \"content\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"application/json\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"schema\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"$ref\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                }\n              },\n              \"required\": [\n                \"$ref\"\n              ]\n            }\n          },\n          \"required\": [\n            \"schema\"\n          ]\n        }\n      },\n      \"required\": [\n        \"application/json\"\n      ]\n    }\n  },\n  \"required\": [\n    \"description\",\n    \"content\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"\
  m200\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-m200-schema.json
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
title: m200
---
