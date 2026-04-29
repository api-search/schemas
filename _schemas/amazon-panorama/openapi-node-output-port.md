---
description: A node output port.
layout: schema
name: NodeOutputPort
properties_list:
- description: ''
  name: Description
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-node-output-port-schema.json
slug: openapi-node-output-port
source_filename: openapi-node-output-port-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-node-output-port-schema.json\",\n  \"title\": \"NodeOutputPort\",\n  \"description\": \"A node output port.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The output port's description.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortName\"\n        },\n        {\n          \"description\": \"The output port's name.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortType\"\n        },\n        {\n          \"description\": \"The output port's type.\"\n        }\n      ]\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-node-output-port-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: NodeOutputPort
---
