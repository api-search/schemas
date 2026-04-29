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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-policy-create-request-schema.json\",\n  \"title\": \"PolicyCreateRequest\",\n  \"description\": \"Request body for creating an escalation policy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Policy name.\",\n      \"example\": \"Default On-Call\"\n    },\n    \"repeat_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of repeat cycles.\",\n      \"example\": 3\n    },\n    \"repeat_delay\": {\n      \"type\": \"integer\",\n      \"description\": \"Delay between cycles in seconds.\",\n      \"example\": 300\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-policy-create-request-schema.json
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
