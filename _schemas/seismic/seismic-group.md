---
description: A user group in the Seismic platform used for organizing users and controlling access to content and features.
layout: schema
name: Seismic Group
properties_list:
- description: Unique identifier of the group.
  name: id
  type: string
- description: Name of the group.
  name: name
  type: string
- description: Description of the group.
  name: description
  type: string
- description: ID of the parent group for hierarchical grouping.
  name: parentId
  type:
  - string
  - 'null'
- description: Number of members in the group.
  name: memberCount
  type: integer
- description: Timestamp when the group was created.
  name: createdAt
  type: string
- description: Timestamp when the group was last modified.
  name: modifiedAt
  type: string
provider_name: Seismic
provider_slug: seismic
schema_file: json-schema/seismic-group-schema.json
slug: seismic-group
source_filename: seismic-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.seismic.com/schemas/group\",\n  \"title\": \"Seismic Group\",\n  \"description\": \"A user group in the Seismic platform used for organizing users and controlling access to content and features.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the group.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the group.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the group.\"\n    },\n    \"parentId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the parent group for hierarchical grouping.\"\n    },\n    \"memberCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of members in the group.\",\n      \"minimum\": 0\n    },\n    \"createdAt\": {\n\
  \      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the group was created.\"\n    },\n    \"modifiedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the group was last modified.\"\n    }\n  },\n  \"required\": [\"id\", \"name\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/json-schema/seismic-group-schema.json
tags: []
title: Seismic Group
---
