---
description: BatchCreateVehicleResponse schema
layout: schema
name: BatchCreateVehicleResponse
properties_list:
- description: ''
  name: vehicles
  type: object
- description: ''
  name: errors
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-batch-create-vehicle-response-schema.json
slug: iot-fleetwise-batch-create-vehicle-response
source_filename: iot-fleetwise-batch-create-vehicle-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-batch-create-vehicle-response-schema.json\",\n  \"title\": \"BatchCreateVehicleResponse\",\n  \"description\": \"BatchCreateVehicleResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vehicles\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/createVehicleResponses\"\n        },\n        {\n          \"description\": \" A list of information about a batch of created vehicles. For more information, see the API data type.\"\n        }\n      ]\n    },\n    \"errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/createVehicleErrors\"\n        },\n        {\n          \"description\": \"A list of information about creation errors, or an empty list if there aren't any errors. \"\n        }\n      ]\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-batch-create-vehicle-response-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: BatchCreateVehicleResponse
---
