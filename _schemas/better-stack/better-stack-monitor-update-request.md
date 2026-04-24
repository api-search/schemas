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
