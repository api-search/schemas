---
description: StartMLDataProcessingJobInput schema from Neptune
layout: schema
name: StartMLDataProcessingJobInput
properties_list:
- description: Unique identifier for the job (auto-generated if omitted).
  name: id
  type: string
- description: S3 URI for input data.
  name: inputDataS3Location
  type: string
- description: S3 URI for output results.
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
- description: Disk volume size in GB (default 0 = auto-selected).
  name: processingInstanceVolumeSizeInGB
  type: integer
- description: Timeout in seconds (default 86400).
  name: processingTimeOutInSeconds
  type: integer
- description: Model type selection.
  name: modelType
  type: string
- description: Data specification file name.
  name: configFileName
  type: string
- description: Subnet IDs in Neptune VPC.
  name: subnets
  type: array
- description: VPC security group IDs.
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
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/data-start-ml-data-processing-job-input-schema.json
slug: data-start-ml-data-processing-job-input
source_filename: data-start-ml-data-processing-job-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-start-ml-data-processing-job-input-schema.json\",\n  \"title\": \"StartMLDataProcessingJobInput\",\n  \"description\": \"StartMLDataProcessingJobInput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the job (auto-generated if omitted).\"\n    },\n    \"inputDataS3Location\": {\n      \"type\": \"string\",\n      \"description\": \"S3 URI for input data.\"\n    },\n    \"processedDataS3Location\": {\n      \"type\": \"string\",\n      \"description\": \"S3 URI for output results.\"\n    },\n    \"previousDataProcessingJobId\": {\n      \"type\": \"string\",\n      \"description\": \"Job ID of a previous job for incremental processing.\"\n    },\n    \"sagemakerIamRoleArn\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"IAM role ARN for SageMaker execution.\"\n    },\n    \"neptuneIamRoleArn\": {\n      \"type\": \"string\",\n      \"description\": \"IAM role ARN for Neptune access.\"\n    },\n    \"processingInstanceType\": {\n      \"type\": \"string\",\n      \"description\": \"ML instance type (default auto-selected ml.r5 type).\"\n    },\n    \"processingInstanceVolumeSizeInGB\": {\n      \"type\": \"integer\",\n      \"description\": \"Disk volume size in GB (default 0 = auto-selected).\"\n    },\n    \"processingTimeOutInSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Timeout in seconds (default 86400).\"\n    },\n    \"modelType\": {\n      \"type\": \"string\",\n      \"description\": \"Model type selection.\",\n      \"enum\": [\n        \"heterogeneous\",\n        \"kge\"\n      ]\n    },\n    \"configFileName\": {\n      \"type\": \"string\",\n      \"description\": \"Data specification file name.\",\n      \"default\": \"training-data-configuration.json\"\
  \n    },\n    \"subnets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Subnet IDs in Neptune VPC.\"\n    },\n    \"securityGroupIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"VPC security group IDs.\"\n    },\n    \"volumeEncryptionKMSKey\": {\n      \"type\": \"string\"\n    },\n    \"s3OutputEncryptionKMSKey\": {\n      \"type\": \"string\"\n    },\n    \"enableInterContainerTrafficEncryption\": {\n      \"type\": \"boolean\",\n      \"default\": true\n    }\n  },\n  \"required\": [\n    \"inputDataS3Location\",\n    \"processedDataS3Location\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-start-ml-data-processing-job-input-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: StartMLDataProcessingJobInput
---
