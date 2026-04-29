---
description: Information required to publish the MQTT message through the AWS IoT message broker.
layout: schema
name: IotTopicPublishAction
properties_list:
- description: ''
  name: mqttTopic
  type: object
- description: ''
  name: payload
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-iot-topic-publish-action-schema.json
slug: iot-events-iot-topic-publish-action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-iot-topic-publish-action-schema.json\",\n  \"title\": \"IotTopicPublishAction\",\n  \"description\": \"Information required to publish the MQTT message through the AWS IoT message broker.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mqttTopic\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MQTTTopic\"\n        },\n        {\n          \"description\": \"The MQTT topic of the message. You can use a string expression that includes variables (<code>$variable.&lt;variable-name&gt;</code>) and input values (<code>$input.&lt;input-name&gt;.&lt;path-to-datum&gt;</code>) as the topic string.\"\n        }\n      ]\n    },\n    \"payload\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Payload\"\n        },\n        {\n      \
  \    \"description\": \"You can configure the action payload when you publish a message to an AWS IoT Core topic.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"mqttTopic\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-iot-topic-publish-action-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: IotTopicPublishAction
---
