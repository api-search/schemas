---
description: NetworkInterfaces schema
layout: schema
name: NetworkInterfaces
properties_list: []
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-network-interfaces-schema.json
slug: iot-fleetwise-network-interfaces
source_filename: iot-fleetwise-network-interfaces-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-network-interfaces-schema.json\",\n  \"title\": \"NetworkInterfaces\",\n  \"description\": \"NetworkInterfaces schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"interfaceId\",\n      \"type\"\n    ],\n    \"properties\": {\n      \"interfaceId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/InterfaceId\"\n          },\n          {\n            \"description\": \"The ID of the network interface.\"\n          }\n        ]\n      },\n      \"type\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/NetworkInterfaceType\"\n          },\n          {\n            \"description\": \"The network protocol for the vehicle. For example, <code>CAN_SIGNAL</code> specifies\
  \ a protocol that defines how data is communicated between electronic control units (ECUs). <code>OBD_SIGNAL</code> specifies a protocol that defines how self-diagnostic data is communicated between ECUs.\"\n          }\n        ]\n      },\n      \"canInterface\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/CanInterface\"\n          },\n          {\n            \"description\": \"Information about a network interface specified by the Controller Area Network (CAN) protocol.\"\n          }\n        ]\n      },\n      \"obdInterface\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ObdInterface\"\n          },\n          {\n            \"description\": \"Information about a network interface specified by the On-board diagnostic (OBD) II protocol.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"<p>Represents a node and its specifications in an in-vehicle communication network. All signal decoders\
  \ must be associated with a network node. </p> <p> To return this information about all the network interfaces specified in a decoder manifest, use the API operation.</p>\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-network-interfaces-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: NetworkInterfaces
---
