---
description: Describes a recommendation option for an Auto Scaling group.
layout: schema
name: AutoScalingGroupRecommendationOption
properties_list:
- description: ''
  name: configuration
  type: object
- description: ''
  name: projectedUtilizationMetrics
  type: object
- description: ''
  name: performanceRisk
  type: object
- description: ''
  name: rank
  type: object
- description: ''
  name: savingsOpportunity
  type: object
- description: ''
  name: migrationEffort
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-auto-scaling-group-recommendation-option-schema.json
slug: compute-optimizer-auto-scaling-group-recommendation-option
source_filename: compute-optimizer-auto-scaling-group-recommendation-option-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-auto-scaling-group-recommendation-option-schema.json\",\n  \"title\": \"AutoScalingGroupRecommendationOption\",\n  \"description\": \"Describes a recommendation option for an Auto Scaling group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupConfiguration\"\n        },\n        {\n          \"description\": \"An array of objects that describe an Auto Scaling group configuration.\"\n        }\n      ]\n    },\n    \"projectedUtilizationMetrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectedUtilizationMetrics\"\n        },\n        {\n          \"description\": \"<p>An array of objects that describe the projected utilization\
  \ metrics of the Auto Scaling group recommendation option.</p> <note> <p>The <code>Cpu</code> and <code>Memory</code> metrics are the only projected utilization metrics returned. Additionally, the <code>Memory</code> metric is returned only for resources that have the unified CloudWatch agent installed on them. For more information, see <a href=\\\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/metrics.html#cw-agent\\\">Enabling Memory Utilization with the CloudWatch Agent</a>.</p> </note>\"\n        }\n      ]\n    },\n    \"performanceRisk\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PerformanceRisk\"\n        },\n        {\n          \"description\": \"<p>The performance risk of the Auto Scaling group configuration recommendation.</p> <p>Performance risk indicates the likelihood of the recommended instance type not meeting the resource needs of your workload. Compute Optimizer calculates an individual performance risk score for each specification\
  \ of the recommended instance, including CPU, memory, EBS throughput, EBS IOPS, disk throughput, disk IOPS, network throughput, and network PPS. The performance risk of the recommended instance is calculated as the maximum performance risk score across the analyzed resource specifications.</p> <p>The value ranges from <code>0</code> - <code>4</code>, with <code>0</code> meaning that the recommended resource is predicted to always provide enough hardware capability. The higher the performance risk is, the more likely you should validate whether the recommendation will meet the performance requirements of your workload before migrating your resource.</p>\"\n        }\n      ]\n    },\n    \"rank\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Rank\"\n        },\n        {\n          \"description\": \"<p>The rank of the Auto Scaling group recommendation option.</p> <p>The top recommendation option is ranked as <code>1</code>.</p>\"\n        }\n      ]\n  \
  \  },\n    \"savingsOpportunity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SavingsOpportunity\"\n        },\n        {\n          \"description\": \"An object that describes the savings opportunity for the Auto Scaling group recommendation option. Savings opportunity includes the estimated monthly savings amount and percentage.\"\n        }\n      ]\n    },\n    \"migrationEffort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MigrationEffort\"\n        },\n        {\n          \"description\": \"<p>The level of effort required to migrate from the current instance type to the recommended instance type.</p> <p>For example, the migration effort is <code>Low</code> if Amazon EMR is the inferred workload type and an Amazon Web Services Graviton instance type is recommended. The migration effort is <code>Medium</code> if a workload type couldn't be inferred but an Amazon Web Services Graviton instance type is recommended.\
  \ The migration effort is <code>VeryLow</code> if both the current and recommended instance types are of the same CPU architecture.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-auto-scaling-group-recommendation-option-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: AutoScalingGroupRecommendationOption
---
