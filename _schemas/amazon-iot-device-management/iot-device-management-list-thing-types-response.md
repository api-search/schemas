---
description: The output for the ListThingTypes operation.
layout: schema
name: ListThingTypesResponse
properties_list:
- description: ''
  name: thingTypes
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-list-thing-types-response-schema.json
slug: iot-device-management-list-thing-types-response
source_filename: iot-device-management-list-thing-types-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-thing-types-response-schema.json\",\n  \"title\": \"ListThingTypesResponse\",\n  \"description\": \"The output for the ListThingTypes operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"thingTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingTypeList\"\n        },\n        {\n          \"description\": \"The thing types.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token for the next set of results. Will not be returned if operation has returned all results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-thing-types-response-schema.json
tags:
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: ListThingTypesResponse
---
