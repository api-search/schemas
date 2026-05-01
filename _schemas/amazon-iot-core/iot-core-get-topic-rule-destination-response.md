---
description: GetTopicRuleDestinationResponse schema
layout: schema
name: GetTopicRuleDestinationResponse
properties_list:
- description: ''
  name: topicRuleDestination
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-get-topic-rule-destination-response-schema.json
slug: iot-core-get-topic-rule-destination-response
source_filename: iot-core-get-topic-rule-destination-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-get-topic-rule-destination-response-schema.json\",\n  \"title\": \"GetTopicRuleDestinationResponse\",\n  \"description\": \"GetTopicRuleDestinationResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"topicRuleDestination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TopicRuleDestination\"\n        },\n        {\n          \"description\": \"The topic rule destination.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-get-topic-rule-destination-response-schema.json
tags:
- Device Management
- IoT
- MQTT
- Message Routing
title: GetTopicRuleDestinationResponse
---
