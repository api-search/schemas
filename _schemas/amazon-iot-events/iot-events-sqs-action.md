---
description: Sends information about the detector model instance and the event that triggered the action to an Amazon SQS queue.
layout: schema
name: SqsAction
properties_list:
- description: ''
  name: queueUrl
  type: object
- description: ''
  name: useBase64
  type: object
- description: ''
  name: payload
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-sqs-action-schema.json
slug: iot-events-sqs-action
source_filename: iot-events-sqs-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-sqs-action-schema.json\",\n  \"title\": \"SqsAction\",\n  \"description\": \"Sends information about the detector model instance and the event that triggered the action to an Amazon SQS queue.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"queueUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueueUrl\"\n        },\n        {\n          \"description\": \"The URL of the SQS queue where the data is written.\"\n        }\n      ]\n    },\n    \"useBase64\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UseBase64\"\n        },\n        {\n          \"description\": \"Set this to TRUE if you want the data to be base-64 encoded before it is written to the queue. Otherwise, set this to FALSE.\"\n        }\n      ]\n    },\n\
  \    \"payload\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Payload\"\n        },\n        {\n          \"description\": \"You can configure the action payload when you send a message to an Amazon SQS queue.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"queueUrl\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-sqs-action-schema.json
tags:
- Event Detection
- IoT
- State Machine
- Automation
title: SqsAction
---
