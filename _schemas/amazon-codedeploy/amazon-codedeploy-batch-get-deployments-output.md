---
description: Represents the output of a <code>BatchGetDeployments</code> operation.
layout: schema
name: BatchGetDeploymentsOutput
properties_list:
- description: ''
  name: deploymentsInfo
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-batch-get-deployments-output-schema.json
slug: amazon-codedeploy-batch-get-deployments-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-deployments-output-schema.json\",\n  \"title\": \"BatchGetDeploymentsOutput\",\n  \"description\": \" Represents the output of a <code>BatchGetDeployments</code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentsInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentsInfoList\"\n        },\n        {\n          \"description\": \" Information about the deployments. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-deployments-output-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: BatchGetDeploymentsOutput
---
