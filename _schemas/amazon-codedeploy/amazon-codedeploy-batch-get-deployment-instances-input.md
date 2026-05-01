---
description: Represents the input of a <code>BatchGetDeploymentInstances</code> operation.
layout: schema
name: BatchGetDeploymentInstancesInput
properties_list:
- description: ''
  name: deploymentId
  type: object
- description: ''
  name: instanceIds
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-batch-get-deployment-instances-input-schema.json
slug: amazon-codedeploy-batch-get-deployment-instances-input
source_filename: amazon-codedeploy-batch-get-deployment-instances-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-deployment-instances-input-schema.json\",\n  \"title\": \"BatchGetDeploymentInstancesInput\",\n  \"description\": \" Represents the input of a <code>BatchGetDeploymentInstances</code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentId\"\n        },\n        {\n          \"description\": \" The unique ID of a deployment. \"\n        }\n      ]\n    },\n    \"instanceIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstancesList\"\n        },\n        {\n          \"description\": \"The unique IDs of instances used in the deployment. The maximum number of instance IDs you can specify is 25.\"\n        }\n      ]\n    }\n\
  \  },\n  \"required\": [\n    \"deploymentId\",\n    \"instanceIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-deployment-instances-input-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: BatchGetDeploymentInstancesInput
---
