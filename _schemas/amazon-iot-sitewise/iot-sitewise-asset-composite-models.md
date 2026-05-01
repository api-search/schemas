---
description: AssetCompositeModels schema
layout: schema
name: AssetCompositeModels
properties_list: []
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-asset-composite-models-schema.json
slug: iot-sitewise-asset-composite-models
source_filename: iot-sitewise-asset-composite-models-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-composite-models-schema.json\",\n  \"title\": \"AssetCompositeModels\",\n  \"description\": \"AssetCompositeModels schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"name\",\n      \"type\",\n      \"properties\"\n    ],\n    \"properties\": {\n      \"name\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Name\"\n          },\n          {\n            \"description\": \"The name of the composite model.\"\n          }\n        ]\n      },\n      \"description\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Description\"\n          },\n          {\n            \"description\": \"The description of the composite model.\"\n          }\n        ]\n      },\n\
  \      \"type\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Name\"\n          },\n          {\n            \"description\": \"The type of the composite model. For alarm composite models, this type is <code>AWS/ALARM</code>.\"\n          }\n        ]\n      },\n      \"properties\": {\n        \"description\": \"The asset properties that this composite model defines.\"\n      },\n      \"id\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ID\"\n          },\n          {\n            \"description\": \" The ID of the asset composite model. \"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains information about a composite model in an asset. This object contains the asset's properties that you define in the composite model.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-composite-models-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: AssetCompositeModels
---
