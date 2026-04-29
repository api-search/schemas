---
description: Detailed data of the service sync configuration.
layout: schema
name: ServiceSyncConfig
properties_list:
- description: ''
  name: branch
  type: object
- description: ''
  name: filePath
  type: object
- description: ''
  name: repositoryName
  type: object
- description: ''
  name: repositoryProvider
  type: object
- description: ''
  name: serviceName
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-service-sync-config-schema.json
slug: amazon-proton-service-sync-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-service-sync-config-schema.json\",\n  \"title\": \"ServiceSyncConfig\",\n  \"description\": \"Detailed data of the service sync configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"branch\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GitBranchName\"\n        },\n        {\n          \"description\": \"The name of the code repository branch that holds the service code Proton will sync with.\"\n        }\n      ]\n    },\n    \"filePath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OpsFilePath\"\n        },\n        {\n          \"description\": \"The file path to the service sync configuration file.\"\n        }\n      ]\n    },\n    \"repositoryName\": {\n      \"allOf\": [\n        {\n          \"$ref\":\
  \ \"#/components/schemas/RepositoryName\"\n        },\n        {\n          \"description\": \"The name of the code repository that holds the service code Proton will sync with.\"\n        }\n      ]\n    },\n    \"repositoryProvider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryProvider\"\n        },\n        {\n          \"description\": \"The name of the repository provider that holds the repository Proton will sync with.\"\n        }\n      ]\n    },\n    \"serviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service that the service instance is added to.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"branch\",\n    \"filePath\",\n    \"repositoryName\",\n    \"repositoryProvider\",\n    \"serviceName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-service-sync-config-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ServiceSyncConfig
---
