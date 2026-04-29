---
description: ''
layout: schema
name: Record3
properties_list:
- description: ''
  name: attributes
  type: object
- description: ''
  name: lastname
  type: string
- description: ''
  name: Title
  type: string
- description: ''
  name: email
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-record3-schema.json
slug: salesforce-record3
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"referenceId\": {\n          \"type\": \"string\",\n          \"example\": \"500123\"\n        }\n      },\n      \"required\": [\n        \"type\",\n        \"referenceId\"\n      ]\n    },\n    \"lastname\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"Title\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"example\": \"user@example.com\"\n    }\n  },\n  \"required\": [\n    \"attributes\",\n    \"lastname\",\n    \"email\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Record3\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-record3-schema.json
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
title: Record3
---
