---
description: EnableMetricsCollectionQuery schema from Auto Scaling
layout: schema
name: EnableMetricsCollectionQuery
properties_list:
- description: ''
  name: AutoScalingGroupName
  type: object
- description: ''
  name: Metrics
  type: object
- description: ''
  name: Granularity
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-enable-metrics-collection-query-schema.json
slug: ec2-auto-scaling-enable-metrics-collection-query
source_filename: ec2-auto-scaling-enable-metrics-collection-query-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-enable-metrics-collection-query-schema.json\",\n  \"title\": \"EnableMetricsCollectionQuery\",\n  \"description\": \"EnableMetricsCollectionQuery schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"Metrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Metrics\"\n        },\n        {\n          \"description\": \"<p>Identifies the metrics to enable.</p> <p>You can specify one or more of the following metrics:</p> <ul> <li> <p> <code>GroupMinSize</code> </p> </li> <li> <p>\
  \ <code>GroupMaxSize</code> </p> </li> <li> <p> <code>GroupDesiredCapacity</code> </p> </li> <li> <p> <code>GroupInServiceInstances</code> </p> </li> <li> <p> <code>GroupPendingInstances</code> </p> </li> <li> <p> <code>GroupStandbyInstances</code> </p> </li> <li> <p> <code>GroupTerminatingInstances</code> </p> </li> <li> <p> <code>GroupTotalInstances</code> </p> </li> <li> <p> <code>GroupInServiceCapacity</code> </p> </li> <li> <p> <code>GroupPendingCapacity</code> </p> </li> <li> <p> <code>GroupStandbyCapacity</code> </p> </li> <li> <p> <code>GroupTerminatingCapacity</code> </p> </li> <li> <p> <code>GroupTotalCapacity</code> </p> </li> <li> <p> <code>WarmPoolDesiredCapacity</code> </p> </li> <li> <p> <code>WarmPoolWarmedCapacity</code> </p> </li> <li> <p> <code>WarmPoolPendingCapacity</code> </p> </li> <li> <p> <code>WarmPoolTerminatingCapacity</code> </p> </li> <li> <p> <code>WarmPoolTotalCapacity</code> </p> </li> <li> <p> <code>GroupAndWarmPoolDesiredCapacity</code> </p> </li> <li>\
  \ <p> <code>GroupAndWarmPoolTotalCapacity</code> </p> </li> </ul> <p>If you specify <code>Granularity</code> and don't specify any metrics, all metrics are enabled.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/ec2-auto-scaling-cloudwatch-monitoring.html#as-group-metrics\\\">Auto Scaling group metrics</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"Granularity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The frequency at which Amazon EC2 Auto Scaling sends aggregated data to CloudWatch. The only valid value is <code>1Minute</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AutoScalingGroupName\",\n    \"Granularity\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-enable-metrics-collection-query-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: EnableMetricsCollectionQuery
---
