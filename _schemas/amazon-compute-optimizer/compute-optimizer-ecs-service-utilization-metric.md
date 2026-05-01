---
description: <p> Describes the utilization metric of an Amazon ECS service. </p> <p>To determine the performance difference between your current Amazon ECS service and the recommended option, compare the utilization metric data of your service against its projected utilization metric data.</p>
layout: schema
name: ECSServiceUtilizationMetric
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
schema_file: json-schema/compute-optimizer-ecs-service-utilization-metric-schema.json
slug: compute-optimizer-ecs-service-utilization-metric
source_filename: compute-optimizer-ecs-service-utilization-metric-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-ecs-service-utilization-metric-schema.json\",\n  \"title\": \"ECSServiceUtilizationMetric\",\n  \"description\": \"<p> Describes the utilization metric of an Amazon ECS service. </p> <p>To determine the performance difference between your current Amazon ECS service and the recommended option, compare the utilization metric data of your service against its projected utilization metric data.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSServiceMetricName\"\n        },\n        {\n          \"description\": \"<p> The name of the utilization metric. </p> <p>The following utilization metrics are available:</p> <ul> <li> <p> <code>Cpu</code> \\u2014 The amount of CPU capacity that's\
  \ used in the service.</p> </li> <li> <p> <code>Memory</code> \\u2014 The amount of memory that's used in the service.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"statistic\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSServiceMetricStatistic\"\n        },\n        {\n          \"description\": \"<p>The statistic of the utilization metric.</p> <p>The Compute Optimizer API, Command Line Interface (CLI), and SDKs return utilization metrics using only the <code>Maximum</code> statistic, which is the highest value observed during the specified period.</p> <p>The Compute Optimizer console displays graphs for some utilization metrics using the <code>Average</code> statistic, which is the value of <code>Sum</code> / <code>SampleCount</code> during the specified period. For more information, see <a href=\\\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/viewing-recommendations.html\\\">Viewing resource recommendations</a> in the <i>Compute\
  \ Optimizer User Guide</i>. You can also get averaged utilization metric data for your resources using Amazon CloudWatch. For more information, see the <a href=\\\"https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/WhatIsCloudWatch.html\\\">Amazon CloudWatch User Guide</a>.</p>\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricValue\"\n        },\n        {\n          \"description\": \" The value of the utilization metric. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-ecs-service-utilization-metric-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: ECSServiceUtilizationMetric
---
