---
description: Information about the target of an Amazon ECS deployment.
layout: schema
name: ECSTarget
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
  name: lastUpdatedAt
  type: object
- description: ''
  name: lifecycleEvents
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: taskSetsInfo
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-ecs-target-schema.json
slug: amazon-codedeploy-ecs-target
source_filename: amazon-codedeploy-ecs-target-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-ecs-target-schema.json\",\n  \"title\": \"ECSTarget\",\n  \"description\": \" Information about the target of an Amazon ECS deployment. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentId\"\n        },\n        {\n          \"description\": \" The unique ID of a deployment. \"\n        }\n      ]\n    },\n    \"targetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetId\"\n        },\n        {\n          \"description\": \" The unique ID of a deployment target that has a type of <code>ecsTarget</code>. \"\n        }\n      ]\n    },\n    \"targetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetArn\"\
  \n        },\n        {\n          \"description\": \" The Amazon Resource Name (ARN) of the target. \"\n        }\n      ]\n    },\n    \"lastUpdatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Time\"\n        },\n        {\n          \"description\": \" The date and time when the target Amazon ECS application was updated by a deployment. \"\n        }\n      ]\n    },\n    \"lifecycleEvents\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LifecycleEventList\"\n        },\n        {\n          \"description\": \" The lifecycle events of the deployment to this target Amazon ECS application. \"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetStatus\"\n        },\n        {\n          \"description\": \" The status an Amazon ECS deployment's target ECS application. \"\n        }\n      ]\n    },\n    \"taskSetsInfo\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/ECSTaskSetList\"\n        },\n        {\n          \"description\": \" The <code>ECSTaskSet</code> objects associated with the ECS target. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-ecs-target-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: ECSTarget
---
