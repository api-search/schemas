---
description: Represents a dataset managed through the Cohere Datasets API, used for embed jobs, fine-tuning, and other batch processing tasks.
layout: schema
name: Cohere Dataset
properties_list:
- description: The unique identifier of the dataset.
  name: id
  type: string
- description: The human-readable name of the dataset.
  name: name
  type: string
- description: The type of dataset, which determines its schema and compatible operations.
  name: dataset_type
  type: string
- description: The current validation status of the dataset after upload.
  name: validation_status
  type: string
- description: The ISO 8601 timestamp when the dataset was created.
  name: created_at
  type: string
- description: The ISO 8601 timestamp when the dataset was last updated.
  name: updated_at
  type: string
- description: The expected schema definition for the dataset records.
  name: schema
  type: string
- description: The field names required in each record of the dataset.
  name: required_fields
  type: array
- description: The field names that are preserved through processing.
  name: preserve_fields
  type: array
- description: The error message if dataset validation failed.
  name: validation_error
  type: string
- description: Warning messages for rows that were dropped during validation.
  name: validation_warnings
  type: array
provider_name: cohere
provider_slug: cohere
schema_file: json-schema/cohere-dataset-schema.json
slug: cohere-dataset
source_filename: cohere-dataset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.cohere.com/schemas/cohere/dataset.json\",\n  \"title\": \"Cohere Dataset\",\n  \"description\": \"Represents a dataset managed through the Cohere Datasets API, used for embed jobs, fine-tuning, and other batch processing tasks.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"dataset_type\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the dataset.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable name of the dataset.\"\n    },\n    \"dataset_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of dataset, which determines its schema and compatible operations.\",\n      \"enum\": [\n        \"embed-input\",\n        \"embed-output\",\n        \"reranker-finetune-input\",\n        \"prompt-completion-finetune-input\",\n    \
  \    \"single-label-classification-finetune-input\",\n        \"chat-finetune-input\"\n      ]\n    },\n    \"validation_status\": {\n      \"type\": \"string\",\n      \"description\": \"The current validation status of the dataset after upload.\",\n      \"enum\": [\"Unknown\", \"Queued\", \"Processing\", \"Validated\", \"Skipped\", \"Failed\"]\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when the dataset was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when the dataset was last updated.\"\n    },\n    \"schema\": {\n      \"type\": \"string\",\n      \"description\": \"The expected schema definition for the dataset records.\"\n    },\n    \"required_fields\": {\n      \"type\": \"array\",\n      \"description\": \"The field names required in each record of the dataset.\",\n     \
  \ \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"preserve_fields\": {\n      \"type\": \"array\",\n      \"description\": \"The field names that are preserved through processing.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"validation_error\": {\n      \"type\": \"string\",\n      \"description\": \"The error message if dataset validation failed.\"\n    },\n    \"validation_warnings\": {\n      \"type\": \"array\",\n      \"description\": \"Warning messages for rows that were dropped during validation.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cohere/refs/heads/main/json-schema/cohere-dataset-schema.json
tags: []
title: Cohere Dataset
---
