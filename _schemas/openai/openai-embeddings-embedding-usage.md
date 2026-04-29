---
description: ''
layout: schema
name: EmbeddingUsage
properties_list:
- description: The number of tokens in the input.
  name: prompt_tokens
  type: integer
- description: The total number of tokens used.
  name: total_tokens
  type: integer
provider_name: OpenAI
provider_slug: openai
schema_file: json-schema/openai-embeddings-embedding-usage-schema.json
slug: openai-embeddings-embedding-usage
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmbeddingUsage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"prompt_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of tokens in the input.\"\n    },\n    \"total_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of tokens used.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/json-schema/openai-embeddings-embedding-usage-schema.json
tags:
- AI
- Artificial Intelligence
- Large Language Models
- T1
title: EmbeddingUsage
---
