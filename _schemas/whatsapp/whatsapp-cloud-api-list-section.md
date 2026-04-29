---
description: ListSection from WhatsApp API
layout: schema
name: ListSection
properties_list:
- description: ''
  name: title
  type: string
- description: ''
  name: rows
  type: array
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-cloud-api-list-section-schema.json
slug: whatsapp-cloud-api-list-section
source_filename: whatsapp-cloud-api-list-section-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-list-section-schema.json\",\n  \"title\": \"ListSection\",\n  \"description\": \"ListSection from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"rows\": {\n      \"type\": \"array\",\n      \"maxItems\": 10,\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"maxLength\": 200\n          },\n          \"title\": {\n            \"type\": \"string\",\n            \"maxLength\": 24\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"maxLength\": 72\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-list-section-schema.json
tags: []
title: ListSection
---
