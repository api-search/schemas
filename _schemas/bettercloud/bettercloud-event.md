---
description: An audit event recording activity in BetterCloud or connected SaaS applications.
layout: schema
name: Event
properties_list:
- description: Unique identifier of the event.
  name: id
  type: string
- description: Event type in dot-notation (e.g., user.suspended, group.created).
  name: type
  type: string
- description: Email of the user or system that triggered the event.
  name: actor_email
  type: string
- description: Email of the user or resource affected by the event.
  name: target_email
  type: string
- description: Human-readable description of what happened.
  name: description
  type: string
- description: When the event occurred.
  name: occurred_at
  type: string
provider_name: BetterCloud
provider_slug: bettercloud
schema_file: json-schema/bettercloud-event-schema.json
slug: bettercloud-event
source_filename: bettercloud-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-event-schema.json\",\n  \"title\": \"Event\",\n  \"description\": \"An audit event recording activity in BetterCloud or connected SaaS applications.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the event.\",\n      \"example\": \"evt-500100\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Event type in dot-notation (e.g., user.suspended, group.created).\",\n      \"example\": \"user.suspended\"\n    },\n    \"actor_email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"nullable\": true,\n      \"description\": \"Email of the user or system that triggered the event.\",\n      \"example\": \"admin@example.com\"\n    },\n    \"target_email\": {\n \
  \     \"type\": \"string\",\n      \"format\": \"email\",\n      \"nullable\": true,\n      \"description\": \"Email of the user or resource affected by the event.\",\n      \"example\": \"jsmith@example.com\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of what happened.\",\n      \"example\": \"User suspended via BetterCloud workflow\"\n    },\n    \"occurred_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the event occurred.\",\n      \"example\": \"2026-04-18T14:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-event-schema.json
tags:
- Automation
- Compliance
- Enterprise
- IT Operations
- SaaS Management
- Security
- Workflows
- User Lifecycle
title: Event
---
