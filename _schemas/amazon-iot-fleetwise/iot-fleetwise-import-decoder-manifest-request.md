---
description: ImportDecoderManifestRequest schema
layout: schema
name: ImportDecoderManifestRequest
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: networkFileDefinitions
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-import-decoder-manifest-request-schema.json
slug: iot-fleetwise-import-decoder-manifest-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-import-decoder-manifest-request-schema.json\",\n  \"title\": \"ImportDecoderManifestRequest\",\n  \"description\": \"ImportDecoderManifestRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/resourceName\"\n        },\n        {\n          \"description\": \" The name of the decoder manifest to import. \"\n        }\n      ]\n    },\n    \"networkFileDefinitions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkFileDefinitions\"\n        },\n        {\n          \"description\": \" The file to load into an Amazon Web Services account. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"networkFileDefinitions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-import-decoder-manifest-request-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: ImportDecoderManifestRequest
---
