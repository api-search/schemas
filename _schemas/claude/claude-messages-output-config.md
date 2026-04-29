---
description: Configuration for structured output format.
layout: schema
name: OutputConfig
properties_list:
- description: The output format type.
  name: type
  type: string
- description: JSON Schema defining the expected output structure.
  name: schema
  type: object
provider_name: Claude
provider_slug: claude
schema_file: json-schema/claude-messages-output-config-schema.json
slug: claude-messages-output-config
source_filename: claude-messages-output-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OutputConfig\",\n  \"type\": \"object\",\n  \"description\": \"Configuration for structured output format.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The output format type.\"\n    },\n    \"schema\": {\n      \"type\": \"object\",\n      \"description\": \"JSON Schema defining the expected output structure.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/json-schema/claude-messages-output-config-schema.json
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
title: OutputConfig
---
