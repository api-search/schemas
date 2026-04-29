---
description: The task or activity the actor performed.
layout: schema
name: ActivityLogAction
properties_list:
- description: The type of the action.
  name: type
  type: string
- description: Metadata of the action.
  name: details
  type: '[''object'', ''null'']'
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-activity-logs-activity-log-action-schema.json
slug: figma-activity-logs-activity-log-action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ActivityLogAction\",\n  \"type\": \"object\",\n  \"description\": \"The task or activity the actor performed.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the action.\"\n    },\n    \"details\": {\n      \"type\": \"['object', 'null']\",\n      \"description\": \"Metadata of the action.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-activity-logs-activity-log-action-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: ActivityLogAction
---
