---
description: Information required to publish the Amazon SNS message.
layout: schema
name: SNSTopicPublishAction
properties_list:
- description: ''
  name: targetArn
  type: object
- description: ''
  name: payload
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-s-n-s-topic-publish-action-schema.json
slug: iot-events-s-n-s-topic-publish-action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-s-n-s-topic-publish-action-schema.json\",\n  \"title\": \"SNSTopicPublishAction\",\n  \"description\": \"Information required to publish the Amazon SNS message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"targetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The ARN of the Amazon SNS target where the message is sent.\"\n        }\n      ]\n    },\n    \"payload\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Payload\"\n        },\n        {\n          \"description\": \"You can configure the action payload when you send a message as an Amazon SNS push notification.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"targetArn\"\n\
  \  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-s-n-s-topic-publish-action-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: SNSTopicPublishAction
---
