---
description: ListBuildBatchesForProjectOutput schema from Amazon CodeBuild
layout: schema
name: ListBuildBatchesForProjectOutput
properties_list:
- description: ''
  name: ids
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-list-build-batches-for-project-output-schema.json
slug: amazon-codebuild-list-build-batches-for-project-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-list-build-batches-for-project-output-schema.json\",\n  \"title\": \"ListBuildBatchesForProjectOutput\",\n  \"description\": \"ListBuildBatchesForProjectOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ids\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildBatchIds\"\n        },\n        {\n          \"description\": \"An array of strings that contains the batch build identifiers.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"If there are more items to return, this contains a token that is passed to a subsequent call to <code>ListBuildBatchesForProject</code> to retrieve\
  \ the next set of items.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-list-build-batches-for-project-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ListBuildBatchesForProjectOutput
---
