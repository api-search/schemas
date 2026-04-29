---
description: <p>Describes a projected utilization metric of a recommendation option, such as an Amazon EC2 instance. This represents the projected utilization of a recommendation option had you used that resource during the analyzed period.</p> <p>Compare the utilization metric data of your resource against its projected utilization metric data to determine the performance difference between your current resource and the recommended option.</p> <note> <p>The <code>Cpu</code> and <code>Memory</code> metrics are the only projected utilization metrics returned when you run the <a>GetEC2RecommendationProjectedMetrics</a> action. Additionally, the <code>Memory</code> metric is returned only for resources that have the unified CloudWatch agent installed on them. For more information, see <a href="https://docs.aws.amazon.com/compute-optimizer/latest/ug/metrics.html#cw-agent">Enabling Memory Utilization with the CloudWatch Agent</a>.</p> </note>
layout: schema
name: ProjectedMetric
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: timestamps
  type: object
- description: ''
  name: values
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-projected-metric-schema.json
slug: compute-optimizer-projected-metric
source_filename: compute-optimizer-projected-metric-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-projected-metric-schema.json\",\n  \"title\": \"ProjectedMetric\",\n  \"description\": \"<p>Describes a projected utilization metric of a recommendation option, such as an Amazon EC2 instance. This represents the projected utilization of a recommendation option had you used that resource during the analyzed period.</p> <p>Compare the utilization metric data of your resource against its projected utilization metric data to determine the performance difference between your current resource and the recommended option.</p> <note> <p>The <code>Cpu</code> and <code>Memory</code> metrics are the only projected utilization metrics returned when you run the <a>GetEC2RecommendationProjectedMetrics</a> action. Additionally, the <code>Memory</code> metric is returned only for resources that\
  \ have the unified CloudWatch agent installed on them. For more information, see <a href=\\\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/metrics.html#cw-agent\\\">Enabling Memory Utilization with the CloudWatch Agent</a>.</p> </note>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricName\"\n        },\n        {\n          \"description\": \"<p>The name of the projected utilization metric.</p> <p>The following projected utilization metrics are returned:</p> <ul> <li> <p> <code>Cpu</code> - The projected percentage of allocated EC2 compute units that would be in use on the recommendation option had you used that resource during the analyzed period. This metric identifies the processing power required to run an application on the recommendation option.</p> <p>Depending on the instance type, tools in your operating system can show a lower percentage than CloudWatch when the instance\
  \ is not allocated a full processor core.</p> <p>Units: Percent</p> </li> <li> <p> <code>Memory</code> - The percentage of memory that would be in use on the recommendation option had you used that resource during the analyzed period. This metric identifies the amount of memory required to run an application on the recommendation option.</p> <p>Units: Percent</p> <note> <p>The <code>Memory</code> metric is returned only for resources that have the unified CloudWatch agent installed on them. For more information, see <a href=\\\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/metrics.html#cw-agent\\\">Enabling Memory Utilization with the CloudWatch Agent</a>.</p> </note> </li> </ul>\"\n        }\n      ]\n    },\n    \"timestamps\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamps\"\n        },\n        {\n          \"description\": \"The timestamps of the projected utilization metric.\"\n        }\n      ]\n    },\n    \"values\": {\n    \
  \  \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricValues\"\n        },\n        {\n          \"description\": \"The values of the projected utilization metrics.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-projected-metric-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: ProjectedMetric
---
