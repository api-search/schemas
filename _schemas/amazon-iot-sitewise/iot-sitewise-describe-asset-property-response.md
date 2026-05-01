---
description: DescribeAssetPropertyResponse schema
layout: schema
name: DescribeAssetPropertyResponse
properties_list:
- description: ''
  name: assetId
  type: object
- description: ''
  name: assetName
  type: object
- description: ''
  name: assetModelId
  type: object
- description: ''
  name: assetProperty
  type: object
- description: ''
  name: compositeModel
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-describe-asset-property-response-schema.json
slug: iot-sitewise-describe-asset-property-response
source_filename: iot-sitewise-describe-asset-property-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-describe-asset-property-response-schema.json\",\n  \"title\": \"DescribeAssetPropertyResponse\",\n  \"description\": \"DescribeAssetPropertyResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the asset.\"\n        }\n      ]\n    },\n    \"assetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the asset.\"\n        }\n      ]\n    },\n    \"assetModelId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the asset\
  \ model.\"\n        }\n      ]\n    },\n    \"assetProperty\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Property\"\n        },\n        {\n          \"description\": \"<p>The asset property's definition, alias, and notification state.</p> <p>This response includes this object for normal asset properties. If you describe an asset property in a composite model, this response includes the asset property information in <code>compositeModel</code>.</p>\"\n        }\n      ]\n    },\n    \"compositeModel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CompositeModelProperty\"\n        },\n        {\n          \"description\": \"The composite asset model that declares this asset property, if this asset property exists in a composite model.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"assetId\",\n    \"assetName\",\n    \"assetModelId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-describe-asset-property-response-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: DescribeAssetPropertyResponse
---
