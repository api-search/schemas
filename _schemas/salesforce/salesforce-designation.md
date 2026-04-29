---
description: ''
layout: schema
name: Designation
properties_list:
- description: ''
  name: designationId
  type: string
- description: ''
  name: percent
  type: integer
- description: ''
  name: amount
  type: number
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-designation-schema.json
slug: salesforce-designation
source_filename: salesforce-designation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"designationId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"percent\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"example\": 42.5\n    }\n  },\n  \"required\": [\n    \"designationId\",\n    \"percent\",\n    \"amount\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Designation\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-designation-schema.json
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
title: Designation
---
