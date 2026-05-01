---
description: A description of the column in the query results.
layout: schema
name: ColumnDescription
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-column-description-schema.json
slug: iot-twinmaker-column-description
source_filename: iot-twinmaker-column-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-column-description-schema.json\",\n  \"title\": \"ColumnDescription\",\n  \"description\": \"A description of the column in the query results.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColumnName\"\n        },\n        {\n          \"description\": \"The name of the column description.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColumnType\"\n        },\n        {\n          \"description\": \"The type of the column description.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-column-description-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: ColumnDescription
---
