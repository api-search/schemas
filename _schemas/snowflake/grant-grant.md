---
description: Properties of a grant that can be granted to a role or user.
layout: schema
name: Grant
properties_list:
- description: Privilege type
  name: privileges
  type: array
- description: Can grantee pass this privilege down?
  name: grant_option
  type: boolean
- description: ''
  name: created_on
  type: string
- description: Entity type being granted to
  name: grantee_type
  type: string
- description: Specific name of object being granted to
  name: grantee_name
  type: string
- description: Type of object granted on
  name: securable_type
  type: string
- description: Name of specific object granted on (not name of privilege!)
  name: securable_name
  type: string
- description: Type of role that granted this privilege to this grantee
  name: granted_by_role_type
  type: string
- description: The role that granted this privilege to this grantee
  name: granted_by_name
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/grant-grant-schema.json
slug: grant-grant
source_filename: grant-grant-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Grant\",\n  \"type\": \"object\",\n  \"description\": \"Properties of a grant that can be granted to a role or user.\",\n  \"properties\": {\n    \"privileges\": {\n      \"type\": \"array\",\n      \"description\": \"Privilege type\"\n    },\n    \"grant_option\": {\n      \"type\": \"boolean\",\n      \"description\": \"Can grantee pass this privilege down?\"\n    },\n    \"created_on\": {\n      \"type\": \"string\"\n    },\n    \"grantee_type\": {\n      \"type\": \"string\",\n      \"description\": \"Entity type being granted to\"\n    },\n    \"grantee_name\": {\n      \"type\": \"string\",\n      \"description\": \"Specific name of object being granted to\"\n    },\n    \"securable_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of object granted on\"\n    },\n    \"securable_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of specific object\
  \ granted on (not name of privilege!)\"\n    },\n    \"granted_by_role_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of role that granted this privilege to this grantee\"\n    },\n    \"granted_by_name\": {\n      \"type\": \"string\",\n      \"description\": \"The role that granted this privilege to this grantee\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/grant-grant-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Grant
---
