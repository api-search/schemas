---
description: GetEC2RecommendationProjectedMetricsRequest schema
layout: schema
name: GetEC2RecommendationProjectedMetricsRequest
properties_list:
- description: ''
  name: instanceArn
  type: object
- description: ''
  name: stat
  type: object
- description: ''
  name: period
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: endTime
  type: object
- description: ''
  name: recommendationPreferences
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-get-ec2-recommendation-projected-metrics-request-schema.json
slug: compute-optimizer-get-ec2-recommendation-projected-metrics-request
source_filename: compute-optimizer-get-ec2-recommendation-projected-metrics-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-ec2-recommendation-projected-metrics-request-schema.json\",\n  \"title\": \"GetEC2RecommendationProjectedMetricsRequest\",\n  \"description\": \"GetEC2RecommendationProjectedMetricsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instanceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the instances for which to return recommendation projected metrics.\"\n        }\n      ]\n    },\n    \"stat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricStatistic\"\n        },\n        {\n          \"description\": \"The statistic of the projected metrics.\"\n        }\n      ]\n    },\n    \"\
  period\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Period\"\n        },\n        {\n          \"description\": \"The granularity, in seconds, of the projected metrics data points.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp of the first projected metrics data point to return.\"\n        }\n      ]\n    },\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp of the last projected metrics data point to return.\"\n        }\n      ]\n    },\n    \"recommendationPreferences\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecommendationPreferences\"\n        },\n        {\n          \"description\": \"An object to specify the preferences for the\
  \ Amazon EC2 recommendation projected metrics to return in the response.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"instanceArn\",\n    \"stat\",\n    \"period\",\n    \"startTime\",\n    \"endTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-ec2-recommendation-projected-metrics-request-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: GetEC2RecommendationProjectedMetricsRequest
---
