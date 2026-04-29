---
description: A response that contains the results of an AWS Lambda function finding aggregation.
layout: schema
name: LambdaFunctionAggregationResponse
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: functionName
  type: object
- description: ''
  name: lambdaTags
  type: object
- description: ''
  name: lastModifiedAt
  type: object
- description: ''
  name: resourceId
  type: object
- description: ''
  name: runtime
  type: object
- description: An object that contains the counts of aggregated finding per severity.
  name: severityCounts
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-lambda-function-aggregation-response-schema.json
slug: inspector-lambda-function-aggregation-response
source_filename: inspector-lambda-function-aggregation-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-lambda-function-aggregation-response-schema.json\",\n  \"title\": \"LambdaFunctionAggregationResponse\",\n  \"description\": \"A response that contains the results of an AWS Lambda function finding aggregation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The ID of the AWS account that owns the AWS Lambda function. \"\n        }\n      ]\n    },\n    \"functionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The AWS Lambda function names included in the aggregation results.\"\n        }\n      ]\n    },\n    \"lambdaTags\": {\n    \
  \  \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags included in the aggregation results.\"\n        }\n      ]\n    },\n    \"lastModifiedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTimeTimestamp\"\n        },\n        {\n          \"description\": \"The date that the AWS Lambda function included in the aggregation results was last changed.\"\n        }\n      ]\n    },\n    \"resourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The resource IDs included in the aggregation results.\"\n        }\n      ]\n    },\n    \"runtime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The runtimes included in the aggregation results.\"\n        }\n      ]\n    },\n   \
  \ \"severityCounts\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"all\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Long\"\n            },\n            {\n              \"description\": \"The total count of findings from all severities.\"\n            }\n          ]\n        },\n        \"critical\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Long\"\n            },\n            {\n              \"description\": \"The total count of critical severity findings.\"\n            }\n          ]\n        },\n        \"high\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Long\"\n            },\n            {\n              \"description\": \"The total count of high severity findings.\"\n            }\n          ]\n        },\n        \"medium\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Long\"\
  \n            },\n            {\n              \"description\": \"The total count of medium severity findings.\"\n            }\n          ]\n        }\n      },\n      \"description\": \"An object that contains the counts of aggregated finding per severity.\"\n    }\n  },\n  \"required\": [\n    \"resourceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-lambda-function-aggregation-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: LambdaFunctionAggregationResponse
---
