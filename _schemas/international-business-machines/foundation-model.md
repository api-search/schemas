---
description: An IBM watsonx.ai foundation model available for text generation and embeddings.
layout: schema
name: Foundation Model
properties_list:
- description: The unique identifier of the foundation model.
  name: model_id
  type: string
- description: The display name of the model.
  name: label
  type: string
- description: The provider of the model (e.g., IBM, Meta).
  name: provider
  type: string
- description: The source of the model.
  name: source
  type: string
- description: A brief description of the model.
  name: short_description
  type: string
- description: Tasks the model can perform.
  name: tasks
  type: array
- description: ''
  name: model_limits
  type: object
provider_name: International Business Machines
provider_slug: international-business-machines
schema_file: json-schema/foundation-model.json
slug: foundation-model
source_filename: foundation-model.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"foundation-model.json\",\n  \"title\": \"Foundation Model\",\n  \"description\": \"An IBM watsonx.ai foundation model available for text generation and embeddings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"model_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the foundation model.\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the model.\"\n    },\n    \"provider\": {\n      \"type\": \"string\",\n      \"description\": \"The provider of the model (e.g., IBM, Meta).\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"The source of the model.\"\n    },\n    \"short_description\": {\n      \"type\": \"string\",\n      \"description\": \"A brief description of the model.\"\n    },\n    \"tasks\": {\n      \"type\": \"array\",\n      \"description\": \"Tasks\
  \ the model can perform.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"label\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"model_limits\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"max_sequence_length\": {\n          \"type\": \"integer\"\n        },\n        \"max_output_tokens\": {\n          \"type\": \"integer\"\n        }\n      }\n    }\n  },\n  \"required\": [\"model_id\", \"label\", \"provider\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/json-schema/foundation-model.json
tags:
- Artificial Intelligence
- Cloud
- Enterprise
- IBM
title: Foundation Model
---
