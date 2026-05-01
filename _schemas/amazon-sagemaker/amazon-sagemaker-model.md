---
description: Model schema from Amazon SageMaker API
layout: schema
name: Model
properties_list:
- description: The name of the model.
  name: ModelName
  type: string
- description: The Amazon Resource Name (ARN) of the model.
  name: ModelArn
  type: string
- description: ''
  name: PrimaryContainer
  type: object
- description: The ARN of the IAM role.
  name: ExecutionRoleArn
  type: string
- description: A timestamp indicating when the model was created.
  name: CreationTime
  type: string
provider_name: Amazon SageMaker
provider_slug: amazon-sagemaker
schema_file: json-schema/amazon-sagemaker-model-schema.json
slug: amazon-sagemaker-model
source_filename: amazon-sagemaker-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-sagemaker/refs/heads/main/json-schema/amazon-sagemaker-model-schema.json\",\n  \"title\": \"Model\",\n  \"description\": \"Model schema from Amazon SageMaker API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ModelName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the model.\"\n    },\n    \"ModelArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the model.\"\n    },\n    \"PrimaryContainer\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Image\": {\n          \"type\": \"string\",\n          \"description\": \"The inference image URI.\"\n        },\n        \"ModelDataUrl\": {\n          \"type\": \"string\",\n          \"description\": \"The S3 path where the model artifacts are stored.\"\n        },\n        \"Environment\": {\n     \
  \     \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Environment variables to set in the container.\"\n        }\n      }\n    },\n    \"ExecutionRoleArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the IAM role.\"\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"A timestamp indicating when the model was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-sagemaker/refs/heads/main/json-schema/amazon-sagemaker-model-schema.json
tags:
- AI
- Inference
- Machine Learning
- MLOps
- Training
title: Model
---
