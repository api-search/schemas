---
description: <p>Represents a CloudWatch metric of your choosing for a target tracking scaling policy to use with Amazon EC2 Auto Scaling.</p> <p>To create your customized metric specification:</p> <ul> <li> <p>Add values for each required property from CloudWatch. You can use an existing metric, or a new metric that you create. To use your own metric, you must first publish the metric to CloudWatch. For more information, see <a href="https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/publishingMetrics.html">Publish custom metrics</a> in the <i>Amazon CloudWatch User Guide</i>.</p> </li> <li> <p>Choose a metric that changes proportionally with capacity. The value of the metric should increase or decrease in inverse proportion to the number of capacity units. That is, the value of the metric should decrease when capacity increases.</p> </li> </ul> <p>For more information about the CloudWatch terminology below, see <a href="https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/cloudwatch_concepts.html">Amazon
  CloudWatch concepts</a>.</p> <note> <p>Each individual service provides information about the metrics, namespace, and dimensions they use. For more information, see <a href="https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/aws-services-cloudwatch-metrics.html">Amazon Web Services services that publish CloudWatch metrics</a> in the <i>Amazon CloudWatch User Guide</i>.</p> </note>
layout: schema
name: CustomizedMetricSpecification
properties_list:
- description: ''
  name: MetricName
  type: object
- description: ''
  name: Namespace
  type: object
- description: ''
  name: Dimensions
  type: object
- description: ''
  name: Statistic
  type: object
- description: ''
  name: Unit
  type: object
- description: ''
  name: Metrics
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-customized-metric-specification-schema.json
slug: ec2-auto-scaling-customized-metric-specification
source_filename: ec2-auto-scaling-customized-metric-specification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-customized-metric-specification-schema.json\",\n  \"title\": \"CustomizedMetricSpecification\",\n  \"description\": \"<p>Represents a CloudWatch metric of your choosing for a target tracking scaling policy to use with Amazon EC2 Auto Scaling.</p> <p>To create your customized metric specification:</p> <ul> <li> <p>Add values for each required property from CloudWatch. You can use an existing metric, or a new metric that you create. To use your own metric, you must first publish the metric to CloudWatch. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/publishingMetrics.html\\\">Publish custom metrics</a> in the <i>Amazon CloudWatch User Guide</i>.</p> </li> <li> <p>Choose a metric that changes proportionally with capacity. The\
  \ value of the metric should increase or decrease in inverse proportion to the number of capacity units. That is, the value of the metric should decrease when capacity increases.</p> </li> </ul> <p>For more information about the CloudWatch terminology below, see <a href=\\\"https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/cloudwatch_concepts.html\\\">Amazon CloudWatch concepts</a>.</p> <note> <p>Each individual service provides information about the metrics, namespace, and dimensions they use. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/aws-services-cloudwatch-metrics.html\\\">Amazon Web Services services that publish CloudWatch metrics</a> in the <i>Amazon CloudWatch User Guide</i>.</p> </note>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MetricName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricName\"\n        },\n        {\n          \"description\": \"The name of\
  \ the metric. To get the exact metric name, namespace, and dimensions, inspect the <a href=\\\"https://docs.aws.amazon.com/AmazonCloudWatch/latest/APIReference/API_Metric.html\\\">Metric</a> object that is returned by a call to <a href=\\\"https://docs.aws.amazon.com/AmazonCloudWatch/latest/APIReference/API_ListMetrics.html\\\">ListMetrics</a>.\"\n        }\n      ]\n    },\n    \"Namespace\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricNamespace\"\n        },\n        {\n          \"description\": \"The namespace of the metric.\"\n        }\n      ]\n    },\n    \"Dimensions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricDimensions\"\n        },\n        {\n          \"description\": \"<p>The dimensions of the metric.</p> <p>Conditional: If you published your metric with dimensions, you must specify the same dimensions in your scaling policy.</p>\"\n        }\n      ]\n    },\n    \"Statistic\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricStatistic\"\n        },\n        {\n          \"description\": \"The statistic of the metric.\"\n        }\n      ]\n    },\n    \"Unit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricUnit\"\n        },\n        {\n          \"description\": \"The unit of the metric. For a complete list of the units that CloudWatch supports, see the <a href=\\\"https://docs.aws.amazon.com/AmazonCloudWatch/latest/APIReference/API_MetricDatum.html\\\">MetricDatum</a> data type in the <i>Amazon CloudWatch API Reference</i>.\"\n        }\n      ]\n    },\n    \"Metrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetTrackingMetricDataQueries\"\n        },\n        {\n          \"description\": \"The metrics to include in the target tracking scaling policy, as a metric data query. This can include both raw metric and metric math expressions.\"\n        }\n     \
  \ ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-customized-metric-specification-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: CustomizedMetricSpecification
---
