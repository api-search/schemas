---
description: CreateRepositoryInput schema from Amazon Proton API
layout: schema
name: CreateRepositoryInput
properties_list:
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
- description: ''
  name: tags
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-create-repository-input-schema.json
slug: amazon-proton-create-repository-input
source_filename: amazon-proton-create-repository-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-create-repository-input-schema.json\",\n  \"title\": \"CreateRepositoryInput\",\n  \"description\": \"CreateRepositoryInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of your AWS CodeStar connection that connects Proton to your repository provider account. For more information, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/userguide/setting-up-for-service.html\\\">Setting up for Proton</a> in the <i>Proton User Guide</i>.\"\n        }\n      ]\n    },\n    \"encryptionKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\
  \n        },\n        {\n          \"description\": \"The ARN of your customer Amazon Web Services Key Management Service (Amazon Web Services KMS) key.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryName\"\n        },\n        {\n          \"description\": \"The repository name (for example, <code>myrepos/myrepo</code>).\"\n        }\n      ]\n    },\n    \"provider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryProvider\"\n        },\n        {\n          \"description\": \"The repository provider.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"<p>An optional list of metadata items that you can associate with the Proton repository. A tag is a key-value pair.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/userguide/resources.html\\\
  \">Proton resources and tagging</a> in the <i>Proton User Guide</i>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"connectionArn\",\n    \"name\",\n    \"provider\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-create-repository-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: CreateRepositoryInput
---
