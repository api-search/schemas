---
description: RetryBuildBatchInput schema from Amazon CodeBuild
layout: schema
name: RetryBuildBatchInput
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: retryType
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-retry-build-batch-input-schema.json
slug: amazon-codebuild-retry-build-batch-input
source_filename: amazon-codebuild-retry-build-batch-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-retry-build-batch-input-schema.json\",\n  \"title\": \"RetryBuildBatchInput\",\n  \"description\": \"RetryBuildBatchInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"Specifies the identifier of the batch build to restart.\"\n        }\n      ]\n    },\n    \"retryType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RetryBuildBatchType\"\n        },\n        {\n          \"description\": \"Specifies the type of retry to perform.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-retry-build-batch-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: RetryBuildBatchInput
---
