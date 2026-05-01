---
description: AssociateVehicleFleetRequest schema
layout: schema
name: AssociateVehicleFleetRequest
properties_list:
- description: ''
  name: vehicleName
  type: object
- description: ''
  name: fleetId
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-associate-vehicle-fleet-request-schema.json
slug: iot-fleetwise-associate-vehicle-fleet-request
source_filename: iot-fleetwise-associate-vehicle-fleet-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-associate-vehicle-fleet-request-schema.json\",\n  \"title\": \"AssociateVehicleFleetRequest\",\n  \"description\": \"AssociateVehicleFleetRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vehicleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/vehicleName\"\n        },\n        {\n          \"description\": \" The unique ID of the vehicle to associate with the fleet. \"\n        }\n      ]\n    },\n    \"fleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/fleetId\"\n        },\n        {\n          \"description\": \" The ID of a fleet. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"vehicleName\",\n    \"fleetId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-associate-vehicle-fleet-request-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: AssociateVehicleFleetRequest
---
