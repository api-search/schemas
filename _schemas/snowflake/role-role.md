---
description: A Snowflake role
layout: schema
name: Role
properties_list:
- description: Name of the role.
  name: name
  type: string
- description: Comment of the role.
  name: comment
  type: string
- description: Date and time when the role was created.
  name: created_on
  type: string
- description: Specifies the role that owns this role.
  name: owner
  type: string
- description: Specifies whether the role being fetched is the user's default role.
  name: is_default
  type: boolean
- description: Specifies whether the role being fetched is the user's current role.
  name: is_current
  type: boolean
- description: Specifies whether the role used to run the command inherits the specified role.
  name: is_inherited
  type: boolean
- description: The number of users to whom this role has been assigned.
  name: assigned_to_users
  type: integer
- description: The number of roles to which this role has been granted.
  name: granted_to_roles
  type: integer
- description: The number of roles that have been granted to this role.
  name: granted_roles
  type: integer
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/role-role-schema.json
slug: role-role
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Role\",\n  \"type\": \"object\",\n  \"description\": \"A Snowflake role\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the role.\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Comment of the role.\"\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the role was created.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the role that owns this role.\"\n    },\n    \"is_default\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether the role being fetched is the user's default role.\"\n    },\n    \"is_current\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether the role being fetched is the user's current role.\"\n    },\n    \"is_inherited\": {\n      \"\
  type\": \"boolean\",\n      \"description\": \"Specifies whether the role used to run the command inherits the specified role.\"\n    },\n    \"assigned_to_users\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of users to whom this role has been assigned.\"\n    },\n    \"granted_to_roles\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of roles to which this role has been granted.\"\n    },\n    \"granted_roles\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of roles that have been granted to this role.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/role-role-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Role
---
