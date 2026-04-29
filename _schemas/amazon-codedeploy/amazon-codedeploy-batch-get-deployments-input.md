---
description: Represents the input of a <code>BatchGetDeployments</code> operation.
layout: schema
name: BatchGetDeploymentsInput
properties_list:
- description: ''
  name: deploymentIds
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-batch-get-deployments-input-schema.json
slug: amazon-codedeploy-batch-get-deployments-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-deployments-input-schema.json\",\n  \"title\": \"BatchGetDeploymentsInput\",\n  \"description\": \" Represents the input of a <code>BatchGetDeployments</code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentsList\"\n        },\n        {\n          \"description\": \" A list of deployment IDs, separated by spaces. The maximum number of deployment IDs you can specify is 25.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"deploymentIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-deployments-input-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: BatchGetDeploymentsInput
---
