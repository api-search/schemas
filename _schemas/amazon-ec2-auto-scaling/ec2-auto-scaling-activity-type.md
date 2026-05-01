---
description: ActivityType schema from Auto Scaling
layout: schema
name: ActivityType
properties_list:
- description: ''
  name: Activity
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-activity-type-schema.json
slug: ec2-auto-scaling-activity-type
source_filename: ec2-auto-scaling-activity-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-activity-type-schema.json\",\n  \"title\": \"ActivityType\",\n  \"description\": \"ActivityType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Activity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Activity\"\n        },\n        {\n          \"description\": \"A scaling activity.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-activity-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: ActivityType
---
