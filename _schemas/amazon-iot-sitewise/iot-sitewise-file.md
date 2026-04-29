---
description: The file in Amazon S3 where your data is saved.
layout: schema
name: File
properties_list:
- description: ''
  name: bucket
  type: object
- description: ''
  name: key
  type: object
- description: ''
  name: versionId
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-file-schema.json
slug: iot-sitewise-file
source_filename: iot-sitewise-file-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-file-schema.json\",\n  \"title\": \"File\",\n  \"description\": \"The file in Amazon S3 where your data is saved. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Bucket\"\n        },\n        {\n          \"description\": \"The name of the Amazon S3 bucket from which data is imported.\"\n        }\n      ]\n    },\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The key of the Amazon S3 object that contains your data. Each object has a key that is a unique identifier. Each object has exactly one key.\"\n        }\n      ]\n    },\n    \"versionId\": {\n      \"allOf\": [\n        {\n     \
  \     \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The version ID to identify a specific version of the Amazon S3 object that contains your data.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"bucket\",\n    \"key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-file-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: File
---
