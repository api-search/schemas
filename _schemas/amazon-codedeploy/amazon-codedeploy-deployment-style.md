---
description: Information about the type of deployment, either in-place or blue/green, you want to run and whether to route deployment traffic behind a load balancer.
layout: schema
name: DeploymentStyle
properties_list:
- description: ''
  name: deploymentType
  type: object
- description: ''
  name: deploymentOption
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-deployment-style-schema.json
slug: amazon-codedeploy-deployment-style
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-deployment-style-schema.json\",\n  \"title\": \"DeploymentStyle\",\n  \"description\": \"Information about the type of deployment, either in-place or blue/green, you want to run and whether to route deployment traffic behind a load balancer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentType\"\n        },\n        {\n          \"description\": \"Indicates whether to run an in-place deployment or a blue/green deployment.\"\n        }\n      ]\n    },\n    \"deploymentOption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentOption\"\n        },\n        {\n          \"description\": \"Indicates whether to route deployment traffic behind\
  \ a load balancer.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-deployment-style-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: DeploymentStyle
---
