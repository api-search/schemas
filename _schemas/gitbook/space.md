---
description: A space in GitBook is a container for documentation or knowledge base content, with configurable visibility and access settings.
layout: schema
name: GitBook Space
properties_list:
- description: The unique identifier of the space.
  name: id
  type: string
- description: The title of the space.
  name: title
  type: string
- description: The emoji icon for the space.
  name: emoji
  type: string
- description: The visibility setting of the space.
  name: visibility
  type: string
- description: The timestamp when the space was created.
  name: createdAt
  type: string
- description: The timestamp when the space was last updated.
  name: updatedAt
  type: string
- description: The timestamp when the space was deleted, if applicable.
  name: deletedAt
  type: string
- description: URLs associated with the space.
  name: urls
  type: object
provider_name: GitBook
provider_slug: gitbook
schema_file: json-schema/space.json
slug: space
source_filename: space.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/gitbook/blob/main/json-schema/space.json\",\n  \"title\": \"GitBook Space\",\n  \"description\": \"A space in GitBook is a container for documentation or knowledge base content, with configurable visibility and access settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the space.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the space.\"\n    },\n    \"emoji\": {\n      \"type\": \"string\",\n      \"description\": \"The emoji icon for the space.\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"public\",\n        \"unlisted\",\n        \"share-link\",\n        \"in-collection\",\n        \"private\"\n      ],\n      \"description\": \"The visibility setting of the space.\"\
  \n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the space was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the space was last updated.\"\n    },\n    \"deletedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the space was deleted, if applicable.\"\n    },\n    \"urls\": {\n      \"type\": \"object\",\n      \"description\": \"URLs associated with the space.\",\n      \"properties\": {\n        \"app\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the space in the GitBook app.\"\n        },\n        \"published\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the space's published site.\"\n        }\n      }\n    }\n\
  \  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/json-schema/space.json
tags:
- Content
- Documentation
- Experience
- Integrations
- Platform
- SDKs
title: GitBook Space
---
