---
description: CursorPaging from WhatsApp API
layout: schema
name: CursorPaging
properties_list:
- description: ''
  name: cursors
  type: object
- description: ''
  name: next
  type: string
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-flows-api-cursor-paging-schema.json
slug: whatsapp-flows-api-cursor-paging
source_filename: whatsapp-flows-api-cursor-paging-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-flows-api-cursor-paging-schema.json\",\n  \"title\": \"CursorPaging\",\n  \"description\": \"CursorPaging from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cursors\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"before\": {\n          \"type\": \"string\"\n        },\n        \"after\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"next\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-flows-api-cursor-paging-schema.json
tags: []
title: CursorPaging
---
