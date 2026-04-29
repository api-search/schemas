---
description: Specifications for defining a vehicle network.
layout: schema
name: NetworkFileDefinition
properties_list:
- description: ''
  name: canDbc
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-network-file-definition-schema.json
slug: iot-fleetwise-network-file-definition
source_filename: iot-fleetwise-network-file-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-network-file-definition-schema.json\",\n  \"title\": \"NetworkFileDefinition\",\n  \"description\": \"Specifications for defining a vehicle network.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"canDbc\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CanDbcDefinition\"\n        },\n        {\n          \"description\": \"Information, including CAN DBC files, about the configurations used to create a decoder manifest.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-network-file-definition-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: NetworkFileDefinition
---
