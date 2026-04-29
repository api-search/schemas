---
description: Describes a granularity of a metric.
layout: schema
name: MetricGranularityType
properties_list:
- description: ''
  name: Granularity
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-metric-granularity-type-schema.json
slug: ec2-auto-scaling-metric-granularity-type
source_filename: ec2-auto-scaling-metric-granularity-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-metric-granularity-type-schema.json\",\n  \"title\": \"MetricGranularityType\",\n  \"description\": \"Describes a granularity of a metric.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Granularity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The granularity. The only valid value is <code>1Minute</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-metric-granularity-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: MetricGranularityType
---
