---
description: An HTTP error resulting from creating a vehicle.
layout: schema
name: CreateVehicleError
properties_list:
- description: ''
  name: vehicleName
  type: object
- description: ''
  name: code
  type: object
- description: ''
  name: message
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-create-vehicle-error-schema.json
slug: iot-fleetwise-create-vehicle-error
source_filename: iot-fleetwise-create-vehicle-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-create-vehicle-error-schema.json\",\n  \"title\": \"CreateVehicleError\",\n  \"description\": \"An HTTP error resulting from creating a vehicle.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vehicleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/vehicleName\"\n        },\n        {\n          \"description\": \"The ID of the vehicle with the error.\"\n        }\n      ]\n    },\n    \"code\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"description\": \"An HTTP error code.\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"description\": \"A description\
  \ of the HTTP error.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-create-vehicle-error-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: CreateVehicleError
---
