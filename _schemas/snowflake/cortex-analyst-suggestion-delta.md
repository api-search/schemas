---
description: ''
layout: schema
name: SuggestionDelta
properties_list:
- description: The index of the suggestions array this delta object represents
  name: index
  type: integer
- description: The delta of a suggestion text, clients should concatenate all deltas for the same index
  name: suggestion_delta
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-analyst-suggestion-delta-schema.json
slug: cortex-analyst-suggestion-delta
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SuggestionDelta\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"index\": {\n      \"type\": \"integer\",\n      \"description\": \"The index of the suggestions array this delta object represents\"\n    },\n    \"suggestion_delta\": {\n      \"type\": \"string\",\n      \"description\": \"The delta of a suggestion text, clients should concatenate all deltas for the same index\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-analyst-suggestion-delta-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: SuggestionDelta
---
