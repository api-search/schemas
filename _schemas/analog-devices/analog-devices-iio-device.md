---
description: Representation of a Linux IIO device as exposed by libiio
layout: schema
name: IIODevice
properties_list:
- description: Device name
  name: name
  type: string
- description: Device identifier
  name: id
  type: string
- description: Optional device label
  name: label
  type: string
- description: List of IIO channels
  name: channels
  type: array
- description: Device-level attributes
  name: attrs
  type: object
provider_name: Analog Devices
provider_slug: analog-devices
schema_file: json-schema/analog-devices-iio-device-schema.json
slug: analog-devices-iio-device
source_filename: analog-devices-iio-device-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/analog-devices/refs/heads/main/json-schema/analog-devices-iio-device-schema.json\",\n  \"title\": \"IIODevice\",\n  \"description\": \"Representation of a Linux IIO device as exposed by libiio\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Device name\",\n      \"example\": \"ad9361-phy\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Device identifier\",\n      \"example\": \"iio:device0\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Optional device label\"\n    },\n    \"channels\": {\n      \"type\": \"array\",\n      \"description\": \"List of IIO channels\",\n      \"items\": {\n        \"$ref\": \"#/$defs/IIOChannel\"\n      }\n    },\n    \"attrs\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Device-level attributes\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"IIOChannel\": {\n      \"type\": \"object\",\n      \"description\": \"An IIO channel (input or output)\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Channel identifier\",\n          \"example\": \"voltage0\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Channel name\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"input\",\n            \"output\"\n          ],\n          \"description\": \"Channel direction\"\n        },\n        \"scan_element\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this is a scan element for buffered capture\"\n        },\n        \"attrs\": {\n          \"type\": \"object\",\n          \"description\": \"Channel attributes\"\
  ,\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/analog-devices/refs/heads/main/json-schema/analog-devices-iio-device-schema.json
tags:
- Embedded Systems
- Hardware
- IoT
- Semiconductor
- Signal Processing
title: IIODevice
---
