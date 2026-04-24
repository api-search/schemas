---
description: Attributes of an incident.
layout: schema
name: IncidentAttributes
properties_list:
- description: Name or subject of the incident.
  name: name
  type: string
- description: URL of the affected monitor.
  name: url
  type: string
- description: HTTP method of the affected check.
  name: http_method
  type: string
- description: Root cause description of the incident.
  name: cause
  type: string
- description: When the incident started.
  name: started_at
  type: string
- description: When the incident was acknowledged.
  name: acknowledged_at
  type: string
- description: When the incident was resolved.
  name: resolved_at
  type: string
- description: Current incident status.
  name: status
  type: string
- description: Team that owns the incident.
  name: team_name
  type: string
- description: Regions where the incident was detected.
  name: regions
  type: array
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-incident-attributes-schema.json
slug: better-stack-incident-attributes
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
title: IncidentAttributes
---
