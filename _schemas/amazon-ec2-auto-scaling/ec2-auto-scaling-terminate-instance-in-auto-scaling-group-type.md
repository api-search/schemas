---
description: TerminateInstanceInAutoScalingGroupType schema from Auto Scaling
layout: schema
name: TerminateInstanceInAutoScalingGroupType
properties_list:
- description: ''
  name: InstanceId
  type: object
- description: ''
  name: ShouldDecrementDesiredCapacity
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-terminate-instance-in-auto-scaling-group-type-schema.json
slug: ec2-auto-scaling-terminate-instance-in-auto-scaling-group-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-terminate-instance-in-auto-scaling-group-type-schema.json\",\n  \"title\": \"TerminateInstanceInAutoScalingGroupType\",\n  \"description\": \"TerminateInstanceInAutoScalingGroupType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen19\"\n        },\n        {\n          \"description\": \"The ID of the instance.\"\n        }\n      ]\n    },\n    \"ShouldDecrementDesiredCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShouldDecrementDesiredCapacity\"\n        },\n        {\n          \"description\": \"Indicates whether terminating the instance also decrements the size of the Auto Scaling group.\"\n    \
  \    }\n      ]\n    }\n  },\n  \"required\": [\n    \"InstanceId\",\n    \"ShouldDecrementDesiredCapacity\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-terminate-instance-in-auto-scaling-group-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: TerminateInstanceInAutoScalingGroupType
---
