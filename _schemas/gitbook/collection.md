---
description: A collection in GitBook that organizes and groups related spaces together within an organization.
layout: schema
name: GitBook Collection
properties_list:
- description: The unique identifier of the collection.
  name: id
  type: string
- description: The title of the collection.
  name: title
  type: string
- description: The description of the collection.
  name: description
  type: string
- description: The timestamp when the collection was created.
  name: createdAt
  type: string
- description: The timestamp when the collection was last updated.
  name: updatedAt
  type: string
provider_name: GitBook
provider_slug: gitbook
schema_file: json-schema/collection.json
slug: collection
source_filename: collection.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/gitbook/blob/main/json-schema/collection.json\",\n  \"title\": \"GitBook Collection\",\n  \"description\": \"A collection in GitBook that organizes and groups related spaces together within an organization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the collection.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the collection.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the collection.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the collection was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n    \
  \  \"description\": \"The timestamp when the collection was last updated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/json-schema/collection.json
tags:
- Content
- Documentation
- Experience
- Integrations
- Platform
- SDKs
title: GitBook Collection
---
