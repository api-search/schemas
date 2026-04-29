---
description: Single incident response.
layout: schema
name: IncidentSingleResponse
properties_list:
- description: ''
  name: data
  type: object
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-incident-single-response-schema.json
slug: better-stack-incident-single-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-incident-single-response-schema.json\",\n  \"title\": \"IncidentSingleResponse\",\n  \"description\": \"Single incident response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"$ref\": \"#/components/schemas/IncidentObject\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-incident-single-response-schema.json
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
title: IncidentSingleResponse
---
