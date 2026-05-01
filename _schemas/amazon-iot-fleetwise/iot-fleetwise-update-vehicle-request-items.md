---
description: updateVehicleRequestItems schema
layout: schema
name: updateVehicleRequestItems
properties_list: []
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-update-vehicle-request-items-schema.json
slug: iot-fleetwise-update-vehicle-request-items
source_filename: iot-fleetwise-update-vehicle-request-items-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-update-vehicle-request-items-schema.json\",\n  \"title\": \"updateVehicleRequestItems\",\n  \"description\": \"updateVehicleRequestItems schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"vehicleName\"\n    ],\n    \"properties\": {\n      \"vehicleName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/vehicleName\"\n          },\n          {\n            \"description\": \"The unique ID of the vehicle to update.\"\n          }\n        ]\n      },\n      \"modelManifestArn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/arn\"\n          },\n          {\n            \"description\": \"The ARN of the vehicle model (model manifest) associated with the vehicle\
  \ to update.\"\n          }\n        ]\n      },\n      \"decoderManifestArn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/arn\"\n          },\n          {\n            \"description\": \"The ARN of the signal decoder manifest associated with the vehicle to update.\"\n          }\n        ]\n      },\n      \"attributes\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/attributesMap\"\n          },\n          {\n            \"description\": \"<p>Static information about a vehicle in a key-value pair. For example:</p> <p> <code>\\\"engineType\\\"</code> : <code>\\\"1.3 L R2\\\"</code> </p>\"\n          }\n        ]\n      },\n      \"attributeUpdateMode\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/UpdateMode\"\n          },\n          {\n            \"description\": \"<p>The method the specified attributes will update the existing attributes on the vehicle. Use<code>Overwite</code>\
  \ to replace the vehicle attributes with the specified attributes. Or use <code>Merge</code> to combine all attributes.</p> <p>This is required if attributes are present in the input.</p>\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Information about the vehicle to update.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-update-vehicle-request-items-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: updateVehicleRequestItems
---
