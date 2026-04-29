---
description: TrainingJob schema from Amazon SageMaker API
layout: schema
name: TrainingJob
properties_list:
- description: The name of the training job.
  name: TrainingJobName
  type: string
- description: The Amazon Resource Name (ARN) of the training job.
  name: TrainingJobArn
  type: string
- description: The status of the training job.
  name: TrainingJobStatus
  type: string
- description: Provides detailed information about the state of the training job.
  name: SecondaryStatus
  type: string
- description: ''
  name: AlgorithmSpecification
  type: object
- description: The ARN of the IAM role.
  name: RoleArn
  type: string
- description: ''
  name: InputDataConfig
  type: array
- description: ''
  name: OutputDataConfig
  type: object
- description: ''
  name: ResourceConfig
  type: object
- description: ''
  name: StoppingCondition
  type: object
- description: ''
  name: HyperParameters
  type: object
- description: ''
  name: ModelArtifacts
  type: object
- description: ''
  name: TrainingStartTime
  type: string
- description: ''
  name: TrainingEndTime
  type: string
- description: ''
  name: CreationTime
  type: string
- description: ''
  name: LastModifiedTime
  type: string
- description: ''
  name: BillableTimeInSeconds
  type: integer
- description: ''
  name: FailureReason
  type: string
provider_name: Amazon SageMaker
provider_slug: amazon-sagemaker
schema_file: json-schema/amazon-sagemaker-training-job-schema.json
slug: amazon-sagemaker-training-job
source_filename: amazon-sagemaker-training-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-sagemaker/refs/heads/main/json-schema/amazon-sagemaker-training-job-schema.json\",\n  \"title\": \"TrainingJob\",\n  \"description\": \"TrainingJob schema from Amazon SageMaker API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TrainingJobName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the training job.\"\n    },\n    \"TrainingJobArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the training job.\"\n    },\n    \"TrainingJobStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the training job.\",\n      \"enum\": [\n        \"InProgress\",\n        \"Completed\",\n        \"Failed\",\n        \"Stopping\",\n        \"Stopped\"\n      ]\n    },\n    \"SecondaryStatus\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Provides detailed information about the state of the training job.\"\n    },\n    \"AlgorithmSpecification\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"TrainingImage\": {\n          \"type\": \"string\"\n        },\n        \"TrainingInputMode\": {\n          \"type\": \"string\"\n        },\n        \"AlgorithmName\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"RoleArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the IAM role.\"\n    },\n    \"InputDataConfig\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"ChannelName\": {\n            \"type\": \"string\"\n          },\n          \"DataSource\": {\n            \"type\": \"object\"\n          }\n        }\n      }\n    },\n    \"OutputDataConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"S3OutputPath\": {\n          \"type\": \"string\"\n        },\n        \"\
  KmsKeyId\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"ResourceConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"InstanceType\": {\n          \"type\": \"string\"\n        },\n        \"InstanceCount\": {\n          \"type\": \"integer\"\n        },\n        \"VolumeSizeInGB\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"StoppingCondition\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"MaxRuntimeInSeconds\": {\n          \"type\": \"integer\"\n        },\n        \"MaxWaitTimeInSeconds\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"HyperParameters\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"ModelArtifacts\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"S3ModelArtifacts\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"TrainingStartTime\": {\n\
  \      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"TrainingEndTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"LastModifiedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"BillableTimeInSeconds\": {\n      \"type\": \"integer\"\n    },\n    \"FailureReason\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-sagemaker/refs/heads/main/json-schema/amazon-sagemaker-training-job-schema.json
tags:
- AI
- AWS
- Inference
- Machine Learning
- MLOps
- Training
title: TrainingJob
---
