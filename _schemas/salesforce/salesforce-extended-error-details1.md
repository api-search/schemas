---
description: ''
layout: schema
name: ExtendedErrorDetails1
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: items
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-extended-error-details1-schema.json
slug: salesforce-extended-error-details1
source_filename: salesforce-extended-error-details1-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"items\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"properties\": {\n          \"type\": \"object\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"type\",\n        \"properties\"\n      ]\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"items\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExtendedErrorDetails1\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-extended-error-details1-schema.json
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
title: ExtendedErrorDetails1
---
