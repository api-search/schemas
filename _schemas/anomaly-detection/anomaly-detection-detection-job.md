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
