---
description: A response that contains the results of a finding aggregation by image layer.
layout: schema
name: ImageLayerAggregationResponse
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: layerHash
  type: object
- description: ''
  name: repository
  type: object
- description: ''
  name: resourceId
  type: object
- description: ''
  name: severityCounts
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-image-layer-aggregation-response-schema.json
slug: inspector-image-layer-aggregation-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-image-layer-aggregation-response-schema.json\",\n  \"title\": \"ImageLayerAggregationResponse\",\n  \"description\": \"A response that contains the results of a finding aggregation by image layer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services account that owns the container image hosting the layer image.\"\n        }\n      ]\n    },\n    \"layerHash\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The layer hash.\"\n        }\n      ]\n    },\n    \"repository\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The repository the layer resides in.\"\n        }\n      ]\n    },\n    \"resourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The resource ID of the container image layer.\"\n        }\n      ]\n    },\n    \"severityCounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SeverityCounts\"\n        },\n        {\n          \"description\": \"An object that represents the count of matched findings per severity.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"accountId\",\n    \"layerHash\",\n    \"repository\",\n    \"resourceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-image-layer-aggregation-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: ImageLayerAggregationResponse
---
