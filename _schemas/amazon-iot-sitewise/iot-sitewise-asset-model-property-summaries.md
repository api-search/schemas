---
description: AssetModelPropertySummaries schema
layout: schema
name: AssetModelPropertySummaries
properties_list: []
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-asset-model-property-summaries-schema.json
slug: iot-sitewise-asset-model-property-summaries
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-model-property-summaries-schema.json\",\n  \"title\": \"AssetModelPropertySummaries\",\n  \"description\": \"AssetModelPropertySummaries schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"name\",\n      \"dataType\",\n      \"type\"\n    ],\n    \"properties\": {\n      \"id\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ID\"\n          },\n          {\n            \"description\": \"The ID of the property.\"\n          }\n        ]\n      },\n      \"name\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Name\"\n          },\n          {\n            \"description\": \"The name of the property.\"\n          }\n        ]\n      },\n      \"dataType\"\
  : {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/PropertyDataType\"\n          },\n          {\n            \"description\": \"The data type of the property.\"\n          }\n        ]\n      },\n      \"dataTypeSpec\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Name\"\n          },\n          {\n            \"description\": \"The data type of the structure for this property. This parameter exists on properties that have the <code>STRUCT</code> data type.\"\n          }\n        ]\n      },\n      \"unit\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/PropertyUnit\"\n          },\n          {\n            \"description\": \"The unit (such as <code>Newtons</code> or <code>RPM</code>) of the property.\"\n          }\n        ]\n      },\n      \"type\": {\n        \"$ref\": \"#/components/schemas/PropertyType\"\n      },\n      \"assetModelCompositeModelId\": {\n        \"allOf\"\
  : [\n          {\n            \"$ref\": \"#/components/schemas/ID\"\n          },\n          {\n            \"description\": \" The ID of the composite model that contains the asset model property. \"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains a summary of a property associated with a model.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-model-property-summaries-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: AssetModelPropertySummaries
---
