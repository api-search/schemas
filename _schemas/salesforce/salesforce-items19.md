---
description: ''
layout: schema
name: Items19
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: properties
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-items19-schema.json
slug: salesforce-items19
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"extendedErrorCode\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n            \"type\"\n          ]\n        }\n      },\n      \"required\": [\n        \"extendedErrorCode\"\n      ]\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"properties\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Items19\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-items19-schema.json
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
title: Items19
---
