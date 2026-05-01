---
description: Contains information about a parent asset and a child asset that are related through an asset hierarchy.
layout: schema
name: AssetHierarchyInfo
properties_list:
- description: ''
  name: parentAssetId
  type: object
- description: ''
  name: childAssetId
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-asset-hierarchy-info-schema.json
slug: iot-sitewise-asset-hierarchy-info
source_filename: iot-sitewise-asset-hierarchy-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-hierarchy-info-schema.json\",\n  \"title\": \"AssetHierarchyInfo\",\n  \"description\": \"Contains information about a parent asset and a child asset that are related through an asset hierarchy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"parentAssetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the parent asset in this asset relationship.\"\n        }\n      ]\n    },\n    \"childAssetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the child asset in this asset relationship.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-hierarchy-info-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: AssetHierarchyInfo
---
