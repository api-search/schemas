---
description: DeleteVehicleResponse schema
layout: schema
name: DeleteVehicleResponse
properties_list:
- description: ''
  name: vehicleName
  type: object
- description: ''
  name: arn
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-delete-vehicle-response-schema.json
slug: iot-fleetwise-delete-vehicle-response
source_filename: iot-fleetwise-delete-vehicle-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-delete-vehicle-response-schema.json\",\n  \"title\": \"DeleteVehicleResponse\",\n  \"description\": \"DeleteVehicleResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vehicleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/vehicleName\"\n        },\n        {\n          \"description\": \"The ID of the deleted vehicle.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the deleted vehicle.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"vehicleName\",\n    \"arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-delete-vehicle-response-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: DeleteVehicleResponse
---
