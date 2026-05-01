---
description: Represents the input of a <code>DeleteDeploymentConfig</code> operation.
layout: schema
name: DeleteDeploymentConfigInput
properties_list:
- description: ''
  name: deploymentConfigName
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-delete-deployment-config-input-schema.json
slug: amazon-codedeploy-delete-deployment-config-input
source_filename: amazon-codedeploy-delete-deployment-config-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-delete-deployment-config-input-schema.json\",\n  \"title\": \"DeleteDeploymentConfigInput\",\n  \"description\": \"Represents the input of a <code>DeleteDeploymentConfig</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentConfigName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentConfigName\"\n        },\n        {\n          \"description\": \"The name of a deployment configuration associated with the IAM user or Amazon Web Services account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"deploymentConfigName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-delete-deployment-config-input-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: DeleteDeploymentConfigInput
---
