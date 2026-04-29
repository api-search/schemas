---
description: An action to be performed when the <code>condition</code> is TRUE.
layout: schema
name: Action
properties_list:
- description: ''
  name: setVariable
  type: object
- description: ''
  name: sns
  type: object
- description: ''
  name: iotTopicPublish
  type: object
- description: ''
  name: setTimer
  type: object
- description: ''
  name: clearTimer
  type: object
- description: ''
  name: resetTimer
  type: object
- description: ''
  name: lambda
  type: object
- description: ''
  name: iotEvents
  type: object
- description: ''
  name: sqs
  type: object
- description: ''
  name: firehose
  type: object
- description: ''
  name: dynamoDB
  type: object
- description: ''
  name: dynamoDBv2
  type: object
- description: ''
  name: iotSiteWise
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-action-schema.json
slug: iot-events-action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-action-schema.json\",\n  \"title\": \"Action\",\n  \"description\": \"An action to be performed when the <code>condition</code> is TRUE.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"setVariable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SetVariableAction\"\n        },\n        {\n          \"description\": \"Sets a variable to a specified value.\"\n        }\n      ]\n    },\n    \"sns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SNSTopicPublishAction\"\n        },\n        {\n          \"description\": \"Sends an Amazon SNS message.\"\n        }\n      ]\n    },\n    \"iotTopicPublish\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IotTopicPublishAction\"\n        },\n      \
  \  {\n          \"description\": \"Publishes an MQTT message with the given topic to the AWS IoT message broker.\"\n        }\n      ]\n    },\n    \"setTimer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SetTimerAction\"\n        },\n        {\n          \"description\": \"Information needed to set the timer.\"\n        }\n      ]\n    },\n    \"clearTimer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClearTimerAction\"\n        },\n        {\n          \"description\": \"Information needed to clear the timer.\"\n        }\n      ]\n    },\n    \"resetTimer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResetTimerAction\"\n        },\n        {\n          \"description\": \"Information needed to reset the timer.\"\n        }\n      ]\n    },\n    \"lambda\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaAction\"\n        },\n        {\n          \"\
  description\": \"Calls a Lambda function, passing in information about the detector model instance and the event that triggered the action.\"\n        }\n      ]\n    },\n    \"iotEvents\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IotEventsAction\"\n        },\n        {\n          \"description\": \"Sends AWS IoT Events input, which passes information about the detector model instance and the event that triggered the action.\"\n        }\n      ]\n    },\n    \"sqs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SqsAction\"\n        },\n        {\n          \"description\": \"Sends information about the detector model instance and the event that triggered the action to an Amazon SQS queue.\"\n        }\n      ]\n    },\n    \"firehose\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirehoseAction\"\n        },\n        {\n          \"description\": \"Sends information about the detector\
  \ model instance and the event that triggered the action to an Amazon Kinesis Data Firehose delivery stream.\"\n        }\n      ]\n    },\n    \"dynamoDB\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DynamoDBAction\"\n        },\n        {\n          \"description\": \"Writes to the DynamoDB table that you created. The default action payload contains all attribute-value pairs that have the information about the detector model instance and the event that triggered the action. You can customize the <a href=\\\"https://docs.aws.amazon.com/iotevents/latest/apireference/API_Payload.html\\\">payload</a>. One column of the DynamoDB table receives all attribute-value pairs in the payload that you specify. For more information, see <a href=\\\"https://docs.aws.amazon.com/iotevents/latest/developerguide/iotevents-event-actions.html\\\">Actions</a> in <i>AWS IoT Events Developer Guide</i>.\"\n        }\n      ]\n    },\n    \"dynamoDBv2\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/DynamoDBv2Action\"\n        },\n        {\n          \"description\": \"Writes to the DynamoDB table that you created. The default action payload contains all attribute-value pairs that have the information about the detector model instance and the event that triggered the action. You can customize the <a href=\\\"https://docs.aws.amazon.com/iotevents/latest/apireference/API_Payload.html\\\">payload</a>. A separate column of the DynamoDB table receives one attribute-value pair in the payload that you specify. For more information, see <a href=\\\"https://docs.aws.amazon.com/iotevents/latest/developerguide/iotevents-event-actions.html\\\">Actions</a> in <i>AWS IoT Events Developer Guide</i>.\"\n        }\n      ]\n    },\n    \"iotSiteWise\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IotSiteWiseAction\"\n        },\n        {\n          \"description\": \"Sends information about the detector model\
  \ instance and the event that triggered the action to an asset property in AWS IoT SiteWise .\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-action-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: Action
---
