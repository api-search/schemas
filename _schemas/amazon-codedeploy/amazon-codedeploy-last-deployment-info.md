---
description: Information about the most recent attempted or successful deployment to a deployment group.
layout: schema
name: LastDeploymentInfo
properties_list:
- description: ''
  name: deploymentId
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: endTime
  type: object
- description: ''
  name: createTime
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-last-deployment-info-schema.json
slug: amazon-codedeploy-last-deployment-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-last-deployment-info-schema.json\",\n  \"title\": \"LastDeploymentInfo\",\n  \"description\": \"Information about the most recent attempted or successful deployment to a deployment group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentId\"\n        },\n        {\n          \"description\": \" The unique ID of a deployment. \"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentStatus\"\n        },\n        {\n          \"description\": \"The status of the most recent deployment.\"\n        }\n      ]\n    },\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\
  \n        },\n        {\n          \"description\": \"A timestamp that indicates when the most recent deployment to the deployment group was complete.\"\n        }\n      ]\n    },\n    \"createTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A timestamp that indicates when the most recent deployment to the deployment group started.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-last-deployment-info-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: LastDeploymentInfo
---
