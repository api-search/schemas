---
description: Browser version and protocol information from the Microsoft Edge DevTools Protocol
layout: schema
name: BrowserVersion
properties_list:
- description: Browser name and version
  name: Browser
  type: string
- description: DevTools Protocol version
  name: Protocol-Version
  type: string
- description: Full user agent string
  name: User-Agent
  type: string
- description: V8 JavaScript engine version
  name: V8-Version
  type: string
- description: WebKit rendering engine version
  name: WebKit-Version
  type: string
- description: WebSocket URL for browser-level debugging
  name: webSocketDebuggerUrl
  type: string
provider_name: Microsoft Edge
provider_slug: microsoft-edge
schema_file: json-schema/devtools-api-browser-version-schema.json
slug: devtools-api-browser-version
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-edge/refs/heads/main/json-schema/devtools-api-browser-version-schema.json\",\n  \"title\": \"BrowserVersion\",\n  \"description\": \"Browser version and protocol information from the Microsoft Edge DevTools Protocol\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Browser\": {\n      \"type\": \"string\",\n      \"description\": \"Browser name and version\"\n    },\n    \"Protocol-Version\": {\n      \"type\": \"string\",\n      \"description\": \"DevTools Protocol version\"\n    },\n    \"User-Agent\": {\n      \"type\": \"string\",\n      \"description\": \"Full user agent string\"\n    },\n    \"V8-Version\": {\n      \"type\": \"string\",\n      \"description\": \"V8 JavaScript engine version\"\n    },\n    \"WebKit-Version\": {\n      \"type\": \"string\",\n      \"description\": \"WebKit rendering engine version\"\n    },\n\
  \    \"webSocketDebuggerUrl\": {\n      \"type\": \"string\",\n      \"description\": \"WebSocket URL for browser-level debugging\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-edge/refs/heads/main/json-schema/devtools-api-browser-version-schema.json
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
title: BrowserVersion
---
