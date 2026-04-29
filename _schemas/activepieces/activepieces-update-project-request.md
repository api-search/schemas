---
description: UpdateProjectRequest schema from Activepieces API
layout: schema
name: UpdateProjectRequest
properties_list:
- description: New project name
  name: displayName
  type: string
- description: Notification settings
  name: notifyStatus
  type: string
provider_name: Activepieces
provider_slug: activepieces
schema_file: json-schema/activepieces-update-project-request-schema.json
slug: activepieces-update-project-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-update-project-request-schema.json\",\n  \"title\": \"UpdateProjectRequest\",\n  \"description\": \"UpdateProjectRequest schema from Activepieces API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"New project name\"\n    },\n    \"notifyStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ALWAYS\",\n        \"NEVER\",\n        \"NEW_ISSUE\"\n      ],\n      \"description\": \"Notification settings\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-update-project-request-schema.json
tags:
- Automation
- No-Code
- Open Source
- Workflow
- AI Agents
- MCP
title: UpdateProjectRequest
---
