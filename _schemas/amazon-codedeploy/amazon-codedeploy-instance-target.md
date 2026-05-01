---
description: A target Amazon EC2 or on-premises instance during a deployment that uses the EC2/On-premises compute platform.
layout: schema
name: InstanceTarget
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
  name: instanceLabel
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-instance-target-schema.json
slug: amazon-codedeploy-instance-target
source_filename: amazon-codedeploy-instance-target-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-instance-target-schema.json\",\n  \"title\": \"InstanceTarget\",\n  \"description\": \" A target Amazon EC2 or on-premises instance during a deployment that uses the EC2/On-premises compute platform. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentId\"\n        },\n        {\n          \"description\": \" The unique ID of a deployment. \"\n        }\n      ]\n    },\n    \"targetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetId\"\n        },\n        {\n          \"description\": \" The unique ID of a deployment target that has a type of <code>instanceTarget</code>. \"\n        }\n      ]\n    },\n    \"targetArn\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/TargetArn\"\n        },\n        {\n          \"description\": \" The Amazon Resource Name (ARN) of the target. \"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetStatus\"\n        },\n        {\n          \"description\": \" The status an EC2/On-premises deployment's target instance. \"\n        }\n      ]\n    },\n    \"lastUpdatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Time\"\n        },\n        {\n          \"description\": \" The date and time when the target instance was updated by a deployment. \"\n        }\n      ]\n    },\n    \"lifecycleEvents\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LifecycleEventList\"\n        },\n        {\n          \"description\": \" The lifecycle events of the deployment to this target instance. \"\n        }\n      ]\n    },\n    \"\
  instanceLabel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetLabel\"\n        },\n        {\n          \"description\": \" A label that identifies whether the instance is an original target (<code>BLUE</code>) or a replacement target (<code>GREEN</code>). \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-instance-target-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: InstanceTarget
---
