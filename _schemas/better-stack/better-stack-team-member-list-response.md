---
description: List of team members.
layout: schema
name: TeamMemberListResponse
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: pagination
  type: object
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-team-member-list-response-schema.json
slug: better-stack-team-member-list-response
source_filename: better-stack-team-member-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-team-member-list-response-schema.json\",\n  \"title\": \"TeamMemberListResponse\",\n  \"description\": \"List of team members.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TeamMemberObject\"\n      }\n    },\n    \"pagination\": {\n      \"$ref\": \"#/components/schemas/Pagination\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-team-member-list-response-schema.json
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
title: TeamMemberListResponse
---
