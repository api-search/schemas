---
description: An application instance's state.
layout: schema
name: ReportedRuntimeContextState
properties_list:
- description: ''
  name: DesiredState
  type: object
- description: ''
  name: DeviceReportedStatus
  type: object
- description: ''
  name: DeviceReportedTime
  type: object
- description: ''
  name: RuntimeContextName
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-reported-runtime-context-state-schema.json
slug: openapi-reported-runtime-context-state
source_filename: openapi-reported-runtime-context-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-reported-runtime-context-state-schema.json\",\n  \"title\": \"ReportedRuntimeContextState\",\n  \"description\": \"An application instance's state.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DesiredState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DesiredState\"\n        },\n        {\n          \"description\": \"The application's desired state.\"\n        }\n      ]\n    },\n    \"DeviceReportedStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceReportedStatus\"\n        },\n        {\n          \"description\": \"The application's reported status.\"\n        }\n      ]\n    },\n    \"DeviceReportedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeStamp\"\n        },\n\
  \        {\n          \"description\": \"When the device reported the application's state.\"\n        }\n      ]\n    },\n    \"RuntimeContextName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuntimeContextName\"\n        },\n        {\n          \"description\": \"The device's name.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DesiredState\",\n    \"DeviceReportedStatus\",\n    \"DeviceReportedTime\",\n    \"RuntimeContextName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-reported-runtime-context-state-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: ReportedRuntimeContextState
---
