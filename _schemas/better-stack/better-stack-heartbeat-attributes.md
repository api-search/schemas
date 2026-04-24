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
