---
description: UpdateWorkspaceResponse schema
layout: schema
name: UpdateWorkspaceResponse
properties_list:
- description: ''
  name: updateDateTime
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-update-workspace-response-schema.json
slug: iot-twinmaker-update-workspace-response
source_filename: iot-twinmaker-update-workspace-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-update-workspace-response-schema.json\",\n  \"title\": \"UpdateWorkspaceResponse\",\n  \"description\": \"UpdateWorkspaceResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"updateDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time of the current update.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"updateDateTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-update-workspace-response-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: UpdateWorkspaceResponse
---
