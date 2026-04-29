---
description: Represents the input of a <code>ListDeployments</code> operation.
layout: schema
name: ListDeploymentsInput
properties_list:
- description: ''
  name: applicationName
  type: object
- description: ''
  name: deploymentGroupName
  type: object
- description: ''
  name: externalId
  type: object
- description: ''
  name: includeOnlyStatuses
  type: object
- description: ''
  name: createTimeRange
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-list-deployments-input-schema.json
slug: amazon-codedeploy-list-deployments-input
source_filename: amazon-codedeploy-list-deployments-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-deployments-input-schema.json\",\n  \"title\": \"ListDeploymentsInput\",\n  \"description\": \"Represents the input of a <code>ListDeployments</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"<p>The name of an CodeDeploy application associated with the IAM user or Amazon Web Services account.</p> <note> <p>If <code>applicationName</code> is specified, then <code>deploymentGroupName</code> must be specified. If it is not specified, then <code>deploymentGroupName</code> must not be specified. </p> </note>\"\n        }\n      ]\n    },\n    \"deploymentGroupName\": {\n      \"allOf\": [\n   \
  \     {\n          \"$ref\": \"#/components/schemas/DeploymentGroupName\"\n        },\n        {\n          \"description\": \"<p>The name of a deployment group for the specified application.</p> <note> <p>If <code>deploymentGroupName</code> is specified, then <code>applicationName</code> must be specified. If it is not specified, then <code>applicationName</code> must not be specified. </p> </note>\"\n        }\n      ]\n    },\n    \"externalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalId\"\n        },\n        {\n          \"description\": \"The unique ID of an external resource for returning deployments linked to the external resource.\"\n        }\n      ]\n    },\n    \"includeOnlyStatuses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentStatusList\"\n        },\n        {\n          \"description\": \"<p>A subset of deployments to list by status:</p> <ul> <li> <p> <code>Created</code>: Include\
  \ created deployments in the resulting list.</p> </li> <li> <p> <code>Queued</code>: Include queued deployments in the resulting list.</p> </li> <li> <p> <code>In Progress</code>: Include in-progress deployments in the resulting list.</p> </li> <li> <p> <code>Succeeded</code>: Include successful deployments in the resulting list.</p> </li> <li> <p> <code>Failed</code>: Include failed deployments in the resulting list.</p> </li> <li> <p> <code>Stopped</code>: Include stopped deployments in the resulting list.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"createTimeRange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeRange\"\n        },\n        {\n          \"description\": \"A time range (start and end) for returning a subset of the list of deployments.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"\
  An identifier returned from the previous list deployments call. It can be used to return the next set of deployments in the list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-deployments-input-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: ListDeploymentsInput
---
