---
description: Represents a Cohere model with its capabilities, supported endpoints, context length, and configuration details.
layout: schema
name: Cohere Model
properties_list:
- description: The unique name of the model for use in API requests.
  name: name
  type: string
- description: The API endpoints the model is compatible with.
  name: endpoints
  type: array
- description: The maximum number of tokens the model can process in a single request.
  name: context_length
  type: integer
- description: The URL for the model's tokenizer configuration file.
  name: tokenizer_url
  type: string
- description: The API endpoints for which this model is the default selection.
  name: default_endpoints
  type: array
- description: Indicates whether the model is a fine-tuned variant of a base model.
  name: finetuned
  type: boolean
provider_name: cohere
provider_slug: cohere
schema_file: json-schema/cohere-model-schema.json
slug: cohere-model
source_filename: cohere-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.cohere.com/schemas/cohere/model.json\",\n  \"title\": \"Cohere Model\",\n  \"description\": \"Represents a Cohere model with its capabilities, supported endpoints, context length, and configuration details.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The unique name of the model for use in API requests.\"\n    },\n    \"endpoints\": {\n      \"type\": \"array\",\n      \"description\": \"The API endpoints the model is compatible with.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"chat\", \"embed\", \"rerank\", \"classify\"]\n      }\n    },\n    \"context_length\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of tokens the model can process in a single request.\",\n      \"minimum\": 1\n    },\n    \"tokenizer_url\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL for the model's tokenizer configuration file.\"\n    },\n    \"default_endpoints\": {\n      \"type\": \"array\",\n      \"description\": \"The API endpoints for which this model is the default selection.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"chat\", \"embed\", \"rerank\", \"classify\"]\n      }\n    },\n    \"finetuned\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the model is a fine-tuned variant of a base model.\"\n    }\n  },\n  \"$defs\": {\n    \"ModelFamily\": {\n      \"type\": \"string\",\n      \"description\": \"The family of Cohere models that a specific model belongs to.\",\n      \"enum\": [\n        \"command\",\n        \"command-r\",\n        \"command-r-plus\",\n        \"embed-english\",\n        \"embed-multilingual\",\n        \"rerank-english\",\n        \"rerank-multilingual\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cohere/refs/heads/main/json-schema/cohere-model-schema.json
tags: []
title: Cohere Model
---
