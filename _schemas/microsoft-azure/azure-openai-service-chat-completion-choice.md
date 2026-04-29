---
description: A chat completion choice.
layout: schema
name: ChatCompletionChoice
properties_list:
- description: The index of the choice in the list.
  name: index
  type: integer
- description: The reason the model stopped generating tokens.
  name: finish_reason
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-openai-service-chat-completion-choice-schema.json
slug: azure-openai-service-chat-completion-choice
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChatCompletionChoice\",\n  \"type\": \"object\",\n  \"description\": \"A chat completion choice.\",\n  \"properties\": {\n    \"index\": {\n      \"type\": \"integer\",\n      \"description\": \"The index of the choice in the list.\"\n    },\n    \"finish_reason\": {\n      \"type\": \"string\",\n      \"description\": \"The reason the model stopped generating tokens.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-openai-service-chat-completion-choice-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: ChatCompletionChoice
---
