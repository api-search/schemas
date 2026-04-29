---
description: Repository schema from Amazon ECR Amazon Elastic Container Registry (ECR) API
layout: schema
name: Repository
properties_list:
- description: The Amazon Resource Name (ARN) of the repository.
  name: repositoryArn
  type: string
- description: The AWS account ID associated with the registry.
  name: registryId
  type: string
- description: The name of the repository.
  name: repositoryName
  type: string
- description: The URI for the repository.
  name: repositoryUri
  type: string
- description: The date and time the repository was created.
  name: createdAt
  type: string
- description: The tag mutability setting for the repository.
  name: imageTagMutability
  type: string
- description: The image scanning configuration for the repository.
  name: imageScanningConfiguration
  type: object
- description: The encryption configuration for the repository.
  name: encryptionConfiguration
  type: object
provider_name: Amazon ECR
provider_slug: amazon-ecr
schema_file: json-schema/ecr-openapi-repository-schema.json
slug: ecr-openapi-repository
source_filename: ecr-openapi-repository-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ecr/refs/heads/main/json-schema/ecr-openapi-repository-schema.json\",\n  \"title\": \"Repository\",\n  \"description\": \"Repository schema from Amazon ECR Amazon Elastic Container Registry (ECR) API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"repositoryArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the repository.\"\n    },\n    \"registryId\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS account ID associated with the registry.\"\n    },\n    \"repositoryName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the repository.\"\n    },\n    \"repositoryUri\": {\n      \"type\": \"string\",\n      \"description\": \"The URI for the repository.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"The date and time the repository was created.\"\n    },\n    \"imageTagMutability\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"MUTABLE\",\n        \"IMMUTABLE\"\n      ],\n      \"description\": \"The tag mutability setting for the repository.\"\n    },\n    \"imageScanningConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"scanOnPush\": {\n          \"type\": \"boolean\"\n        }\n      },\n      \"description\": \"The image scanning configuration for the repository.\"\n    },\n    \"encryptionConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"encryptionType\": {\n          \"type\": \"string\"\n        },\n        \"kmsKey\": {\n          \"type\": \"string\"\n        }\n      },\n      \"description\": \"The encryption configuration for the repository.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecr/refs/heads/main/json-schema/ecr-openapi-repository-schema.json
tags:
- Amazon Web Services
- AWS
- Container Images
- Container Registry
- Containers
- Docker
- ECR
- OCI
title: Repository
---
