---
description: CreateTopicRuleDestinationResponse schema
layout: schema
name: CreateTopicRuleDestinationResponse
properties_list:
- description: ''
  name: topicRuleDestination
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-create-topic-rule-destination-response-schema.json
slug: iot-device-management-create-topic-rule-destination-response
source_filename: iot-device-management-create-topic-rule-destination-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-topic-rule-destination-response-schema.json\",\n  \"title\": \"CreateTopicRuleDestinationResponse\",\n  \"description\": \"CreateTopicRuleDestinationResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"topicRuleDestination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TopicRuleDestination\"\n        },\n        {\n          \"description\": \"The topic rule destination.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-topic-rule-destination-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: CreateTopicRuleDestinationResponse
---
