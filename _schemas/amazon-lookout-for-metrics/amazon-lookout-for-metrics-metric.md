---
description: A calculation made by contrasting a measure and a dimension from your source data.
layout: schema
name: Metric
properties_list:
- description: ''
  name: MetricName
  type: object
- description: ''
  name: AggregationFunction
  type: object
- description: ''
  name: Namespace
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-metric-schema.json
slug: amazon-lookout-for-metrics-metric
source_filename: amazon-lookout-for-metrics-metric-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-metric-schema.json\",\n  \"title\": \"Metric\",\n  \"description\": \"A calculation made by contrasting a measure and a dimension from your source data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MetricName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColumnName\"\n        },\n        {\n          \"description\": \"The name of the metric.\"\n        }\n      ]\n    },\n    \"AggregationFunction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregationFunction\"\n        },\n        {\n          \"description\": \"The function with which the metric is calculated.\"\n        }\n      ]\n    },\n    \"Namespace\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Namespace\"\
  \n        },\n        {\n          \"description\": \"The namespace for the metric.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MetricName\",\n    \"AggregationFunction\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-metric-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: Metric
---
