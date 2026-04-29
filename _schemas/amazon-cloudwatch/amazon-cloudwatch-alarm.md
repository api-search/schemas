---
description: Represents an Amazon CloudWatch metric alarm with its associated configuration, state, and notification actions.
layout: schema
name: Amazon CloudWatch Alarm
properties_list:
- description: The name of the alarm
  name: alarmName
  type: string
- description: The Amazon Resource Name (ARN) of the alarm
  name: alarmArn
  type: string
- description: The description for the alarm
  name: alarmDescription
  type: string
- description: The time stamp of the last update to the alarm configuration
  name: alarmConfigurationUpdatedTimestamp
  type: string
- description: Indicates whether actions should be executed during any changes to the alarm state
  name: actionsEnabled
  type: boolean
- description: The actions to execute when this alarm transitions to the ALARM state
  name: alarmActions
  type: array
- description: The actions to execute when this alarm transitions to the OK state
  name: okActions
  type: array
- description: The actions to execute when this alarm transitions to the INSUFFICIENT_DATA state
  name: insufficientDataActions
  type: array
- description: The state value for the alarm
  name: stateValue
  type: string
- description: An explanation for the alarm state in human-readable text format
  name: stateReason
  type: string
- description: An explanation for the alarm state in JSON format
  name: stateReasonData
  type: string
- description: The time stamp of the last update to the alarm state
  name: stateUpdatedTimestamp
  type: string
- description: The name of the metric associated with the alarm
  name: metricName
  type: string
- description: The namespace of the metric associated with the alarm
  name: namespace
  type: string
- description: The statistic for the metric specified in MetricName
  name: statistic
  type: string
- description: The percentile statistic for the metric specified in MetricName
  name: extendedStatistic
  type: string
- description: The dimensions for the metric specified in MetricName
  name: dimensions
  type: array
- description: The length in seconds of the evaluation period for the alarm
  name: period
  type: integer
- description: The number of periods over which data is compared to the specified threshold
  name: evaluationPeriods
  type: integer
- description: The number of data points that must be breaching to trigger the alarm
  name: datapointsToAlarm
  type: integer
- description: The value against which the specified statistic is compared
  name: threshold
  type: number
- description: The arithmetic operation to use when comparing the specified statistic and threshold
  name: comparisonOperator
  type: string
- description: Sets how this alarm is to handle missing data points
  name: treatMissingData
  type: string
- description: The unit of measure for the statistic
  name: unit
  type: string
- description: Tags associated with the alarm
  name: tags
  type: array
