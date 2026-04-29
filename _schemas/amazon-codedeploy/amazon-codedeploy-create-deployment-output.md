---
description: Represents the output of a <code>CreateDeployment</code> operation.
layout: schema
name: CreateDeploymentOutput
properties_list:
- description: ''
  name: deploymentId
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-create-deployment-output-schema.json
slug: amazon-codedeploy-create-deployment-output
source_filename: amazon-codedeploy-create-deployment-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-create-deployment-output-schema.json\",\n  \"title\": \"CreateDeploymentOutput\",\n  \"description\": \" Represents the output of a <code>CreateDeployment</code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentId\"\n        },\n        {\n          \"description\": \" The unique ID of a deployment. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-create-deployment-output-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: CreateDeploymentOutput
---
