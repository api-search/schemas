---
description: GetAssetPropertyValueResponse schema
layout: schema
name: GetAssetPropertyValueResponse
properties_list:
- description: ''
  name: propertyValue
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-get-asset-property-value-response-schema.json
slug: iot-sitewise-get-asset-property-value-response
source_filename: iot-sitewise-get-asset-property-value-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-get-asset-property-value-response-schema.json\",\n  \"title\": \"GetAssetPropertyValueResponse\",\n  \"description\": \"GetAssetPropertyValueResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"propertyValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetPropertyValue\"\n        },\n        {\n          \"description\": \"The current asset property value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-get-asset-property-value-response-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: GetAssetPropertyValueResponse
---
