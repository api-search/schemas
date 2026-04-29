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
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Protocol\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"TCP\",\n        \"HTTP\"\n      ]\n    },\n    \"Path\": {\n      \"type\": \"string\"\n    },\n    \"Interval\": {\n      \"type\": \"integer\",\n      \"description\": \"Interval in seconds between health checks.\"\n    },\n    \"Timeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Timeout in seconds for each health check.\"\n    },\n    \"HealthyThreshold\": {\n      \"type\": \"integer\"\n    },\n    \"UnhealthyThreshold\": {\n      \"type\": \"integer\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-health-check-configuration-schema.json\",\n  \"title\": \"HealthCheckConfiguration\",\n  \"description\": \"HealthCheckConfiguration schema from AWS App Runner\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-health-check-configuration-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Microservices
- Serverless
title: HealthCheckConfiguration
---
