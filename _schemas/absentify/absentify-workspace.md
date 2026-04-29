---
description: Workspace settings and configuration.
layout: schema
name: Workspace
properties_list:
- description: Unique identifier of the workspace.
  name: id
  type: string
- description: Name of the workspace.
  name: name
  type: string
- description: Timestamp when the workspace was created.
  name: createdAt
  type: string
- description: Timestamp when the workspace was last updated.
  name: updatedAt
  type: string
provider_name: Absentify
provider_slug: absentify
schema_file: json-schema/absentify-workspace-schema.json
slug: absentify-workspace
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/absentify/main/json-schema/absentify-workspace-schema.json\",\n  \"title\": \"Workspace\",\n  \"description\": \"Workspace settings and configuration.\",\n  \"type\": \"object\",\n  \"x-schema-source\": \"openapi-spec\",\n  \"x-provider\": \"absentify\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the workspace.\",\n      \"example\": \"500001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the workspace.\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the workspace was created.\",\n      \"example\": \"2024-01-01T00:00:00Z\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"Timestamp when the workspace was last updated.\",\n      \"example\": \"2025-06-01T09:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/absentify/refs/heads/main/json-schema/absentify-workspace-schema.json
tags:
- Absence Management
- HR
- Leave Management
- Microsoft Teams
- Human Resources
title: Workspace
---
