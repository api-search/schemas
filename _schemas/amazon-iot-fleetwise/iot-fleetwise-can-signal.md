---
description: Information about a single controller area network (CAN) signal and the messages it receives and transmits.
layout: schema
name: CanSignal
properties_list:
- description: ''
  name: messageId
  type: object
- description: ''
  name: isBigEndian
  type: object
- description: ''
  name: isSigned
  type: object
- description: ''
  name: startBit
  type: object
- description: ''
  name: offset
  type: object
- description: ''
  name: factor
  type: object
- description: ''
  name: length
  type: object
- description: ''
  name: name
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-can-signal-schema.json
slug: iot-fleetwise-can-signal
source_filename: iot-fleetwise-can-signal-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-can-signal-schema.json\",\n  \"title\": \"CanSignal\",\n  \"description\": \"Information about a single controller area network (CAN) signal and the messages it receives and transmits.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"messageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/nonNegativeInteger\"\n        },\n        {\n          \"description\": \"The ID of the message.\"\n        }\n      ]\n    },\n    \"isBigEndian\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/boolean\"\n        },\n        {\n          \"description\": \"Whether the byte ordering of a CAN message is big-endian.\"\n        }\n      ]\n    },\n    \"isSigned\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/boolean\"\
  \n        },\n        {\n          \"description\": \"Whether the message data is specified as a signed value.\"\n        }\n      ]\n    },\n    \"startBit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/nonNegativeInteger\"\n        },\n        {\n          \"description\": \"<p>Indicates the beginning of the CAN signal. This should always be the least significant bit (LSB).</p> <p>This value might be different from the value in a DBC file. For little endian signals, <code>startBit</code> is the same value as in the DBC file. For big endian signals in a DBC file, the start bit is the most significant bit (MSB). You will have to calculate the LSB instead and pass it as the <code>startBit</code>.</p>\"\n        }\n      ]\n    },\n    \"offset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/double\"\n        },\n        {\n          \"description\": \"The offset used to calculate the signal value. Combined with factor, the\
  \ calculation is <code>value = raw_value * factor + offset</code>.\"\n        }\n      ]\n    },\n    \"factor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/double\"\n        },\n        {\n          \"description\": \"A multiplier used to decode the CAN message.\"\n        }\n      ]\n    },\n    \"length\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/nonNegativeInteger\"\n        },\n        {\n          \"description\": \"How many bytes of data are in the message.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CanSignalName\"\n        },\n        {\n          \"description\": \"The name of the signal.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"messageId\",\n    \"isBigEndian\",\n    \"isSigned\",\n    \"startBit\",\n    \"offset\",\n    \"factor\",\n    \"length\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-can-signal-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: CanSignal
---
