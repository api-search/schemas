---
description: ''
layout: schema
name: Output
properties_list:
- description: ''
  name: results
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-output-schema.json
slug: salesforce-output
source_filename: salesforce-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"output\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"output\"\n      ]\n    }\n  },\n  \"required\": [\n    \"results\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Output\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-output-schema.json
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
title: Output
---
