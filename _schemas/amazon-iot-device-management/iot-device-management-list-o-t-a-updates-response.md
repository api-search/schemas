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
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-list-o-t-a-updates-response-schema.json
slug: iot-device-management-list-o-t-a-updates-response
source_filename: iot-device-management-list-o-t-a-updates-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-o-t-a-updates-response-schema.json\",\n  \"title\": \"ListOTAUpdatesResponse\",\n  \"description\": \"ListOTAUpdatesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"otaUpdates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OTAUpdatesSummary\"\n        },\n        {\n          \"description\": \"A list of OTA update jobs.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token to use to get the next set of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-o-t-a-updates-response-schema.json
tags:
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: ListOTAUpdatesResponse
---
