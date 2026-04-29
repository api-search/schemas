---
description: The non-streaming response object for the VQ Suggestions request
layout: schema
name: GenerateVerifiedQuerySuggestionsResponse
properties_list:
- description: Unique request ID
  name: request_id
  type: string
- description: ''
  name: vq_suggestions
  type: array
- description: ''
  name: warnings
  type: array
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-analyst-generate-verified-query-suggestions-response-schema.json
slug: cortex-analyst-generate-verified-query-suggestions-response
source_filename: cortex-analyst-generate-verified-query-suggestions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GenerateVerifiedQuerySuggestionsResponse\",\n  \"type\": \"object\",\n  \"description\": \"The non-streaming response object for the VQ Suggestions request\",\n  \"properties\": {\n    \"request_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique request ID\"\n    },\n    \"vq_suggestions\": {\n      \"type\": \"array\"\n    },\n    \"warnings\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-analyst-generate-verified-query-suggestions-response-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: GenerateVerifiedQuerySuggestionsResponse
---
