---
description: Represents an AI assistant that can be configured with instructions, tools, and a model to respond to user messages within threads.
layout: schema
name: OpenAI Assistant
properties_list:
- description: The unique identifier of the assistant
  name: id
  type: string
- description: The object type, always assistant
  name: object
  type: string
- description: Unix timestamp of when the assistant was created
  name: created_at
  type: integer
- description: The name of the assistant
  name: name
  type:
  - string
  - 'null'
- description: The description of the assistant
  name: description
  type:
  - string
  - 'null'
- description: ID of the model used by the assistant
  name: model
  type: string
- description: The system instructions that the assistant uses
  name: instructions
  type:
  - string
  - 'null'
- description: List of tools enabled on the assistant
  name: tools
  type: array
- description: Key-value pairs attached to the assistant (max 16 pairs)
  name: metadata
  type: object
- description: Sampling temperature for the assistant
  name: temperature
  type: number
- description: Nucleus sampling parameter
  name: top_p
  type: number
- description: Specifies the format the model must output
  name: response_format
  type: object
provider_name: OpenAI APIs
provider_slug: openai-apis
schema_file: json-schema/openai-assistant-schema.json
slug: openai-assistant
source_filename: openai-assistant-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.openai.com/schemas/openai/assistant.json\",\n  \"title\": \"OpenAI Assistant\",\n  \"description\": \"Represents an AI assistant that can be configured with instructions, tools, and a model to respond to user messages within threads.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the assistant\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"const\": \"assistant\",\n      \"description\": \"The object type, always assistant\"\n    },\n    \"created_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of when the assistant was created\"\n    },\n    \"name\": {\n      \"type\": [\"string\", \"null\"],\n      \"maxLength\": 256,\n      \"description\": \"The name of the assistant\"\n    },\n    \"description\": {\n      \"type\": [\"string\", \"\
  null\"],\n      \"maxLength\": 512,\n      \"description\": \"The description of the assistant\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the model used by the assistant\"\n    },\n    \"instructions\": {\n      \"type\": [\"string\", \"null\"],\n      \"maxLength\": 256000,\n      \"description\": \"The system instructions that the assistant uses\"\n    },\n    \"tools\": {\n      \"type\": \"array\",\n      \"maxItems\": 128,\n      \"items\": {\n        \"$ref\": \"#/$defs/Tool\"\n      },\n      \"description\": \"List of tools enabled on the assistant\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value pairs attached to the assistant (max 16 pairs)\"\n    },\n    \"temperature\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 2,\n      \"description\": \"Sampling temperature for the assistant\"\n    },\n    \"top_p\": {\n      \"type\": \"number\",\n      \"minimum\"\
  : 0,\n      \"maximum\": 1,\n      \"description\": \"Nucleus sampling parameter\"\n    },\n    \"response_format\": {\n      \"description\": \"Specifies the format the model must output\",\n      \"oneOf\": [\n        {\n          \"type\": \"string\",\n          \"const\": \"auto\"\n        },\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"enum\": [\"text\", \"json_object\", \"json_schema\"]\n            }\n          }\n        }\n      ]\n    }\n  },\n  \"required\": [\"id\", \"object\", \"created_at\", \"model\", \"tools\"],\n  \"$defs\": {\n    \"Tool\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"code_interpreter\", \"file_search\", \"function\"],\n          \"description\": \"The type of tool\"\n        },\n        \"function\": {\n          \"type\": \"object\",\n          \"properties\"\
  : {\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"The name of the function\"\n            },\n            \"description\": {\n              \"type\": \"string\",\n              \"description\": \"A description of the function\"\n            },\n            \"parameters\": {\n              \"type\": \"object\",\n              \"description\": \"The parameters as a JSON Schema object\"\n            }\n          },\n          \"description\": \"Function definition (only for function type tools)\"\n        }\n      },\n      \"required\": [\"type\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/json-schema/openai-assistant-schema.json
tags:
- Artificial Intelligence
- Embeddings
- Image Generation
- Language Models
- Speech
title: OpenAI Assistant
---
