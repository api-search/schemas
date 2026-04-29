---
description: Definition of a tool that the model can use.
layout: schema
name: Tool
properties_list:
- description: The name of the tool. Must match the regex ^[a-zA-Z0-9_-]{1,64}$.
  name: name
  type: string
- description: A detailed description of what the tool does, when it should be used, and what each parameter means.
  name: description
  type: string
- description: JSON Schema object defining the expected parameters for the tool.
  name: input_schema
  type: object
- description: The type of tool. Omit for custom tools. Use specific type strings for server tools like web_search_20260209, code_execution_20260120, text_editor_20250728, etc.
  name: type
  type: string
provider_name: Claude
provider_slug: claude
schema_file: json-schema/claude-messages-tool-schema.json
slug: claude-messages-tool
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Tool\",\n  \"type\": \"object\",\n  \"description\": \"Definition of a tool that the model can use.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the tool. Must match the regex ^[a-zA-Z0-9_-]{1,64}$.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A detailed description of what the tool does, when it should be used, and what each parameter means.\"\n    },\n    \"input_schema\": {\n      \"type\": \"object\",\n      \"description\": \"JSON Schema object defining the expected parameters for the tool.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of tool. Omit for custom tools. Use specific type strings for server tools like web_search_20260209, code_execution_20260120, text_editor_20250728, etc.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/json-schema/claude-messages-tool-schema.json
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
title: Tool
---
