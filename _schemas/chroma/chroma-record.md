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
