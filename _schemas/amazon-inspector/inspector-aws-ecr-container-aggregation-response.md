---
description: An aggregation of information about Amazon ECR containers.
layout: schema
name: AwsEcrContainerAggregationResponse
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: architecture
  type: object
- description: ''
  name: imageSha
  type: object
- description: ''
  name: imageTags
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
schema_file: json-schema/inspector-aws-ecr-container-aggregation-response-schema.json
slug: inspector-aws-ecr-container-aggregation-response
source_filename: inspector-aws-ecr-container-aggregation-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-aws-ecr-container-aggregation-response-schema.json\",\n  \"title\": \"AwsEcrContainerAggregationResponse\",\n  \"description\": \"An aggregation of information about Amazon ECR containers.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID of the account that owns the container.\"\n        }\n      ]\n    },\n    \"architecture\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The architecture of the container.\"\n        }\n      ]\n    },\n    \"imageSha\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The SHA value of the container image.\"\n        }\n      ]\n    },\n    \"imageTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\n        },\n        {\n          \"description\": \"The container image stags.\"\n        }\n      ]\n    },\n    \"repository\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The container repository.\"\n        }\n      ]\n    },\n    \"resourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The resource ID of the container.\"\n        }\n      ]\n    },\n    \"severityCounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SeverityCounts\"\n        },\n        {\n          \"description\": \"The number\
  \ of finding by severity.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"resourceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-aws-ecr-container-aggregation-response-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: AwsEcrContainerAggregationResponse
---
