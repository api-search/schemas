---
description: PutScalingPolicyType schema from Auto Scaling
layout: schema
name: PutScalingPolicyType
properties_list:
- description: ''
  name: AutoScalingGroupName
  type: object
- description: ''
  name: PolicyName
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
  name: MetricAggregationType
  type: object
- description: ''
  name: StepAdjustments
  type: object
- description: ''
  name: EstimatedInstanceWarmup
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
schema_file: json-schema/ec2-auto-scaling-put-scaling-policy-type-schema.json
slug: ec2-auto-scaling-put-scaling-policy-type
source_filename: ec2-auto-scaling-put-scaling-policy-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-put-scaling-policy-type-schema.json\",\n  \"title\": \"PutScalingPolicyType\",\n  \"description\": \"PutScalingPolicyType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"PolicyName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the policy.\"\n        }\n      ]\n    },\n    \"PolicyType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen64\"\n\
  \        },\n        {\n          \"description\": \"<p>One of the following policy types: </p> <ul> <li> <p> <code>TargetTrackingScaling</code> </p> </li> <li> <p> <code>StepScaling</code> </p> </li> <li> <p> <code>SimpleScaling</code> (default)</p> </li> <li> <p> <code>PredictiveScaling</code> </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"AdjustmentType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"<p>Specifies how the scaling adjustment is interpreted (for example, an absolute number or a percentage). The valid values are <code>ChangeInCapacity</code>, <code>ExactCapacity</code>, and <code>PercentChangeInCapacity</code>.</p> <p>Required if the policy type is <code>StepScaling</code> or <code>SimpleScaling</code>. For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/as-scaling-simple-step.html#as-scaling-adjustment\\\">Scaling adjustment\
  \ types</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"MinAdjustmentStep\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MinAdjustmentStep\"\n        },\n        {\n          \"description\": \"Available for backward compatibility. Use <code>MinAdjustmentMagnitude</code> instead.\"\n        }\n      ]\n    },\n    \"MinAdjustmentMagnitude\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MinAdjustmentMagnitude\"\n        },\n        {\n          \"description\": \"<p>The minimum value to scale by when the adjustment type is <code>PercentChangeInCapacity</code>. For example, suppose that you create a step scaling policy to scale out an Auto Scaling group by 25 percent and you specify a <code>MinAdjustmentMagnitude</code> of 2. If the group has 4 instances and the scaling policy is performed, 25 percent of 4 is 1. However, because you specified a <code>MinAdjustmentMagnitude</code>\
  \ of 2, Amazon EC2 Auto Scaling scales out the group by 2 instances.</p> <p>Valid only if the policy type is <code>StepScaling</code> or <code>SimpleScaling</code>. For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/as-scaling-simple-step.html#as-scaling-adjustment\\\">Scaling adjustment types</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p> <note> <p>Some Auto Scaling groups use instance weights. In this case, set the <code>MinAdjustmentMagnitude</code> to a value that is at least as large as your largest instance weight.</p> </note>\"\n        }\n      ]\n    },\n    \"ScalingAdjustment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyIncrement\"\n        },\n        {\n          \"description\": \"<p>The amount by which to scale, based on the specified adjustment type. A positive value adds to the current capacity while a negative number removes from the current capacity. For exact capacity, you must\
  \ specify a positive value.</p> <p>Required if the policy type is <code>SimpleScaling</code>. (Not used with any other policy type.) </p>\"\n        }\n      ]\n    },\n    \"Cooldown\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Cooldown\"\n        },\n        {\n          \"description\": \"<p>A cooldown period, in seconds, that applies to a specific simple scaling policy. When a cooldown period is specified here, it overrides the default cooldown.</p> <p>Valid only if the policy type is <code>SimpleScaling</code>. For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/Cooldown.html\\\">Scaling cooldowns for Amazon EC2 Auto Scaling</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p> <p>Default: None</p>\"\n        }\n      ]\n    },\n    \"MetricAggregationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen32\"\n        },\n        {\n          \"description\"\
  : \"<p>The aggregation type for the CloudWatch metrics. The valid values are <code>Minimum</code>, <code>Maximum</code>, and <code>Average</code>. If the aggregation type is null, the value is treated as <code>Average</code>.</p> <p>Valid only if the policy type is <code>StepScaling</code>.</p>\"\n        }\n      ]\n    },\n    \"StepAdjustments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StepAdjustments\"\n        },\n        {\n          \"description\": \"<p>A set of adjustments that enable you to scale based on the size of the alarm breach.</p> <p>Required if the policy type is <code>StepScaling</code>. (Not used with any other policy type.) </p>\"\n        }\n      ]\n    },\n    \"EstimatedInstanceWarmup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EstimatedInstanceWarmup\"\n        },\n        {\n          \"description\": \"<p> <i>Not needed if the default instance warmup is defined for the group.</i> </p>\
  \ <p>The estimated time, in seconds, until a newly launched instance can contribute to the CloudWatch metrics. This warm-up period applies to instances launched due to a specific target tracking or step scaling policy. When a warm-up period is specified here, it overrides the default instance warmup.</p> <p>Valid only if the policy type is <code>TargetTrackingScaling</code> or <code>StepScaling</code>.</p> <note> <p>The default is to use the value for the default instance warmup defined for the group. If default instance warmup is null, then <code>EstimatedInstanceWarmup</code> falls back to the value of default cooldown.</p> </note>\"\n        }\n      ]\n    },\n    \"TargetTrackingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetTrackingConfiguration\"\n        },\n        {\n          \"description\": \"<p>A target tracking scaling policy. Provides support for predefined or custom metrics.</p> <p>The following predefined metrics are\
  \ available:</p> <ul> <li> <p> <code>ASGAverageCPUUtilization</code> </p> </li> <li> <p> <code>ASGAverageNetworkIn</code> </p> </li> <li> <p> <code>ASGAverageNetworkOut</code> </p> </li> <li> <p> <code>ALBRequestCountPerTarget</code> </p> </li> </ul> <p>If you specify <code>ALBRequestCountPerTarget</code> for the metric, you must specify the <code>ResourceLabel</code> property with the <code>PredefinedMetricSpecification</code>.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/APIReference/API_TargetTrackingConfiguration.html\\\">TargetTrackingConfiguration</a> in the <i>Amazon EC2 Auto Scaling API Reference</i>.</p> <p>Required if the policy type is <code>TargetTrackingScaling</code>.</p>\"\n        }\n      ]\n    },\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScalingPolicyEnabled\"\n        },\n        {\n          \"description\": \"Indicates whether the scaling policy is enabled or disabled.\
  \ The default is enabled. For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/as-enable-disable-scaling-policy.html\\\">Disabling a scaling policy for an Auto Scaling group</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.\"\n        }\n      ]\n    },\n    \"PredictiveScalingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PredictiveScalingConfiguration\"\n        },\n        {\n          \"description\": \"<p>A predictive scaling policy. Provides support for predefined and custom metrics.</p> <p>Predefined metrics include CPU utilization, network in/out, and the Application Load Balancer request count.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/APIReference/API_PredictiveScalingConfiguration.html\\\">PredictiveScalingConfiguration</a> in the <i>Amazon EC2 Auto Scaling API Reference</i>.</p> <p>Required if the policy type is <code>PredictiveScaling</code>.</p>\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AutoScalingGroupName\",\n    \"PolicyName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-put-scaling-policy-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: PutScalingPolicyType
---
