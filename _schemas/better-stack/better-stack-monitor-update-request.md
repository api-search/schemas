---
description: Request body for updating an existing monitor (all fields optional).
layout: schema
name: MonitorUpdateRequest
properties_list:
- description: New URL to monitor.
  name: url
  type: string
- description: New human-readable name.
  name: pronounceable_name
  type: string
- description: New check interval in seconds.
  name: check_frequency
  type: integer
- description: SSL verification setting.
  name: verify_ssl
  type: boolean
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
schema_file: json-schema/better-stack-monitor-update-request-schema.json
slug: better-stack-monitor-update-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-monitor-update-request-schema.json\",\n  \"title\": \"MonitorUpdateRequest\",\n  \"description\": \"Request body for updating an existing monitor (all fields optional).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"New URL to monitor.\",\n      \"example\": \"https://example.com\"\n    },\n    \"pronounceable_name\": {\n      \"type\": \"string\",\n      \"description\": \"New human-readable name.\",\n      \"example\": \"Updated API Monitor\"\n    },\n    \"check_frequency\": {\n      \"type\": \"integer\",\n      \"description\": \"New check interval in seconds.\",\n      \"example\": 300\n    },\n    \"verify_ssl\": {\n      \"type\": \"boolean\",\n      \"description\": \"SSL verification\
  \ setting.\",\n      \"example\": true\n    },\n    \"email\": {\n      \"type\": \"boolean\",\n      \"description\": \"Alert via email.\",\n      \"example\": true\n    },\n    \"sms\": {\n      \"type\": \"boolean\",\n      \"description\": \"Alert via SMS.\",\n      \"example\": false\n    },\n    \"call\": {\n      \"type\": \"boolean\",\n      \"description\": \"Alert via phone call.\",\n      \"example\": false\n    },\n    \"push\": {\n      \"type\": \"boolean\",\n      \"description\": \"Alert via push notification.\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-monitor-update-request-schema.json
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
title: MonitorUpdateRequest
---
