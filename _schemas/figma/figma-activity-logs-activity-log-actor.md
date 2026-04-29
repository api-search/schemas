---
description: The user who performed the action.
layout: schema
name: ActivityLogActor
properties_list:
- description: The type of the user.
  name: type
  type: string
- description: The ID of the user.
  name: id
  type: string
- description: The name of the user.
  name: name
  type: string
- description: The email of the user.
  name: email
  type: string
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-activity-logs-activity-log-actor-schema.json
slug: figma-activity-logs-activity-log-actor
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ActivityLogActor\",\n  \"type\": \"['object', 'null']\",\n  \"description\": \"The user who performed the action.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the user.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the user.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the user.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"The email of the user.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-activity-logs-activity-log-actor-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: ActivityLogActor
---
