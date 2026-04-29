---
description: ListStreamsResponse schema
layout: schema
name: ListStreamsResponse
properties_list:
- description: ''
  name: streams
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-list-streams-response-schema.json
slug: iot-core-list-streams-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-streams-response-schema.json\",\n  \"title\": \"ListStreamsResponse\",\n  \"description\": \"ListStreamsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"streams\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamsSummary\"\n        },\n        {\n          \"description\": \"A list of streams.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token used to get the next set of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-streams-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: ListStreamsResponse
---
