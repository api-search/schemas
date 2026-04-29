---
description: Identifies a version of code that App Runner refers to within a source code repository.
layout: schema
name: SourceCodeVersion
properties_list:
- description: ''
  name: Type
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-sourcecodeversion-schema.json
slug: amazon-app-runner-sourcecodeversion
source_filename: amazon-app-runner-sourcecodeversion-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"SourceCodeVersion\",\n  \"description\": \"Identifies a version of code that App Runner refers to within a source code repository.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Type\": {},\n    \"Value\": {}\n  },\n  \"required\": [\n    \"Type\",\n    \"Value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-sourcecodeversion-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: SourceCodeVersion
---
