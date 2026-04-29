---
description: Attributes of an uptime monitor.
layout: schema
name: MonitorAttributes
properties_list:
- description: The URL being monitored.
  name: url
  type: string
- description: Human-readable name for the monitor.
  name: pronounceable_name
  type: string
- description: Type of monitoring check.
  name: monitor_type
  type: string
- description: Current operational status of the monitor.
  name: status
  type: string
- description: ID of the monitor group this monitor belongs to.
  name: monitor_group_id
  type: string
- description: ID of the escalation policy for this monitor.
  name: policy_id
  type: string
- description: How often to check the URL in seconds.
  name: check_frequency
  type: integer
- description: Whether to verify SSL certificate validity.
  name: verify_ssl
  type: boolean
- description: Days before SSL expiration to start alerting.
  name: ssl_expiration
  type: integer
- description: Whether to alert via phone call.
  name: call
  type: boolean
- description: Whether to alert via SMS.
  name: sms
  type: boolean
- description: Whether to alert via email.
  name: email
  type: boolean
- description: Whether to alert via push notification.
  name: push
  type: boolean
- description: Geographic regions from which to check the monitor.
  name: regions
  type: array
- description: When the monitor was created.
  name: created_at
  type: string
- description: When the monitor was last updated.
  name: updated_at
  type: string
- description: When the monitor was paused, if applicable.
  name: paused_at
  type: string
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-monitor-attributes-schema.json
slug: better-stack-monitor-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-monitor-attributes-schema.json\",\n  \"title\": \"MonitorAttributes\",\n  \"description\": \"Attributes of an uptime monitor.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL being monitored.\",\n      \"example\": \"https://example.com\"\n    },\n    \"pronounceable_name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the monitor.\",\n      \"example\": \"Production API\"\n    },\n    \"monitor_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of monitoring check.\",\n      \"enum\": [\n        \"status\",\n        \"expected_status_code\",\n        \"keyword\",\n        \"keyword_absence\",\n        \"ping\",\n        \"tcp\",\n \
  \       \"udp\",\n        \"smtp\",\n        \"pop\",\n        \"imap\"\n      ],\n      \"example\": \"status\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current operational status of the monitor.\",\n      \"enum\": [\n        \"paused\",\n        \"pending\",\n        \"maintenance\",\n        \"up\",\n        \"validating\",\n        \"down\"\n      ],\n      \"example\": \"up\"\n    },\n    \"monitor_group_id\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"ID of the monitor group this monitor belongs to.\",\n      \"example\": null\n    },\n    \"policy_id\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"ID of the escalation policy for this monitor.\",\n      \"example\": \"300010\"\n    },\n    \"check_frequency\": {\n      \"type\": \"integer\",\n      \"description\": \"How often to check the URL in seconds.\",\n      \"example\": 180\n    },\n    \"verify_ssl\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to verify SSL certificate validity.\",\n      \"example\": true\n    },\n    \"ssl_expiration\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"description\": \"Days before SSL expiration to start alerting.\",\n      \"example\": 30\n    },\n    \"call\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to alert via phone call.\",\n      \"example\": false\n    },\n    \"sms\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to alert via SMS.\",\n      \"example\": true\n    },\n    \"email\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to alert via email.\",\n      \"example\": true\n    },\n    \"push\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to alert via push notification.\",\n      \"example\": true\n    },\n    \"regions\": {\n      \"type\": \"array\",\n      \"description\": \"Geographic regions from which to\
  \ check the monitor.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"us\",\n        \"eu\"\n      ]\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the monitor was created.\",\n      \"example\": \"2025-01-15T10:00:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the monitor was last updated.\",\n      \"example\": \"2026-04-01T08:30:00Z\"\n    },\n    \"paused_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"description\": \"When the monitor was paused, if applicable.\",\n      \"example\": null\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-monitor-attributes-schema.json
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
title: MonitorAttributes
---
