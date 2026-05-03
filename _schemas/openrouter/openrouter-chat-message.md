---
description: A single message exchanged in an OpenRouter chat completion request or response, compatible with the OpenAI chat completions schema.
layout: schema
name: OpenRouter Chat Message
properties_list:
- description: The role of the message author.
  name: role
  type: string
- description: Message content as a plain string or array of content parts.
  name: content
  type: object
- description: Optional name of the message author.
  name: name
  type: string
- description: When role is tool, references the tool call this message responds to.
  name: tool_call_id
  type: string
- description: ''
  name: tool_calls
  type: array
provider_name: OpenRouter
provider_slug: openrouter
schema_file: json-schema/openrouter-chat-message-schema.json
slug: openrouter-chat-message
source_filename: openrouter-chat-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/openrouter/refs/heads/main/json-schema/openrouter-chat-message-schema.json\",\n  \"title\": \"OpenRouter Chat Message\",\n  \"description\": \"A single message exchanged in an OpenRouter chat completion request or response, compatible with the OpenAI chat completions schema.\",\n  \"type\": \"object\",\n  \"required\": [\"role\"],\n  \"properties\": {\n    \"role\": {\n      \"type\": \"string\",\n      \"enum\": [\"system\", \"user\", \"assistant\", \"tool\"],\n      \"description\": \"The role of the message author.\"\n    },\n    \"content\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"enum\": [\"text\", \"image_url\"\
  ]\n              },\n              \"text\": { \"type\": \"string\" },\n              \"image_url\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"url\": { \"type\": \"string\", \"format\": \"uri\" }\n                }\n              }\n            },\n            \"required\": [\"type\"]\n          }\n        }\n      ],\n      \"description\": \"Message content as a plain string or array of content parts.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Optional name of the message author.\"\n    },\n    \"tool_call_id\": {\n      \"type\": \"string\",\n      \"description\": \"When role is tool, references the tool call this message responds to.\"\n    },\n    \"tool_calls\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"string\" },\n          \"type\": { \"type\": \"string\", \"enum\": [\"function\"] },\n\
  \          \"function\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": { \"type\": \"string\" },\n              \"arguments\": { \"type\": \"string\" }\n            },\n            \"required\": [\"name\", \"arguments\"]\n          }\n        },\n        \"required\": [\"id\", \"type\", \"function\"]\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openrouter/refs/heads/main/json-schema/openrouter-chat-message-schema.json
tags:
- Artificial Intelligence
- Gateway
- Large Language Models
- Router
title: OpenRouter Chat Message
---
