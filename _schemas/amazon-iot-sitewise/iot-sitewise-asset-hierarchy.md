---
description: Describes an asset hierarchy that contains a hierarchy's name and ID.
layout: schema
name: AssetHierarchy
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: name
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-asset-hierarchy-schema.json
slug: iot-sitewise-asset-hierarchy
source_filename: iot-sitewise-asset-hierarchy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-hierarchy-schema.json\",\n  \"title\": \"AssetHierarchy\",\n  \"description\": \"Describes an asset hierarchy that contains a hierarchy's name and ID.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the hierarchy. This ID is a <code>hierarchyId</code>.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The hierarchy name provided in the <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_CreateAssetModel.html\\\">CreateAssetModel</a> or <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_UpdateAssetModel.html\\\
  \">UpdateAssetModel</a> API operation.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-hierarchy-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: AssetHierarchy
---
