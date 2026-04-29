---
description: Represents the input of a <code>GetDeploymentInstance</code> operation.
layout: schema
name: GetDeploymentInstanceInput
properties_list:
- description: ''
  name: deploymentId
  type: object
- description: ''
  name: instanceId
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-get-deployment-instance-input-schema.json
slug: amazon-codedeploy-get-deployment-instance-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-get-deployment-instance-input-schema.json\",\n  \"title\": \"GetDeploymentInstanceInput\",\n  \"description\": \" Represents the input of a <code>GetDeploymentInstance</code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentId\"\n        },\n        {\n          \"description\": \" The unique ID of a deployment. \"\n        }\n      ]\n    },\n    \"instanceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceId\"\n        },\n        {\n          \"description\": \" The unique ID of an instance in the deployment group. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"deploymentId\",\n    \"instanceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-get-deployment-instance-input-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: GetDeploymentInstanceInput
---
