---
description: <p>Describes a utilization metric of an Amazon Elastic Block Store (Amazon EBS) volume.</p> <p>Compare the utilization metric data of your resource against its projected utilization metric data to determine the performance difference between your current resource and the recommended option.</p>
layout: schema
name: EBSUtilizationMetric
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: statistic
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-ebs-utilization-metric-schema.json
slug: compute-optimizer-ebs-utilization-metric
source_filename: compute-optimizer-ebs-utilization-metric-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-ebs-utilization-metric-schema.json\",\n  \"title\": \"EBSUtilizationMetric\",\n  \"description\": \"<p>Describes a utilization metric of an Amazon Elastic Block Store (Amazon EBS) volume.</p> <p>Compare the utilization metric data of your resource against its projected utilization metric data to determine the performance difference between your current resource and the recommended option.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EBSMetricName\"\n        },\n        {\n          \"description\": \"<p>The name of the utilization metric.</p> <p>The following utilization metrics are available:</p> <ul> <li> <p> <code>VolumeReadOpsPerSecond</code> - The completed read operations\
  \ per second from the volume in a specified period of time.</p> <p>Unit: Count</p> </li> <li> <p> <code>VolumeWriteOpsPerSecond</code> - The completed write operations per second to the volume in a specified period of time.</p> <p>Unit: Count</p> </li> <li> <p> <code>VolumeReadBytesPerSecond</code> - The bytes read per second from the volume in a specified period of time.</p> <p>Unit: Bytes</p> </li> <li> <p> <code>VolumeWriteBytesPerSecond</code> - The bytes written to the volume in a specified period of time.</p> <p>Unit: Bytes</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"statistic\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricStatistic\"\n        },\n        {\n          \"description\": \"<p>The statistic of the utilization metric.</p> <p>The Compute Optimizer API, Command Line Interface (CLI), and SDKs return utilization metrics using only the <code>Maximum</code> statistic, which is the highest value observed during the specified period.</p>\
  \ <p>The Compute Optimizer console displays graphs for some utilization metrics using the <code>Average</code> statistic, which is the value of <code>Sum</code> / <code>SampleCount</code> during the specified period. For more information, see <a href=\\\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/viewing-recommendations.html\\\">Viewing resource recommendations</a> in the <i>Compute Optimizer User Guide</i>. You can also get averaged utilization metric data for your resources using Amazon CloudWatch. For more information, see the <a href=\\\"https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/WhatIsCloudWatch.html\\\">Amazon CloudWatch User Guide</a>.</p>\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricValue\"\n        },\n        {\n          \"description\": \"The value of the utilization metric.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-ebs-utilization-metric-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: EBSUtilizationMetric
---
