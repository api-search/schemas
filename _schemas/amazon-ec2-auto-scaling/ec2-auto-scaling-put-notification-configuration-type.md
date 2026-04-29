---
description: PutNotificationConfigurationType schema from Auto Scaling
layout: schema
name: PutNotificationConfigurationType
properties_list:
- description: ''
  name: AutoScalingGroupName
  type: object
- description: ''
  name: TopicARN
  type: object
- description: ''
  name: NotificationTypes
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-put-notification-configuration-type-schema.json
slug: ec2-auto-scaling-put-notification-configuration-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-put-notification-configuration-type-schema.json\",\n  \"title\": \"PutNotificationConfigurationType\",\n  \"description\": \"PutNotificationConfigurationType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"TopicARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Amazon SNS topic.\"\n        }\n      ]\n    },\n    \"NotificationTypes\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/AutoScalingNotificationTypes\"\n        },\n        {\n          \"description\": \"The type of event that causes the notification to be sent. To query the notification types supported by Amazon EC2 Auto Scaling, call the <a>DescribeAutoScalingNotificationTypes</a> API.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AutoScalingGroupName\",\n    \"TopicARN\",\n    \"NotificationTypes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-put-notification-configuration-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: PutNotificationConfigurationType
---
