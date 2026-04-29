---
description: ''
layout: schema
name: Error
properties_list:
- description: ''
  name: errorCode
  type: string
- description: ''
  name: errorMessage
  type: string
- description: ''
  name: recordId
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-error-schema.json
slug: salesforce-error
source_filename: salesforce-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorCode\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"recordId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"errorCode\",\n    \"errorMessage\",\n    \"recordId\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-error-schema.json
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
title: Error
---
