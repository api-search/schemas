---
description: Request body for creating an escalation policy.
layout: schema
name: PolicyCreateRequest
properties_list:
- description: Policy name.
  name: name
  type: string
- description: Number of repeat cycles.
  name: repeat_count
  type: integer
- description: Delay between cycles in seconds.
  name: repeat_delay
  type: integer
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-policy-create-request-schema.json
slug: better-stack-policy-create-request
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
title: PolicyCreateRequest
---
