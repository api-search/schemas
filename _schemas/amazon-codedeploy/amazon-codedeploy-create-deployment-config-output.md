---
description: Represents the output of a <code>CreateDeploymentConfig</code> operation.
layout: schema
name: CreateDeploymentConfigOutput
properties_list:
- description: ''
  name: deploymentConfigId
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-create-deployment-config-output-schema.json
slug: amazon-codedeploy-create-deployment-config-output
source_filename: amazon-codedeploy-create-deployment-config-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-create-deployment-config-output-schema.json\",\n  \"title\": \"CreateDeploymentConfigOutput\",\n  \"description\": \"Represents the output of a <code>CreateDeploymentConfig</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentConfigId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentConfigId\"\n        },\n        {\n          \"description\": \"A unique deployment configuration ID.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-create-deployment-config-output-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: CreateDeploymentConfigOutput
---
