---
description: Request body for creating a chat completion.
layout: schema
name: ChatCompletionRequest
properties_list:
- description: Provider and model name in the format provider/model-name (e.g., openai/gpt-4o, anthropic/claude-3-5-sonnet-20241022).
  name: model
  type: string
- description: Array of messages comprising the conversation.
  name: messages
  type: array
- description: Sampling temperature between 0 and 2.
  name: temperature
  type: number
- description: Maximum number of tokens to generate.
  name: max_tokens
  type: integer
- description: Whether to stream the response as SSE.
  name: stream
  type: boolean
- description: Nucleus sampling probability.
  name: top_p
  type: number
- description: Number of completions to generate.
  name: n
  type: integer
provider_name: Bifrost
provider_slug: bifrost
schema_file: json-schema/bifrost-chat-completion-request-schema.json
slug: bifrost-chat-completion-request
tags:
- AI Gateway
- LLM
- Load Balancing
- Open Source
- OpenAI Compatible
- MCP
title: ChatCompletionRequest
---
