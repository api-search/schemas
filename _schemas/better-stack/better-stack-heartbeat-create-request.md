---
description: Request body for creating a heartbeat.
layout: schema
name: HeartbeatCreateRequest
properties_list:
- description: Name for the heartbeat.
  name: name
  type: string
- description: Expected period in seconds.
  name: period
  type: integer
- description: Grace period in seconds.
  name: grace
  type: integer
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
schema_file: json-schema/better-stack-heartbeat-create-request-schema.json
slug: better-stack-heartbeat-create-request
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
title: HeartbeatCreateRequest
---
