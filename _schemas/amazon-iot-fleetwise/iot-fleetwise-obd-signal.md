---
description: Information about signal messages using the on-board diagnostics (OBD) II protocol in a vehicle.
layout: schema
name: ObdSignal
properties_list:
- description: ''
  name: pidResponseLength
  type: object
- description: ''
  name: serviceMode
  type: object
- description: ''
  name: pid
  type: object
- description: ''
  name: scaling
  type: object
- description: ''
  name: offset
  type: object
- description: ''
  name: startByte
  type: object
- description: ''
  name: byteLength
  type: object
- description: ''
  name: bitRightShift
  type: object
- description: ''
  name: bitMaskLength
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-obd-signal-schema.json
slug: iot-fleetwise-obd-signal
source_filename: iot-fleetwise-obd-signal-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-obd-signal-schema.json\",\n  \"title\": \"ObdSignal\",\n  \"description\": \"Information about signal messages using the on-board diagnostics (OBD) II protocol in a vehicle.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pidResponseLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/positiveInteger\"\n        },\n        {\n          \"description\": \"The length of the requested data.\"\n        }\n      ]\n    },\n    \"serviceMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/nonNegativeInteger\"\n        },\n        {\n          \"description\": \"The mode of operation (diagnostic service) in a message.\"\n        }\n      ]\n    },\n    \"pid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/nonNegativeInteger\"\n        },\n        {\n          \"description\": \"The diagnostic code used to request data from a vehicle for this signal.\"\n        }\n      ]\n    },\n    \"scaling\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/double\"\n        },\n        {\n          \"description\": \"A multiplier used to decode the message.\"\n        }\n      ]\n    },\n    \"offset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/double\"\n        },\n        {\n          \"description\": \"The offset used to calculate the signal value. Combined with scaling, the calculation is <code>value = raw_value * scaling + offset</code>.\"\n        }\n      ]\n    },\n    \"startByte\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/nonNegativeInteger\"\n        },\n        {\n          \"description\": \"Indicates the beginning of the message.\"\n        }\n      ]\n    },\n    \"\
  byteLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ObdByteLength\"\n        },\n        {\n          \"description\": \"The length of a message.\"\n        }\n      ]\n    },\n    \"bitRightShift\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/nonNegativeInteger\"\n        },\n        {\n          \"description\": \"The number of positions to shift bits in the message.\"\n        }\n      ]\n    },\n    \"bitMaskLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ObdBitmaskLength\"\n        },\n        {\n          \"description\": \"The number of bits to mask in a message.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"pidResponseLength\",\n    \"serviceMode\",\n    \"pid\",\n    \"scaling\",\n    \"offset\",\n    \"startByte\",\n    \"byteLength\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-obd-signal-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: ObdSignal
---
