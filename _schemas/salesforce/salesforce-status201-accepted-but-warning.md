---
description: ''
layout: schema
name: Status201-AcceptedButWarning
properties_list:
- description: ''
  name: outputs
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-status201-accepted-but-warning-schema.json
slug: salesforce-status201-accepted-but-warning
source_filename: salesforce-status201-accepted-but-warning-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"outputs\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"error\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"results\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"required\": [\n          \"error\",\n          \"results\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"outputs\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Status201-AcceptedButWarning\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-status201-accepted-but-warning-schema.json
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
title: Status201-AcceptedButWarning
---
