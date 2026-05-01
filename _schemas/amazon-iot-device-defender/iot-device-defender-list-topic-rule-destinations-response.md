---
description: ListTopicRuleDestinationsResponse schema
layout: schema
name: ListTopicRuleDestinationsResponse
properties_list:
- description: ''
  name: destinationSummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-list-topic-rule-destinations-response-schema.json
slug: iot-device-defender-list-topic-rule-destinations-response
source_filename: iot-device-defender-list-topic-rule-destinations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-topic-rule-destinations-response-schema.json\",\n  \"title\": \"ListTopicRuleDestinationsResponse\",\n  \"description\": \"ListTopicRuleDestinationsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"destinationSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TopicRuleDestinationSummaries\"\n        },\n        {\n          \"description\": \"Information about a topic rule destination.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to use to get the next set of results, or <b>null</b> if there are no additional results.\"\n        }\n      ]\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-topic-rule-destinations-response-schema.json
tags:
- Compliance
- IoT
- Security
- Vulnerability Management
title: ListTopicRuleDestinationsResponse
---
