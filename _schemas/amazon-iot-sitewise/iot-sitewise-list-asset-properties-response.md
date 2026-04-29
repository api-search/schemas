---
description: ListAssetPropertiesResponse schema
layout: schema
name: ListAssetPropertiesResponse
properties_list:
- description: ''
  name: assetPropertySummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-list-asset-properties-response-schema.json
slug: iot-sitewise-list-asset-properties-response
source_filename: iot-sitewise-list-asset-properties-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-list-asset-properties-response-schema.json\",\n  \"title\": \"ListAssetPropertiesResponse\",\n  \"description\": \"ListAssetPropertiesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetPropertySummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetPropertySummaries\"\n        },\n        {\n          \"description\": \"A list that summarizes the properties associated with the specified asset.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token for the next set of results, or null if there are no additional results.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n   \
  \ \"assetPropertySummaries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-list-asset-properties-response-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: ListAssetPropertiesResponse
---
