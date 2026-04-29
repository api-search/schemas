---
description: ''
layout: schema
name: Content1
properties_list:
- description: ''
  name: application/json
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-content1-schema.json
slug: salesforce-content1
source_filename: salesforce-content1-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"application/json\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"schema\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"$ref\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                }\n              },\n              \"required\": [\n                \"$ref\"\n              ]\n            }\n          },\n          \"required\": [\n            \"type\",\n            \"items\"\n          ]\n        }\n      },\n      \"required\": [\n        \"schema\"\n      ]\n    }\n  },\n  \"required\": [\n    \"application/json\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n \
  \ \"title\": \"Content1\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-content1-schema.json
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
title: Content1
---
