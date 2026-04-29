---
description: AlarmActions schema
layout: schema
name: AlarmActions
properties_list: []
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-alarm-actions-schema.json
slug: iot-events-alarm-actions
source_filename: iot-events-alarm-actions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-alarm-actions-schema.json\",\n  \"title\": \"AlarmActions\",\n  \"description\": \"AlarmActions schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"sns\": {\n        \"$ref\": \"#/components/schemas/SNSTopicPublishAction\"\n      },\n      \"iotTopicPublish\": {\n        \"$ref\": \"#/components/schemas/IotTopicPublishAction\"\n      },\n      \"lambda\": {\n        \"$ref\": \"#/components/schemas/LambdaAction\"\n      },\n      \"iotEvents\": {\n        \"$ref\": \"#/components/schemas/IotEventsAction\"\n      },\n      \"sqs\": {\n        \"$ref\": \"#/components/schemas/SqsAction\"\n      },\n      \"firehose\": {\n        \"$ref\": \"#/components/schemas/FirehoseAction\"\n      },\n      \"dynamoDB\": {\n        \"$ref\": \"#/components/schemas/DynamoDBAction\"\
  \n      },\n      \"dynamoDBv2\": {\n        \"$ref\": \"#/components/schemas/DynamoDBv2Action\"\n      },\n      \"iotSiteWise\": {\n        \"$ref\": \"#/components/schemas/IotSiteWiseAction\"\n      }\n    },\n    \"description\": \"Specifies one of the following actions to receive notifications when the alarm state changes.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-alarm-actions-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: AlarmActions
---
