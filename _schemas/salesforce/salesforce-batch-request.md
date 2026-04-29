---
description: ''
layout: schema
name: BatchRequest
properties_list:
- description: ''
  name: method
  type: string
- description: ''
  name: url
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-batch-request-schema.json
slug: salesforce-batch-request
source_filename: salesforce-batch-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"method\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    }\n  },\n  \"required\": [\n    \"method\",\n    \"url\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-batch-request-schema.json
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
title: BatchRequest
---
