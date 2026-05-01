---
description: <p>Represents a node and its specifications in an in-vehicle communication network. All signal decoders must be associated with a network node. </p> <p> To return this information about all the network interfaces specified in a decoder manifest, use the API operation.</p>
layout: schema
name: NetworkInterface
properties_list:
- description: ''
  name: interfaceId
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: canInterface
  type: object
- description: ''
  name: obdInterface
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-network-interface-schema.json
slug: iot-fleetwise-network-interface
source_filename: iot-fleetwise-network-interface-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-network-interface-schema.json\",\n  \"title\": \"NetworkInterface\",\n  \"description\": \"<p>Represents a node and its specifications in an in-vehicle communication network. All signal decoders must be associated with a network node. </p> <p> To return this information about all the network interfaces specified in a decoder manifest, use the API operation.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"interfaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InterfaceId\"\n        },\n        {\n          \"description\": \"The ID of the network interface.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkInterfaceType\"\n        },\n        {\n          \"\
  description\": \"The network protocol for the vehicle. For example, <code>CAN_SIGNAL</code> specifies a protocol that defines how data is communicated between electronic control units (ECUs). <code>OBD_SIGNAL</code> specifies a protocol that defines how self-diagnostic data is communicated between ECUs.\"\n        }\n      ]\n    },\n    \"canInterface\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CanInterface\"\n        },\n        {\n          \"description\": \"Information about a network interface specified by the Controller Area Network (CAN) protocol.\"\n        }\n      ]\n    },\n    \"obdInterface\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ObdInterface\"\n        },\n        {\n          \"description\": \"Information about a network interface specified by the On-board diagnostic (OBD) II protocol.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"interfaceId\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-network-interface-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: NetworkInterface
---
