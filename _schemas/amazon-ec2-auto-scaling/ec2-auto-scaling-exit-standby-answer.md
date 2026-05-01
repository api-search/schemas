---
description: ExitStandbyAnswer schema from Auto Scaling
layout: schema
name: ExitStandbyAnswer
properties_list:
- description: ''
  name: Activities
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-exit-standby-answer-schema.json
slug: ec2-auto-scaling-exit-standby-answer
source_filename: ec2-auto-scaling-exit-standby-answer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-exit-standby-answer-schema.json\",\n  \"title\": \"ExitStandbyAnswer\",\n  \"description\": \"ExitStandbyAnswer schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Activities\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Activities\"\n        },\n        {\n          \"description\": \"The activities related to moving instances out of <code>Standby</code> mode.\"\n        }\n      ]\n    }\n  },\n  \"example\": {\n    \"Activities\": [\n      {\n        \"ActivityId\": \"142928e1-a2dc-453a-9b24-b85ad6735928\",\n        \"AutoScalingGroupName\": \"my-auto-scaling-group\",\n        \"Cause\": \"At 2015-04-12T15:14:29Z instance i-93633f9b was moved out of standby in response to a user request, increasing the capacity from\
  \ 1 to 2.\",\n        \"Description\": \"Moving EC2 instance out of Standby: i-93633f9b\",\n        \"Details\": \"details\",\n        \"Progress\": 30,\n        \"StartTime\": \"2015-04-12T15:14:29.886000+00:00\",\n        \"StatusCode\": \"PreInService\"\n      }\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-exit-standby-answer-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: ExitStandbyAnswer
---
