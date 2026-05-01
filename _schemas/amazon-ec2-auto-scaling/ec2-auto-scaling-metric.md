---
description: Represents a specific metric.
layout: schema
name: Metric
properties_list:
- description: ''
  name: Namespace
  type: object
- description: ''
  name: MetricName
  type: object
- description: ''
  name: Dimensions
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-metric-schema.json
slug: ec2-auto-scaling-metric
source_filename: ec2-auto-scaling-metric-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-metric-schema.json\",\n  \"title\": \"Metric\",\n  \"description\": \"Represents a specific metric. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Namespace\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricNamespace\"\n        },\n        {\n          \"description\": \"The namespace of the metric. For more information, see the table in <a href=\\\"https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/aws-services-cloudwatch-metrics.html\\\">Amazon Web Services services that publish CloudWatch metrics </a> in the <i>Amazon CloudWatch User Guide</i>.\"\n        }\n      ]\n    },\n    \"MetricName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricName\"\n        },\n        {\n          \"\
  description\": \"The name of the metric.\"\n        }\n      ]\n    },\n    \"Dimensions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricDimensions\"\n        },\n        {\n          \"description\": \"<p>The dimensions for the metric. For the list of available dimensions, see the Amazon Web Services documentation available from the table in <a href=\\\"https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/aws-services-cloudwatch-metrics.html\\\">Amazon Web Services services that publish CloudWatch metrics </a> in the <i>Amazon CloudWatch User Guide</i>. </p> <p>Conditional: If you published your metric with dimensions, you must specify the same dimensions in your scaling policy.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Namespace\",\n    \"MetricName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-metric-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: Metric
---
