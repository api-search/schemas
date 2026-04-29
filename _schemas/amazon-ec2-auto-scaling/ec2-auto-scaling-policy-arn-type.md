---
description: Contains the output of PutScalingPolicy.
layout: schema
name: PolicyARNType
properties_list:
- description: ''
  name: PolicyARN
  type: object
- description: ''
  name: Alarms
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-policy-arn-type-schema.json
slug: ec2-auto-scaling-policy-arn-type
source_filename: ec2-auto-scaling-policy-arn-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-policy-arn-type-schema.json\",\n  \"title\": \"PolicyARNType\",\n  \"description\": \"Contains the output of PutScalingPolicy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PolicyARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the policy.\"\n        }\n      ]\n    },\n    \"Alarms\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Alarms\"\n        },\n        {\n          \"description\": \"The CloudWatch alarms created for the target tracking scaling policy.\"\n        }\n      ]\n    }\n  },\n  \"example\": {\n    \"Alarms\": [\n      {\n        \"AlarmARN\": \"arn:aws:cloudwatch:us-west-2:123456789012:alarm:TargetTracking-my-asg-AlarmHigh-fc0e4183-23ac-497e-9992-691c9980c38e\"\
  ,\n        \"AlarmName\": \"TargetTracking-my-asg-AlarmHigh-fc0e4183-23ac-497e-9992-691c9980c38e\"\n      },\n      {\n        \"AlarmARN\": \"arn:aws:cloudwatch:us-west-2:123456789012:alarm:TargetTracking-my-asg-AlarmLow-61a39305-ed0c-47af-bd9e-471a352ee1a2\",\n        \"AlarmName\": \"TargetTracking-my-asg-AlarmLow-61a39305-ed0c-47af-bd9e-471a352ee1a2\"\n      }\n    ],\n    \"PolicyARN\": \"arn:aws:autoscaling:us-west-2:123456789012:scalingPolicy:228f02c2-c665-4bfd-aaac-8b04080bea3c:autoScalingGroupName/my-auto-scaling-group:policyName/alb1000-target-tracking-scaling-policy\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-policy-arn-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: PolicyARNType
---
