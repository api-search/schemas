---
description: Describes a scaling policy.
layout: schema
name: ScalingPolicy
properties_list:
- description: ''
  name: AutoScalingGroupName
  type: object
- description: ''
  name: PolicyName
  type: object
- description: ''
  name: PolicyARN
  type: object
- description: ''
  name: PolicyType
  type: object
- description: ''
  name: AdjustmentType
  type: object
- description: ''
  name: MinAdjustmentStep
  type: object
- description: ''
  name: MinAdjustmentMagnitude
  type: object
- description: ''
  name: ScalingAdjustment
  type: object
- description: ''
  name: Cooldown
  type: object
- description: ''
  name: StepAdjustments
  type: object
- description: ''
  name: MetricAggregationType
  type: object
- description: ''
  name: EstimatedInstanceWarmup
  type: object
- description: ''
  name: Alarms
  type: object
- description: ''
  name: TargetTrackingConfiguration
  type: object
- description: ''
  name: Enabled
  type: object
- description: ''
  name: PredictiveScalingConfiguration
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-scaling-policy-schema.json
slug: ec2-auto-scaling-scaling-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-scaling-policy-schema.json\",\n  \"title\": \"ScalingPolicy\",\n  \"description\": \"Describes a scaling policy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"PolicyName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the scaling policy.\"\n        }\n      ]\n    },\n    \"PolicyARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n       \
  \   \"description\": \"The Amazon Resource Name (ARN) of the policy.\"\n        }\n      ]\n    },\n    \"PolicyType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen64\"\n        },\n        {\n          \"description\": \"<p>One of the following policy types: </p> <ul> <li> <p> <code>TargetTrackingScaling</code> </p> </li> <li> <p> <code>StepScaling</code> </p> </li> <li> <p> <code>SimpleScaling</code> (default)</p> </li> <li> <p> <code>PredictiveScaling</code> </p> </li> </ul> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/as-scaling-target-tracking.html\\\">Target tracking scaling policies</a> and <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/as-scaling-simple-step.html\\\">Step and simple scaling policies</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"AdjustmentType\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"Specifies how the scaling adjustment is interpreted (for example, an absolute number or a percentage). The valid values are <code>ChangeInCapacity</code>, <code>ExactCapacity</code>, and <code>PercentChangeInCapacity</code>.\"\n        }\n      ]\n    },\n    \"MinAdjustmentStep\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MinAdjustmentStep\"\n        },\n        {\n          \"description\": \"Available for backward compatibility. Use <code>MinAdjustmentMagnitude</code> instead.\"\n        }\n      ]\n    },\n    \"MinAdjustmentMagnitude\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MinAdjustmentMagnitude\"\n        },\n        {\n          \"description\": \"The minimum value to scale by when the adjustment type is <code>PercentChangeInCapacity</code>. \"\n        }\n      ]\n    },\n    \"ScalingAdjustment\": {\n    \
  \  \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyIncrement\"\n        },\n        {\n          \"description\": \"The amount by which to scale, based on the specified adjustment type. A positive value adds to the current capacity while a negative number removes from the current capacity.\"\n        }\n      ]\n    },\n    \"Cooldown\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Cooldown\"\n        },\n        {\n          \"description\": \"The duration of the policy's cooldown period, in seconds.\"\n        }\n      ]\n    },\n    \"StepAdjustments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StepAdjustments\"\n        },\n        {\n          \"description\": \"A set of adjustments that enable you to scale based on the size of the alarm breach.\"\n        }\n      ]\n    },\n    \"MetricAggregationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen32\"\
  \n        },\n        {\n          \"description\": \"The aggregation type for the CloudWatch metrics. The valid values are <code>Minimum</code>, <code>Maximum</code>, and <code>Average</code>.\"\n        }\n      ]\n    },\n    \"EstimatedInstanceWarmup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EstimatedInstanceWarmup\"\n        },\n        {\n          \"description\": \"The estimated time, in seconds, until a newly launched instance can contribute to the CloudWatch metrics.\"\n        }\n      ]\n    },\n    \"Alarms\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Alarms\"\n        },\n        {\n          \"description\": \"The CloudWatch alarms related to the policy.\"\n        }\n      ]\n    },\n    \"TargetTrackingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetTrackingConfiguration\"\n        },\n        {\n          \"description\": \"A target tracking scaling\
  \ policy.\"\n        }\n      ]\n    },\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScalingPolicyEnabled\"\n        },\n        {\n          \"description\": \"Indicates whether the policy is enabled (<code>true</code>) or disabled (<code>false</code>).\"\n        }\n      ]\n    },\n    \"PredictiveScalingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PredictiveScalingConfiguration\"\n        },\n        {\n          \"description\": \"A predictive scaling policy.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-scaling-policy-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: ScalingPolicy
---
