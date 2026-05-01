---
description: CancelInstanceRefreshAnswer schema from Auto Scaling
layout: schema
name: CancelInstanceRefreshAnswer
properties_list:
- description: ''
  name: InstanceRefreshId
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-cancel-instance-refresh-answer-schema.json
slug: ec2-auto-scaling-cancel-instance-refresh-answer
source_filename: ec2-auto-scaling-cancel-instance-refresh-answer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-cancel-instance-refresh-answer-schema.json\",\n  \"title\": \"CancelInstanceRefreshAnswer\",\n  \"description\": \"CancelInstanceRefreshAnswer schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceRefreshId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The instance refresh ID associated with the request. This is the unique ID assigned to the instance refresh when it was started.\"\n        }\n      ]\n    }\n  },\n  \"example\": {\n    \"InstanceRefreshId\": \"08b91cf7-8fa6-48af-b6a6-d227f40f1b9b\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-cancel-instance-refresh-answer-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: CancelInstanceRefreshAnswer
---
