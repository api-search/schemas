---
description: ''
layout: schema
name: Fields
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: items
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-fields-schema.json
slug: salesforce-fields
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"items\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"type\"\n      ]\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"items\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Fields\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-fields-schema.json
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
title: Fields
---
