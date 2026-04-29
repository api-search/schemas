---
description: ''
layout: schema
name: PutMetricAlarmInput
properties_list:
- description: The name for the alarm.
  name: AlarmName
  type: string
- description: The description for the alarm.
  name: AlarmDescription
  type: string
- description: Indicates whether actions should be executed during any changes to the alarm state.
  name: ActionsEnabled
  type: boolean
- description: The actions to execute when this alarm transitions to an OK state.
  name: OKActions
  type: array
- description: The actions to execute when this alarm transitions to the ALARM state.
  name: AlarmActions
  type: array
- description: The actions to execute when this alarm transitions to the INSUFFICIENT_DATA state.
  name: InsufficientDataActions
  type: array
- description: The name for the metric associated with the alarm.
  name: MetricName
  type: string
- description: The namespace for the metric associated with the alarm.
  name: Namespace
  type: string
- description: The percentile statistic for the metric specified in MetricName.
  name: ExtendedStatistic
  type: string
- description: The dimensions for the metric specified in MetricName.
  name: Dimensions
  type: array
- description: The length, in seconds, used each time the metric specified in MetricName is evaluated.
  name: Period
  type: integer
- description: The number of periods over which data is compared to the specified threshold.
  name: EvaluationPeriods
  type: integer
- description: The number of data points that must be breaching to trigger the alarm.
  name: DatapointsToAlarm
  type: integer
- description: The value against which the specified statistic is compared.
  name: Threshold
  type: number
- description: Sets how this alarm is to handle missing data points.
  name: TreatMissingData
  type: string
- description: Used only for alarms based on percentiles.
  name: EvaluateLowSampleCountPercentile
  type: string
- description: An array of MetricDataQuery structures for metric math expression alarms.
  name: Metrics
  type: array
- description: A list of key-value pairs to associate with the alarm.
  name: Tags
  type: array
- description: If this is an alarm based on an anomaly detection model, make this value match the ID of the ANOMALY_DETECTION_BAND function.
  name: ThresholdMetricId
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-put-metric-alarm-input-schema.json
slug: cloudwatch-put-metric-alarm-input
source_filename: cloudwatch-put-metric-alarm-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PutMetricAlarmInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AlarmName\": {\n      \"type\": \"string\",\n      \"description\": \"The name for the alarm.\"\n    },\n    \"AlarmDescription\": {\n      \"type\": \"string\",\n      \"description\": \"The description for the alarm.\"\n    },\n    \"ActionsEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether actions should be executed during any changes to the alarm state.\"\n    },\n    \"OKActions\": {\n      \"type\": \"array\",\n      \"description\": \"The actions to execute when this alarm transitions to an OK state.\"\n    },\n    \"AlarmActions\": {\n      \"type\": \"array\",\n      \"description\": \"The actions to execute when this alarm transitions to the ALARM state.\"\n    },\n    \"InsufficientDataActions\": {\n      \"type\": \"array\",\n      \"description\": \"The actions to execute\
  \ when this alarm transitions to the INSUFFICIENT_DATA state.\"\n    },\n    \"MetricName\": {\n      \"type\": \"string\",\n      \"description\": \"The name for the metric associated with the alarm.\"\n    },\n    \"Namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace for the metric associated with the alarm.\"\n    },\n    \"ExtendedStatistic\": {\n      \"type\": \"string\",\n      \"description\": \"The percentile statistic for the metric specified in MetricName.\"\n    },\n    \"Dimensions\": {\n      \"type\": \"array\",\n      \"description\": \"The dimensions for the metric specified in MetricName.\"\n    },\n    \"Period\": {\n      \"type\": \"integer\",\n      \"description\": \"The length, in seconds, used each time the metric specified in MetricName is evaluated.\"\n    },\n    \"EvaluationPeriods\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of periods over which data is compared to the specified threshold.\"\n   \
  \ },\n    \"DatapointsToAlarm\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of data points that must be breaching to trigger the alarm.\"\n    },\n    \"Threshold\": {\n      \"type\": \"number\",\n      \"description\": \"The value against which the specified statistic is compared.\"\n    },\n    \"TreatMissingData\": {\n      \"type\": \"string\",\n      \"description\": \"Sets how this alarm is to handle missing data points.\"\n    },\n    \"EvaluateLowSampleCountPercentile\": {\n      \"type\": \"string\",\n      \"description\": \"Used only for alarms based on percentiles.\"\n    },\n    \"Metrics\": {\n      \"type\": \"array\",\n      \"description\": \"An array of MetricDataQuery structures for metric math expression alarms.\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"description\": \"A list of key-value pairs to associate with the alarm.\"\n    },\n    \"ThresholdMetricId\": {\n      \"type\": \"string\",\n      \"description\": \"\
  If this is an alarm based on an anomaly detection model, make this value match the ID of the ANOMALY_DETECTION_BAND function.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-put-metric-alarm-input-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: PutMetricAlarmInput
---
