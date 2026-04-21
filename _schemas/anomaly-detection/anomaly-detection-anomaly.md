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
