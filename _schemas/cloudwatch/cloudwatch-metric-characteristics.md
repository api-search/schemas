---
description: This object includes parameters that you can use to provide information to CloudWatch to help it build more accurate anomaly detection models.
layout: schema
name: MetricCharacteristics
properties_list:
- description: Set this parameter to true if values for this metric consistently include spikes that should not be considered to be anomalies.
  name: PeriodicSpikes
  type: boolean
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-metric-characteristics-schema.json
slug: cloudwatch-metric-characteristics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricCharacteristics\",\n  \"type\": \"object\",\n  \"description\": \"This object includes parameters that you can use to provide information to CloudWatch to help it build more accurate anomaly detection models.\",\n  \"properties\": {\n    \"PeriodicSpikes\": {\n      \"type\": \"boolean\",\n      \"description\": \"Set this parameter to true if values for this metric consistently include spikes that should not be considered to be anomalies.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-metric-characteristics-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: MetricCharacteristics
---
