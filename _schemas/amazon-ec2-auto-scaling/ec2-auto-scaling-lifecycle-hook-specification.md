---
description: <p>Describes information used to specify a lifecycle hook for an Auto Scaling group.</p> <p>For more information, see <a href="https://docs.aws.amazon.com/autoscaling/ec2/userguide/lifecycle-hooks.html">Amazon EC2 Auto Scaling lifecycle hooks</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p>
layout: schema
name: LifecycleHookSpecification
properties_list:
- description: ''
  name: LifecycleHookName
  type: object
- description: ''
  name: LifecycleTransition
  type: object
- description: ''
  name: NotificationMetadata
  type: object
- description: ''
  name: HeartbeatTimeout
  type: object
- description: ''
  name: DefaultResult
  type: object
- description: ''
  name: NotificationTargetARN
  type: object
- description: ''
  name: RoleARN
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-lifecycle-hook-specification-schema.json
slug: ec2-auto-scaling-lifecycle-hook-specification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-lifecycle-hook-specification-schema.json\",\n  \"title\": \"LifecycleHookSpecification\",\n  \"description\": \"<p>Describes information used to specify a lifecycle hook for an Auto Scaling group.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/lifecycle-hooks.html\\\">Amazon EC2 Auto Scaling lifecycle hooks</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LifecycleHookName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AsciiStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the lifecycle hook.\"\n        }\n      ]\n    },\n    \"LifecycleTransition\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/LifecycleTransition\"\n        },\n        {\n          \"description\": \"<p>The lifecycle transition. For Auto Scaling groups, there are two major lifecycle transitions.</p> <ul> <li> <p>To create a lifecycle hook for scale-out events, specify <code>autoscaling:EC2_INSTANCE_LAUNCHING</code>.</p> </li> <li> <p>To create a lifecycle hook for scale-in events, specify <code>autoscaling:EC2_INSTANCE_TERMINATING</code>.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"NotificationMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen1023\"\n        },\n        {\n          \"description\": \"Additional information that you want to include any time Amazon EC2 Auto Scaling sends a message to the notification target.\"\n        }\n      ]\n    },\n    \"HeartbeatTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HeartbeatTimeout\"\n        },\n        {\n          \"description\"\
  : \"The maximum time, in seconds, that can elapse before the lifecycle hook times out. The range is from <code>30</code> to <code>7200</code> seconds. The default value is <code>3600</code> seconds (1 hour).\"\n        }\n      ]\n    },\n    \"DefaultResult\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LifecycleActionResult\"\n        },\n        {\n          \"description\": \"<p>The action the Auto Scaling group takes when the lifecycle hook timeout elapses or if an unexpected failure occurs. The default value is <code>ABANDON</code>.</p> <p>Valid values: <code>CONTINUE</code> | <code>ABANDON</code> </p>\"\n        }\n      ]\n    },\n    \"NotificationTargetARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationTargetResourceName\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the notification target that Amazon EC2 Auto Scaling sends notifications to when an instance\
  \ is in a wait state for the lifecycle hook. You can specify an Amazon SNS topic or an Amazon SQS queue.\"\n        }\n      ]\n    },\n    \"RoleARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"<p>The ARN of the IAM role that allows the Auto Scaling group to publish to the specified notification target. For information about creating this role, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/prepare-for-lifecycle-notifications.html#lifecycle-hook-notification-target\\\">Configure a notification target for a lifecycle hook</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p> <p>Valid only if the notification target is an Amazon SNS topic or an Amazon SQS queue.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LifecycleHookName\",\n    \"LifecycleTransition\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-lifecycle-hook-specification-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: LifecycleHookSpecification
---
