---
description: A detected anomaly in a time series or multivariate data stream, including the affected metric, timestamp, severity score, and contextual metadata.
layout: schema
name: Anomaly
properties_list:
- description: Unique identifier for the detected anomaly.
  name: id
  type: string
- description: Name of the metric or signal in which the anomaly was detected.
  name: metric_name
  type: string
- description: ISO 8601 timestamp when the anomaly was detected.
  name: timestamp
  type: string
- description: The observed metric value at the time of the anomaly.
  name: value
  type: number
- description: The expected metric value based on historical patterns.
  name: expected_value
  type: number
- description: Normalized anomaly severity score between 0 (normal) and 1 (highly anomalous).
  name: anomaly_score
  type: number
- description: Categorical severity level of the anomaly.
  name: severity
  type: string
- description: Whether the anomaly is a spike above expected, a dip below, or bidirectional.
  name: direction
  type: string
- description: The detection algorithm that identified this anomaly.
  name: algorithm
  type: string
- description: Current status of the anomaly alert.
  name: status
  type: string
- description: Identifier of the time series or data stream this anomaly belongs to.
  name: series_id
  type: string
- description: Key-value pairs providing additional context dimensions for the anomaly (e.g., region, service, host).
  name: dimensions
  type: object
- description: List of related anomaly IDs grouped in the same root cause cluster.
  name: related_anomalies
  type: array
provider_name: Anomaly Detection
provider_slug: anomaly-detection
schema_file: json-schema/anomaly-detection-anomaly-schema.json
slug: anomaly-detection-anomaly
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/anomaly-detection/refs/heads/main/json-schema/anomaly-detection-anomaly-schema.json\",\n  \"title\": \"Anomaly\",\n  \"description\": \"A detected anomaly in a time series or multivariate data stream, including the affected metric, timestamp, severity score, and contextual metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the detected anomaly.\",\n      \"example\": \"anom-500123\"\n    },\n    \"metric_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the metric or signal in which the anomaly was detected.\",\n      \"example\": \"cpu_utilization\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the anomaly was detected.\",\n   \
  \   \"example\": \"2026-04-19T14:30:00Z\"\n    },\n    \"value\": {\n      \"type\": \"number\",\n      \"description\": \"The observed metric value at the time of the anomaly.\",\n      \"example\": 98.7\n    },\n    \"expected_value\": {\n      \"type\": \"number\",\n      \"description\": \"The expected metric value based on historical patterns.\",\n      \"example\": 62.3\n    },\n    \"anomaly_score\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 1,\n      \"description\": \"Normalized anomaly severity score between 0 (normal) and 1 (highly anomalous).\",\n      \"example\": 0.94\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\"low\", \"medium\", \"high\", \"critical\"],\n      \"description\": \"Categorical severity level of the anomaly.\",\n      \"example\": \"high\"\n    },\n    \"direction\": {\n      \"type\": \"string\",\n      \"enum\": [\"above\", \"below\", \"both\"],\n      \"description\": \"Whether the anomaly\
  \ is a spike above expected, a dip below, or bidirectional.\",\n      \"example\": \"above\"\n    },\n    \"algorithm\": {\n      \"type\": \"string\",\n      \"description\": \"The detection algorithm that identified this anomaly.\",\n      \"example\": \"SARIMA\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"resolved\", \"acknowledged\", \"suppressed\"],\n      \"description\": \"Current status of the anomaly alert.\",\n      \"example\": \"active\"\n    },\n    \"series_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the time series or data stream this anomaly belongs to.\",\n      \"example\": \"ts-prod-cluster-01\"\n    },\n    \"dimensions\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value pairs providing additional context dimensions for the anomaly (e.g., region, service, host).\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\"region\": \"\
  us-east-1\", \"host\": \"web-server-42\"}\n    },\n    \"related_anomalies\": {\n      \"type\": \"array\",\n      \"description\": \"List of related anomaly IDs grouped in the same root cause cluster.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\"id\", \"metric_name\", \"timestamp\", \"value\", \"anomaly_score\", \"severity\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/anomaly-detection/refs/heads/main/json-schema/anomaly-detection-anomaly-schema.json
tags:
- Anomaly Detection
- Artificial Intelligence
- Data Science
- Fraud Detection
- Machine Learning
- Monitoring
- Observability
- Outlier Detection
- Pattern Recognition
- Security
- Time Series
title: Anomaly
---
