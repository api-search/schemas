---
description: A node interface.
layout: schema
name: NodeInterface
properties_list:
- description: ''
  name: Inputs
  type: object
- description: ''
  name: Outputs
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-node-interface-schema.json
slug: openapi-node-interface
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-node-interface-schema.json\",\n  \"title\": \"NodeInterface\",\n  \"description\": \"A node interface.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Inputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputPortList\"\n        },\n        {\n          \"description\": \"The node interface's inputs.\"\n        }\n      ]\n    },\n    \"Outputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputPortList\"\n        },\n        {\n          \"description\": \"The node interface's outputs.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Inputs\",\n    \"Outputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-node-interface-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: NodeInterface
---
