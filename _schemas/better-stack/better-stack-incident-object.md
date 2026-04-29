---
description: A single incident resource.
layout: schema
name: IncidentObject
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
schema_file: json-schema/better-stack-incident-object-schema.json
slug: better-stack-incident-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-incident-object-schema.json\",\n  \"title\": \"IncidentObject\",\n  \"description\": \"A single incident resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier.\",\n      \"example\": \"900100\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type.\",\n      \"example\": \"incident\"\n    },\n    \"attributes\": {\n      \"$ref\": \"#/components/schemas/IncidentAttributes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-incident-object-schema.json
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
title: IncidentObject
---
