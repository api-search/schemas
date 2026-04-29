---
description: ''
layout: schema
name: PrescribableField
properties_list:
- description: ''
  name: customDefinitions
  type: array
- description: ''
  name: field
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-prescribable-field-schema.json
slug: salesforce-prescribable-field
source_filename: salesforce-prescribable-field-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"customDefinitions\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"field\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"label\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"label\",\n        \"name\",\n        \"type\"\n      ]\n    }\n  },\n  \"required\": [\n    \"customDefinitions\",\n    \"field\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PrescribableField\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-prescribable-field-schema.json
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
title: PrescribableField
---
