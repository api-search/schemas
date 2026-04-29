---
description: AssociateAssetsRequest schema
layout: schema
name: AssociateAssetsRequest
properties_list:
- description: ''
  name: hierarchyId
  type: object
- description: ''
  name: childAssetId
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-associate-assets-request-schema.json
slug: iot-sitewise-associate-assets-request
source_filename: iot-sitewise-associate-assets-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-associate-assets-request-schema.json\",\n  \"title\": \"AssociateAssetsRequest\",\n  \"description\": \"AssociateAssetsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hierarchyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of a hierarchy in the parent asset's model. Hierarchies allow different groupings of assets to be formed that all come from the same asset model. For more information, see <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/userguide/asset-hierarchies.html\\\">Asset hierarchies</a> in the <i>IoT SiteWise User Guide</i>.\"\n        }\n      ]\n    },\n    \"childAssetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\
  \n        },\n        {\n          \"description\": \"The ID of the child asset to be associated.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"A unique case-sensitive identifier that you can provide to ensure the idempotency of the request. Don't reuse this client token if a new idempotent request is required.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"hierarchyId\",\n    \"childAssetId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-associate-assets-request-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: AssociateAssetsRequest
---
