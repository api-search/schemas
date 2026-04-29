---
description: Aggregated statistics about a measure affected by an anomaly.
layout: schema
name: ItemizedMetricStats
properties_list:
- description: ''
  name: MetricName
  type: object
- description: ''
  name: OccurrenceCount
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-itemized-metric-stats-schema.json
slug: amazon-lookout-for-metrics-itemized-metric-stats
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-itemized-metric-stats-schema.json\",\n  \"title\": \"ItemizedMetricStats\",\n  \"description\": \"Aggregated statistics about a measure affected by an anomaly.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MetricName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColumnName\"\n        },\n        {\n          \"description\": \"The name of the measure.\"\n        }\n      ]\n    },\n    \"OccurrenceCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of times that the measure appears.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-itemized-metric-stats-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: ItemizedMetricStats
---
