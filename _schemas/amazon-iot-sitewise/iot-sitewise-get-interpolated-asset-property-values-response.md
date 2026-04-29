---
description: GetInterpolatedAssetPropertyValuesResponse schema
layout: schema
name: GetInterpolatedAssetPropertyValuesResponse
properties_list:
- description: ''
  name: interpolatedAssetPropertyValues
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-get-interpolated-asset-property-values-response-schema.json
slug: iot-sitewise-get-interpolated-asset-property-values-response
source_filename: iot-sitewise-get-interpolated-asset-property-values-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-get-interpolated-asset-property-values-response-schema.json\",\n  \"title\": \"GetInterpolatedAssetPropertyValuesResponse\",\n  \"description\": \"GetInterpolatedAssetPropertyValuesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"interpolatedAssetPropertyValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InterpolatedAssetPropertyValues\"\n        },\n        {\n          \"description\": \"The requested interpolated values.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token for the next set of results, or null if there are no additional results.\"\n        }\n      ]\n    }\n  },\n\
  \  \"required\": [\n    \"interpolatedAssetPropertyValues\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-get-interpolated-asset-property-values-response-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: GetInterpolatedAssetPropertyValuesResponse
---
