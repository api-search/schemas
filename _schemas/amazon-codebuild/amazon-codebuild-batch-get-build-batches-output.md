---
description: BatchGetBuildBatchesOutput schema from Amazon CodeBuild
layout: schema
name: BatchGetBuildBatchesOutput
properties_list:
- description: ''
  name: buildBatches
  type: object
- description: ''
  name: buildBatchesNotFound
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-batch-get-build-batches-output-schema.json
slug: amazon-codebuild-batch-get-build-batches-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-get-build-batches-output-schema.json\",\n  \"title\": \"BatchGetBuildBatchesOutput\",\n  \"description\": \"BatchGetBuildBatchesOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"buildBatches\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildBatches\"\n        },\n        {\n          \"description\": \"An array of <code>BuildBatch</code> objects that represent the retrieved batch builds.\"\n        }\n      ]\n    },\n    \"buildBatchesNotFound\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildBatchIds\"\n        },\n        {\n          \"description\": \"An array that contains the identifiers of any batch builds that are not found.\"\n        }\n      ]\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-get-build-batches-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: BatchGetBuildBatchesOutput
---
