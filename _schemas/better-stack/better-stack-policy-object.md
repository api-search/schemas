---
description: A single escalation policy resource.
layout: schema
name: PolicyObject
properties_list:
- description: Unique identifier.
  name: id
  type: string
- description: Resource type.
  name: type
  type: string
- description: ''
  name: attributes
  type: object
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-policy-object-schema.json
slug: better-stack-policy-object
source_filename: better-stack-policy-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-policy-object-schema.json\",\n  \"title\": \"PolicyObject\",\n  \"description\": \"A single escalation policy resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier.\",\n      \"example\": \"300010\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type.\",\n      \"example\": \"policy\"\n    },\n    \"attributes\": {\n      \"$ref\": \"#/components/schemas/PolicyAttributes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-policy-object-schema.json
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
title: PolicyObject
---
