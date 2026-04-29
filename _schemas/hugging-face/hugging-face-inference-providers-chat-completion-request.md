---
description: ''
layout: schema
name: ChatCompletionRequest
properties_list:
- description: Model ID to use. Can be a Hugging Face model ID (e.g., meta-llama/Llama-3-70b-chat-hf) or a provider-specific identifier.
  name: model
  type: string
- description: List of messages comprising the conversation
  name: messages
  type: array
- description: Penalize tokens based on frequency in text so far
  name: frequency_penalty
  type: number
- description: Whether to return log probabilities
  name: logprobs
  type: boolean
- description: Maximum number of tokens to generate
  name: max_tokens
  type: integer
- description: Penalize tokens based on presence in text so far
  name: presence_penalty
  type: number
- description: Constrains effort on reasoning for models that support it. Common values are none, minimal, low, medium, high, xhigh.
  name: reasoning_effort
  type: string
- description: ''
  name: response_format
  type: string
- description: Random seed for reproducibility
  name: seed
  type: integer
- description: Up to 4 sequences where generation will stop
  name: stop
  type: array
- description: Whether to stream partial responses using SSE
  name: stream
  type: boolean
- description: ''
  name: stream_options
  type: object
- description: Sampling temperature
  name: temperature
  type: number
- description: Controls tool usage
  name: tool_choice
  type: string
- description: Prompt prepended before tools
  name: tool_prompt
  type: string
- description: List of tools the model may call
  name: tools
  type: array
- description: Number of most likely tokens to return per position
  name: top_logprobs
  type: integer
- description: Nucleus sampling parameter
  name: top_p
  type: number
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-providers-chat-completion-request-schema.json
slug: hugging-face-inference-providers-chat-completion-request
source_filename: hugging-face-inference-providers-chat-completion-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChatCompletionRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Model ID to use. Can be a Hugging Face model ID (e.g., meta-llama/Llama-3-70b-chat-hf) or a provider-specific identifier.\"\n    },\n    \"messages\": {\n      \"type\": \"array\",\n      \"description\": \"List of messages comprising the conversation\"\n    },\n    \"frequency_penalty\": {\n      \"type\": \"number\",\n      \"description\": \"Penalize tokens based on frequency in text so far\"\n    },\n    \"logprobs\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to return log probabilities\"\n    },\n    \"max_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of tokens to generate\"\n    },\n    \"presence_penalty\": {\n      \"type\": \"number\",\n      \"description\": \"Penalize tokens based\
  \ on presence in text so far\"\n    },\n    \"reasoning_effort\": {\n      \"type\": \"string\",\n      \"description\": \"Constrains effort on reasoning for models that support it. Common values are none, minimal, low, medium, high, xhigh.\"\n    },\n    \"response_format\": {\n      \"type\": \"string\"\n    },\n    \"seed\": {\n      \"type\": \"integer\",\n      \"description\": \"Random seed for reproducibility\"\n    },\n    \"stop\": {\n      \"type\": \"array\",\n      \"description\": \"Up to 4 sequences where generation will stop\"\n    },\n    \"stream\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to stream partial responses using SSE\"\n    },\n    \"stream_options\": {\n      \"type\": \"object\"\n    },\n    \"temperature\": {\n      \"type\": \"number\",\n      \"description\": \"Sampling temperature\"\n    },\n    \"tool_choice\": {\n      \"type\": \"string\",\n      \"description\": \"Controls tool usage\"\n    },\n    \"tool_prompt\": {\n     \
  \ \"type\": \"string\",\n      \"description\": \"Prompt prepended before tools\"\n    },\n    \"tools\": {\n      \"type\": \"array\",\n      \"description\": \"List of tools the model may call\"\n    },\n    \"top_logprobs\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of most likely tokens to return per position\"\n    },\n    \"top_p\": {\n      \"type\": \"number\",\n      \"description\": \"Nucleus sampling parameter\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-providers-chat-completion-request-schema.json
tags: []
title: ChatCompletionRequest
---
