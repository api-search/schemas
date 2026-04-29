---
description: Information about an Auto Scaling group.
layout: schema
name: AutoScalingGroup
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: hook
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-auto-scaling-group-schema.json
slug: amazon-codedeploy-auto-scaling-group
source_filename: amazon-codedeploy-auto-scaling-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-auto-scaling-group-schema.json\",\n  \"title\": \"AutoScalingGroup\",\n  \"description\": \"Information about an Auto Scaling group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupName\"\n        },\n        {\n          \"description\": \"The Auto Scaling group name.\"\n        }\n      ]\n    },\n    \"hook\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupHook\"\n        },\n        {\n          \"description\": \"An Auto Scaling lifecycle event hook name.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-auto-scaling-group-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: AutoScalingGroup
---
