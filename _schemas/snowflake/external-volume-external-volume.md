---
description: A Snowflake external volume
layout: schema
name: ExternalVolume
properties_list:
- description: String that specifies the identifier (the name) for the external volume; must be unique in your account.
  name: name
  type: string
- description: Set of named cloud storage locations in different regions and, optionally, cloud platforms.
  name: storage_locations
  type: array
- description: Specifies whether write operations are allowed for the external volume; must be set to TRUE for Iceberg tables that use Snowflake as the catalog.
  name: allow_writes
  type: boolean
- description: String (literal) that specifies a comment for the external volume.
  name: comment
  type: string
- description: Date and time when the external volume was created.
  name: created_on
  type: string
- description: Role that owns the external volume
  name: owner
  type: string
- description: The type of role that owns the external volume
  name: owner_role_type
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/external-volume-external-volume-schema.json
slug: external-volume-external-volume
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExternalVolume\",\n  \"type\": \"object\",\n  \"description\": \"A Snowflake external volume\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"String that specifies the identifier (the name) for the external volume; must be unique in your account.\"\n    },\n    \"storage_locations\": {\n      \"type\": \"array\",\n      \"description\": \"Set of named cloud storage locations in different regions and, optionally, cloud platforms.\"\n    },\n    \"allow_writes\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether write operations are allowed for the external volume; must be set to TRUE for Iceberg tables that use Snowflake as the catalog.\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"String (literal) that specifies a comment for the external volume.\"\n    },\n    \"created_on\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"Date and time when the external volume was created.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Role that owns the external volume\"\n    },\n    \"owner_role_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of role that owns the external volume\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/external-volume-external-volume-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ExternalVolume
---
