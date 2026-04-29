---
description: CreateInferenceEndpointRequest schema from Neptune
layout: schema
name: CreateInferenceEndpointRequest
properties_list:
- description: Unique identifier for the endpoint (auto-generated timestamped name if omitted).
  name: id
  type: string
- description: Job ID from a completed training job.
  name: mlModelTrainingJobId
  type: string
- description: Job ID from a completed transform job.
  name: mlModelTransformJobId
  type: string
- description: Whether this is an update to an existing endpoint.
  name: update
  type: boolean
- description: ''
  name: neptuneIamRoleArn
  type: string
- description: The model type.
  name: modelName
  type: string
- description: ML instance type for the inference endpoint.
  name: instanceType
  type: string
- description: Minimum number of EC2 instances to deploy.
  name: instanceCount
  type: integer
- description: ''
  name: volumeEncryptionKMSKey
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/ml-create-inference-endpoint-request-schema.json
slug: ml-create-inference-endpoint-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/ml-create-inference-endpoint-request-schema.json\",\n  \"title\": \"CreateInferenceEndpointRequest\",\n  \"description\": \"CreateInferenceEndpointRequest schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the endpoint (auto-generated timestamped name if omitted).\"\n    },\n    \"mlModelTrainingJobId\": {\n      \"type\": \"string\",\n      \"description\": \"Job ID from a completed training job.\"\n    },\n    \"mlModelTransformJobId\": {\n      \"type\": \"string\",\n      \"description\": \"Job ID from a completed transform job.\"\n    },\n    \"update\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is an update to an existing endpoint.\",\n      \"default\": false\n\
  \    },\n    \"neptuneIamRoleArn\": {\n      \"type\": \"string\"\n    },\n    \"modelName\": {\n      \"type\": \"string\",\n      \"description\": \"The model type.\",\n      \"enum\": [\n        \"rgcn\",\n        \"kge\",\n        \"transe\",\n        \"distmult\",\n        \"rotate\"\n      ]\n    },\n    \"instanceType\": {\n      \"type\": \"string\",\n      \"description\": \"ML instance type for the inference endpoint.\",\n      \"default\": \"ml.m5.xlarge\"\n    },\n    \"instanceCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Minimum number of EC2 instances to deploy.\",\n      \"default\": 1\n    },\n    \"volumeEncryptionKMSKey\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/ml-create-inference-endpoint-request-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: CreateInferenceEndpointRequest
---
