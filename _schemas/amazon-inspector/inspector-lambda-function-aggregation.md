---
description: The details that define a findings aggregation based on AWS Lambda functions.
layout: schema
name: LambdaFunctionAggregation
properties_list:
- description: ''
  name: functionNames
  type: object
- description: ''
  name: functionTags
  type: object
- description: ''
  name: resourceIds
  type: object
- description: ''
  name: runtimes
  type: object
- description: ''
  name: sortBy
  type: object
- description: ''
  name: sortOrder
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-lambda-function-aggregation-schema.json
slug: inspector-lambda-function-aggregation
source_filename: inspector-lambda-function-aggregation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-lambda-function-aggregation-schema.json\",\n  \"title\": \"LambdaFunctionAggregation\",\n  \"description\": \"The details that define a findings aggregation based on AWS Lambda functions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"functionNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"The AWS Lambda function names to include in the aggregation results.\"\n        }\n      ]\n    },\n    \"functionTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapFilterList\"\n        },\n        {\n          \"description\": \"The tags to include in the aggregation results.\"\n        }\n      ]\n    },\n    \"resourceIds\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"The resource IDs to include in the aggregation results.\"\n        }\n      ]\n    },\n    \"runtimes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"Returns findings aggregated by AWS Lambda function runtime environments.\"\n        }\n      ]\n    },\n    \"sortBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunctionSortBy\"\n        },\n        {\n          \"description\": \"The finding severity to use for sorting the results.\"\n        }\n      ]\n    },\n    \"sortOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortOrder\"\n        },\n        {\n          \"description\": \"The order to use for sorting the results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-lambda-function-aggregation-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: LambdaFunctionAggregation
---
