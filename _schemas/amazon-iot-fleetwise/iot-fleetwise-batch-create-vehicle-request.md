---
description: BatchCreateVehicleRequest schema
layout: schema
name: BatchCreateVehicleRequest
properties_list:
- description: ''
  name: vehicles
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-batch-create-vehicle-request-schema.json
slug: iot-fleetwise-batch-create-vehicle-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-batch-create-vehicle-request-schema.json\",\n  \"title\": \"BatchCreateVehicleRequest\",\n  \"description\": \"BatchCreateVehicleRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vehicles\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/createVehicleRequestItems\"\n        },\n        {\n          \"description\": \" A list of information about each vehicle to create. For more information, see the API data type.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"vehicles\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-batch-create-vehicle-request-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: BatchCreateVehicleRequest
---
