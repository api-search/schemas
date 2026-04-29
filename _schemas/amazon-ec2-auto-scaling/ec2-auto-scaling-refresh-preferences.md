---
description: Describes the preferences for an instance refresh.
layout: schema
name: RefreshPreferences
properties_list:
- description: ''
  name: MinHealthyPercentage
  type: object
- description: ''
  name: InstanceWarmup
  type: object
- description: ''
  name: CheckpointPercentages
  type: object
- description: ''
  name: CheckpointDelay
  type: object
- description: ''
  name: SkipMatching
  type: object
- description: ''
  name: AutoRollback
  type: object
- description: ''
  name: ScaleInProtectedInstances
  type: object
- description: ''
  name: StandbyInstances
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-refresh-preferences-schema.json
slug: ec2-auto-scaling-refresh-preferences
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-refresh-preferences-schema.json\",\n  \"title\": \"RefreshPreferences\",\n  \"description\": \"Describes the preferences for an instance refresh.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MinHealthyPercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntPercent\"\n        },\n        {\n          \"description\": \"<p>The amount of capacity in the Auto Scaling group that must pass your group's health checks to allow the operation to continue. The value is expressed as a percentage of the desired capacity of the Auto Scaling group (rounded up to the nearest integer). The default is <code>90</code>.</p> <p>Setting the minimum healthy percentage to 100 percent limits the rate of replacement to one instance at a time. In contrast,\
  \ setting it to 0 percent has the effect of replacing all instances at the same time. </p>\"\n        }\n      ]\n    },\n    \"InstanceWarmup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RefreshInstanceWarmup\"\n        },\n        {\n          \"description\": \"<p>A time period, in seconds, during which an instance refresh waits before moving on to replacing the next instance after a new instance enters the <code>InService</code> state.</p> <p>This property is not required for normal usage. Instead, use the <code>DefaultInstanceWarmup</code> property of the Auto Scaling group. The <code>InstanceWarmup</code> and <code>DefaultInstanceWarmup</code> properties work the same way. Only specify this property if you must override the <code>DefaultInstanceWarmup</code> property. </p> <p> If you do not specify this property, the instance warmup by default is the value of the <code>DefaultInstanceWarmup</code> property, if defined (which is recommended in all\
  \ cases), or the <code>HealthCheckGracePeriod</code> property otherwise.</p>\"\n        }\n      ]\n    },\n    \"CheckpointPercentages\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CheckpointPercentages\"\n        },\n        {\n          \"description\": \"<p>(Optional) Threshold values for each checkpoint in ascending order. Each number must be unique. To replace all instances in the Auto Scaling group, the last number in the array must be <code>100</code>.</p> <p>For usage examples, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/asg-adding-checkpoints-instance-refresh.html\\\">Adding checkpoints to an instance refresh</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"CheckpointDelay\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CheckpointDelay\"\n        },\n        {\n          \"description\": \"(Optional) The amount of time, in seconds, to wait\
  \ after a checkpoint before continuing. This property is optional, but if you specify a value for it, you must also specify a value for <code>CheckpointPercentages</code>. If you specify a value for <code>CheckpointPercentages</code> and not for <code>CheckpointDelay</code>, the <code>CheckpointDelay</code> defaults to <code>3600</code> (1 hour). \"\n        }\n      ]\n    },\n    \"SkipMatching\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SkipMatching\"\n        },\n        {\n          \"description\": \"<p>(Optional) Indicates whether skip matching is enabled. If enabled (<code>true</code>), then Amazon EC2 Auto Scaling skips replacing instances that match the desired configuration. If no desired configuration is specified, then it skips replacing instances that have the same launch template and instance types that the Auto Scaling group was using before the start of the instance refresh. The default is <code>false</code>.</p> <p>For more information,\
  \ see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/asg-instance-refresh-skip-matching.html\\\">Use an instance refresh with skip matching</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"AutoRollback\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoRollback\"\n        },\n        {\n          \"description\": \"<p>(Optional) Indicates whether to roll back the Auto Scaling group to its previous configuration if the instance refresh fails. The default is <code>false</code>.</p> <p>A rollback is not supported in the following situations: </p> <ul> <li> <p>There is no desired configuration specified for the instance refresh.</p> </li> <li> <p>The Auto Scaling group has a launch template that uses an Amazon Web Services Systems Manager parameter instead of an AMI ID for the <code>ImageId</code> property.</p> </li> <li> <p>The Auto Scaling group uses the launch template's <code>$Latest</code>\
  \ or <code>$Default</code> version.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"ScaleInProtectedInstances\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScaleInProtectedInstances\"\n        },\n        {\n          \"description\": \"<p>Choose the behavior that you want Amazon EC2 Auto Scaling to use if instances protected from scale in are found. </p> <p>The following lists the valid values:</p> <dl> <dt>Refresh</dt> <dd> <p>Amazon EC2 Auto Scaling replaces instances that are protected from scale in.</p> </dd> <dt>Ignore</dt> <dd> <p>Amazon EC2 Auto Scaling ignores instances that are protected from scale in and continues to replace instances that are not protected.</p> </dd> <dt>Wait (default)</dt> <dd> <p>Amazon EC2 Auto Scaling waits one hour for you to remove scale-in protection. Otherwise, the instance refresh will fail.</p> </dd> </dl>\"\n        }\n      ]\n    },\n    \"StandbyInstances\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/StandbyInstances\"\n        },\n        {\n          \"description\": \"<p>Choose the behavior that you want Amazon EC2 Auto Scaling to use if instances in <code>Standby</code> state are found.</p> <p>The following lists the valid values:</p> <dl> <dt>Terminate</dt> <dd> <p>Amazon EC2 Auto Scaling terminates instances that are in <code>Standby</code>.</p> </dd> <dt>Ignore</dt> <dd> <p>Amazon EC2 Auto Scaling ignores instances that are in <code>Standby</code> and continues to replace instances that are in the <code>InService</code> state.</p> </dd> <dt>Wait (default)</dt> <dd> <p>Amazon EC2 Auto Scaling waits one hour for you to return the instances to service. Otherwise, the instance refresh will fail.</p> </dd> </dl>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-refresh-preferences-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: RefreshPreferences
---
