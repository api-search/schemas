---
description: Information about a deployment configuration.
layout: schema
name: DeploymentConfig
properties_list:
- description: ''
  name: concurrentDeploymentPercentage
  type: object
- description: ''
  name: failureThresholdPercentage
  type: object
- description: ''
  name: robotDeploymentTimeoutInSeconds
  type: object
- description: ''
  name: downloadConditionFile
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-deployment-config-schema.json
slug: amazon-robomaker-openapi-deployment-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-deployment-config-schema.json\",\n  \"title\": \"DeploymentConfig\",\n  \"description\": \"Information about a deployment configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"concurrentDeploymentPercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Percentage\"\n        },\n        {\n          \"description\": \"The percentage of robots receiving the deployment at the same time.\"\n        }\n      ]\n    },\n    \"failureThresholdPercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Percentage\"\n        },\n        {\n          \"description\": \"The percentage of deployments that need to fail before stopping deployment.\"\n        }\n      ]\n    },\n    \"robotDeploymentTimeoutInSeconds\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentTimeout\"\n        },\n        {\n          \"description\": \"The amount of time, in seconds, to wait for deployment to a single robot to complete. Choose a time between 1 minute and 7 days. The default is 5 hours.\"\n        }\n      ]\n    },\n    \"downloadConditionFile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Object\"\n        },\n        {\n          \"description\": \"The download condition file.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-deployment-config-schema.json
tags:
- AWS
- Robotics
- Simulation
title: DeploymentConfig
---
