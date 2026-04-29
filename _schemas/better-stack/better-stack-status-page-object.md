---
description: A single status page resource.
layout: schema
name: StatusPageObject
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
schema_file: json-schema/better-stack-status-page-object-schema.json
slug: better-stack-status-page-object
source_filename: better-stack-status-page-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-status-page-object-schema.json\",\n  \"title\": \"StatusPageObject\",\n  \"description\": \"A single status page resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier.\",\n      \"example\": \"700010\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type.\",\n      \"example\": \"status_page\"\n    },\n    \"attributes\": {\n      \"$ref\": \"#/components/schemas/StatusPageAttributes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-status-page-object-schema.json
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
title: StatusPageObject
---
