---
description: ''
layout: schema
name: GrantOf
properties_list:
- description: Date and time when the grant was created
  name: created_on
  type: string
- description: The name of the service role
  name: role
  type: string
- description: The type of the grantee, can be USER or ROLE
  name: granted_to
  type: string
- description: The name of the grantee
  name: grantee_name
  type: string
- description: The name of role that granted the service role to the grantee
  name: granted_by
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/service-grant-of-schema.json
slug: service-grant-of
source_filename: service-grant-of-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GrantOf\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the grant was created\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the service role\"\n    },\n    \"granted_to\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the grantee, can be USER or ROLE\"\n    },\n    \"grantee_name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the grantee\"\n    },\n    \"granted_by\": {\n      \"type\": \"string\",\n      \"description\": \"The name of role that granted the service role to the grantee\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/service-grant-of-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: GrantOf
---
