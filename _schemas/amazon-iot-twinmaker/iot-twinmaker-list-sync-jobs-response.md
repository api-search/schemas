---
description: ListSyncJobsResponse schema
layout: schema
name: ListSyncJobsResponse
properties_list:
- description: ''
  name: syncJobSummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-list-sync-jobs-response-schema.json
slug: iot-twinmaker-list-sync-jobs-response
source_filename: iot-twinmaker-list-sync-jobs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-list-sync-jobs-response-schema.json\",\n  \"title\": \"ListSyncJobsResponse\",\n  \"description\": \"ListSyncJobsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"syncJobSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyncJobSummaries\"\n        },\n        {\n          \"description\": \"The listed SyncJob summaries.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The string that specifies the next page of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-list-sync-jobs-response-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: ListSyncJobsResponse
---
