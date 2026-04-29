---
description: Represents a single row in the query results.
layout: schema
name: Row
properties_list:
- description: ''
  name: rowData
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-row-schema.json
slug: iot-twinmaker-row
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-row-schema.json\",\n  \"title\": \"Row\",\n  \"description\": \"Represents a single row in the query results.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rowData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RowData\"\n        },\n        {\n          \"description\": \"The data in a row of query results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-row-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: Row
---
