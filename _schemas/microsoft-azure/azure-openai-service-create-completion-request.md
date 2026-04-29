---
description: Request body for creating a text completion.
layout: schema
name: CreateCompletionRequest
properties_list:
- description: The prompt(s) to generate completions for.
  name: prompt
  type: string
- description: The maximum number of tokens that can be generated.
  name: max_tokens
  type: integer
- description: Sampling temperature to use.
  name: temperature
  type: number
- description: Nucleus sampling parameter.
  name: top_p
  type: number
- description: How many completions to generate for each prompt.
  name: n
  type: integer
- description: Whether to stream back partial progress.
  name: stream
  type: boolean
- description: Up to 4 sequences where the API will stop generating further tokens.
  name: stop
  type: string
- description: Penalizes new tokens based on whether they appear in the text so far.
  name: presence_penalty
  type: number
- description: Penalizes new tokens based on their existing frequency in the text.
  name: frequency_penalty
  type: number
- description: A unique identifier representing your end-user.
  name: user
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-openai-service-create-completion-request-schema.json
slug: azure-openai-service-create-completion-request
source_filename: azure-openai-service-create-completion-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateCompletionRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a text completion.\",\n  \"properties\": {\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"The prompt(s) to generate completions for.\"\n    },\n    \"max_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of tokens that can be generated.\"\n    },\n    \"temperature\": {\n      \"type\": \"number\",\n      \"description\": \"Sampling temperature to use.\"\n    },\n    \"top_p\": {\n      \"type\": \"number\",\n      \"description\": \"Nucleus sampling parameter.\"\n    },\n    \"n\": {\n      \"type\": \"integer\",\n      \"description\": \"How many completions to generate for each prompt.\"\n    },\n    \"stream\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to stream back partial progress.\"\n    },\n    \"\
  stop\": {\n      \"type\": \"string\",\n      \"description\": \"Up to 4 sequences where the API will stop generating further tokens.\"\n    },\n    \"presence_penalty\": {\n      \"type\": \"number\",\n      \"description\": \"Penalizes new tokens based on whether they appear in the text so far.\"\n    },\n    \"frequency_penalty\": {\n      \"type\": \"number\",\n      \"description\": \"Penalizes new tokens based on their existing frequency in the text.\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier representing your end-user.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-openai-service-create-completion-request-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: CreateCompletionRequest
---
