---
description: A signal to a camera node to start or stop processing video.
layout: schema
name: NodeSignal
properties_list:
- description: ''
  name: NodeInstanceId
  type: object
- description: ''
  name: Signal
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-node-signal-schema.json
slug: openapi-node-signal
source_filename: openapi-node-signal-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-node-signal-schema.json\",\n  \"title\": \"NodeSignal\",\n  \"description\": \"A signal to a camera node to start or stop processing video.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NodeInstanceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeInstanceId\"\n        },\n        {\n          \"description\": \"The camera node's name, from the application manifest.\"\n        }\n      ]\n    },\n    \"Signal\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeSignalValue\"\n        },\n        {\n          \"description\": \"The signal value.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"NodeInstanceId\",\n    \"Signal\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-node-signal-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: NodeSignal
---
