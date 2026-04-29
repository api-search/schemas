---
description: ''
layout: schema
name: Record7
properties_list:
- description: ''
  name: attributes
  type: object
- description: ''
  name: Name
  type: string
- description: ''
  name: Id
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-record7-schema.json
slug: salesforce-record7
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"type\"\n      ]\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"Id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    }\n  },\n  \"required\": [\n    \"attributes\",\n    \"Name\",\n    \"Id\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Record7\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-record7-schema.json
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
title: Record7
---
