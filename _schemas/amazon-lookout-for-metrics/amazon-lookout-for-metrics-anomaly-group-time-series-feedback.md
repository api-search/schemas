---
description: Feedback for an anomalous metric.
layout: schema
name: AnomalyGroupTimeSeriesFeedback
properties_list:
- description: ''
  name: AnomalyGroupId
  type: object
- description: ''
  name: TimeSeriesId
  type: object
- description: ''
  name: IsAnomaly
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-anomaly-group-time-series-feedback-schema.json
slug: amazon-lookout-for-metrics-anomaly-group-time-series-feedback
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-anomaly-group-time-series-feedback-schema.json\",\n  \"title\": \"AnomalyGroupTimeSeriesFeedback\",\n  \"description\": \"Feedback for an anomalous metric.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnomalyGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UUID\"\n        },\n        {\n          \"description\": \"The ID of the anomaly group.\"\n        }\n      ]\n    },\n    \"TimeSeriesId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeSeriesId\"\n        },\n        {\n          \"description\": \"The ID of the metric.\"\n        }\n      ]\n    },\n    \"IsAnomaly\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n\
  \          \"description\": \"Feedback on whether the metric is a legitimate anomaly.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AnomalyGroupId\",\n    \"TimeSeriesId\",\n    \"IsAnomaly\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-anomaly-group-time-series-feedback-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: AnomalyGroupTimeSeriesFeedback
---
