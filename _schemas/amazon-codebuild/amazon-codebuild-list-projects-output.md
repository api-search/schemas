---
description: ListProjectsOutput schema from Amazon CodeBuild
layout: schema
name: ListProjectsOutput
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: projects
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-list-projects-output-schema.json
slug: amazon-codebuild-list-projects-output
source_filename: amazon-codebuild-list-projects-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-list-projects-output-schema.json\",\n  \"title\": \"ListProjectsOutput\",\n  \"description\": \"ListProjectsOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"If there are more than 100 items in the list, only the first 100 items are returned, along with a unique string called a <i>nextToken</i>. To get the next batch of items in the list, call this operation again, adding the next token to the call.\"\n        }\n      ]\n    },\n    \"projects\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectNames\"\n        },\n        {\n          \"description\": \"The\
  \ list of build project names, with each build project name representing a single build project.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-list-projects-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ListProjectsOutput
---
