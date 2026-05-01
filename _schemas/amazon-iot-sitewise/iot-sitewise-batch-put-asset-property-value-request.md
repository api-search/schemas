---
description: BatchPutAssetPropertyValueRequest schema
layout: schema
name: BatchPutAssetPropertyValueRequest
properties_list:
- description: ''
  name: entries
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-batch-put-asset-property-value-request-schema.json
slug: iot-sitewise-batch-put-asset-property-value-request
source_filename: iot-sitewise-batch-put-asset-property-value-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-put-asset-property-value-request-schema.json\",\n  \"title\": \"BatchPutAssetPropertyValueRequest\",\n  \"description\": \"BatchPutAssetPropertyValueRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PutAssetPropertyValueEntries\"\n        },\n        {\n          \"description\": \"The list of asset property value entries for the batch put request. You can specify up to 10 entries per request.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"entries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-put-asset-property-value-request-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: BatchPutAssetPropertyValueRequest
---
