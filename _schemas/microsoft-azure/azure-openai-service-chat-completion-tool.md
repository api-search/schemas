---
description: A tool the model may call.
layout: schema
name: ChatCompletionTool
properties_list:
- description: The type of the tool.
  name: type
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-openai-service-chat-completion-tool-schema.json
slug: azure-openai-service-chat-completion-tool
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChatCompletionTool\",\n  \"type\": \"object\",\n  \"description\": \"A tool the model may call.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the tool.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-openai-service-chat-completion-tool-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: ChatCompletionTool
---
