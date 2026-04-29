---
description: GetDeploymentResponse schema from Amazon CodeDeploy
layout: schema
name: GetDeploymentResponse
properties_list:
- description: ''
  name: deploymentInfo
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-get-deployment-response-schema.json
slug: amazon-codedeploy-get-deployment-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-get-deployment-response-schema.json\",\n  \"title\": \"GetDeploymentResponse\",\n  \"description\": \"GetDeploymentResponse schema from Amazon CodeDeploy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentInfo\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"deploymentId\": {\n          \"type\": \"string\"\n        },\n        \"applicationName\": {\n          \"type\": \"string\"\n        },\n        \"deploymentGroupName\": {\n          \"type\": \"string\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Created\",\n            \"Queued\",\n            \"InProgress\",\n            \"Baking\",\n            \"Succeeded\",\n            \"Failed\",\n            \"Stopped\",\n            \"Ready\"\
  \n          ]\n        },\n        \"createTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"startTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"completeTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"description\": {\n          \"type\": \"string\"\n        },\n        \"creator\": {\n          \"type\": \"string\"\n        },\n        \"computePlatform\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-get-deployment-response-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: GetDeploymentResponse
---
