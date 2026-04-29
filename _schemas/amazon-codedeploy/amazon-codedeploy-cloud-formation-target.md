---
description: Information about the target to be updated by an CloudFormation blue/green deployment. This target type is used for all deployments initiated by a CloudFormation stack update.
layout: schema
name: CloudFormationTarget
properties_list:
- description: ''
  name: deploymentId
  type: object
- description: ''
  name: targetId
  type: object
- description: ''
  name: lastUpdatedAt
  type: object
- description: ''
  name: lifecycleEvents
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: resourceType
  type: object
- description: ''
  name: targetVersionWeight
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-cloud-formation-target-schema.json
slug: amazon-codedeploy-cloud-formation-target
source_filename: amazon-codedeploy-cloud-formation-target-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-cloud-formation-target-schema.json\",\n  \"title\": \"CloudFormationTarget\",\n  \"description\": \" Information about the target to be updated by an CloudFormation blue/green deployment. This target type is used for all deployments initiated by a CloudFormation stack update.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentId\"\n        },\n        {\n          \"description\": \"The unique ID of an CloudFormation blue/green deployment.\"\n        }\n      ]\n    },\n    \"targetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetId\"\n        },\n        {\n          \"description\": \" The unique ID of a deployment target that has a type\
  \ of\\u00a0<code>CloudFormationTarget</code>. \"\n        }\n      ]\n    },\n    \"lastUpdatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Time\"\n        },\n        {\n          \"description\": \" The date and time when the target application was updated by an CloudFormation blue/green deployment. \"\n        }\n      ]\n    },\n    \"lifecycleEvents\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LifecycleEventList\"\n        },\n        {\n          \"description\": \" The lifecycle events of the CloudFormation blue/green deployment to this target application. \"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetStatus\"\n        },\n        {\n          \"description\": \" The status of an CloudFormation blue/green deployment's target application. \"\n        }\n      ]\n    },\n    \"resourceType\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/CloudFormationResourceType\"\n        },\n        {\n          \"description\": \"The resource type for the CloudFormation blue/green deployment.\"\n        }\n      ]\n    },\n    \"targetVersionWeight\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TrafficWeight\"\n        },\n        {\n          \"description\": \"The percentage of production traffic that the target version of an CloudFormation blue/green deployment receives.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-cloud-formation-target-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: CloudFormationTarget
---
