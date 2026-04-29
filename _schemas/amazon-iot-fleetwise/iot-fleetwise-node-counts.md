---
description: Information about the number of nodes and node types in a vehicle network.
layout: schema
name: NodeCounts
properties_list:
- description: ''
  name: totalNodes
  type: object
- description: ''
  name: totalBranches
  type: object
- description: ''
  name: totalSensors
  type: object
- description: ''
  name: totalAttributes
  type: object
- description: ''
  name: totalActuators
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-node-counts-schema.json
slug: iot-fleetwise-node-counts
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-node-counts-schema.json\",\n  \"title\": \"NodeCounts\",\n  \"description\": \"Information about the number of nodes and node types in a vehicle network.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalNodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/number\"\n        },\n        {\n          \"description\": \"The total number of nodes in a vehicle network.\"\n        }\n      ]\n    },\n    \"totalBranches\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/number\"\n        },\n        {\n          \"description\": \"The total number of nodes in a vehicle network that represent branches.\"\n        }\n      ]\n    },\n    \"totalSensors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/number\"\
  \n        },\n        {\n          \"description\": \"The total number of nodes in a vehicle network that represent sensors.\"\n        }\n      ]\n    },\n    \"totalAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/number\"\n        },\n        {\n          \"description\": \"The total number of nodes in a vehicle network that represent attributes.\"\n        }\n      ]\n    },\n    \"totalActuators\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/number\"\n        },\n        {\n          \"description\": \"The total number of nodes in a vehicle network that represent actuators.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-node-counts-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: NodeCounts
---
