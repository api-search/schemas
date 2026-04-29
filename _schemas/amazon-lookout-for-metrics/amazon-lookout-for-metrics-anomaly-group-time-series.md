---
description: An anomalous metric in an anomaly group.
layout: schema
name: AnomalyGroupTimeSeries
properties_list:
- description: ''
  name: AnomalyGroupId
  type: object
- description: ''
  name: TimeSeriesId
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-anomaly-group-time-series-schema.json
slug: amazon-lookout-for-metrics-anomaly-group-time-series
source_filename: amazon-lookout-for-metrics-anomaly-group-time-series-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-anomaly-group-time-series-schema.json\",\n  \"title\": \"AnomalyGroupTimeSeries\",\n  \"description\": \"An anomalous metric in an anomaly group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnomalyGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UUID\"\n        },\n        {\n          \"description\": \"The ID of the anomaly group.\"\n        }\n      ]\n    },\n    \"TimeSeriesId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeSeriesId\"\n        },\n        {\n          \"description\": \"The ID of the metric.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AnomalyGroupId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-anomaly-group-time-series-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: AnomalyGroupTimeSeries
---
