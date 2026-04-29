---
description: ''
layout: schema
name: ChatCompletionChoice
properties_list:
- description: The index of the choice in the list.
  name: index
  type: integer
- description: 'The reason the model stopped generating tokens. stop means the model hit a natural stop point or a provided stop sequence. length means the maximum token limit was reached. tool_calls means the model '
  name: finish_reason
  type: string
- description: Log probability information for the choice.
  name: logprobs
  type: object
provider_name: ChatGPT
provider_slug: chatgpt
schema_file: json-schema/chatgpt-chat-completions-chat-completion-choice-schema.json
slug: chatgpt-chat-completions-chat-completion-choice
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChatCompletionChoice\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"index\": {\n      \"type\": \"integer\",\n      \"description\": \"The index of the choice in the list.\"\n    },\n    \"finish_reason\": {\n      \"type\": \"string\",\n      \"description\": \"The reason the model stopped generating tokens. stop means\\nthe model hit a natural stop point or a provided stop\\nsequence. length means the maximum token limit was reached.\\ntool_calls means the model called a tool. content_filter\\nmeans content was omitted due to a flag from content filters.\\n\"\n    },\n    \"logprobs\": {\n      \"type\": \"object\",\n      \"description\": \"Log probability information for the choice.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chatgpt/refs/heads/main/json-schema/chatgpt-chat-completions-chat-completion-choice-schema.json
tags:
- Agents
- AI
- ChatGPT
- Embeddings
- Fine-Tuning
- GPT-4
- GPT-5
- Language Model
- OpenAI
- Realtime
title: ChatCompletionChoice
---
