---
description: ''
layout: schema
name: JavaFunction
properties_list:
- description: List of external access integrations attached to this function/procedure
  name: external_access_integrations
  type: array
- description: Secrets to be used with this function/procedure for external access
  name: secrets
  type: object
- description: Specifies where Snowflake should write the compiled code for inline procedures
  name: target_path
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/procedure-java-function-schema.json
slug: procedure-java-function
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JavaFunction\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"external_access_integrations\": {\n      \"type\": \"array\",\n      \"description\": \"List of external access integrations attached to this function/procedure\"\n    },\n    \"secrets\": {\n      \"type\": \"object\",\n      \"description\": \"Secrets to be used with this function/procedure for external access\"\n    },\n    \"target_path\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies where Snowflake should write the compiled code for inline procedures\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/procedure-java-function-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: JavaFunction
---
