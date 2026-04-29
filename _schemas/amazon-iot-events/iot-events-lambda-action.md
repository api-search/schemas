---
description: Calls a Lambda function, passing in information about the detector model instance and the event that triggered the action.
layout: schema
name: LambdaAction
properties_list:
- description: ''
  name: functionArn
  type: object
- description: ''
  name: payload
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-lambda-action-schema.json
slug: iot-events-lambda-action
source_filename: iot-events-lambda-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-lambda-action-schema.json\",\n  \"title\": \"LambdaAction\",\n  \"description\": \"Calls a Lambda function, passing in information about the detector model instance and the event that triggered the action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"functionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The ARN of the Lambda function that is executed.\"\n        }\n      ]\n    },\n    \"payload\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Payload\"\n        },\n        {\n          \"description\": \"You can configure the action payload when you send a message to a Lambda function.\"\n        }\n      ]\n    }\n  },\n  \"required\":\
  \ [\n    \"functionArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-lambda-action-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: LambdaAction
---
