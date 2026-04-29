---
description: GetECSServiceRecommendationProjectedMetricsRequest schema
layout: schema
name: GetECSServiceRecommendationProjectedMetricsRequest
properties_list:
- description: ''
  name: serviceArn
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
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-get-ecs-service-recommendation-projected-metrics-request-schema.json
slug: compute-optimizer-get-ecs-service-recommendation-projected-metrics-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-ecs-service-recommendation-projected-metrics-request-schema.json\",\n  \"title\": \"GetECSServiceRecommendationProjectedMetricsRequest\",\n  \"description\": \"GetECSServiceRecommendationProjectedMetricsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceArn\"\n        },\n        {\n          \"description\": \"<p> The ARN that identifies the Amazon ECS service. </p> <p> The following is the format of the ARN: </p> <p> <code>arn:aws:ecs:region:aws_account_id:service/cluster-name/service-name</code> </p>\"\n        }\n      ]\n    },\n    \"stat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricStatistic\"\n        },\n \
  \       {\n          \"description\": \" The statistic of the projected metrics. \"\n        }\n      ]\n    },\n    \"period\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Period\"\n        },\n        {\n          \"description\": \" The granularity, in seconds, of the projected metrics data points. \"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The timestamp of the first projected metrics data point to return. \"\n        }\n      ]\n    },\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The timestamp of the last projected metrics data point to return. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"serviceArn\",\n    \"stat\",\n    \"period\",\n    \"startTime\",\n    \"endTime\"\n\
  \  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-ecs-service-recommendation-projected-metrics-request-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: GetECSServiceRecommendationProjectedMetricsRequest
---
