---
description: Sends information about the detector model instance and the event that triggered the action to an Amazon Kinesis Data Firehose delivery stream.
layout: schema
name: FirehoseAction
properties_list:
- description: ''
  name: deliveryStreamName
  type: object
- description: ''
  name: separator
  type: object
- description: ''
  name: payload
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-firehose-action-schema.json
slug: iot-events-firehose-action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-firehose-action-schema.json\",\n  \"title\": \"FirehoseAction\",\n  \"description\": \"Sends information about the detector model instance and the event that triggered the action to an Amazon Kinesis Data Firehose delivery stream.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deliveryStreamName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeliveryStreamName\"\n        },\n        {\n          \"description\": \"The name of the Kinesis Data Firehose delivery stream where the data is written.\"\n        }\n      ]\n    },\n    \"separator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirehoseSeparator\"\n        },\n        {\n          \"description\": \"A character separator that is used to separate records written\
  \ to the Kinesis Data Firehose delivery stream. Valid values are: '\\\\n' (newline), '\\\\t' (tab), '\\\\r\\\\n' (Windows newline), ',' (comma).\"\n        }\n      ]\n    },\n    \"payload\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Payload\"\n        },\n        {\n          \"description\": \"You can configure the action payload when you send a message to an Amazon Kinesis Data Firehose delivery stream.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"deliveryStreamName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-firehose-action-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: FirehoseAction
---
