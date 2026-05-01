---
description: AssetHierarchies schema
layout: schema
name: AssetHierarchies
properties_list: []
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-asset-hierarchies-schema.json
slug: iot-sitewise-asset-hierarchies
source_filename: iot-sitewise-asset-hierarchies-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-hierarchies-schema.json\",\n  \"title\": \"AssetHierarchies\",\n  \"description\": \"AssetHierarchies schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"name\"\n    ],\n    \"properties\": {\n      \"id\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ID\"\n          },\n          {\n            \"description\": \"The ID of the hierarchy. This ID is a <code>hierarchyId</code>.\"\n          }\n        ]\n      },\n      \"name\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Name\"\n          },\n          {\n            \"description\": \"The hierarchy name provided in the <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_CreateAssetModel.html\\\
  \">CreateAssetModel</a> or <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_UpdateAssetModel.html\\\">UpdateAssetModel</a> API operation.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Describes an asset hierarchy that contains a hierarchy's name and ID.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-hierarchies-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: AssetHierarchies
---
