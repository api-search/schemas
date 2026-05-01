---
description: DescribeLifecycleHookTypesAnswer schema from Auto Scaling
layout: schema
name: DescribeLifecycleHookTypesAnswer
properties_list:
- description: ''
  name: LifecycleHookTypes
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-describe-lifecycle-hook-types-answer-schema.json
slug: ec2-auto-scaling-describe-lifecycle-hook-types-answer
source_filename: ec2-auto-scaling-describe-lifecycle-hook-types-answer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-lifecycle-hook-types-answer-schema.json\",\n  \"title\": \"DescribeLifecycleHookTypesAnswer\",\n  \"description\": \"DescribeLifecycleHookTypesAnswer schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LifecycleHookTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingNotificationTypes\"\n        },\n        {\n          \"description\": \"The lifecycle hook types.\"\n        }\n      ]\n    }\n  },\n  \"example\": {\n    \"LifecycleHookTypes\": [\n      \"autoscaling:EC2_INSTANCE_LAUNCHING\",\n      \"autoscaling:EC2_INSTANCE_TERMINATING\"\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-lifecycle-hook-types-answer-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: DescribeLifecycleHookTypesAnswer
---
