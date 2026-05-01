---
description: Describes an alarm.
layout: schema
name: Alarm
properties_list:
- description: ''
  name: AlarmName
  type: object
- description: ''
  name: AlarmARN
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-alarm-schema.json
slug: ec2-auto-scaling-alarm
source_filename: ec2-auto-scaling-alarm-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-alarm-schema.json\",\n  \"title\": \"Alarm\",\n  \"description\": \"Describes an alarm.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AlarmName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the alarm.\"\n        }\n      ]\n    },\n    \"AlarmARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the alarm.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-alarm-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: Alarm
---
