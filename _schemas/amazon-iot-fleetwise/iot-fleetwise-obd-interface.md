---
description: A network interface that specifies the On-board diagnostic (OBD) II network protocol.
layout: schema
name: ObdInterface
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: requestMessageId
  type: object
- description: ''
  name: obdStandard
  type: object
- description: ''
  name: pidRequestIntervalSeconds
  type: object
- description: ''
  name: dtcRequestIntervalSeconds
  type: object
- description: ''
  name: useExtendedIds
  type: object
- description: ''
  name: hasTransmissionEcu
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-obd-interface-schema.json
slug: iot-fleetwise-obd-interface
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-obd-interface-schema.json\",\n  \"title\": \"ObdInterface\",\n  \"description\": \"A network interface that specifies the On-board diagnostic (OBD) II network protocol.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ObdInterfaceName\"\n        },\n        {\n          \"description\": \"The name of the interface.\"\n        }\n      ]\n    },\n    \"requestMessageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/nonNegativeInteger\"\n        },\n        {\n          \"description\": \"The ID of the message requesting vehicle data.\"\n        }\n      ]\n    },\n    \"obdStandard\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ObdStandard\"\
  \n        },\n        {\n          \"description\": \"The standard OBD II PID.\"\n        }\n      ]\n    },\n    \"pidRequestIntervalSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/nonNegativeInteger\"\n        },\n        {\n          \"description\": \"The maximum number message requests per second.\"\n        }\n      ]\n    },\n    \"dtcRequestIntervalSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/nonNegativeInteger\"\n        },\n        {\n          \"description\": \"The maximum number message requests per diagnostic trouble code per second.\"\n        }\n      ]\n    },\n    \"useExtendedIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/boolean\"\n        },\n        {\n          \"description\": \"Whether to use extended IDs in the message.\"\n        }\n      ]\n    },\n    \"hasTransmissionEcu\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/boolean\"\
  \n        },\n        {\n          \"description\": \"Whether the vehicle has a transmission control module (TCM).\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"requestMessageId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-obd-interface-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: ObdInterface
---
