---
description: CreateSignalCatalogRequest schema
layout: schema
name: CreateSignalCatalogRequest
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
  name: tags
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-create-signal-catalog-request-schema.json
slug: iot-fleetwise-create-signal-catalog-request
source_filename: iot-fleetwise-create-signal-catalog-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-create-signal-catalog-request-schema.json\",\n  \"title\": \"CreateSignalCatalogRequest\",\n  \"description\": \"CreateSignalCatalogRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/resourceName\"\n        },\n        {\n          \"description\": \" The name of the signal catalog to create. \"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/description\"\n        },\n        {\n          \"description\": \"A brief description of the signal catalog.\"\n        }\n      ]\n    },\n    \"nodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Nodes\"\n        },\n        {\n\
  \          \"description\": \" A list of information about nodes, which are a general abstraction of signals. For more information, see the API data type.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"Metadata that can be used to manage the signal catalog.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-create-signal-catalog-request-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: CreateSignalCatalogRequest
---
