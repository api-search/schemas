---
description: Information about blue/green deployment options for a deployment group.
layout: schema
name: BlueGreenDeploymentConfiguration
properties_list:
- description: ''
  name: terminateBlueInstancesOnDeploymentSuccess
  type: object
- description: ''
  name: deploymentReadyOption
  type: object
- description: ''
  name: greenFleetProvisioningOption
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-blue-green-deployment-configuration-schema.json
slug: amazon-codedeploy-blue-green-deployment-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-blue-green-deployment-configuration-schema.json\",\n  \"title\": \"BlueGreenDeploymentConfiguration\",\n  \"description\": \"Information about blue/green deployment options for a deployment group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"terminateBlueInstancesOnDeploymentSuccess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlueInstanceTerminationOption\"\n        },\n        {\n          \"description\": \"Information about whether to terminate instances in the original fleet during a blue/green deployment.\"\n        }\n      ]\n    },\n    \"deploymentReadyOption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentReadyOption\"\n        },\n        {\n          \"description\": \"Information about\
  \ the action to take when newly provisioned instances are ready to receive traffic in a blue/green deployment.\"\n        }\n      ]\n    },\n    \"greenFleetProvisioningOption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GreenFleetProvisioningOption\"\n        },\n        {\n          \"description\": \"Information about how instances are provisioned for a replacement environment in a blue/green deployment.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-blue-green-deployment-configuration-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: BlueGreenDeploymentConfiguration
---
