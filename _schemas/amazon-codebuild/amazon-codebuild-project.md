---
description: Project schema from Amazon CodeBuild
layout: schema
name: Project
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: arn
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: created
  type: string
- description: ''
  name: lastModified
  type: string
- description: ''
  name: serviceRole
  type: string
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-project-schema.json
slug: amazon-codebuild-project
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-project-schema.json\",\n  \"title\": \"Project\",\n  \"description\": \"Project schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"arn\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"serviceRole\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-project-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: Project
---
