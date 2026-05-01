---
description: RollbackInstanceRefreshAnswer schema from Auto Scaling
layout: schema
name: RollbackInstanceRefreshAnswer
properties_list:
- description: ''
  name: InstanceRefreshId
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-rollback-instance-refresh-answer-schema.json
slug: ec2-auto-scaling-rollback-instance-refresh-answer
source_filename: ec2-auto-scaling-rollback-instance-refresh-answer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-rollback-instance-refresh-answer-schema.json\",\n  \"title\": \"RollbackInstanceRefreshAnswer\",\n  \"description\": \"RollbackInstanceRefreshAnswer schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceRefreshId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The instance refresh ID associated with the request. This is the unique ID assigned to the instance refresh when it was started.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-rollback-instance-refresh-answer-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: RollbackInstanceRefreshAnswer
---
