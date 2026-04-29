---
description: Describes an enabled Auto Scaling group metric.
layout: schema
name: EnabledMetric
properties_list:
- description: ''
  name: Metric
  type: object
- description: ''
  name: Granularity
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-enabled-metric-schema.json
slug: ec2-auto-scaling-enabled-metric
source_filename: ec2-auto-scaling-enabled-metric-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-enabled-metric-schema.json\",\n  \"title\": \"EnabledMetric\",\n  \"description\": \"Describes an enabled Auto Scaling group metric.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Metric\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"<p>One of the following metrics:</p> <ul> <li> <p> <code>GroupMinSize</code> </p> </li> <li> <p> <code>GroupMaxSize</code> </p> </li> <li> <p> <code>GroupDesiredCapacity</code> </p> </li> <li> <p> <code>GroupInServiceInstances</code> </p> </li> <li> <p> <code>GroupPendingInstances</code> </p> </li> <li> <p> <code>GroupStandbyInstances</code> </p> </li> <li> <p> <code>GroupTerminatingInstances</code> </p> </li> <li> <p> <code>GroupTotalInstances</code>\
  \ </p> </li> <li> <p> <code>GroupInServiceCapacity</code> </p> </li> <li> <p> <code>GroupPendingCapacity</code> </p> </li> <li> <p> <code>GroupStandbyCapacity</code> </p> </li> <li> <p> <code>GroupTerminatingCapacity</code> </p> </li> <li> <p> <code>GroupTotalCapacity</code> </p> </li> <li> <p> <code>WarmPoolDesiredCapacity</code> </p> </li> <li> <p> <code>WarmPoolWarmedCapacity</code> </p> </li> <li> <p> <code>WarmPoolPendingCapacity</code> </p> </li> <li> <p> <code>WarmPoolTerminatingCapacity</code> </p> </li> <li> <p> <code>WarmPoolTotalCapacity</code> </p> </li> <li> <p> <code>GroupAndWarmPoolDesiredCapacity</code> </p> </li> <li> <p> <code>GroupAndWarmPoolTotalCapacity</code> </p> </li> </ul> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/ec2-auto-scaling-cloudwatch-monitoring.html#as-group-metrics\\\">Auto Scaling group metrics</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"Granularity\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The granularity of the metric. The only valid value is <code>1Minute</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-enabled-metric-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: EnabledMetric
---
