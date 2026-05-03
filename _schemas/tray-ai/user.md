---
description: A user in the Tray.ai platform, either an external embedded user or an organization member.
layout: schema
name: Tray.ai User
properties_list:
- description: Tray internal user identifier
  name: id
  type: string
- description: Display name of the user
  name: name
  type: string
- description: External user identifier set during creation (embedded users only)
  name: externalUserId
  type: string
- description: Email address of the user
  name: email
  type: string
- description: Whether the user is marked as a test user (excluded from billing)
  name: isTestUser
  type: boolean
- description: Role of the user in the organization
  name: role
  type: string
- description: Account status (active, invited, etc.)
  name: status
  type: string
provider_name: Tray.ai
provider_slug: tray-ai
schema_file: json-schema/user.json
slug: user
source_filename: user.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/json-schema/user.json\",\n  \"title\": \"Tray.ai User\",\n  \"description\": \"A user in the Tray.ai platform, either an external embedded user or an organization member.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Tray internal user identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the user\"\n    },\n    \"externalUserId\": {\n      \"type\": \"string\",\n      \"description\": \"External user identifier set during creation (embedded users only)\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the user\"\n    },\n    \"isTestUser\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user is\
  \ marked as a test user (excluded from billing)\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"Role of the user in the organization\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Account status (active, invited, etc.)\"\n    }\n  },\n  \"required\": [\"id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/json-schema/user.json
tags:
- Automation
- Integration
- iPaaS
title: Tray.ai User
---
