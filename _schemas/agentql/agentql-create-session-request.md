---
description: Request body for creating a remote browser session.
layout: schema
name: CreateSessionRequest
properties_list:
- description: Operating system to simulate in the browser user agent.
  name: browser_ua_preset
  type: string
- description: Browser behavior profile.
  name: browser_profile
  type: string
- description: Seconds of inactivity before the session is automatically terminated.
  name: inactivity_timeout_seconds
  type: integer
- description: Proxy configuration for the browser session.
  name: proxy
  type: object
provider_name: AgentQL
provider_slug: agentql
schema_file: json-schema/agentql-create-session-request-schema.json
slug: agentql-create-session-request
source_filename: agentql-create-session-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agentql/refs/heads/main/json-schema/agentql-create-session-request-schema.json\",\n  \"title\": \"CreateSessionRequest\",\n  \"description\": \"Request body for creating a remote browser session.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"browser_ua_preset\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"windows\",\n        \"macos\",\n        \"linux\"\n      ],\n      \"description\": \"Operating system to simulate in the browser user agent.\",\n      \"example\": \"macos\"\n    },\n    \"browser_profile\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"light\",\n        \"stealth\"\n      ],\n      \"description\": \"Browser behavior profile.\",\n      \"example\": \"stealth\"\n    },\n    \"inactivity_timeout_seconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Seconds of inactivity before\
  \ the session is automatically terminated.\",\n      \"example\": 300\n    },\n    \"proxy\": {\n      \"type\": \"object\",\n      \"description\": \"Proxy configuration for the browser session.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"tetra\",\n            \"custom\"\n          ],\n          \"example\": \"tetra\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agentql/refs/heads/main/json-schema/agentql-create-session-request-schema.json
tags:
- Agents
- Artificial Intelligence
- Web Scraping
- Data Extraction
- Browser Automation
- REST API
title: CreateSessionRequest
---
