---
description: Represents the input of a <code>BatchGetDeploymentGroups</code> operation.
layout: schema
name: BatchGetDeploymentGroupsInput
properties_list:
- description: ''
  name: applicationName
  type: object
- description: ''
  name: deploymentGroupNames
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-batch-get-deployment-groups-input-schema.json
slug: amazon-codedeploy-batch-get-deployment-groups-input
source_filename: amazon-codedeploy-batch-get-deployment-groups-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-deployment-groups-input-schema.json\",\n  \"title\": \"BatchGetDeploymentGroupsInput\",\n  \"description\": \"Represents the input of a <code>BatchGetDeploymentGroups</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of an CodeDeploy application associated with the applicable IAM or Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"deploymentGroupNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentGroupsList\"\n        },\n        {\n          \"description\": \"The names of the deployment groups.\"\n        }\n     \
  \ ]\n    }\n  },\n  \"required\": [\n    \"applicationName\",\n    \"deploymentGroupNames\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-deployment-groups-input-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: BatchGetDeploymentGroupsInput
---
