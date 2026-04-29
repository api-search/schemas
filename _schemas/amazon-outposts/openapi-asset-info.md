---
description: Information about hardware assets.
layout: schema
name: AssetInfo
properties_list:
- description: ''
  name: AssetId
  type: object
- description: ''
  name: RackId
  type: object
- description: ''
  name: AssetType
  type: object
- description: ''
  name: ComputeAttributes
  type: object
- description: ''
  name: AssetLocation
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-asset-info-schema.json
slug: openapi-asset-info
source_filename: openapi-asset-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-asset-info-schema.json\",\n  \"title\": \"AssetInfo\",\n  \"description\": \" Information about hardware assets. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AssetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetId\"\n        },\n        {\n          \"description\": \" The ID of the asset. \"\n        }\n      ]\n    },\n    \"RackId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RackId\"\n        },\n        {\n          \"description\": \" The rack ID of the asset. \"\n        }\n      ]\n    },\n    \"AssetType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetType\"\n        },\n        {\n          \"description\": \" The type of the asset. \"\n        }\n      ]\n    },\n\
  \    \"ComputeAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputeAttributes\"\n        },\n        {\n          \"description\": \" Information about compute hardware assets. \"\n        }\n      ]\n    },\n    \"AssetLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetLocation\"\n        },\n        {\n          \"description\": \" The position of an asset in a rack. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-asset-info-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: AssetInfo
---
