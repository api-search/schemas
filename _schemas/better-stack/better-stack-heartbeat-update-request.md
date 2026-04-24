---
description: Request body for updating a heartbeat (all fields optional).
layout: schema
name: HeartbeatUpdateRequest
properties_list:
- description: New name for the heartbeat.
  name: name
  type: string
- description: New period in seconds.
  name: period
  type: integer
- description: New grace period in seconds.
  name: grace
  type: integer
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-heartbeat-update-request-schema.json
slug: better-stack-heartbeat-update-request
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
title: HeartbeatUpdateRequest
---
