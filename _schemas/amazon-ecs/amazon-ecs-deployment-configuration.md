---
description: Deployment parameters that control how many tasks run during the deployment and the ordering of stopping and starting tasks.
layout: schema
name: DeploymentConfiguration
properties_list:
- description: ''
  name: deploymentCircuitBreaker
  type: object
- description: The upper limit (as a percentage of the service's desiredCount) of the number of running tasks that can be running during a deployment.
  name: maximumPercent
  type: integer
- description: The lower limit (as a percentage of the service's desiredCount) of the number of running tasks that must remain running during a deployment.
  name: minimumHealthyPercent
  type: integer
- description: ''
  name: alarms
  type: object
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-deployment-configuration-schema.json
slug: amazon-ecs-deployment-configuration
source_filename: amazon-ecs-deployment-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeploymentConfiguration\",\n  \"type\": \"object\",\n  \"description\": \"Deployment parameters that control how many tasks run during the deployment and the ordering of stopping and starting tasks.\",\n  \"properties\": {\n    \"deploymentCircuitBreaker\": {\n      \"type\": \"object\"\n    },\n    \"maximumPercent\": {\n      \"type\": \"integer\",\n      \"description\": \"The upper limit (as a percentage of the service's desiredCount) of the number of running tasks that can be running during a deployment.\"\n    },\n    \"minimumHealthyPercent\": {\n      \"type\": \"integer\",\n      \"description\": \"The lower limit (as a percentage of the service's desiredCount) of the number of running tasks that must remain running during a deployment.\"\n    },\n    \"alarms\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-deployment-configuration-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: DeploymentConfiguration
---
