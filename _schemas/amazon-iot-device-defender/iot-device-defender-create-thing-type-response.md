---
description: The output of the CreateThingType operation.
layout: schema
name: CreateThingTypeResponse
properties_list:
- description: ''
  name: thingTypeName
  type: object
- description: ''
  name: thingTypeArn
  type: object
- description: ''
  name: thingTypeId
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-create-thing-type-response-schema.json
slug: iot-device-defender-create-thing-type-response
source_filename: iot-device-defender-create-thing-type-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-create-thing-type-response-schema.json\",\n  \"title\": \"CreateThingTypeResponse\",\n  \"description\": \"The output of the CreateThingType operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"thingTypeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingTypeName\"\n        },\n        {\n          \"description\": \"The name of the thing type.\"\n        }\n      ]\n    },\n    \"thingTypeArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingTypeArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the thing type.\"\n        }\n      ]\n    },\n    \"thingTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingTypeId\"\
  \n        },\n        {\n          \"description\": \"The thing type ID.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-create-thing-type-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: CreateThingTypeResponse
---
