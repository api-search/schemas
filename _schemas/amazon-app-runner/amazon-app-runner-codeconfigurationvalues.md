---
description: Describes the basic configuration needed for building and running an App Runner service. This type doesn't support the full set of possible configuration options. Fur full configuration capabilities, use a <code>apprunner.yaml</code> file in the source code repository.
layout: schema
name: CodeConfigurationValues
properties_list:
- description: ''
  name: Runtime
  type: object
- description: ''
  name: BuildCommand
  type: object
- description: ''
  name: StartCommand
  type: object
- description: ''
  name: Port
  type: object
- description: ''
  name: RuntimeEnvironmentVariables
  type: object
- description: ''
  name: RuntimeEnvironmentSecrets
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-codeconfigurationvalues-schema.json
slug: amazon-app-runner-codeconfigurationvalues
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CodeConfigurationValues\",\n  \"description\": \"Describes the basic configuration needed for building and running an App Runner service. This type doesn't support the full set of possible configuration options. Fur full configuration capabilities, use a <code>apprunner.yaml</code> file in the source code repository.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Runtime\": {},\n    \"BuildCommand\": {},\n    \"StartCommand\": {},\n    \"Port\": {},\n    \"RuntimeEnvironmentVariables\": {},\n    \"RuntimeEnvironmentSecrets\": {}\n  },\n  \"required\": [\n    \"Runtime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-codeconfigurationvalues-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: CodeConfigurationValues
---
