---
description: ''
layout: schema
name: PlatformEventSchemabyEventName
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: namespace
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: fields
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-platform-event-schemaby-event-name-schema.json
slug: salesforce-platform-event-schemaby-event-name
source_filename: salesforce-platform-event-schemaby-event-name-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"type\": {\n            \"type\": \"object\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"name\",\n          \"type\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"namespace\",\n    \"type\",\n    \"fields\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"PlatformEventSchemabyEventName\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-platform-event-schemaby-event-name-schema.json
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
title: PlatformEventSchemabyEventName
---
