---
description: <p>The Amazon Simple Notification Service (Amazon SNS) notification settings associated with a specific job. The <code>Notification</code> object is returned as a part of the response syntax of the <code>DescribeJob</code> action in the <code>JobMetadata</code> data type.</p> <p>When the notification settings are defined during job creation, you can choose to notify based on a specific set of job states using the <code>JobStatesToNotify</code> array of strings, or you can specify that you want to have Amazon SNS notifications sent out for all job states with <code>NotifyAll</code> set to true.</p>
layout: schema
name: Notification
properties_list:
- description: ''
  name: SnsTopicARN
  type: object
- description: ''
  name: JobStatesToNotify
  type: object
- description: ''
  name: NotifyAll
  type: object
- description: ''
  name: DevicePickupSnsTopicARN
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-notification-schema.json
slug: amazon-snow-family-notification
source_filename: amazon-snow-family-notification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-notification-schema.json\",\n  \"title\": \"Notification\",\n  \"description\": \"<p>The Amazon Simple Notification Service (Amazon SNS) notification settings associated with a specific job. The <code>Notification</code> object is returned as a part of the response syntax of the <code>DescribeJob</code> action in the <code>JobMetadata</code> data type.</p> <p>When the notification settings are defined during job creation, you can choose to notify based on a specific set of job states using the <code>JobStatesToNotify</code> array of strings, or you can specify that you want to have Amazon SNS notifications sent out for all job states with <code>NotifyAll</code> set to true.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SnsTopicARN\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/SnsTopicARN\"\n        },\n        {\n          \"description\": \"<p>The new SNS <code>TopicArn</code> that you want to associate with this job. You can create Amazon Resource Names (ARNs) for topics by using the <a href=\\\"https://docs.aws.amazon.com/sns/latest/api/API_CreateTopic.html\\\">CreateTopic</a> Amazon SNS API action.</p> <p>You can subscribe email addresses to an Amazon SNS topic through the Amazon Web Services Management Console, or by using the <a href=\\\"https://docs.aws.amazon.com/sns/latest/api/API_Subscribe.html\\\">Subscribe</a> Amazon Simple Notification Service (Amazon SNS) API action.</p>\"\n        }\n      ]\n    },\n    \"JobStatesToNotify\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStateList\"\n        },\n        {\n          \"description\": \"The list of job states that will trigger a notification for this job.\"\n        }\n      ]\n    },\n    \"NotifyAll\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Any change in job state will trigger a notification for this job.\"\n        }\n      ]\n    },\n    \"DevicePickupSnsTopicARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnsTopicARN\"\n        },\n        {\n          \"description\": \"Used to send SNS notifications for the person picking up the device (identified during job creation).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-notification-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: Notification
---
