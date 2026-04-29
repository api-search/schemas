---
description: A tool use content block in a response, indicating the model wants to use a tool.
layout: schema
name: ToolUseBlock
properties_list:
- description: ''
  name: type
  type: string
- description: A unique identifier for this particular tool use block. Used to match tool results to tool use requests.
  name: id
  type: string
- description: The name of the tool being used.
  name: name
  type: string
- description: An object containing the input passed to the tool, conforming to the tool's input_schema.
  name: input
  type: object
provider_name: Claude
provider_slug: claude
schema_file: json-schema/claude-messages-tool-use-block-schema.json
slug: claude-messages-tool-use-block
source_filename: claude-messages-tool-use-block-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ToolUseBlock\",\n  \"type\": \"object\",\n  \"description\": \"A tool use content block in a response, indicating the model wants to use a tool.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for this particular tool use block. Used to match tool results to tool use requests.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the tool being used.\"\n    },\n    \"input\": {\n      \"type\": \"object\",\n      \"description\": \"An object containing the input passed to the tool, conforming to the tool's input_schema.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/json-schema/claude-messages-tool-use-block-schema.json
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
title: ToolUseBlock
---
