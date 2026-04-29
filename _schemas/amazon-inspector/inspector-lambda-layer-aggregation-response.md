---
description: A response that contains the results of an AWS Lambda function layer finding aggregation.
layout: schema
name: LambdaLayerAggregationResponse
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: functionName
  type: object
- description: ''
  name: layerArn
  type: object
- description: ''
  name: resourceId
  type: object
- description: An object that contains the counts of aggregated finding per severity.
  name: severityCounts
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-lambda-layer-aggregation-response-schema.json
slug: inspector-lambda-layer-aggregation-response
source_filename: inspector-lambda-layer-aggregation-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-lambda-layer-aggregation-response-schema.json\",\n  \"title\": \"LambdaLayerAggregationResponse\",\n  \"description\": \"A response that contains the results of an AWS Lambda function layer finding aggregation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The account ID of the AWS Lambda function layer.\"\n        }\n      ]\n    },\n    \"functionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The names of the AWS Lambda functions associated with the layers.\"\n        }\n      ]\n    },\n    \"layerArn\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the AWS Lambda function layer.\"\n        }\n      ]\n    },\n    \"resourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The Resource ID of the AWS Lambda function layer.\"\n        }\n      ]\n    },\n    \"severityCounts\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"all\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Long\"\n            },\n            {\n              \"description\": \"The total count of findings from all severities.\"\n            }\n          ]\n        },\n        \"critical\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Long\"\n            },\n            {\n              \"description\"\
  : \"The total count of critical severity findings.\"\n            }\n          ]\n        },\n        \"high\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Long\"\n            },\n            {\n              \"description\": \"The total count of high severity findings.\"\n            }\n          ]\n        },\n        \"medium\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Long\"\n            },\n            {\n              \"description\": \"The total count of medium severity findings.\"\n            }\n          ]\n        }\n      },\n      \"description\": \"An object that contains the counts of aggregated finding per severity.\"\n    }\n  },\n  \"required\": [\n    \"accountId\",\n    \"functionName\",\n    \"layerArn\",\n    \"resourceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-lambda-layer-aggregation-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: LambdaLayerAggregationResponse
---
