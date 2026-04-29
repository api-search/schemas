---
description: ''
layout: schema
name: ServiceRoleGrantTo
properties_list:
- description: Date and time when the grant was created
  name: created_on
  type: string
- description: The name of the privilege
  name: privilege
  type: string
- description: The type of of the securable
  name: granted_on
  type: string
- description: The name of the securable
  name: name
  type: string
- description: The type of the grantee
  name: granted_to
  type: string
- description: The name of the grantee
  name: grantee_name
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/service-service-role-grant-to-schema.json
slug: service-service-role-grant-to
source_filename: service-service-role-grant-to-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceRoleGrantTo\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the grant was created\"\n    },\n    \"privilege\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the privilege\"\n    },\n    \"granted_on\": {\n      \"type\": \"string\",\n      \"description\": \"The type of of the securable\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the securable\"\n    },\n    \"granted_to\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the grantee\"\n    },\n    \"grantee_name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the grantee\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/service-service-role-grant-to-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ServiceRoleGrantTo
---
