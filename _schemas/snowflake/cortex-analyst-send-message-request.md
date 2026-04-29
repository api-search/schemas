---
description: The request object for sendMessage requests
layout: schema
name: SendMessageRequest
properties_list:
- description: The path to a file stored in a Snowflake Stage holding the semantic model yaml. Must be a fully qualified stage url
  name: semantic_model_file
  type: string
- description: A string containing the entire semantic model yaml
  name: semantic_model
  type: string
- description: The name of the Snowflake native semantic model object
  name: semantic_view
  type: string
- description: A list of semantic model objects. If set, other semantic model properties are ignored
  name: semantic_models
  type: array
- description: Whether to stream the response or not
  name: stream
  type: boolean
- description: Whether to response with SQL or natural language. One of 'sql_generation' or 'answer_generation'
  name: operation
  type: string
- description: Warehouse name to use for result set handling. Only used when 'operation' is 'answer_generation'
  name: warehouse
  type: string
- description: ''
  name: messages
  type: array
- description: an optional field to specify the source of the request. e.g "eval", "prod"
  name: source
  type: string
- description: JSON serialized string of experimental API fields (undocumented).
  name: experimental
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-analyst-send-message-request-schema.json
slug: cortex-analyst-send-message-request
source_filename: cortex-analyst-send-message-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SendMessageRequest\",\n  \"type\": \"object\",\n  \"description\": \"The request object for sendMessage requests\",\n  \"properties\": {\n    \"semantic_model_file\": {\n      \"type\": \"string\",\n      \"description\": \"The path to a file stored in a Snowflake Stage holding the semantic model yaml. Must be a fully qualified stage url\"\n    },\n    \"semantic_model\": {\n      \"type\": \"string\",\n      \"description\": \"A string containing the entire semantic model yaml\"\n    },\n    \"semantic_view\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Snowflake native semantic model object\"\n    },\n    \"semantic_models\": {\n      \"type\": \"array\",\n      \"description\": \"A list of semantic model objects. If set, other semantic model properties are ignored\"\n    },\n    \"stream\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to stream\
  \ the response or not\"\n    },\n    \"operation\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to response with SQL or natural language. One of 'sql_generation' or 'answer_generation'\"\n    },\n    \"warehouse\": {\n      \"type\": \"string\",\n      \"description\": \"Warehouse name to use for result set handling. Only used when 'operation' is 'answer_generation'\"\n    },\n    \"messages\": {\n      \"type\": \"array\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"an optional field to specify the source of the request. e.g \\\"eval\\\", \\\"prod\\\"\"\n    },\n    \"experimental\": {\n      \"type\": \"string\",\n      \"description\": \"JSON serialized string of experimental API fields (undocumented).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-analyst-send-message-request-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: SendMessageRequest
---
