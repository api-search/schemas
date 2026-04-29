---
description: Contains current status information for an asset model. For more information, see <a href="https://docs.aws.amazon.com/iot-sitewise/latest/userguide/asset-and-model-states.html">Asset and model states</a> in the <i>IoT SiteWise User Guide</i>.
layout: schema
name: AssetModelStatus
properties_list:
- description: ''
  name: state
  type: object
- description: ''
  name: error
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-asset-model-status-schema.json
slug: iot-sitewise-asset-model-status
source_filename: iot-sitewise-asset-model-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-model-status-schema.json\",\n  \"title\": \"AssetModelStatus\",\n  \"description\": \"Contains current status information for an asset model. For more information, see <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/userguide/asset-and-model-states.html\\\">Asset and model states</a> in the <i>IoT SiteWise User Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"state\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetModelState\"\n        },\n        {\n          \"description\": \"The current state of the asset model.\"\n        }\n      ]\n    },\n    \"error\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorDetails\"\n        },\n        {\n          \"description\": \"Contains associated\
  \ error information, if any.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"state\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-model-status-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: AssetModelStatus
---
