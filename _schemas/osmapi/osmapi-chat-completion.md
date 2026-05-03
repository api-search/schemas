---
description: Schema for an osmAPI chat completion response object
layout: schema
name: osmAPI Chat Completion Response
properties_list:
- description: Unique identifier for the completion
  name: id
  type: string
- description: Object type identifier
  name: object
  type: string
- description: Unix timestamp of creation
  name: created
  type: integer
- description: Model used for the completion
  name: model
  type: string
- description: ''
  name: choices
  type: array
- description: ''
  name: usage
  type: object
- description: ''
  name: metadata
  type: object
provider_name: osmAPI
provider_slug: osmapi
schema_file: json-schema/osmapi-chat-completion-schema.json
slug: osmapi-chat-completion
source_filename: osmapi-chat-completion-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/osmapi/refs/heads/main/json-schema/osmapi-chat-completion-schema.json\",\n  \"title\": \"osmAPI Chat Completion Response\",\n  \"description\": \"Schema for an osmAPI chat completion response object\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the completion\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"description\": \"Object type identifier\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of creation\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Model used for the completion\"\n    },\n    \"choices\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"index\": {\n       \
  \     \"type\": \"integer\"\n          },\n          \"message\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"role\": {\n                \"type\": \"string\"\n              },\n              \"content\": {\n                \"type\": \"string\"\n              },\n              \"reasoning\": {\n                \"type\": \"string\"\n              },\n              \"tool_calls\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\"\n                }\n              },\n              \"images\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          },\n          \"finish_reason\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"usage\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"prompt_tokens\": {\n          \"type\"\
  : \"integer\"\n        },\n        \"completion_tokens\": {\n          \"type\": \"integer\"\n        },\n        \"total_tokens\": {\n          \"type\": \"integer\"\n        },\n        \"reasoning_tokens\": {\n          \"type\": \"integer\"\n        },\n        \"cost_usd_total\": {\n          \"type\": \"number\"\n        },\n        \"cost_usd_input\": {\n          \"type\": \"number\"\n        },\n        \"cost_usd_output\": {\n          \"type\": \"number\"\n        }\n      }\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"requested_model\": {\n          \"type\": \"string\"\n        },\n        \"used_model\": {\n          \"type\": \"string\"\n        },\n        \"used_provider\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/osmapi/refs/heads/main/json-schema/osmapi-chat-completion-schema.json
tags:
- AI
- Anthropic
- Gateway
- LLM
- OpenAI
- Routing
title: osmAPI Chat Completion Response
---
