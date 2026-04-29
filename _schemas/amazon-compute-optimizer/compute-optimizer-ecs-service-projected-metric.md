---
description: <p> Describes the projected metrics of an Amazon ECS service recommendation option. </p> <p>To determine the performance difference between your current Amazon ECS service and the recommended option, compare the metric data of your service against its projected metric data.</p>
layout: schema
name: ECSServiceProjectedMetric
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: timestamps
  type: object
- description: ''
  name: upperBoundValues
  type: object
- description: ''
  name: lowerBoundValues
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-ecs-service-projected-metric-schema.json
slug: compute-optimizer-ecs-service-projected-metric
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-ecs-service-projected-metric-schema.json\",\n  \"title\": \"ECSServiceProjectedMetric\",\n  \"description\": \"<p> Describes the projected metrics of an Amazon ECS service recommendation option. </p> <p>To determine the performance difference between your current Amazon ECS service and the recommended option, compare the metric data of your service against its projected metric data.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSServiceMetricName\"\n        },\n        {\n          \"description\": \"<p> The name of the projected metric. </p> <p>The following metrics are available:</p> <ul> <li> <p> <code>Cpu</code> \\u2014 The percentage of allocated compute units that are currently\
  \ in use on the service tasks.</p> </li> <li> <p> <code>Memory</code> \\u2014 The percentage of memory that's currently in use on the service tasks.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"timestamps\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamps\"\n        },\n        {\n          \"description\": \" The timestamps of the projected metric. \"\n        }\n      ]\n    },\n    \"upperBoundValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricValues\"\n        },\n        {\n          \"description\": \" The upper bound values for the projected metric. \"\n        }\n      ]\n    },\n    \"lowerBoundValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricValues\"\n        },\n        {\n          \"description\": \" The lower bound values for the projected metric. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-ecs-service-projected-metric-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: ECSServiceProjectedMetric
---
