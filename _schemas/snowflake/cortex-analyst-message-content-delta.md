---
description: ''
layout: schema
name: MessageContentDelta
properties_list:
- description: ''
  name: type
  type: string
- description: The index of the content array this delta object represents
  name: index
  type: integer
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-analyst-message-content-delta-schema.json
slug: cortex-analyst-message-content-delta
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MessageContentDelta\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"index\": {\n      \"type\": \"integer\",\n      \"description\": \"The index of the content array this delta object represents\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-analyst-message-content-delta-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: MessageContentDelta
---
