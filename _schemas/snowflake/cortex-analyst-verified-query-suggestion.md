---
description: A suggestion to add or remove or replace a Verified Query to a semantic model.
layout: schema
name: VerifiedQuerySuggestion
properties_list:
- description: Score of the suggestion, higher is better.
  name: score
  type: number
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-analyst-verified-query-suggestion-schema.json
slug: cortex-analyst-verified-query-suggestion
source_filename: cortex-analyst-verified-query-suggestion-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VerifiedQuerySuggestion\",\n  \"type\": \"object\",\n  \"description\": \"A suggestion to add or remove or replace a Verified Query to a semantic model.\",\n  \"properties\": {\n    \"score\": {\n      \"type\": \"number\",\n      \"description\": \"Score of the suggestion, higher is better.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-analyst-verified-query-suggestion-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: VerifiedQuerySuggestion
---
