---
description: DescribeAutoScalingNotificationTypesAnswer schema from Auto Scaling
layout: schema
name: DescribeAutoScalingNotificationTypesAnswer
properties_list:
- description: ''
  name: AutoScalingNotificationTypes
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-describe-auto-scaling-notification-types-answer-schema.json
slug: ec2-auto-scaling-describe-auto-scaling-notification-types-answer
source_filename: ec2-auto-scaling-describe-auto-scaling-notification-types-answer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-auto-scaling-notification-types-answer-schema.json\",\n  \"title\": \"DescribeAutoScalingNotificationTypesAnswer\",\n  \"description\": \"DescribeAutoScalingNotificationTypesAnswer schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingNotificationTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingNotificationTypes\"\n        },\n        {\n          \"description\": \"The notification types.\"\n        }\n      ]\n    }\n  },\n  \"example\": {\n    \"AutoScalingNotificationTypes\": [\n      \"autoscaling:EC2_INSTANCE_LAUNCH\",\n      \"autoscaling:EC2_INSTANCE_LAUNCH_ERROR\",\n      \"autoscaling:EC2_INSTANCE_TERMINATE\",\n      \"autoscaling:EC2_INSTANCE_TERMINATE_ERROR\",\n      \"autoscaling:TEST_NOTIFICATION\"\
  \n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-auto-scaling-notification-types-answer-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: DescribeAutoScalingNotificationTypesAnswer
---
