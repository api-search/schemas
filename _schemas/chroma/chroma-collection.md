---
description: A Chroma collection stores embeddings, documents, and associated metadata. Collections are the primary unit for organizing and searching vector data within a database.
layout: schema
name: Chroma Collection
properties_list:
- description: The unique identifier of the collection, assigned by the server on creation
  name: id
  type: string
- description: The name of the collection, used as a human-readable identifier within a database
  name: name
  type: string
- description: Arbitrary key-value metadata associated with the collection, used for organizing and describing the collection's purpose and configuration
  name: metadata
  type:
  - object
  - 'null'
- description: The name of the tenant this collection belongs to
  name: tenant
  type: string
- description: The name of the database this collection belongs to
  name: database
  type: string
provider_name: Chroma
provider_slug: chroma
schema_file: json-schema/chroma-collection-schema.json
slug: chroma-collection
source_filename: chroma-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://trychroma.com/schemas/chroma/collection.json\",\n  \"title\": \"Chroma Collection\",\n  \"description\": \"A Chroma collection stores embeddings, documents, and associated metadata. Collections are the primary unit for organizing and searching vector data within a database.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the collection, assigned by the server on creation\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"maxLength\": 512,\n      \"pattern\": \"^[a-zA-Z0-9_-]+$\",\n      \"description\": \"The name of the collection, used as a human-readable identifier within a database\"\n    },\n    \"metadata\": {\n      \"type\": [\"object\", \"null\"],\n      \"additionalProperties\"\
  : true,\n      \"description\": \"Arbitrary key-value metadata associated with the collection, used for organizing and describing the collection's purpose and configuration\"\n    },\n    \"tenant\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the tenant this collection belongs to\"\n    },\n    \"database\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the database this collection belongs to\"\n    }\n  },\n  \"$defs\": {\n    \"CollectionConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration options that can be set in collection metadata to control embedding and indexing behavior\",\n      \"properties\": {\n        \"hnsw:space\": {\n          \"type\": \"string\",\n          \"enum\": [\"l2\", \"ip\", \"cosine\"],\n          \"default\": \"l2\",\n          \"description\": \"The distance function used for nearest neighbor search. l2 is Euclidean distance, ip is inner product, cosine is cosine similarity.\"\
  \n        },\n        \"hnsw:construction_ef\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"default\": 100,\n          \"description\": \"The size of the dynamic candidate list during HNSW index construction. Higher values improve recall at the cost of indexing speed.\"\n        },\n        \"hnsw:search_ef\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"default\": 10,\n          \"description\": \"The size of the dynamic candidate list during search. Higher values improve recall at the cost of search speed.\"\n        },\n        \"hnsw:M\": {\n          \"type\": \"integer\",\n          \"minimum\": 2,\n          \"default\": 16,\n          \"description\": \"The maximum number of bi-directional links per element in the HNSW graph. Higher values improve recall at the cost of memory.\"\n        },\n        \"hnsw:num_threads\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"default\": 4,\n    \
  \      \"description\": \"Number of threads to use during HNSW index construction\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chroma/refs/heads/main/json-schema/chroma-collection-schema.json
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
title: Chroma Collection
---
