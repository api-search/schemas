---
description: Represents the input of a <code>ListDeploymentConfigs</code> operation.
layout: schema
name: ListDeploymentConfigsInput
properties_list:
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-list-deployment-configs-input-schema.json
slug: amazon-codedeploy-list-deployment-configs-input
source_filename: amazon-codedeploy-list-deployment-configs-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-deployment-configs-input-schema.json\",\n  \"title\": \"ListDeploymentConfigsInput\",\n  \"description\": \"Represents the input of a <code>ListDeploymentConfigs</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"An identifier returned from the previous <code>ListDeploymentConfigs</code> call. It can be used to return the next set of deployment configurations in the list. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-deployment-configs-input-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: ListDeploymentConfigsInput
---
