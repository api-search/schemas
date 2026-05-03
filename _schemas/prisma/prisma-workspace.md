---
description: A workspace is the top-level organizational unit in the Prisma Data Platform that contains projects, team members, and billing configuration. Workspaces provide shared access control and resource management across all contained projects and databases.
layout: schema
name: Prisma Workspace
properties_list:
- description: Unique identifier for the workspace
  name: id
  type: string
- description: Display name of the workspace
  name: name
  type: string
- description: URL-friendly identifier for the workspace, used in console URLs and API paths
  name: slug
  type: string
- description: Current billing plan for the workspace that determines resource limits and feature availability
  name: plan
  type: string
- description: Team members with access to the workspace
  name: members
  type: array
- description: ISO 8601 timestamp when the workspace was created
  name: createdAt
  type: string
- description: ISO 8601 timestamp when the workspace was last updated
  name: updatedAt
  type: string
provider_name: Prisma
provider_slug: prisma
schema_file: json-schema/prisma-workspace-schema.json
slug: prisma-workspace
source_filename: prisma-workspace-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://prisma.io/schemas/workspace.json\",\n  \"title\": \"Prisma Workspace\",\n  \"description\": \"A workspace is the top-level organizational unit in the Prisma Data Platform that contains projects, team members, and billing configuration. Workspaces provide shared access control and resource management across all contained projects and databases.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the workspace\",\n      \"examples\": [\"ws_abc123def456\"]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the workspace\",\n      \"minLength\": 1,\n      \"maxLength\": 255,\n      \"examples\": [\"My Workspace\"]\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"URL-friendly identifier for the workspace, used in console URLs and\
  \ API paths\",\n      \"pattern\": \"^[a-z0-9][a-z0-9-]*[a-z0-9]$\",\n      \"examples\": [\"my-workspace\"]\n    },\n    \"plan\": {\n      \"type\": \"string\",\n      \"description\": \"Current billing plan for the workspace that determines resource limits and feature availability\",\n      \"enum\": [\"free\", \"pro\", \"business\", \"enterprise\"]\n    },\n    \"members\": {\n      \"type\": \"array\",\n      \"description\": \"Team members with access to the workspace\",\n      \"items\": {\n        \"$ref\": \"#/$defs/WorkspaceMember\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the workspace was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the workspace was last updated\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"slug\", \"plan\", \"createdAt\", \"updatedAt\"\
  ],\n  \"additionalProperties\": false,\n  \"$defs\": {\n    \"WorkspaceMember\": {\n      \"type\": \"object\",\n      \"description\": \"A member of a workspace with an assigned role controlling access permissions\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the membership\"\n        },\n        \"userId\": {\n          \"type\": \"string\",\n          \"description\": \"Identifier of the user\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"Email address of the member\"\n        },\n        \"role\": {\n          \"type\": \"string\",\n          \"description\": \"Role assigned to the member within the workspace\",\n          \"enum\": [\"owner\", \"admin\", \"member\", \"viewer\"]\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Current status of the membership\",\n\
  \          \"enum\": [\"active\", \"invited\", \"suspended\"]\n        },\n        \"joinedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the member joined\"\n        }\n      },\n      \"required\": [\"id\", \"userId\", \"email\", \"role\", \"status\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/prisma/refs/heads/main/json-schema/prisma-workspace-schema.json
tags: []
title: Prisma Workspace
---
