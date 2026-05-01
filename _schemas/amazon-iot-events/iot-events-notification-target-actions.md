---
description: Specifies an AWS Lambda function to manage alarm notifications. You can create one or use the <a href="https://docs.aws.amazon.com/iotevents/latest/developerguide/lambda-support.html">AWS Lambda function provided by AWS IoT Events</a>.
layout: schema
name: NotificationTargetActions
properties_list:
- description: Calls a Lambda function, passing in information about the detector model instance and the event that triggered the action.
  name: lambdaAction
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-notification-target-actions-schema.json
slug: iot-events-notification-target-actions
source_filename: iot-events-notification-target-actions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-notification-target-actions-schema.json\",\n  \"title\": \"NotificationTargetActions\",\n  \"description\": \"Specifies an AWS Lambda function to manage alarm notifications. You can create one or use the <a href=\\\"https://docs.aws.amazon.com/iotevents/latest/developerguide/lambda-support.html\\\">AWS Lambda function provided by AWS IoT Events</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lambdaAction\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"functionArn\"\n      ],\n      \"properties\": {\n        \"functionArn\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/AmazonResourceName\"\n            },\n            {\n              \"description\": \"The ARN of the Lambda function that is executed.\"\n        \
  \    }\n          ]\n        },\n        \"payload\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Payload\"\n            },\n            {\n              \"description\": \"You can configure the action payload when you send a message to a Lambda function.\"\n            }\n          ]\n        }\n      },\n      \"description\": \"Calls a Lambda function, passing in information about the detector model instance and the event that triggered the action.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-notification-target-actions-schema.json
tags:
- Event Detection
- IoT
- State Machine
- Automation
title: NotificationTargetActions
---
