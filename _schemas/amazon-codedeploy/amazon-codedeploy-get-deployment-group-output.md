---
description: Represents the output of a <code>GetDeploymentGroup</code> operation.
layout: schema
name: GetDeploymentGroupOutput
properties_list:
- description: ''
  name: deploymentGroupInfo
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-get-deployment-group-output-schema.json
slug: amazon-codedeploy-get-deployment-group-output
source_filename: amazon-codedeploy-get-deployment-group-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-get-deployment-group-output-schema.json\",\n  \"title\": \"GetDeploymentGroupOutput\",\n  \"description\": \"Represents the output of a <code>GetDeploymentGroup</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentGroupInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentGroupInfo\"\n        },\n        {\n          \"description\": \"Information about the deployment group.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-get-deployment-group-output-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: GetDeploymentGroupOutput
---
