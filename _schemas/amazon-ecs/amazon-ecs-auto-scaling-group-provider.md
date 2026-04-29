---
description: ''
layout: schema
name: AutoScalingGroupProvider
properties_list:
- description: The ARN of the Auto Scaling group.
  name: autoScalingGroupArn
  type: string
- description: ''
  name: managedScaling
  type: object
- description: ''
  name: managedTerminationProtection
  type: string
- description: ''
  name: managedDraining
  type: string
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-auto-scaling-group-provider-schema.json
slug: amazon-ecs-auto-scaling-group-provider
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AutoScalingGroupProvider\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"autoScalingGroupArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the Auto Scaling group.\"\n    },\n    \"managedScaling\": {\n      \"type\": \"object\"\n    },\n    \"managedTerminationProtection\": {\n      \"type\": \"string\"\n    },\n    \"managedDraining\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-auto-scaling-group-provider-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: AutoScalingGroupProvider
---
