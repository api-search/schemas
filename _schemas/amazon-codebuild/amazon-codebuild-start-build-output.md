---
description: StartBuildOutput schema from Amazon CodeBuild
layout: schema
name: StartBuildOutput
properties_list:
- description: ''
  name: build
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-start-build-output-schema.json
slug: amazon-codebuild-start-build-output
source_filename: amazon-codebuild-start-build-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-start-build-output-schema.json\",\n  \"title\": \"StartBuildOutput\",\n  \"description\": \"StartBuildOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"build\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Build\"\n        },\n        {\n          \"description\": \"Information about the build to be run.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-start-build-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: StartBuildOutput
---
