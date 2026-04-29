---
description: BatchDeleteBuildsInput schema from Amazon CodeBuild
layout: schema
name: BatchDeleteBuildsInput
properties_list:
- description: ''
  name: ids
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-batch-delete-builds-input-schema.json
slug: amazon-codebuild-batch-delete-builds-input
source_filename: amazon-codebuild-batch-delete-builds-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-delete-builds-input-schema.json\",\n  \"title\": \"BatchDeleteBuildsInput\",\n  \"description\": \"BatchDeleteBuildsInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ids\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildIds\"\n        },\n        {\n          \"description\": \"The IDs of the builds to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ids\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-delete-builds-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: BatchDeleteBuildsInput
---
