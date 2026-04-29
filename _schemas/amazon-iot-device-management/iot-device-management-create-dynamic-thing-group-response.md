---
description: CreateDynamicThingGroupResponse schema
layout: schema
name: CreateDynamicThingGroupResponse
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
- description: ''
  name: indexName
  type: object
- description: ''
  name: queryString
  type: object
- description: ''
  name: queryVersion
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-create-dynamic-thing-group-response-schema.json
slug: iot-device-management-create-dynamic-thing-group-response
source_filename: iot-device-management-create-dynamic-thing-group-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-dynamic-thing-group-response-schema.json\",\n  \"title\": \"CreateDynamicThingGroupResponse\",\n  \"description\": \"CreateDynamicThingGroupResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"thingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingGroupName\"\n        },\n        {\n          \"description\": \"The dynamic thing group name.\"\n        }\n      ]\n    },\n    \"thingGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingGroupArn\"\n        },\n        {\n          \"description\": \"The dynamic thing group ARN.\"\n        }\n      ]\n    },\n    \"thingGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingGroupId\"\
  \n        },\n        {\n          \"description\": \"The dynamic thing group ID.\"\n        }\n      ]\n    },\n    \"indexName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IndexName\"\n        },\n        {\n          \"description\": \"The dynamic thing group index name.\"\n        }\n      ]\n    },\n    \"queryString\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryString\"\n        },\n        {\n          \"description\": \"The dynamic thing group search query string.\"\n        }\n      ]\n    },\n    \"queryVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryVersion\"\n        },\n        {\n          \"description\": \"The dynamic thing group query version.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-dynamic-thing-group-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: CreateDynamicThingGroupResponse
---
