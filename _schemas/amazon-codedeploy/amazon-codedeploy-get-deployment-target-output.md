---
description: GetDeploymentTargetOutput schema from Amazon CodeDeploy
layout: schema
name: GetDeploymentTargetOutput
properties_list:
- description: ''
  name: deploymentTarget
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-get-deployment-target-output-schema.json
slug: amazon-codedeploy-get-deployment-target-output
source_filename: amazon-codedeploy-get-deployment-target-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-get-deployment-target-output-schema.json\",\n  \"title\": \"GetDeploymentTargetOutput\",\n  \"description\": \"GetDeploymentTargetOutput schema from Amazon CodeDeploy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentTarget\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentTarget\"\n        },\n        {\n          \"description\": \" A deployment target that contains information about a deployment such as its status, lifecycle events, and when it was last updated. It also contains metadata about the deployment target. The deployment target metadata depends on the deployment target's type (<code>instanceTarget</code>, <code>lambdaTarget</code>, or <code>ecsTarget</code>). \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-get-deployment-target-output-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: GetDeploymentTargetOutput
---
