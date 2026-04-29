---
description: Describes a custom scaling metric for a predictive scaling policy.
layout: schema
name: PredictiveScalingCustomizedScalingMetric
properties_list:
- description: ''
  name: MetricDataQueries
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-predictive-scaling-customized-scaling-metric-schema.json
slug: ec2-auto-scaling-predictive-scaling-customized-scaling-metric
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-predictive-scaling-customized-scaling-metric-schema.json\",\n  \"title\": \"PredictiveScalingCustomizedScalingMetric\",\n  \"description\": \"Describes a custom scaling metric for a predictive scaling policy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MetricDataQueries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricDataQueries\"\n        },\n        {\n          \"description\": \"One or more metric data queries to provide the data points for a scaling metric. Use multiple metric data queries only if you are performing a math expression on returned data. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MetricDataQueries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-predictive-scaling-customized-scaling-metric-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: PredictiveScalingCustomizedScalingMetric
---
