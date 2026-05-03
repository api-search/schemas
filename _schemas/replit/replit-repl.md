---
description: A Repl is a coding environment on the Replit platform.
layout: schema
name: Replit Repl
properties_list:
- description: Unique identifier for the Repl.
  name: id
  type: string
- description: URL-friendly identifier for the Repl.
  name: slug
  type: string
- description: Display name of the Repl.
  name: title
  type: string
- description: Description of what the Repl does.
  name: description
  type:
  - string
  - 'null'
- description: Primary programming language (e.g., nodejs, python3, ruby).
  name: language
  type: string
- description: Whether the Repl is private.
  name: isPrivate
  type: boolean
- description: URL to the Repl on Replit.
  name: url
  type: string
- description: When the Repl was created.
  name: createdAt
  type: string
- description: When the Repl was last updated.
  name: updatedAt
  type: string
- description: The user or organization that owns this Repl.
  name: owner
  type: object
provider_name: Replit
provider_slug: replit
schema_file: json-schema/replit-repl-schema.json
slug: replit-repl
source_filename: replit-repl-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/replit/json-schema/replit-repl-schema.json\",\n  \"title\": \"Replit Repl\",\n  \"description\": \"A Repl is a coding environment on the Replit platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the Repl.\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"URL-friendly identifier for the Repl.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the Repl.\"\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Description of what the Repl does.\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Primary programming language (e.g., nodejs, python3, ruby).\"\n    },\n    \"isPrivate\": {\n      \"type\": \"boolean\"\
  ,\n      \"description\": \"Whether the Repl is private.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the Repl on Replit.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the Repl was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the Repl was last updated.\"\n    },\n    \"owner\": {\n      \"type\": \"object\",\n      \"description\": \"The user or organization that owns this Repl.\",\n      \"properties\": {\n        \"id\": { \"type\": \"integer\" },\n        \"username\": { \"type\": \"string\" },\n        \"displayName\": { \"type\": \"string\" }\n      }\n    }\n  },\n  \"required\": [\"id\", \"slug\", \"title\", \"language\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/replit/refs/heads/main/json-schema/replit-repl-schema.json
tags:
- Code
- Compiling
- Development Environment
- Programming Languages
- Version Control
title: Replit Repl
---
