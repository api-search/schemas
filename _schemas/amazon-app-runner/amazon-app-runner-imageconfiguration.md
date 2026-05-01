---
description: Describes the configuration that App Runner uses to run an App Runner service using an image pulled from a source image repository.
layout: schema
name: ImageConfiguration
properties_list:
- description: ''
  name: RuntimeEnvironmentVariables
  type: object
- description: ''
  name: StartCommand
  type: object
- description: ''
  name: Port
  type: object
- description: ''
  name: RuntimeEnvironmentSecrets
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-imageconfiguration-schema.json
slug: amazon-app-runner-imageconfiguration
source_filename: amazon-app-runner-imageconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ImageConfiguration\",\n  \"description\": \"Describes the configuration that App Runner uses to run an App Runner service using an image pulled from a source image repository.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RuntimeEnvironmentVariables\": {},\n    \"StartCommand\": {},\n    \"Port\": {},\n    \"RuntimeEnvironmentSecrets\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-imageconfiguration-schema.json
tags:
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: ImageConfiguration
---
