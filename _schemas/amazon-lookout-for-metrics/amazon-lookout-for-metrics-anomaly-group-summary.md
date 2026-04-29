---
description: Details about a group of anomalous metrics.
layout: schema
name: AnomalyGroupSummary
properties_list:
- description: ''
  name: StartTime
  type: object
- description: ''
  name: EndTime
  type: object
- description: ''
  name: AnomalyGroupId
  type: object
- description: ''
  name: AnomalyGroupScore
  type: object
- description: ''
  name: PrimaryMetricName
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-anomaly-group-summary-schema.json
slug: amazon-lookout-for-metrics-anomaly-group-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-anomaly-group-summary-schema.json\",\n  \"title\": \"AnomalyGroupSummary\",\n  \"description\": \"Details about a group of anomalous metrics.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestampString\"\n        },\n        {\n          \"description\": \"The start time for the group.\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestampString\"\n        },\n        {\n          \"description\": \"The end time for the group.\"\n        }\n      ]\n    },\n    \"AnomalyGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UUID\"\n        },\n        {\n\
  \          \"description\": \"The ID of the anomaly group.\"\n        }\n      ]\n    },\n    \"AnomalyGroupScore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Score\"\n        },\n        {\n          \"description\": \"The severity score of the group.\"\n        }\n      ]\n    },\n    \"PrimaryMetricName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricName\"\n        },\n        {\n          \"description\": \"The name of the primary affected measure for the group.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-anomaly-group-summary-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: AnomalyGroupSummary
---
