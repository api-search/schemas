---
description: Represents the input of a <code>CreateDeploymentConfig</code> operation.
layout: schema
name: CreateDeploymentConfigInput
properties_list:
- description: ''
  name: deploymentConfigName
  type: object
- description: ''
  name: minimumHealthyHosts
  type: object
- description: ''
  name: trafficRoutingConfig
  type: object
- description: ''
  name: computePlatform
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-create-deployment-config-input-schema.json
slug: amazon-codedeploy-create-deployment-config-input
source_filename: amazon-codedeploy-create-deployment-config-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-create-deployment-config-input-schema.json\",\n  \"title\": \"CreateDeploymentConfigInput\",\n  \"description\": \"Represents the input of a <code>CreateDeploymentConfig</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentConfigName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentConfigName\"\n        },\n        {\n          \"description\": \"The name of the deployment configuration to create.\"\n        }\n      ]\n    },\n    \"minimumHealthyHosts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MinimumHealthyHosts\"\n        },\n        {\n          \"description\": \"<p>The minimum number of healthy instances that should be available at any time during the deployment. There\
  \ are two parameters expected in the input: type and value.</p> <p>The type parameter takes either of the following values:</p> <ul> <li> <p>HOST_COUNT: The value parameter represents the minimum number of healthy instances as an absolute value.</p> </li> <li> <p>FLEET_PERCENT: The value parameter represents the minimum number of healthy instances as a percentage of the total number of instances in the deployment. If you specify FLEET_PERCENT, at the start of the deployment, CodeDeploy converts the percentage to the equivalent number of instances and rounds up fractional instances.</p> </li> </ul> <p>The value parameter takes an integer.</p> <p>For example, to set a minimum of 95% healthy instance, specify a type of FLEET_PERCENT and a value of 95.</p>\"\n        }\n      ]\n    },\n    \"trafficRoutingConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TrafficRoutingConfig\"\n        },\n        {\n          \"description\": \"The configuration that\
  \ specifies how the deployment traffic is routed.\"\n        }\n      ]\n    },\n    \"computePlatform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputePlatform\"\n        },\n        {\n          \"description\": \"The destination platform type for the deployment (<code>Lambda</code>, <code>Server</code>, or <code>ECS</code>).\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"deploymentConfigName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-create-deployment-config-input-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: CreateDeploymentConfigInput
---
