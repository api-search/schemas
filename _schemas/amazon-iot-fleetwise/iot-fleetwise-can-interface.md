---
description: A single controller area network (CAN) device interface.
layout: schema
name: CanInterface
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: protocolName
  type: object
- description: ''
  name: protocolVersion
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-can-interface-schema.json
slug: iot-fleetwise-can-interface
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-can-interface-schema.json\",\n  \"title\": \"CanInterface\",\n  \"description\": \"A single controller area network (CAN) device interface.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CanInterfaceName\"\n        },\n        {\n          \"description\": \"The unique name of the interface.\"\n        }\n      ]\n    },\n    \"protocolName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProtocolName\"\n        },\n        {\n          \"description\": \"The name of the communication protocol for the interface.\"\n        }\n      ]\n    },\n    \"protocolVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProtocolVersion\"\n\
  \        },\n        {\n          \"description\": \"The version of the communication protocol for the interface.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-can-interface-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: CanInterface
---
