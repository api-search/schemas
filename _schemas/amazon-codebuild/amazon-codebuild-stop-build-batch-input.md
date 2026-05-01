---
description: StopBuildBatchInput schema from Amazon CodeBuild
layout: schema
name: StopBuildBatchInput
properties_list:
- description: ''
  name: id
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-stop-build-batch-input-schema.json
slug: amazon-codebuild-stop-build-batch-input
source_filename: amazon-codebuild-stop-build-batch-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-stop-build-batch-input-schema.json\",\n  \"title\": \"StopBuildBatchInput\",\n  \"description\": \"StopBuildBatchInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The identifier of the batch build to stop.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-stop-build-batch-input-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: StopBuildBatchInput
---
