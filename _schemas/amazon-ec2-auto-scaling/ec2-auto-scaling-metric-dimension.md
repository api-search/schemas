---
description: Describes the dimension of a metric.
layout: schema
name: MetricDimension
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-metric-dimension-schema.json
slug: ec2-auto-scaling-metric-dimension
source_filename: ec2-auto-scaling-metric-dimension-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-metric-dimension-schema.json\",\n  \"title\": \"MetricDimension\",\n  \"description\": \"Describes the dimension of a metric.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricDimensionName\"\n        },\n        {\n          \"description\": \"The name of the dimension.\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricDimensionValue\"\n        },\n        {\n          \"description\": \"The value of the dimension.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"Value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-metric-dimension-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: MetricDimension
---
