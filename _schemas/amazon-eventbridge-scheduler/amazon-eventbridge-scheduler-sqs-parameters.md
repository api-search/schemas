---
description: The templated target type for the Amazon SQS <a href="https://docs.aws.amazon.com/AWSSimpleQueueService/latest/APIReference/API_SendMessage.html"> <code>SendMessage</code> </a> API operation. Contains the message group ID to use when the target is a FIFO queue. If you specify an Amazon SQS FIFO queue as a target, the queue must have content-based deduplication enabled. For more information, see <a href="https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/using-messagededuplicationid-property.html">Using the Amazon SQS message deduplication ID</a> in the <i>Amazon SQS Developer Guide</i>.
layout: schema
name: SqsParameters
properties_list:
- description: ''
  name: MessageGroupId
  type: object
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-sqs-parameters-schema.json
slug: amazon-eventbridge-scheduler-sqs-parameters
source_filename: amazon-eventbridge-scheduler-sqs-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-sqs-parameters-schema.json\",\n  \"title\": \"SqsParameters\",\n  \"description\": \"The templated target type for the Amazon SQS <a href=\\\"https://docs.aws.amazon.com/AWSSimpleQueueService/latest/APIReference/API_SendMessage.html\\\"> <code>SendMessage</code> </a> API operation. Contains the message group ID to use when the target is a FIFO queue. If you specify an Amazon SQS FIFO queue as a target, the queue must have content-based deduplication enabled. For more information, see <a href=\\\"https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/using-messagededuplicationid-property.html\\\">Using the Amazon SQS message deduplication ID</a> in the <i>Amazon SQS Developer Guide</i>. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"\
  MessageGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MessageGroupId\"\n        },\n        {\n          \"description\": \"The FIFO message group ID to use as the target.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-sqs-parameters-schema.json
tags:
- Amazon Web Services
- Cron
- Event-Driven
- Scheduling
- Serverless
title: SqsParameters
---
