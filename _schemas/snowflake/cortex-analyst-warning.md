---
description: Represents a warning within a chat.
layout: schema
name: Warning
properties_list:
- description: A human-readable message describing the warning
  name: message
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-analyst-warning-schema.json
slug: cortex-analyst-warning
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Warning\",\n  \"type\": \"object\",\n  \"description\": \"Represents a warning within a chat.\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable message describing the warning\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-analyst-warning-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Warning
---
