---
description: StartInstanceRefreshAnswer schema from Auto Scaling
layout: schema
name: StartInstanceRefreshAnswer
properties_list:
- description: ''
  name: InstanceRefreshId
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-start-instance-refresh-answer-schema.json
slug: ec2-auto-scaling-start-instance-refresh-answer
source_filename: ec2-auto-scaling-start-instance-refresh-answer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-start-instance-refresh-answer-schema.json\",\n  \"title\": \"StartInstanceRefreshAnswer\",\n  \"description\": \"StartInstanceRefreshAnswer schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceRefreshId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"A unique ID for tracking the progress of the instance refresh.\"\n        }\n      ]\n    }\n  },\n  \"example\": {\n    \"InstanceRefreshId\": \"08b91cf7-8fa6-48af-b6a6-d227f40f1b9b\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-start-instance-refresh-answer-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: StartInstanceRefreshAnswer
---
