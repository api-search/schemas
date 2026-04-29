---
description: ''
layout: schema
name: Info
properties_list:
- description: Loaded model ID
  name: model_id
  type: string
- description: Model revision SHA
  name: model_sha
  type: string
- description: Model data type
  name: model_dtype
  type: string
- description: Device type (cuda, cpu)
  name: model_device_type
  type: string
- description: Pipeline task tag
  name: model_pipeline_tag
  type: string
- description: ''
  name: max_concurrent_requests
  type: integer
- description: ''
  name: max_best_of
  type: integer
- description: ''
  name: max_stop_sequences
  type: integer
- description: Maximum input token length
  name: max_input_length
  type: integer
- description: Maximum total tokens (input + output)
  name: max_total_tokens
  type: integer
- description: ''
  name: waiting_served_ratio
  type: number
- description: ''
  name: max_batch_total_tokens
  type: integer
- description: ''
  name: max_waiting_tokens
  type: integer
- description: ''
  name: validation_workers
  type: integer
- description: ''
  name: max_client_batch_size
  type: integer
- description: TGI version
  name: version
  type: string
- description: TGI build SHA
  name: sha
  type: string
- description: Docker image label
  name: docker_label
  type: string
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-text-generation-inference-info-schema.json
slug: hugging-face-text-generation-inference-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Info\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"model_id\": {\n      \"type\": \"string\",\n      \"description\": \"Loaded model ID\"\n    },\n    \"model_sha\": {\n      \"type\": \"string\",\n      \"description\": \"Model revision SHA\"\n    },\n    \"model_dtype\": {\n      \"type\": \"string\",\n      \"description\": \"Model data type\"\n    },\n    \"model_device_type\": {\n      \"type\": \"string\",\n      \"description\": \"Device type (cuda, cpu)\"\n    },\n    \"model_pipeline_tag\": {\n      \"type\": \"string\",\n      \"description\": \"Pipeline task tag\"\n    },\n    \"max_concurrent_requests\": {\n      \"type\": \"integer\"\n    },\n    \"max_best_of\": {\n      \"type\": \"integer\"\n    },\n    \"max_stop_sequences\": {\n      \"type\": \"integer\"\n    },\n    \"max_input_length\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum input token\
  \ length\"\n    },\n    \"max_total_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum total tokens (input + output)\"\n    },\n    \"waiting_served_ratio\": {\n      \"type\": \"number\"\n    },\n    \"max_batch_total_tokens\": {\n      \"type\": \"integer\"\n    },\n    \"max_waiting_tokens\": {\n      \"type\": \"integer\"\n    },\n    \"validation_workers\": {\n      \"type\": \"integer\"\n    },\n    \"max_client_batch_size\": {\n      \"type\": \"integer\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"TGI version\"\n    },\n    \"sha\": {\n      \"type\": \"string\",\n      \"description\": \"TGI build SHA\"\n    },\n    \"docker_label\": {\n      \"type\": \"string\",\n      \"description\": \"Docker image label\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-text-generation-inference-info-schema.json
tags: []
title: Info
---
