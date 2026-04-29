---
description: CreateProjectRequest schema from Amazon CodeBuild
layout: schema
name: CreateProjectRequest
properties_list:
- description: The name of the build project.
  name: name
  type: string
- description: A description of the build project.
  name: description
  type: string
- description: ''
  name: source
  type: object
- description: ''
  name: environment
  type: object
- description: The ARN of the IAM role for CodeBuild.
  name: serviceRole
  type: string
- description: Build timeout in minutes.
  name: timeoutInMinutes
  type: integer
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-create-project-request-schema.json
slug: amazon-codebuild-create-project-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-create-project-request-schema.json\",\n  \"title\": \"CreateProjectRequest\",\n  \"description\": \"CreateProjectRequest schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the build project.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the build project.\"\n    },\n    \"source\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"type\"\n      ],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"CODECOMMIT\",\n            \"CODEPIPELINE\",\n            \"GITHUB\",\n            \"GITHUB_ENTERPRISE\",\n            \"BITBUCKET\",\n      \
  \      \"S3\",\n            \"NO_SOURCE\"\n          ]\n        },\n        \"location\": {\n          \"type\": \"string\"\n        },\n        \"buildspec\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"environment\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"type\",\n        \"image\",\n        \"computeType\"\n      ],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"WINDOWS_CONTAINER\",\n            \"LINUX_CONTAINER\",\n            \"LINUX_GPU_CONTAINER\",\n            \"ARM_CONTAINER\"\n          ]\n        },\n        \"image\": {\n          \"type\": \"string\"\n        },\n        \"computeType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"BUILD_GENERAL1_SMALL\",\n            \"BUILD_GENERAL1_MEDIUM\",\n            \"BUILD_GENERAL1_LARGE\",\n            \"BUILD_GENERAL1_2XLARGE\"\n          ]\n        },\n        \"environmentVariables\"\
  : {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"value\": {\n                \"type\": \"string\"\n              },\n              \"type\": {\n                \"type\": \"string\",\n                \"enum\": [\n                  \"PLAINTEXT\",\n                  \"PARAMETER_STORE\",\n                  \"SECRETS_MANAGER\"\n                ]\n              }\n            }\n          }\n        }\n      }\n    },\n    \"serviceRole\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the IAM role for CodeBuild.\"\n    },\n    \"timeoutInMinutes\": {\n      \"type\": \"integer\",\n      \"description\": \"Build timeout in minutes.\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"source\",\n    \"environment\",\n    \"serviceRole\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-create-project-request-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: CreateProjectRequest
---
