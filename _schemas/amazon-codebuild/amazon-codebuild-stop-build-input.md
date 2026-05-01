---
description: StopBuildInput schema from Amazon CodeBuild
layout: schema
name: StopBuildInput
properties_list:
- description: ''
  name: id
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-stop-build-input-schema.json
slug: amazon-codebuild-stop-build-input
source_filename: amazon-codebuild-stop-build-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-stop-build-input-schema.json\",\n  \"title\": \"StopBuildInput\",\n  \"description\": \"StopBuildInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The ID of the build.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-stop-build-input-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: StopBuildInput
---
