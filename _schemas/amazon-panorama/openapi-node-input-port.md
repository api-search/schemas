---
description: A node input port.
layout: schema
name: NodeInputPort
properties_list:
- description: ''
  name: DefaultValue
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: MaxConnections
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-node-input-port-schema.json
slug: openapi-node-input-port
source_filename: openapi-node-input-port-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-node-input-port-schema.json\",\n  \"title\": \"NodeInputPort\",\n  \"description\": \"A node input port.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DefaultValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortDefaultValue\"\n        },\n        {\n          \"description\": \"The input port's default value.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The input port's description.\"\n        }\n      ]\n    },\n    \"MaxConnections\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxConnections\"\n        },\n        {\n          \"description\": \"The input port's max\
  \ connections.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortName\"\n        },\n        {\n          \"description\": \"The input port's name.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortType\"\n        },\n        {\n          \"description\": \"The input port's type.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-node-input-port-schema.json
tags:
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: NodeInputPort
---
