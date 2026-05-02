---
description: Schema for a Mistral AI batch job object, representing an asynchronous batch processing job with status tracking and result references.
layout: schema
name: Mistral AI Batch Job
properties_list:
- description: Unique identifier for the batch job.
  name: id
  type: string
- description: The object type.
  name: object
  type: string
- description: The model used for batch processing.
  name: model
  type: string
- description: The API endpoint used for each request in the batch.
  name: endpoint
  type: string
- description: File IDs containing input data in JSONL format.
  name: input_files
  type: array
- description: The current status of the batch job.
  name: status
  type: string
- description: Unix timestamp when the job was created.
  name: created_at
  type: integer
- description: Unix timestamp when the job started processing.
  name: started_at
  type: integer
- description: Unix timestamp when the job completed.
  name: completed_at
  type: integer
- description: Total number of requests in the batch.
  name: total_requests
  type: integer
- description: Number of requests that have completed processing.
  name: completed_requests
  type: integer
- description: Number of requests that succeeded.
  name: succeeded_requests
  type: integer
- description: Number of requests that failed.
  name: failed_requests
  type: integer
- description: File ID of the output file containing successful results.
  name: output_file
  type: string
- description: File ID of the error file containing failed request details.
  name: error_file
  type: string
- description: Custom metadata associated with the batch job.
  name: metadata
  type: object
provider_name: Mistral AI
provider_slug: mistral-ai
schema_file: json-schema/mistral-ai-batch-job-schema.json
slug: mistral-ai-batch-job
source_filename: mistral-ai-batch-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://mistral.ai/schemas/mistral-ai/batch-job.json\",\n  \"title\": \"Mistral AI Batch Job\",\n  \"description\": \"Schema for a Mistral AI batch job object, representing an asynchronous batch processing job with status tracking and result references.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"model\", \"endpoint\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the batch job.\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"description\": \"The object type.\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"The model used for batch processing.\"\n    },\n    \"endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The API endpoint used for each request in the batch.\",\n      \"enum\": [\n        \"/v1/chat/completions\"\
  ,\n        \"/v1/embeddings\",\n        \"/v1/fim/completions\",\n        \"/v1/moderations\",\n        \"/v1/chat/moderations\",\n        \"/v1/ocr\",\n        \"/v1/classifications\",\n        \"/v1/conversations\",\n        \"/v1/audio/transcriptions\"\n      ]\n    },\n    \"input_files\": {\n      \"type\": \"array\",\n      \"description\": \"File IDs containing input data in JSONL format.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uuid\"\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the batch job.\",\n      \"enum\": [\n        \"QUEUED\",\n        \"RUNNING\",\n        \"SUCCESS\",\n        \"FAILED\",\n        \"TIMEOUT_EXCEEDED\",\n        \"CANCELLATION_REQUESTED\",\n        \"CANCELLED\"\n      ]\n    },\n    \"created_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp when the job was created.\"\n    },\n    \"started_at\": {\n      \"type\": \"\
  integer\",\n      \"description\": \"Unix timestamp when the job started processing.\"\n    },\n    \"completed_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp when the job completed.\"\n    },\n    \"total_requests\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of requests in the batch.\",\n      \"minimum\": 0\n    },\n    \"completed_requests\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of requests that have completed processing.\",\n      \"minimum\": 0\n    },\n    \"succeeded_requests\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of requests that succeeded.\",\n      \"minimum\": 0\n    },\n    \"failed_requests\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of requests that failed.\",\n      \"minimum\": 0\n    },\n    \"output_file\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"File ID of the output file containing\
  \ successful results.\"\n    },\n    \"error_file\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"File ID of the error file containing failed request details.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Custom metadata associated with the batch job.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mistral-ai/refs/heads/main/json-schema/mistral-ai-batch-job-schema.json
tags:
- Agents
- Artificial Intelligence
- Batch Processing
- Chat
- Embeddings
- Fine-Tuning
- Large Language Models
- OCR
title: Mistral AI Batch Job
---
