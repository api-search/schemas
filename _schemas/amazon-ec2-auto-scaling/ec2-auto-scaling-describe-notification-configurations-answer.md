---
description: DescribeNotificationConfigurationsAnswer schema from Auto Scaling
layout: schema
name: DescribeNotificationConfigurationsAnswer
properties_list:
- description: ''
  name: NotificationConfigurations
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-describe-notification-configurations-answer-schema.json
slug: ec2-auto-scaling-describe-notification-configurations-answer
source_filename: ec2-auto-scaling-describe-notification-configurations-answer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-notification-configurations-answer-schema.json\",\n  \"title\": \"DescribeNotificationConfigurationsAnswer\",\n  \"description\": \"DescribeNotificationConfigurationsAnswer schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NotificationConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationConfigurations\"\n        },\n        {\n          \"description\": \"The notification configurations.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlString\"\n        },\n        {\n          \"description\": \"A string that indicates that the response contains more items than can be returned in a single response. To receive\
  \ additional items, specify this string for the <code>NextToken</code> value when requesting the next set of items. This value is null when there are no more items to return.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"NotificationConfigurations\"\n  ],\n  \"example\": {\n    \"NotificationConfigurations\": [\n      {\n        \"AutoScalingGroupName\": \"my-auto-scaling-group\",\n        \"NotificationType\": \"autoscaling:TEST_NOTIFICATION\",\n        \"TopicARN\": \"arn:aws:sns:us-west-2:123456789012:my-sns-topic-2\"\n      },\n      {\n        \"AutoScalingGroupName\": \"my-auto-scaling-group\",\n        \"NotificationType\": \"autoscaling:TEST_NOTIFICATION\",\n        \"TopicARN\": \"arn:aws:sns:us-west-2:123456789012:my-sns-topic\"\n      }\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-notification-configurations-answer-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: DescribeNotificationConfigurationsAnswer
---
