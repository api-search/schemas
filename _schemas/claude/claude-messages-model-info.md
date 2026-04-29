---
description: Metadata about a Claude model.
layout: schema
name: ModelInfo
properties_list:
- description: Unique model identifier.
  name: id
  type: string
- description: Object type. Always "model" for model objects.
  name: type
  type: string
- description: A human-readable name for the model.
  name: display_name
  type: string
- description: RFC 3339 datetime string representing when the model was released.
  name: created_at
  type: string
provider_name: Claude
provider_slug: claude
schema_file: json-schema/claude-messages-model-info-schema.json
slug: claude-messages-model-info
source_filename: claude-messages-model-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ModelInfo\",\n  \"type\": \"object\",\n  \"description\": \"Metadata about a Claude model.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique model identifier.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Object type. Always \\\"model\\\" for model objects.\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable name for the model.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"RFC 3339 datetime string representing when the model was released.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/json-schema/claude-messages-model-info-schema.json
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
title: ModelInfo
---
