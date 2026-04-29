---
description: ''
layout: schema
name: Password
properties_list:
- description: ''
  name: tokenUrl
  type: string
- description: ''
  name: scopes
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-password-schema.json
slug: salesforce-password
source_filename: salesforce-password-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"tokenUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"scopes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"api\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"api\"\n      ]\n    }\n  },\n  \"required\": [\n    \"tokenUrl\",\n    \"scopes\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Password\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-password-schema.json
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
title: Password
---
