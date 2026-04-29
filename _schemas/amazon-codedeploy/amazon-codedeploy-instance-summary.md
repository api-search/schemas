---
description: Information about an instance in a deployment.InstanceSummary is deprecated, use DeploymentTarget instead.
layout: schema
name: InstanceSummary
properties_list:
- description: ''
  name: deploymentId
  type: object
- description: ''
  name: instanceId
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: lastUpdatedAt
  type: object
- description: ''
  name: lifecycleEvents
  type: object
- description: ''
  name: instanceType
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-instance-summary-schema.json
slug: amazon-codedeploy-instance-summary
source_filename: amazon-codedeploy-instance-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-instance-summary-schema.json\",\n  \"title\": \"InstanceSummary\",\n  \"description\": \"Information about an instance in a deployment.InstanceSummary is deprecated, use DeploymentTarget instead.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentId\"\n        },\n        {\n          \"description\": \" The unique ID of a deployment. \"\n        }\n      ]\n    },\n    \"instanceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceId\"\n        },\n        {\n          \"description\": \"The instance ID.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceStatus\"\
  \n        },\n        {\n          \"description\": \"<p>The deployment status for this instance:</p> <ul> <li> <p> <code>Pending</code>: The deployment is pending for this instance.</p> </li> <li> <p> <code>In Progress</code>: The deployment is in progress for this instance.</p> </li> <li> <p> <code>Succeeded</code>: The deployment has succeeded for this instance.</p> </li> <li> <p> <code>Failed</code>: The deployment has failed for this instance.</p> </li> <li> <p> <code>Skipped</code>: The deployment has been skipped for this instance.</p> </li> <li> <p> <code>Unknown</code>: The deployment status is unknown for this instance.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"lastUpdatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A timestamp that indicates when the instance information was last updated.\"\n        }\n      ]\n    },\n    \"lifecycleEvents\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/LifecycleEventList\"\n        },\n        {\n          \"description\": \"A list of lifecycle events for this instance.\"\n        }\n      ]\n    },\n    \"instanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceType\"\n        },\n        {\n          \"description\": \"<p>Information about which environment an instance belongs to in a blue/green deployment.</p> <ul> <li> <p>BLUE: The instance is part of the original environment.</p> </li> <li> <p>GREEN: The instance is part of the replacement environment.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"deprecated\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-instance-summary-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: InstanceSummary
---
