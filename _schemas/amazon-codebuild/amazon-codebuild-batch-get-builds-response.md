---
description: BatchGetBuildsResponse schema from Amazon CodeBuild
layout: schema
name: BatchGetBuildsResponse
properties_list:
- description: ''
  name: builds
  type: array
- description: ''
  name: buildsNotFound
  type: array
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-batch-get-builds-response-schema.json
slug: amazon-codebuild-batch-get-builds-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-get-builds-response-schema.json\",\n  \"title\": \"BatchGetBuildsResponse\",\n  \"description\": \"BatchGetBuildsResponse schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"builds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Build\"\n      }\n    },\n    \"buildsNotFound\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-get-builds-response-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: BatchGetBuildsResponse
---
