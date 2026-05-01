---
description: Represents the output of a <code>GetDeploymentInstance</code> operation.
layout: schema
name: GetDeploymentInstanceOutput
properties_list:
- description: ''
  name: instanceSummary
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-get-deployment-instance-output-schema.json
slug: amazon-codedeploy-get-deployment-instance-output
source_filename: amazon-codedeploy-get-deployment-instance-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-get-deployment-instance-output-schema.json\",\n  \"title\": \"GetDeploymentInstanceOutput\",\n  \"description\": \" Represents the output of a <code>GetDeploymentInstance</code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instanceSummary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceSummary\"\n        },\n        {\n          \"description\": \" Information about the instance. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-get-deployment-instance-output-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: GetDeploymentInstanceOutput
---
