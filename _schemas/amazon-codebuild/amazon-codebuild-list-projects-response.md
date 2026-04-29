---
description: ListProjectsResponse schema from Amazon CodeBuild
layout: schema
name: ListProjectsResponse
properties_list:
- description: ''
  name: projects
  type: array
- description: ''
  name: nextToken
  type: string
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-list-projects-response-schema.json
slug: amazon-codebuild-list-projects-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-list-projects-response-schema.json\",\n  \"title\": \"ListProjectsResponse\",\n  \"description\": \"ListProjectsResponse schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"projects\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-list-projects-response-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ListProjectsResponse
---
