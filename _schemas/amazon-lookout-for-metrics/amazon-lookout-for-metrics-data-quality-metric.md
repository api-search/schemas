---
description: An array that describes a data quality metric. Each <code>DataQualityMetric</code> object contains the data quality metric name, its value, a description of the metric, and the affected column.
layout: schema
name: DataQualityMetric
properties_list:
- description: ''
  name: MetricType
  type: object
- description: ''
  name: MetricDescription
  type: object
- description: ''
  name: RelatedColumnName
  type: object
- description: ''
  name: MetricValue
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-data-quality-metric-schema.json
slug: amazon-lookout-for-metrics-data-quality-metric
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-data-quality-metric-schema.json\",\n  \"title\": \"DataQualityMetric\",\n  \"description\": \"An array that describes a data quality metric. Each <code>DataQualityMetric</code> object contains the data quality metric name, its value, a description of the metric, and the affected column.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MetricType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataQualityMetricType\"\n        },\n        {\n          \"description\": \"The name of the data quality metric.\"\n        }\n      ]\n    },\n    \"MetricDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataQualityMetricDescription\"\n        },\n        {\n          \"description\": \"A description\
  \ of the data quality metric.\"\n        }\n      ]\n    },\n    \"RelatedColumnName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RelatedColumnName\"\n        },\n        {\n          \"description\": \"The column that is being monitored.\"\n        }\n      ]\n    },\n    \"MetricValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"The value of the data quality metric.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-data-quality-metric-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: DataQualityMetric
---
