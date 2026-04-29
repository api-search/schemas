---
description: Detailed data of an Proton service resource.
layout: schema
name: Service
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: branchName
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: lastModifiedAt
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: pipeline
  type: object
- description: ''
  name: repositoryConnectionArn
  type: object
- description: ''
  name: repositoryId
  type: object
- description: ''
  name: spec
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: statusMessage
  type: object
- description: ''
  name: templateName
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-service-schema.json
slug: amazon-proton-service
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-service-schema.json\",\n  \"title\": \"Service\",\n  \"description\": \"Detailed data of an Proton service resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the service.\"\n        }\n      ]\n    },\n    \"branchName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GitBranchName\"\n        },\n        {\n          \"description\": \"The name of the code repository branch that holds the code that's deployed in Proton.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n       \
  \ },\n        {\n          \"description\": \"The time when the service was created.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description of the service.\"\n        }\n      ]\n    },\n    \"lastModifiedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the service was last modified.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service.\"\n        }\n      ]\n    },\n    \"pipeline\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServicePipeline\"\n        },\n        {\n          \"description\": \"The service pipeline detail data.\"\
  \n        }\n      ]\n    },\n    \"repositoryConnectionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the repository connection. For more information, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/userguide/setting-up-for-service.html#setting-up-vcontrol\\\">Setting up an AWS CodeStar connection</a> in the <i>Proton User Guide</i>.\"\n        }\n      ]\n    },\n    \"repositoryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryId\"\n        },\n        {\n          \"description\": \"The ID of the source code repository.\"\n        }\n      ]\n    },\n    \"spec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpecContents\"\n        },\n        {\n          \"description\": \"The formatted specification that defines the service.\"\n        }\n      ]\n    },\n    \"status\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceStatus\"\n        },\n        {\n          \"description\": \"The status of the service.\"\n        }\n      ]\n    },\n    \"statusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusMessage\"\n        },\n        {\n          \"description\": \"A service status message.\"\n        }\n      ]\n    },\n    \"templateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service template.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\",\n    \"createdAt\",\n    \"lastModifiedAt\",\n    \"name\",\n    \"spec\",\n    \"status\",\n    \"templateName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-service-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: Service
---
