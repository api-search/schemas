---
description: Response to an arm or disarm command.
layout: schema
name: SystemStatusResponse
properties_list:
- description: ID of the system.
  name: systemId
  type: string
- description: New system status after command.
  name: status
  type: string
- description: Timestamp of the status change.
  name: timestamp
  type: string
provider_name: ADT
provider_slug: adt
schema_file: json-schema/platform-api-system-status-response-schema.json
slug: platform-api-system-status-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-system-status-response-schema.json\",\n  \"title\": \"SystemStatusResponse\",\n  \"description\": \"Response to an arm or disarm command.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"systemId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the system.\",\n      \"example\": \"sys-001\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"New system status after command.\",\n      \"example\": \"armed_away\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the status change.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-system-status-response-schema.json
tags:
- Access Control
- Automation
- Home Security
- IoT
- Monitoring
- Security
- Smart Home
title: SystemStatusResponse
---
