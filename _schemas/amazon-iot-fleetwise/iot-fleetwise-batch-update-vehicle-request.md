---
description: BatchUpdateVehicleRequest schema
layout: schema
name: BatchUpdateVehicleRequest
properties_list:
- description: ''
  name: vehicles
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-batch-update-vehicle-request-schema.json
slug: iot-fleetwise-batch-update-vehicle-request
source_filename: iot-fleetwise-batch-update-vehicle-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-batch-update-vehicle-request-schema.json\",\n  \"title\": \"BatchUpdateVehicleRequest\",\n  \"description\": \"BatchUpdateVehicleRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vehicles\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/updateVehicleRequestItems\"\n        },\n        {\n          \"description\": \" A list of information about the vehicles to update. For more information, see the API data type.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"vehicles\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-batch-update-vehicle-request-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: BatchUpdateVehicleRequest
---
