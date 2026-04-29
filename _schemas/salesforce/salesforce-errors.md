---
description: ''
layout: schema
name: Errors
properties_list:
- description: ''
  name: field
  type: string
- description: ''
  name: message
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-errors-schema.json
slug: salesforce-errors
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"field\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"field\",\n    \"message\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Errors\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-errors-schema.json
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
title: Errors
---
