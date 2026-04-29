---
description: ''
layout: schema
name: Info
properties_list:
- description: ''
  name: title
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: version
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-info-schema.json
slug: salesforce-info
source_filename: salesforce-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"A sample description.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"title\",\n    \"description\",\n    \"version\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Info\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-info-schema.json
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
title: Info
---
