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
