---
description: Response containing the remote browser session details.
layout: schema
name: CreateSessionResponse
properties_list:
- description: Unique identifier for the created session.
  name: session_id
  type: string
- description: WebSocket URL for Chrome DevTools Protocol access.
  name: cdp_url
  type: string
- description: ISO 8601 timestamp when the session will expire.
  name: expires_at
  type: string
provider_name: AgentQL
provider_slug: agentql
schema_file: json-schema/agentql-create-session-response-schema.json
slug: agentql-create-session-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agentql/refs/heads/main/json-schema/agentql-create-session-response-schema.json\",\n  \"title\": \"CreateSessionResponse\",\n  \"description\": \"Response containing the remote browser session details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"session_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the created session.\",\n      \"example\": \"sess-a1b2c3d4e5f6\"\n    },\n    \"cdp_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"WebSocket URL for Chrome DevTools Protocol access.\",\n      \"example\": \"wss://tetra.agentql.com/sessions/sess-a1b2c3d4/cdp\"\n    },\n    \"expires_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the session will expire.\",\n      \"example\": \"2026-04-19T15:30:00Z\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agentql/refs/heads/main/json-schema/agentql-create-session-response-schema.json
tags:
- Agents
- Artificial Intelligence
- Web Scraping
- Data Extraction
- Browser Automation
- REST API
title: CreateSessionResponse
---
