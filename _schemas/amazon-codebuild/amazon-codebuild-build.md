---
description: Build schema from Amazon CodeBuild
layout: schema
name: Build
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: arn
  type: string
- description: ''
  name: buildNumber
  type: integer
- description: ''
  name: startTime
  type: string
- description: ''
  name: endTime
  type: string
- description: ''
  name: currentPhase
  type: string
- description: ''
  name: buildStatus
  type: string
- description: ''
  name: projectName
  type: string
- description: ''
  name: sourceVersion
  type: string
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-build-schema.json
slug: amazon-codebuild-build
source_filename: amazon-codebuild-build-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-build-schema.json\",\n  \"title\": \"Build\",\n  \"description\": \"Build schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"arn\": {\n      \"type\": \"string\"\n    },\n    \"buildNumber\": {\n      \"type\": \"integer\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"currentPhase\": {\n      \"type\": \"string\"\n    },\n    \"buildStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SUCCEEDED\",\n        \"FAILED\",\n        \"FAULT\",\n        \"TIMED_OUT\",\n        \"IN_PROGRESS\",\n        \"STOPPED\"\n      ]\n    },\n    \"projectName\"\
  : {\n      \"type\": \"string\"\n    },\n    \"sourceVersion\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-build-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: Build
---
