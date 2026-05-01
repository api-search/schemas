---
description: Rows schema
layout: schema
name: Rows
properties_list: []
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-rows-schema.json
slug: iot-twinmaker-rows
source_filename: iot-twinmaker-rows-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-rows-schema.json\",\n  \"title\": \"Rows\",\n  \"description\": \"Rows schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"rowData\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/RowData\"\n          },\n          {\n            \"description\": \"The data in a row of query results.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Represents a single row in the query results.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-rows-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: Rows
---
