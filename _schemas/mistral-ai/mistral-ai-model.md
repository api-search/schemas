---
description: Schema for a Mistral AI model object, representing a base or fine-tuned language model with its capabilities and metadata.
layout: schema
name: Mistral AI Model
properties_list:
- description: The unique model identifier used in API requests.
  name: id
  type: string
- description: The object type, always model.
  name: object
  type: string
- description: Unix timestamp when the model was created.
  name: created
  type: integer
- description: The organization that owns the model.
  name: owned_by
  type: string
- description: The human-readable display name of the model.
  name: name
  type: string
- description: A description of the model and its intended use cases.
  name: description
  type: string
- description: Maximum context length in tokens supported by the model.
  name: max_context_length
  type: integer
- description: Alternative identifiers that can be used to reference the model.
  name: aliases
  type: array
- description: The deprecation date of the model, if scheduled.
  name: deprecation
  type: string
- description: ''
  name: capabilities
  type: object
- description: Whether this is a base model or a fine-tuned model.
  name: type
  type: string
provider_name: Mistral AI
provider_slug: mistral-ai
schema_file: json-schema/mistral-ai-model-schema.json
slug: mistral-ai-model
source_filename: mistral-ai-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://mistral.ai/schemas/mistral-ai/model.json\",\n  \"title\": \"Mistral AI Model\",\n  \"description\": \"Schema for a Mistral AI model object, representing a base or fine-tuned language model with its capabilities and metadata.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"object\"],\n  \"$defs\": {\n    \"ModelCapabilities\": {\n      \"type\": \"object\",\n      \"description\": \"The capabilities supported by a model.\",\n      \"properties\": {\n        \"completion_chat\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the model supports chat completions.\"\n        },\n        \"completion_fim\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the model supports fill-in-the-middle completions.\"\n        },\n        \"function_calling\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the model\
  \ supports function calling.\"\n        },\n        \"fine_tuning\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the model can be used as a base for fine-tuning.\"\n        },\n        \"vision\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the model supports vision and image inputs.\"\n        }\n      }\n    }\n  },\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique model identifier used in API requests.\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"description\": \"The object type, always model.\",\n      \"const\": \"model\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp when the model was created.\"\n    },\n    \"owned_by\": {\n      \"type\": \"string\",\n      \"description\": \"The organization that owns the model.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"\
  The human-readable display name of the model.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the model and its intended use cases.\"\n    },\n    \"max_context_length\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum context length in tokens supported by the model.\",\n      \"minimum\": 1\n    },\n    \"aliases\": {\n      \"type\": \"array\",\n      \"description\": \"Alternative identifiers that can be used to reference the model.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"deprecation\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The deprecation date of the model, if scheduled.\"\n    },\n    \"capabilities\": {\n      \"$ref\": \"#/$defs/ModelCapabilities\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Whether this is a base model or a fine-tuned model.\",\n      \"enum\": [\"base\", \"fine-tuned\"\
  ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mistral-ai/refs/heads/main/json-schema/mistral-ai-model-schema.json
tags:
- Agents
- Artificial Intelligence
- Batch Processing
- Chat
- Embeddings
- Fine-Tuning
- Large Language Models
- OCR
title: Mistral AI Model
---
