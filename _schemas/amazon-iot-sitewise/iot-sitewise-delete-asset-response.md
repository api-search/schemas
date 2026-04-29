---
description: DeleteAssetResponse schema
layout: schema
name: DeleteAssetResponse
properties_list:
- description: ''
  name: assetStatus
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-delete-asset-response-schema.json
slug: iot-sitewise-delete-asset-response
source_filename: iot-sitewise-delete-asset-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-delete-asset-response-schema.json\",\n  \"title\": \"DeleteAssetResponse\",\n  \"description\": \"DeleteAssetResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetStatus\"\n        },\n        {\n          \"description\": \"The status of the asset, which contains a state (<code>DELETING</code> after successfully calling this operation) and any error message.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"assetStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-delete-asset-response-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: DeleteAssetResponse
---
