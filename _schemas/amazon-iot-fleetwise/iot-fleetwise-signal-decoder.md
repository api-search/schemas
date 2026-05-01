---
description: Information about a signal decoder.
layout: schema
name: SignalDecoder
properties_list:
- description: ''
  name: fullyQualifiedName
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: interfaceId
  type: object
- description: ''
  name: canSignal
  type: object
- description: ''
  name: obdSignal
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-signal-decoder-schema.json
slug: iot-fleetwise-signal-decoder
source_filename: iot-fleetwise-signal-decoder-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-signal-decoder-schema.json\",\n  \"title\": \"SignalDecoder\",\n  \"description\": \"Information about a signal decoder.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fullyQualifiedName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FullyQualifiedName\"\n        },\n        {\n          \"description\": \"The fully qualified name of a signal decoder as defined in a vehicle model.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SignalDecoderType\"\n        },\n        {\n          \"description\": \"The network protocol for the vehicle. For example, <code>CAN_SIGNAL</code> specifies a protocol that defines how data is communicated between electronic control units (ECUs).\
  \ <code>OBD_SIGNAL</code> specifies a protocol that defines how self-diagnostic data is communicated between ECUs.\"\n        }\n      ]\n    },\n    \"interfaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InterfaceId\"\n        },\n        {\n          \"description\": \"The ID of a network interface that specifies what network protocol a vehicle follows.\"\n        }\n      ]\n    },\n    \"canSignal\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CanSignal\"\n        },\n        {\n          \"description\": \"Information about signal decoder using the Controller Area Network (CAN) protocol.\"\n        }\n      ]\n    },\n    \"obdSignal\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ObdSignal\"\n        },\n        {\n          \"description\": \"Information about signal decoder using the On-board diagnostic (OBD) II protocol.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n\
  \    \"fullyQualifiedName\",\n    \"type\",\n    \"interfaceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-signal-decoder-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: SignalDecoder
---
