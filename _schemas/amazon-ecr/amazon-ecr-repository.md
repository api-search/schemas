---
description: Schema representing an Amazon Elastic Container Registry repository, which stores Docker container images and OCI artifacts.
layout: schema
name: Amazon ECR Repository
properties_list:
- description: The Amazon Resource Name (ARN) that identifies the repository.
  name: repositoryArn
  type: string
- description: The AWS account ID associated with the registry that contains the repository.
  name: registryId
  type: string
- description: The name of the repository.
  name: repositoryName
  type: string
- description: The URI for the repository, used for docker pull and push operations.
  name: repositoryUri
  type: string
- description: The date and time, in JavaScript date format, when the repository was created.
  name: createdAt
  type: string
- description: The tag mutability setting for the repository. When set to IMMUTABLE, all image tags within the repository are prevented from being overwritten.
  name: imageTagMutability
  type: string
- description: The image scanning configuration for the repository.
  name: imageScanningConfiguration
  type: object
- description: The encryption configuration for the repository.
  name: encryptionConfiguration
  type: object
- description: The number of images in the repository.
  name: imageCount
  type: integer
- description: The JSON repository policy text associated with the repository.
  name: repositoryPolicy
  type: string
- description: The lifecycle policy for the repository.
  name: lifecyclePolicy
  type: object
- description: The metadata tags applied to the repository.
  name: tags
  type: array
provider_name: Amazon ECR
provider_slug: amazon-ecr
schema_file: json-schema/amazon-ecr-repository-schema.json
slug: amazon-ecr-repository
source_filename: amazon-ecr-repository-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.apis.io/schemas/amazon-ecr-repository.json\",\n  \"title\": \"Amazon ECR Repository\",\n  \"description\": \"Schema representing an Amazon Elastic Container Registry repository, which stores Docker container images and OCI artifacts.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"repositoryName\"\n  ],\n  \"properties\": {\n    \"repositoryArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) that identifies the repository.\",\n      \"pattern\": \"^arn:aws[a-zA-Z-]*:ecr:[a-z0-9-]+:[0-9]{12}:repository/.+$\"\n    },\n    \"registryId\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS account ID associated with the registry that contains the repository.\",\n      \"pattern\": \"^[0-9]{12}$\"\n    },\n    \"repositoryName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the repository.\",\n      \"\
  minLength\": 2,\n      \"maxLength\": 256,\n      \"pattern\": \"^(?:[a-z0-9]+(?:[._-][a-z0-9]+)*/)*[a-z0-9]+(?:[._-][a-z0-9]+)*$\"\n    },\n    \"repositoryUri\": {\n      \"type\": \"string\",\n      \"description\": \"The URI for the repository, used for docker pull and push operations.\",\n      \"format\": \"uri\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time, in JavaScript date format, when the repository was created.\"\n    },\n    \"imageTagMutability\": {\n      \"type\": \"string\",\n      \"description\": \"The tag mutability setting for the repository. When set to IMMUTABLE, all image tags within the repository are prevented from being overwritten.\",\n      \"enum\": [\n        \"MUTABLE\",\n        \"IMMUTABLE\"\n      ],\n      \"default\": \"MUTABLE\"\n    },\n    \"imageScanningConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"The image scanning configuration\
  \ for the repository.\",\n      \"properties\": {\n        \"scanOnPush\": {\n          \"type\": \"boolean\",\n          \"description\": \"The setting that determines whether images are scanned after being pushed to a repository.\",\n          \"default\": false\n        }\n      }\n    },\n    \"encryptionConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"The encryption configuration for the repository.\",\n      \"required\": [\n        \"encryptionType\"\n      ],\n      \"properties\": {\n        \"encryptionType\": {\n          \"type\": \"string\",\n          \"description\": \"The encryption type to use.\",\n          \"enum\": [\n            \"AES256\",\n            \"KMS\"\n          ]\n        },\n        \"kmsKey\": {\n          \"type\": \"string\",\n          \"description\": \"If you use the KMS encryption type, specify the KMS key to use for encryption.\"\n        }\n      }\n    },\n    \"imageCount\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"The number of images in the repository.\",\n      \"minimum\": 0\n    },\n    \"repositoryPolicy\": {\n      \"type\": \"string\",\n      \"description\": \"The JSON repository policy text associated with the repository.\"\n    },\n    \"lifecyclePolicy\": {\n      \"type\": \"object\",\n      \"description\": \"The lifecycle policy for the repository.\",\n      \"properties\": {\n        \"lifecyclePolicyText\": {\n          \"type\": \"string\",\n          \"description\": \"The JSON lifecycle policy text.\"\n        },\n        \"registryId\": {\n          \"type\": \"string\",\n          \"description\": \"The registry ID associated with the lifecycle policy.\"\n        },\n        \"repositoryName\": {\n          \"type\": \"string\",\n          \"description\": \"The repository name associated with the lifecycle policy.\"\n        },\n        \"lastEvaluatedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The time stamp\
  \ of the last time the lifecycle policy was run.\"\n        }\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"The metadata tags applied to the repository.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\n          \"Key\",\n          \"Value\"\n        ],\n        \"properties\": {\n          \"Key\": {\n            \"type\": \"string\",\n            \"description\": \"The key of the tag.\",\n            \"minLength\": 1,\n            \"maxLength\": 128\n          },\n          \"Value\": {\n            \"type\": \"string\",\n            \"description\": \"The value of the tag.\",\n            \"minLength\": 0,\n            \"maxLength\": 256\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecr/refs/heads/main/json-schema/amazon-ecr-repository-schema.json
tags:
- Amazon Web Services
- Container Images
- Container Registry
- Containers
- Docker
- ECR
- OCI
title: Amazon ECR Repository
---
