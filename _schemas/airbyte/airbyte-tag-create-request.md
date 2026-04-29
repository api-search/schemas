---
description: TagCreateRequest schema from Airbyte API
layout: schema
name: TagCreateRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: color
  type: string
- description: ''
  name: workspaceId
  type: object
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-tag-create-request-schema.json
slug: airbyte-tag-create-request
source_filename: airbyte-tag-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-tag-create-request-schema.json\",\n  \"title\": \"TagCreateRequest\",\n  \"description\": \"TagCreateRequest schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"color\": {\n      \"type\": \"string\"\n    },\n    \"workspaceId\": {\n      \"$ref\": \"#/components/schemas/WorkspaceId\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"color\",\n    \"workspaceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-tag-create-request-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: TagCreateRequest
---
