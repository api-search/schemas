---
description: createVehicleRequestItems schema
layout: schema
name: createVehicleRequestItems
properties_list: []
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-create-vehicle-request-items-schema.json
slug: iot-fleetwise-create-vehicle-request-items
source_filename: iot-fleetwise-create-vehicle-request-items-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-create-vehicle-request-items-schema.json\",\n  \"title\": \"createVehicleRequestItems\",\n  \"description\": \"createVehicleRequestItems schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"vehicleName\",\n      \"modelManifestArn\",\n      \"decoderManifestArn\"\n    ],\n    \"properties\": {\n      \"vehicleName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/vehicleName\"\n          },\n          {\n            \"description\": \"The unique ID of the vehicle to create.\"\n          }\n        ]\n      },\n      \"modelManifestArn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/arn\"\n          },\n          {\n            \"description\": \"The ARN of the\
  \ vehicle model (model manifest) to create the vehicle from.\"\n          }\n        ]\n      },\n      \"decoderManifestArn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/arn\"\n          },\n          {\n            \"description\": \"The Amazon Resource Name (ARN) of a decoder manifest associated with the vehicle to create. \"\n          }\n        ]\n      },\n      \"attributes\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/attributesMap\"\n          },\n          {\n            \"description\": \"Static information about a vehicle in a key-value pair. For example: <code>\\\"engine Type\\\"</code> : <code>\\\"v6\\\"</code> \"\n          }\n        ]\n      },\n      \"associationBehavior\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/VehicleAssociationBehavior\"\n          },\n          {\n            \"description\": \"An option to create a new Amazon Web Services\
  \ IoT thing when creating a vehicle, or to validate an existing thing as a vehicle.\"\n          }\n        ]\n      },\n      \"tags\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/TagList\"\n          },\n          {\n            \"description\": \"Metadata which can be used to manage the vehicle.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Information about the vehicle to create.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-create-vehicle-request-items-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: createVehicleRequestItems
---
