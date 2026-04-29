---
description: Information about a deployment configuration.
layout: schema
name: DeploymentConfigInfo
properties_list:
- description: ''
  name: deploymentConfigId
  type: object
- description: ''
  name: deploymentConfigName
  type: object
- description: ''
  name: minimumHealthyHosts
  type: object
- description: ''
  name: createTime
  type: object
- description: ''
  name: computePlatform
  type: object
- description: ''
  name: trafficRoutingConfig
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-deployment-config-info-schema.json
slug: amazon-codedeploy-deployment-config-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-deployment-config-info-schema.json\",\n  \"title\": \"DeploymentConfigInfo\",\n  \"description\": \"Information about a deployment configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentConfigId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentConfigId\"\n        },\n        {\n          \"description\": \"The deployment configuration ID.\"\n        }\n      ]\n    },\n    \"deploymentConfigName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentConfigName\"\n        },\n        {\n          \"description\": \"The deployment configuration name.\"\n        }\n      ]\n    },\n    \"minimumHealthyHosts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MinimumHealthyHosts\"\
  \n        },\n        {\n          \"description\": \"Information about the number or percentage of minimum healthy instance.\"\n        }\n      ]\n    },\n    \"createTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the deployment configuration was created.\"\n        }\n      ]\n    },\n    \"computePlatform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputePlatform\"\n        },\n        {\n          \"description\": \"The destination platform type for the deployment (<code>Lambda</code>, <code>Server</code>, or <code>ECS</code>).\"\n        }\n      ]\n    },\n    \"trafficRoutingConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TrafficRoutingConfig\"\n        },\n        {\n          \"description\": \"The configuration that specifies how the deployment traffic is routed. Used for deployments\
  \ with a Lambda or Amazon ECS compute platform only.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-deployment-config-info-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: DeploymentConfigInfo
---
