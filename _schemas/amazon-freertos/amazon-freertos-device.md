---
description: A FreeRTOS-capable microcontroller device registered in AWS IoT.
layout: schema
name: Device
properties_list:
- description: IoT thing name for the device.
  name: thingName
  type: string
- description: ARN of the IoT thing.
  name: thingArn
  type: string
- description: Type classification of the device.
  name: thingTypeName
  type: string
- description: Device attributes (hardware model, firmware version, etc.)
  name: attributes
  type: object
- description: Thing record version.
  name: version
  type: integer
provider_name: Amazon FreeRTOS
provider_slug: amazon-freertos
schema_file: json-schema/amazon-freertos-device-schema.json
slug: amazon-freertos-device
source_filename: amazon-freertos-device-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-freertos/refs/heads/main/json-schema/amazon-freertos-device-schema.json\",\n  \"title\": \"Device\",\n  \"description\": \"A FreeRTOS-capable microcontroller device registered in AWS IoT.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"thingName\": {\n      \"type\": \"string\",\n      \"description\": \"IoT thing name for the device.\"\n    },\n    \"thingArn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the IoT thing.\"\n    },\n    \"thingTypeName\": {\n      \"type\": \"string\",\n      \"description\": \"Type classification of the device.\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Device attributes (hardware model, firmware version, etc.)\"\n    },\n    \"version\": {\n      \"type\": \"\
  integer\",\n      \"description\": \"Thing record version.\"\n    }\n  },\n  \"required\": [\n    \"thingName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-freertos/refs/heads/main/json-schema/amazon-freertos-device-schema.json
tags:
- Embedded Systems
- IoT
- Microcontrollers
- RTOS
title: Device
---
