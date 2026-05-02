---
description: An Insomnia workspace is the top-level organizational unit that groups related API requests, environments, mock servers, and design specifications. Workspaces can represent a Design Document for API design or a Collection for request organization.
layout: schema
name: Insomnia Workspace
properties_list:
- description: Unique identifier for the workspace, typically prefixed with wrk_.
  name: _id
  type: string
- description: Human-readable name of the workspace.
  name: name
  type: string
- description: Optional description providing context about the workspace purpose.
  name: description
  type: string
- description: 'The workspace scope: design for API specification design, collection for request organization.'
  name: scope
  type: string
- description: Identifier of the parent project or organization.
  name: parentId
  type:
  - string
  - 'null'
- description: Unix timestamp in milliseconds when the workspace was created.
  name: created
  type: integer
- description: Unix timestamp in milliseconds when the workspace was last modified.
  name: modified
  type: integer
- description: Whether the workspace is private and not shared with team members.
  name: isPrivate
  type: boolean
- description: The resource type identifier.
  name: _type
  type: string
provider_name: Insomnia
provider_slug: insomnia
schema_file: json-schema/workspace.json
slug: workspace
source_filename: workspace.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/insomnia/refs/heads/main/json-schema/workspace.json\",\n  \"title\": \"Insomnia Workspace\",\n  \"description\": \"An Insomnia workspace is the top-level organizational unit that groups related API requests, environments, mock servers, and design specifications. Workspaces can represent a Design Document for API design or a Collection for request organization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the workspace, typically prefixed with wrk_.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the workspace.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description providing context about the workspace purpose.\"\n    },\n    \"scope\": {\n\
  \      \"type\": \"string\",\n      \"enum\": [\"design\", \"collection\"],\n      \"description\": \"The workspace scope: design for API specification design, collection for request organization.\"\n    },\n    \"parentId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Identifier of the parent project or organization.\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp in milliseconds when the workspace was created.\"\n    },\n    \"modified\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp in milliseconds when the workspace was last modified.\"\n    },\n    \"isPrivate\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the workspace is private and not shared with team members.\",\n      \"default\": false\n    },\n    \"_type\": {\n      \"type\": \"string\",\n      \"const\": \"workspace\",\n      \"description\": \"The resource type identifier.\"\n    }\n  },\n  \"required\"\
  : [\"_id\", \"name\", \"scope\", \"_type\"],\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/insomnia/refs/heads/main/json-schema/workspace.json
tags:
- API Design
- CLI
- Clients
- Mocking
- Platform
- Testing
title: Insomnia Workspace
---
