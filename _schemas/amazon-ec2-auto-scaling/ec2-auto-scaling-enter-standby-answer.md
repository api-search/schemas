---
description: EnterStandbyAnswer schema from Auto Scaling
layout: schema
name: EnterStandbyAnswer
properties_list:
- description: ''
  name: Activities
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-enter-standby-answer-schema.json
slug: ec2-auto-scaling-enter-standby-answer
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-enter-standby-answer-schema.json\",\n  \"title\": \"EnterStandbyAnswer\",\n  \"description\": \"EnterStandbyAnswer schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Activities\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Activities\"\n        },\n        {\n          \"description\": \"The activities related to moving instances into <code>Standby</code> mode.\"\n        }\n      ]\n    }\n  },\n  \"example\": {\n    \"Activities\": [\n      {\n        \"ActivityId\": \"ffa056b4-6ed3-41ba-ae7c-249dfae6eba1\",\n        \"AutoScalingGroupName\": \"my-auto-scaling-group\",\n        \"Cause\": \"At 2015-04-12T15:10:23Z instance i-93633f9b was moved to standby in response to a user request, shrinking the capacity from\
  \ 2 to 1.\",\n        \"Description\": \"Moving EC2 instance to Standby: i-93633f9b\",\n        \"Details\": \"details\",\n        \"Progress\": 50,\n        \"StartTime\": \"2015-04-12T15:10:23.640000+00:00\",\n        \"StatusCode\": \"InProgress\"\n      }\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-enter-standby-answer-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: EnterStandbyAnswer
---
