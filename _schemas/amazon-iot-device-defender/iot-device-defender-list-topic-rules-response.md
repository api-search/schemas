---
description: The output from the ListTopicRules operation.
layout: schema
name: ListTopicRulesResponse
properties_list:
- description: ''
  name: rules
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-list-topic-rules-response-schema.json
slug: iot-device-defender-list-topic-rules-response
source_filename: iot-device-defender-list-topic-rules-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-topic-rules-response-schema.json\",\n  \"title\": \"ListTopicRulesResponse\",\n  \"description\": \"The output from the ListTopicRules operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TopicRuleList\"\n        },\n        {\n          \"description\": \"The rules.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to use to get the next set of results, or <b>null</b> if there are no additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-topic-rules-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: ListTopicRulesResponse
---
