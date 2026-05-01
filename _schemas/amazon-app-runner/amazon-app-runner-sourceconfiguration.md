---
description: Describes the source deployed to an App Runner service. It can be a code or an image repository.
layout: schema
name: SourceConfiguration
properties_list:
- description: ''
  name: CodeRepository
  type: object
- description: ''
  name: ImageRepository
  type: object
- description: ''
  name: AutoDeploymentsEnabled
  type: object
- description: ''
  name: AuthenticationConfiguration
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-sourceconfiguration-schema.json
slug: amazon-app-runner-sourceconfiguration
source_filename: amazon-app-runner-sourceconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"SourceConfiguration\",\n  \"description\": \"Describes the source deployed to an App Runner service. It can be a code or an image repository.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CodeRepository\": {},\n    \"ImageRepository\": {},\n    \"AutoDeploymentsEnabled\": {},\n    \"AuthenticationConfiguration\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-sourceconfiguration-schema.json
tags:
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: SourceConfiguration
---
