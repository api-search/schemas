---
description: CreateSyncJobRequest schema
layout: schema
name: CreateSyncJobRequest
properties_list:
- description: ''
  name: syncRole
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-create-sync-job-request-schema.json
slug: iot-twinmaker-create-sync-job-request
source_filename: iot-twinmaker-create-sync-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-create-sync-job-request-schema.json\",\n  \"title\": \"CreateSyncJobRequest\",\n  \"description\": \"CreateSyncJobRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"syncRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The SyncJob IAM role. This IAM role is used by the SyncJob to read from the syncSource, and create, update, or delete the corresponding resources.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The SyncJob tags.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"syncRole\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-create-sync-job-request-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: CreateSyncJobRequest
---
