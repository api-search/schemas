---
description: Request body for updating a heartbeat (all fields optional).
layout: schema
name: HeartbeatUpdateRequest
properties_list:
- description: New name for the heartbeat.
  name: name
  type: string
- description: New period in seconds.
  name: period
  type: integer
- description: New grace period in seconds.
  name: grace
  type: integer
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-heartbeat-update-request-schema.json
slug: better-stack-heartbeat-update-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-heartbeat-update-request-schema.json\",\n  \"title\": \"HeartbeatUpdateRequest\",\n  \"description\": \"Request body for updating a heartbeat (all fields optional).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"New name for the heartbeat.\",\n      \"example\": \"Updated Backup Job\"\n    },\n    \"period\": {\n      \"type\": \"integer\",\n      \"description\": \"New period in seconds.\",\n      \"example\": 86400\n    },\n    \"grace\": {\n      \"type\": \"integer\",\n      \"description\": \"New grace period in seconds.\",\n      \"example\": 7200\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-heartbeat-update-request-schema.json
tags:
- Incidents
- Logs
- Monitoring
- Platform
- Status
- Uptime
- Observability
- On-Call
- Heartbeats
title: HeartbeatUpdateRequest
---
