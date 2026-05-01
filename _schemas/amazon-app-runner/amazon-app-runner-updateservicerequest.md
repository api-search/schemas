---
description: ''
layout: schema
name: UpdateServiceRequest
properties_list:
- description: ''
  name: ServiceArn
  type: object
- description: ''
  name: SourceConfiguration
  type: object
- description: ''
  name: InstanceConfiguration
  type: object
- description: ''
  name: AutoScalingConfigurationArn
  type: object
- description: ''
  name: HealthCheckConfiguration
  type: object
- description: ''
  name: NetworkConfiguration
  type: object
- description: ''
  name: ObservabilityConfiguration
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-updateservicerequest-schema.json
slug: amazon-app-runner-updateservicerequest
source_filename: amazon-app-runner-updateservicerequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"UpdateServiceRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServiceArn\": {},\n    \"SourceConfiguration\": {},\n    \"InstanceConfiguration\": {},\n    \"AutoScalingConfigurationArn\": {},\n    \"HealthCheckConfiguration\": {},\n    \"NetworkConfiguration\": {},\n    \"ObservabilityConfiguration\": {}\n  },\n  \"required\": [\n    \"ServiceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-updateservicerequest-schema.json
tags:
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: UpdateServiceRequest
---
