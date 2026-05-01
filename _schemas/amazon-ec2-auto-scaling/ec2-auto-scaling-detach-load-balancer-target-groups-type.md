---
description: DetachLoadBalancerTargetGroupsType schema from Auto Scaling
layout: schema
name: DetachLoadBalancerTargetGroupsType
properties_list:
- description: ''
  name: AutoScalingGroupName
  type: object
- description: ''
  name: TargetGroupARNs
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-detach-load-balancer-target-groups-type-schema.json
slug: ec2-auto-scaling-detach-load-balancer-target-groups-type
source_filename: ec2-auto-scaling-detach-load-balancer-target-groups-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-detach-load-balancer-target-groups-type-schema.json\",\n  \"title\": \"DetachLoadBalancerTargetGroupsType\",\n  \"description\": \"DetachLoadBalancerTargetGroupsType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"TargetGroupARNs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetGroupARNs\"\n        },\n        {\n          \"description\": \"The Amazon Resource Names (ARN) of the target groups. You can specify up to 10 target groups.\"\n        }\n      ]\n    }\n \
  \ },\n  \"required\": [\n    \"AutoScalingGroupName\",\n    \"TargetGroupARNs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-detach-load-balancer-target-groups-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: DetachLoadBalancerTargetGroupsType
---
