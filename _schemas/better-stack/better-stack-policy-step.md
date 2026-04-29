---
description: A step in an escalation policy.
layout: schema
name: PolicyStep
properties_list:
- description: Step resource type.
  name: type
  type: string
- description: ''
  name: attributes
  type: object
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-policy-step-schema.json
slug: better-stack-policy-step
source_filename: better-stack-policy-step-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-policy-step-schema.json\",\n  \"title\": \"PolicyStep\",\n  \"description\": \"A step in an escalation policy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Step resource type.\",\n      \"example\": \"step\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"step_type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of notification step.\",\n          \"enum\": [\n            \"notification\",\n            \"wait\"\n          ],\n          \"example\": \"notification\"\n        },\n        \"wait_before\": {\n          \"type\": \"integer\",\n          \"description\": \"Seconds to wait before this step.\",\n          \"example\": 0\n        }\n    \
  \  }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-policy-step-schema.json
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
title: PolicyStep
---
