---
description: Describes a source image repository.
layout: schema
name: ImageRepository
properties_list:
- description: ''
  name: ImageIdentifier
  type: object
- description: ''
  name: ImageConfiguration
  type: object
- description: ''
  name: ImageRepositoryType
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-imagerepository-schema.json
slug: amazon-app-runner-imagerepository
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ImageRepository\",\n  \"description\": \"Describes a source image repository.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ImageIdentifier\": {},\n    \"ImageConfiguration\": {},\n    \"ImageRepositoryType\": {}\n  },\n  \"required\": [\n    \"ImageIdentifier\",\n    \"ImageRepositoryType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-imagerepository-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: ImageRepository
---
