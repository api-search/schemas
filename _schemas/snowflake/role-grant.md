---
description: ''
layout: schema
name: Grant
properties_list:
- description: Type of the securable to be granted.
  name: securable_type
  type: string
- description: If true, allows the recipient role to grant the privileges to other roles.
  name: grant_option
  type: boolean
- description: List of privileges to be granted.
  name: privileges
  type: array
- description: Date and time when the grant was created
  name: created_on
  type: string
- description: The role that granted this privilege to this grantee
  name: granted_by
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/role-grant-schema.json
slug: role-grant
source_filename: role-grant-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Grant\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"securable_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the securable to be granted.\"\n    },\n    \"grant_option\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, allows the recipient role to grant the privileges to other roles.\"\n    },\n    \"privileges\": {\n      \"type\": \"array\",\n      \"description\": \"List of privileges to be granted.\"\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the grant was created\"\n    },\n    \"granted_by\": {\n      \"type\": \"string\",\n      \"description\": \"The role that granted this privilege to this grantee\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/role-grant-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Grant
---
