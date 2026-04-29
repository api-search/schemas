---
description: Detailed data of a linked repository—a repository that has been registered with Proton.
layout: schema
name: Repository
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: connectionArn
  type: object
- description: ''
  name: encryptionKey
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: provider
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-repository-schema.json
slug: amazon-proton-repository
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-repository-schema.json\",\n  \"title\": \"Repository\",\n  \"description\": \"Detailed data of a linked repository\\u2014a repository that has been registered with Proton.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the linked repository.\"\n        }\n      ]\n    },\n    \"connectionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of your AWS CodeStar connection that connects Proton to your repository provider account.\"\n        }\n      ]\n    },\n    \"encryptionKey\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"Your customer Amazon Web Services KMS encryption key.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryName\"\n        },\n        {\n          \"description\": \"The repository name.\"\n        }\n      ]\n    },\n    \"provider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryProvider\"\n        },\n        {\n          \"description\": \"The repository provider.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\",\n    \"connectionArn\",\n    \"name\",\n    \"provider\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-repository-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: Repository
---
