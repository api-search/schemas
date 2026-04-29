---
description: StartBuildBatchOutput schema from Amazon CodeBuild
layout: schema
name: StartBuildBatchOutput
properties_list:
- description: ''
  name: buildBatch
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-start-build-batch-output-schema.json
slug: amazon-codebuild-start-build-batch-output
source_filename: amazon-codebuild-start-build-batch-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-start-build-batch-output-schema.json\",\n  \"title\": \"StartBuildBatchOutput\",\n  \"description\": \"StartBuildBatchOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"buildBatch\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildBatch\"\n        },\n        {\n          \"description\": \"A <code>BuildBatch</code> object that contains information about the batch build.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-start-build-batch-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: StartBuildBatchOutput
---
