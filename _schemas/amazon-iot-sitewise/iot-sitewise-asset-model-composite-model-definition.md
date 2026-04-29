---
description: Contains a composite model definition in an asset model. This composite model definition is applied to all assets created from the asset model.
layout: schema
name: AssetModelCompositeModelDefinition
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
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-asset-model-composite-model-definition-schema.json
slug: iot-sitewise-asset-model-composite-model-definition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-model-composite-model-definition-schema.json\",\n  \"title\": \"AssetModelCompositeModelDefinition\",\n  \"description\": \"Contains a composite model definition in an asset model. This composite model definition is applied to all assets created from the asset model.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the composite model.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description of the composite model.\"\n        }\n      ]\n    },\n    \"type\": {\n   \
  \   \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The type of the composite model. For alarm composite models, this type is <code>AWS/ALARM</code>.\"\n        }\n      ]\n    },\n    \"properties\": {\n      \"description\": \"The asset property definitions for this composite model.\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-model-composite-model-definition-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: AssetModelCompositeModelDefinition
---
