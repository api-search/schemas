---
description: BatchUpdateVehicleResponse schema
layout: schema
name: BatchUpdateVehicleResponse
properties_list:
- description: ''
  name: vehicles
  type: object
- description: ''
  name: errors
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-batch-update-vehicle-response-schema.json
slug: iot-fleetwise-batch-update-vehicle-response
source_filename: iot-fleetwise-batch-update-vehicle-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-batch-update-vehicle-response-schema.json\",\n  \"title\": \"BatchUpdateVehicleResponse\",\n  \"description\": \"BatchUpdateVehicleResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vehicles\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/updateVehicleResponseItems\"\n        },\n        {\n          \"description\": \"<p> A list of information about the batch of updated vehicles. </p> <note> <p>This list contains only unique IDs for the vehicles that were updated.</p> </note>\"\n        }\n      ]\n    },\n    \"errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/updateVehicleErrors\"\n        },\n        {\n          \"description\": \"A list of information about errors returned while updating a\
  \ batch of vehicles, or, if there aren't any errors, an empty list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-batch-update-vehicle-response-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: BatchUpdateVehicleResponse
---
