---
description: Contains the notification settings of an alarm model. The settings apply to all alarms that were created based on this alarm model.
layout: schema
name: NotificationAction
properties_list:
- description: ''
  name: action
  type: object
- description: ''
  name: smsConfigurations
  type: object
- description: ''
  name: emailConfigurations
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-notification-action-schema.json
slug: iot-events-notification-action
source_filename: iot-events-notification-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-notification-action-schema.json\",\n  \"title\": \"NotificationAction\",\n  \"description\": \"Contains the notification settings of an alarm model. The settings apply to all alarms that were created based on this alarm model.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationTargetActions\"\n        },\n        {\n          \"description\": \"Specifies an AWS Lambda function to manage alarm notifications. You can create one or use the <a href=\\\"https://docs.aws.amazon.com/iotevents/latest/developerguide/lambda-support.html\\\">AWS Lambda function provided by AWS IoT Events</a>.\"\n        }\n      ]\n    },\n    \"smsConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/SMSConfigurations\"\n        },\n        {\n          \"description\": \"Contains the configuration information of SMS notifications.\"\n        }\n      ]\n    },\n    \"emailConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailConfigurations\"\n        },\n        {\n          \"description\": \"Contains the configuration information of email notifications.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"action\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-notification-action-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: NotificationAction
---
