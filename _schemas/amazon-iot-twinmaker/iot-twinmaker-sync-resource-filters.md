---
description: SyncResourceFilters schema
layout: schema
name: SyncResourceFilters
properties_list: []
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-sync-resource-filters-schema.json
slug: iot-twinmaker-sync-resource-filters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-sync-resource-filters-schema.json\",\n  \"title\": \"SyncResourceFilters\",\n  \"description\": \"SyncResourceFilters schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"state\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/SyncResourceState\"\n          },\n          {\n            \"description\": \"The sync resource filter's state.\"\n          }\n        ]\n      },\n      \"resourceType\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/SyncResourceType\"\n          },\n          {\n            \"description\": \"The sync resource filter resource type\"\n          }\n        ]\n      },\n      \"resourceId\": {\n        \"allOf\": [\n          {\n   \
  \         \"$ref\": \"#/components/schemas/Id\"\n          },\n          {\n            \"description\": \"The sync resource filter resource ID.\"\n          }\n        ]\n      },\n      \"externalId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Id\"\n          },\n          {\n            \"description\": \"The external ID.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"The sync resource filter.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-sync-resource-filters-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: SyncResourceFilters
---
