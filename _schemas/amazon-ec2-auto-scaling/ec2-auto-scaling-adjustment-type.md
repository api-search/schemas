---
description: Describes a policy adjustment type.
layout: schema
name: AdjustmentType
properties_list:
- description: ''
  name: AdjustmentType
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-adjustment-type-schema.json
slug: ec2-auto-scaling-adjustment-type
source_filename: ec2-auto-scaling-adjustment-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-adjustment-type-schema.json\",\n  \"title\": \"AdjustmentType\",\n  \"description\": \"Describes a policy adjustment type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdjustmentType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The policy adjustment type. The valid values are <code>ChangeInCapacity</code>, <code>ExactCapacity</code>, and <code>PercentChangeInCapacity</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-adjustment-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: AdjustmentType
---
