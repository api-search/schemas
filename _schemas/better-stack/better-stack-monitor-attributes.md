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
