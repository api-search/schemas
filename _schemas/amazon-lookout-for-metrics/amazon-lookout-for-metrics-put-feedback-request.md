---
description: PutFeedbackRequest schema from Amazon Lookout for Metrics API
layout: schema
name: PutFeedbackRequest
properties_list:
- description: ''
  name: AnomalyDetectorArn
  type: object
- description: ''
  name: AnomalyGroupTimeSeriesFeedback
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-put-feedback-request-schema.json
slug: amazon-lookout-for-metrics-put-feedback-request
source_filename: amazon-lookout-for-metrics-put-feedback-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-put-feedback-request-schema.json\",\n  \"title\": \"PutFeedbackRequest\",\n  \"description\": \"PutFeedbackRequest schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnomalyDetectorArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the anomaly detector.\"\n        }\n      ]\n    },\n    \"AnomalyGroupTimeSeriesFeedback\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyGroupTimeSeriesFeedback\"\n        },\n        {\n          \"description\": \"Feedback for an anomalous metric.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AnomalyDetectorArn\"\
  ,\n    \"AnomalyGroupTimeSeriesFeedback\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-put-feedback-request-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: PutFeedbackRequest
---
