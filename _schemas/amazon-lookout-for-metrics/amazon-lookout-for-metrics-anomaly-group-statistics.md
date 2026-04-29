---
description: Aggregated statistics for a group of anomalous metrics.
layout: schema
name: AnomalyGroupStatistics
properties_list:
- description: ''
  name: EvaluationStartDate
  type: object
- description: ''
  name: TotalCount
  type: object
- description: ''
  name: ItemizedMetricStatsList
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-anomaly-group-statistics-schema.json
slug: amazon-lookout-for-metrics-anomaly-group-statistics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-anomaly-group-statistics-schema.json\",\n  \"title\": \"AnomalyGroupStatistics\",\n  \"description\": \"Aggregated statistics for a group of anomalous metrics.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EvaluationStartDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestampString\"\n        },\n        {\n          \"description\": \"The start of the time range that was searched.\"\n        }\n      ]\n    },\n    \"TotalCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of groups found.\"\n        }\n      ]\n    },\n    \"ItemizedMetricStatsList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ItemizedMetricStatsList\"\
  \n        },\n        {\n          \"description\": \"Statistics for individual metrics within the group.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-anomaly-group-statistics-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: AnomalyGroupStatistics
---
