---
description: Aggregated details about the data quality metrics collected for the <code>AnomalyDetectorArn</code> provided in the <a>GetDataQualityMetrics</a> object.
layout: schema
name: AnomalyDetectorDataQualityMetric
properties_list:
- description: ''
  name: StartTimestamp
  type: object
- description: ''
  name: MetricSetDataQualityMetricList
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-anomaly-detector-data-quality-metric-schema.json
slug: amazon-lookout-for-metrics-anomaly-detector-data-quality-metric
source_filename: amazon-lookout-for-metrics-anomaly-detector-data-quality-metric-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-anomaly-detector-data-quality-metric-schema.json\",\n  \"title\": \"AnomalyDetectorDataQualityMetric\",\n  \"description\": \"Aggregated details about the data quality metrics collected for the <code>AnomalyDetectorArn</code> provided in the <a>GetDataQualityMetrics</a> object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StartTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The start time for the data quality metrics collection.\"\n        }\n      ]\n    },\n    \"MetricSetDataQualityMetricList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricSetDataQualityMetricList\"\n        },\n        {\n          \"description\"\
  : \"An array of <code>DataQualityMetricList</code> objects. Each object in the array contains information about a data quality metric.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-anomaly-detector-data-quality-metric-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: AnomalyDetectorDataQualityMetric
---
