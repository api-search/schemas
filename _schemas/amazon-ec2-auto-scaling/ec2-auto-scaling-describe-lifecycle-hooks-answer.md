---
description: DescribeLifecycleHooksAnswer schema from Auto Scaling
layout: schema
name: DescribeLifecycleHooksAnswer
properties_list:
- description: ''
  name: LifecycleHooks
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-describe-lifecycle-hooks-answer-schema.json
slug: ec2-auto-scaling-describe-lifecycle-hooks-answer
source_filename: ec2-auto-scaling-describe-lifecycle-hooks-answer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-lifecycle-hooks-answer-schema.json\",\n  \"title\": \"DescribeLifecycleHooksAnswer\",\n  \"description\": \"DescribeLifecycleHooksAnswer schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LifecycleHooks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LifecycleHooks\"\n        },\n        {\n          \"description\": \"The lifecycle hooks for the specified group.\"\n        }\n      ]\n    }\n  },\n  \"example\": {\n    \"LifecycleHooks\": [\n      {\n        \"AutoScalingGroupName\": \"my-auto-scaling-group\",\n        \"DefaultResult\": \"ABANDON\",\n        \"GlobalTimeout\": 172800,\n        \"HeartbeatTimeout\": 3600,\n        \"LifecycleHookName\": \"my-lifecycle-hook\",\n        \"LifecycleTransition\"\
  : \"autoscaling:EC2_INSTANCE_LAUNCHING\",\n        \"NotificationTargetARN\": \"arn:aws:sns:us-west-2:123456789012:my-sns-topic\",\n        \"RoleARN\": \"arn:aws:iam::123456789012:role/my-auto-scaling-role\"\n      }\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-lifecycle-hooks-answer-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: DescribeLifecycleHooksAnswer
---
