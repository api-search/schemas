---
description: Schema for an osmAPI model object
layout: schema
name: osmAPI Model
properties_list:
- description: Unique model identifier
  name: id
  type: string
- description: Human-readable model name
  name: name
  type: string
- description: Alternative identifiers for the model
  name: aliases
  type: array
- description: Unix timestamp of model creation
  name: created
  type: number
- description: Description of the model
  name: description
  type: string
- description: Model family grouping
  name: family
  type: string
- description: ''
  name: architecture
  type: object
- description: ''
  name: top_provider
  type: object
- description: ''
  name: providers
  type: array
- description: ''
  name: pricing
  type: object
- description: Maximum context window size in tokens
  name: context_length
  type: integer
- description: ''
  name: per_request_limits
  type: object
- description: ''
  name: supported_parameters
  type: array
- description: ''
  name: json_output
  type: boolean
- description: ''
  name: structured_outputs
  type: boolean
- description: ''
  name: free
  type: boolean
- description: ''
  name: deprecated_at
  type: string
- description: ''
  name: deactivated_at
  type: string
- description: ''
  name: stability
  type: string
provider_name: osmAPI
provider_slug: osmapi
schema_file: json-schema/osmapi-model-schema.json
slug: osmapi-model
source_filename: osmapi-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/osmapi/refs/heads/main/json-schema/osmapi-model-schema.json\",\n  \"title\": \"osmAPI Model\",\n  \"description\": \"Schema for an osmAPI model object\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique model identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable model name\"\n    },\n    \"aliases\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Alternative identifiers for the model\"\n    },\n    \"created\": {\n      \"type\": \"number\",\n      \"description\": \"Unix timestamp of model creation\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the model\"\n    },\n    \"family\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Model family grouping\"\n    },\n    \"architecture\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"input_modalities\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"output_modalities\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"tokenizer\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"top_provider\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"is_moderated\": {\n          \"type\": \"boolean\"\n        }\n      }\n    },\n    \"providers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"pricing\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"prompt\": {\n          \"type\": \"string\"\n        },\n        \"completion\": {\n          \"\
  type\": \"string\"\n        },\n        \"image\": {\n          \"type\": \"string\"\n        },\n        \"request\": {\n          \"type\": \"string\"\n        },\n        \"caching\": {\n          \"type\": \"string\"\n        },\n        \"web_search\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"context_length\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum context window size in tokens\"\n    },\n    \"per_request_limits\": {\n      \"type\": \"object\"\n    },\n    \"supported_parameters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"json_output\": {\n      \"type\": \"boolean\"\n    },\n    \"structured_outputs\": {\n      \"type\": \"boolean\"\n    },\n    \"free\": {\n      \"type\": \"boolean\"\n    },\n    \"deprecated_at\": {\n      \"type\": \"string\"\n    },\n    \"deactivated_at\": {\n      \"type\": \"string\"\n    },\n    \"stability\": {\n      \"type\": \"string\"\
  \n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/osmapi/refs/heads/main/json-schema/osmapi-model-schema.json
tags:
- AI
- Anthropic
- Gateway
- LLM
- OpenAI
- Routing
title: osmAPI Model
---
