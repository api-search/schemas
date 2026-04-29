---
description: ''
layout: schema
name: FunctionDefinition
properties_list:
- description: The name of the function to be called. Must be a-z, A-Z, 0-9, or contain underscores and dashes, with a maximum length of 64.
  name: name
  type: string
- description: A description of what the function does, used by the model to choose when and how to call the function.
  name: description
  type: string
- description: The parameters the functions accepts, described as a JSON Schema object. Omitting parameters defines a function with an empty parameter list.
  name: parameters
  type: object
- description: Whether to enable strict schema adherence when generating the function call. When set to true, the model will always follow the exact schema defined in the parameters field.
  name: strict
  type: boolean
provider_name: ChatGPT
provider_slug: chatgpt
schema_file: json-schema/chatgpt-chat-completions-function-definition-schema.json
slug: chatgpt-chat-completions-function-definition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FunctionDefinition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the function to be called. Must be a-z, A-Z,\\n0-9, or contain underscores and dashes, with a maximum\\nlength of 64.\\n\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of what the function does, used by the model\\nto choose when and how to call the function.\\n\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"description\": \"The parameters the functions accepts, described as a JSON\\nSchema object. Omitting parameters defines a function with\\nan empty parameter list.\\n\"\n    },\n    \"strict\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable strict schema adherence when generating\\nthe function call. When set to true, the model will\
  \ always\\nfollow the exact schema defined in the parameters field.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chatgpt/refs/heads/main/json-schema/chatgpt-chat-completions-function-definition-schema.json
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
title: FunctionDefinition
---
