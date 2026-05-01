---
description: The details that define a findings aggregation based on an AWS Lambda function's layers.
layout: schema
name: LambdaLayerAggregation
properties_list:
- description: ''
  name: functionNames
  type: object
- description: ''
  name: layerArns
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
schema_file: json-schema/inspector-lambda-layer-aggregation-schema.json
slug: inspector-lambda-layer-aggregation
source_filename: inspector-lambda-layer-aggregation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-lambda-layer-aggregation-schema.json\",\n  \"title\": \"LambdaLayerAggregation\",\n  \"description\": \"The details that define a findings aggregation based on an AWS Lambda function's layers.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"functionNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"The names of the AWS Lambda functions associated with the layers.\"\n        }\n      ]\n    },\n    \"layerArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the AWS Lambda function layer. \"\n        }\n      ]\n    },\n    \"resourceIds\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"The resource IDs for the AWS Lambda function layers.\"\n        }\n      ]\n    },\n    \"sortBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaLayerSortBy\"\n        },\n        {\n          \"description\": \"The finding severity to use for sorting the results.\"\n        }\n      ]\n    },\n    \"sortOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortOrder\"\n        },\n        {\n          \"description\": \"The order to use for sorting the results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-lambda-layer-aggregation-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: LambdaLayerAggregation
---
