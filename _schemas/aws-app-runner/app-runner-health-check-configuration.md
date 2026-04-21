---
description: HealthCheckConfiguration schema from AWS App Runner
layout: schema
name: HealthCheckConfiguration
properties_list:
- description: ''
  name: Protocol
  type: string
- description: ''
  name: Path
  type: string
- description: Interval in seconds between health checks.
  name: Interval
  type: integer
- description: Timeout in seconds for each health check.
  name: Timeout
  type: integer
- description: ''
  name: HealthyThreshold
  type: integer
- description: ''
  name: UnhealthyThreshold
  type: integer
provider_name: AWS App Runner
provider_slug: aws-app-runner
schema_file: json-schema/app-runner-health-check-configuration-schema.json
slug: app-runner-health-check-configuration
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Microservices
- Serverless
title: HealthCheckConfiguration
---
