---
description: The status of an anomaly detector run.
layout: schema
name: ExecutionStatus
properties_list:
- description: ''
  name: Timestamp
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: FailureReason
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-execution-status-schema.json
slug: amazon-lookout-for-metrics-execution-status
source_filename: amazon-lookout-for-metrics-execution-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-execution-status-schema.json\",\n  \"title\": \"ExecutionStatus\",\n  \"description\": \"The status of an anomaly detector run.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Timestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestampString\"\n        },\n        {\n          \"description\": \"The run's timestamp.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyDetectionTaskStatus\"\n        },\n        {\n          \"description\": \"The run's status.\"\n        }\n      ]\n    },\n    \"FailureReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyDetectionTaskStatusMessage\"\n        },\n    \
  \    {\n          \"description\": \"The reason that the run failed, if applicable.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-execution-status-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: ExecutionStatus
---
