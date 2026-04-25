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
