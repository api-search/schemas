---
description: A single audit log entry.
layout: schema
name: AuditLogEntry
properties_list:
- description: Log entry ID.
  name: id
  type: string
- description: User who performed the action.
  name: user
  type: string
- description: Action performed.
  name: action
  type: string
- description: Unix timestamp.
  name: timestamp
  type: integer
provider_name: BigPanda
provider_slug: bigpanda
schema_file: json-schema/bigpanda-audit-log-entry-schema.json
slug: bigpanda-audit-log-entry
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"AuditLogEntry\",\n  \"type\": \"object\",\n  \"description\": \"A single audit log entry.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Log entry ID.\",\n      \"example\": \"log-abc123\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"User who performed the action.\",\n      \"example\": \"admin@example.com\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"Action performed.\",\n      \"example\": \"created_environment\"\n    },\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp.\",\n      \"example\": 1713000000\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bigpanda/refs/heads/main/json-schema/bigpanda-audit-log-entry-schema.json
tags:
- Incidents
- Monitoring
- Platform
title: AuditLogEntry
---
