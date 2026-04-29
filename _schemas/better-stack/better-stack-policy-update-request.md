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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-policy-update-request-schema.json\",\n  \"title\": \"PolicyUpdateRequest\",\n  \"description\": \"Request body for updating an escalation policy (all fields optional).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"New policy name.\",\n      \"example\": \"Updated On-Call Policy\"\n    },\n    \"repeat_count\": {\n      \"type\": \"integer\",\n      \"description\": \"New repeat count.\",\n      \"example\": 5\n    },\n    \"repeat_delay\": {\n      \"type\": \"integer\",\n      \"description\": \"New repeat delay in seconds.\",\n      \"example\": 600\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-policy-update-request-schema.json
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
