---
description: UpdateSignalCatalogRequest schema
layout: schema
name: UpdateSignalCatalogRequest
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
  name: nodesToUpdate
  type: object
- description: ''
  name: nodesToRemove
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-update-signal-catalog-request-schema.json
slug: iot-fleetwise-update-signal-catalog-request
source_filename: iot-fleetwise-update-signal-catalog-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-update-signal-catalog-request-schema.json\",\n  \"title\": \"UpdateSignalCatalogRequest\",\n  \"description\": \"UpdateSignalCatalogRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/resourceName\"\n        },\n        {\n          \"description\": \" The name of the signal catalog to update. \"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/description\"\n        },\n        {\n          \"description\": \" A brief description of the signal catalog to update.\"\n        }\n      ]\n    },\n    \"nodesToAdd\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Nodes\"\n      \
  \  },\n        {\n          \"description\": \" A list of information about nodes to add to the signal catalog. \"\n        }\n      ]\n    },\n    \"nodesToUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Nodes\"\n        },\n        {\n          \"description\": \" A list of information about nodes to update in the signal catalog. \"\n        }\n      ]\n    },\n    \"nodesToRemove\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePaths\"\n        },\n        {\n          \"description\": \" A list of <code>fullyQualifiedName</code> of nodes to remove from the signal catalog. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-update-signal-catalog-request-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: UpdateSignalCatalogRequest
---
