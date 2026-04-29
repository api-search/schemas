---
description: Single heartbeat response.
layout: schema
name: HeartbeatSingleResponse
properties_list:
- description: ''
  name: data
  type: object
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-heartbeat-single-response-schema.json
slug: better-stack-heartbeat-single-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-heartbeat-single-response-schema.json\",\n  \"title\": \"HeartbeatSingleResponse\",\n  \"description\": \"Single heartbeat response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"$ref\": \"#/components/schemas/HeartbeatObject\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-heartbeat-single-response-schema.json
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
title: HeartbeatSingleResponse
---
