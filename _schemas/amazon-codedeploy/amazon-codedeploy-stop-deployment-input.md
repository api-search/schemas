---
description: Represents the input of a <code>StopDeployment</code> operation.
layout: schema
name: StopDeploymentInput
properties_list:
- description: ''
  name: deploymentId
  type: object
- description: ''
  name: autoRollbackEnabled
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-stop-deployment-input-schema.json
slug: amazon-codedeploy-stop-deployment-input
source_filename: amazon-codedeploy-stop-deployment-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-stop-deployment-input-schema.json\",\n  \"title\": \"StopDeploymentInput\",\n  \"description\": \" Represents the input of a <code>StopDeployment</code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentId\"\n        },\n        {\n          \"description\": \" The unique ID of a deployment. \"\n        }\n      ]\n    },\n    \"autoRollbackEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \" Indicates, when a deployment is stopped, whether instances that have been updated should be rolled back to the previous version of the application revision. \"\n       \
  \ }\n      ]\n    }\n  },\n  \"required\": [\n    \"deploymentId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-stop-deployment-input-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: StopDeploymentInput
---