provider_name: Amazon CloudWatch
provider_slug: amazon-cloudwatch
schema_file: json-schema/amazon-cloudwatch-alarm-schema.json
slug: amazon-cloudwatch-alarm
source_filename: amazon-cloudwatch-alarm-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/amazon/cloudwatch/alarm.json\",\n  \"title\": \"Amazon CloudWatch Alarm\",\n  \"description\": \"Represents an Amazon CloudWatch metric alarm with its associated configuration, state, and notification actions.\",\n  \"type\": \"object\",\n  \"required\": [\"alarmName\", \"comparisonOperator\", \"evaluationPeriods\"],\n  \"properties\": {\n    \"alarmName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the alarm\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"alarmArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the alarm\",\n      \"pattern\": \"^arn:aws:cloudwatch:[a-z0-9-]+:[0-9]{12}:alarm:.+$\"\n    },\n    \"alarmDescription\": {\n      \"type\": \"string\",\n      \"description\": \"The description for the alarm\",\n      \"maxLength\": 1024\n    },\n    \"alarmConfigurationUpdatedTimestamp\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time stamp of the last update to the alarm configuration\"\n    },\n    \"actionsEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether actions should be executed during any changes to the alarm state\"\n    },\n    \"alarmActions\": {\n      \"type\": \"array\",\n      \"description\": \"The actions to execute when this alarm transitions to the ALARM state\",\n      \"items\": {\n        \"type\": \"string\",\n        \"description\": \"The ARN of an action (SNS topic, Auto Scaling policy, etc.)\"\n      },\n      \"maxItems\": 5\n    },\n    \"okActions\": {\n      \"type\": \"array\",\n      \"description\": \"The actions to execute when this alarm transitions to the OK state\",\n      \"items\": {\n        \"type\": \"string\",\n        \"description\": \"The ARN of an action\"\n      },\n      \"maxItems\": 5\n    },\n    \"insufficientDataActions\": {\n\
  \      \"type\": \"array\",\n      \"description\": \"The actions to execute when this alarm transitions to the INSUFFICIENT_DATA state\",\n      \"items\": {\n        \"type\": \"string\",\n        \"description\": \"The ARN of an action\"\n      },\n      \"maxItems\": 5\n    },\n    \"stateValue\": {\n      \"type\": \"string\",\n      \"description\": \"The state value for the alarm\",\n      \"enum\": [\"OK\", \"ALARM\", \"INSUFFICIENT_DATA\"]\n    },\n    \"stateReason\": {\n      \"type\": \"string\",\n      \"description\": \"An explanation for the alarm state in human-readable text format\",\n      \"maxLength\": 1023\n    },\n    \"stateReasonData\": {\n      \"type\": \"string\",\n      \"description\": \"An explanation for the alarm state in JSON format\"\n    },\n    \"stateUpdatedTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time stamp of the last update to the alarm state\"\n    },\n    \"metricName\": {\n   \
  \   \"type\": \"string\",\n      \"description\": \"The name of the metric associated with the alarm\",\n      \"minLength\": 1,\n      \"maxLength\": 256\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace of the metric associated with the alarm\",\n      \"minLength\": 1,\n      \"maxLength\": 256\n    },\n    \"statistic\": {\n      \"type\": \"string\",\n      \"description\": \"The statistic for the metric specified in MetricName\",\n      \"enum\": [\"SampleCount\", \"Average\", \"Sum\", \"Minimum\", \"Maximum\"]\n    },\n    \"extendedStatistic\": {\n      \"type\": \"string\",\n      \"description\": \"The percentile statistic for the metric specified in MetricName\",\n      \"pattern\": \"^p(\\\\d{1,2}(\\\\.\\\\d{0,2})?|100)$\"\n    },\n    \"dimensions\": {\n      \"type\": \"array\",\n      \"description\": \"The dimensions for the metric specified in MetricName\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Dimension\"\n \
  \     },\n      \"maxItems\": 30\n    },\n    \"period\": {\n      \"type\": \"integer\",\n      \"description\": \"The length in seconds of the evaluation period for the alarm\",\n      \"minimum\": 10\n    },\n    \"evaluationPeriods\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of periods over which data is compared to the specified threshold\",\n      \"minimum\": 1\n    },\n    \"datapointsToAlarm\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of data points that must be breaching to trigger the alarm\",\n      \"minimum\": 1\n    },\n    \"threshold\": {\n      \"type\": \"number\",\n      \"description\": \"The value against which the specified statistic is compared\"\n    },\n    \"comparisonOperator\": {\n      \"type\": \"string\",\n      \"description\": \"The arithmetic operation to use when comparing the specified statistic and threshold\",\n      \"enum\": [\n        \"GreaterThanOrEqualToThreshold\",\n        \"GreaterThanThreshold\"\
  ,\n        \"LessThanThreshold\",\n        \"LessThanOrEqualToThreshold\",\n        \"LessThanLowerOrGreaterThanUpperThreshold\",\n        \"LessThanLowerThreshold\",\n        \"GreaterThanUpperThreshold\"\n      ]\n    },\n    \"treatMissingData\": {\n      \"type\": \"string\",\n      \"description\": \"Sets how this alarm is to handle missing data points\",\n      \"enum\": [\"breaching\", \"notBreaching\", \"ignore\", \"missing\"]\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"The unit of measure for the statistic\",\n      \"enum\": [\n        \"Seconds\",\n        \"Microseconds\",\n        \"Milliseconds\",\n        \"Bytes\",\n        \"Kilobytes\",\n        \"Megabytes\",\n        \"Gigabytes\",\n        \"Terabytes\",\n        \"Bits\",\n        \"Kilobits\",\n        \"Megabits\",\n        \"Gigabits\",\n        \"Terabits\",\n        \"Percent\",\n        \"Count\",\n        \"Bytes/Second\",\n        \"Kilobytes/Second\",\n        \"Megabytes/Second\"\
  ,\n        \"Gigabytes/Second\",\n        \"Terabytes/Second\",\n        \"Bits/Second\",\n        \"Kilobits/Second\",\n        \"Megabits/Second\",\n        \"Gigabits/Second\",\n        \"Terabits/Second\",\n        \"Count/Second\",\n        \"None\"\n      ]\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags associated with the alarm\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Tag\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"Dimension\": {\n      \"type\": \"object\",\n      \"description\": \"A dimension is a name/value pair that is part of the identity of a metric\",\n      \"required\": [\"name\", \"value\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the dimension\",\n          \"minLength\": 1,\n          \"maxLength\": 256\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The value of the dimension\",\n      \
  \    \"minLength\": 1,\n          \"maxLength\": 1024\n        }\n      }\n    },\n    \"Tag\": {\n      \"type\": \"object\",\n      \"description\": \"A key-value pair associated with the alarm\",\n      \"required\": [\"key\"],\n      \"properties\": {\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"The key of the tag\",\n          \"minLength\": 1,\n          \"maxLength\": 128\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The value of the tag\",\n          \"maxLength\": 256\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudwatch/refs/heads/main/json-schema/amazon-cloudwatch-alarm-schema.json
tags:
- AWS
- CloudWatch
- Monitoring
- Observability
- Metrics
- Logs
title: Amazon CloudWatch Alarm
---
