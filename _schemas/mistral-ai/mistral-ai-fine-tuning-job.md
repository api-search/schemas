---
description: Schema for a Mistral AI fine-tuning job, including training configuration, hyperparameters, integrations, and job status tracking.
layout: schema
name: Mistral AI Fine-Tuning Job
properties_list:
- description: Unique identifier for the fine-tuning job.
  name: id
  type: string
- description: The base model being fine-tuned.
  name: model
  type: string
- description: The current status of the fine-tuning job.
  name: status
  type: string
- description: The type of fine-tuning job.
  name: job_type
  type: string
- description: Whether the job was configured to auto-start after validation.
  name: auto_start
  type: boolean
- description: Training files used for this job.
  name: training_files
  type: array
- description: Validation files used for evaluating the model during training.
  name: validation_files
  type: array
- description: ''
  name: hyperparameters
  type: object
- description: The ID of the resulting fine-tuned model, set after successful completion.
  name: fine_tuned_model
  type: string
- description: External integrations enabled for this job.
  name: integrations
  type: array
- description: Unix timestamp when the job was created.
  name: created_at
  type: integer
- description: Unix timestamp when the job was last modified.
  name: modified_at
  type: integer
- description: A suffix appended to the fine-tuned model name.
  name: suffix
  type: string
provider_name: Mistral AI
provider_slug: mistral-ai
schema_file: json-schema/mistral-ai-fine-tuning-job-schema.json
slug: mistral-ai-fine-tuning-job
source_filename: mistral-ai-fine-tuning-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://mistral.ai/schemas/mistral-ai/fine-tuning-job.json\",\n  \"title\": \"Mistral AI Fine-Tuning Job\",\n  \"description\": \"Schema for a Mistral AI fine-tuning job, including training configuration, hyperparameters, integrations, and job status tracking.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"model\", \"status\"],\n  \"$defs\": {\n    \"TrainingFile\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a training file with an optional weight.\",\n      \"required\": [\"file_id\"],\n      \"properties\": {\n        \"file_id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The ID of the uploaded training file.\"\n        },\n        \"weight\": {\n          \"type\": \"number\",\n          \"description\": \"The relative weight of this training file in the training mix.\",\n          \"minimum\": 0,\n\
  \          \"default\": 1.0\n        }\n      }\n    },\n    \"Hyperparameters\": {\n      \"type\": \"object\",\n      \"description\": \"Configurable hyperparameters for a fine-tuning job.\",\n      \"properties\": {\n        \"training_steps\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of training steps to run.\",\n          \"minimum\": 1\n        },\n        \"learning_rate\": {\n          \"type\": \"number\",\n          \"description\": \"The learning rate for optimization.\",\n          \"minimum\": 0,\n          \"exclusiveMinimum\": true\n        },\n        \"weight_decay\": {\n          \"type\": \"number\",\n          \"description\": \"Weight decay coefficient for regularization.\",\n          \"minimum\": 0\n        },\n        \"warmup_fraction\": {\n          \"type\": \"number\",\n          \"description\": \"Fraction of total steps used for learning rate warmup.\",\n          \"minimum\": 0,\n          \"maximum\": 1\n        }\n  \
  \    }\n    },\n    \"Integration\": {\n      \"type\": \"object\",\n      \"description\": \"An external integration for experiment tracking during training.\",\n      \"required\": [\"type\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The integration provider type.\",\n          \"enum\": [\"wandb\"]\n        },\n        \"project\": {\n          \"type\": \"string\",\n          \"description\": \"The project name in the integration platform.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The run name in the integration platform.\"\n        },\n        \"api_key\": {\n          \"type\": \"string\",\n          \"description\": \"API key for authenticating with the integration service.\"\n        }\n      }\n    }\n  },\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the fine-tuning\
  \ job.\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"The base model being fine-tuned.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the fine-tuning job.\",\n      \"enum\": [\n        \"QUEUED\",\n        \"STARTED\",\n        \"VALIDATING\",\n        \"VALIDATED\",\n        \"RUNNING\",\n        \"FAILED_VALIDATION\",\n        \"FAILED\",\n        \"SUCCESS\",\n        \"CANCELLED\",\n        \"CANCELLATION_REQUESTED\"\n      ]\n    },\n    \"job_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of fine-tuning job.\"\n    },\n    \"auto_start\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the job was configured to auto-start after validation.\"\n    },\n    \"training_files\": {\n      \"type\": \"array\",\n      \"description\": \"Training files used for this job.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TrainingFile\"\n      }\n  \
  \  },\n    \"validation_files\": {\n      \"type\": \"array\",\n      \"description\": \"Validation files used for evaluating the model during training.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uuid\"\n      }\n    },\n    \"hyperparameters\": {\n      \"$ref\": \"#/$defs/Hyperparameters\"\n    },\n    \"fine_tuned_model\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the resulting fine-tuned model, set after successful completion.\"\n    },\n    \"integrations\": {\n      \"type\": \"array\",\n      \"description\": \"External integrations enabled for this job.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Integration\"\n      }\n    },\n    \"created_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp when the job was created.\"\n    },\n    \"modified_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp when the job was last modified.\"\n    },\n    \"suffix\": {\n  \
  \    \"type\": \"string\",\n      \"description\": \"A suffix appended to the fine-tuned model name.\",\n      \"maxLength\": 18\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mistral-ai/refs/heads/main/json-schema/mistral-ai-fine-tuning-job-schema.json
tags:
- Agents
- Artificial Intelligence
- Batch Processing
- Chat
- Embeddings
- Fine-Tuning
- Large Language Models
- OCR
title: Mistral AI Fine-Tuning Job
---
