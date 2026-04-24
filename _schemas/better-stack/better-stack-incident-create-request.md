---
description: Request body for creating a manual incident.
layout: schema
name: IncidentCreateRequest
properties_list:
- description: Name or description of the incident.
  name: name
  type: string
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
schema_file: json-schema/better-stack-incident-create-request-schema.json
slug: better-stack-incident-create-request
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
title: IncidentCreateRequest
---
