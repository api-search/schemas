---
description: A single result from a message batch.
layout: schema
name: MessageBatchResult
properties_list:
- description: The developer-provided custom_id from the original request.
  name: custom_id
  type: string
- description: The result of the request.
  name: result
  type: object
provider_name: Claude
provider_slug: claude
schema_file: json-schema/claude-messages-message-batch-result-schema.json
slug: claude-messages-message-batch-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MessageBatchResult\",\n  \"type\": \"object\",\n  \"description\": \"A single result from a message batch.\",\n  \"properties\": {\n    \"custom_id\": {\n      \"type\": \"string\",\n      \"description\": \"The developer-provided custom_id from the original request.\"\n    },\n    \"result\": {\n      \"type\": \"object\",\n      \"description\": \"The result of the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/json-schema/claude-messages-message-batch-result-schema.json
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
title: MessageBatchResult
---
