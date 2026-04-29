---
description: ''
layout: schema
name: CreateMessageBatchRequest
properties_list:
- description: Array of batch request objects. Each contains a custom_id and params.
  name: requests
  type: array
provider_name: Claude
provider_slug: claude
schema_file: json-schema/claude-messages-create-message-batch-request-schema.json
slug: claude-messages-create-message-batch-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateMessageBatchRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requests\": {\n      \"type\": \"array\",\n      \"description\": \"Array of batch request objects. Each contains a custom_id and params.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/json-schema/claude-messages-create-message-batch-request-schema.json
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
title: CreateMessageBatchRequest
---
