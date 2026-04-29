---
description: An IIO context representing a local or remote IIO system
layout: schema
name: IIOContext
properties_list:
- description: Context name (e.g., local, ip, usb)
  name: name
  type: string
- description: Context description
  name: description
  type: string
- description: IIO XML version
  name: xml_version
  type: string
- description: IIO devices in this context
  name: devices
  type: array
- description: Context-level attributes
  name: attrs
  type: object
provider_name: Analog Devices
provider_slug: analog-devices
schema_file: json-schema/analog-devices-iio-context-schema.json
slug: analog-devices-iio-context
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/analog-devices/refs/heads/main/json-schema/analog-devices-iio-context-schema.json\",\n  \"title\": \"IIOContext\",\n  \"description\": \"An IIO context representing a local or remote IIO system\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Context name (e.g., local, ip, usb)\",\n      \"example\": \"local\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Context description\"\n    },\n    \"xml_version\": {\n      \"type\": \"string\",\n      \"description\": \"IIO XML version\"\n    },\n    \"devices\": {\n      \"type\": \"array\",\n      \"description\": \"IIO devices in this context\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"attrs\": {\n      \"type\": \"object\",\n      \"description\": \"Context-level\
  \ attributes\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/analog-devices/refs/heads/main/json-schema/analog-devices-iio-context-schema.json
tags:
- Embedded Systems
- Hardware
- IoT
- Semiconductor
- Signal Processing
title: IIOContext
---
