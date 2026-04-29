---
description: Represents the output of a <code>GetDeploymentConfig</code> operation.
layout: schema
name: GetDeploymentConfigOutput
properties_list:
- description: ''
  name: deploymentConfigInfo
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-get-deployment-config-output-schema.json
slug: amazon-codedeploy-get-deployment-config-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-get-deployment-config-output-schema.json\",\n  \"title\": \"GetDeploymentConfigOutput\",\n  \"description\": \"Represents the output of a <code>GetDeploymentConfig</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentConfigInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentConfigInfo\"\n        },\n        {\n          \"description\": \"Information about the deployment configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-get-deployment-config-output-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: GetDeploymentConfigOutput
---
