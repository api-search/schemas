---
description: ''
layout: schema
name: Metadata2
properties_list:
- description: ''
  name: enrichedFields
  type: array
- description: ''
  name: eventChannel
  type: string
- description: ''
  name: selectedEntity
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-metadata2-schema.json
slug: salesforce-metadata2
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"enrichedFields\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          }\n        },\n        \"required\": [\n          \"name\"\n        ]\n      }\n    },\n    \"eventChannel\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"selectedEntity\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"enrichedFields\",\n    \"eventChannel\",\n    \"selectedEntity\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Metadata2\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-metadata2-schema.json
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
title: Metadata2
---
