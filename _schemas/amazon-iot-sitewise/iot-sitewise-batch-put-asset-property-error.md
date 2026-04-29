---
description: Contains error information from updating a batch of asset property values.
layout: schema
name: BatchPutAssetPropertyError
properties_list:
- description: ''
  name: errorCode
  type: object
- description: ''
  name: errorMessage
  type: object
- description: ''
  name: timestamps
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-batch-put-asset-property-error-schema.json
slug: iot-sitewise-batch-put-asset-property-error
source_filename: iot-sitewise-batch-put-asset-property-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-put-asset-property-error-schema.json\",\n  \"title\": \"BatchPutAssetPropertyError\",\n  \"description\": \"Contains error information from updating a batch of asset property values.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchPutAssetPropertyValueErrorCode\"\n        },\n        {\n          \"description\": \"The error code.\"\n        }\n      ]\n    },\n    \"errorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorMessage\"\n        },\n        {\n          \"description\": \"The associated error message.\"\n        }\n      ]\n    },\n    \"timestamps\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamps\"\
  \n        },\n        {\n          \"description\": \"A list of timestamps for each error, if any.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"errorCode\",\n    \"errorMessage\",\n    \"timestamps\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-put-asset-property-error-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: BatchPutAssetPropertyError
---
