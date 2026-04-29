---
description: An app connection (credentials for a third-party service)
layout: schema
name: Connection
properties_list:
- description: Connection ID
  name: id
  type: string
- description: ''
  name: created
  type: string
- description: ''
  name: updated
  type: string
- description: Connection name
  name: name
  type: string
- description: Integration piece name
  name: pieceName
  type: string
- description: Project ID
  name: projectId
  type: string
- description: Connection status
  name: status
  type: string
- description: Authentication type
  name: type
  type: string
provider_name: Activepieces
provider_slug: activepieces
schema_file: json-schema/activepieces-connection-schema.json
slug: activepieces-connection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-connection-schema.json\",\n  \"title\": \"Connection\",\n  \"description\": \"An app connection (credentials for a third-party service)\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Connection ID\",\n      \"example\": \"conn-abc123\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Connection name\",\n      \"example\": \"My Gmail Account\"\n    },\n    \"pieceName\": {\n      \"type\": \"string\",\n      \"description\": \"Integration piece name\",\n      \"example\": \"@activepieces/piece-gmail\"\n    },\n    \"\
  projectId\": {\n      \"type\": \"string\",\n      \"description\": \"Project ID\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"ERROR\",\n        \"EXPIRED\"\n      ],\n      \"description\": \"Connection status\",\n      \"example\": \"ACTIVE\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"OAUTH2\",\n        \"API_KEY\",\n        \"BASIC_AUTH\",\n        \"CUSTOM_AUTH\"\n      ],\n      \"description\": \"Authentication type\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-connection-schema.json
tags:
- Automation
- No-Code
- Open Source
- Workflow
- AI Agents
- MCP
title: Connection
---
