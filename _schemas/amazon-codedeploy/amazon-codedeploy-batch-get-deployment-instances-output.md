---
description: Represents the output of a <code>BatchGetDeploymentInstances</code> operation.
layout: schema
name: BatchGetDeploymentInstancesOutput
properties_list:
- description: ''
  name: instancesSummary
  type: object
- description: ''
  name: errorMessage
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-batch-get-deployment-instances-output-schema.json
slug: amazon-codedeploy-batch-get-deployment-instances-output
source_filename: amazon-codedeploy-batch-get-deployment-instances-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-deployment-instances-output-schema.json\",\n  \"title\": \"BatchGetDeploymentInstancesOutput\",\n  \"description\": \"Represents the output of a <code>BatchGetDeploymentInstances</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instancesSummary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceSummaryList\"\n        },\n        {\n          \"description\": \"Information about the instance.\"\n        }\n      ]\n    },\n    \"errorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorMessage\"\n        },\n        {\n          \"description\": \"Information about errors that might have occurred during the API call.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-deployment-instances-output-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: BatchGetDeploymentInstancesOutput
---
