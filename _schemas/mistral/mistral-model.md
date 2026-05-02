---
description: A language model available on the Mistral AI platform, including base models and user fine-tuned models with capability and configuration metadata.
layout: schema
name: Mistral Model
properties_list:
- description: Unique identifier for the model
  name: id
  type: string
- description: Object type identifier
  name: object
  type: string
- description: Unix timestamp when the model was created
  name: created
  type: integer
- description: Organization that owns the model
  name: owned_by
  type: string
- description: Human-readable name of the model
  name: name
  type:
  - string
  - 'null'
- description: Description of the model and its capabilities
  name: description
  type:
  - string
  - 'null'
- description: Maximum context window length in tokens
  name: max_context_length
  type: integer
- description: Alternative names that can reference this model
  name: aliases
  type: array
- description: Deprecation date if the model is being retired
  name: deprecation
  type:
  - string
  - 'null'
- description: ''
  name: capabilities
  type: object
- description: Whether this is a base platform model or a user fine-tuned model
  name: type
  type: string
provider_name: Mistral AI
provider_slug: mistral
schema_file: json-schema/mistral-model-schema.json
slug: mistral-model
source_filename: mistral-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.mistral.ai/schemas/mistral/model.json\",\n  \"title\": \"Mistral Model\",\n  \"description\": \"A language model available on the Mistral AI platform, including base models and user fine-tuned models with capability and configuration metadata.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"object\", \"created\", \"owned_by\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the model\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"enum\": [\"model\"],\n      \"description\": \"Object type identifier\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp when the model was created\"\n    },\n    \"owned_by\": {\n      \"type\": \"string\",\n      \"description\": \"Organization that owns the model\"\n    },\n    \"name\": {\n      \"type\": [\"\
  string\", \"null\"],\n      \"description\": \"Human-readable name of the model\"\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Description of the model and its capabilities\"\n    },\n    \"max_context_length\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"Maximum context window length in tokens\"\n    },\n    \"aliases\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Alternative names that can reference this model\"\n    },\n    \"deprecation\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Deprecation date if the model is being retired\"\n    },\n    \"capabilities\": {\n      \"$ref\": \"#/$defs/Capabilities\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"base\", \"fine-tuned\"],\n      \"description\": \"Whether this is a base platform model\
  \ or a user fine-tuned model\"\n    }\n  },\n  \"$defs\": {\n    \"Capabilities\": {\n      \"type\": \"object\",\n      \"description\": \"Supported capabilities of the model\",\n      \"properties\": {\n        \"completion_chat\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the model supports chat completions\"\n        },\n        \"completion_fim\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the model supports fill-in-the-middle completions\"\n        },\n        \"function_calling\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the model supports function calling\"\n        },\n        \"fine_tuning\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the model can be fine-tuned\"\n        },\n        \"vision\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the model supports vision/image inputs\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/json-schema/mistral-model-schema.json
tags: []
title: Mistral Model
---
