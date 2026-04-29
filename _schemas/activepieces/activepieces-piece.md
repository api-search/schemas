---
description: An Activepieces integration piece
layout: schema
name: Piece
properties_list:
- description: Piece package name
  name: name
  type: string
- description: Human-readable name
  name: displayName
  type: string
- description: Piece description
  name: description
  type: string
- description: Piece version
  name: version
  type: string
- description: Piece icon URL
  name: iconUrl
  type: string
- description: Piece categories
  name: categories
  type: array
provider_name: Activepieces
provider_slug: activepieces
schema_file: json-schema/activepieces-piece-schema.json
slug: activepieces-piece
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-piece-schema.json\",\n  \"title\": \"Piece\",\n  \"description\": \"An Activepieces integration piece\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Piece package name\",\n      \"example\": \"@activepieces/piece-github\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name\",\n      \"example\": \"GitHub\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Piece description\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Piece version\",\n      \"example\": \"0.5.0\"\n    },\n    \"iconUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Piece icon URL\"\n\
  \    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Piece categories\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-piece-schema.json
tags:
- Automation
- No-Code
- Open Source
- Workflow
- AI Agents
- MCP
title: Piece
---
