---
description: ''
layout: schema
name: TokenInfo
properties_list:
- description: ''
  name: token
  type: string
- description: ''
  name: expiration_seconds
  type: integer
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-analyst-token-info-schema.json
slug: cortex-analyst-token-info
source_filename: cortex-analyst-token-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TokenInfo\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\"\n    },\n    \"expiration_seconds\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-analyst-token-info-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: TokenInfo
---
