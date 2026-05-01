---
description: DescribeAdjustmentTypesAnswer schema from Auto Scaling
layout: schema
name: DescribeAdjustmentTypesAnswer
properties_list:
- description: ''
  name: AdjustmentTypes
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-describe-adjustment-types-answer-schema.json
slug: ec2-auto-scaling-describe-adjustment-types-answer
source_filename: ec2-auto-scaling-describe-adjustment-types-answer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-adjustment-types-answer-schema.json\",\n  \"title\": \"DescribeAdjustmentTypesAnswer\",\n  \"description\": \"DescribeAdjustmentTypesAnswer schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdjustmentTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdjustmentTypes\"\n        },\n        {\n          \"description\": \"The policy adjustment types.\"\n        }\n      ]\n    }\n  },\n  \"example\": {\n    \"AdjustmentTypes\": [\n      {\n        \"AdjustmentType\": \"ChangeInCapacity\"\n      },\n      {\n        \"AdjustmentType\": \"ExactCapcity\"\n      },\n      {\n        \"AdjustmentType\": \"PercentChangeInCapacity\"\n      }\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-adjustment-types-answer-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: DescribeAdjustmentTypesAnswer
---
