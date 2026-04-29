---
description: AssetModelCompositeModels schema
layout: schema
name: AssetModelCompositeModels
properties_list: []
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-asset-model-composite-models-schema.json
slug: iot-sitewise-asset-model-composite-models
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-model-composite-models-schema.json\",\n  \"title\": \"AssetModelCompositeModels\",\n  \"description\": \"AssetModelCompositeModels schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"name\",\n      \"type\"\n    ],\n    \"properties\": {\n      \"name\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Name\"\n          },\n          {\n            \"description\": \"The name of the composite model.\"\n          }\n        ]\n      },\n      \"description\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Description\"\n          },\n          {\n            \"description\": \"The description of the composite model.\"\n          }\n        ]\n      },\n    \
  \  \"type\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Name\"\n          },\n          {\n            \"description\": \"The type of the composite model. For alarm composite models, this type is <code>AWS/ALARM</code>.\"\n          }\n        ]\n      },\n      \"properties\": {\n        \"description\": \"The asset property definitions for this composite model.\"\n      },\n      \"id\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ID\"\n          },\n          {\n            \"description\": \" The ID of the asset model composite model. \"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains information about a composite model in an asset model. This object contains the asset property definitions that you define in the composite model.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-model-composite-models-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: AssetModelCompositeModels
---
