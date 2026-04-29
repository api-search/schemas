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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-policy-attributes-schema.json\",\n  \"title\": \"PolicyAttributes\",\n  \"description\": \"Attributes of an escalation policy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the escalation policy.\",\n      \"example\": \"Default On-Call\"\n    },\n    \"repeat_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times to repeat the escalation cycle.\",\n      \"example\": 3\n    },\n    \"repeat_delay\": {\n      \"type\": \"integer\",\n      \"description\": \"Delay in seconds between repeat cycles.\",\n      \"example\": 300\n    },\n    \"incident_token\": {\n      \"type\": \"string\",\n      \"description\": \"Unique token for the policy.\",\n      \"example\": \"abc123\"\n    },\n\
  \    \"policy_group_id\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"ID of the policy group.\",\n      \"example\": null\n    },\n    \"team_name\": {\n      \"type\": \"string\",\n      \"description\": \"Team owning this policy.\",\n      \"example\": \"my-team\"\n    },\n    \"steps\": {\n      \"type\": \"array\",\n      \"description\": \"Escalation steps in sequence.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PolicyStep\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-policy-attributes-schema.json
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
