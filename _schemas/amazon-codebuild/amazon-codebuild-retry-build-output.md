---
description: RetryBuildOutput schema from Amazon CodeBuild
layout: schema
name: RetryBuildOutput
properties_list:
- description: ''
  name: build
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-retry-build-output-schema.json
slug: amazon-codebuild-retry-build-output
source_filename: amazon-codebuild-retry-build-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-retry-build-output-schema.json\",\n  \"title\": \"RetryBuildOutput\",\n  \"description\": \"RetryBuildOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"build\": {\n      \"$ref\": \"#/components/schemas/Build\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-retry-build-output-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: RetryBuildOutput
---
