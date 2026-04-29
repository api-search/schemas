---
description: A single heartbeat resource.
layout: schema
name: HeartbeatObject
properties_list:
- description: Unique identifier.
  name: id
  type: string
- description: Resource type.
  name: type
  type: string
- description: ''
  name: attributes
  type: object
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-heartbeat-object-schema.json
slug: better-stack-heartbeat-object
source_filename: better-stack-heartbeat-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-heartbeat-object-schema.json\",\n  \"title\": \"HeartbeatObject\",\n  \"description\": \"A single heartbeat resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier.\",\n      \"example\": \"100200\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type.\",\n      \"example\": \"heartbeat\"\n    },\n    \"attributes\": {\n      \"$ref\": \"#/components/schemas/HeartbeatAttributes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-heartbeat-object-schema.json
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
title: HeartbeatObject
---
