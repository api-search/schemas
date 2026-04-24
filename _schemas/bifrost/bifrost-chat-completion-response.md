---
description: Response from a chat completion request.
layout: schema
name: ChatCompletionResponse
properties_list:
- description: Unique identifier for the completion.
  name: id
  type: string
- description: Object type, always chat.completion.
  name: object
  type: string
- description: Unix timestamp of when the completion was created.
  name: created
  type: integer
- description: Provider and model used for the completion.
  name: model
  type: string
- description: Array of completion choices.
  name: choices
  type: array
- description: ''
  name: usage
  type: object
provider_name: Bifrost
provider_slug: bifrost
schema_file: json-schema/bifrost-chat-completion-response-schema.json
slug: bifrost-chat-completion-response
tags:
- AI Gateway
- LLM
- Load Balancing
- Open Source
- OpenAI Compatible
- MCP
title: ChatCompletionResponse
---
