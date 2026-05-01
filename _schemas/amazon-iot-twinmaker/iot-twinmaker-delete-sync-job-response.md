---
description: DeleteSyncJobResponse schema
layout: schema
name: DeleteSyncJobResponse
properties_list:
- description: ''
  name: state
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-delete-sync-job-response-schema.json
slug: iot-twinmaker-delete-sync-job-response
source_filename: iot-twinmaker-delete-sync-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-delete-sync-job-response-schema.json\",\n  \"title\": \"DeleteSyncJobResponse\",\n  \"description\": \"DeleteSyncJobResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"state\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyncJobState\"\n        },\n        {\n          \"description\": \"The SyncJob response state.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"state\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-delete-sync-job-response-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: DeleteSyncJobResponse
---
