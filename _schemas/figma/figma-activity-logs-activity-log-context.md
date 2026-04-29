---
description: Contextual information about the event.
layout: schema
name: ActivityLogContext
properties_list:
- description: The third-party application that triggered the event.
  name: clientName
  type: '[''string'', ''null'']'
- description: The IP address from of the client that sent the event request.
  name: ipAddress
  type: string
- description: If Figma's Support team triggered the event.
  name: isFigmaSupportTeamAction
  type: boolean
- description: The id of the organization where the event took place.
  name: orgId
  type: string
- description: The id of the team where the event took place.
  name: teamId
  type: '[''string'', ''null'']'
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-activity-logs-activity-log-context-schema.json
slug: figma-activity-logs-activity-log-context
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ActivityLogContext\",\n  \"type\": \"object\",\n  \"description\": \"Contextual information about the event.\",\n  \"properties\": {\n    \"clientName\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The third-party application that triggered the event.\"\n    },\n    \"ipAddress\": {\n      \"type\": \"string\",\n      \"description\": \"The IP address from of the client that sent the event request.\"\n    },\n    \"isFigmaSupportTeamAction\": {\n      \"type\": \"boolean\",\n      \"description\": \"If Figma's Support team triggered the event.\"\n    },\n    \"orgId\": {\n      \"type\": \"string\",\n      \"description\": \"The id of the organization where the event took place.\"\n    },\n    \"teamId\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The id of the team where the event took place.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-activity-logs-activity-log-context-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: ActivityLogContext
---
