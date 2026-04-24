---
description: Attributes of an escalation policy.
layout: schema
name: PolicyAttributes
properties_list:
- description: Name of the escalation policy.
  name: name
  type: string
- description: Number of times to repeat the escalation cycle.
  name: repeat_count
  type: integer
- description: Delay in seconds between repeat cycles.
  name: repeat_delay
  type: integer
- description: Unique token for the policy.
  name: incident_token
  type: string
- description: ID of the policy group.
  name: policy_group_id
  type: string
- description: Team owning this policy.
  name: team_name
  type: string
- description: Escalation steps in sequence.
  name: steps
  type: array
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-policy-attributes-schema.json
slug: better-stack-policy-attributes
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
title: PolicyAttributes
---
