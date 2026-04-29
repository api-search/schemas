---
description: Attributes of a team member.
layout: schema
name: TeamMemberAttributes
properties_list:
- description: Team member's email address.
  name: email
  type: string
- description: Team member's display name.
  name: name
  type: string
- description: Team member role.
  name: role
  type: string
- description: When the member joined or was invited.
  name: created_at
  type: string
- description: When the record was last updated.
  name: updated_at
  type: string
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-team-member-attributes-schema.json
slug: better-stack-team-member-attributes
source_filename: better-stack-team-member-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-team-member-attributes-schema.json\",\n  \"title\": \"TeamMemberAttributes\",\n  \"description\": \"Attributes of a team member.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Team member's email address.\",\n      \"example\": \"jsmith@example.com\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Team member's display name.\",\n      \"example\": \"Jane Smith\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"Team member role.\",\n      \"enum\": [\n        \"owner\",\n        \"admin\",\n        \"member\",\n        \"viewer\"\n      ],\n      \"example\": \"admin\"\n    },\n    \"created_at\": {\n\
  \      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the member joined or was invited.\",\n      \"example\": \"2025-01-10T08:00:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the record was last updated.\",\n      \"example\": \"2026-03-01T12:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-team-member-attributes-schema.json
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
title: TeamMemberAttributes
---
