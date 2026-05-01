---
description: UpdateDecoderManifestResponse schema
layout: schema
name: UpdateDecoderManifestResponse
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: arn
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-update-decoder-manifest-response-schema.json
slug: iot-fleetwise-update-decoder-manifest-response
source_filename: iot-fleetwise-update-decoder-manifest-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-update-decoder-manifest-response-schema.json\",\n  \"title\": \"UpdateDecoderManifestResponse\",\n  \"description\": \"UpdateDecoderManifestResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/resourceName\"\n        },\n        {\n          \"description\": \" The name of the updated decoder manifest. \"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/arn\"\n        },\n        {\n          \"description\": \" The Amazon Resource Name (ARN) of the updated decoder manifest. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-update-decoder-manifest-response-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: UpdateDecoderManifestResponse
---
