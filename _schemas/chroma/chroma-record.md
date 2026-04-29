---
description: A Chroma record represents a single item stored in a collection, consisting of an embedding vector, optional document text, optional metadata, and an optional URI reference.
layout: schema
name: Chroma Record
properties_list:
- description: A unique identifier for the record within the collection. Must be unique across all records in the collection.
  name: id
  type: string
- description: The vector embedding for this record. Each element is a floating point number representing a dimension of the embedding space.
  name: embedding
  type:
  - array
  - 'null'
- description: The text document associated with this record. If provided without an embedding, the server will automatically generate an embedding from the document text.
  name: document
  type:
  - string
  - 'null'
- description: Key-value metadata associated with the record. Values can be strings, numbers, integers, or booleans. Metadata is searchable using where filters.
  name: metadata
  type:
  - object
  - 'null'
- description: An optional URI reference associated with the record, typically pointing to the source content or an external resource.
  name: uri
  type:
  - string
  - 'null'
provider_name: Chroma
provider_slug: chroma
schema_file: json-schema/chroma-record-schema.json
slug: chroma-record
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://trychroma.com/schemas/chroma/record.json\",\n  \"title\": \"Chroma Record\",\n  \"description\": \"A Chroma record represents a single item stored in a collection, consisting of an embedding vector, optional document text, optional metadata, and an optional URI reference.\",\n  \"type\": \"object\",\n  \"required\": [\"id\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"description\": \"A unique identifier for the record within the collection. Must be unique across all records in the collection.\"\n    },\n    \"embedding\": {\n      \"type\": [\"array\", \"null\"],\n      \"items\": {\n        \"type\": \"number\",\n        \"format\": \"float\"\n      },\n      \"description\": \"The vector embedding for this record. Each element is a floating point number representing a dimension of the embedding space.\"\n    },\n    \"document\"\
  : {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The text document associated with this record. If provided without an embedding, the server will automatically generate an embedding from the document text.\"\n    },\n    \"metadata\": {\n      \"type\": [\"object\", \"null\"],\n      \"additionalProperties\": {\n        \"oneOf\": [\n          { \"type\": \"string\" },\n          { \"type\": \"number\" },\n          { \"type\": \"integer\" },\n          { \"type\": \"boolean\" }\n        ]\n      },\n      \"description\": \"Key-value metadata associated with the record. Values can be strings, numbers, integers, or booleans. Metadata is searchable using where filters.\"\n    },\n    \"uri\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"An optional URI reference associated with the record, typically pointing to the source content or an external resource.\"\n    }\n  },\n  \"$defs\": {\n    \"Embedding\": {\n     \
  \ \"type\": \"array\",\n      \"items\": {\n        \"type\": \"number\",\n        \"format\": \"float\"\n      },\n      \"description\": \"A vector embedding represented as an array of floating point numbers\"\n    },\n    \"WhereFilter\": {\n      \"type\": \"object\",\n      \"description\": \"A metadata filter expression used to narrow search results based on record metadata values. Supports comparison operators ($eq, $ne, $gt, $gte, $lt, $lte, $in, $nin) and logical operators ($and, $or).\",\n      \"additionalProperties\": true\n    },\n    \"WhereDocumentFilter\": {\n      \"type\": \"object\",\n      \"description\": \"A document content filter expression used to filter records by their document text. Supports $contains, $not_contains for substring matching and $regex, $not_regex for pattern matching.\",\n      \"additionalProperties\": true\n    },\n    \"IncludeField\": {\n      \"type\": \"string\",\n      \"enum\": [\"embeddings\", \"documents\", \"metadatas\", \"distances\"\
  , \"uris\"],\n      \"description\": \"A field that can be included in query and get responses\"\n    },\n    \"QueryResult\": {\n      \"type\": \"object\",\n      \"description\": \"The result of a vector similarity query, containing matched record IDs and optionally their embeddings, documents, metadatas, distances, and URIs\",\n      \"required\": [\"ids\"],\n      \"properties\": {\n        \"ids\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"description\": \"Nested arrays of record IDs, one array per query\"\n        },\n        \"embeddings\": {\n          \"type\": [\"array\", \"null\"],\n          \"items\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"$ref\": \"#/$defs/Embedding\"\n            }\n          },\n          \"description\": \"Nested arrays of embedding vectors, one array per query\"\
  \n        },\n        \"documents\": {\n          \"type\": [\"array\", \"null\"],\n          \"items\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": [\"string\", \"null\"]\n            }\n          },\n          \"description\": \"Nested arrays of documents, one array per query\"\n        },\n        \"metadatas\": {\n          \"type\": [\"array\", \"null\"],\n          \"items\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": [\"object\", \"null\"],\n              \"additionalProperties\": true\n            }\n          },\n          \"description\": \"Nested arrays of metadata objects, one array per query\"\n        },\n        \"distances\": {\n          \"type\": [\"array\", \"null\"],\n          \"items\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"number\",\n              \"format\": \"float\"\n            }\n          },\n          \"description\": \"\
  Nested arrays of distance scores, one array per query\"\n        },\n        \"uris\": {\n          \"type\": [\"array\", \"null\"],\n          \"items\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": [\"string\", \"null\"]\n            }\n          },\n          \"description\": \"Nested arrays of URIs, one array per query\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chroma/refs/heads/main/json-schema/chroma-record-schema.json
tags:
- AI
- AI Native
- Apache 2.0
- Cloud
- Embeddings
- Hybrid Search
- JavaScript
- LLM
- Machine Learning
- Multi-Modal
- Open Source
- Python
- RAG
- Retrieval
- SDK
- Search
- Serverless
- TypeScript
- Vector Database
title: Chroma Record
---
