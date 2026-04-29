---
description: BatchGetBuildBatchesInput schema from Amazon CodeBuild
layout: schema
name: BatchGetBuildBatchesInput
properties_list:
- description: ''
  name: ids
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-batch-get-build-batches-input-schema.json
slug: amazon-codebuild-batch-get-build-batches-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-get-build-batches-input-schema.json\",\n  \"title\": \"BatchGetBuildBatchesInput\",\n  \"description\": \"BatchGetBuildBatchesInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ids\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildBatchIds\"\n        },\n        {\n          \"description\": \"An array that contains the batch build identifiers to retrieve.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ids\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-get-build-batches-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: BatchGetBuildBatchesInput
---
