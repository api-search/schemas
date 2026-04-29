---
description: Contains an image file.
layout: schema
name: ImageFile
properties_list:
- description: ''
  name: data
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-image-file-schema.json
slug: iot-sitewise-image-file
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-image-file-schema.json\",\n  \"title\": \"ImageFile\",\n  \"description\": \"Contains an image file.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageFileData\"\n        },\n        {\n          \"description\": \"The image file contents, represented as a base64-encoded string. The file size must be less than 1 MB.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageFileType\"\n        },\n        {\n          \"description\": \"The file type of the image.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"data\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-image-file-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: ImageFile
---
