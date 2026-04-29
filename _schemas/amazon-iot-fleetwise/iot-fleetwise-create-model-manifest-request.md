---
description: CreateModelManifestRequest schema
layout: schema
name: CreateModelManifestRequest
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: nodes
  type: object
- description: ''
  name: signalCatalogArn
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-create-model-manifest-request-schema.json
slug: iot-fleetwise-create-model-manifest-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-create-model-manifest-request-schema.json\",\n  \"title\": \"CreateModelManifestRequest\",\n  \"description\": \"CreateModelManifestRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/resourceName\"\n        },\n        {\n          \"description\": \" The name of the vehicle model to create.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/description\"\n        },\n        {\n          \"description\": \" A brief description of the vehicle model. \"\n        }\n      ]\n    },\n    \"nodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/listOfStrings\"\n        },\n   \
  \     {\n          \"description\": \" A list of nodes, which are a general abstraction of signals. \"\n        }\n      ]\n    },\n    \"signalCatalogArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/arn\"\n        },\n        {\n          \"description\": \" The Amazon Resource Name (ARN) of a signal catalog. \"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"Metadata that can be used to manage the vehicle model.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"nodes\",\n    \"signalCatalogArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-create-model-manifest-request-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: CreateModelManifestRequest
---
