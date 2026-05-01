---
description: ListOTAUpdatesResponse schema
layout: schema
name: ListOTAUpdatesResponse
properties_list:
- description: ''
  name: otaUpdates
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-list-o-t-a-updates-response-schema.json
slug: iot-core-list-o-t-a-updates-response
source_filename: iot-core-list-o-t-a-updates-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-o-t-a-updates-response-schema.json\",\n  \"title\": \"ListOTAUpdatesResponse\",\n  \"description\": \"ListOTAUpdatesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"otaUpdates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OTAUpdatesSummary\"\n        },\n        {\n          \"description\": \"A list of OTA update jobs.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token to use to get the next set of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-o-t-a-updates-response-schema.json
tags:
- Device Management
- IoT
- MQTT
- Message Routing
title: ListOTAUpdatesResponse
---
