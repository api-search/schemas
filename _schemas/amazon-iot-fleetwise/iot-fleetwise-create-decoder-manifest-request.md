---
description: CreateDecoderManifestRequest schema
layout: schema
name: CreateDecoderManifestRequest
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: modelManifestArn
  type: object
- description: ''
  name: signalDecoders
  type: object
- description: ''
  name: networkInterfaces
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-create-decoder-manifest-request-schema.json
slug: iot-fleetwise-create-decoder-manifest-request
source_filename: iot-fleetwise-create-decoder-manifest-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-create-decoder-manifest-request-schema.json\",\n  \"title\": \"CreateDecoderManifestRequest\",\n  \"description\": \"CreateDecoderManifestRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/resourceName\"\n        },\n        {\n          \"description\": \" The unique name of the decoder manifest to create.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/description\"\n        },\n        {\n          \"description\": \" A brief description of the decoder manifest. \"\n        }\n      ]\n    },\n    \"modelManifestArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/arn\"\
  \n        },\n        {\n          \"description\": \" The Amazon Resource Name (ARN) of the vehicle model (model manifest). \"\n        }\n      ]\n    },\n    \"signalDecoders\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SignalDecoders\"\n        },\n        {\n          \"description\": \" A list of information about signal decoders. \"\n        }\n      ]\n    },\n    \"networkInterfaces\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkInterfaces\"\n        },\n        {\n          \"description\": \" A list of information about available network interfaces. \"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"Metadata that can be used to manage the decoder manifest.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"modelManifestArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-create-decoder-manifest-request-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: CreateDecoderManifestRequest
---
