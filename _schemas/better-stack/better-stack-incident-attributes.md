---
description: Attributes of an incident.
layout: schema
name: IncidentAttributes
properties_list:
- description: Name or subject of the incident.
  name: name
  type: string
- description: URL of the affected monitor.
  name: url
  type: string
- description: HTTP method of the affected check.
  name: http_method
  type: string
- description: Root cause description of the incident.
  name: cause
  type: string
- description: When the incident started.
  name: started_at
  type: string
- description: When the incident was acknowledged.
  name: acknowledged_at
  type: string
- description: When the incident was resolved.
  name: resolved_at
  type: string
- description: Current incident status.
  name: status
  type: string
- description: Team that owns the incident.
  name: team_name
  type: string
- description: Regions where the incident was detected.
  name: regions
  type: array
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-incident-attributes-schema.json
slug: better-stack-incident-attributes
source_filename: better-stack-incident-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-incident-attributes-schema.json\",\n  \"title\": \"IncidentAttributes\",\n  \"description\": \"Attributes of an incident.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name or subject of the incident.\",\n      \"example\": \"Production API\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"nullable\": true,\n      \"description\": \"URL of the affected monitor.\",\n      \"example\": \"https://example.com\"\n    },\n    \"http_method\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"HTTP method of the affected check.\",\n      \"example\": \"GET\"\n    },\n    \"cause\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\"\
  : \"Root cause description of the incident.\",\n      \"example\": \"Connection timeout\"\n    },\n    \"started_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the incident started.\",\n      \"example\": \"2026-04-18T14:00:00Z\"\n    },\n    \"acknowledged_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"description\": \"When the incident was acknowledged.\",\n      \"example\": \"2026-04-18T14:05:00Z\"\n    },\n    \"resolved_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"description\": \"When the incident was resolved.\",\n      \"example\": \"2026-04-18T14:15:00Z\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current incident status.\",\n      \"enum\": [\n        \"Started\",\n        \"Resolved\"\n      ],\n      \"example\": \"Resolved\"\n    },\n    \"team_name\": {\n   \
  \   \"type\": \"string\",\n      \"description\": \"Team that owns the incident.\",\n      \"example\": \"my-team\"\n    },\n    \"regions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Regions where the incident was detected.\",\n      \"example\": [\n        \"us\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-incident-attributes-schema.json
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
title: IncidentAttributes
---
