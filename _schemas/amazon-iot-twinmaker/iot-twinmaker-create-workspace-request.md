---
description: CreateWorkspaceRequest schema
layout: schema
name: CreateWorkspaceRequest
properties_list:
- description: ''
  name: description
  type: object
- description: ''
  name: s3Location
  type: object
- description: ''
  name: role
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-create-workspace-request-schema.json
slug: iot-twinmaker-create-workspace-request
source_filename: iot-twinmaker-create-workspace-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-create-workspace-request-schema.json\",\n  \"title\": \"CreateWorkspaceRequest\",\n  \"description\": \"CreateWorkspaceRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description of the workspace.\"\n        }\n      ]\n    },\n    \"s3Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Location\"\n        },\n        {\n          \"description\": \"The ARN of the S3 bucket where resources associated with the workspace are stored.\"\n        }\n      ]\n    },\n    \"role\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n\
  \        },\n        {\n          \"description\": \"The ARN of the execution role associated with the workspace.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Metadata that you can use to manage the workspace\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"s3Location\",\n    \"role\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-create-workspace-request-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: CreateWorkspaceRequest
---
