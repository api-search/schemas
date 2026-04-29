---
description: Information about a line item asset.
layout: schema
name: LineItemAssetInformation
properties_list:
- description: ''
  name: AssetId
  type: object
- description: ''
  name: MacAddressList
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-line-item-asset-information-schema.json
slug: openapi-line-item-asset-information
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-line-item-asset-information-schema.json\",\n  \"title\": \"LineItemAssetInformation\",\n  \"description\": \" Information about a line item asset. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AssetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetId\"\n        },\n        {\n          \"description\": \" The ID of the asset. \"\n        }\n      ]\n    },\n    \"MacAddressList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MacAddressList\"\n        },\n        {\n          \"description\": \" The MAC addresses of the asset. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-line-item-asset-information-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: LineItemAssetInformation
---
