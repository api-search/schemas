---
description: BatchAssociateProjectAssetsRequest schema
layout: schema
name: BatchAssociateProjectAssetsRequest
properties_list:
- description: ''
  name: assetIds
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-batch-associate-project-assets-request-schema.json
slug: iot-sitewise-batch-associate-project-assets-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-associate-project-assets-request-schema.json\",\n  \"title\": \"BatchAssociateProjectAssetsRequest\",\n  \"description\": \"BatchAssociateProjectAssetsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IDs\"\n        },\n        {\n          \"description\": \"The IDs of the assets to be associated to the project.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"A unique case-sensitive identifier that you can provide to ensure the idempotency of the request. Don't reuse this client token if a new idempotent request is required.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"assetIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-associate-project-assets-request-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: BatchAssociateProjectAssetsRequest
---
