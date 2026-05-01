---
description: UpdateModelManifestRequest schema
layout: schema
name: UpdateModelManifestRequest
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: nodesToAdd
  type: object
- description: ''
  name: nodesToRemove
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-update-model-manifest-request-schema.json
slug: iot-fleetwise-update-model-manifest-request
source_filename: iot-fleetwise-update-model-manifest-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-update-model-manifest-request-schema.json\",\n  \"title\": \"UpdateModelManifestRequest\",\n  \"description\": \"UpdateModelManifestRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/resourceName\"\n        },\n        {\n          \"description\": \" The name of the vehicle model to update. \"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/description\"\n        },\n        {\n          \"description\": \" A brief description of the vehicle model. \"\n        }\n      ]\n    },\n    \"nodesToAdd\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePaths\"\n        },\n \
  \       {\n          \"description\": \" A list of <code>fullyQualifiedName</code> of nodes, which are a general abstraction of signals, to add to the vehicle model. \"\n        }\n      ]\n    },\n    \"nodesToRemove\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePaths\"\n        },\n        {\n          \"description\": \" A list of <code>fullyQualifiedName</code> of nodes, which are a general abstraction of signals, to remove from the vehicle model. \"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ManifestStatus\"\n        },\n        {\n          \"description\": \" The state of the vehicle model. If the status is <code>ACTIVE</code>, the vehicle model can't be edited. If the status is <code>DRAFT</code>, you can edit the vehicle model. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-update-model-manifest-request-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: UpdateModelManifestRequest
---
