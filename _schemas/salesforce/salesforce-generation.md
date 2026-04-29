---
description: ''
layout: schema
name: Generation
properties_list:
- description: ''
  name: parameters
  type: string
- description: ''
  name: responseId
  type: string
- description: ''
  name: text
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-generation-schema.json
slug: salesforce-generation
source_filename: salesforce-generation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"parameters\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"responseId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"parameters\",\n    \"responseId\",\n    \"text\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Generation\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-generation-schema.json
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
title: Generation
---
