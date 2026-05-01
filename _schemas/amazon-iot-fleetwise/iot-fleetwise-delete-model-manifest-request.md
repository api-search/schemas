---
description: DeleteModelManifestRequest schema
layout: schema
name: DeleteModelManifestRequest
properties_list:
- description: ''
  name: name
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-delete-model-manifest-request-schema.json
slug: iot-fleetwise-delete-model-manifest-request
source_filename: iot-fleetwise-delete-model-manifest-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-delete-model-manifest-request-schema.json\",\n  \"title\": \"DeleteModelManifestRequest\",\n  \"description\": \"DeleteModelManifestRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/resourceName\"\n        },\n        {\n          \"description\": \" The name of the model manifest to delete. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-delete-model-manifest-request-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: DeleteModelManifestRequest
---
