---
description: ListSyncResourcesResponse schema
layout: schema
name: ListSyncResourcesResponse
properties_list:
- description: ''
  name: syncResources
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-list-sync-resources-response-schema.json
slug: iot-twinmaker-list-sync-resources-response
source_filename: iot-twinmaker-list-sync-resources-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-list-sync-resources-response-schema.json\",\n  \"title\": \"ListSyncResourcesResponse\",\n  \"description\": \"ListSyncResourcesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"syncResources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyncResourceSummaries\"\n        },\n        {\n          \"description\": \"The sync resources.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The string that specifies the next page of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-list-sync-resources-response-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: ListSyncResourcesResponse
---
