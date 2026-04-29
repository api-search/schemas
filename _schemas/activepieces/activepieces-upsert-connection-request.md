---
description: Request body for creating or updating a connection
layout: schema
name: UpsertConnectionRequest
properties_list:
- description: Connection name
  name: name
  type: string
- description: Piece package name
  name: pieceName
  type: string
- description: Project ID
  name: projectId
  type: string
- description: ''
  name: type
  type: string
- description: Authentication credentials
  name: value
  type: object
provider_name: Activepieces
provider_slug: activepieces
schema_file: json-schema/activepieces-upsert-connection-request-schema.json
slug: activepieces-upsert-connection-request
source_filename: activepieces-upsert-connection-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-upsert-connection-request-schema.json\",\n  \"title\": \"UpsertConnectionRequest\",\n  \"description\": \"Request body for creating or updating a connection\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Connection name\",\n      \"example\": \"My GitHub Connection\"\n    },\n    \"pieceName\": {\n      \"type\": \"string\",\n      \"description\": \"Piece package name\",\n      \"example\": \"@activepieces/piece-github\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"Project ID\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"OAUTH2\",\n        \"API_KEY\",\n        \"BASIC_AUTH\",\n        \"CUSTOM_AUTH\"\n      ]\n    },\n    \"value\": {\n  \
  \    \"type\": \"object\",\n      \"description\": \"Authentication credentials\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"pieceName\",\n    \"projectId\",\n    \"type\",\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-upsert-connection-request-schema.json
tags:
- Automation
- No-Code
- Open Source
- Workflow
- AI Agents
- MCP
title: UpsertConnectionRequest
---
