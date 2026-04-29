---
description: Parameters used when defining a mitigation action that move a set of things to a thing group.
layout: schema
name: AddThingsToThingGroupParams
properties_list:
- description: ''
  name: thingGroupNames
  type: object
- description: ''
  name: overrideDynamicGroups
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-add-things-to-thing-group-params-schema.json
slug: iot-device-management-add-things-to-thing-group-params
source_filename: iot-device-management-add-things-to-thing-group-params-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-add-things-to-thing-group-params-schema.json\",\n  \"title\": \"AddThingsToThingGroupParams\",\n  \"description\": \"Parameters used when defining a mitigation action that move a set of things to a thing group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"thingGroupNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingGroupNames\"\n        },\n        {\n          \"description\": \"The list of groups to which you want to add the things that triggered the mitigation action. You can add a thing to a maximum of 10 groups, but you can't add a thing to more than one group in the same hierarchy.\"\n        }\n      ]\n    },\n    \"overrideDynamicGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\
  \n        },\n        {\n          \"description\": \"Specifies if this mitigation action can move the things that triggered the mitigation action even if they are part of one or more dynamic thing groups.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"thingGroupNames\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-add-things-to-thing-group-params-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: AddThingsToThingGroupParams
---
