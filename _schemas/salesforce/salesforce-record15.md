---
description: ''
layout: schema
name: Record15
properties_list:
- description: ''
  name: attributes
  type: object
- description: ''
  name: Name
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-record15-schema.json
slug: salesforce-record15
source_filename: salesforce-record15-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        }\n      },\n      \"required\": [\n        \"type\",\n        \"url\"\n      ]\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    }\n  },\n  \"required\": [\n    \"attributes\",\n    \"Name\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Record15\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-record15-schema.json
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
title: Record15
---
