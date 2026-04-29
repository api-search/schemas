---
description: CreateWorkspaceResponse schema
layout: schema
name: CreateWorkspaceResponse
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: creationDateTime
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-create-workspace-response-schema.json
slug: iot-twinmaker-create-workspace-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-create-workspace-response-schema.json\",\n  \"title\": \"CreateWorkspaceResponse\",\n  \"description\": \"CreateWorkspaceResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TwinMakerArn\"\n        },\n        {\n          \"description\": \"The ARN of the workspace.\"\n        }\n      ]\n    },\n    \"creationDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when the workspace was created.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\",\n    \"creationDateTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-create-workspace-response-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: CreateWorkspaceResponse
---
