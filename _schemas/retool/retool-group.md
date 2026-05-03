---
description: A group in a Retool organization used to manage permissions for apps, resources, and workflows.
layout: schema
name: Retool Group
properties_list:
- description: The numeric identifier for the group.
  name: id
  type: integer
- description: The name of the group.
  name: name
  type: string
- description: Users who are members of this group.
  name: members
  type: array
- description: Timestamp when the group was created.
  name: createdAt
  type: string
- description: Timestamp when the group was last updated.
  name: updatedAt
  type: string
provider_name: Retool
provider_slug: retool
schema_file: json-schema/retool-group-schema.json
slug: retool-group
source_filename: retool-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/retool/json-schema/retool-group-schema.json\",\n  \"title\": \"Retool Group\",\n  \"description\": \"A group in a Retool organization used to manage permissions for apps, resources, and workflows.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The numeric identifier for the group.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the group.\"\n    },\n    \"members\": {\n      \"type\": \"array\",\n      \"description\": \"Users who are members of this group.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"string\", \"format\": \"uuid\" },\n          \"email\": { \"type\": \"string\", \"format\": \"email\" }\n        }\n      }\n    },\n    \"\
  createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the group was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the group was last updated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/retool/refs/heads/main/json-schema/retool-group-schema.json
tags:
- Admin Panel
- Dashboard
- Internal Tools
- Low Code
- No Code
title: Retool Group
---
