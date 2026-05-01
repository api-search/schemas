---
description: CreateAlarmModelResponse schema
layout: schema
name: CreateAlarmModelResponse
properties_list:
- description: ''
  name: creationTime
  type: object
- description: ''
  name: alarmModelArn
  type: object
- description: ''
  name: alarmModelVersion
  type: object
- description: ''
  name: lastUpdateTime
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-create-alarm-model-response-schema.json
slug: iot-events-create-alarm-model-response
source_filename: iot-events-create-alarm-model-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-create-alarm-model-response-schema.json\",\n  \"title\": \"CreateAlarmModelResponse\",\n  \"description\": \"CreateAlarmModelResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time the alarm model was created, in the Unix epoch format.\"\n        }\n      ]\n    },\n    \"alarmModelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlarmModelArn\"\n        },\n        {\n          \"description\": \"The ARN of the alarm model. For more information, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs)</a> in\
  \ the <i>AWS General Reference</i>.\"\n        }\n      ]\n    },\n    \"alarmModelVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlarmModelVersion\"\n        },\n        {\n          \"description\": \"The version of the alarm model.\"\n        }\n      ]\n    },\n    \"lastUpdateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time the alarm model was last updated, in the Unix epoch format.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlarmModelVersionStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the alarm model. The status can be one of the following values:</p> <ul> <li> <p> <code>ACTIVE</code> - The alarm model is active and it's ready to evaluate data.</p> </li> <li> <p> <code>ACTIVATING</code> - AWS IoT Events is activating your\
  \ alarm model. Activating an alarm model can take up to a few minutes.</p> </li> <li> <p> <code>INACTIVE</code> - The alarm model is inactive, so it isn't ready to evaluate data. Check your alarm model information and update the alarm model.</p> </li> <li> <p> <code>FAILED</code> - You couldn't create or update the alarm model. Check your alarm model information and try again.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-create-alarm-model-response-schema.json
tags:
- Event Detection
- IoT
- State Machine
- Automation
title: CreateAlarmModelResponse
---
