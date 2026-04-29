---
description: Represents the embedding output from the Cohere Embed API, including vector representations in multiple numeric formats.
layout: schema
name: Cohere Embedding
properties_list:
- description: Unique identifier for the embedding request.
  name: id
  type: string
- description: Container for embedding vectors organized by type. Each type maps to an array of embedding vectors.
  name: embeddings
  type: object
- description: The text entries for which embeddings were returned.
  name: texts
  type: array
- description: The image entries for which embeddings were returned.
  name: images
  type: array
provider_name: cohere
provider_slug: cohere
schema_file: json-schema/cohere-embedding-schema.json
slug: cohere-embedding
source_filename: cohere-embedding-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.cohere.com/schemas/cohere/embedding.json\",\n  \"title\": \"Cohere Embedding\",\n  \"description\": \"Represents the embedding output from the Cohere Embed API, including vector representations in multiple numeric formats.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the embedding request.\"\n    },\n    \"embeddings\": {\n      \"type\": \"object\",\n      \"description\": \"Container for embedding vectors organized by type. Each type maps to an array of embedding vectors.\",\n      \"properties\": {\n        \"float\": {\n          \"type\": \"array\",\n          \"description\": \"Default float embeddings for each input. Supported with all Embed models.\",\n          \"items\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"number\"\n        \
  \    }\n          }\n        },\n        \"int8\": {\n          \"type\": \"array\",\n          \"description\": \"Signed int8 embeddings for each input. Supported with Embed v3.0 and newer models.\",\n          \"items\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"integer\",\n              \"minimum\": -128,\n              \"maximum\": 127\n            }\n          }\n        },\n        \"uint8\": {\n          \"type\": \"array\",\n          \"description\": \"Unsigned int8 embeddings for each input. Supported with Embed v3.0 and newer models.\",\n          \"items\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"integer\",\n              \"minimum\": 0,\n              \"maximum\": 255\n            }\n          }\n        },\n        \"binary\": {\n          \"type\": \"array\",\n          \"description\": \"Signed binary embeddings for each input. Supported with Embed v3.0 and newer models.\",\n\
  \          \"items\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"integer\"\n            }\n          }\n        },\n        \"base64\": {\n          \"type\": \"array\",\n          \"description\": \"Base64-encoded embeddings for each input. Supported with Embed v3.0 and newer models.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"pattern\": \"^[A-Za-z0-9+/]+=*$\"\n          }\n        }\n      }\n    },\n    \"texts\": {\n      \"type\": \"array\",\n      \"description\": \"The text entries for which embeddings were returned.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"images\": {\n      \"type\": \"array\",\n      \"description\": \"The image entries for which embeddings were returned.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"EmbeddingInputType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of input\
  \ for embedding generation. Determines how the model processes the input.\",\n      \"enum\": [\n        \"search_document\",\n        \"search_query\",\n        \"classification\",\n        \"clustering\",\n        \"image\"\n      ]\n    },\n    \"TruncateOption\": {\n      \"type\": \"string\",\n      \"description\": \"How to handle inputs longer than the maximum token length.\",\n      \"enum\": [\"NONE\", \"START\", \"END\"]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cohere/refs/heads/main/json-schema/cohere-embedding-schema.json
tags: []
title: Cohere Embedding
---
