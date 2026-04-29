---
description: Token usage statistics for the completion.
layout: schema
name: UsageStats
properties_list:
- description: Number of tokens in the prompt.
  name: prompt_tokens
  type: integer
- description: Number of tokens generated.
  name: completion_tokens
  type: integer
- description: Total tokens used.
  name: total_tokens
  type: integer
provider_name: Bifrost
provider_slug: bifrost
schema_file: json-schema/bifrost-usage-stats-schema.json
slug: bifrost-usage-stats
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"UsageStats\",\n  \"type\": \"object\",\n  \"description\": \"Token usage statistics for the completion.\",\n  \"properties\": {\n    \"prompt_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of tokens in the prompt.\",\n      \"example\": 12\n    },\n    \"completion_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of tokens generated.\",\n      \"example\": 14\n    },\n    \"total_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"Total tokens used.\",\n      \"example\": 26\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bifrost/refs/heads/main/json-schema/bifrost-usage-stats-schema.json
tags:
- AI Gateway
- LLM
- Load Balancing
- Open Source
- OpenAI Compatible
- MCP
title: UsageStats
---
