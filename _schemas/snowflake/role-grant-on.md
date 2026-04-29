---
description: ''
layout: schema
name: GrantOn
properties_list:
- description: Date and time when the grant was created
  name: created_on
  type: string
- description: The name of the privilege
  name: privilege
  type: string
- description: The type of of the role
  name: granted_on
  type: string
- description: The name of the role
  name: name
  type: string
- description: The type of the grantee
  name: granted_to
  type: string
- description: The name of the grantee
  name: grantee_name
  type: string
- description: If true, allows the recipient role to grant the privileges to other roles.
  name: grant_option
  type: string
- description: The role that granted this privilege to this grantee
  name: granted_by
  type: string
- description: Type of the role that granted this privilege to this grantee
  name: granted_by_role_type
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/role-grant-on-schema.json
slug: role-grant-on
source_filename: role-grant-on-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GrantOn\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the grant was created\"\n    },\n    \"privilege\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the privilege\"\n    },\n    \"granted_on\": {\n      \"type\": \"string\",\n      \"description\": \"The type of of the role\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the role\"\n    },\n    \"granted_to\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the grantee\"\n    },\n    \"grantee_name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the grantee\"\n    },\n    \"grant_option\": {\n      \"type\": \"string\",\n      \"description\": \"If true, allows the recipient role to grant the privileges to other roles.\"\n    },\n\
  \    \"granted_by\": {\n      \"type\": \"string\",\n      \"description\": \"The role that granted this privilege to this grantee\"\n    },\n    \"granted_by_role_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the role that granted this privilege to this grantee\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/role-grant-on-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: GrantOn
---
