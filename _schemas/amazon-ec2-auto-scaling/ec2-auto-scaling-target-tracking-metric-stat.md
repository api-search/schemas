---
description: <p>This structure defines the CloudWatch metric to return, along with the statistic and unit.</p> <p>For more information about the CloudWatch terminology below, see <a href="https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/cloudwatch_concepts.html">Amazon CloudWatch concepts</a> in the <i>Amazon CloudWatch User Guide</i>.</p>
layout: schema
name: TargetTrackingMetricStat
properties_list:
- description: ''
  name: Metric
  type: object
- description: ''
  name: Stat
  type: object
- description: ''
  name: Unit
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-target-tracking-metric-stat-schema.json
slug: ec2-auto-scaling-target-tracking-metric-stat
source_filename: ec2-auto-scaling-target-tracking-metric-stat-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-target-tracking-metric-stat-schema.json\",\n  \"title\": \"TargetTrackingMetricStat\",\n  \"description\": \"<p>This structure defines the CloudWatch metric to return, along with the statistic and unit.</p> <p>For more information about the CloudWatch terminology below, see <a href=\\\"https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/cloudwatch_concepts.html\\\">Amazon CloudWatch concepts</a> in the <i>Amazon CloudWatch User Guide</i>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Metric\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Metric\"\n        },\n        {\n          \"description\": \"The metric to use.\"\n        }\n      ]\n    },\n    \"Stat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMetricStat\"\
  \n        },\n        {\n          \"description\": \"<p>The statistic to return. It can include any CloudWatch statistic or extended statistic. For a list of valid values, see the table in <a href=\\\"https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/cloudwatch_concepts.html#Statistic\\\">Statistics</a> in the <i>Amazon CloudWatch User Guide</i>.</p> <p>The most commonly used metric for scaling is <code>Average</code>.</p>\"\n        }\n      ]\n    },\n    \"Unit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricUnit\"\n        },\n        {\n          \"description\": \"The unit to use for the returned data points. For a complete list of the units that CloudWatch supports, see the <a href=\\\"https://docs.aws.amazon.com/AmazonCloudWatch/latest/APIReference/API_MetricDatum.html\\\">MetricDatum</a> data type in the <i>Amazon CloudWatch API Reference</i>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Metric\",\n    \"Stat\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-target-tracking-metric-stat-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: TargetTrackingMetricStat
---
