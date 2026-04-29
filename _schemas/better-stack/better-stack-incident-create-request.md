---
description: Request body for creating a manual incident.
layout: schema
name: IncidentCreateRequest
properties_list:
- description: Name or description of the incident.
  name: name
  type: string
- description: Alert via email.
  name: email
  type: boolean
- description: Alert via SMS.
  name: sms
  type: boolean
- description: Alert via phone call.
  name: call
  type: boolean
- description: Alert via push notification.
  name: push
  type: boolean
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-incident-create-request-schema.json
slug: better-stack-incident-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-incident-create-request-schema.json\",\n  \"title\": \"IncidentCreateRequest\",\n  \"description\": \"Request body for creating a manual incident.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name or description of the incident.\",\n      \"example\": \"Database degraded\"\n    },\n    \"email\": {\n      \"type\": \"boolean\",\n      \"description\": \"Alert via email.\",\n      \"example\": true\n    },\n    \"sms\": {\n      \"type\": \"boolean\",\n      \"description\": \"Alert via SMS.\",\n      \"example\": false\n    },\n    \"call\": {\n      \"type\": \"boolean\",\n      \"description\": \"Alert via phone call.\",\n      \"example\": false\n    },\n    \"push\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Alert via push notification.\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-incident-create-request-schema.json
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
title: IncidentCreateRequest
---
