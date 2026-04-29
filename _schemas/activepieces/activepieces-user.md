---
description: An Activepieces platform user
layout: schema
name: User
properties_list:
- description: User ID
  name: id
  type: string
- description: ''
  name: created
  type: string
- description: ''
  name: updated
  type: string
- description: User email
  name: email
  type: string
- description: First name
  name: firstName
  type: string
- description: Last name
  name: lastName
  type: string
- description: User status
  name: status
  type: string
- description: Platform role
  name: platformRole
  type: string
provider_name: Activepieces
provider_slug: activepieces
schema_file: json-schema/activepieces-user-schema.json
slug: activepieces-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-user-schema.json\",\n  \"title\": \"User\",\n  \"description\": \"An Activepieces platform user\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"User ID\",\n      \"example\": \"user-abc123\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"User email\",\n      \"example\": \"user@example.com\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"First name\",\n      \"example\": \"Jane\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Last name\",\n      \"example\": \"Smith\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"INACTIVE\",\n        \"SHADOW\"\n      ],\n      \"description\": \"User status\"\n    },\n    \"platformRole\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ADMIN\",\n        \"MEMBER\"\n      ],\n      \"description\": \"Platform role\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-user-schema.json
tags:
- Automation
- No-Code
- Open Source
- Workflow
- AI Agents
- MCP
title: User
---
