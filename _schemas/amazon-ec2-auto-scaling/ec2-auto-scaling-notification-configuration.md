---
description: Describes a notification.
layout: schema
name: NotificationConfiguration
properties_list:
- description: ''
  name: AutoScalingGroupName
  type: object
- description: ''
  name: TopicARN
  type: object
- description: ''
  name: NotificationType
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-notification-configuration-schema.json
slug: ec2-auto-scaling-notification-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-notification-configuration-schema.json\",\n  \"title\": \"NotificationConfiguration\",\n  \"description\": \"Describes a notification.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"TopicARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Amazon SNS topic.\"\n        }\n      ]\n    },\n    \"NotificationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\
  \n        },\n        {\n          \"description\": \"<p>One of the following event notification types:</p> <ul> <li> <p> <code>autoscaling:EC2_INSTANCE_LAUNCH</code> </p> </li> <li> <p> <code>autoscaling:EC2_INSTANCE_LAUNCH_ERROR</code> </p> </li> <li> <p> <code>autoscaling:EC2_INSTANCE_TERMINATE</code> </p> </li> <li> <p> <code>autoscaling:EC2_INSTANCE_TERMINATE_ERROR</code> </p> </li> <li> <p> <code>autoscaling:TEST_NOTIFICATION</code> </p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-notification-configuration-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: NotificationConfiguration
---
