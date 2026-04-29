---
description: UpdateWorkspaceRequest schema
layout: schema
name: UpdateWorkspaceRequest
properties_list:
- description: ''
  name: description
  type: object
- description: ''
  name: role
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-update-workspace-request-schema.json
slug: iot-twinmaker-update-workspace-request
source_filename: iot-twinmaker-update-workspace-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-update-workspace-request-schema.json\",\n  \"title\": \"UpdateWorkspaceRequest\",\n  \"description\": \"UpdateWorkspaceRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description of the workspace.\"\n        }\n      ]\n    },\n    \"role\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The ARN of the execution role associated with the workspace.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-update-workspace-request-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: UpdateWorkspaceRequest
---
