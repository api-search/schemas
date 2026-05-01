---
description: BatchGetBuildsOutput schema from Amazon CodeBuild
layout: schema
name: BatchGetBuildsOutput
properties_list:
- description: ''
  name: builds
  type: object
- description: ''
  name: buildsNotFound
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-batch-get-builds-output-schema.json
slug: amazon-codebuild-batch-get-builds-output
source_filename: amazon-codebuild-batch-get-builds-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-get-builds-output-schema.json\",\n  \"title\": \"BatchGetBuildsOutput\",\n  \"description\": \"BatchGetBuildsOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"builds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Builds\"\n        },\n        {\n          \"description\": \"Information about the requested builds.\"\n        }\n      ]\n    },\n    \"buildsNotFound\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildIds\"\n        },\n        {\n          \"description\": \"The IDs of builds for which information could not be found.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-get-builds-output-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: BatchGetBuildsOutput
---
