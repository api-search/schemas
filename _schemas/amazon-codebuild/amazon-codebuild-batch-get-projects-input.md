---
description: BatchGetProjectsInput schema from Amazon CodeBuild
layout: schema
name: BatchGetProjectsInput
properties_list:
- description: ''
  name: names
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-batch-get-projects-input-schema.json
slug: amazon-codebuild-batch-get-projects-input
source_filename: amazon-codebuild-batch-get-projects-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-get-projects-input-schema.json\",\n  \"title\": \"BatchGetProjectsInput\",\n  \"description\": \"BatchGetProjectsInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"names\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectNames\"\n        },\n        {\n          \"description\": \"The names or ARNs of the build projects. To get information about a project shared with your Amazon Web Services account, its ARN must be specified. You cannot specify a shared project using its name.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"names\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-get-projects-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: BatchGetProjectsInput
---
