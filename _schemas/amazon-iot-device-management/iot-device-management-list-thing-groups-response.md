---
description: ListThingGroupsResponse schema
layout: schema
name: ListThingGroupsResponse
properties_list:
- description: ''
  name: thingGroups
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-list-thing-groups-response-schema.json
slug: iot-device-management-list-thing-groups-response
source_filename: iot-device-management-list-thing-groups-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-thing-groups-response-schema.json\",\n  \"title\": \"ListThingGroupsResponse\",\n  \"description\": \"ListThingGroupsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"thingGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingGroupNameAndArnList\"\n        },\n        {\n          \"description\": \"The thing groups.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to use to get the next set of results. Will not be returned if operation has returned all results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-thing-groups-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: ListThingGroupsResponse
---
