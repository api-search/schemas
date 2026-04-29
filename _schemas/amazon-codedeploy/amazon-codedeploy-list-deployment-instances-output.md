---
description: Represents the output of a <code>ListDeploymentInstances</code> operation.
layout: schema
name: ListDeploymentInstancesOutput
properties_list:
- description: ''
  name: instancesList
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-list-deployment-instances-output-schema.json
slug: amazon-codedeploy-list-deployment-instances-output
source_filename: amazon-codedeploy-list-deployment-instances-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-deployment-instances-output-schema.json\",\n  \"title\": \"ListDeploymentInstancesOutput\",\n  \"description\": \"Represents the output of a <code>ListDeploymentInstances</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instancesList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstancesList\"\n        },\n        {\n          \"description\": \"A list of instance IDs.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If a large amount of information is returned, an identifier is also returned. It can be used in a subsequent list deployment instances call to return the next set of\
  \ deployment instances in the list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-deployment-instances-output-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: ListDeploymentInstancesOutput
---
