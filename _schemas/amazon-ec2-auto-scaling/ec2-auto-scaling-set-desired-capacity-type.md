---
description: SetDesiredCapacityType schema from Auto Scaling
layout: schema
name: SetDesiredCapacityType
properties_list:
- description: ''
  name: AutoScalingGroupName
  type: object
- description: ''
  name: DesiredCapacity
  type: object
- description: ''
  name: HonorCooldown
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-set-desired-capacity-type-schema.json
slug: ec2-auto-scaling-set-desired-capacity-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-set-desired-capacity-type-schema.json\",\n  \"title\": \"SetDesiredCapacityType\",\n  \"description\": \"SetDesiredCapacityType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"DesiredCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupDesiredCapacity\"\n        },\n        {\n          \"description\": \"The desired capacity is the initial capacity of the Auto Scaling group after this operation completes and the capacity it attempts to maintain.\"\n\
  \        }\n      ]\n    },\n    \"HonorCooldown\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HonorCooldown\"\n        },\n        {\n          \"description\": \"Indicates whether Amazon EC2 Auto Scaling waits for the cooldown period to complete before initiating a scaling activity to set your Auto Scaling group to its new capacity. By default, Amazon EC2 Auto Scaling does not honor the cooldown period during manual scaling activities.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AutoScalingGroupName\",\n    \"DesiredCapacity\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-set-desired-capacity-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: SetDesiredCapacityType
---
