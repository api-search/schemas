---
description: ''
layout: schema
name: CreateAutoScalingConfigurationRequest
properties_list:
- description: ''
  name: AutoScalingConfigurationName
  type: object
- description: ''
  name: MaxConcurrency
  type: object
- description: ''
  name: MinSize
  type: object
- description: ''
  name: MaxSize
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-createautoscalingconfigurationrequest-schema.json
slug: amazon-app-runner-createautoscalingconfigurationrequest
source_filename: amazon-app-runner-createautoscalingconfigurationrequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreateAutoScalingConfigurationRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingConfigurationName\": {},\n    \"MaxConcurrency\": {},\n    \"MinSize\": {},\n    \"MaxSize\": {},\n    \"Tags\": {}\n  },\n  \"required\": [\n    \"AutoScalingConfigurationName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-createautoscalingconfigurationrequest-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: CreateAutoScalingConfigurationRequest
---
