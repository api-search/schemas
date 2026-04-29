---
description: ListActiveViolationsResponse schema
layout: schema
name: ListActiveViolationsResponse
properties_list:
- description: ''
  name: activeViolations
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-list-active-violations-response-schema.json
slug: iot-core-list-active-violations-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-active-violations-response-schema.json\",\n  \"title\": \"ListActiveViolationsResponse\",\n  \"description\": \"ListActiveViolationsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"activeViolations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActiveViolations\"\n        },\n        {\n          \"description\": \"The list of active violations.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token that can be used to retrieve the next set of results, or <code>null</code> if there are no additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-active-violations-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: ListActiveViolationsResponse
---
