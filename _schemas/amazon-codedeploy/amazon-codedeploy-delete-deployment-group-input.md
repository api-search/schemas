---
description: Represents the input of a <code>DeleteDeploymentGroup</code> operation.
layout: schema
name: DeleteDeploymentGroupInput
properties_list:
- description: ''
  name: applicationName
  type: object
- description: ''
  name: deploymentGroupName
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-delete-deployment-group-input-schema.json
slug: amazon-codedeploy-delete-deployment-group-input
source_filename: amazon-codedeploy-delete-deployment-group-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-delete-deployment-group-input-schema.json\",\n  \"title\": \"DeleteDeploymentGroupInput\",\n  \"description\": \"Represents the input of a <code>DeleteDeploymentGroup</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of an CodeDeploy application associated with the IAM user or Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"deploymentGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentGroupName\"\n        },\n        {\n          \"description\": \"The name of a deployment group for the specified application.\"\n        }\n\
  \      ]\n    }\n  },\n  \"required\": [\n    \"applicationName\",\n    \"deploymentGroupName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-delete-deployment-group-input-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: DeleteDeploymentGroupInput
---
