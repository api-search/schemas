---
description: Confirmation of a deleted message batch.
layout: schema
name: DeletedMessageBatch
properties_list:
- description: The ID of the deleted batch.
  name: id
  type: string
- description: ''
  name: type
  type: string
provider_name: Claude
provider_slug: claude
schema_file: json-schema/claude-messages-deleted-message-batch-schema.json
slug: claude-messages-deleted-message-batch
source_filename: claude-messages-deleted-message-batch-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeletedMessageBatch\",\n  \"type\": \"object\",\n  \"description\": \"Confirmation of a deleted message batch.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the deleted batch.\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/json-schema/claude-messages-deleted-message-batch-schema.json
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
title: DeletedMessageBatch
---
