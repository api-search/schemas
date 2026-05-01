---
description: CreateFleetRequest schema
layout: schema
name: CreateFleetRequest
properties_list:
- description: ''
  name: fleetId
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: signalCatalogArn
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-create-fleet-request-schema.json
slug: iot-fleetwise-create-fleet-request
source_filename: iot-fleetwise-create-fleet-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-create-fleet-request-schema.json\",\n  \"title\": \"CreateFleetRequest\",\n  \"description\": \"CreateFleetRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/fleetId\"\n        },\n        {\n          \"description\": \" The unique ID of the fleet to create. \"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/description\"\n        },\n        {\n          \"description\": \" A brief description of the fleet to create. \"\n        }\n      ]\n    },\n    \"signalCatalogArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/arn\"\n        },\n        {\n          \"description\"\
  : \" The Amazon Resource Name (ARN) of a signal catalog. \"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"Metadata that can be used to manage the fleet.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"fleetId\",\n    \"signalCatalogArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-create-fleet-request-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: CreateFleetRequest
---
