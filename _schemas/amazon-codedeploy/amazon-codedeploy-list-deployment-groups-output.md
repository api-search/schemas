---
description: Represents the output of a <code>ListDeploymentGroups</code> operation.
layout: schema
name: ListDeploymentGroupsOutput
properties_list:
- description: ''
  name: applicationName
  type: object
- description: ''
  name: deploymentGroups
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-list-deployment-groups-output-schema.json
slug: amazon-codedeploy-list-deployment-groups-output
source_filename: amazon-codedeploy-list-deployment-groups-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-deployment-groups-output-schema.json\",\n  \"title\": \"ListDeploymentGroupsOutput\",\n  \"description\": \"Represents the output of a <code>ListDeploymentGroups</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The application name.\"\n        }\n      ]\n    },\n    \"deploymentGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentGroupsList\"\n        },\n        {\n          \"description\": \"A list of deployment group names.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\
  \n        },\n        {\n          \"description\": \"If a large amount of information is returned, an identifier is also returned. It can be used in a subsequent list deployment groups call to return the next set of deployment groups in the list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-deployment-groups-output-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: ListDeploymentGroupsOutput
---
