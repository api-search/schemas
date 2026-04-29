---
description: Request body for creating a chat completion.
layout: schema
name: CreateChatCompletionRequest
properties_list:
- description: A list of messages comprising the conversation so far.
  name: messages
  type: array
- description: Sampling temperature between 0 and 2. Higher values make the output more random, while lower values make it more focused and deterministic.
  name: temperature
  type: number
- description: An alternative to sampling with temperature called nucleus sampling.
  name: top_p
  type: number
- description: How many chat completion choices to generate for each input message.
  name: n
  type: integer
- description: If set, partial message deltas will be sent as server-sent events.
  name: stream
  type: boolean
- description: Up to 4 sequences where the API will stop generating further tokens.
  name: stop
  type: string
- description: The maximum number of tokens that can be generated in the chat completion.
  name: max_tokens
  type: integer
- description: Positive values penalize new tokens based on whether they appear in the text so far.
  name: presence_penalty
  type: number
- description: Positive values penalize new tokens based on their existing frequency in the text so far.
  name: frequency_penalty
  type: number
- description: An object specifying the format that the model must output.
  name: response_format
  type: object
- description: If specified, the system will make a best effort to sample deterministically.
  name: seed
  type: integer
- description: A list of tools the model may call.
  name: tools
  type: array
- description: Controls which (if any) tool is called by the model.
  name: tool_choice
  type: string
- description: A unique identifier representing your end-user.
  name: user
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-openai-service-create-chat-completion-request-schema.json
slug: azure-openai-service-create-chat-completion-request
source_filename: azure-openai-service-create-chat-completion-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateChatCompletionRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a chat completion.\",\n  \"properties\": {\n    \"messages\": {\n      \"type\": \"array\",\n      \"description\": \"A list of messages comprising the conversation so far.\"\n    },\n    \"temperature\": {\n      \"type\": \"number\",\n      \"description\": \"Sampling temperature between 0 and 2. Higher values make the output more random, while lower values make it more focused and deterministic.\"\n    },\n    \"top_p\": {\n      \"type\": \"number\",\n      \"description\": \"An alternative to sampling with temperature called nucleus sampling.\"\n    },\n    \"n\": {\n      \"type\": \"integer\",\n      \"description\": \"How many chat completion choices to generate for each input message.\"\n    },\n    \"stream\": {\n      \"type\": \"boolean\",\n      \"description\": \"If set, partial\
  \ message deltas will be sent as server-sent events.\"\n    },\n    \"stop\": {\n      \"type\": \"string\",\n      \"description\": \"Up to 4 sequences where the API will stop generating further tokens.\"\n    },\n    \"max_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of tokens that can be generated in the chat completion.\"\n    },\n    \"presence_penalty\": {\n      \"type\": \"number\",\n      \"description\": \"Positive values penalize new tokens based on whether they appear in the text so far.\"\n    },\n    \"frequency_penalty\": {\n      \"type\": \"number\",\n      \"description\": \"Positive values penalize new tokens based on their existing frequency in the text so far.\"\n    },\n    \"response_format\": {\n      \"type\": \"object\",\n      \"description\": \"An object specifying the format that the model must output.\"\n    },\n    \"seed\": {\n      \"type\": \"integer\",\n      \"description\": \"If specified, the system will make\
  \ a best effort to sample deterministically.\"\n    },\n    \"tools\": {\n      \"type\": \"array\",\n      \"description\": \"A list of tools the model may call.\"\n    },\n    \"tool_choice\": {\n      \"type\": \"string\",\n      \"description\": \"Controls which (if any) tool is called by the model.\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier representing your end-user.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-openai-service-create-chat-completion-request-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: CreateChatCompletionRequest
---
