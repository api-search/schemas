---
description: ''
layout: schema
name: Record6
properties_list:
- description: ''
  name: attributes
  type: object
- description: ''
  name: id
  type: string
- description: ''
  name: NumberOfEmployees
  type: integer
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-record6-schema.json
slug: salesforce-record6
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"type\"\n      ]\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"NumberOfEmployees\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    }\n  },\n  \"required\": [\n    \"attributes\",\n    \"id\",\n    \"NumberOfEmployees\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Record6\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-record6-schema.json
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
title: Record6
---
