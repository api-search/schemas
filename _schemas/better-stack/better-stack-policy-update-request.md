---
description: Request body for updating an escalation policy (all fields optional).
layout: schema
name: PolicyUpdateRequest
properties_list:
- description: New policy name.
  name: name
  type: string
- description: New repeat count.
  name: repeat_count
  type: integer
- description: New repeat delay in seconds.
  name: repeat_delay
  type: integer
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-policy-update-request-schema.json
slug: better-stack-policy-update-request
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
title: PolicyUpdateRequest
---
