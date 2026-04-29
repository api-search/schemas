---
description: CreateAlarmModelRequest schema
layout: schema
name: CreateAlarmModelRequest
properties_list:
- description: ''
  name: alarmModelName
  type: object
- description: ''
  name: alarmModelDescription
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: key
  type: object
- description: ''
  name: severity
  type: object
- description: ''
  name: alarmRule
  type: object
- description: ''
  name: alarmNotification
  type: object
- description: ''
  name: alarmEventActions
  type: object
- description: ''
  name: alarmCapabilities
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-create-alarm-model-request-schema.json
slug: iot-events-create-alarm-model-request
source_filename: iot-events-create-alarm-model-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-create-alarm-model-request-schema.json\",\n  \"title\": \"CreateAlarmModelRequest\",\n  \"description\": \"CreateAlarmModelRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"alarmModelName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlarmModelName\"\n        },\n        {\n          \"description\": \"A unique name that helps you identify the alarm model. You can't change this name after you create the alarm model.\"\n        }\n      ]\n    },\n    \"alarmModelDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlarmModelDescription\"\n        },\n        {\n          \"description\": \"A description that tells you what the alarm model detects.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The ARN of the IAM role that allows the alarm to perform actions and access AWS resources. For more information, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs)</a> in the <i>AWS General Reference</i>.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"<p>A list of key-value pairs that contain metadata for the alarm model. The tags help you manage the alarm model. For more information, see <a href=\\\"https://docs.aws.amazon.com/iotevents/latest/developerguide/tagging-iotevents.html\\\">Tagging your AWS IoT Events resources</a> in the <i>AWS IoT Events Developer Guide</i>.</p> <p>You can create up to 50 tags for one alarm model.</p>\"\n\
  \        }\n      ]\n    },\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeJsonPath\"\n        },\n        {\n          \"description\": \"An input attribute used as a key to create an alarm. AWS IoT Events routes <a href=\\\"https://docs.aws.amazon.com/iotevents/latest/apireference/API_Input.html\\\">inputs</a> associated with this key to the alarm.\"\n        }\n      ]\n    },\n    \"severity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Severity\"\n        },\n        {\n          \"description\": \"A non-negative integer that reflects the severity level of the alarm.\"\n        }\n      ]\n    },\n    \"alarmRule\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlarmRule\"\n        },\n        {\n          \"description\": \"Defines when your alarm is invoked.\"\n        }\n      ]\n    },\n    \"alarmNotification\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/AlarmNotification\"\n        },\n        {\n          \"description\": \"Contains information about one or more notification actions.\"\n        }\n      ]\n    },\n    \"alarmEventActions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlarmEventActions\"\n        },\n        {\n          \"description\": \"Contains information about one or more alarm actions.\"\n        }\n      ]\n    },\n    \"alarmCapabilities\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlarmCapabilities\"\n        },\n        {\n          \"description\": \"Contains the configuration information of alarm state changes.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"alarmModelName\",\n    \"roleArn\",\n    \"alarmRule\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-create-alarm-model-request-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: CreateAlarmModelRequest
---
