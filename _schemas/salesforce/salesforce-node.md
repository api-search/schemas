---
description: ''
layout: schema
name: Node
properties_list:
- description: ''
  name: Id
  type: string
- description: ''
  name: Name
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-node-schema.json
slug: salesforce-node
source_filename: salesforce-node-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"Name\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"value\"\n      ]\n    }\n  },\n  \"required\": [\n    \"Id\",\n    \"Name\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Node\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-node-schema.json
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
title: Node
---
