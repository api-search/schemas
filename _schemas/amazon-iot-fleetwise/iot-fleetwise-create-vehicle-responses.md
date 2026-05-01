---
description: createVehicleResponses schema
layout: schema
name: createVehicleResponses
properties_list: []
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-create-vehicle-responses-schema.json
slug: iot-fleetwise-create-vehicle-responses
source_filename: iot-fleetwise-create-vehicle-responses-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-create-vehicle-responses-schema.json\",\n  \"title\": \"createVehicleResponses\",\n  \"description\": \"createVehicleResponses schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"vehicleName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/vehicleName\"\n          },\n          {\n            \"description\": \"The unique ID of the vehicle to create.\"\n          }\n        ]\n      },\n      \"arn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/arn\"\n          },\n          {\n            \"description\": \"The ARN of the created vehicle.\"\n          }\n        ]\n      },\n      \"thingArn\": {\n        \"allOf\": [\n          {\n            \"$ref\"\
  : \"#/components/schemas/arn\"\n          },\n          {\n            \"description\": \"The ARN of a created or validated Amazon Web Services IoT thing.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Information about a created vehicle.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-create-vehicle-responses-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: createVehicleResponses
---
