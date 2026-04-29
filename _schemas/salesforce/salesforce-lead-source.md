---
description: ''
layout: schema
name: LeadSource
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: description
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-lead-source-schema.json
slug: salesforce-lead-source
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"A sample description.\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"description\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LeadSource\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-lead-source-schema.json
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
title: LeadSource
---
