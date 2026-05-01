---
description: Describes the runtime configuration of an App Runner service instance (scaling unit).
layout: schema
name: InstanceConfiguration
properties_list:
- description: ''
  name: Cpu
  type: object
- description: ''
  name: Memory
  type: object
- description: ''
  name: InstanceRoleArn
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-instanceconfiguration-schema.json
slug: amazon-app-runner-instanceconfiguration
source_filename: amazon-app-runner-instanceconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"InstanceConfiguration\",\n  \"description\": \"Describes the runtime configuration of an App Runner service instance (scaling unit).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Cpu\": {},\n    \"Memory\": {},\n    \"InstanceRoleArn\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-instanceconfiguration-schema.json
tags:
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: InstanceConfiguration
---
