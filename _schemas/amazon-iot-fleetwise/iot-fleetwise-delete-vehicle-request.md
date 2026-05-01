---
description: DeleteVehicleRequest schema
layout: schema
name: DeleteVehicleRequest
properties_list:
- description: ''
  name: vehicleName
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-delete-vehicle-request-schema.json
slug: iot-fleetwise-delete-vehicle-request
source_filename: iot-fleetwise-delete-vehicle-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-delete-vehicle-request-schema.json\",\n  \"title\": \"DeleteVehicleRequest\",\n  \"description\": \"DeleteVehicleRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vehicleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/vehicleName\"\n        },\n        {\n          \"description\": \"The ID of the vehicle to delete. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"vehicleName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-delete-vehicle-request-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: DeleteVehicleRequest
---
