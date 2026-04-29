---
description: Token usage information for the request.
layout: schema
name: Usage
properties_list:
- description: The number of input tokens consumed.
  name: input_tokens
  type: integer
- description: The number of output tokens generated.
  name: output_tokens
  type: integer
- description: The number of input tokens used to create a cache entry.
  name: cache_creation_input_tokens
  type: integer
- description: The number of input tokens read from cache.
  name: cache_read_input_tokens
  type: integer
provider_name: Claude
provider_slug: claude
schema_file: json-schema/claude-messages-usage-schema.json
slug: claude-messages-usage
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Usage\",\n  \"type\": \"object\",\n  \"description\": \"Token usage information for the request.\",\n  \"properties\": {\n    \"input_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of input tokens consumed.\"\n    },\n    \"output_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of output tokens generated.\"\n    },\n    \"cache_creation_input_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of input tokens used to create a cache entry.\"\n    },\n    \"cache_read_input_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of input tokens read from cache.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/json-schema/claude-messages-usage-schema.json
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
title: Usage
---
