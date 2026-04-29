---
description: The output of the CreateThing operation.
layout: schema
name: CreateThingResponse
properties_list:
- description: ''
  name: thingName
  type: object
- description: ''
  name: thingArn
  type: object
- description: ''
  name: thingId
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-create-thing-response-schema.json
slug: iot-core-create-thing-response
source_filename: iot-core-create-thing-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-create-thing-response-schema.json\",\n  \"title\": \"CreateThingResponse\",\n  \"description\": \"The output of the CreateThing operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"thingName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingName\"\n        },\n        {\n          \"description\": \"The name of the new thing.\"\n        }\n      ]\n    },\n    \"thingArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingArn\"\n        },\n        {\n          \"description\": \"The ARN of the new thing.\"\n        }\n      ]\n    },\n    \"thingId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingId\"\n        },\n        {\n          \"description\": \"The thing ID.\"\n     \
  \   }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-create-thing-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: CreateThingResponse
---
