---
description: ''
layout: schema
name: Credentials
properties_list:
- description: ''
  name: testCredential
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-credentials-schema.json
slug: salesforce-credentials
source_filename: salesforce-credentials-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"testCredential\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"encrypted\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        }\n      },\n      \"required\": [\n        \"value\",\n        \"encrypted\"\n      ]\n    }\n  },\n  \"required\": [\n    \"testCredential\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Credentials\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-credentials-schema.json
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
title: Credentials
---
