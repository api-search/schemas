---
description: CreateDataProcessingJobRequest schema from Neptune
layout: schema
name: CreateDataProcessingJobRequest
properties_list:
- description: Unique identifier for the job (auto-generated UUID if omitted).
  name: id
  type: string
- description: S3 URI for the input data.
  name: inputDataS3Location
  type: string
- description: S3 URI where processed output is written.
  name: processedDataS3Location
  type: string
- description: Job ID of a previous job for incremental processing.
  name: previousDataProcessingJobId
  type: string
- description: IAM role ARN for SageMaker execution.
  name: sagemakerIamRoleArn
  type: string
- description: IAM role ARN for Neptune access.
  name: neptuneIamRoleArn
  type: string
- description: ML instance type (default auto-selected ml.r5 type).
  name: processingInstanceType
  type: string
- description: Disk volume size in GB (default 0 means auto-selected).
  name: processingInstanceVolumeSizeInGB
  type: integer
- description: Timeout in seconds (default 86400, i.e., 1 day).
  name: processingTimeOutInSeconds
  type: integer
- description: The type of model to prepare data for.
  name: modelType
  type: string
- description: The data specification configuration file name.
  name: configFileName
  type: string
- description: VPC subnet IDs for SageMaker processing.
  name: subnets
  type: array
- description: VPC security group IDs.
  name: securityGroupIds
  type: array
- description: KMS key for storage volume encryption.
  name: volumeEncryptionKMSKey
  type: string
- description: KMS key for S3 output encryption.
  name: s3OutputEncryptionKMSKey
  type: string
- description: Whether to enable inter-container traffic encryption.
  name: enableInterContainerTrafficEncryption
  type: boolean
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/ml-create-data-processing-job-request-schema.json
slug: ml-create-data-processing-job-request
source_filename: ml-create-data-processing-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/ml-create-data-processing-job-request-schema.json\",\n  \"title\": \"CreateDataProcessingJobRequest\",\n  \"description\": \"CreateDataProcessingJobRequest schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the job (auto-generated UUID if omitted).\"\n    },\n    \"inputDataS3Location\": {\n      \"type\": \"string\",\n      \"description\": \"S3 URI for the input data.\"\n    },\n    \"processedDataS3Location\": {\n      \"type\": \"string\",\n      \"description\": \"S3 URI where processed output is written.\"\n    },\n    \"previousDataProcessingJobId\": {\n      \"type\": \"string\",\n      \"description\": \"Job ID of a previous job for incremental processing.\"\n    },\n    \"sagemakerIamRoleArn\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"IAM role ARN for SageMaker execution.\"\n    },\n    \"neptuneIamRoleArn\": {\n      \"type\": \"string\",\n      \"description\": \"IAM role ARN for Neptune access.\"\n    },\n    \"processingInstanceType\": {\n      \"type\": \"string\",\n      \"description\": \"ML instance type (default auto-selected ml.r5 type).\"\n    },\n    \"processingInstanceVolumeSizeInGB\": {\n      \"type\": \"integer\",\n      \"description\": \"Disk volume size in GB (default 0 means auto-selected).\"\n    },\n    \"processingTimeOutInSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Timeout in seconds (default 86400, i.e., 1 day).\",\n      \"default\": 86400\n    },\n    \"modelType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of model to prepare data for.\",\n      \"enum\": [\n        \"heterogeneous\",\n        \"kge\"\n      ]\n    },\n    \"configFileName\": {\n      \"type\": \"string\",\n      \"\
  description\": \"The data specification configuration file name.\",\n      \"default\": \"training-data-configuration.json\"\n    },\n    \"subnets\": {\n      \"type\": \"array\",\n      \"description\": \"VPC subnet IDs for SageMaker processing.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"securityGroupIds\": {\n      \"type\": \"array\",\n      \"description\": \"VPC security group IDs.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"volumeEncryptionKMSKey\": {\n      \"type\": \"string\",\n      \"description\": \"KMS key for storage volume encryption.\"\n    },\n    \"s3OutputEncryptionKMSKey\": {\n      \"type\": \"string\",\n      \"description\": \"KMS key for S3 output encryption.\"\n    },\n    \"enableInterContainerTrafficEncryption\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable inter-container traffic encryption.\",\n      \"default\": true\n    }\n  },\n  \"required\": [\n    \"inputDataS3Location\"\
  ,\n    \"processedDataS3Location\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/ml-create-data-processing-job-request-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: CreateDataProcessingJobRequest
---
