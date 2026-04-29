---
description: A Snowflake database role
layout: schema
name: DatabaseRole
properties_list:
- description: Name of the database role
  name: name
  type: string
- description: User comment associated to an object in the dictionary
  name: comment
  type: string
- description: Date and time when the database role was created
  name: created_on
  type: string
- description: How many roles this database role has been granted to
  name: granted_to_roles
  type: integer
- description: How many database roles this database role has been granted to
  name: granted_to_database_roles
  type: integer
- description: How many database roles this database role has been granted
  name: granted_database_roles
  type: integer
- description: Role that owns the database role
  name: owner
  type: string
- description: The type of role that owns the database role
  name: owner_role_type
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/database-role-database-role-schema.json
slug: database-role-database-role
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DatabaseRole\",\n  \"type\": \"object\",\n  \"description\": \"A Snowflake database role\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the database role\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"User comment associated to an object in the dictionary\"\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the database role was created\"\n    },\n    \"granted_to_roles\": {\n      \"type\": \"integer\",\n      \"description\": \"How many roles this database role has been granted to\"\n    },\n    \"granted_to_database_roles\": {\n      \"type\": \"integer\",\n      \"description\": \"How many database roles this database role has been granted to\"\n    },\n    \"granted_database_roles\": {\n      \"type\": \"integer\",\n      \"description\": \"\
  How many database roles this database role has been granted\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Role that owns the database role\"\n    },\n    \"owner_role_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of role that owns the database role\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/database-role-database-role-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: DatabaseRole
---
