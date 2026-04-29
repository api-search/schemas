---
description: ''
layout: schema
name: SingleEmail
properties_list:
- description: ''
  name: Max
  type: integer
- description: ''
  name: Remaining
  type: integer
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-single-email-schema.json
slug: salesforce-single-email
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Max\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"Remaining\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    }\n  },\n  \"required\": [\n    \"Max\",\n    \"Remaining\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SingleEmail\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-single-email-schema.json
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
title: SingleEmail
---
