---
description: A workspace within the API Fiddle platform used to organize and group related API design projects.
layout: schema
name: API Fiddle Workspace
properties_list:
- description: Unique identifier for the workspace.
  name: id
  type: string
- description: Name of the workspace.
  name: name
  type: string
- description: A detailed description of the workspace.
  name: description
  type: string
- description: Identifier of the user who owns the workspace.
  name: ownerId
  type: string
- description: List of members with access to the workspace.
  name: members
  type: array
- description: List of project identifiers within this workspace.
  name: projects
  type: array
- description: Timestamp when the workspace was created.
  name: createdAt
  type: string
- description: Timestamp when the workspace was last updated.
  name: updatedAt
  type: string
provider_name: API-Fiddle
provider_slug: api-fiddle
schema_file: json-schema/api-fiddle-workspace-schema.json
slug: api-fiddle-workspace
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-fiddle.com/schemas/workspace.json\",\n  \"title\": \"API Fiddle Workspace\",\n  \"description\": \"A workspace within the API Fiddle platform used to organize and group related API design projects.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the workspace.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the workspace.\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A detailed description of the workspace.\"\n    },\n    \"ownerId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the user who owns the workspace.\"\n    },\n    \"members\": {\n      \"type\": \"array\",\n      \"description\": \"List of members with access to the workspace.\"\
  ,\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"userId\": {\n            \"type\": \"string\",\n            \"description\": \"Identifier of the member.\"\n          },\n          \"role\": {\n            \"type\": \"string\",\n            \"enum\": [\"viewer\", \"editor\", \"admin\", \"owner\"],\n            \"description\": \"Role of the member within the workspace.\"\n          },\n          \"joinedAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Timestamp when the member joined the workspace.\"\n          }\n        },\n        \"required\": [\"userId\", \"role\"]\n      }\n    },\n    \"projects\": {\n      \"type\": \"array\",\n      \"description\": \"List of project identifiers within this workspace.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Timestamp when the workspace was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the workspace was last updated.\"\n    }\n  },\n  \"required\": [\"id\", \"name\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/api-fiddle/refs/heads/main/json-schema/api-fiddle-workspace-schema.json
tags:
- API Design
- OpenAPI
- Collaboration
- Documentation
- Platform
title: API Fiddle Workspace
---
