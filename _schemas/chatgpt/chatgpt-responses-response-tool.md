---
description: ''
layout: schema
name: ResponseTool
properties_list:
- description: The type of the tool.
  name: type
  type: string
- description: The name of the function. Required for function type tools.
  name: name
  type: string
- description: A description of what the function does.
  name: description
  type: string
- description: The parameters the function accepts, described as a JSON Schema object. Required for function type tools.
  name: parameters
  type: object
- description: Whether strict schema adherence is enabled for function tools.
  name: strict
  type: boolean
- description: The IDs of the vector stores to search. Required for file_search type tools.
  name: vector_store_ids
  type: array
- description: The maximum number of results to return from file search.
  name: max_num_results
  type: integer
- description: Ranking options for file search results.
  name: ranking_options
  type: object
- description: The container for the code interpreter tool. Specifies the sandbox environment.
  name: container
  type: object
- description: The width of the computer display in pixels. Required for computer_use_preview type.
  name: display_width
  type: integer
- description: The height of the computer display in pixels. Required for computer_use_preview type.
  name: display_height
  type: integer
- description: The environment of the computer. Required for computer_use_preview type.
  name: environment
  type: string
- description: A label for the MCP server. Required for mcp type tools.
  name: server_label
  type: string
- description: The URL of the MCP server. Required for mcp type tools.
  name: server_url
  type: string
- description: The list of allowed tool names from the MCP server.
  name: allowed_tools
  type: array
- description: Headers to pass to the MCP server for authentication.
  name: headers
  type: object
provider_name: ChatGPT
provider_slug: chatgpt
schema_file: json-schema/chatgpt-responses-response-tool-schema.json
slug: chatgpt-responses-response-tool
source_filename: chatgpt-responses-response-tool-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResponseTool\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the tool.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the function. Required for function type tools.\\n\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of what the function does.\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"description\": \"The parameters the function accepts, described as a JSON\\nSchema object. Required for function type tools.\\n\"\n    },\n    \"strict\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether strict schema adherence is enabled for function tools.\\n\"\n    },\n    \"vector_store_ids\": {\n      \"type\": \"array\",\n      \"description\": \"The IDs of the vector stores to\
  \ search. Required for\\nfile_search type tools.\\n\"\n    },\n    \"max_num_results\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of results to return from file search.\\n\"\n    },\n    \"ranking_options\": {\n      \"type\": \"object\",\n      \"description\": \"Ranking options for file search results.\"\n    },\n    \"container\": {\n      \"type\": \"object\",\n      \"description\": \"The container for the code interpreter tool. Specifies\\nthe sandbox environment.\\n\"\n    },\n    \"display_width\": {\n      \"type\": \"integer\",\n      \"description\": \"The width of the computer display in pixels. Required\\nfor computer_use_preview type.\\n\"\n    },\n    \"display_height\": {\n      \"type\": \"integer\",\n      \"description\": \"The height of the computer display in pixels. Required\\nfor computer_use_preview type.\\n\"\n    },\n    \"environment\": {\n      \"type\": \"string\",\n      \"description\": \"The environment of the computer.\
  \ Required for\\ncomputer_use_preview type.\\n\"\n    },\n    \"server_label\": {\n      \"type\": \"string\",\n      \"description\": \"A label for the MCP server. Required for mcp type tools.\\n\"\n    },\n    \"server_url\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of the MCP server. Required for mcp type tools.\\n\"\n    },\n    \"allowed_tools\": {\n      \"type\": \"array\",\n      \"description\": \"The list of allowed tool names from the MCP server.\\n\"\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"description\": \"Headers to pass to the MCP server for authentication.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chatgpt/refs/heads/main/json-schema/chatgpt-responses-response-tool-schema.json
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
title: ResponseTool
---
