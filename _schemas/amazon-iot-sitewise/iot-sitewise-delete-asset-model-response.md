---
description: DeleteAssetModelResponse schema
layout: schema
name: DeleteAssetModelResponse
properties_list:
- description: ''
  name: assetModelStatus
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-delete-asset-model-response-schema.json
slug: iot-sitewise-delete-asset-model-response
source_filename: iot-sitewise-delete-asset-model-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-delete-asset-model-response-schema.json\",\n  \"title\": \"DeleteAssetModelResponse\",\n  \"description\": \"DeleteAssetModelResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetModelStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetModelStatus\"\n        },\n        {\n          \"description\": \"The status of the asset model, which contains a state (<code>DELETING</code> after successfully calling this operation) and any error message.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"assetModelStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-delete-asset-model-response-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: DeleteAssetModelResponse
---
