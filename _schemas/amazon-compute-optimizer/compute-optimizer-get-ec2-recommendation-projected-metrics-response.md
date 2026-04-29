---
description: GetEC2RecommendationProjectedMetricsResponse schema
layout: schema
name: GetEC2RecommendationProjectedMetricsResponse
properties_list:
- description: ''
  name: recommendedOptionProjectedMetrics
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-get-ec2-recommendation-projected-metrics-response-schema.json
slug: compute-optimizer-get-ec2-recommendation-projected-metrics-response
source_filename: compute-optimizer-get-ec2-recommendation-projected-metrics-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-ec2-recommendation-projected-metrics-response-schema.json\",\n  \"title\": \"GetEC2RecommendationProjectedMetricsResponse\",\n  \"description\": \"GetEC2RecommendationProjectedMetricsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"recommendedOptionProjectedMetrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecommendedOptionProjectedMetrics\"\n        },\n        {\n          \"description\": \"An array of objects that describes projected metrics.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-ec2-recommendation-projected-metrics-response-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: GetEC2RecommendationProjectedMetricsResponse
---
