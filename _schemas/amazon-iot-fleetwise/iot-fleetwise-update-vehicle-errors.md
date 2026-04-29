---
description: updateVehicleErrors schema
layout: schema
name: updateVehicleErrors
properties_list: []
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-update-vehicle-errors-schema.json
slug: iot-fleetwise-update-vehicle-errors
source_filename: iot-fleetwise-update-vehicle-errors-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-update-vehicle-errors-schema.json\",\n  \"title\": \"updateVehicleErrors\",\n  \"description\": \"updateVehicleErrors schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"vehicleName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/vehicleName\"\n          },\n          {\n            \"description\": \"The ID of the vehicle with the error.\"\n          }\n        ]\n      },\n      \"code\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/number\"\n          },\n          {\n            \"description\": \"The relevant HTTP error code (400+).\"\n          }\n        ]\n      },\n      \"message\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"\
  #/components/schemas/string\"\n          },\n          {\n            \"description\": \"A message associated with the error.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"An HTTP error resulting from updating the description for a vehicle.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-update-vehicle-errors-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: updateVehicleErrors
---
