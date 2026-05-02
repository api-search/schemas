---
description: A document ingestion pipeline (index) in LlamaCloud that processes, embeds, and indexes documents for retrieval in RAG applications.
layout: schema
name: LlamaIndex Pipeline
properties_list:
- description: Unique identifier of the pipeline.
  name: id
  type: string
- description: Human-readable name of the pipeline.
  name: name
  type: string
- description: Identifier of the project the pipeline belongs to.
  name: project_id
  type: string
- description: Current processing status of the pipeline.
  name: status
  type: string
- description: Name of the embedding model used for vectorization.
  name: embedding_model
  type: string
- description: Scheduled sync frequency in seconds. Zero means manual sync only.
  name: sync_interval
  type: integer
- description: Data sources connected to this pipeline for automatic ingestion.
  name: data_sources
  type: array
- description: Data sinks where processed content is stored.
  name: data_sinks
  type: array
- description: Timestamp when the pipeline was created.
  name: created_at
  type: string
- description: Timestamp when the pipeline was last updated.
  name: updated_at
  type: string
provider_name: llamaindex
provider_slug: llamaindex
schema_file: json-schema/llamaindex-pipeline-schema.json
slug: llamaindex-pipeline
source_filename: llamaindex-pipeline-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://llamaindex.ai/schemas/llamaindex/pipeline.json\",\n  \"title\": \"LlamaIndex Pipeline\",\n  \"description\": \"A document ingestion pipeline (index) in LlamaCloud that processes, embeds, and indexes documents for retrieval in RAG applications.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"project_id\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the pipeline.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the pipeline.\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"project_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the project the pipeline belongs to.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"syncing\", \"error\", \"idle\"],\n      \"description\"\
  : \"Current processing status of the pipeline.\"\n    },\n    \"embedding_model\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the embedding model used for vectorization.\"\n    },\n    \"sync_interval\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Scheduled sync frequency in seconds. Zero means manual sync only.\"\n    },\n    \"data_sources\": {\n      \"type\": \"array\",\n      \"description\": \"Data sources connected to this pipeline for automatic ingestion.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DataSource\"\n      }\n    },\n    \"data_sinks\": {\n      \"type\": \"array\",\n      \"description\": \"Data sinks where processed content is stored.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DataSink\"\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the pipeline was created.\"\n    },\n    \"updated_at\": {\n\
  \      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the pipeline was last updated.\"\n    }\n  },\n  \"$defs\": {\n    \"DataSource\": {\n      \"type\": \"object\",\n      \"description\": \"A data source that provides documents for automatic ingestion into a pipeline.\",\n      \"required\": [\"id\", \"name\", \"source_type\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the data source.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable name of the data source.\",\n          \"minLength\": 1,\n          \"maxLength\": 255\n        },\n        \"source_type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of the data source (e.g., document, table, api, database, web).\"\n        },\n        \"project_id\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Identifier of the project the data source belongs to.\"\n        },\n        \"config\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true,\n          \"description\": \"Configuration specific to the data source type.\"\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the data source was created.\"\n        }\n      }\n    },\n    \"DataSink\": {\n      \"type\": \"object\",\n      \"description\": \"A data sink that receives processed and embedded content, such as a vector database.\",\n      \"required\": [\"id\", \"name\", \"sink_type\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the data sink.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable name of the data sink.\",\n          \"minLength\": 1,\n  \
  \        \"maxLength\": 255\n        },\n        \"sink_type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of the data sink (e.g., vector_store).\"\n        },\n        \"config\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true,\n          \"description\": \"Configuration specific to the data sink type.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/json-schema/llamaindex-pipeline-schema.json
tags: []
title: LlamaIndex Pipeline
---
