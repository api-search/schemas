---
description: CreateModelTransformJobRequest schema from Neptune
layout: schema
name: CreateModelTransformJobRequest
properties_list:
- description: ''
  name: id
  type: string
- description: Job ID of the completed data processing job.
  name: dataProcessingJobId
  type: string
- description: Job ID of the completed model training job.
  name: mlModelTrainingJobId
  type: string
- description: Name of a completed SageMaker training job.
  name: trainingJobName
  type: string
- description: S3 location for transform output artifacts.
  name: modelTransformOutputS3Location
  type: string
- description: ''
  name: sagemakerIamRoleArn
  type: string
- description: ''
  name: neptuneIamRoleArn
  type: string
- description: ''
  name: baseProcessingInstanceType
  type: string
- description: ''
  name: baseProcessingInstanceVolumeSizeInGB
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
  name: customModelTransformParameters
  type: object
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/ml-create-model-transform-job-request-schema.json
slug: ml-create-model-transform-job-request
source_filename: ml-create-model-transform-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/ml-create-model-transform-job-request-schema.json\",\n  \"title\": \"CreateModelTransformJobRequest\",\n  \"description\": \"CreateModelTransformJobRequest schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"dataProcessingJobId\": {\n      \"type\": \"string\",\n      \"description\": \"Job ID of the completed data processing job.\"\n    },\n    \"mlModelTrainingJobId\": {\n      \"type\": \"string\",\n      \"description\": \"Job ID of the completed model training job.\"\n    },\n    \"trainingJobName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of a completed SageMaker training job.\"\n    },\n    \"modelTransformOutputS3Location\": {\n      \"type\": \"string\",\n      \"description\": \"S3 location for transform\
  \ output artifacts.\"\n    },\n    \"sagemakerIamRoleArn\": {\n      \"type\": \"string\"\n    },\n    \"neptuneIamRoleArn\": {\n      \"type\": \"string\"\n    },\n    \"baseProcessingInstanceType\": {\n      \"type\": \"string\"\n    },\n    \"baseProcessingInstanceVolumeSizeInGB\": {\n      \"type\": \"integer\"\n    },\n    \"subnets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"securityGroupIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"volumeEncryptionKMSKey\": {\n      \"type\": \"string\"\n    },\n    \"s3OutputEncryptionKMSKey\": {\n      \"type\": \"string\"\n    },\n    \"enableInterContainerTrafficEncryption\": {\n      \"type\": \"boolean\",\n      \"default\": true\n    },\n    \"customModelTransformParameters\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"sourceS3DirectoryPath\": {\n          \"type\": \"string\"\n        },\n\
  \        \"transformEntryPointScript\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"modelTransformOutputS3Location\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/ml-create-model-transform-job-request-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: CreateModelTransformJobRequest
---
