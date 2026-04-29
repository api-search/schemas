---
description: Configuration for an anomaly detection job that analyzes one or more time series using a specified algorithm and detection settings.
layout: schema
name: DetectionJob
properties_list:
- description: Unique identifier for the detection job.
  name: id
  type: string
- description: Human-readable name for the detection job.
  name: name
  type: string
- description: Description of what this detection job monitors and why.
  name: description
  type: string
- description: Current operational status of the detection job.
  name: status
  type: string
- description: The anomaly detection algorithm used by this job.
  name: algorithm
  type: string
- description: Detection mode — batch retrospective, streaming real-time, or multivariate correlation-based.
  name: mode
  type: string
- description: Sensitivity level controlling the anomaly detection threshold. Higher values detect more subtle anomalies.
  name: sensitivity
  type: number
- description: Seasonality pattern used for baseline modeling.
  name: seasonality
  type: string
- description: List of time series identifiers analyzed by this job.
  name: series_ids
  type: array
- description: Timestamp when the job was created.
  name: created_at
  type: string
- description: Timestamp when the job was last modified.
  name: modified_at
  type: string
provider_name: Anomaly Detection
provider_slug: anomaly-detection
schema_file: json-schema/anomaly-detection-detection-job-schema.json
slug: anomaly-detection-detection-job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/anomaly-detection/refs/heads/main/json-schema/anomaly-detection-detection-job-schema.json\",\n  \"title\": \"DetectionJob\",\n  \"description\": \"Configuration for an anomaly detection job that analyzes one or more time series using a specified algorithm and detection settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the detection job.\",\n      \"example\": \"job-500456\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the detection job.\",\n      \"example\": \"Production API Latency Anomaly Detector\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of what this detection job monitors and why.\",\n      \"example\": \"Monitors API p99 latency\
  \ for anomalies using daily seasonality.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"pending\", \"running\", \"paused\", \"closed\", \"failed\"],\n      \"description\": \"Current operational status of the detection job.\",\n      \"example\": \"running\"\n    },\n    \"algorithm\": {\n      \"type\": \"string\",\n      \"enum\": [\"basic\", \"agile\", \"robust\", \"iforest\", \"lof\", \"ocsvm\", \"autoencoder\", \"sr-cnn\", \"sarima\", \"graph-attention-network\"],\n      \"description\": \"The anomaly detection algorithm used by this job.\",\n      \"example\": \"agile\"\n    },\n    \"mode\": {\n      \"type\": \"string\",\n      \"enum\": [\"batch\", \"streaming\", \"multivariate\"],\n      \"description\": \"Detection mode — batch retrospective, streaming real-time, or multivariate correlation-based.\",\n      \"example\": \"streaming\"\n    },\n    \"sensitivity\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 10,\n  \
  \    \"description\": \"Sensitivity level controlling the anomaly detection threshold. Higher values detect more subtle anomalies.\",\n      \"example\": 3\n    },\n    \"seasonality\": {\n      \"type\": \"string\",\n      \"enum\": [\"hourly\", \"daily\", \"weekly\", \"none\", \"auto\"],\n      \"description\": \"Seasonality pattern used for baseline modeling.\",\n      \"example\": \"daily\"\n    },\n    \"series_ids\": {\n      \"type\": \"array\",\n      \"description\": \"List of time series identifiers analyzed by this job.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\"ts-api-latency-p99\", \"ts-api-error-rate\"]\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the job was created.\",\n      \"example\": \"2026-04-01T00:00:00Z\"\n    },\n    \"modified_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp\
  \ when the job was last modified.\",\n      \"example\": \"2026-04-19T00:00:00Z\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"status\", \"algorithm\", \"mode\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/anomaly-detection/refs/heads/main/json-schema/anomaly-detection-detection-job-schema.json
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
title: DetectionJob
---
