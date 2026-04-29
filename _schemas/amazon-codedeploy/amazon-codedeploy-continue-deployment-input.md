---
description: ContinueDeploymentInput schema from Amazon CodeDeploy
layout: schema
name: ContinueDeploymentInput
properties_list:
- description: ''
  name: deploymentId
  type: object
- description: ''
  name: deploymentWaitType
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-continue-deployment-input-schema.json
slug: amazon-codedeploy-continue-deployment-input
source_filename: amazon-codedeploy-continue-deployment-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-continue-deployment-input-schema.json\",\n  \"title\": \"ContinueDeploymentInput\",\n  \"description\": \"ContinueDeploymentInput schema from Amazon CodeDeploy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentId\"\n        },\n        {\n          \"description\": \" The unique ID of a blue/green deployment for which you want to start rerouting traffic to the replacement environment. \"\n        }\n      ]\n    },\n    \"deploymentWaitType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentWaitType\"\n        },\n        {\n          \"description\": \" The status of the deployment's waiting period. <code>READY_WAIT</code> indicates that\
  \ the deployment is ready to start shifting traffic. <code>TERMINATION_WAIT</code> indicates that the traffic is shifted, but the original target is not terminated. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-continue-deployment-input-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: ContinueDeploymentInput
---
