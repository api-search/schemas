---
description: Information about two target groups and how traffic is routed during an Amazon ECS deployment. An optional test traffic route can be specified.
layout: schema
name: TargetGroupPairInfo
properties_list:
- description: ''
  name: targetGroups
  type: object
- description: ''
  name: prodTrafficRoute
  type: object
- description: ''
  name: testTrafficRoute
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-target-group-pair-info-schema.json
slug: amazon-codedeploy-target-group-pair-info
source_filename: amazon-codedeploy-target-group-pair-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-target-group-pair-info-schema.json\",\n  \"title\": \"TargetGroupPairInfo\",\n  \"description\": \" Information about two target groups and how traffic is routed during an Amazon ECS deployment. An optional test traffic route can be specified. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"targetGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetGroupInfoList\"\n        },\n        {\n          \"description\": \" One pair of target groups. One is associated with the original task set. The second is associated with the task set that serves traffic after the deployment is complete. \"\n        }\n      ]\n    },\n    \"prodTrafficRoute\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TrafficRoute\"\n \
  \       },\n        {\n          \"description\": \" The path used by a load balancer to route production traffic when an Amazon ECS deployment is complete. \"\n        }\n      ]\n    },\n    \"testTrafficRoute\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TrafficRoute\"\n        },\n        {\n          \"description\": \" An optional path used by a load balancer to route test traffic after an Amazon ECS deployment. Validation can occur while test traffic is served during a deployment. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-target-group-pair-info-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: TargetGroupPairInfo
---
