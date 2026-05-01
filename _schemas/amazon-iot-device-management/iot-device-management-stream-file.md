---
description: Represents a file to stream.
layout: schema
name: StreamFile
properties_list:
- description: ''
  name: fileId
  type: object
- description: ''
  name: s3Location
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-stream-file-schema.json
slug: iot-device-management-stream-file
source_filename: iot-device-management-stream-file-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-stream-file-schema.json\",\n  \"title\": \"StreamFile\",\n  \"description\": \"Represents a file to stream.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fileId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileId\"\n        },\n        {\n          \"description\": \"The file ID.\"\n        }\n      ]\n    },\n    \"s3Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Location\"\n        },\n        {\n          \"description\": \"The location of the file in S3.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-stream-file-schema.json
tags:
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: StreamFile
---
