---
description: An event returned by the Activity Logs API.
layout: schema
name: ActivityLog
properties_list:
- description: The ID of the event.
  name: id
  type: string
- description: The timestamp of the event in seconds since the Unix epoch.
  name: timestamp
  type: number
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-activity-logs-activity-log-schema.json
slug: figma-activity-logs-activity-log
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ActivityLog\",\n  \"type\": \"object\",\n  \"description\": \"An event returned by the Activity Logs API.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the event.\"\n    },\n    \"timestamp\": {\n      \"type\": \"number\",\n      \"description\": \"The timestamp of the event in seconds since the Unix epoch.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-activity-logs-activity-log-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: ActivityLog
---
