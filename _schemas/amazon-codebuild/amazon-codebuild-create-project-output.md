---
description: CreateProjectOutput schema from Amazon CodeBuild
layout: schema
name: CreateProjectOutput
properties_list:
- description: ''
  name: project
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-create-project-output-schema.json
slug: amazon-codebuild-create-project-output
source_filename: amazon-codebuild-create-project-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-create-project-output-schema.json\",\n  \"title\": \"CreateProjectOutput\",\n  \"description\": \"CreateProjectOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"project\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Project\"\n        },\n        {\n          \"description\": \"Information about the build project that was created.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-create-project-output-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: CreateProjectOutput
---
