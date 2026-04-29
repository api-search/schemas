---
description: SourceConfiguration schema from AWS App Runner
layout: schema
name: SourceConfiguration
properties_list:
- description: ''
  name: CodeRepository
  type: object
- description: ''
  name: ImageRepository
  type: object
- description: ''
  name: AutoDeploymentsEnabled
  type: boolean
- description: ''
  name: AuthenticationConfiguration
  type: object
provider_name: AWS App Runner
provider_slug: aws-app-runner
schema_file: json-schema/app-runner-source-configuration-schema.json
slug: app-runner-source-configuration
source_filename: app-runner-source-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"CodeRepository\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"RepositoryUrl\": {\n          \"type\": \"string\"\n        },\n        \"SourceCodeVersion\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"Type\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"BRANCH\"\n              ]\n            },\n            \"Value\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"CodeConfiguration\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"ConfigurationSource\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"REPOSITORY\",\n                \"API\"\n              ]\n            },\n            \"CodeConfigurationValues\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Runtime\": {\n\
  \                  \"type\": \"string\",\n                  \"enum\": [\n                    \"PYTHON_3\",\n                    \"NODEJS_12\",\n                    \"NODEJS_14\",\n                    \"NODEJS_16\",\n                    \"NODEJS_18\",\n                    \"CORRETTO_8\",\n                    \"CORRETTO_11\",\n                    \"GO_1\",\n                    \"DOTNET_6\",\n                    \"PHP_81\",\n                    \"RUBY_31\"\n                  ]\n                },\n                \"BuildCommand\": {\n                  \"type\": \"string\"\n                },\n                \"StartCommand\": {\n                  \"type\": \"string\"\n                },\n                \"Port\": {\n                  \"type\": \"string\"\n                },\n                \"RuntimeEnvironmentVariables\": {\n                  \"type\": \"object\",\n                  \"additionalProperties\": {\n                    \"type\": \"string\"\n                  }\n             \
  \   },\n                \"RuntimeEnvironmentSecrets\": {\n                  \"type\": \"object\",\n                  \"additionalProperties\": {\n                    \"type\": \"string\"\n                  }\n                }\n              }\n            }\n          }\n        },\n        \"SourceDirectory\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"ImageRepository\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ImageIdentifier\": {\n          \"type\": \"string\"\n        },\n        \"ImageConfiguration\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"RuntimeEnvironmentVariables\": {\n              \"type\": \"object\",\n              \"additionalProperties\": {\n                \"type\": \"string\"\n              }\n            },\n            \"RuntimeEnvironmentSecrets\": {\n              \"type\": \"object\",\n              \"additionalProperties\": {\n                \"type\": \"string\"\n    \
  \          }\n            },\n            \"StartCommand\": {\n              \"type\": \"string\"\n            },\n            \"Port\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"ImageRepositoryType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"ECR\",\n            \"ECR_PUBLIC\"\n          ]\n        }\n      }\n    },\n    \"AutoDeploymentsEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"AuthenticationConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ConnectionArn\": {\n          \"type\": \"string\"\n        },\n        \"AccessRoleArn\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-source-configuration-schema.json\",\n  \"title\": \"SourceConfiguration\",\n  \"description\"\
  : \"SourceConfiguration schema from AWS App Runner\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-source-configuration-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Microservices
- Serverless
title: SourceConfiguration
---
