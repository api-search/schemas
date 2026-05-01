---
description: AssetModelProperties schema
layout: schema
name: AssetModelProperties
properties_list: []
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-asset-model-properties-schema.json
slug: iot-sitewise-asset-model-properties
source_filename: iot-sitewise-asset-model-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-model-properties-schema.json\",\n  \"title\": \"AssetModelProperties\",\n  \"description\": \"AssetModelProperties schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"name\",\n      \"dataType\",\n      \"type\"\n    ],\n    \"properties\": {\n      \"id\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ID\"\n          },\n          {\n            \"description\": \"The ID of the asset model property.\"\n          }\n        ]\n      },\n      \"name\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Name\"\n          },\n          {\n            \"description\": \"The name of the asset model property.\"\n          }\n        ]\n      },\n      \"dataType\"\
  : {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/PropertyDataType\"\n          },\n          {\n            \"description\": \"The data type of the asset model property.\"\n          }\n        ]\n      },\n      \"dataTypeSpec\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Name\"\n          },\n          {\n            \"description\": \"The data type of the structure for this property. This parameter exists on properties that have the <code>STRUCT</code> data type.\"\n          }\n        ]\n      },\n      \"unit\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/PropertyUnit\"\n          },\n          {\n            \"description\": \"The unit of the asset model property, such as <code>Newtons</code> or <code>RPM</code>.\"\n          }\n        ]\n      },\n      \"type\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/PropertyType\"\n  \
  \        },\n          {\n            \"description\": \"The property type (see <code>PropertyType</code>).\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains information about an asset model property.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-model-properties-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: AssetModelProperties
---
