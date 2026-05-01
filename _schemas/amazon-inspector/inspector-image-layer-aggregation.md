---
description: The details that define an aggregation based on container image layers.
layout: schema
name: ImageLayerAggregation
properties_list:
- description: ''
  name: layerHashes
  type: object
- description: ''
  name: repositories
  type: object
- description: ''
  name: resourceIds
  type: object
- description: ''
  name: sortBy
  type: object
- description: ''
  name: sortOrder
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-image-layer-aggregation-schema.json
slug: inspector-image-layer-aggregation
source_filename: inspector-image-layer-aggregation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-image-layer-aggregation-schema.json\",\n  \"title\": \"ImageLayerAggregation\",\n  \"description\": \"The details that define an aggregation based on container image layers.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"layerHashes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"The hashes associated with the layers.\"\n        }\n      ]\n    },\n    \"repositories\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"The repository associated with the container image hosting the layers.\"\n        }\n      ]\n    },\n    \"resourceIds\": {\n      \"allOf\": [\n        {\n         \
  \ \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"The ID of the container image layer.\"\n        }\n      ]\n    },\n    \"sortBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageLayerSortBy\"\n        },\n        {\n          \"description\": \"The value to sort results by.\"\n        }\n      ]\n    },\n    \"sortOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortOrder\"\n        },\n        {\n          \"description\": \"The order to sort results by.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-image-layer-aggregation-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: ImageLayerAggregation
---
