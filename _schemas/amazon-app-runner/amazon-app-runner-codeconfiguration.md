---
description: Describes the configuration that App Runner uses to build and run an App Runner service from a source code repository.
layout: schema
name: CodeConfiguration
properties_list:
- description: ''
  name: ConfigurationSource
  type: object
- description: ''
  name: CodeConfigurationValues
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-codeconfiguration-schema.json
slug: amazon-app-runner-codeconfiguration
source_filename: amazon-app-runner-codeconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CodeConfiguration\",\n  \"description\": \"Describes the configuration that App Runner uses to build and run an App Runner service from a source code repository.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationSource\": {},\n    \"CodeConfigurationValues\": {}\n  },\n  \"required\": [\n    \"ConfigurationSource\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-codeconfiguration-schema.json
tags:
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: CodeConfiguration
---
