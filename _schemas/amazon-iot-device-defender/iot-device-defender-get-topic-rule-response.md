---
description: The output from the GetTopicRule operation.
layout: schema
name: GetTopicRuleResponse
properties_list:
- description: ''
  name: ruleArn
  type: object
- description: ''
  name: rule
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-get-topic-rule-response-schema.json
slug: iot-device-defender-get-topic-rule-response
source_filename: iot-device-defender-get-topic-rule-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-get-topic-rule-response-schema.json\",\n  \"title\": \"GetTopicRuleResponse\",\n  \"description\": \"The output from the GetTopicRule operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ruleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleArn\"\n        },\n        {\n          \"description\": \"The rule ARN.\"\n        }\n      ]\n    },\n    \"rule\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TopicRule\"\n        },\n        {\n          \"description\": \"The rule.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-get-topic-rule-response-schema.json
tags:
- Compliance
- IoT
- Security
- Vulnerability Management
title: GetTopicRuleResponse
---
