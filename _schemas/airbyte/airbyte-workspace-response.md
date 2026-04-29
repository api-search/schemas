---
description: Provides details of a single workspace.
layout: schema
name: WorkspaceResponse
properties_list:
- description: ''
  name: workspaceId
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: dataResidency
  type: string
- description: ''
  name: notifications
  type: object
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-workspace-response-schema.json
slug: airbyte-workspace-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-workspace-response-schema.json\",\n  \"title\": \"WorkspaceResponse\",\n  \"description\": \"Provides details of a single workspace.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"workspaceId\": {\n      \"format\": \"UUID\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"dataResidency\": {\n      \"type\": \"string\"\n    },\n    \"notifications\": {\n      \"$ref\": \"#/components/schemas/NotificationsConfig\"\n    }\n  },\n  \"required\": [\n    \"workspaceId\",\n    \"name\",\n    \"dataResidency\",\n    \"notifications\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-workspace-response-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: WorkspaceResponse
---
