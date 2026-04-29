---
description: GetFeedbackResponse schema from Amazon Lookout for Metrics API
layout: schema
name: GetFeedbackResponse
properties_list:
- description: ''
  name: AnomalyGroupTimeSeriesFeedback
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-get-feedback-response-schema.json
slug: amazon-lookout-for-metrics-get-feedback-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-get-feedback-response-schema.json\",\n  \"title\": \"GetFeedbackResponse\",\n  \"description\": \"GetFeedbackResponse schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnomalyGroupTimeSeriesFeedback\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeSeriesFeedbackList\"\n        },\n        {\n          \"description\": \"Feedback for an anomalous metric.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The pagination token that's included if more results are available.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-get-feedback-response-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: GetFeedbackResponse
---
