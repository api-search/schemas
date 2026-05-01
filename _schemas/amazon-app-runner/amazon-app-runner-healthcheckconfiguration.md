---
description: Describes the settings for the health check that App Runner performs to monitor the health of a service.
layout: schema
name: HealthCheckConfiguration
properties_list:
- description: ''
  name: Protocol
  type: object
- description: ''
  name: Path
  type: object
- description: ''
  name: Interval
  type: object
- description: ''
  name: Timeout
  type: object
- description: ''
  name: HealthyThreshold
  type: object
- description: ''
  name: UnhealthyThreshold
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-healthcheckconfiguration-schema.json
slug: amazon-app-runner-healthcheckconfiguration
source_filename: amazon-app-runner-healthcheckconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HealthCheckConfiguration\",\n  \"description\": \"Describes the settings for the health check that App Runner performs to monitor the health of a service.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Protocol\": {},\n    \"Path\": {},\n    \"Interval\": {},\n    \"Timeout\": {},\n    \"HealthyThreshold\": {},\n    \"UnhealthyThreshold\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-healthcheckconfiguration-schema.json
tags:
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: HealthCheckConfiguration
---
