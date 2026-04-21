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
tags: []
title: Cohere Embedding
---
