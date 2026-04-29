---
description: SkipWaitTimeForInstanceTerminationInput schema from Amazon CodeDeploy
layout: schema
name: SkipWaitTimeForInstanceTerminationInput
properties_list:
- description: ''
  name: deploymentId
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-skip-wait-time-for-instance-termination-input-schema.json
slug: amazon-codedeploy-skip-wait-time-for-instance-termination-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-skip-wait-time-for-instance-termination-input-schema.json\",\n  \"title\": \"SkipWaitTimeForInstanceTerminationInput\",\n  \"description\": \"SkipWaitTimeForInstanceTerminationInput schema from Amazon CodeDeploy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentId\"\n        },\n        {\n          \"description\": \" The unique ID of a blue/green deployment for which you want to skip the instance termination wait time. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-skip-wait-time-for-instance-termination-input-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: SkipWaitTimeForInstanceTerminationInput
---
