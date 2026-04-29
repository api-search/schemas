---
description: Provides details of a single tag.
layout: schema
name: TagResponse
properties_list:
- description: ''
  name: tagId
  type: object
- description: ''
  name: name
  type: string
- description: A hexadecimal color value
  name: color
  type: string
- description: ''
  name: workspaceId
  type: object
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-tag-response-schema.json
slug: airbyte-tag-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-tag-response-schema.json\",\n  \"title\": \"TagResponse\",\n  \"description\": \"Provides details of a single tag.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tagId\": {\n      \"$ref\": \"#/components/schemas/TagId\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"color\": {\n      \"description\": \"A hexadecimal color value\",\n      \"type\": \"string\"\n    },\n    \"workspaceId\": {\n      \"$ref\": \"#/components/schemas/WorkspaceId\"\n    }\n  },\n  \"required\": [\n    \"tagId\",\n    \"name\",\n    \"color\",\n    \"workspaceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-tag-response-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: TagResponse
---
