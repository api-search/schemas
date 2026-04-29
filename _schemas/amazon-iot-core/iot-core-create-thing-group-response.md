---
description: CreateThingGroupResponse schema
layout: schema
name: CreateThingGroupResponse
properties_list:
- description: ''
  name: thingGroupName
  type: object
- description: ''
  name: thingGroupArn
  type: object
- description: ''
  name: thingGroupId
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-create-thing-group-response-schema.json
slug: iot-core-create-thing-group-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-create-thing-group-response-schema.json\",\n  \"title\": \"CreateThingGroupResponse\",\n  \"description\": \"CreateThingGroupResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"thingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingGroupName\"\n        },\n        {\n          \"description\": \"The thing group name.\"\n        }\n      ]\n    },\n    \"thingGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingGroupArn\"\n        },\n        {\n          \"description\": \"The thing group ARN.\"\n        }\n      ]\n    },\n    \"thingGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingGroupId\"\n        },\n        {\n          \"description\": \"\
  The thing group ID.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-create-thing-group-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: CreateThingGroupResponse
---
