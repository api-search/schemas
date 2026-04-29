---
description: BrowserSession schema from Palo Alto Networks Prisma Access Browser Management API
layout: schema
name: BrowserSession
properties_list:
- description: Unique identifier of the browser session.
  name: session_id
  type: string
- description: User ID of the session owner.
  name: user_id
  type: string
- description: Device ID used in this session.
  name: device_id
  type: string
- description: Client IP address.
  name: ip_address
  type: string
- description: Policy applied during this session.
  name: policy_id
  type: string
- description: Prisma Access Browser version.
  name: browser_version
  type: string
- description: Session status.
  name: status
  type: string
- description: ''
  name: started_at
  type: string
- description: ''
  name: ended_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-access-browser-api-browser-session-schema.json
slug: prisma-access-browser-api-browser-session
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BrowserSession\",\n  \"description\": \"BrowserSession schema from Palo Alto Networks Prisma Access Browser Management API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-browser-api-browser-session-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"session_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the browser session.\"\n    },\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"User ID of the session owner.\"\n    },\n    \"device_id\": {\n      \"type\": \"string\",\n      \"description\": \"Device ID used in this session.\"\n    },\n    \"ip_address\": {\n      \"type\": \"string\",\n      \"description\": \"Client IP address.\"\n    },\n    \"policy_id\": {\n      \"type\": \"string\",\n      \"description\": \"Policy applied during\
  \ this session.\"\n    },\n    \"browser_version\": {\n      \"type\": \"string\",\n      \"description\": \"Prisma Access Browser version.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"active\",\n        \"terminated\"\n      ],\n      \"description\": \"Session status.\"\n    },\n    \"started_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"ended_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-browser-api-browser-session-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: BrowserSession
---
