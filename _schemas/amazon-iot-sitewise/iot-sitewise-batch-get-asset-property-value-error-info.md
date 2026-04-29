---
description: The error information, such as the error code and the timestamp.
layout: schema
name: BatchGetAssetPropertyValueErrorInfo
properties_list:
- description: ''
  name: errorCode
  type: object
- description: ''
  name: errorTimestamp
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-batch-get-asset-property-value-error-info-schema.json
slug: iot-sitewise-batch-get-asset-property-value-error-info
source_filename: iot-sitewise-batch-get-asset-property-value-error-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-get-asset-property-value-error-info-schema.json\",\n  \"title\": \"BatchGetAssetPropertyValueErrorInfo\",\n  \"description\": \"The error information, such as the error code and the timestamp.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchGetAssetPropertyValueErrorCode\"\n        },\n        {\n          \"description\": \"The error code.\"\n        }\n      ]\n    },\n    \"errorTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the error occurred, in Unix epoch time.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"errorCode\",\n    \"errorTimestamp\"\n\
  \  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-get-asset-property-value-error-info-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: BatchGetAssetPropertyValueErrorInfo
---
