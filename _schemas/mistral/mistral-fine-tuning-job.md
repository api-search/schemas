---
description: A fine-tuning job for customizing a Mistral model on user-provided training data, with configurable hyperparameters, status tracking, and integration support.
layout: schema
name: Mistral Fine-Tuning Job
properties_list:
- description: Unique identifier for the fine-tuning job
  name: id
  type: string
- description: Whether training starts automatically after validation
  name: auto_start
  type: boolean
- description: The base model being fine-tuned
  name: model
  type: string
- description: Current status of the fine-tuning job
  name: status
  type: string
- description: Type of fine-tuning job (e.g., text, vision, classifier)
  name: job_type
  type: string
- description: Unix timestamp when the job was created
  name: created_at
  type: integer
- description: Unix timestamp when the job was last modified
  name: modified_at
  type: integer
- description: IDs of training data files
  name: training_files
  type: array
- description: IDs of validation data files
  name: validation_files
  type: array
- description: ''
  name: hyperparameters
  type: object
- description: ID of the resulting fine-tuned model upon completion
  name: fine_tuned_model
  type:
  - string
  - 'null'
- description: User-specified suffix appended to the fine-tuned model name
  name: suffix
  type: string
- description: Third-party integrations for experiment tracking
  name: integrations
  type: array
provider_name: Mistral AI
provider_slug: mistral
schema_file: json-schema/mistral-fine-tuning-job-schema.json
slug: mistral-fine-tuning-job
source_filename: mistral-fine-tuning-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.mistral.ai/schemas/mistral/fine-tuning-job.json\",\n  \"title\": \"Mistral Fine-Tuning Job\",\n  \"description\": \"A fine-tuning job for customizing a Mistral model on user-provided training data, with configurable hyperparameters, status tracking, and integration support.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"model\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the fine-tuning job\"\n    },\n    \"auto_start\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether training starts automatically after validation\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"The base model being fine-tuned\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"QUEUED\",\n        \"STARTED\"\
  ,\n        \"VALIDATING\",\n        \"VALIDATED\",\n        \"RUNNING\",\n        \"FAILED_VALIDATION\",\n        \"FAILED\",\n        \"SUCCESS\",\n        \"CANCELLED\",\n        \"CANCELLATION_REQUESTED\"\n      ],\n      \"description\": \"Current status of the fine-tuning job\"\n    },\n    \"job_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of fine-tuning job (e.g., text, vision, classifier)\"\n    },\n    \"created_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp when the job was created\"\n    },\n    \"modified_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp when the job was last modified\"\n    },\n    \"training_files\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uuid\"\n      },\n      \"description\": \"IDs of training data files\"\n    },\n    \"validation_files\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\"\
  : \"string\",\n        \"format\": \"uuid\"\n      },\n      \"description\": \"IDs of validation data files\"\n    },\n    \"hyperparameters\": {\n      \"$ref\": \"#/$defs/Hyperparameters\"\n    },\n    \"fine_tuned_model\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the resulting fine-tuned model upon completion\"\n    },\n    \"suffix\": {\n      \"type\": \"string\",\n      \"maxLength\": 18,\n      \"description\": \"User-specified suffix appended to the fine-tuned model name\"\n    },\n    \"integrations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Integration\"\n      },\n      \"description\": \"Third-party integrations for experiment tracking\"\n    }\n  },\n  \"$defs\": {\n    \"Hyperparameters\": {\n      \"type\": \"object\",\n      \"description\": \"Hyperparameters for the fine-tuning job\",\n      \"properties\": {\n        \"training_steps\": {\n          \"type\": \"integer\",\n          \"minimum\"\
  : 1,\n          \"description\": \"Number of training steps\"\n        },\n        \"learning_rate\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"description\": \"Learning rate\"\n        },\n        \"weight_decay\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"description\": \"Weight decay regularization factor\"\n        },\n        \"warmup_fraction\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"maximum\": 1,\n          \"description\": \"Fraction of total steps for learning rate warmup\"\n        },\n        \"epochs\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"description\": \"Number of training epochs\"\n        },\n        \"seq_len\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum sequence length for training\"\n        }\n      }\n    },\n    \"Integration\": {\n      \"type\": \"object\",\n      \"description\": \"A third-party\
  \ integration for experiment tracking\",\n      \"required\": [\"type\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"wandb\"],\n          \"description\": \"Integration provider type\"\n        },\n        \"project\": {\n          \"type\": \"string\",\n          \"description\": \"Project name in the integration platform\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Run name in the integration platform\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/json-schema/mistral-fine-tuning-job-schema.json
tags: []
title: Mistral Fine-Tuning Job
---
