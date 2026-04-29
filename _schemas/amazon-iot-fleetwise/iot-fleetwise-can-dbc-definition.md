---
description: Configurations used to create a decoder manifest.
layout: schema
name: CanDbcDefinition
properties_list:
- description: ''
  name: networkInterface
  type: object
- description: ''
  name: canDbcFiles
  type: object
- description: ''
  name: signalsMap
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-can-dbc-definition-schema.json
slug: iot-fleetwise-can-dbc-definition
source_filename: iot-fleetwise-can-dbc-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-can-dbc-definition-schema.json\",\n  \"title\": \"CanDbcDefinition\",\n  \"description\": \"Configurations used to create a decoder manifest.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"networkInterface\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InterfaceId\"\n        },\n        {\n          \"description\": \"Contains information about a network interface.\"\n        }\n      ]\n    },\n    \"canDbcFiles\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkFilesList\"\n        },\n        {\n          \"description\": \"A list of DBC files. You can upload only one DBC file for each network interface and specify up to five (inclusive) files in the list.\"\n        }\n      ]\n    },\n    \"signalsMap\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelSignalsMap\"\n        },\n        {\n          \"description\": \"Pairs every signal specified in your vehicle model with a signal decoder.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"networkInterface\",\n    \"canDbcFiles\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-can-dbc-definition-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: CanDbcDefinition
---
