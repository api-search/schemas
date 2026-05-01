---
description: <p> Describes the projected utilization metrics of an Amazon ECS service recommendation option. </p> <p>To determine the performance difference between your current Amazon ECS service and the recommended option, compare the utilization metric data of your service against its projected utilization metric data.</p>
layout: schema
name: ECSServiceProjectedUtilizationMetric
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: statistic
  type: object
- description: ''
  name: lowerBoundValue
  type: object
- description: ''
  name: upperBoundValue
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-ecs-service-projected-utilization-metric-schema.json
slug: compute-optimizer-ecs-service-projected-utilization-metric
source_filename: compute-optimizer-ecs-service-projected-utilization-metric-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-ecs-service-projected-utilization-metric-schema.json\",\n  \"title\": \"ECSServiceProjectedUtilizationMetric\",\n  \"description\": \"<p> Describes the projected utilization metrics of an Amazon ECS service recommendation option. </p> <p>To determine the performance difference between your current Amazon ECS service and the recommended option, compare the utilization metric data of your service against its projected utilization metric data.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSServiceMetricName\"\n        },\n        {\n          \"description\": \"<p> The name of the projected utilization metric. </p> <p>The following utilization metrics are available:</p> <ul> <li>\
  \ <p> <code>Cpu</code> \\u2014 The percentage of allocated compute units that are currently in use on the service tasks.</p> </li> <li> <p> <code>Memory</code> \\u2014 The percentage of memory that's currently in use on the service tasks.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"statistic\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSServiceMetricStatistic\"\n        },\n        {\n          \"description\": \"<p>The statistic of the projected utilization metric.</p> <p>The Compute Optimizer API, Command Line Interface (CLI), and SDKs return utilization metrics using only the <code>Maximum</code> statistic, which is the highest value observed during the specified period.</p> <p>The Compute Optimizer console displays graphs for some utilization metrics using the <code>Average</code> statistic, which is the value of <code>Sum</code> / <code>SampleCount</code> during the specified period. For more information, see <a href=\\\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/viewing-recommendations.html\\\
  \">Viewing resource recommendations</a> in the <i>Compute Optimizer User Guide</i>. You can also get averaged utilization metric data for your resources using Amazon CloudWatch. For more information, see the <a href=\\\"https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/WhatIsCloudWatch.html\\\">Amazon CloudWatch User Guide</a>.</p>\"\n        }\n      ]\n    },\n    \"lowerBoundValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LowerBoundValue\"\n        },\n        {\n          \"description\": \" The lower bound values for the projected utilization metrics. \"\n        }\n      ]\n    },\n    \"upperBoundValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpperBoundValue\"\n        },\n        {\n          \"description\": \" The upper bound values for the projected utilization metrics. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-ecs-service-projected-utilization-metric-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: ECSServiceProjectedUtilizationMetric
---
