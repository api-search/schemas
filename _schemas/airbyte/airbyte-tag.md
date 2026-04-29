---
description: A tag that can be associated with a connection. Useful for grouping and organizing connections in a workspace.
layout: schema
name: Tag
properties_list:
- description: ''
  name: tagId
  type: object
- description: ''
  name: workspaceId
  type: object
- description: ''
  name: name
  type: string
- description: ''
  name: color
  type: string
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-tag-schema.json
slug: airbyte-tag
source_filename: airbyte-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"A tag that can be associated with a connection. Useful for grouping and organizing connections in a workspace.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tagId\": {\n      \"$ref\": \"#/components/schemas/TagId\"\n    },\n    \"workspaceId\": {\n      \"$ref\": \"#/components/schemas/WorkspaceId\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"color\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"tagId\",\n    \"workspaceId\",\n    \"name\",\n    \"color\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-tag-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: Tag
---
