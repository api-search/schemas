---
description: Describes a lifecycle hook. A lifecycle hook lets you create solutions that are aware of events in the Auto Scaling instance lifecycle, and then perform a custom action on instances when the corresponding lifecycle event occurs.
layout: schema
name: LifecycleHook
properties_list:
- description: ''
  name: LifecycleHookName
  type: object
- description: ''
  name: AutoScalingGroupName
  type: object
- description: ''
  name: LifecycleTransition
  type: object
- description: ''
  name: NotificationTargetARN
  type: object
- description: ''
  name: RoleARN
  type: object
- description: ''
  name: NotificationMetadata
  type: object
- description: ''
  name: HeartbeatTimeout
  type: object
- description: ''
  name: GlobalTimeout
  type: object
- description: ''
  name: DefaultResult
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-lifecycle-hook-schema.json
slug: ec2-auto-scaling-lifecycle-hook
source_filename: ec2-auto-scaling-lifecycle-hook-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-lifecycle-hook-schema.json\",\n  \"title\": \"LifecycleHook\",\n  \"description\": \"Describes a lifecycle hook. A lifecycle hook lets you create solutions that are aware of events in the Auto Scaling instance lifecycle, and then perform a custom action on instances when the corresponding lifecycle event occurs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LifecycleHookName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AsciiStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the lifecycle hook.\"\n        }\n      ]\n    },\n    \"AutoScalingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"\
  The name of the Auto Scaling group for the lifecycle hook.\"\n        }\n      ]\n    },\n    \"LifecycleTransition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LifecycleTransition\"\n        },\n        {\n          \"description\": \"<p>The lifecycle transition.</p> <p>Valid values: <code>autoscaling:EC2_INSTANCE_LAUNCHING</code> | <code>autoscaling:EC2_INSTANCE_TERMINATING</code> </p>\"\n        }\n      ]\n    },\n    \"NotificationTargetARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationTargetResourceName\"\n        },\n        {\n          \"description\": \"The ARN of the target that Amazon EC2 Auto Scaling sends notifications to when an instance is in a wait state for the lifecycle hook.\"\n        }\n      ]\n    },\n    \"RoleARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The ARN of the IAM\
  \ role that allows the Auto Scaling group to publish to the specified notification target (an Amazon SNS topic or an Amazon SQS queue).\"\n        }\n      ]\n    },\n    \"NotificationMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen1023\"\n        },\n        {\n          \"description\": \"Additional information that is included any time Amazon EC2 Auto Scaling sends a message to the notification target.\"\n        }\n      ]\n    },\n    \"HeartbeatTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HeartbeatTimeout\"\n        },\n        {\n          \"description\": \"The maximum time, in seconds, that can elapse before the lifecycle hook times out. If the lifecycle hook times out, Amazon EC2 Auto Scaling performs the action that you specified in the <code>DefaultResult</code> property.\"\n        }\n      ]\n    },\n    \"GlobalTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/GlobalTimeout\"\n        },\n        {\n          \"description\": \"The maximum time, in seconds, that an instance can remain in a wait state. The maximum is 172800 seconds (48 hours) or 100 times <code>HeartbeatTimeout</code>, whichever is smaller.\"\n        }\n      ]\n    },\n    \"DefaultResult\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LifecycleActionResult\"\n        },\n        {\n          \"description\": \"<p>The action the Auto Scaling group takes when the lifecycle hook timeout elapses or if an unexpected failure occurs.</p> <p>Valid values: <code>CONTINUE</code> | <code>ABANDON</code> </p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-lifecycle-hook-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: LifecycleHook
---
