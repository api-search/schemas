---
description: BatchGetProjectsOutput schema from Amazon CodeBuild
layout: schema
name: BatchGetProjectsOutput
properties_list:
- description: ''
  name: projects
  type: object
- description: ''
  name: projectsNotFound
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-batch-get-projects-output-schema.json
slug: amazon-codebuild-batch-get-projects-output
source_filename: amazon-codebuild-batch-get-projects-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-get-projects-output-schema.json\",\n  \"title\": \"BatchGetProjectsOutput\",\n  \"description\": \"BatchGetProjectsOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"projects\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Projects\"\n        },\n        {\n          \"description\": \"Information about the requested build projects.\"\n        }\n      ]\n    },\n    \"projectsNotFound\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectNames\"\n        },\n        {\n          \"description\": \"The names of build projects for which information could not be found.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-get-projects-output-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: BatchGetProjectsOutput
---
