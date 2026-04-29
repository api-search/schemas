---
description: Schema for an Amazon CloudWatch alarm resource, representing a watch over a single CloudWatch metric or the result of a math expression based on CloudWatch metrics. The alarm triggers actions when the metric or expression value breaches a defined threshold over a specified number of evaluation periods.
layout: schema
name: Amazon CloudWatch Alarm
properties_list:
- description: The name of the alarm. This name must be unique within the Region and within the AWS account. The maximum length is 255 characters.
  name: AlarmName
  type: string
- description: The Amazon Resource Name (ARN) of the alarm, in the format arn:aws:cloudwatch:region:account-id:alarm:alarm-name.
  name: AlarmArn
  type: string
- description: The description for the alarm. Up to 1024 characters.
  name: AlarmDescription
  type: string
- description: The time stamp of the last update to the alarm configuration, in ISO 8601 format.
  name: AlarmConfigurationUpdatedTimestamp
  type: string
- description: Indicates whether actions should be executed during any changes to the alarm state. When set to false, the alarm state changes but no actions are executed.
  name: ActionsEnabled
  type: boolean
- description: The actions to execute when this alarm transitions to the OK state from any other state. Each action is specified as an ARN. A maximum of 5 actions are allowed.
  name: OKActions
  type: array
- description: The actions to execute when this alarm transitions to the ALARM state from any other state. Each action is specified as an ARN. A maximum of 5 actions are allowed.
  name: AlarmActions
  type: array
- description: The actions to execute when this alarm transitions to the INSUFFICIENT_DATA state from any other state. Each action is specified as an ARN. A maximum of 5 actions are allowed.
  name: InsufficientDataActions
  type: array
- description: The current state value for the alarm. OK indicates the metric or expression is within the defined threshold. ALARM indicates the metric or expression is outside of the defined threshold. INSUFFICIENT
  name: StateValue
  type: string
- description: An explanation for the alarm state, in text format. Provides a human-readable explanation of why the alarm is in its current state.
  name: StateReason
  type: string
- description: An explanation for the alarm state, in JSON format. Contains machine-readable data about the evaluation that led to the current alarm state.
  name: StateReasonData
  type: string
- description: The time stamp of the last update to the alarm's StateValue or StateReasonData, in ISO 8601 format.
  name: StateUpdatedTimestamp
  type: string
- description: The date and time that the alarm's StateValue most recently changed, in ISO 8601 format.
  name: StateTransitionedTimestamp
  type: string
- description: The name of the metric associated with the alarm, if this is a single-metric alarm.
  name: MetricName
  type: string
- description: The namespace of the metric associated with the alarm. Namespaces that begin with AWS/ are reserved for AWS services.
  name: Namespace
  type: string
- description: The statistic for the metric specified in MetricName, other than percentile.
  name: Statistic
  type: string
- description: The percentile statistic for the metric specified in MetricName. Specify a value between p0.0 and p100.
  name: ExtendedStatistic
  type: string
- description: The dimensions for the metric specified in MetricName. A maximum of 30 dimensions are allowed per metric.
  name: Dimensions
  type: array
- description: The length, in seconds, used each time the metric specified in MetricName is evaluated. Valid values are 10, 30, and any multiple of 60. For high-resolution metrics, the period can be 10 or 30 seconds
  name: Period
  type: integer
- description: The unit of measure for the statistic. If you do not specify Unit, CloudWatch retrieves all unit types that have been published for the metric.
  name: Unit
  type: string
- description: The number of periods over which data is compared to the specified threshold. An alarm is triggered only if enough periods breach the threshold according to DatapointsToAlarm.
  name: EvaluationPeriods
  type: integer
- description: The number of data points that must be breaching to trigger the alarm. This is used only if you are setting an M out of N alarm. The value must be less than or equal to EvaluationPeriods.
  name: DatapointsToAlarm
  type: integer
- description: The value against which the specified statistic is compared. This value is used with ComparisonOperator to determine if the alarm should transition to the ALARM state.
  name: Threshold
  type: number
- description: The arithmetic operation to use when comparing the specified statistic and threshold. The specified statistic value is used as the first operand. The anomaly-detection-specific operators are used with
  name: ComparisonOperator
  type: string
