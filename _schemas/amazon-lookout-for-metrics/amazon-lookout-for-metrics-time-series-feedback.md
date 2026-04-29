---
description: Details about feedback submitted for an anomalous metric.
layout: schema
name: TimeSeriesFeedback
properties_list:
- description: ''
  name: TimeSeriesId
  type: object
- description: ''
  name: IsAnomaly
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-time-series-feedback-schema.json
slug: amazon-lookout-for-metrics-time-series-feedback
source_filename: amazon-lookout-for-metrics-time-series-feedback-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-time-series-feedback-schema.json\",\n  \"title\": \"TimeSeriesFeedback\",\n  \"description\": \"Details about feedback submitted for an anomalous metric.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TimeSeriesId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeSeriesId\"\n        },\n        {\n          \"description\": \"The ID of the metric.\"\n        }\n      ]\n    },\n    \"IsAnomaly\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Feedback on whether the metric is a legitimate anomaly.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-time-series-feedback-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: TimeSeriesFeedback
---
