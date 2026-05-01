---
description: DetachInstancesAnswer schema from Auto Scaling
layout: schema
name: DetachInstancesAnswer
properties_list:
- description: ''
  name: Activities
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-detach-instances-answer-schema.json
slug: ec2-auto-scaling-detach-instances-answer
source_filename: ec2-auto-scaling-detach-instances-answer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-detach-instances-answer-schema.json\",\n  \"title\": \"DetachInstancesAnswer\",\n  \"description\": \"DetachInstancesAnswer schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Activities\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Activities\"\n        },\n        {\n          \"description\": \"The activities related to detaching the instances from the Auto Scaling group.\"\n        }\n      ]\n    }\n  },\n  \"example\": {\n    \"Activities\": [\n      {\n        \"ActivityId\": \"5091cb52-547a-47ce-a236-c9ccbc2cb2c9\",\n        \"AutoScalingGroupName\": \"my-auto-scaling-group\",\n        \"Cause\": \"At 2015-04-12T15:02:16Z instance i-93633f9b was detached in response to a user request, shrinking the capacity\
  \ from 2 to 1.\",\n        \"Description\": \"Detaching EC2 instance: i-93633f9b\",\n        \"Details\": \"details\",\n        \"Progress\": 50,\n        \"StartTime\": \"2015-04-12T15:02:16.179000+00:00\",\n        \"StatusCode\": \"InProgress\"\n      }\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-detach-instances-answer-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: DetachInstancesAnswer
---
