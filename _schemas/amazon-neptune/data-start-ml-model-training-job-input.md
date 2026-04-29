---
description: StartMLModelTrainingJobInput schema from Neptune
layout: schema
name: StartMLModelTrainingJobInput
properties_list:
- description: ''
  name: id
  type: string
- description: Job ID of the completed data processing job.
  name: dataProcessingJobId
  type: string
- description: S3 location for model artifacts.
  name: trainModelS3Location
  type: string
- description: ''
  name: previousModelTrainingJobId
  type: string
- description: ''
  name: sagemakerIamRoleArn
  type: string
- description: ''
  name: neptuneIamRoleArn
  type: string
- description: The model type to use.
  name: modelName
  type: string
- description: ''
  name: baseProcessingInstanceType
  type: string
- description: ''
  name: trainingInstanceType
  type: string
- description: ''
  name: trainingInstanceVolumeSizeInGB
  type: integer
- description: ''
  name: trainingTimeOutInSeconds
  type: integer
- description: ''
  name: maxHPONumberOfTrainingJobs
  type: integer
- description: ''
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
- description: ''
  name: enableManagedSpotTraining
  type: boolean
- description: ''
  name: customModelTrainingParameters
  type: object
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/data-start-ml-model-training-job-input-schema.json
slug: data-start-ml-model-training-job-input
source_filename: data-start-ml-model-training-job-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-start-ml-model-training-job-input-schema.json\",\n  \"title\": \"StartMLModelTrainingJobInput\",\n  \"description\": \"StartMLModelTrainingJobInput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"dataProcessingJobId\": {\n      \"type\": \"string\",\n      \"description\": \"Job ID of the completed data processing job.\"\n    },\n    \"trainModelS3Location\": {\n      \"type\": \"string\",\n      \"description\": \"S3 location for model artifacts.\"\n    },\n    \"previousModelTrainingJobId\": {\n      \"type\": \"string\"\n    },\n    \"sagemakerIamRoleArn\": {\n      \"type\": \"string\"\n    },\n    \"neptuneIamRoleArn\": {\n      \"type\": \"string\"\n    },\n    \"modelName\": {\n      \"type\": \"string\",\n      \"\
  description\": \"The model type to use.\",\n      \"enum\": [\n        \"rgcn\",\n        \"transe\",\n        \"distmult\",\n        \"rotate\",\n        \"custom\"\n      ]\n    },\n    \"baseProcessingInstanceType\": {\n      \"type\": \"string\"\n    },\n    \"trainingInstanceType\": {\n      \"type\": \"string\",\n      \"default\": \"ml.p3.2xlarge\"\n    },\n    \"trainingInstanceVolumeSizeInGB\": {\n      \"type\": \"integer\"\n    },\n    \"trainingTimeOutInSeconds\": {\n      \"type\": \"integer\",\n      \"default\": 86400\n    },\n    \"maxHPONumberOfTrainingJobs\": {\n      \"type\": \"integer\",\n      \"default\": 2\n    },\n    \"maxHPOParallelTrainingJobs\": {\n      \"type\": \"integer\",\n      \"default\": 2\n    },\n    \"subnets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"securityGroupIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"volumeEncryptionKMSKey\"\
  : {\n      \"type\": \"string\"\n    },\n    \"s3OutputEncryptionKMSKey\": {\n      \"type\": \"string\"\n    },\n    \"enableInterContainerTrafficEncryption\": {\n      \"type\": \"boolean\",\n      \"default\": true\n    },\n    \"enableManagedSpotTraining\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"customModelTrainingParameters\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"sourceS3DirectoryPath\": {\n          \"type\": \"string\"\n        },\n        \"trainingEntryPointScript\": {\n          \"type\": \"string\"\n        },\n        \"transformEntryPointScript\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"dataProcessingJobId\",\n    \"trainModelS3Location\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-start-ml-model-training-job-input-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: StartMLModelTrainingJobInput
---
