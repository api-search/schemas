---
description: A single team member resource.
layout: schema
name: TeamMemberObject
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
schema_file: json-schema/better-stack-team-member-object-schema.json
slug: better-stack-team-member-object
source_filename: better-stack-team-member-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-team-member-object-schema.json\",\n  \"title\": \"TeamMemberObject\",\n  \"description\": \"A single team member resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier.\",\n      \"example\": \"200001\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type.\",\n      \"example\": \"team_member\"\n    },\n    \"attributes\": {\n      \"$ref\": \"#/components/schemas/TeamMemberAttributes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-team-member-object-schema.json
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
title: TeamMemberObject
---
