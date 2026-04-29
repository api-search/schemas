---
description: GetVehicleRequest schema
layout: schema
name: GetVehicleRequest
properties_list:
- description: ''
  name: vehicleName
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-get-vehicle-request-schema.json
slug: iot-fleetwise-get-vehicle-request
source_filename: iot-fleetwise-get-vehicle-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-get-vehicle-request-schema.json\",\n  \"title\": \"GetVehicleRequest\",\n  \"description\": \"GetVehicleRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vehicleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/vehicleName\"\n        },\n        {\n          \"description\": \" The ID of the vehicle to retrieve information about. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"vehicleName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-get-vehicle-request-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: GetVehicleRequest
---
