---
description: The request object for getting VQ suggestions
layout: schema
name: GenerateVerifiedQuerySuggestionsRequest
properties_list:
- description: Warehouse name to use for processing suggestions.
  name: warehouse
  type: string
- description: JSON serialized string of experimental API fields (undocumented).
  name: experimental
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-analyst-generate-verified-query-suggestions-request-schema.json
slug: cortex-analyst-generate-verified-query-suggestions-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GenerateVerifiedQuerySuggestionsRequest\",\n  \"type\": \"object\",\n  \"description\": \"The request object for getting VQ suggestions\",\n  \"properties\": {\n    \"warehouse\": {\n      \"type\": \"string\",\n      \"description\": \"Warehouse name to use for processing suggestions.\"\n    },\n    \"experimental\": {\n      \"type\": \"string\",\n      \"description\": \"JSON serialized string of experimental API fields (undocumented).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-analyst-generate-verified-query-suggestions-request-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: GenerateVerifiedQuerySuggestionsRequest
---
