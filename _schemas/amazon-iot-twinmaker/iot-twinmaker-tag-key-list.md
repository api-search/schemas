---
description: TagKeyList schema
layout: schema
name: TagKeyList
properties_list: []
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-tag-key-list-schema.json
slug: iot-twinmaker-tag-key-list
source_filename: iot-twinmaker-tag-key-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-tag-key-list-schema.json\",\n  \"title\": \"TagKeyList\",\n  \"description\": \"TagKeyList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"pattern\": \"([\\\\p{L}\\\\p{Z}\\\\p{N}_.:/=+\\\\-@]*)\",\n    \"minLength\": 1,\n    \"maxLength\": 128\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-tag-key-list-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: TagKeyList
---
