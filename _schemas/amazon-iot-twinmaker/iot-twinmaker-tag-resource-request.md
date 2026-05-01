---
description: TagResourceRequest schema
layout: schema
name: TagResourceRequest
properties_list:
- description: ''
  name: resourceARN
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-tag-resource-request-schema.json
slug: iot-twinmaker-tag-resource-request
source_filename: iot-twinmaker-tag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-tag-resource-request-schema.json\",\n  \"title\": \"TagResourceRequest\",\n  \"description\": \"TagResourceRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TwinMakerArn\"\n        },\n        {\n          \"description\": \"The ARN of the resource.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Metadata to add to this resource.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"resourceARN\",\n    \"tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-tag-resource-request-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: TagResourceRequest
---
