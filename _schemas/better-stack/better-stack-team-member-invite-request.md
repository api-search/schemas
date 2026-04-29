---
description: Request body for inviting a team member.
layout: schema
name: TeamMemberInviteRequest
properties_list:
- description: Email address of the person to invite.
  name: email
  type: string
- description: Role to assign.
  name: role
  type: string
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-team-member-invite-request-schema.json
slug: better-stack-team-member-invite-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-team-member-invite-request-schema.json\",\n  \"title\": \"TeamMemberInviteRequest\",\n  \"description\": \"Request body for inviting a team member.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the person to invite.\",\n      \"example\": \"newmember@example.com\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"Role to assign.\",\n      \"enum\": [\n        \"admin\",\n        \"member\",\n        \"viewer\"\n      ],\n      \"example\": \"member\"\n    }\n  },\n  \"required\": [\n    \"email\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-team-member-invite-request-schema.json
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
title: TeamMemberInviteRequest
---
