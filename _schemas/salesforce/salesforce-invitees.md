---
description: ''
layout: schema
name: Invitees
properties_list:
- description: ''
  name: emails
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-invitees-schema.json
slug: salesforce-invitees
source_filename: salesforce-invitees-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"emails\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": \"user@example.com\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"emails\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Invitees\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-invitees-schema.json
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
title: Invitees
---
