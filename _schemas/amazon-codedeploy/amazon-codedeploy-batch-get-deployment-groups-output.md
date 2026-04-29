---
description: Represents the output of a <code>BatchGetDeploymentGroups</code> operation.
layout: schema
name: BatchGetDeploymentGroupsOutput
properties_list:
- description: ''
  name: deploymentGroupsInfo
  type: object
- description: ''
  name: errorMessage
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-batch-get-deployment-groups-output-schema.json
slug: amazon-codedeploy-batch-get-deployment-groups-output
source_filename: amazon-codedeploy-batch-get-deployment-groups-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-deployment-groups-output-schema.json\",\n  \"title\": \"BatchGetDeploymentGroupsOutput\",\n  \"description\": \"Represents the output of a <code>BatchGetDeploymentGroups</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentGroupsInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentGroupInfoList\"\n        },\n        {\n          \"description\": \"Information about the deployment groups.\"\n        }\n      ]\n    },\n    \"errorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorMessage\"\n        },\n        {\n          \"description\": \"Information about errors that might have occurred during the API call.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-deployment-groups-output-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: BatchGetDeploymentGroupsOutput
---
