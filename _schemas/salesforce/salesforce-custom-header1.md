---
description: ''
layout: schema
name: CustomHeader1
properties_list:
- description: ''
  name: headerName
  type: string
- description: ''
  name: headerValue
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: sequenceNumber
  type: integer
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-custom-header1-schema.json
slug: salesforce-custom-header1
source_filename: salesforce-custom-header1-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"headerName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"headerValue\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"sequenceNumber\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    }\n  },\n  \"required\": [\n    \"headerName\",\n    \"headerValue\",\n    \"id\",\n    \"sequenceNumber\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CustomHeader1\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-custom-header1-schema.json
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
title: CustomHeader1
---
