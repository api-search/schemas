---
description: Specifies the credentials of the stage.
layout: schema
name: Credentials
properties_list:
- description: Type of the credential, can be either AWS or AZURE.
  name: credential_type
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/stage-credentials-schema.json
slug: stage-credentials
source_filename: stage-credentials-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Credentials\",\n  \"type\": \"object\",\n  \"description\": \"Specifies the credentials of the stage.\",\n  \"properties\": {\n    \"credential_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the credential, can be either AWS or AZURE.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/stage-credentials-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Credentials
---
