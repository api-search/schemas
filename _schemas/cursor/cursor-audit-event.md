---
description: An audit log event from the Cursor Admin API.
layout: schema
name: Cursor Audit Event
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: timestamp
  type: string
- description: Type of audit event (e.g. login, member.added, settings.updated).
  name: eventType
  type: string
- description: ''
  name: userId
  type: string
- description: ''
  name: userEmail
  type: string
- description: ''
  name: details
  type: object
provider_name: Cursor
provider_slug: cursor
schema_file: json-schema/cursor-audit-event-schema.json
slug: cursor-audit-event
source_filename: cursor-audit-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cursor/refs/heads/main/json-schema/cursor-audit-event-schema.json\",\n  \"title\": \"Cursor Audit Event\",\n  \"description\": \"An audit log event from the Cursor Admin API.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"timestamp\", \"eventType\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"eventType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of audit event (e.g. login, member.added, settings.updated).\"\n    },\n    \"userId\": {\n      \"type\": \"string\"\n    },\n    \"userEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\"\n    },\n    \"details\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cursor/refs/heads/main/json-schema/cursor-audit-event-schema.json
tags:
- AI
- AI Editor
- Code Generation
- Coding Assistant
- Copilot
- Developer Tools
- LLM
- Productivity
- VSCode Fork
title: Cursor Audit Event
---
