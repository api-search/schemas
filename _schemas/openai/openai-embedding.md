---
description: A response object returned by the OpenAI Embeddings API. Contains a list of embedding vectors representing the input text as floating-point numbers, along with the model used and token usage statistics.
layout: schema
name: OpenAI Embedding Response
properties_list:
- description: The object type, which is always list.
  name: object
  type: string
- description: The list of embedding objects, one for each input.
  name: data
  type: array
- description: The name of the model used to generate the embeddings (e.g., text-embedding-3-small, text-embedding-3-large, text-embedding-ada-002).
  name: model
  type: string
- description: ''
  name: usage
  type: object
provider_name: OpenAI
provider_slug: openai
schema_file: json-schema/openai-embedding-schema.json
slug: openai-embedding
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://platform.openai.com/schemas/openai/embedding.json\",\n  \"title\": \"OpenAI Embedding Response\",\n  \"description\": \"A response object returned by the OpenAI Embeddings API. Contains a list of embedding vectors representing the input text as floating-point numbers, along with the model used and token usage statistics.\",\n  \"type\": \"object\",\n  \"required\": [\"object\", \"data\", \"model\", \"usage\"],\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"const\": \"list\",\n      \"description\": \"The object type, which is always list.\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"The list of embedding objects, one for each input.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Embedding\"\n      }\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the model used to generate\
  \ the embeddings (e.g., text-embedding-3-small, text-embedding-3-large, text-embedding-ada-002).\"\n    },\n    \"usage\": {\n      \"$ref\": \"#/$defs/Usage\"\n    }\n  },\n  \"$defs\": {\n    \"Embedding\": {\n      \"type\": \"object\",\n      \"description\": \"Represents an embedding vector returned by the Embeddings API. Each embedding corresponds to one input in the request.\",\n      \"required\": [\"object\", \"embedding\", \"index\"],\n      \"properties\": {\n        \"object\": {\n          \"type\": \"string\",\n          \"const\": \"embedding\",\n          \"description\": \"The object type, which is always embedding.\"\n        },\n        \"embedding\": {\n          \"oneOf\": [\n            {\n              \"type\": \"array\",\n              \"description\": \"The embedding vector, which is a list of floats. The length of vector depends on the model (1536 for text-embedding-ada-002, up to 3072 for text-embedding-3-large) and the dimensions parameter if specified.\",\n\
  \              \"items\": {\n                \"type\": \"number\",\n                \"format\": \"float\"\n              }\n            },\n            {\n              \"type\": \"string\",\n              \"description\": \"The embedding vector as a base64-encoded string, returned when encoding_format is base64.\"\n            }\n          ],\n          \"description\": \"The embedding vector representing the input text. The format depends on the encoding_format request parameter.\"\n        },\n        \"index\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The index of the embedding in the list of embeddings, corresponding to the position of the input in the request.\"\n        }\n      }\n    },\n    \"Usage\": {\n      \"type\": \"object\",\n      \"description\": \"Token usage statistics for the embedding request.\",\n      \"required\": [\"prompt_tokens\", \"total_tokens\"],\n      \"properties\": {\n        \"prompt_tokens\": {\n\
  \          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The number of tokens in the input text.\"\n        },\n        \"total_tokens\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The total number of tokens used in the request. For embeddings, this is the same as prompt_tokens.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/json-schema/openai-embedding-schema.json
tags:
- AI
- Artificial Intelligence
- Large Language Models
- T1
title: OpenAI Embedding Response
---
