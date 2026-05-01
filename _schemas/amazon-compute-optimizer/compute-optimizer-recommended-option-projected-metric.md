---
description: <p>Describes a projected utilization metric of a recommendation option.</p> <note> <p>The <code>Cpu</code> and <code>Memory</code> metrics are the only projected utilization metrics returned when you run the <a>GetEC2RecommendationProjectedMetrics</a> action. Additionally, the <code>Memory</code> metric is returned only for resources that have the unified CloudWatch agent installed on them. For more information, see <a href="https://docs.aws.amazon.com/compute-optimizer/latest/ug/metrics.html#cw-agent">Enabling Memory Utilization with the CloudWatch Agent</a>.</p> </note>
layout: schema
name: RecommendedOptionProjectedMetric
properties_list:
- description: ''
  name: recommendedInstanceType
  type: object
- description: ''
  name: rank
  type: object
- description: ''
  name: projectedMetrics
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-recommended-option-projected-metric-schema.json
slug: compute-optimizer-recommended-option-projected-metric
source_filename: compute-optimizer-recommended-option-projected-metric-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-recommended-option-projected-metric-schema.json\",\n  \"title\": \"RecommendedOptionProjectedMetric\",\n  \"description\": \"<p>Describes a projected utilization metric of a recommendation option.</p> <note> <p>The <code>Cpu</code> and <code>Memory</code> metrics are the only projected utilization metrics returned when you run the <a>GetEC2RecommendationProjectedMetrics</a> action. Additionally, the <code>Memory</code> metric is returned only for resources that have the unified CloudWatch agent installed on them. For more information, see <a href=\\\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/metrics.html#cw-agent\\\">Enabling Memory Utilization with the CloudWatch Agent</a>.</p> </note>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"recommendedInstanceType\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecommendedInstanceType\"\n        },\n        {\n          \"description\": \"The recommended instance type.\"\n        }\n      ]\n    },\n    \"rank\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Rank\"\n        },\n        {\n          \"description\": \"<p>The rank of the recommendation option projected metric.</p> <p>The top recommendation option is ranked as <code>1</code>.</p> <p>The projected metric rank correlates to the recommendation option rank. For example, the projected metric ranked as <code>1</code> is related to the recommendation option that is also ranked as <code>1</code> in the same response.</p>\"\n        }\n      ]\n    },\n    \"projectedMetrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectedMetrics\"\n        },\n        {\n          \"description\": \"An array of objects that describe a projected utilization\
  \ metric.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-recommended-option-projected-metric-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: RecommendedOptionProjectedMetric
---
