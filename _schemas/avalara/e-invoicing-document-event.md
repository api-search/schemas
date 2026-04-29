---
description: DocumentEvent schema from Avalara API
layout: schema
name: DocumentEvent
properties_list:
- description: ''
  name: eventDate
  type: string
- description: ''
  name: eventType
  type: string
- description: ''
  name: message
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/e-invoicing-document-event-schema.json
slug: e-invoicing-document-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/e-invoicing-document-event-schema.json\",\n  \"title\": \"DocumentEvent\",\n  \"description\": \"DocumentEvent schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"eventType\": {\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/e-invoicing-document-event-schema.json
tags:
- Taxes
title: DocumentEvent
---
