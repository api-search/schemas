---
description: ''
layout: schema
name: CompletionUsage
properties_list:
- description: Number of tokens in the prompt.
  name: prompt_tokens
  type: integer
- description: Number of tokens in the generated completion.
  name: completion_tokens
  type: integer
- description: Total number of tokens used in the request (prompt + completion).
  name: total_tokens
  type: integer
- description: Breakdown of completion tokens.
  name: completion_tokens_details
  type: object
- description: Breakdown of prompt tokens.
  name: prompt_tokens_details
  type: object
provider_name: OpenAI
provider_slug: openai
schema_file: json-schema/openai-chat-completions-completion-usage-schema.json
slug: openai-chat-completions-completion-usage
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompletionUsage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"prompt_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of tokens in the prompt.\"\n    },\n    \"completion_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of tokens in the generated completion.\"\n    },\n    \"total_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of tokens used in the request (prompt + completion).\"\n    },\n    \"completion_tokens_details\": {\n      \"type\": \"object\",\n      \"description\": \"Breakdown of completion tokens.\"\n    },\n    \"prompt_tokens_details\": {\n      \"type\": \"object\",\n      \"description\": \"Breakdown of prompt tokens.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/json-schema/openai-chat-completions-completion-usage-schema.json
tags:
- AI
- Artificial Intelligence
- Large Language Models
- T1
title: CompletionUsage
---
