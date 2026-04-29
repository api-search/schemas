---
description: The file format of the data.
layout: schema
name: FileFormat
properties_list:
- description: ''
  name: csv
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-file-format-schema.json
slug: iot-sitewise-file-format
source_filename: iot-sitewise-file-format-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-file-format-schema.json\",\n  \"title\": \"FileFormat\",\n  \"description\": \"The file format of the data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"csv\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Csv\"\n        },\n        {\n          \"description\": \"The .csv file format.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-file-format-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: FileFormat
---
