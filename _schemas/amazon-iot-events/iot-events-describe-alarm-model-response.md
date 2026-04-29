---
description: DescribeAlarmModelResponse schema
layout: schema
name: DescribeAlarmModelResponse
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
- description: ''
  name: statusMessage
  type: object
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
schema_file: json-schema/iot-events-describe-alarm-model-response-schema.json
slug: iot-events-describe-alarm-model-response
source_filename: iot-events-describe-alarm-model-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-describe-alarm-model-response-schema.json\",\n  \"title\": \"DescribeAlarmModelResponse\",\n  \"description\": \"DescribeAlarmModelResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time the alarm model was created, in the Unix epoch format.\"\n        }\n      ]\n    },\n    \"alarmModelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlarmModelArn\"\n        },\n        {\n          \"description\": \"The ARN of the alarm model. For more information, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs)</a>\
  \ in the <i>AWS General Reference</i>.\"\n        }\n      ]\n    },\n    \"alarmModelVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlarmModelVersion\"\n        },\n        {\n          \"description\": \"The version of the alarm model.\"\n        }\n      ]\n    },\n    \"lastUpdateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time the alarm model was last updated, in the Unix epoch format.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlarmModelVersionStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the alarm model. The status can be one of the following values:</p> <ul> <li> <p> <code>ACTIVE</code> - The alarm model is active and it's ready to evaluate data.</p> </li> <li> <p> <code>ACTIVATING</code> - AWS IoT Events is activating\
  \ your alarm model. Activating an alarm model can take up to a few minutes.</p> </li> <li> <p> <code>INACTIVE</code> - The alarm model is inactive, so it isn't ready to evaluate data. Check your alarm model information and update the alarm model.</p> </li> <li> <p> <code>FAILED</code> - You couldn't create or update the alarm model. Check your alarm model information and try again.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"statusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusMessage\"\n        },\n        {\n          \"description\": \" Contains information about the status of the alarm model. \"\n        }\n      ]\n    },\n    \"alarmModelName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlarmModelName\"\n        },\n        {\n          \"description\": \"The name of the alarm model.\"\n        }\n      ]\n    },\n    \"alarmModelDescription\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/AlarmModelDescription\"\n        },\n        {\n          \"description\": \"The description of the alarm model.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The ARN of the IAM role that allows the alarm to perform actions and access AWS resources. For more information, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs)</a> in the <i>AWS General Reference</i>.\"\n        }\n      ]\n    },\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeJsonPath\"\n        },\n        {\n          \"description\": \"An input attribute used as a key to create an alarm. AWS IoT Events routes <a href=\\\"https://docs.aws.amazon.com/iotevents/latest/apireference/API_Input.html\\\">inputs</a> associated\
  \ with this key to the alarm.\"\n        }\n      ]\n    },\n    \"severity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Severity\"\n        },\n        {\n          \"description\": \"A non-negative integer that reflects the severity level of the alarm.\"\n        }\n      ]\n    },\n    \"alarmRule\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlarmRule\"\n        },\n        {\n          \"description\": \"Defines when your alarm is invoked.\"\n        }\n      ]\n    },\n    \"alarmNotification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlarmNotification\"\n        },\n        {\n          \"description\": \"Contains information about one or more notification actions.\"\n        }\n      ]\n    },\n    \"alarmEventActions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlarmEventActions\"\n        },\n        {\n          \"description\": \"Contains\
  \ information about one or more alarm actions.\"\n        }\n      ]\n    },\n    \"alarmCapabilities\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlarmCapabilities\"\n        },\n        {\n          \"description\": \"Contains the configuration information of alarm state changes.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-describe-alarm-model-response-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: DescribeAlarmModelResponse
---
