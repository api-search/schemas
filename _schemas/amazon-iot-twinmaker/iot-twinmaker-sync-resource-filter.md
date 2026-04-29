---
description: The sync resource filter.
layout: schema
name: SyncResourceFilter
properties_list:
- description: ''
  name: state
  type: object
- description: ''
  name: resourceType
  type: object
- description: ''
  name: resourceId
  type: object
- description: ''
  name: externalId
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-sync-resource-filter-schema.json
slug: iot-twinmaker-sync-resource-filter
source_filename: iot-twinmaker-sync-resource-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-sync-resource-filter-schema.json\",\n  \"title\": \"SyncResourceFilter\",\n  \"description\": \"The sync resource filter.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"state\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyncResourceState\"\n        },\n        {\n          \"description\": \"The sync resource filter's state.\"\n        }\n      ]\n    },\n    \"resourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyncResourceType\"\n        },\n        {\n          \"description\": \"The sync resource filter resource type\"\n        }\n      ]\n    },\n    \"resourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\"\
  : \"The sync resource filter resource ID.\"\n        }\n      ]\n    },\n    \"externalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The external ID.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-sync-resource-filter-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: SyncResourceFilter
---
