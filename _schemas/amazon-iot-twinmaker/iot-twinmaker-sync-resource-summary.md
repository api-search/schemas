---
description: The sync resource summary.
layout: schema
name: SyncResourceSummary
properties_list:
- description: ''
  name: resourceType
  type: object
- description: ''
  name: externalId
  type: object
- description: ''
  name: resourceId
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: updateDateTime
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-sync-resource-summary-schema.json
slug: iot-twinmaker-sync-resource-summary
source_filename: iot-twinmaker-sync-resource-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-sync-resource-summary-schema.json\",\n  \"title\": \"SyncResourceSummary\",\n  \"description\": \"The sync resource summary.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyncResourceType\"\n        },\n        {\n          \"description\": \"The resource type.\"\n        }\n      ]\n    },\n    \"externalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The external ID.\"\n        }\n      ]\n    },\n    \"resourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The resource ID.\"\n        }\n      ]\n\
  \    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyncResourceStatus\"\n        },\n        {\n          \"description\": \"The sync resource summary status.\"\n        }\n      ]\n    },\n    \"updateDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The update date and time.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-sync-resource-summary-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: SyncResourceSummary
---
