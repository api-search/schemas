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
