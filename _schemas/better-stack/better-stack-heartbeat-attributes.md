---
description: Attributes of a heartbeat monitor.
layout: schema
name: HeartbeatAttributes
properties_list:
- description: Human-readable name for the heartbeat.
  name: name
  type: string
- description: The URL to ping to signal the heartbeat.
  name: url
  type: string
- description: Expected period between heartbeat pings in seconds.
  name: period
  type: integer
- description: Grace period in seconds before alerting.
  name: grace
  type: integer
- description: Current status of the heartbeat.
  name: status
  type: string
- description: Alert via phone call.
  name: call
  type: boolean
- description: Alert via SMS.
  name: sms
  type: boolean
- description: Alert via email.
  name: email
  type: boolean
- description: Alert via push notification.
  name: push
  type: boolean
- description: When the heartbeat was created.
  name: created_at
  type: string
- description: When the heartbeat was last updated.
  name: updated_at
  type: string
- description: When the heartbeat was paused.
  name: paused_at
  type: string
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-heartbeat-attributes-schema.json
slug: better-stack-heartbeat-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-heartbeat-attributes-schema.json\",\n  \"title\": \"HeartbeatAttributes\",\n  \"description\": \"Attributes of a heartbeat monitor.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the heartbeat.\",\n      \"example\": \"Daily Backup Job\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to ping to signal the heartbeat.\",\n      \"example\": \"https://uptime.betterstack.com/api/v1/heartbeat/abc123\"\n    },\n    \"period\": {\n      \"type\": \"integer\",\n      \"description\": \"Expected period between heartbeat pings in seconds.\",\n      \"example\": 86400\n    },\n    \"grace\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Grace period in seconds before alerting.\",\n      \"example\": 3600\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the heartbeat.\",\n      \"enum\": [\n        \"paused\",\n        \"pending\",\n        \"up\",\n        \"down\"\n      ],\n      \"example\": \"up\"\n    },\n    \"call\": {\n      \"type\": \"boolean\",\n      \"description\": \"Alert via phone call.\",\n      \"example\": false\n    },\n    \"sms\": {\n      \"type\": \"boolean\",\n      \"description\": \"Alert via SMS.\",\n      \"example\": false\n    },\n    \"email\": {\n      \"type\": \"boolean\",\n      \"description\": \"Alert via email.\",\n      \"example\": true\n    },\n    \"push\": {\n      \"type\": \"boolean\",\n      \"description\": \"Alert via push notification.\",\n      \"example\": true\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the heartbeat was created.\"\
  ,\n      \"example\": \"2025-06-01T00:00:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the heartbeat was last updated.\",\n      \"example\": \"2026-04-01T00:00:00Z\"\n    },\n    \"paused_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"description\": \"When the heartbeat was paused.\",\n      \"example\": null\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-heartbeat-attributes-schema.json
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
title: HeartbeatAttributes
---
