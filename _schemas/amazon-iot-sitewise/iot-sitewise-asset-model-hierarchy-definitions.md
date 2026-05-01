---
description: AssetModelHierarchyDefinitions schema
layout: schema
name: AssetModelHierarchyDefinitions
properties_list: []
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-asset-model-hierarchy-definitions-schema.json
slug: iot-sitewise-asset-model-hierarchy-definitions
source_filename: iot-sitewise-asset-model-hierarchy-definitions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-model-hierarchy-definitions-schema.json\",\n  \"title\": \"AssetModelHierarchyDefinitions\",\n  \"description\": \"AssetModelHierarchyDefinitions schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"name\",\n      \"childAssetModelId\"\n    ],\n    \"properties\": {\n      \"name\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Name\"\n          },\n          {\n            \"description\": \"The name of the asset model hierarchy definition (as specified in the <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_CreateAssetModel.html\\\">CreateAssetModel</a> or <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_UpdateAssetModel.html\\\">UpdateAssetModel</a>\
  \ API operation).\"\n          }\n        ]\n      },\n      \"childAssetModelId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ID\"\n          },\n          {\n            \"description\": \"The ID of an asset model for this hierarchy.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains an asset model hierarchy used in asset model creation. An asset model hierarchy determines the kind (or type) of asset that can belong to a hierarchy.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-model-hierarchy-definitions-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: AssetModelHierarchyDefinitions
---
