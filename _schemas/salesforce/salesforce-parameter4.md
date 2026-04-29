---
description: ''
layout: schema
name: Parameter4
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: in
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: required
  type: boolean
- description: ''
  name: schema
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-parameter4-schema.json
slug: salesforce-parameter4
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"in\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"A sample description.\"\n    },\n    \"required\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"schema\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"type\"\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"in\",\n    \"description\",\n    \"required\",\n    \"schema\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Parameter4\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-parameter4-schema.json
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
title: Parameter4
---