- description: Sets how this alarm is to handle missing data points. breaching treats missing data as breaching the threshold. notBreaching treats missing data as being within the threshold. ignore maintains the cur
  name: TreatMissingData
  type: string
- description: Used only for alarms based on percentile statistics. If ignore, the alarm state does not change during periods with too few data points to be statistically significant.
  name: EvaluateLowSampleCountPercentile
  type: string
- description: An array of MetricDataQuery structures indicating the metrics to be returned and the math expressions to perform. Used for metric math expression-based alarms.
  name: Metrics
  type: array
- description: If this is an alarm based on an anomaly detection model, make this value match the ID of the ANOMALY_DETECTION_BAND function.
  name: ThresholdMetricId
  type: string
- description: A list of key-value pairs to associate with the alarm. You can associate as many as 50 tags with an alarm.
  name: Tags
  type: array
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-alarm-schema.json
slug: cloudwatch-alarm
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.apis.io/cloudwatch/cloudwatch-alarm-schema.json\",\n  \"title\": \"Amazon CloudWatch Alarm\",\n  \"description\": \"Schema for an Amazon CloudWatch alarm resource, representing a watch over a single CloudWatch metric or the result of a math expression based on CloudWatch metrics. The alarm triggers actions when the metric or expression value breaches a defined threshold over a specified number of evaluation periods.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"AlarmName\",\n    \"ComparisonOperator\",\n    \"EvaluationPeriods\"\n  ],\n  \"properties\": {\n    \"AlarmName\": {\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"maxLength\": 255,\n      \"description\": \"The name of the alarm. This name must be unique within the Region and within the AWS account. The maximum length is 255 characters.\"\n    },\n    \"AlarmArn\": {\n      \"type\": \"string\"\
  ,\n      \"minLength\": 1,\n      \"maxLength\": 1600,\n      \"pattern\": \"^arn:aws[a-zA-Z-]*:cloudwatch:[a-z0-9-]+:[0-9]{12}:alarm:.+$\",\n      \"description\": \"The Amazon Resource Name (ARN) of the alarm, in the format arn:aws:cloudwatch:region:account-id:alarm:alarm-name.\"\n    },\n    \"AlarmDescription\": {\n      \"type\": \"string\",\n      \"maxLength\": 1024,\n      \"description\": \"The description for the alarm. Up to 1024 characters.\"\n    },\n    \"AlarmConfigurationUpdatedTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time stamp of the last update to the alarm configuration, in ISO 8601 format.\"\n    },\n    \"ActionsEnabled\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Indicates whether actions should be executed during any changes to the alarm state. When set to false, the alarm state changes but no actions are executed.\"\n    },\n    \"OKActions\": {\n      \"\
  type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"maxLength\": 1024,\n        \"description\": \"An ARN identifying an action to perform when the alarm transitions to the OK state. Supported resources include Amazon SNS topics, Auto Scaling policies, and Amazon EC2 actions.\"\n      },\n      \"maxItems\": 5,\n      \"description\": \"The actions to execute when this alarm transitions to the OK state from any other state. Each action is specified as an ARN. A maximum of 5 actions are allowed.\"\n    },\n    \"AlarmActions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"maxLength\": 1024,\n        \"description\": \"An ARN identifying an action to perform when the alarm transitions to the ALARM state. Supported resources include Amazon SNS topics, Auto Scaling policies, Amazon EC2 actions, and Systems Manager OpsItems.\"\n      },\n      \"maxItems\": 5,\n      \"description\": \"The actions to execute when this\
  \ alarm transitions to the ALARM state from any other state. Each action is specified as an ARN. A maximum of 5 actions are allowed.\"\n    },\n    \"InsufficientDataActions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"maxLength\": 1024,\n        \"description\": \"An ARN identifying an action to perform when the alarm transitions to the INSUFFICIENT_DATA state.\"\n      },\n      \"maxItems\": 5,\n      \"description\": \"The actions to execute when this alarm transitions to the INSUFFICIENT_DATA state from any other state. Each action is specified as an ARN. A maximum of 5 actions are allowed.\"\n    },\n    \"StateValue\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"OK\",\n        \"ALARM\",\n        \"INSUFFICIENT_DATA\"\n      ],\n      \"description\": \"The current state value for the alarm. OK indicates the metric or expression is within the defined threshold. ALARM indicates the metric or expression is outside\
  \ of the defined threshold. INSUFFICIENT_DATA indicates there is not enough data to determine the alarm state.\"\n    },\n    \"StateReason\": {\n      \"type\": \"string\",\n      \"maxLength\": 1023,\n      \"description\": \"An explanation for the alarm state, in text format. Provides a human-readable explanation of why the alarm is in its current state.\"\n    },\n    \"StateReasonData\": {\n      \"type\": \"string\",\n      \"maxLength\": 4000,\n      \"description\": \"An explanation for the alarm state, in JSON format. Contains machine-readable data about the evaluation that led to the current alarm state.\"\n    },\n    \"StateUpdatedTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time stamp of the last update to the alarm's StateValue or StateReasonData, in ISO 8601 format.\"\n    },\n    \"StateTransitionedTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date\
  \ and time that the alarm's StateValue most recently changed, in ISO 8601 format.\"\n    },\n    \"MetricName\": {\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"maxLength\": 255,\n      \"description\": \"The name of the metric associated with the alarm, if this is a single-metric alarm.\"\n    },\n    \"Namespace\": {\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"maxLength\": 255,\n      \"pattern\": \"[^:].*\",\n      \"description\": \"The namespace of the metric associated with the alarm. Namespaces that begin with AWS/ are reserved for AWS services.\"\n    },\n    \"Statistic\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SampleCount\",\n        \"Average\",\n        \"Sum\",\n        \"Minimum\",\n        \"Maximum\"\n      ],\n      \"description\": \"The statistic for the metric specified in MetricName, other than percentile.\"\n    },\n    \"ExtendedStatistic\": {\n      \"type\": \"string\",\n      \"pattern\": \"^p(\\\\d{1,2}(\\\
  \\.\\\\d{0,2})?|100)$\",\n      \"description\": \"The percentile statistic for the metric specified in MetricName. Specify a value between p0.0 and p100.\"\n    },\n    \"Dimensions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Dimension\"\n      },\n      \"maxItems\": 30,\n      \"description\": \"The dimensions for the metric specified in MetricName. A maximum of 30 dimensions are allowed per metric.\"\n    },\n    \"Period\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"The length, in seconds, used each time the metric specified in MetricName is evaluated. Valid values are 10, 30, and any multiple of 60. For high-resolution metrics, the period can be 10 or 30 seconds.\"\n    },\n    \"Unit\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Seconds\",\n        \"Microseconds\",\n        \"Milliseconds\",\n        \"Bytes\",\n        \"Kilobytes\",\n        \"Megabytes\",\n        \"Gigabytes\",\n \
  \       \"Terabytes\",\n        \"Bits\",\n        \"Kilobits\",\n        \"Megabits\",\n        \"Gigabits\",\n        \"Terabits\",\n        \"Percent\",\n        \"Count\",\n        \"Bytes/Second\",\n        \"Kilobytes/Second\",\n        \"Megabytes/Second\",\n        \"Gigabytes/Second\",\n        \"Terabytes/Second\",\n        \"Bits/Second\",\n        \"Kilobits/Second\",\n        \"Megabits/Second\",\n        \"Gigabits/Second\",\n        \"Terabits/Second\",\n        \"Count/Second\",\n        \"None\"\n      ],\n      \"description\": \"The unit of measure for the statistic. If you do not specify Unit, CloudWatch retrieves all unit types that have been published for the metric.\"\n    },\n    \"EvaluationPeriods\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"The number of periods over which data is compared to the specified threshold. An alarm is triggered only if enough periods breach the threshold according to DatapointsToAlarm.\"\n   \
  \ },\n    \"DatapointsToAlarm\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"The number of data points that must be breaching to trigger the alarm. This is used only if you are setting an M out of N alarm. The value must be less than or equal to EvaluationPeriods.\"\n    },\n    \"Threshold\": {\n      \"type\": \"number\",\n      \"description\": \"The value against which the specified statistic is compared. This value is used with ComparisonOperator to determine if the alarm should transition to the ALARM state.\"\n    },\n    \"ComparisonOperator\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"GreaterThanOrEqualToThreshold\",\n        \"GreaterThanThreshold\",\n        \"LessThanThreshold\",\n        \"LessThanOrEqualToThreshold\",\n        \"LessThanLowerOrGreaterThanUpperThreshold\",\n        \"LessThanLowerThreshold\",\n        \"GreaterThanUpperThreshold\"\n      ],\n      \"description\": \"The arithmetic operation to use when\
  \ comparing the specified statistic and threshold. The specified statistic value is used as the first operand. The anomaly-detection-specific operators are used with anomaly detection models.\"\n    },\n    \"TreatMissingData\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"breaching\",\n        \"notBreaching\",\n        \"ignore\",\n        \"missing\"\n      ],\n      \"default\": \"missing\",\n      \"description\": \"Sets how this alarm is to handle missing data points. breaching treats missing data as breaching the threshold. notBreaching treats missing data as being within the threshold. ignore maintains the current alarm state. missing is the default and treats the missing data point as missing.\"\n    },\n    \"EvaluateLowSampleCountPercentile\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"evaluate\",\n        \"ignore\"\n      ],\n      \"description\": \"Used only for alarms based on percentile statistics. If ignore, the alarm state does not change\
  \ during periods with too few data points to be statistically significant.\"\n    },\n    \"Metrics\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/MetricDataQuery\"\n      },\n      \"description\": \"An array of MetricDataQuery structures indicating the metrics to be returned and the math expressions to perform. Used for metric math expression-based alarms.\"\n    },\n    \"ThresholdMetricId\": {\n      \"type\": \"string\",\n      \"description\": \"If this is an alarm based on an anomaly detection model, make this value match the ID of the ANOMALY_DETECTION_BAND function.\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Tag\"\n      },\n      \"description\": \"A list of key-value pairs to associate with the alarm. You can associate as many as 50 tags with an alarm.\"\n    }\n  },\n  \"$defs\": {\n    \"Dimension\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"Name\",\n    \
  \    \"Value\"\n      ],\n      \"properties\": {\n        \"Name\": {\n          \"type\": \"string\",\n          \"minLength\": 1,\n          \"maxLength\": 255,\n          \"description\": \"The name of the dimension. Dimension names must contain only ASCII characters, must include at least one non-whitespace character, and cannot start with a colon (:).\"\n        },\n        \"Value\": {\n          \"type\": \"string\",\n          \"minLength\": 1,\n          \"maxLength\": 1024,\n          \"description\": \"The value of the dimension. Dimension values must contain only ASCII characters and must include at least one non-whitespace character.\"\n        }\n      },\n      \"description\": \"A dimension is a name/value pair that is part of the identity of a metric. Because dimensions are part of the unique identifier for a metric, whenever you add a unique name/value pair to one of your metrics, you are creating a new variation of that metric.\"\n    },\n    \"MetricDataQuery\": {\n\
  \      \"type\": \"object\",\n      \"required\": [\n        \"Id\"\n      ],\n      \"properties\": {\n        \"Id\": {\n          \"type\": \"string\",\n          \"minLength\": 1,\n          \"maxLength\": 255,\n          \"pattern\": \"^[a-z][a-zA-Z0-9_]*$\",\n          \"description\": \"A short name used to tie this object to the results in the response. Must be unique within a single request and must start with a lowercase letter.\"\n        },\n        \"MetricStat\": {\n          \"$ref\": \"#/$defs/MetricStat\"\n        },\n        \"Expression\": {\n          \"type\": \"string\",\n          \"minLength\": 1,\n          \"maxLength\": 2048,\n          \"description\": \"This field can contain a Metrics Insights query, or a metric math expression to be performed on the returned data.\"\n        },\n        \"Label\": {\n          \"type\": \"string\",\n          \"description\": \"A human-readable label for this metric or expression. This is especially useful when this is an\
  \ expression, so that you know what the value represents.\"\n        },\n        \"ReturnData\": {\n          \"type\": \"boolean\",\n          \"default\": true,\n          \"description\": \"When used in GetMetricData, indicates whether to return the timestamps and raw data values of this metric. When used in PutMetricAlarm, determines whether this expression result is used as the alarm value.\"\n        },\n        \"Period\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"The granularity, in seconds, of the returned data points. For metrics with regular resolution, a period can be as short as one minute (60 seconds). For high-resolution metrics, a period can be as short as 1 second.\"\n        },\n        \"AccountId\": {\n          \"type\": \"string\",\n          \"minLength\": 1,\n          \"maxLength\": 255,\n          \"description\": \"The ID of the account where the metrics are located, if this is a cross-account alarm.\"\n    \
  \    }\n      },\n      \"description\": \"This structure is used in both GetMetricData and PutMetricAlarm. It defines which metric to return data for, or which math expression to evaluate.\"\n    },\n    \"MetricStat\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"Metric\",\n        \"Period\",\n        \"Stat\"\n      ],\n      \"properties\": {\n        \"Metric\": {\n          \"$ref\": \"#/$defs/Metric\"\n        },\n        \"Period\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"The granularity, in seconds, of the returned data points.\"\n        },\n        \"Stat\": {\n          \"type\": \"string\",\n          \"description\": \"The statistic to return. It can include any CloudWatch statistic or extended statistic.\"\n        },\n        \"Unit\": {\n          \"type\": \"string\",\n          \"description\": \"When you are using a Put operation, this defines what unit you want to use when storing the metric.\"\
  \n        }\n      },\n      \"description\": \"This structure defines the metric to be returned, along with the statistics, period, and units.\"\n    },\n    \"Metric\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Namespace\": {\n          \"type\": \"string\",\n          \"minLength\": 1,\n          \"maxLength\": 255,\n          \"description\": \"The namespace of the metric.\"\n        },\n        \"MetricName\": {\n          \"type\": \"string\",\n          \"minLength\": 1,\n          \"maxLength\": 255,\n          \"description\": \"The name of the metric.\"\n        },\n        \"Dimensions\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Dimension\"\n          },\n          \"maxItems\": 30,\n          \"description\": \"The dimensions for the metric.\"\n        }\n      },\n      \"description\": \"Represents a specific metric.\"\n    },\n    \"Tag\": {\n      \"type\": \"object\",\n      \"required\": [\n  \
  \      \"Key\",\n        \"Value\"\n      ],\n      \"properties\": {\n        \"Key\": {\n          \"type\": \"string\",\n          \"minLength\": 1,\n          \"maxLength\": 128,\n          \"description\": \"A string that you can use to assign a value. The combination of tag keys and values can help you organize and categorize your resources.\"\n        },\n        \"Value\": {\n          \"type\": \"string\",\n          \"minLength\": 0,\n          \"maxLength\": 256,\n          \"description\": \"The value for the specified tag key.\"\n        }\n      },\n      \"description\": \"A key-value pair associated with a CloudWatch resource.\"\n    }\n  },\n  \"examples\": [\n    {\n      \"AlarmName\": \"HighCPUAlarm\",\n      \"AlarmDescription\": \"Alarm when CPU exceeds 80%\",\n      \"ActionsEnabled\": true,\n      \"AlarmActions\": [\n        \"arn:aws:sns:us-east-1:123456789012:my-topic\"\n      ],\n      \"MetricName\": \"CPUUtilization\",\n      \"Namespace\": \"AWS/EC2\",\n\
  \      \"Statistic\": \"Average\",\n      \"Dimensions\": [\n        {\n          \"Name\": \"InstanceId\",\n          \"Value\": \"i-0123456789abcdef0\"\n        }\n      ],\n      \"Period\": 300,\n      \"EvaluationPeriods\": 3,\n      \"DatapointsToAlarm\": 2,\n      \"Threshold\": 80.0,\n      \"ComparisonOperator\": \"GreaterThanThreshold\",\n      \"TreatMissingData\": \"missing\"\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-alarm-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: Amazon CloudWatch Alarm
---
