---
description: A Zesty.io role defines a set of permissions that can be assigned to users for controlling access to instance resources.
layout: schema
name: Zesty Role
properties_list:
- description: The Zesty Universal Identifier for the role.
  name: ZUID
  type: string
- description: The name of the role.
  name: name
  type: string
- description: The instance ZUID this role is scoped to.
  name: instanceZUID
  type: string
- description: Whether this is a built-in system role.
  name: systemRole
  type: boolean
- description: Timestamp when the role was created.
  name: createdAt
  type: string
- description: Timestamp when the role was last updated.
  name: updatedAt
  type: string
provider_name: Zesty
provider_slug: zesty
schema_file: json-schema/role.json
slug: role
source_filename: role.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/zesty/blob/main/json-schema/role.json\",\n  \"title\": \"Zesty Role\",\n  \"description\": \"A Zesty.io role defines a set of permissions that can be assigned to users for controlling access to instance resources.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ZUID\": {\n      \"type\": \"string\",\n      \"description\": \"The Zesty Universal Identifier for the role.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the role.\"\n    },\n    \"instanceZUID\": {\n      \"type\": \"string\",\n      \"description\": \"The instance ZUID this role is scoped to.\"\n    },\n    \"systemRole\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a built-in system role.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp\
  \ when the role was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the role was last updated.\"\n    }\n  },\n  \"required\": [\"ZUID\", \"name\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/json-schema/role.json
tags:
- CMS
- Composable
- Content Management
- Headless CMS
- Media
title: Zesty Role
---
