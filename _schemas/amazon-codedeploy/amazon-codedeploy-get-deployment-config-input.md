---
description: Represents the input of a <code>GetDeploymentConfig</code> operation.
layout: schema
name: GetDeploymentConfigInput
properties_list:
- description: ''
  name: deploymentConfigName
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-get-deployment-config-input-schema.json
slug: amazon-codedeploy-get-deployment-config-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-get-deployment-config-input-schema.json\",\n  \"title\": \"GetDeploymentConfigInput\",\n  \"description\": \"Represents the input of a <code>GetDeploymentConfig</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentConfigName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentConfigName\"\n        },\n        {\n          \"description\": \"The name of a deployment configuration associated with the IAM user or Amazon Web Services account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"deploymentConfigName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-get-deployment-config-input-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: GetDeploymentConfigInput
---
