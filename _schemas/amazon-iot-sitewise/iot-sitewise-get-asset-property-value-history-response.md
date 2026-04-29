---
description: GetAssetPropertyValueHistoryResponse schema
layout: schema
name: GetAssetPropertyValueHistoryResponse
properties_list:
- description: ''
  name: assetPropertyValueHistory
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-get-asset-property-value-history-response-schema.json
slug: iot-sitewise-get-asset-property-value-history-response
source_filename: iot-sitewise-get-asset-property-value-history-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-get-asset-property-value-history-response-schema.json\",\n  \"title\": \"GetAssetPropertyValueHistoryResponse\",\n  \"description\": \"GetAssetPropertyValueHistoryResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetPropertyValueHistory\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetPropertyValueHistory\"\n        },\n        {\n          \"description\": \"The asset property's value history.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token for the next set of results, or null if there are no additional results.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"assetPropertyValueHistory\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-get-asset-property-value-history-response-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: GetAssetPropertyValueHistoryResponse
---
