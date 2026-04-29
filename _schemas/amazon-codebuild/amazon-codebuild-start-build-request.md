---
description: StartBuildRequest schema from Amazon CodeBuild
layout: schema
name: StartBuildRequest
properties_list:
- description: The name of the CodeBuild build project.
  name: projectName
  type: string
- description: The version of the build input to be built.
  name: sourceVersion
  type: string
- description: ''
  name: environmentVariablesOverride
  type: array
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-start-build-request-schema.json
slug: amazon-codebuild-start-build-request
source_filename: amazon-codebuild-start-build-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-start-build-request-schema.json\",\n  \"title\": \"StartBuildRequest\",\n  \"description\": \"StartBuildRequest schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"projectName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the CodeBuild build project.\"\n    },\n    \"sourceVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the build input to be built.\"\n    },\n    \"environmentVariablesOverride\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"type\": \"string\"\
  \n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"projectName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-start-build-request-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: StartBuildRequest
---
