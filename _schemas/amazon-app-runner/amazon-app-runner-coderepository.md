---
description: Describes a source code repository.
layout: schema
name: CodeRepository
properties_list:
- description: ''
  name: RepositoryUrl
  type: object
- description: ''
  name: SourceCodeVersion
  type: object
- description: ''
  name: CodeConfiguration
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-coderepository-schema.json
slug: amazon-app-runner-coderepository
source_filename: amazon-app-runner-coderepository-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CodeRepository\",\n  \"description\": \"Describes a source code repository.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RepositoryUrl\": {},\n    \"SourceCodeVersion\": {},\n    \"CodeConfiguration\": {}\n  },\n  \"required\": [\n    \"RepositoryUrl\",\n    \"SourceCodeVersion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-coderepository-schema.json
tags:
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: CodeRepository
---
