---
description: Sends an AWS IoT Events input, passing in information about the detector model instance and the event that triggered the action.
layout: schema
name: IotEventsAction
properties_list:
- description: ''
  name: inputName
  type: object
- description: ''
  name: payload
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-iot-events-action-schema.json
slug: iot-events-iot-events-action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-iot-events-action-schema.json\",\n  \"title\": \"IotEventsAction\",\n  \"description\": \"Sends an AWS IoT Events input, passing in information about the detector model instance and the event that triggered the action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputName\"\n        },\n        {\n          \"description\": \"The name of the AWS IoT Events input where the data is sent.\"\n        }\n      ]\n    },\n    \"payload\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Payload\"\n        },\n        {\n          \"description\": \"You can configure the action payload when you send a message to an AWS IoT Events input.\"\n        }\n      ]\n    }\n \
  \ },\n  \"required\": [\n    \"inputName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-iot-events-action-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: IotEventsAction
---
