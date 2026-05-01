---
description: AssetPropertyValueHistory schema
layout: schema
name: AssetPropertyValueHistory
properties_list: []
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-asset-property-value-history-schema.json
slug: iot-sitewise-asset-property-value-history
source_filename: iot-sitewise-asset-property-value-history-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-property-value-history-schema.json\",\n  \"title\": \"AssetPropertyValueHistory\",\n  \"description\": \"AssetPropertyValueHistory schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"value\",\n      \"timestamp\"\n    ],\n    \"properties\": {\n      \"value\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Variant\"\n          },\n          {\n            \"description\": \"The value of the asset property (see <code>Variant</code>).\"\n          }\n        ]\n      },\n      \"timestamp\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/TimeInNanos\"\n          },\n          {\n            \"description\": \"The timestamp of the asset property value.\"\n\
  \          }\n        ]\n      },\n      \"quality\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Quality\"\n          },\n          {\n            \"description\": \"The quality of the asset property value.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains asset property value information.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-property-value-history-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: AssetPropertyValueHistory
---
