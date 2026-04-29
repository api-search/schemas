---
description: CreateModelTrainingJobRequest schema from Neptune
layout: schema
name: CreateModelTrainingJobRequest
properties_list:
- description: Unique identifier for the job.
  name: id
  type: string
- description: Job ID of the completed data processing job.
  name: dataProcessingJobId
  type: string
- description: S3 location for model artifacts output.
  name: trainModelS3Location
  type: string
- description: Job ID of a previous training job for incremental training.
  name: previousModelTrainingJobId
  type: string
- description: ''
  name: sagemakerIamRoleArn
  type: string
- description: ''
  name: neptuneIamRoleArn
  type: string
- description: 'The model type to train: rgcn (relational graph convolutional network), transe, distmult, rotate, or custom.'
  name: modelName
  type: string
- description: ML instance type for data preparation step.
  name: baseProcessingInstanceType
  type: string
- description: ML instance type for the training step.
  name: trainingInstanceType
  type: string
- description: Disk volume size for training instance in GB.
  name: trainingInstanceVolumeSizeInGB
  type: integer
- description: Training job timeout in seconds.
  name: trainingTimeOutInSeconds
  type: integer
- description: Maximum total training jobs for hyperparameter tuning. Minimum 10 recommended for meaningful results.
  name: maxHPONumberOfTrainingJobs
  type: integer
- description: Maximum parallel training jobs.
  name: maxHPOParallelTrainingJobs
  type: integer
- description: ''
  name: subnets
  type: array
- description: ''
  name: securityGroupIds
  type: array
- description: ''
  name: volumeEncryptionKMSKey
  type: string
- description: ''
  name: s3OutputEncryptionKMSKey
  type: string
- description: ''
  name: enableInterContainerTrafficEncryption
  type: boolean
- description: Whether to use EC2 spot instances for training.
  name: enableManagedSpotTraining
  type: boolean
- description: Custom model training configuration.
  name: customModelTrainingParameters
  type: object
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/ml-create-model-training-job-request-schema.json
slug: ml-create-model-training-job-request
source_filename: ml-create-model-training-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/ml-create-model-training-job-request-schema.json\",\n  \"title\": \"CreateModelTrainingJobRequest\",\n  \"description\": \"CreateModelTrainingJobRequest schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the job.\"\n    },\n    \"dataProcessingJobId\": {\n      \"type\": \"string\",\n      \"description\": \"Job ID of the completed data processing job.\"\n    },\n    \"trainModelS3Location\": {\n      \"type\": \"string\",\n      \"description\": \"S3 location for model artifacts output.\"\n    },\n    \"previousModelTrainingJobId\": {\n      \"type\": \"string\",\n      \"description\": \"Job ID of a previous training job for incremental training.\"\n    },\n    \"sagemakerIamRoleArn\": {\n   \
  \   \"type\": \"string\"\n    },\n    \"neptuneIamRoleArn\": {\n      \"type\": \"string\"\n    },\n    \"modelName\": {\n      \"type\": \"string\",\n      \"description\": \"The model type to train: rgcn (relational graph convolutional network), transe, distmult, rotate, or custom.\",\n      \"enum\": [\n        \"rgcn\",\n        \"transe\",\n        \"distmult\",\n        \"rotate\",\n        \"custom\"\n      ]\n    },\n    \"baseProcessingInstanceType\": {\n      \"type\": \"string\",\n      \"description\": \"ML instance type for data preparation step.\"\n    },\n    \"trainingInstanceType\": {\n      \"type\": \"string\",\n      \"description\": \"ML instance type for the training step.\",\n      \"default\": \"ml.p3.2xlarge\"\n    },\n    \"trainingInstanceVolumeSizeInGB\": {\n      \"type\": \"integer\",\n      \"description\": \"Disk volume size for training instance in GB.\"\n    },\n    \"trainingTimeOutInSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"\
  Training job timeout in seconds.\",\n      \"default\": 86400\n    },\n    \"maxHPONumberOfTrainingJobs\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum total training jobs for hyperparameter tuning. Minimum 10 recommended for meaningful results.\",\n      \"default\": 2\n    },\n    \"maxHPOParallelTrainingJobs\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum parallel training jobs.\",\n      \"default\": 2\n    },\n    \"subnets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"securityGroupIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"volumeEncryptionKMSKey\": {\n      \"type\": \"string\"\n    },\n    \"s3OutputEncryptionKMSKey\": {\n      \"type\": \"string\"\n    },\n    \"enableInterContainerTrafficEncryption\": {\n      \"type\": \"boolean\",\n      \"default\": true\n    },\n    \"enableManagedSpotTraining\": {\n    \
  \  \"type\": \"boolean\",\n      \"description\": \"Whether to use EC2 spot instances for training.\",\n      \"default\": false\n    },\n    \"customModelTrainingParameters\": {\n      \"type\": \"object\",\n      \"description\": \"Custom model training configuration.\",\n      \"properties\": {\n        \"sourceS3DirectoryPath\": {\n          \"type\": \"string\",\n          \"description\": \"S3 path to the custom training script directory.\"\n        },\n        \"trainingEntryPointScript\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the training entry point script.\"\n        },\n        \"transformEntryPointScript\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the transform entry point script.\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"dataProcessingJobId\",\n    \"trainModelS3Location\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/ml-create-model-training-job-request-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: CreateModelTrainingJobRequest
---
