---
description: ExcludedInstanceTypes schema from Auto Scaling
layout: schema
name: ExcludedInstanceTypes
properties_list: []
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-excluded-instance-types-schema.json
slug: ec2-auto-scaling-excluded-instance-types
source_filename: ec2-auto-scaling-excluded-instance-types-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-excluded-instance-types-schema.json\",\n  \"title\": \"ExcludedInstanceTypes\",\n  \"description\": \"ExcludedInstanceTypes schema from Auto Scaling\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/ExcludedInstance\"\n  },\n  \"maxItems\": 400\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-excluded-instance-types-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: ExcludedInstanceTypes
---
