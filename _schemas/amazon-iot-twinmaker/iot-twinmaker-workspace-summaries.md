---
description: WorkspaceSummaries schema
layout: schema
name: WorkspaceSummaries
properties_list: []
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-workspace-summaries-schema.json
slug: iot-twinmaker-workspace-summaries
source_filename: iot-twinmaker-workspace-summaries-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-workspace-summaries-schema.json\",\n  \"title\": \"WorkspaceSummaries\",\n  \"description\": \"WorkspaceSummaries schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"workspaceId\",\n      \"arn\",\n      \"creationDateTime\",\n      \"updateDateTime\"\n    ],\n    \"properties\": {\n      \"workspaceId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Id\"\n          },\n          {\n            \"description\": \"The ID of the workspace.\"\n          }\n        ]\n      },\n      \"arn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/TwinMakerArn\"\n          },\n          {\n            \"description\": \"The ARN of the workspace.\"\n          }\n        ]\n\
  \      },\n      \"description\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Description\"\n          },\n          {\n            \"description\": \"The description of the workspace.\"\n          }\n        ]\n      },\n      \"creationDateTime\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Timestamp\"\n          },\n          {\n            \"description\": \"The date and time when the workspace was created.\"\n          }\n        ]\n      },\n      \"updateDateTime\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Timestamp\"\n          },\n          {\n            \"description\": \"The date and time when the workspace was last updated.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"An object that contains information about a workspace.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-workspace-summaries-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: WorkspaceSummaries
---
