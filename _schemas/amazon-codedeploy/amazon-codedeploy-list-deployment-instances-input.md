---
description: Represents the input of a <code>ListDeploymentInstances</code> operation.
layout: schema
name: ListDeploymentInstancesInput
properties_list:
- description: ''
  name: deploymentId
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: instanceStatusFilter
  type: object
- description: ''
  name: instanceTypeFilter
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-list-deployment-instances-input-schema.json
slug: amazon-codedeploy-list-deployment-instances-input
source_filename: amazon-codedeploy-list-deployment-instances-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-deployment-instances-input-schema.json\",\n  \"title\": \"ListDeploymentInstancesInput\",\n  \"description\": \" Represents the input of a <code>ListDeploymentInstances</code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentId\"\n        },\n        {\n          \"description\": \" The unique ID of a deployment. \"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"An identifier returned from the previous list deployment instances call. It can be used to return the next set of deployment instances in the list.\"\n      \
  \  }\n      ]\n    },\n    \"instanceStatusFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceStatusList\"\n        },\n        {\n          \"description\": \"<p>A subset of instances to list by status:</p> <ul> <li> <p> <code>Pending</code>: Include those instances with pending deployments.</p> </li> <li> <p> <code>InProgress</code>: Include those instances where deployments are still in progress.</p> </li> <li> <p> <code>Succeeded</code>: Include those instances with successful deployments.</p> </li> <li> <p> <code>Failed</code>: Include those instances with failed deployments.</p> </li> <li> <p> <code>Skipped</code>: Include those instances with skipped deployments.</p> </li> <li> <p> <code>Unknown</code>: Include those instances with deployments in an unknown state.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"instanceTypeFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceTypeList\"\n \
  \       },\n        {\n          \"description\": \"The set of instances in a blue/green deployment, either those in the original environment (\\\"BLUE\\\") or those in the replacement environment (\\\"GREEN\\\"), for which you want to view instance information.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"deploymentId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-deployment-instances-input-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: ListDeploymentInstancesInput
---
