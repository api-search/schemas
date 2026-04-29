---
description: A debuggable browser target from the Microsoft Edge DevTools Protocol HTTP API
layout: schema
name: Target
properties_list:
- description: Target description
  name: description
  type: string
- description: URL to the DevTools frontend for this target
  name: devtoolsFrontendUrl
  type: string
- description: URL to the target's favicon
  name: faviconUrl
  type: string
- description: Unique target identifier
  name: id
  type: string
- description: Page title
  name: title
  type: string
- description: Target type
  name: type
  type: string
- description: Current URL of the target
  name: url
  type: string
- description: WebSocket URL for debugging this target
  name: webSocketDebuggerUrl
  type: string
provider_name: Microsoft Edge
provider_slug: microsoft-edge
schema_file: json-schema/devtools-api-target-schema.json
slug: devtools-api-target
source_filename: devtools-api-target-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-edge/refs/heads/main/json-schema/devtools-api-target-schema.json\",\n  \"title\": \"Target\",\n  \"description\": \"A debuggable browser target from the Microsoft Edge DevTools Protocol HTTP API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Target description\"\n    },\n    \"devtoolsFrontendUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL to the DevTools frontend for this target\"\n    },\n    \"faviconUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL to the target's favicon\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique target identifier\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Page title\"\n    },\n    \"type\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Target type\",\n      \"enum\": [\"page\", \"background_page\", \"service_worker\", \"worker\", \"iframe\", \"other\"]\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Current URL of the target\"\n    },\n    \"webSocketDebuggerUrl\": {\n      \"type\": \"string\",\n      \"description\": \"WebSocket URL for debugging this target\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-edge/refs/heads/main/json-schema/devtools-api-target-schema.json
tags:
- Browser
- Chromium
- Developer Tools
- Edge
- Extensions
- Microsoft
- Progressive Web Apps
- Web Development
- WebView
title: Target
---
