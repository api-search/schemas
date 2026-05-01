---
description: GetSyncJobResponse schema
layout: schema
name: GetSyncJobResponse
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: workspaceId
  type: object
- description: ''
  name: syncSource
  type: object
- description: ''
  name: syncRole
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: creationDateTime
  type: object
- description: ''
  name: updateDateTime
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-get-sync-job-response-schema.json
slug: iot-twinmaker-get-sync-job-response
source_filename: iot-twinmaker-get-sync-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-get-sync-job-response-schema.json\",\n  \"title\": \"GetSyncJobResponse\",\n  \"description\": \"GetSyncJobResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TwinMakerArn\"\n        },\n        {\n          \"description\": \"The sync job ARN.\"\n        }\n      ]\n    },\n    \"workspaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The ID of the workspace that contains the sync job.\"\n        }\n      ]\n    },\n    \"syncSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyncSource\"\n        },\n        {\n          \"description\": \"<p>The sync\
  \ soucre.</p> <note> <p>Currently the only supported syncSource is <code>SITEWISE </code>.</p> </note>\"\n        }\n      ]\n    },\n    \"syncRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The sync IAM role.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyncJobStatus\"\n        },\n        {\n          \"description\": \"The SyncJob response status.\"\n        }\n      ]\n    },\n    \"creationDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The creation date and time.\"\n        }\n      ]\n    },\n    \"updateDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The update date and time.\"\n        }\n  \
  \    ]\n    }\n  },\n  \"required\": [\n    \"arn\",\n    \"workspaceId\",\n    \"syncSource\",\n    \"syncRole\",\n    \"status\",\n    \"creationDateTime\",\n    \"updateDateTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-get-sync-job-response-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: GetSyncJobResponse
---
