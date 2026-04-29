---
description: GetSignalCatalogResponse schema
layout: schema
name: GetSignalCatalogResponse
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
  name: nodeCounts
  type: object
- description: ''
  name: creationTime
  type: object
- description: ''
  name: lastModificationTime
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-get-signal-catalog-response-schema.json
slug: iot-fleetwise-get-signal-catalog-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-get-signal-catalog-response-schema.json\",\n  \"title\": \"GetSignalCatalogResponse\",\n  \"description\": \"GetSignalCatalogResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/resourceName\"\n        },\n        {\n          \"description\": \" The name of the signal catalog. \"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/arn\"\n        },\n        {\n          \"description\": \" The Amazon Resource Name (ARN) of the signal catalog. \"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/description\"\n        },\n        {\n      \
  \    \"description\": \" A brief description of the signal catalog. \"\n        }\n      ]\n    },\n    \"nodeCounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeCounts\"\n        },\n        {\n          \"description\": \" The total number of network nodes specified in a signal catalog. \"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/timestamp\"\n        },\n        {\n          \"description\": \" The time the signal catalog was created in seconds since epoch (January 1, 1970 at midnight UTC time). \"\n        }\n      ]\n    },\n    \"lastModificationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/timestamp\"\n        },\n        {\n          \"description\": \"The last time the signal catalog was modified.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"arn\",\n    \"creationTime\",\n    \"lastModificationTime\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-get-signal-catalog-response-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: GetSignalCatalogResponse
---
