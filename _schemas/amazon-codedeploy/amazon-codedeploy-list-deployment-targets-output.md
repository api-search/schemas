---
description: ListDeploymentTargetsOutput schema from Amazon CodeDeploy
layout: schema
name: ListDeploymentTargetsOutput
properties_list:
- description: ''
  name: targetIds
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-list-deployment-targets-output-schema.json
slug: amazon-codedeploy-list-deployment-targets-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-deployment-targets-output-schema.json\",\n  \"title\": \"ListDeploymentTargetsOutput\",\n  \"description\": \"ListDeploymentTargetsOutput schema from Amazon CodeDeploy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"targetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetIdList\"\n        },\n        {\n          \"description\": \" The unique IDs of deployment targets. \"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \" If a large amount of information is returned, a token identifier is also returned. It can be used in a subsequent <code>ListDeploymentTargets</code> call to return the next\
  \ set of deployment targets in the list. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-deployment-targets-output-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: ListDeploymentTargetsOutput
---
