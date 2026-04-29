---
description: A single request within a message batch.
layout: schema
name: BatchRequestItem
properties_list:
- description: Developer-provided identifier for this request. Must be unique within the batch. Used to match results to requests.
  name: custom_id
  type: string
provider_name: Claude
provider_slug: claude
schema_file: json-schema/claude-messages-batch-request-item-schema.json
slug: claude-messages-batch-request-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchRequestItem\",\n  \"type\": \"object\",\n  \"description\": \"A single request within a message batch.\",\n  \"properties\": {\n    \"custom_id\": {\n      \"type\": \"string\",\n      \"description\": \"Developer-provided identifier for this request. Must be unique within the batch. Used to match results to requests.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/json-schema/claude-messages-batch-request-item-schema.json
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
title: BatchRequestItem
---
