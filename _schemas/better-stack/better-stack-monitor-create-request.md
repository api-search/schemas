---
description: Request body for creating a new monitor.
layout: schema
name: MonitorCreateRequest
properties_list:
- description: The URL to monitor.
  name: url
  type: string
- description: Human-readable name for the monitor.
  name: pronounceable_name
  type: string
- description: Type of monitoring check.
  name: monitor_type
  type: string
- description: Check interval in seconds.
  name: check_frequency
  type: integer
- description: Whether to verify SSL certificate.
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
- description: Regions to monitor from.
  name: regions
  type: array
- description: Escalation policy ID.
  name: policy_id
  type: string
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-monitor-create-request-schema.json
slug: better-stack-monitor-create-request
source_filename: better-stack-monitor-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-monitor-create-request-schema.json\",\n  \"title\": \"MonitorCreateRequest\",\n  \"description\": \"Request body for creating a new monitor.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to monitor.\",\n      \"example\": \"https://example.com\"\n    },\n    \"pronounceable_name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the monitor.\",\n      \"example\": \"Production API\"\n    },\n    \"monitor_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of monitoring check.\",\n      \"enum\": [\n        \"status\",\n        \"expected_status_code\",\n        \"keyword\",\n        \"keyword_absence\",\n        \"ping\",\n        \"\
  tcp\"\n      ],\n      \"example\": \"status\"\n    },\n    \"check_frequency\": {\n      \"type\": \"integer\",\n      \"description\": \"Check interval in seconds.\",\n      \"example\": 180\n    },\n    \"verify_ssl\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to verify SSL certificate.\",\n      \"example\": true\n    },\n    \"email\": {\n      \"type\": \"boolean\",\n      \"description\": \"Alert via email.\",\n      \"example\": true\n    },\n    \"sms\": {\n      \"type\": \"boolean\",\n      \"description\": \"Alert via SMS.\",\n      \"example\": false\n    },\n    \"call\": {\n      \"type\": \"boolean\",\n      \"description\": \"Alert via phone call.\",\n      \"example\": false\n    },\n    \"push\": {\n      \"type\": \"boolean\",\n      \"description\": \"Alert via push notification.\",\n      \"example\": true\n    },\n    \"regions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\"\
  : \"Regions to monitor from.\",\n      \"example\": [\n        \"us\",\n        \"eu\"\n      ]\n    },\n    \"policy_id\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Escalation policy ID.\",\n      \"example\": \"300010\"\n    }\n  },\n  \"required\": [\n    \"url\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-monitor-create-request-schema.json
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
title: MonitorCreateRequest
---
