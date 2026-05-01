---
description: The parameters for using a Amazon SQS stream as a source.
layout: schema
name: PipeTargetSqsQueueParameters
properties_list:
- description: ''
  name: MessageDeduplicationId
  type: object
- description: ''
  name: MessageGroupId
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-pipe-target-sqs-queue-parameters-schema.json
slug: amazon-eventbridge-pipes-pipe-target-sqs-queue-parameters
source_filename: amazon-eventbridge-pipes-pipe-target-sqs-queue-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-target-sqs-queue-parameters-schema.json\",\n  \"title\": \"PipeTargetSqsQueueParameters\",\n  \"description\": \"The parameters for using a Amazon SQS stream as a source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MessageDeduplicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MessageDeduplicationId\"\n        },\n        {\n          \"description\": \"<p>This parameter applies only to FIFO (first-in-first-out) queues.</p> <p>The token used for deduplication of sent messages.</p>\"\n        }\n      ]\n    },\n    \"MessageGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MessageGroupId\"\n        },\n        {\n          \"description\": \"The FIFO message group ID to use as\
  \ the target.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-target-sqs-queue-parameters-schema.json
tags:
- Amazon Web Services
- Event-Driven
- Integration
- Messaging
- Serverless
title: PipeTargetSqsQueueParameters
---
