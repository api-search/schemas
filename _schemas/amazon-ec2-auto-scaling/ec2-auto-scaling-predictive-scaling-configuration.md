---
description: Represents a predictive scaling policy configuration to use with Amazon EC2 Auto Scaling.
layout: schema
name: PredictiveScalingConfiguration
properties_list:
- description: ''
  name: MetricSpecifications
  type: object
- description: ''
  name: Mode
  type: object
- description: ''
  name: SchedulingBufferTime
  type: object
- description: ''
  name: MaxCapacityBreachBehavior
  type: object
- description: ''
  name: MaxCapacityBuffer
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-predictive-scaling-configuration-schema.json
slug: ec2-auto-scaling-predictive-scaling-configuration
source_filename: ec2-auto-scaling-predictive-scaling-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-predictive-scaling-configuration-schema.json\",\n  \"title\": \"PredictiveScalingConfiguration\",\n  \"description\": \"Represents a predictive scaling policy configuration to use with Amazon EC2 Auto Scaling.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MetricSpecifications\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PredictiveScalingMetricSpecifications\"\n        },\n        {\n          \"description\": \"<p>This structure includes the metrics and target utilization to use for predictive scaling. </p> <p>This is an array, but we currently only support a single metric specification. That is, you can specify a target value and a single metric pair, or a target value and one scaling metric and one load metric.</p>\"\n        }\n \
  \     ]\n    },\n    \"Mode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PredictiveScalingMode\"\n        },\n        {\n          \"description\": \"The predictive scaling mode. Defaults to <code>ForecastOnly</code> if not specified.\"\n        }\n      ]\n    },\n    \"SchedulingBufferTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PredictiveScalingSchedulingBufferTime\"\n        },\n        {\n          \"description\": \"<p>The amount of time, in seconds, by which the instance launch time can be advanced. For example, the forecast says to add capacity at 10:00 AM, and you choose to pre-launch instances by 5 minutes. In that case, the instances will be launched at 9:55 AM. The intention is to give resources time to be provisioned. It can take a few minutes to launch an EC2 instance. The actual amount of time required depends on several factors, such as the size of the instance and whether there are startup scripts\
  \ to complete. </p> <p>The value must be less than the forecast interval duration of 3600 seconds (60 minutes). Defaults to 300 seconds if not specified. </p>\"\n        }\n      ]\n    },\n    \"MaxCapacityBreachBehavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PredictiveScalingMaxCapacityBreachBehavior\"\n        },\n        {\n          \"description\": \"<p>Defines the behavior that should be applied if the forecast capacity approaches or exceeds the maximum capacity of the Auto Scaling group. Defaults to <code>HonorMaxCapacity</code> if not specified.</p> <p>The following are possible values:</p> <ul> <li> <p> <code>HonorMaxCapacity</code> - Amazon EC2 Auto Scaling cannot scale out capacity higher than the maximum capacity. The maximum capacity is enforced as a hard limit. </p> </li> <li> <p> <code>IncreaseMaxCapacity</code> - Amazon EC2 Auto Scaling can scale out capacity higher than the maximum capacity when the forecast capacity is close to\
  \ or exceeds the maximum capacity. The upper limit is determined by the forecasted capacity and the value for <code>MaxCapacityBuffer</code>.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"MaxCapacityBuffer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PredictiveScalingMaxCapacityBuffer\"\n        },\n        {\n          \"description\": \"<p>The size of the capacity buffer to use when the forecast capacity is close to or exceeds the maximum capacity. The value is specified as a percentage relative to the forecast capacity. For example, if the buffer is 10, this means a 10 percent buffer, such that if the forecast capacity is 50, and the maximum capacity is 40, then the effective maximum capacity is 55.</p> <p>If set to 0, Amazon EC2 Auto Scaling may scale capacity higher than the maximum capacity to equal but not exceed forecast capacity. </p> <p>Required if the <code>MaxCapacityBreachBehavior</code> property is set to <code>IncreaseMaxCapacity</code>,\
  \ and cannot be used otherwise.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MetricSpecifications\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-predictive-scaling-configuration-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: PredictiveScalingConfiguration
---
