---
description: Represents a CloudWatch metric alarm
layout: schema
name: Alarm
properties_list:
- description: The name of the alarm
  name: alarmName
  type: string
- description: The ARN of the alarm
  name: alarmArn
  type: string
- description: The description of the alarm
  name: alarmDescription
  type: string
- description: The state value for the alarm
  name: stateValue
  type: string
- description: An explanation for the alarm state
  name: stateReason
  type: string
- description: The time stamp of the last update to the state
  name: stateUpdatedTimestamp
  type: string
- description: The name of the metric associated with the alarm
  name: metricName
  type: string
- description: The namespace of the metric associated with the alarm
  name: namespace
  type: string
- description: The statistic for the metric associated with the alarm
  name: statistic
  type: string
- description: The dimensions for the metric associated with the alarm
  name: dimensions
  type: array
- description: The period in seconds over which the statistic is applied
  name: period
  type: integer
- description: The number of periods over which data is compared to the threshold
  name: evaluationPeriods
  type: integer
- description: The value to compare with the specified statistic
  name: threshold
  type: number
- description: The arithmetic operation to use when comparing the statistic and threshold
  name: comparisonOperator
  type: string
- description: How missing data points are treated
  name: treatMissingData
  type: string
- description: Whether actions are executed during alarm state changes
  name: actionsEnabled
  type: boolean
- description: The actions to execute when the alarm transitions to ALARM state
  name: alarmActions
  type: array
- description: The actions to execute when the alarm transitions to OK state
  name: okActions
  type: array
- description: The actions to execute when the alarm transitions to INSUFFICIENT_DATA state
  name: insufficientDataActions
  type: array
provider_name: Amazon CloudWatch
provider_slug: amazon-cloudwatch
schema_file: json-schema/cloudwatch-alarm-schema.json
slug: cloudwatch-alarm
source_filename: cloudwatch-alarm-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudwatch/refs/heads/main/json-schema/cloudwatch-alarm-schema.json\",\n  \"title\": \"Alarm\",\n  \"description\": \"Represents a CloudWatch metric alarm\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"alarmName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the alarm\"\n    },\n    \"alarmArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the alarm\"\n    },\n    \"alarmDescription\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the alarm\"\n    },\n    \"stateValue\": {\n      \"type\": \"string\",\n      \"description\": \"The state value for the alarm\",\n      \"enum\": [\n        \"OK\",\n        \"ALARM\",\n        \"INSUFFICIENT_DATA\"\n      ]\n    },\n    \"stateReason\": {\n      \"type\": \"string\",\n      \"description\": \"An explanation\
  \ for the alarm state\"\n    },\n    \"stateUpdatedTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time stamp of the last update to the state\"\n    },\n    \"metricName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the metric associated with the alarm\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace of the metric associated with the alarm\"\n    },\n    \"statistic\": {\n      \"type\": \"string\",\n      \"description\": \"The statistic for the metric associated with the alarm\"\n    },\n    \"dimensions\": {\n      \"type\": \"array\",\n      \"description\": \"The dimensions for the metric associated with the alarm\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"type\": \"string\"\n          }\n        }\n\
  \      }\n    },\n    \"period\": {\n      \"type\": \"integer\",\n      \"description\": \"The period in seconds over which the statistic is applied\"\n    },\n    \"evaluationPeriods\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of periods over which data is compared to the threshold\"\n    },\n    \"threshold\": {\n      \"type\": \"number\",\n      \"description\": \"The value to compare with the specified statistic\"\n    },\n    \"comparisonOperator\": {\n      \"type\": \"string\",\n      \"description\": \"The arithmetic operation to use when comparing the statistic and threshold\"\n    },\n    \"treatMissingData\": {\n      \"type\": \"string\",\n      \"description\": \"How missing data points are treated\"\n    },\n    \"actionsEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether actions are executed during alarm state changes\"\n    },\n    \"alarmActions\": {\n      \"type\": \"array\",\n      \"description\": \"The actions\
  \ to execute when the alarm transitions to ALARM state\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"okActions\": {\n      \"type\": \"array\",\n      \"description\": \"The actions to execute when the alarm transitions to OK state\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"insufficientDataActions\": {\n      \"type\": \"array\",\n      \"description\": \"The actions to execute when the alarm transitions to INSUFFICIENT_DATA state\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudwatch/refs/heads/main/json-schema/cloudwatch-alarm-schema.json
tags:
- AWS
- CloudWatch
- Monitoring
- Observability
- Metrics
- Logs
title: Alarm
---
