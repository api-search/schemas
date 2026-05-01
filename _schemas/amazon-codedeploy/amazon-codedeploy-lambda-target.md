---
description: Information about the target Lambda function during an Lambda deployment.
layout: schema
name: LambdaTarget
properties_list:
- description: ''
  name: deploymentId
  type: object
- description: ''
  name: targetId
  type: object
- description: ''
  name: targetArn
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
  name: lambdaFunctionInfo
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-lambda-target-schema.json
slug: amazon-codedeploy-lambda-target
source_filename: amazon-codedeploy-lambda-target-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-lambda-target-schema.json\",\n  \"title\": \"LambdaTarget\",\n  \"description\": \" Information about the target Lambda function during an Lambda deployment. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentId\"\n        },\n        {\n          \"description\": \" The unique ID of a deployment. \"\n        }\n      ]\n    },\n    \"targetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetId\"\n        },\n        {\n          \"description\": \" The unique ID of a deployment target that has a type of <code>lambdaTarget</code>. \"\n        }\n      ]\n    },\n    \"targetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetArn\"\
  \n        },\n        {\n          \"description\": \" The Amazon Resource Name (ARN) of the target. \"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetStatus\"\n        },\n        {\n          \"description\": \" The status an Lambda deployment's target Lambda function. \"\n        }\n      ]\n    },\n    \"lastUpdatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Time\"\n        },\n        {\n          \"description\": \" The date and time when the target Lambda function was updated by a deployment. \"\n        }\n      ]\n    },\n    \"lifecycleEvents\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LifecycleEventList\"\n        },\n        {\n          \"description\": \" The lifecycle events of the deployment to this target Lambda function. \"\n        }\n      ]\n    },\n    \"lambdaFunctionInfo\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/LambdaFunctionInfo\"\n        },\n        {\n          \"description\": \" A <code>LambdaFunctionInfo</code> object that describes a target Lambda function. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-lambda-target-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: LambdaTarget
---
