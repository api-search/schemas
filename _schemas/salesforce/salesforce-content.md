---
description: ''
layout: schema
name: Content
properties_list:
- description: ''
  name: application/json
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-content-schema.json
slug: salesforce-content
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"application/json\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"schema\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"$ref\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n            \"$ref\"\n          ]\n        }\n      },\n      \"required\": [\n        \"schema\"\n      ]\n    }\n  },\n  \"required\": [\n    \"application/json\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Content\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-content-schema.json
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
title: Content
---
