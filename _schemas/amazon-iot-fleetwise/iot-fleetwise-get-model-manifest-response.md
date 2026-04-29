---
description: GetModelManifestResponse schema
layout: schema
name: GetModelManifestResponse
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: signalCatalogArn
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: creationTime
  type: object
- description: ''
  name: lastModificationTime
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-get-model-manifest-response-schema.json
slug: iot-fleetwise-get-model-manifest-response
source_filename: iot-fleetwise-get-model-manifest-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-get-model-manifest-response-schema.json\",\n  \"title\": \"GetModelManifestResponse\",\n  \"description\": \"GetModelManifestResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/resourceName\"\n        },\n        {\n          \"description\": \" The name of the vehicle model. \"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/arn\"\n        },\n        {\n          \"description\": \" The Amazon Resource Name (ARN) of the vehicle model. \"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/description\"\n        },\n        {\n        \
  \  \"description\": \" A brief description of the vehicle model. \"\n        }\n      ]\n    },\n    \"signalCatalogArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/arn\"\n        },\n        {\n          \"description\": \" The ARN of the signal catalog associated with the vehicle model. \"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ManifestStatus\"\n        },\n        {\n          \"description\": \" The state of the vehicle model. If the status is <code>ACTIVE</code>, the vehicle model can't be edited. You can edit the vehicle model if the status is marked <code>DRAFT</code>.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/timestamp\"\n        },\n        {\n          \"description\": \"The time the vehicle model was created, in seconds since epoch (January 1, 1970 at midnight UTC time).\"\
  \n        }\n      ]\n    },\n    \"lastModificationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/timestamp\"\n        },\n        {\n          \"description\": \"The last time the vehicle model was modified.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"arn\",\n    \"creationTime\",\n    \"lastModificationTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-get-model-manifest-response-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: GetModelManifestResponse
---
