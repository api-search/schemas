---
description: Describes a recommendation option for an Amazon Elastic Block Store (Amazon EBS) instance.
layout: schema
name: VolumeRecommendationOption
properties_list:
- description: ''
  name: configuration
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
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-volume-recommendation-option-schema.json
slug: compute-optimizer-volume-recommendation-option
source_filename: compute-optimizer-volume-recommendation-option-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-volume-recommendation-option-schema.json\",\n  \"title\": \"VolumeRecommendationOption\",\n  \"description\": \"Describes a recommendation option for an Amazon Elastic Block Store (Amazon EBS) instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeConfiguration\"\n        },\n        {\n          \"description\": \"An array of objects that describe a volume configuration.\"\n        }\n      ]\n    },\n    \"performanceRisk\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PerformanceRisk\"\n        },\n        {\n          \"description\": \"<p>The performance risk of the volume recommendation option.</p> <p>Performance risk is the likelihood\
  \ of the recommended volume type meeting the performance requirement of your workload.</p> <p>The value ranges from <code>0</code> - <code>4</code>, with <code>0</code> meaning that the recommended resource is predicted to always provide enough hardware capability. The higher the performance risk is, the more likely you should validate whether the recommendation will meet the performance requirements of your workload before migrating your resource.</p>\"\n        }\n      ]\n    },\n    \"rank\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Rank\"\n        },\n        {\n          \"description\": \"<p>The rank of the volume recommendation option.</p> <p>The top recommendation option is ranked as <code>1</code>.</p>\"\n        }\n      ]\n    },\n    \"savingsOpportunity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SavingsOpportunity\"\n        },\n        {\n          \"description\": \"An object that describes the savings\
  \ opportunity for the EBS volume recommendation option. Savings opportunity includes the estimated monthly savings amount and percentage.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-volume-recommendation-option-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: VolumeRecommendationOption
---
