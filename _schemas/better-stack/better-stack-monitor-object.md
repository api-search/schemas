---
description: A single monitor resource following JSON:API format.
layout: schema
name: MonitorObject
properties_list:
- description: Unique identifier of the monitor.
  name: id
  type: string
- description: Resource type identifier.
  name: type
  type: string
- description: ''
  name: attributes
  type: object
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-monitor-object-schema.json
slug: better-stack-monitor-object
source_filename: better-stack-monitor-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-monitor-object-schema.json\",\n  \"title\": \"MonitorObject\",\n  \"description\": \"A single monitor resource following JSON:API format.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the monitor.\",\n      \"example\": \"500123\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type identifier.\",\n      \"example\": \"monitor\"\n    },\n    \"attributes\": {\n      \"$ref\": \"#/components/schemas/MonitorAttributes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-monitor-object-schema.json
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
title: MonitorObject
---
