---
description: BrowserUser schema from Palo Alto Networks Prisma Access Browser Management API
layout: schema
name: BrowserUser
properties_list:
- description: Unique identifier of the browser user.
  name: user_id
  type: string
- description: User email address.
  name: email
  type: string
- description: User display name.
  name: display_name
  type: string
- description: ID of the browser policy assigned to this user.
  name: policy_id
  type: string
- description: Current number of active browser sessions.
  name: active_sessions
  type: integer
- description: ''
  name: last_active_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-access-browser-api-browser-user-schema.json
slug: prisma-access-browser-api-browser-user
source_filename: prisma-access-browser-api-browser-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BrowserUser\",\n  \"description\": \"BrowserUser schema from Palo Alto Networks Prisma Access Browser Management API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-browser-api-browser-user-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the browser user.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"User email address.\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"User display name.\"\n    },\n    \"policy_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the browser policy assigned to this user.\"\n    },\n    \"active_sessions\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Current number of active browser sessions.\"\n    },\n    \"last_active_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-browser-api-browser-user-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: BrowserUser
---
