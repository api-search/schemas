---
description: Contains information about a composite model in an asset model. This object contains the asset property definitions that you define in the composite model.
layout: schema
name: AssetModelCompositeModel
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: type
  type: object
- description: The asset property definitions for this composite model.
  name: properties
  type: object
- description: ''
  name: id
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-asset-model-composite-model-schema.json
slug: iot-sitewise-asset-model-composite-model
source_filename: iot-sitewise-asset-model-composite-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-model-composite-model-schema.json\",\n  \"title\": \"AssetModelCompositeModel\",\n  \"description\": \"Contains information about a composite model in an asset model. This object contains the asset property definitions that you define in the composite model.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the composite model.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description of the composite model.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The type of the composite model. For alarm composite models, this type is <code>AWS/ALARM</code>.\"\n        }\n      ]\n    },\n    \"properties\": {\n      \"description\": \"The asset property definitions for this composite model.\"\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \" The ID of the asset model composite model. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-model-composite-model-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: AssetModelCompositeModel
---
