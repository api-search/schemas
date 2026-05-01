---
description: Details the state of Amazon Inspector for each resource type Amazon Inspector scans.
layout: schema
name: ResourceState
properties_list:
- description: ''
  name: ec2
  type: object
- description: ''
  name: ecr
  type: object
- description: An object that described the state of Amazon Inspector scans for an account.
  name: lambda
  type: object
- description: An object that described the state of Amazon Inspector scans for an account.
  name: lambdaCode
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-resource-state-schema.json
slug: inspector-resource-state
source_filename: inspector-resource-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-resource-state-schema.json\",\n  \"title\": \"ResourceState\",\n  \"description\": \"Details the state of Amazon Inspector for each resource type Amazon Inspector scans.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ec2\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/State\"\n        },\n        {\n          \"description\": \"An object detailing the state of Amazon Inspector scanning for Amazon EC2 resources.\"\n        }\n      ]\n    },\n    \"ecr\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/State\"\n        },\n        {\n          \"description\": \"An object detailing the state of Amazon Inspector scanning for Amazon ECR resources.\"\n        }\n      ]\n    },\n    \"lambda\": {\n      \"type\": \"object\",\n\
  \      \"required\": [\n        \"errorCode\",\n        \"errorMessage\",\n        \"status\"\n      ],\n      \"properties\": {\n        \"errorCode\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/ErrorCode\"\n            },\n            {\n              \"description\": \"The error code explaining why the account failed to enable Amazon Inspector.\"\n            }\n          ]\n        },\n        \"errorMessage\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/NonEmptyString\"\n            },\n            {\n              \"description\": \"The error message received when the account failed to enable Amazon Inspector.\"\n            }\n          ]\n        },\n        \"status\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Status\"\n            },\n            {\n              \"description\": \"The status of Amazon Inspector for the account.\"\n       \
  \     }\n          ]\n        }\n      },\n      \"description\": \"An object that described the state of Amazon Inspector scans for an account.\"\n    },\n    \"lambdaCode\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"errorCode\",\n        \"errorMessage\",\n        \"status\"\n      ],\n      \"properties\": {\n        \"errorCode\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/ErrorCode\"\n            },\n            {\n              \"description\": \"The error code explaining why the account failed to enable Amazon Inspector.\"\n            }\n          ]\n        },\n        \"errorMessage\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/NonEmptyString\"\n            },\n            {\n              \"description\": \"The error message received when the account failed to enable Amazon Inspector.\"\n            }\n          ]\n        },\n        \"status\": {\n          \"\
  allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Status\"\n            },\n            {\n              \"description\": \"The status of Amazon Inspector for the account.\"\n            }\n          ]\n        }\n      },\n      \"description\": \"An object that described the state of Amazon Inspector scans for an account.\"\n    }\n  },\n  \"required\": [\n    \"ec2\",\n    \"ecr\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-resource-state-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: ResourceState
---
