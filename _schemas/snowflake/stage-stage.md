---
description: A Snowflake stage.
layout: schema
name: Stage
properties_list:
- description: Specifies whether the stage is permanent or temporary.
  name: kind
  type: string
- description: URL for the external stage; blank for an internal stage.
  name: url
  type: string
- description: The S3-compatible API endpoint associated with the stage; always NULL for stages that are not S3-compatible.
  name: endpoint
  type: string
- description: Specifies a comment for the stage.
  name: comment
  type: string
- description: Encryption parameters of the stage.
  name: encryption
  type: object
- description: Directory table parameters of the stage.
  name: directory_table
  type: object
- description: Date and time when the stage was created.
  name: created_on
  type: string
- description: Indicates that the external stage has access credentials; always false for an internal stage.
  name: has_credentials
  type: boolean
- description: Indicates that the external stage contains encrypted files; always false for an internal stage.
  name: has_encryption_key
  type: boolean
- description: Role that owns the stage.
  name: owner
  type: string
- description: The type of role that owns the object, either ROLE or DATABASE_ROLE. If a Snowflake Native App owns the object, the value is APPLICATION. Snowflake returns NULL if you delete the object because a dele
  name: owner_role_type
  type: string
- description: Region where the stage is located.
  name: region
  type: string
- description: Cloud provider; always NULL for an internal stage.
  name: cloud
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/stage-stage-schema.json
slug: stage-stage
source_filename: stage-stage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Stage\",\n  \"type\": \"object\",\n  \"description\": \"A Snowflake stage.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies whether the stage is permanent or temporary.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"URL for the external stage; blank for an internal stage.\"\n    },\n    \"endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The S3-compatible API endpoint associated with the stage; always NULL for stages that are not S3-compatible.\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies a comment for the stage.\"\n    },\n    \"encryption\": {\n      \"type\": \"object\",\n      \"description\": \"Encryption parameters of the stage.\"\n    },\n    \"directory_table\": {\n      \"type\": \"object\",\n      \"description\": \"Directory\
  \ table parameters of the stage.\"\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the stage was created.\"\n    },\n    \"has_credentials\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates that the external stage has access credentials; always false for an internal stage.\"\n    },\n    \"has_encryption_key\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates that the external stage contains encrypted files; always false for an internal stage.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Role that owns the stage.\"\n    },\n    \"owner_role_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of role that owns the object, either ROLE or DATABASE_ROLE. If a Snowflake Native App owns the object, the value is APPLICATION. Snowflake returns NULL if you delete the object because a deleted object does not have an owner role.\"\n    },\n  \
  \  \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Region where the stage is located.\"\n    },\n    \"cloud\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud provider; always NULL for an internal stage.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/stage-stage-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Stage
---
