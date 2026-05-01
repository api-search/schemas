---
description: An array of <code>DataQualityMetric</code> objects that describes one or more data quality metrics.
layout: schema
name: MetricSetDataQualityMetric
properties_list:
- description: ''
  name: MetricSetArn
  type: object
- description: ''
  name: DataQualityMetricList
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-metric-set-data-quality-metric-schema.json
slug: amazon-lookout-for-metrics-metric-set-data-quality-metric
source_filename: amazon-lookout-for-metrics-metric-set-data-quality-metric-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-metric-set-data-quality-metric-schema.json\",\n  \"title\": \"MetricSetDataQualityMetric\",\n  \"description\": \"An array of <code>DataQualityMetric</code> objects that describes one or more data quality metrics.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MetricSetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the data quality metric array.\"\n        }\n      ]\n    },\n    \"DataQualityMetricList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataQualityMetricList\"\n        },\n        {\n          \"description\": \"The array of data quality metrics contained in the data quality metric set.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-metric-set-data-quality-metric-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: MetricSetDataQualityMetric
---
