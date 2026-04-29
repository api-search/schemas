---
description: A named time series used as input for anomaly detection, containing an ordered sequence of timestamped metric values.
layout: schema
name: TimeSeries
properties_list:
- description: Unique identifier for the time series.
  name: id
  type: string
- description: Human-readable name for the time series.
  name: name
  type: string
- description: Description of what this time series measures.
  name: description
  type: string
- description: The metric being tracked in this series.
  name: metric
  type: string
- description: Unit of measurement for the metric values.
  name: unit
  type: string
- description: Time granularity between data points (ISO 8601 duration).
  name: granularity
  type: string
- description: The dominant seasonality pattern observed in this series.
  name: seasonality
  type: string
- description: Ordered list of timestamped data points.
  name: data_points
  type: array
- description: Timestamp when this time series was created.
  name: created_at
  type: string
- description: Dimensional metadata tags for this series.
  name: dimensions
  type: object
provider_name: Anomaly Detection
provider_slug: anomaly-detection
schema_file: json-schema/anomaly-detection-time-series-schema.json
slug: anomaly-detection-time-series
source_filename: anomaly-detection-time-series-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/anomaly-detection/refs/heads/main/json-schema/anomaly-detection-time-series-schema.json\",\n  \"title\": \"TimeSeries\",\n  \"description\": \"A named time series used as input for anomaly detection, containing an ordered sequence of timestamped metric values.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the time series.\",\n      \"example\": \"ts-prod-cluster-01\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the time series.\",\n      \"example\": \"Production Cluster CPU Utilization\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of what this time series measures.\",\n      \"example\": \"Average CPU utilization across production web cluster\
  \ nodes.\"\n    },\n    \"metric\": {\n      \"type\": \"string\",\n      \"description\": \"The metric being tracked in this series.\",\n      \"example\": \"cpu_utilization\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of measurement for the metric values.\",\n      \"example\": \"percent\"\n    },\n    \"granularity\": {\n      \"type\": \"string\",\n      \"description\": \"Time granularity between data points (ISO 8601 duration).\",\n      \"example\": \"PT1M\"\n    },\n    \"seasonality\": {\n      \"type\": \"string\",\n      \"enum\": [\"hourly\", \"daily\", \"weekly\", \"none\"],\n      \"description\": \"The dominant seasonality pattern observed in this series.\",\n      \"example\": \"daily\"\n    },\n    \"data_points\": {\n      \"type\": \"array\",\n      \"description\": \"Ordered list of timestamped data points.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DataPoint\"\n      }\n    },\n    \"created_at\": {\n      \"type\"\
  : \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when this time series was created.\",\n      \"example\": \"2026-01-01T00:00:00Z\"\n    },\n    \"dimensions\": {\n      \"type\": \"object\",\n      \"description\": \"Dimensional metadata tags for this series.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\"id\", \"name\", \"metric\"],\n  \"$defs\": {\n    \"DataPoint\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp of the data point.\",\n          \"example\": \"2026-04-19T14:00:00Z\"\n        },\n        \"value\": {\n          \"type\": \"number\",\n          \"description\": \"Metric value at this timestamp.\",\n          \"example\": 72.5\n        }\n      },\n      \"required\": [\"timestamp\", \"value\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/anomaly-detection/refs/heads/main/json-schema/anomaly-detection-time-series-schema.json
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
title: TimeSeries
---
